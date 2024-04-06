# Comparing `tmp/pytest_broadcaster-0.6.0.tar.gz` & `tmp/pytest_broadcaster-0.7.0.tar.gz`

## Comparing `pytest_broadcaster-0.6.0.tar` & `pytest_broadcaster-0.7.0.tar`

### file list

```diff
@@ -1,164 +1,165 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/.python-version
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/requirements-dev.lock
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/requirements.lock
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/SUMMARY.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/index.md
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/why.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/.overrides/main.html
--rwxr-xr-x   0        0        0     8775 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg
--rwxr-xr-x   0        0        0     8760 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/assets/pytest-discover-logo-transparent.svg
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/css/material.css
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/css/style.css
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/recipes/SUMMARY.md
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/recipes/code_generation.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/SUMMARY.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/index.md
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/SUMMARY.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/error_message.md
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/index.md
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/location.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/session_finish.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/session_start.md
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/traceback.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/warning_message.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/index.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/test_case.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/test_directory.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/test_module.md
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/collect_report/test_suite.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/index.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/outcome.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_call.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_error.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_finished.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_setup.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/events/steps/test_case_teardown.md
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/hooks/SUMMARY.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/hooks/pytest_broadcaster_add_destination.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/hooks/pytest_broadcaster_set_reporter.md
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/interfaces/SUMMARY.md
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/interfaces/destination.md
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/interfaces/reporter.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/result/SUMMARY.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/result/session_result/index.md
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/reference/result/session_result/test_case_report.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/collect_report.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/error_message.json
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/location.json
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/outcome.json
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/session_event.json
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/session_finish.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/session_result.json
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/session_start.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case.json
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_call.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_error.json
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_finished.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_report.json
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_setup.json
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_case_teardown.json
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_directory.json
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_module.json
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/test_suite.json
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/traceback.json
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/schemas/warning_message.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/SUMMARY.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/http_webhook.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/http_webhook_stream.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/json_file.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/docs/usage/json_lines.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/scripts/deploy-docs.sh
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/scripts/generate-documentation.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/fake_lib/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/fake_lib/with_errors.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/fake_lib/with_warnings.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/__about__.pyi
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/__init__.py
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/__init__.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_fields.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_json_files.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_reporter.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_utils.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_webhook.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/hooks/__init__.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/interfaces/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/__init__.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/collect_report.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/error_message.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/location.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/outcome.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_event.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_finish.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_result.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_start.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_call.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_error.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_finished.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_report.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_setup.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_teardown.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_directory.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_module.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_suite.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/traceback.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/warning_message.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/collect_report.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/error_message.json
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/location.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/outcome.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/session_event.json
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/session_finish.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/session_result.json
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/session_start.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case.json
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_call.json
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_error.json
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_finished.json
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_report.json
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_setup.json
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_case_teardown.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_directory.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_module.json
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/test_suite.json
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/traceback.json
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/src/schemas/warning_message.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/_utils.py
--rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_basic.py
--rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_basic_failure.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_basic_skip.py
--rw-r--r--   0        0        0    14594 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_basic_xfail.py
--rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_skip_within_test.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/call/test_xfail_within_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/_utils.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_basic.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_basic_marker.py
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_basic_parametrization.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_basic_suite.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_errors.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_errors_third_party.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_multi_cases.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_multi_files.py
--rw-r--r--   0        0        0    23526 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_multi_suite.py
--rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_nested_directories.py
--rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_nested_markers.py
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_warnings.py
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/collect/test_warnings_third_party.py
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/tests/destination/test_http_webhook.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/LICENSE
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/README.md
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 pytest_broadcaster-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/.python-version
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/requirements-dev.lock
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/requirements.lock
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/SUMMARY.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/index.md
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/why.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/.overrides/main.html
+-rwxr-xr-x   0        0        0     8775 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg
+-rwxr-xr-x   0        0        0     8760 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/assets/pytest-discover-logo-transparent.svg
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/css/material.css
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/css/style.css
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/recipes/SUMMARY.md
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/recipes/code_generation.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/SUMMARY.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/index.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/SUMMARY.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/error_message.md
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/index.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/location.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/session_finish.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/session_start.md
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/traceback.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/warning_message.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/collect_report/index.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/collect_report/test_case.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/collect_report/test_directory.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/collect_report/test_module.md
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/collect_report/test_suite.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/steps/index.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/steps/outcome.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/steps/test_case_call.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/steps/test_case_error.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/steps/test_case_finished.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/steps/test_case_setup.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/events/steps/test_case_teardown.md
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/hooks/SUMMARY.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/hooks/pytest_broadcaster_add_destination.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/hooks/pytest_broadcaster_set_reporter.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/interfaces/SUMMARY.md
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/interfaces/destination.md
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/interfaces/reporter.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/result/SUMMARY.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/result/session_result/index.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/reference/result/session_result/test_case_report.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/collect_report.json
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/error_message.json
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/location.json
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/outcome.json
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/session_event.json
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/session_finish.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/session_result.json
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/session_start.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_case.json
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_case_call.json
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_case_error.json
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_case_finished.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_case_report.json
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_case_setup.json
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_case_teardown.json
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_directory.json
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_module.json
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/test_suite.json
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/traceback.json
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/schemas/warning_message.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/usage/SUMMARY.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/usage/http_webhook.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/usage/http_webhook_stream.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/usage/json_file.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/docs/usage/json_lines.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/scripts/deploy-docs.sh
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/scripts/generate-documentation.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/fake_lib/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/fake_lib/with_errors.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/fake_lib/with_warnings.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/__about__.pyi
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/__init__.py
+-rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/__init__.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_fields.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_json_files.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_reporter.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_utils.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_webhook.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/hooks/__init__.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/interfaces/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/__init__.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/collect_report.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/error_message.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/location.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/outcome.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/session_event.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/session_finish.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/session_result.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/session_start.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_call.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_error.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_finished.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_report.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_setup.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_teardown.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_directory.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_module.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_suite.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/traceback.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/warning_message.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/collect_report.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/error_message.json
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/location.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/outcome.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/session_event.json
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/session_finish.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/session_result.json
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/session_start.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_case.json
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_case_call.json
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_case_error.json
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_case_finished.json
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_case_report.json
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_case_setup.json
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_case_teardown.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_directory.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_module.json
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/test_suite.json
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/traceback.json
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/src/schemas/warning_message.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/call/__init__.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/call/_utils.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/call/test_basic.py
+-rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/call/test_basic_failure.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/call/test_basic_skip.py
+-rw-r--r--   0        0        0    14594 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/call/test_basic_xfail.py
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/call/test_skip_within_test.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/call/test_xfail_within_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/_utils.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_basic.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_basic_marker.py
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_basic_parametrization.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_basic_suite.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_errors.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_errors_third_party.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_multi_cases.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_multi_files.py
+-rw-r--r--   0        0        0    23526 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_multi_suite.py
+-rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_nested_directories.py
+-rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_nested_markers.py
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_warnings.py
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/collect/test_warnings_third_party.py
+-rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/tests/destination/test_http_webhook.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/LICENSE
+-rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/README.md
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 pytest_broadcaster-0.7.0/PKG-INFO
```

### Comparing `pytest_broadcaster-0.6.0/mkdocs.yml` & `pytest_broadcaster-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/requirements-dev.lock` & `pytest_broadcaster-0.7.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/.github/workflows/cd.yml` & `pytest_broadcaster-0.7.0/.github/workflows/docs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -33,12 +33,7 @@
           git fetch origin gh-pages --depth=1
 
       - name: Build the docs
         run: rye run ci-docs
         env:
           VERSION: "${{  github.ref_name }}"
           ALIAS: latest
-
-      - name: Build and publish the packag on pypi
-        run: |
-          rye build --clean
-          rye publish --yes --token ${{ secrets.PYPI_TOKEN }}
```

### Comparing `pytest_broadcaster-0.6.0/.github/workflows/ci.yml` & `pytest_broadcaster-0.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/why.md` & `pytest_broadcaster-0.7.0/docs/why.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg` & `pytest_broadcaster-0.7.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/assets/pytest-discover-logo-transparent.svg` & `pytest_broadcaster-0.7.0/docs/assets/pytest-discover-logo-transparent.svg`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/css/mkdocstrings.css` & `pytest_broadcaster-0.7.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/css/style.css` & `pytest_broadcaster-0.7.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/recipes/code_generation.md` & `pytest_broadcaster-0.7.0/docs/recipes/code_generation.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/reference/events/SUMMARY.md` & `pytest_broadcaster-0.7.0/docs/reference/events/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/collect_report.json` & `pytest_broadcaster-0.7.0/docs/schemas/collect_report.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9283234126984128%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/collect_report.json'",*

 * * "'properties'": "{'items': {'items': {'oneOf': {0: {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_directory.json'}, "*

 * *                 "1: {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_module.json'}, "*

 * *                 "2: {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/l […]*

```diff
@@ -1,34 +1,34 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/collect_report.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/collect_report.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "A report of collected items.",
     "properties": {
         "event": {
             "const": "collect_report",
             "description": "The event type. Always set to 'collect_report'."
         },
         "items": {
             "description": "An array of collected items. Each collected item is a test directory, test module, test suite, or test case. Top level directory is always first element in the array, followed by test cases, then test suites, then test modules, then test directories for each level of nesting.",
             "items": {
                 "oneOf": [
                     {
-                        "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_directory.json",
+                        "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_directory.json",
                         "description": "A test directory."
                     },
                     {
-                        "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_module.json",
+                        "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_module.json",
                         "description": "A test module."
                     },
                     {
-                        "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_suite.json",
+                        "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_suite.json",
                         "description": "A test suite."
                     },
                     {
-                        "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case.json",
+                        "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case.json",
                         "description": "A test case."
                     }
                 ]
             },
             "type": "array"
         },
         "node_id": {
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/error_message.json` & `pytest_broadcaster-0.7.0/docs/schemas/error_message.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9255952380952381%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/error_message.json'",*

 * * "'properties'": "{'location': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/location.json'}, "*

 * *                 "'traceback': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/traceback.json'}}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/error_message.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/error_message.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "An error message.",
     "properties": {
         "event": {
             "const": "error_message",
             "description": "The event type. Always 'error_message'."
         },
@@ -12,19 +12,19 @@
             "type": "string"
         },
         "exception_value": {
             "description": "The exception value as a string.",
             "type": "string"
         },
         "location": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/location.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/location.json",
             "description": "The location of the error."
         },
         "traceback": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/traceback.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/traceback.json",
             "description": "The traceback of the error. A traceback contains entries for each frame of the call stack."
         },
         "when": {
             "description": "When the error message is emitted.",
             "enum": [
                 "config",
                 "collect",
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/session_finish.json` & `pytest_broadcaster-0.7.0/docs/schemas/session_finish.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_finish.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/session_finish.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_finish.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when the session is finished.",
     "properties": {
         "event": {
             "const": "session_finish",
             "description": "The event type. Always set to 'session_finish'."
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/session_result.json` & `pytest_broadcaster-0.7.0/docs/schemas/session_result.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9268707482993197%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_result.json'",*

 * * "'properties'": "{'errors': {'items': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/error_message.json'}}, "*

 * *                 "'warnings': {'items': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/warning_message.json'}}, "*

 * *                 "'collect_reports': {'items': {'$ref': "*

 * *                 "'https://charbo […]*

```diff
@@ -1,23 +1,23 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/session_result.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_result.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Result of a pytest session, including collect reports and test reports.",
     "properties": {
         "collect_reports": {
             "description": "Collect reports generated during the session.",
             "items": {
-                "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/collect_report.json"
+                "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/collect_report.json"
             },
             "type": "array"
         },
         "errors": {
             "description": "Errors generated during the session.",
             "items": {
-                "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/error_message.json"
+                "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/error_message.json"
             },
             "type": "array"
         },
         "exit_status": {
             "description": "The exit status of the pytest run. 0 indicates success, non-zero indicates failure.",
             "type": "integer"
         },
@@ -28,22 +28,22 @@
         "pytest_version": {
             "description": "The version of pytest that generated the report.",
             "type": "string"
         },
         "test_reports": {
             "description": "Test reports generated during the session.",
             "items": {
-                "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_report.json"
+                "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_report.json"
             },
             "type": "array"
         },
         "warnings": {
             "description": "Warnings generated during the session.",
             "items": {
-                "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/warning_message.json"
+                "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/warning_message.json"
             },
             "type": "array"
         }
     },
     "required": [
         "pytest_version",
         "plugin_version",
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/session_start.json` & `pytest_broadcaster-0.7.0/src/schemas/session_start.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'session_start.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/session_start.json",
+    "$id": "session_start.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when the test session is started.",
     "properties": {
         "event": {
             "const": "session_start",
             "description": "The event type. Always set to `session_start`."
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_case.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_case.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "A collected test case.",
     "properties": {
         "doc": {
             "description": "The test docstring (optional).",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_case_call.json` & `pytest_broadcaster-0.7.0/src/schemas/test_case_call.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9260204081632654%*

 * *Differences: {"'$id'": "'test_case_call.json'",*

 * * "'properties'": "{'outcome': {'$ref': 'outcome.json/#'}, 'error': {'$ref': "*

 * *                 "'test_case_error.json/#'}}"}*

```diff
@@ -1,30 +1,30 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_call.json",
+    "$id": "test_case_call.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when a call step has been executed in a test case.",
     "properties": {
         "duration": {
             "description": "Duration of the call step in seconds.",
             "type": "number"
         },
         "error": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_error.json",
+            "$ref": "test_case_error.json/#",
             "description": "Error details if the call step failed."
         },
         "event_type": {
             "const": "case_call",
             "description": "The event type. Always set to 'case_call'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/outcome.json",
+            "$ref": "outcome.json/#",
             "description": "Outcome of the call step."
         },
         "start": {
             "description": "Start time of the call step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_case_error.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_case_error.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9241071428571429%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json'",*

 * * "'properties'": "{'traceback': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/traceback.json'}}"}*

```diff
@@ -1,18 +1,18 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_error.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "An error which occured during the execution of a test case (either setup, call or teardown).",
     "properties": {
         "message": {
             "description": "Error message.",
             "type": "string"
         },
         "traceback": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/traceback.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/traceback.json",
             "description": "Error traceback."
         }
     },
     "required": [
         "message"
     ],
     "title": "Test Case Error",
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_case_finished.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_case_finished.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9270833333333333%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_outcome.json'",*

 * * "'properties'": "{'outcome': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json'}}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_outcome.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_outcome.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when a test case is finished (meaning all of setup, call and teardown steps are finished).",
     "properties": {
         "duration": {
             "description": "Duration of the test case in seconds (including setup and teardown).",
             "type": "number"
         },
@@ -12,15 +12,15 @@
             "description": "The event type. Always set to 'case_finished'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/outcome.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
             "description": "Outcome of the test case."
         },
         "start": {
             "description": "Start time of the test case (including setup).",
             "format": "date-time",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_case_report.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_case_report.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9221938775510203%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_report.json'",*

 * * "'properties'": "{'outcome': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json'}, "*

 * *                 "'setup': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_setup.json'}, "*

 * *                 "'call': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schema […]*

```diff
@@ -1,38 +1,38 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_report.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_report.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Report for a single test case.",
     "properties": {
         "call": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_call.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_call.json",
             "description": "Call step of the test case (optional)."
         },
         "duration": {
             "description": "Duration of the test case in seconds (including setup and teardown).",
             "type": "number"
         },
         "finished": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_finished.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_finished.json",
             "description": "View of the test case after it has finished."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/outcome.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
             "description": "Outcome of the test case."
         },
         "setup": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_setup.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_setup.json",
             "description": "Setup step of the test case."
         },
         "teardown": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_teardown.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_teardown.json",
             "description": "Teardown step of the test case."
         }
     },
     "required": [
         "node_id",
         "outcome",
         "duration",
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_case_setup.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_case_setup.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9260204081632654%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_setup.json'",*

 * * "'properties'": "{'outcome': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json'}, "*

 * *                 "'error': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json'}}"}*

```diff
@@ -1,30 +1,30 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_setup.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_setup.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Pytest Test Case Setup",
     "properties": {
         "duration": {
             "description": "Duration of the setup step in seconds.",
             "type": "number"
         },
         "error": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_error.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json",
             "description": "Error details if the setup step failed."
         },
         "event_type": {
             "const": "case_setup",
             "description": "The event type. Always set to 'case_setup'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/outcome.json",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
             "description": "Outcome of the setup step."
         },
         "start": {
             "description": "Start time of the setup step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_case_teardown.json` & `pytest_broadcaster-0.7.0/src/schemas/test_case_teardown.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9260204081632654%*

 * *Differences: {"'$id'": "'test_case_teardown.json'",*

 * * "'properties'": "{'outcome': {'$ref': 'outcome.json/#'}, 'error': {'$ref': "*

 * *                 "'test_case_error.json/#'}}"}*

```diff
@@ -1,30 +1,30 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_teardown.json",
+    "$id": "test_case_teardown.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Pytest Test Case Teardown",
     "properties": {
         "duration": {
             "description": "Duration of the teardown step in seconds.",
             "type": "number"
         },
         "error": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_case_error.json",
+            "$ref": "test_case_error.json/#",
             "description": "Error details if the teardown step failed."
         },
         "event_type": {
             "const": "case_teardown",
             "description": "The event type. Always set to 'case_teardown'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/outcome.json",
+            "$ref": "outcome.json/#",
             "description": "Outcome of the teardown step."
         },
         "start": {
             "description": "Start time of the teardown step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_directory.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_directory.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_directory.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_directory.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_directory.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "A collected test directory.",
     "properties": {
         "name": {
             "description": "The directory name.",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_module.json` & `pytest_broadcaster-0.7.0/src/schemas/test_module.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'test_module.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_module.json",
+    "$id": "test_module.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "A collected test module (test file).",
     "properties": {
         "doc": {
             "description": "The module docstring.",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/test_suite.json` & `pytest_broadcaster-0.7.0/src/schemas/test_suite.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'test_suite.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/test_suite.json",
+    "$id": "test_suite.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "A collected test suite (test class).",
     "properties": {
         "doc": {
             "description": "The suite docstring.",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/traceback.json` & `pytest_broadcaster-0.7.0/src/schemas/traceback.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'traceback.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/traceback.json",
+    "$id": "traceback.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "An error traceback.",
     "properties": {
         "entries": {
             "description": "Traceback frame entries.",
             "items": {
                 "properties": {
```

### Comparing `pytest_broadcaster-0.6.0/docs/schemas/warning_message.json` & `pytest_broadcaster-0.7.0/docs/schemas/warning_message.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9270833333333333%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/warning_message.json'",*

 * * "'properties'": "{'location': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/location.json#'}}"}*

```diff
@@ -1,22 +1,22 @@
 {
-    "$id": "https://charbonnierg.github.com/pytest-broadcaster/schemas/warning_message.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/warning_message.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "A warning message.",
     "properties": {
         "category": {
             "description": "The category of the warning message.",
             "type": "string"
         },
         "event": {
             "const": "warning_message",
             "description": "The event type. Always 'warning_message'."
         },
         "location": {
-            "$ref": "https://charbonnierg.github.com/pytest-broadcaster/schemas/location.json#",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/location.json#",
             "description": "The location of the warning message."
         },
         "message": {
             "description": "The string content of the warning message.",
             "type": "string"
         },
         "node_id": {
```

### Comparing `pytest_broadcaster-0.6.0/docs/usage/http_webhook.md` & `pytest_broadcaster-0.7.0/docs/usage/http_webhook.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/docs/usage/http_webhook_stream.md` & `pytest_broadcaster-0.7.0/docs/usage/http_webhook_stream.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/scripts/generate-documentation.py` & `pytest_broadcaster-0.7.0/scripts/generate-documentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Generate the code reference pages."""
 
 from __future__ import annotations
 
 import json
+import os
 import shutil
 from os import environ
 from pathlib import Path
 from typing import Any
 from urllib.parse import urljoin
 
 import mkdocs_gen_files.nav
 
-REPOSITORY = "https://charbonnierg.github.com/pytest-broadcaster"
+REPOSITORY = "https://charbonnierg.github.io/pytest-broadcaster"
 
 SOURCES = Path(__file__).parent.parent.joinpath("src/schemas")
 
 
 def replace_refs_and_ids(schema: dict[str, Any], ref_prefix: str) -> None:
     if "$ref" in schema:
         ref_template: str = schema["$ref"]
@@ -36,20 +37,25 @@
 def create_schema(source: Path, output_directory: Path, ref_prefix: str) -> None:
     destination = output_directory.joinpath(source.name)
     content = json.loads(source.read_text())
     replace_refs_and_ids(content, ref_prefix)
     destination.write_text(json.dumps(content, indent=2))
 
 
-def generate_schemas(ref_prefix: str, output_directory: str):
+def generate_schemas(version: str, repository: str, output_directory: str):
     # Validate reference and output
-    if not (ref_prefix and output_directory):
-        raise ValueError("repository and output_directory are required")
+    if not (version and repository and output_directory):
+        raise ValueError("version, repository and output_directory are required")
     if output_directory.startswith("/"):
         raise ValueError("output must be relative")
+    ref_prefix = repository
+    if not ref_prefix.endswith("/"):
+        ref_prefix += "/"
+    # Join with version
+    ref_prefix = urljoin(ref_prefix, version)
     # Clean output directory
     destination = Path(output_directory)
     shutil.rmtree(destination, ignore_errors=True)
     destination.mkdir(parents=False, exist_ok=True)
     # Normalize repository and output
     if not ref_prefix.endswith("/"):
         ref_prefix += "/"
@@ -124,10 +130,11 @@
         else:
             license_file.write("No license file found")
 
 
 # generate_references()
 generate_license_file()
 generate_schemas(
-    ref_prefix=environ.get("REPOSITORY", REPOSITORY),
+    version=os.environ.get("VERSION", "latest"),
+    repository=environ.get("REPOSITORY", REPOSITORY),
     output_directory="docs/schemas",
 )
```

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/plugin.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_fields.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_fields.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_json_files.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_json_files.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_reporter.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_utils.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/_internal/_webhook.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/_internal/_webhook.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/hooks/__init__.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/interfaces/__init__.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/collect_report.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/collect_report.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/error_message.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/error_message.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_event.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/session_event.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_result.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/session_result.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/session_start.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/session_start.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_call.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_call.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_finished.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_finished.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_report.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_report.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_setup.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_setup.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_case_teardown.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_case_teardown.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_module.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_module.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/test_suite.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/test_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/traceback.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/traceback.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/pytest_broadcaster/models/warning_message.py` & `pytest_broadcaster-0.7.0/src/pytest_broadcaster/models/warning_message.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/collect_report.json` & `pytest_broadcaster-0.7.0/src/schemas/collect_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/error_message.json` & `pytest_broadcaster-0.7.0/src/schemas/error_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/session_event.json` & `pytest_broadcaster-0.7.0/src/schemas/session_event.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/session_finish.json` & `pytest_broadcaster-0.7.0/src/schemas/session_finish.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/session_result.json` & `pytest_broadcaster-0.7.0/src/schemas/session_result.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/session_start.json` & `pytest_broadcaster-0.7.0/docs/schemas/session_start.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_start.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "session_start.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_start.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when the test session is started.",
     "properties": {
         "event": {
             "const": "session_start",
             "description": "The event type. Always set to `session_start`."
         },
```

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_case.json` & `pytest_broadcaster-0.7.0/src/schemas/test_case.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_case_call.json` & `pytest_broadcaster-0.7.0/src/schemas/test_case_setup.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7776360544217688%*

 * *Differences: {"'$id'": "'test_case_setup.json'",*

 * * "'description'": "'Pytest Test Case Setup'",*

 * * "'properties'": '{\'event_type\': {\'const\': \'case_setup\', \'description\': "The event type. '*

 * *                 'Always set to \'case_setup\'."}, \'outcome\': {\'description\': \'Outcome of the '*

 * *                 "setup step.'}, 'duration': {'description': 'Duration of the setup step in "*

 * *                 "seconds.'}, 'start': {'description': 'Start time of the setup step in ISO 8601 "*

 * *                 "format.'}, 'stop':  […]*

```diff
@@ -1,47 +1,47 @@
 {
-    "$id": "test_case_call.json",
+    "$id": "test_case_setup.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
-    "description": "Event emitted when a call step has been executed in a test case.",
+    "description": "Pytest Test Case Setup",
     "properties": {
         "duration": {
-            "description": "Duration of the call step in seconds.",
+            "description": "Duration of the setup step in seconds.",
             "type": "number"
         },
         "error": {
             "$ref": "test_case_error.json/#",
-            "description": "Error details if the call step failed."
+            "description": "Error details if the setup step failed."
         },
         "event_type": {
-            "const": "case_call",
-            "description": "The event type. Always set to 'case_call'."
+            "const": "case_setup",
+            "description": "The event type. Always set to 'case_setup'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
             "$ref": "outcome.json/#",
-            "description": "Outcome of the call step."
+            "description": "Outcome of the setup step."
         },
         "start": {
-            "description": "Start time of the call step in ISO 8601 format.",
+            "description": "Start time of the setup step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
         "stop": {
-            "description": "Stop time of the call step in ISO 8601 format.",
+            "description": "Stop time of the setup step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         }
     },
     "required": [
         "node_id",
         "event_type",
         "outcome",
         "duration",
         "start",
         "stop"
     ],
-    "title": "Test Case Call",
+    "title": "Test Case Setup",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_case_finished.json` & `pytest_broadcaster-0.7.0/src/schemas/test_case_finished.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_case_report.json` & `pytest_broadcaster-0.7.0/src/schemas/test_case_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_case_setup.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_case_call.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7750850340136054%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_call.json'",*

 * * "'description'": "'Event emitted when a call step has been executed in a test case.'",*

 * * "'properties'": '{\'event_type\': {\'const\': \'case_call\', \'description\': "The event type. '*

 * *                 'Always set to \'case_call\'."}, \'outcome\': {\'$ref\': '*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json', "*

 * *                 "'description': 'Outcome of the  […]*

```diff
@@ -1,47 +1,47 @@
 {
-    "$id": "test_case_setup.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_call.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
-    "description": "Pytest Test Case Setup",
+    "description": "Event emitted when a call step has been executed in a test case.",
     "properties": {
         "duration": {
-            "description": "Duration of the setup step in seconds.",
+            "description": "Duration of the call step in seconds.",
             "type": "number"
         },
         "error": {
-            "$ref": "test_case_error.json/#",
-            "description": "Error details if the setup step failed."
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json",
+            "description": "Error details if the call step failed."
         },
         "event_type": {
-            "const": "case_setup",
-            "description": "The event type. Always set to 'case_setup'."
+            "const": "case_call",
+            "description": "The event type. Always set to 'case_call'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
-            "$ref": "outcome.json/#",
-            "description": "Outcome of the setup step."
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
+            "description": "Outcome of the call step."
         },
         "start": {
-            "description": "Start time of the setup step in ISO 8601 format.",
+            "description": "Start time of the call step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
         "stop": {
-            "description": "Stop time of the setup step in ISO 8601 format.",
+            "description": "Stop time of the call step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         }
     },
     "required": [
         "node_id",
         "event_type",
         "outcome",
         "duration",
         "start",
         "stop"
     ],
-    "title": "Test Case Setup",
+    "title": "Test Case Call",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_case_teardown.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_case_teardown.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9260204081632654%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_teardown.json'",*

 * * "'properties'": "{'outcome': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json'}, "*

 * *                 "'error': {'$ref': "*

 * *                 "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json'}}"}*

```diff
@@ -1,30 +1,30 @@
 {
-    "$id": "test_case_teardown.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_teardown.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Pytest Test Case Teardown",
     "properties": {
         "duration": {
             "description": "Duration of the teardown step in seconds.",
             "type": "number"
         },
         "error": {
-            "$ref": "test_case_error.json/#",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json",
             "description": "Error details if the teardown step failed."
         },
         "event_type": {
             "const": "case_teardown",
             "description": "The event type. Always set to 'case_teardown'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
-            "$ref": "outcome.json/#",
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
             "description": "Outcome of the teardown step."
         },
         "start": {
             "description": "Start time of the teardown step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_directory.json` & `pytest_broadcaster-0.7.0/src/schemas/test_directory.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_module.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_module.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_module.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "test_module.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_module.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "A collected test module (test file).",
     "properties": {
         "doc": {
             "description": "The module docstring.",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/src/schemas/test_suite.json` & `pytest_broadcaster-0.7.0/docs/schemas/test_suite.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_suite.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "test_suite.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_suite.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "A collected test suite (test class).",
     "properties": {
         "doc": {
             "description": "The suite docstring.",
             "type": "string"
         },
```

### Comparing `pytest_broadcaster-0.6.0/src/schemas/traceback.json` & `pytest_broadcaster-0.7.0/docs/schemas/traceback.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/traceback.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "traceback.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/traceback.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "An error traceback.",
     "properties": {
         "entries": {
             "description": "Traceback frame entries.",
             "items": {
                 "properties": {
```

### Comparing `pytest_broadcaster-0.6.0/src/schemas/warning_message.json` & `pytest_broadcaster-0.7.0/src/schemas/warning_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/call/_utils.py` & `pytest_broadcaster-0.7.0/tests/call/_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/call/test_basic.py` & `pytest_broadcaster-0.7.0/tests/call/test_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/call/test_basic_failure.py` & `pytest_broadcaster-0.7.0/tests/call/test_basic_failure.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/call/test_basic_skip.py` & `pytest_broadcaster-0.7.0/tests/call/test_basic_skip.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/call/test_basic_xfail.py` & `pytest_broadcaster-0.7.0/tests/call/test_basic_xfail.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/call/test_skip_within_test.py` & `pytest_broadcaster-0.7.0/tests/call/test_skip_within_test.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/call/test_xfail_within_test.py` & `pytest_broadcaster-0.7.0/tests/call/test_xfail_within_test.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/_utils.py` & `pytest_broadcaster-0.7.0/tests/collect/_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_basic.py` & `pytest_broadcaster-0.7.0/tests/collect/test_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_basic_marker.py` & `pytest_broadcaster-0.7.0/tests/collect/test_basic_marker.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_basic_parametrization.py` & `pytest_broadcaster-0.7.0/tests/collect/test_basic_parametrization.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_basic_suite.py` & `pytest_broadcaster-0.7.0/tests/collect/test_basic_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_errors.py` & `pytest_broadcaster-0.7.0/tests/collect/test_errors.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_errors_third_party.py` & `pytest_broadcaster-0.7.0/tests/collect/test_errors_third_party.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_multi_cases.py` & `pytest_broadcaster-0.7.0/tests/collect/test_multi_cases.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_multi_files.py` & `pytest_broadcaster-0.7.0/tests/collect/test_multi_files.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_multi_suite.py` & `pytest_broadcaster-0.7.0/tests/collect/test_multi_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_nested_directories.py` & `pytest_broadcaster-0.7.0/tests/collect/test_nested_directories.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_nested_markers.py` & `pytest_broadcaster-0.7.0/tests/collect/test_nested_markers.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_warnings.py` & `pytest_broadcaster-0.7.0/tests/collect/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/collect/test_warnings_third_party.py` & `pytest_broadcaster-0.7.0/tests/collect/test_warnings_third_party.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/tests/destination/test_http_webhook.py` & `pytest_broadcaster-0.7.0/tests/destination/test_http_webhook.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/LICENSE` & `pytest_broadcaster-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/README.md` & `pytest_broadcaster-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/pyproject.toml` & `pytest_broadcaster-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.6.0/PKG-INFO` & `pytest_broadcaster-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-broadcaster
-Version: 0.6.0
+Version: 0.7.0
 Summary: Pytest plugin to broadcast pytest output to various destinations
 Project-URL: Source, https://github.com/charbonnierg/pytest-broadcaster
 Project-URL: Tracker, https://github.com/charbonnierg/pytest-broadcaster/issues
 Author-email: Guillaume Charbonnier <gu.charbon@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pytest
```

