# Comparing `tmp/pytest_broadcaster-0.8.0.tar.gz` & `tmp/pytest_broadcaster-0.9.0.tar.gz`

## Comparing `pytest_broadcaster-0.8.0.tar` & `pytest_broadcaster-0.9.0.tar`

### file list

```diff
@@ -1,171 +1,175 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/.python-version
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/mkdocs.yml
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/requirements-dev.lock
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/requirements.lock
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/SUMMARY.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/index.md
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/why.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/.overrides/main.html
--rwxr-xr-x   0        0        0     8775 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg
--rwxr-xr-x   0        0        0     8760 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/assets/pytest-discover-logo-transparent.svg
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/css/material.css
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/css/style.css
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/recipes/SUMMARY.md
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/recipes/code_generation.md
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/SUMMARY.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/index.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/plugin.md
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/SUMMARY.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/error_message.md
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/index.md
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/location.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/session_finish.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/session_start.md
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/traceback.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/warning_message.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/collect_report/index.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/collect_report/test_case.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/collect_report/test_directory.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/collect_report/test_module.md
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/collect_report/test_suite.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/steps/index.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/steps/outcome.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/steps/test_case_call.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/steps/test_case_error.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/steps/test_case_finished.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/steps/test_case_setup.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/events/steps/test_case_teardown.md
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/hooks/SUMMARY.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/hooks/pytest_broadcaster_add_destination.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/hooks/pytest_broadcaster_set_reporter.md
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/interfaces/SUMMARY.md
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/interfaces/destination.md
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/interfaces/reporter.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/result/SUMMARY.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/result/session_result/index.md
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/reference/result/session_result/test_case_report.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/collect_report.json
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/error_message.json
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/location.json
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/outcome.json
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/session_event.json
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/session_finish.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/session_result.json
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/session_start.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_case.json
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_case_call.json
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_case_error.json
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_case_finished.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_case_report.json
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_case_setup.json
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_case_teardown.json
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_directory.json
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_module.json
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/test_suite.json
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/traceback.json
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/schemas/warning_message.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/usage/SUMMARY.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/usage/http_webhook.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/usage/http_webhook_stream.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/usage/json_file.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/docs/usage/json_lines.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/scripts/deploy-docs.sh
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/scripts/generate-documentation.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/_testing/http_server.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/_testing/setup.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/_testing/fake_lib/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/_testing/fake_lib/with_errors.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/_testing/fake_lib/with_warnings.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/__about__.pyi
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/__init__.py
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/__init__.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_fields.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_json_files.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_pyproject.py
--rw-r--r--   0        0        0    13417 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_reporter.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_utils.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_webhook.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/hooks/__init__.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/interfaces/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/collect_report.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/error_message.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/location.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/outcome.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/project.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/python_distribution.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/session_event.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/session_finish.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/session_result.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/session_start.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_call.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_error.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_finished.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_report.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_setup.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_teardown.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_directory.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_module.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_suite.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/traceback.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/warning_message.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/collect_report.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/error_message.json
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/location.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/outcome.json
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/project.json
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/python_distribution.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/session_event.json
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/session_finish.json
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/session_result.json
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/session_start.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_case.json
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_case_call.json
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_case_error.json
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_case_finished.json
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_case_report.json
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_case_setup.json
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_case_teardown.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_directory.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_module.json
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/test_suite.json
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/traceback.json
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/src/schemas/warning_message.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/call/__init__.py
--rw-r--r--   0        0        0    11948 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/call/test_basic.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/call/test_basic_failure.py
--rw-r--r--   0        0        0    10387 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/call/test_basic_skip.py
--rw-r--r--   0        0        0    17526 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/call/test_basic_xfail.py
--rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/call/test_skip_within_test.py
--rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/call/test_xfail_within_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/__init__.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_basic.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_basic_marker.py
--rw-r--r--   0        0        0    10587 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_basic_parametrization.py
--rw-r--r--   0        0        0    10831 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_basic_suite.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_errors.py
--rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_errors_third_party.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_multi_cases.py
--rw-r--r--   0        0        0    13245 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_multi_files.py
--rw-r--r--   0        0        0    26216 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_multi_suite.py
--rw-r--r--   0        0        0    13845 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_nested_directories.py
--rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_nested_markers.py
--rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_warnings.py
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/collect/test_warnings_third_party.py
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/tests/destination/test_http_webhook.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/LICENSE
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/README.md
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 pytest_broadcaster-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/.python-version
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/requirements-dev.lock
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/requirements.lock
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/SUMMARY.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/index.md
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/why.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/.overrides/main.html
+-rwxr-xr-x   0        0        0     8775 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg
+-rwxr-xr-x   0        0        0     8760 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/assets/pytest-discover-logo-transparent.svg
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/css/material.css
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/css/style.css
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/recipes/SUMMARY.md
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/recipes/code_generation.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/SUMMARY.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/index.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/plugin.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/SUMMARY.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/error_message.md
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/index.md
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/location.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/project.md
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/python.md
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/session_finish.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/session_start.md
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/traceback.md
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/warning_message.md
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/collect_report/index.md
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/collect_report/test_case.md
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/collect_report/test_directory.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/collect_report/test_module.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/collect_report/test_suite.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/steps/index.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/steps/outcome.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/steps/test_case_call.md
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/steps/test_case_error.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/steps/test_case_finished.md
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/steps/test_case_setup.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/events/steps/test_case_teardown.md
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/hooks/SUMMARY.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/hooks/pytest_broadcaster_add_destination.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/hooks/pytest_broadcaster_set_reporter.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/interfaces/SUMMARY.md
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/interfaces/destination.md
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/interfaces/reporter.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/result/SUMMARY.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/result/session_result/index.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/reference/result/session_result/test_case_report.md
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/collect_report.json
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/error_message.json
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/location.json
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/outcome.json
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/project.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/python_distribution.json
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/session_event.json
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/session_finish.json
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/session_result.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/session_start.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_case.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_case_call.json
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_case_error.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_case_finished.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_case_report.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_case_setup.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_case_teardown.json
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_directory.json
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_module.json
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/test_suite.json
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/traceback.json
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/schemas/warning_message.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/usage/SUMMARY.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/usage/http_webhook.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/usage/http_webhook_stream.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/usage/json_file.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/docs/usage/json_lines.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/scripts/deploy-docs.sh
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/scripts/generate-documentation.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/_testing/http_server.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/_testing/setup.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/_testing/fake_lib/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/_testing/fake_lib/with_errors.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/_testing/fake_lib/with_warnings.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/__about__.pyi
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/__init__.py
+-rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/__init__.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_fields.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_json_files.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_pyproject.py
+-rw-r--r--   0        0        0    13417 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_reporter.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_utils.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_webhook.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/hooks/__init__.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/interfaces/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/collect_report.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/error_message.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/location.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/outcome.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/project.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/python_distribution.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/session_event.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/session_finish.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/session_result.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/session_start.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_call.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_error.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_finished.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_report.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_setup.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_teardown.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_directory.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_module.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_suite.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/traceback.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/warning_message.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/collect_report.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/error_message.json
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/location.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/outcome.json
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/project.json
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/python_distribution.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/session_event.json
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/session_finish.json
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/session_result.json
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/session_start.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_case.json
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_case_call.json
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_case_error.json
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_case_finished.json
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_case_report.json
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_case_setup.json
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_case_teardown.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_directory.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_module.json
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/test_suite.json
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/traceback.json
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/src/schemas/warning_message.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/call/__init__.py
+-rw-r--r--   0        0        0    11948 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/call/test_basic.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/call/test_basic_failure.py
+-rw-r--r--   0        0        0    10387 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/call/test_basic_skip.py
+-rw-r--r--   0        0        0    17526 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/call/test_basic_xfail.py
+-rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/call/test_skip_within_test.py
+-rw-r--r--   0        0        0    11299 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/call/test_xfail_within_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/__init__.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_basic.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_basic_marker.py
+-rw-r--r--   0        0        0    10587 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_basic_parametrization.py
+-rw-r--r--   0        0        0    10831 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_basic_suite.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_errors.py
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_errors_third_party.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_multi_cases.py
+-rw-r--r--   0        0        0    13245 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_multi_files.py
+-rw-r--r--   0        0        0    26216 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_multi_suite.py
+-rw-r--r--   0        0        0    13845 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_nested_directories.py
+-rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_nested_markers.py
+-rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_warnings.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/collect/test_warnings_third_party.py
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/tests/destination/test_http_webhook.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/README.md
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 pytest_broadcaster-0.9.0/PKG-INFO
```

### Comparing `pytest_broadcaster-0.8.0/mkdocs.yml` & `pytest_broadcaster-0.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/requirements-dev.lock` & `pytest_broadcaster-0.9.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/.github/workflows/ci.yml` & `pytest_broadcaster-0.9.0/.github/workflows/pypi.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-name: Continuous Integration
+name: PyPi Release
 
 on:
   workflow_dispatch:
   push:
-    branches: [main]
-  pull_request:
+    tags:
+      - 'v[0-9]+.[0-9]+.[0-9]+-[a-zA-Z]*'
+      - 'v[0-9]+.[0-9]+.[0-9]'
 
 jobs:
-  validation:
-    name: Validate
+  build:
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+    permissions:
+      contents: write
+
     steps:
       - uses: actions/checkout@v4
+
       # Uses the same action as rye
       # See: https://github.com/astral-sh/rye/blob/main/.github/workflows/python-lint.yml
       - name: Install the latest version of rye
         uses: eifinger/setup-rye@v2
         with:
           enable-cache: true
-          cache-prefix: 'validation-${{ matrix.python-version }}'
+          cache-prefix: 'pypi'
 
-      - name: Override python version required by project
-        run: echo "${{ matrix.python-version }}" > .python-version
+      - name: Build the docs
+        run: rye run bootstrap
 
-      - name: Run validation
-        run: rye run ci
+      - name: Build and publish the packag on pypi
+        run: |
+          rye build --clean
+          rye publish --yes --token ${{ secrets.PYPI_TOKEN }}
```

### Comparing `pytest_broadcaster-0.8.0/.github/workflows/docs.yml` & `pytest_broadcaster-0.9.0/.github/workflows/docs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 name: GitHub Pages Documentation
 
 on:
+  workflow_dispatch:
   push:
     tags:
       - 'v[0-9]+.[0-9]+.[0-9]+-[a-zA-Z]*'
       - 'v[0-9]+.[0-9]+.[0-9]'
-  workflow_dispatch:
 
 jobs:
   build:
     runs-on: ubuntu-latest
     permissions:
       contents: write
 
     steps:
       - uses: actions/checkout@v4
-        with:
-          fetch-depth: 1
 
       # Uses the same action as rye
       # See: https://github.com/astral-sh/rye/blob/main/.github/workflows/python-lint.yml
       - name: Install the latest version of rye
         uses: eifinger/setup-rye@v2
         with:
           enable-cache: true
```

### Comparing `pytest_broadcaster-0.8.0/docs/why.md` & `pytest_broadcaster-0.9.0/docs/why.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg` & `pytest_broadcaster-0.9.0/docs/assets/pytest-discover-logo-darkmode-transparent.svg`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/assets/pytest-discover-logo-transparent.svg` & `pytest_broadcaster-0.9.0/docs/assets/pytest-discover-logo-transparent.svg`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/css/mkdocstrings.css` & `pytest_broadcaster-0.9.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/css/style.css` & `pytest_broadcaster-0.9.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/recipes/code_generation.md` & `pytest_broadcaster-0.9.0/docs/recipes/code_generation.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/reference/events/SUMMARY.md` & `pytest_broadcaster-0.9.0/docs/reference/events/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/collect_report.json` & `pytest_broadcaster-0.9.0/docs/schemas/collect_report.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9428571428571428%*

 * *Differences: {"'properties'": "{'session_id': OrderedDict([('type', 'string'), ('description', 'The unique if "*

 * *                 "of this test session used to aggregate events together.')]), 'timestamp': "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time'), ('description', 'The "*

 * *                 "date and time when the report was generated in ISO 8601 format.')])}",*

 * * "'required'": "{insert: [(1, 'session_id'), (3, 'timestamp')]}"}*

```diff
@@ -30,17 +30,28 @@
                 ]
             },
             "type": "array"
         },
         "node_id": {
             "description": "The node id of the node for which items were collected (the top level root directory has an empty node id).",
             "type": "string"
+        },
+        "session_id": {
+            "description": "The unique if of this test session used to aggregate events together.",
+            "type": "string"
+        },
+        "timestamp": {
+            "description": "The date and time when the report was generated in ISO 8601 format.",
+            "format": "date-time",
+            "type": "string"
         }
     },
     "required": [
         "event",
+        "session_id",
         "node_id",
+        "timestamp",
         "items"
     ],
     "title": "Collect Report",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/error_message.json` & `pytest_broadcaster-0.9.0/docs/schemas/error_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/session_event.json` & `pytest_broadcaster-0.9.0/docs/schemas/session_event.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/session_finish.json` & `pytest_broadcaster-0.9.0/src/schemas/session_finish.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'$id'": "'session_finish.json'",*

 * * "'properties'": "{'session_id': OrderedDict([('type', 'string'), ('description', 'The unique if "*

 * *                 "of this test session used to aggregate events together.')]), 'timestamp': "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time'), ('description', 'The "*

 * *                 "time when the session finished in ISO 8601 format.')])}",*

 * * "'required'": "{insert: [(1, 'session_id'), (2, 'timestamp')]}"}*

```diff
@@ -1,21 +1,32 @@
 {
-    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_finish.json",
+    "$id": "session_finish.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when the session is finished.",
     "properties": {
         "event": {
             "const": "session_finish",
             "description": "The event type. Always set to 'session_finish'."
         },
         "exit_status": {
             "description": "The status which pytest will return to the system. 0 means success, 1 means test failure, anything else is an error.",
             "type": "integer"
+        },
+        "session_id": {
+            "description": "The unique if of this test session used to aggregate events together.",
+            "type": "string"
+        },
+        "timestamp": {
+            "description": "The time when the session finished in ISO 8601 format.",
+            "format": "date-time",
+            "type": "string"
         }
     },
     "required": [
         "event",
+        "session_id",
+        "timestamp",
         "exit_status"
     ],
     "title": "Session Finish",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/session_result.json` & `pytest_broadcaster-0.9.0/docs/schemas/session_start.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6662608225108225%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_start.json'",*

 * * "'description'": "'Event emitted when the test session is started.'",*

 * * "'properties'": "{'pytest_version': {'description': 'The version of pytest that is running the "*

 * *                 "tests.'}, 'plugin_version': {'description': 'The version of pytest-broadcaster "*

 * *                 "plugin that is used to produce the report.'}, 'event': OrderedDict([('const', "*

 * *                 "'session_start'), ('descripti […]*

```diff
@@ -1,58 +1,46 @@
 {
-    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_result.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_start.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
-    "description": "Result of a pytest session, including collect reports and test reports.",
+    "description": "Event emitted when the test session is started.",
     "properties": {
-        "collect_reports": {
-            "description": "Collect reports generated during the session.",
-            "items": {
-                "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/collect_report.json"
-            },
-            "type": "array"
-        },
-        "errors": {
-            "description": "Errors generated during the session.",
-            "items": {
-                "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/error_message.json"
-            },
-            "type": "array"
-        },
-        "exit_status": {
-            "description": "The exit status of the pytest run. 0 indicates success, non-zero indicates failure.",
-            "type": "integer"
+        "event": {
+            "const": "session_start",
+            "description": "The event type. Always set to `session_start`."
         },
         "plugin_version": {
-            "description": "The version of the plugin that generated the report.",
+            "description": "The version of pytest-broadcaster plugin that is used to produce the report.",
             "type": "string"
         },
+        "project": {
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/project.json",
+            "description": "The project that is being tested."
+        },
         "pytest_version": {
-            "description": "The version of pytest that generated the report.",
+            "description": "The version of pytest that is running the tests.",
             "type": "string"
         },
-        "test_reports": {
-            "description": "Test reports generated during the session.",
-            "items": {
-                "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_report.json"
-            },
-            "type": "array"
-        },
-        "warnings": {
-            "description": "Warnings generated during the session.",
-            "items": {
-                "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/warning_message.json"
-            },
-            "type": "array"
+        "python": {
+            "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/python_distribution.json",
+            "description": "The Python distribution that is running the tests."
+        },
+        "session_id": {
+            "description": "The unique if of this test session used to aggregate events together.",
+            "type": "string"
+        },
+        "timestamp": {
+            "description": "The date and time when the test session was started in ISO 8601 format.",
+            "format": "date-time",
+            "type": "string"
         }
     },
     "required": [
+        "event",
+        "session_id",
+        "timestamp",
+        "python",
         "pytest_version",
-        "plugin_version",
-        "exit_status",
-        "warnings",
-        "errors",
-        "collect_reports",
-        "test_reports"
+        "plugin_version"
     ],
-    "title": "Session Result",
+    "title": "Session Start",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/session_start.json` & `pytest_broadcaster-0.9.0/src/schemas/session_start.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8520408163265306%*

 * *Differences: {"'$id'": "'session_start.json'",*

 * * "'properties'": "{'session_id': OrderedDict([('type', 'string'), ('description', 'The unique if "*

 * *                 "of this test session used to aggregate events together.')]), 'timestamp': "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time'), ('description', 'The "*

 * *                 "date and time when the test session was started in ISO 8601 format.')]), "*

 * *                 "'python': OrderedDict([('$ref', 'python_distribution.json/#'), ('descriptio […]*

```diff
@@ -1,26 +1,46 @@
 {
-    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_start.json",
+    "$id": "session_start.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when the test session is started.",
     "properties": {
         "event": {
             "const": "session_start",
             "description": "The event type. Always set to `session_start`."
         },
         "plugin_version": {
             "description": "The version of pytest-broadcaster plugin that is used to produce the report.",
             "type": "string"
         },
+        "project": {
+            "$ref": "project.json/#",
+            "description": "The project that is being tested."
+        },
         "pytest_version": {
             "description": "The version of pytest that is running the tests.",
             "type": "string"
+        },
+        "python": {
+            "$ref": "python_distribution.json/#",
+            "description": "The Python distribution that is running the tests."
+        },
+        "session_id": {
+            "description": "The unique if of this test session used to aggregate events together.",
+            "type": "string"
+        },
+        "timestamp": {
+            "description": "The date and time when the test session was started in ISO 8601 format.",
+            "format": "date-time",
+            "type": "string"
         }
     },
     "required": [
         "event",
+        "session_id",
+        "timestamp",
+        "python",
         "pytest_version",
         "plugin_version"
     ],
     "title": "Session Start",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_case.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_case.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_case_call.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_case_call.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8961038961038961%*

 * *Differences: {"'properties'": '{\'event\': OrderedDict([(\'const\', \'case_call\'), (\'description\', "The '*

 * *                 'event type. Always set to \'case_call\'.")]), \'session_id\': '*

 * *                 "OrderedDict([('type', 'string'), ('description', 'The unique if of this test "*

 * *                 "session used to aggregate events together.')]), 'start_timestamp': "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time'), ('description', 'Start "*

 * *                 "time of the call step in ISO 86 […]*

```diff
@@ -7,41 +7,46 @@
             "description": "Duration of the call step in seconds.",
             "type": "number"
         },
         "error": {
             "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json",
             "description": "Error details if the call step failed."
         },
-        "event_type": {
+        "event": {
             "const": "case_call",
             "description": "The event type. Always set to 'case_call'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
             "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
             "description": "Outcome of the call step."
         },
-        "start": {
+        "session_id": {
+            "description": "The unique if of this test session used to aggregate events together.",
+            "type": "string"
+        },
+        "start_timestamp": {
             "description": "Start time of the call step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
-        "stop": {
+        "stop_timestamp": {
             "description": "Stop time of the call step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         }
     },
     "required": [
+        "event",
         "node_id",
-        "event_type",
-        "outcome",
+        "session_id",
+        "start_timestamp",
+        "stop_timestamp",
         "duration",
-        "start",
-        "stop"
+        "outcome"
     ],
     "title": "Test Case Call",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_case_error.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_case_error.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_case_finished.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_case_finished.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.882034632034632%*

 * *Differences: {"'properties'": '{\'event\': OrderedDict([(\'const\', \'case_finished\'), (\'description\', "The '*

 * *                 'event type. Always set to \'case_finished\'.")]), \'session_id\': '*

 * *                 "OrderedDict([('type', 'string'), ('description', 'The unique if of this test "*

 * *                 "session used to aggregate events together.')]), 'start_timestamp': "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time'), ('description', 'Start "*

 * *                 "time of the test case ( […]*

```diff
@@ -1,44 +1,48 @@
 {
     "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_outcome.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when a test case is finished (meaning all of setup, call and teardown steps are finished).",
     "properties": {
-        "duration": {
-            "description": "Duration of the test case in seconds (including setup and teardown).",
-            "type": "number"
-        },
-        "event_type": {
+        "event": {
             "const": "case_finished",
             "description": "The event type. Always set to 'case_finished'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
             "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
             "description": "Outcome of the test case."
         },
-        "start": {
+        "session_id": {
+            "description": "The unique if of this test session used to aggregate events together.",
+            "type": "string"
+        },
+        "start_timestamp": {
             "description": "Start time of the test case (including setup).",
             "format": "date-time",
             "type": "string"
         },
-        "stop": {
+        "stop_timestamp": {
             "description": "Stop time of the test case (including teardown).",
             "format": "date-time",
             "type": "string"
+        },
+        "total_duration": {
+            "description": "Total duration of the test case in seconds (including setup and teardown).",
+            "type": "number"
         }
     },
     "required": [
+        "event",
+        "session_id",
         "node_id",
-        "event_type",
-        "outcome",
-        "finished",
-        "duration",
-        "start",
-        "stop"
+        "start_timestamp",
+        "stop_timestamp",
+        "total_duration",
+        "outcome"
     ],
     "title": "Test Case Finished",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_case_report.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_case_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_case_setup.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_case_setup.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8961038961038961%*

 * *Differences: {"'properties'": '{\'event\': OrderedDict([(\'const\', \'case_setup\'), (\'description\', "The '*

 * *                 'event type. Always set to \'case_setup\'.")]), \'session_id\': '*

 * *                 "OrderedDict([('type', 'string'), ('description', 'The unique if of this test "*

 * *                 "session used to aggregate events together.')]), 'start_timestamp': "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time'), ('description', 'Start "*

 * *                 "time of the setup step in ISO […]*

```diff
@@ -7,41 +7,46 @@
             "description": "Duration of the setup step in seconds.",
             "type": "number"
         },
         "error": {
             "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json",
             "description": "Error details if the setup step failed."
         },
-        "event_type": {
+        "event": {
             "const": "case_setup",
             "description": "The event type. Always set to 'case_setup'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
             "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
             "description": "Outcome of the setup step."
         },
-        "start": {
+        "session_id": {
+            "description": "The unique if of this test session used to aggregate events together.",
+            "type": "string"
+        },
+        "start_timestamp": {
             "description": "Start time of the setup step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
-        "stop": {
+        "stop_timestamp": {
             "description": "Stop time of the setup step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         }
     },
     "required": [
+        "event",
         "node_id",
-        "event_type",
-        "outcome",
+        "session_id",
+        "start_timestamp",
+        "stop_timestamp",
         "duration",
-        "start",
-        "stop"
+        "outcome"
     ],
     "title": "Test Case Setup",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_case_teardown.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_case_teardown.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8961038961038961%*

 * *Differences: {"'properties'": '{\'event\': OrderedDict([(\'const\', \'case_teardown\'), (\'description\', "The '*

 * *                 'event type. Always set to \'case_teardown\'.")]), \'session_id\': '*

 * *                 "OrderedDict([('type', 'string'), ('description', 'The unique if of this test "*

 * *                 "session used to aggregate events together.')]), 'start_timestamp': "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time'), ('description', 'Start "*

 * *                 "time of the teardown st […]*

```diff
@@ -7,41 +7,46 @@
             "description": "Duration of the teardown step in seconds.",
             "type": "number"
         },
         "error": {
             "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/test_case_error.json",
             "description": "Error details if the teardown step failed."
         },
-        "event_type": {
+        "event": {
             "const": "case_teardown",
             "description": "The event type. Always set to 'case_teardown'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
             "$ref": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/outcome.json",
             "description": "Outcome of the teardown step."
         },
-        "start": {
+        "session_id": {
+            "description": "The unique if of this test session used to aggregate events together.",
+            "type": "string"
+        },
+        "start_timestamp": {
             "description": "Start time of the teardown step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
-        "stop": {
+        "stop_timestamp": {
             "description": "Stop time of the teardown step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         }
     },
     "required": [
+        "event",
+        "session_id",
         "node_id",
-        "event_type",
-        "outcome",
+        "start_timestamp",
+        "stop_timestamp",
         "duration",
-        "start",
-        "stop"
+        "outcome"
     ],
     "title": "Test Case Teardown",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_directory.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_directory.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_module.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_module.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/test_suite.json` & `pytest_broadcaster-0.9.0/docs/schemas/test_suite.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/traceback.json` & `pytest_broadcaster-0.9.0/docs/schemas/traceback.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/schemas/warning_message.json` & `pytest_broadcaster-0.9.0/docs/schemas/warning_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/usage/http_webhook.md` & `pytest_broadcaster-0.9.0/docs/usage/http_webhook.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/docs/usage/http_webhook_stream.md` & `pytest_broadcaster-0.9.0/docs/usage/http_webhook_stream.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/scripts/generate-documentation.py` & `pytest_broadcaster-0.9.0/scripts/generate-documentation.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/_testing/http_server.py` & `pytest_broadcaster-0.9.0/src/_testing/http_server.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/_testing/setup.py` & `pytest_broadcaster-0.9.0/src/_testing/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/plugin.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_fields.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 def field_parameters(item: pytest.Item) -> dict[str, str]:
     return {k: type(v).__name__ for k, v in sorted(get_test_args(item).items())}
 
 
 def field_python() -> PythonDistribution:
     packages = [
-        Package(name=x.metadata.get("Name"), version=x.version)
+        Package(name=x.metadata.get("Name"), version=x.version)  # pyright: ignore[reportAttributeAccessIssue]
         for x in importlib.metadata.distributions()
     ]
     platform_os = platform.system()
     if platform_os == "Linux":
         platform_os = Platform.linux
     elif platform_os == "Darwin":
         platform_os = Platform.darwin
```

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_json_files.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_json_files.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_pyproject.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_pyproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import sys
 from importlib.metadata import version
 from pathlib import Path
 from typing import Any
 
-if sys.version_info < (3, 11):
-    import tomli as toml
+if sys.version_info >= (3, 11):
+    import tomllib as toml
 else:
-    import toml
+    import tomli as toml
 
 
 def get_pyproject() -> Path | None:
     parent_path = Path.cwd()
     while True:
         try_path = parent_path / "pyproject.toml"
         if try_path.exists():
```

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_reporter.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_utils.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/_internal/_webhook.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/_internal/_webhook.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/hooks/__init__.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/interfaces/__init__.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/collect_report.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/collect_report.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/error_message.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/error_message.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/project.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/project.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/python_distribution.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/python_distribution.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/session_event.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/session_event.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/session_finish.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/session_finish.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/session_result.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/session_result.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/session_start.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/session_start.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_call.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_call.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_finished.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_finished.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_report.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_report.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_setup.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_setup.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_case_teardown.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_case_teardown.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_module.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_module.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/test_suite.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/test_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/traceback.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/traceback.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/pytest_broadcaster/models/warning_message.py` & `pytest_broadcaster-0.9.0/src/pytest_broadcaster/models/warning_message.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/collect_report.json` & `pytest_broadcaster-0.9.0/src/schemas/collect_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/error_message.json` & `pytest_broadcaster-0.9.0/src/schemas/error_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/project.json` & `pytest_broadcaster-0.9.0/src/schemas/project.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/python_distribution.json` & `pytest_broadcaster-0.9.0/src/schemas/python_distribution.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/session_event.json` & `pytest_broadcaster-0.9.0/src/schemas/session_event.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/session_finish.json` & `pytest_broadcaster-0.9.0/docs/schemas/session_finish.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_finish.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "session_finish.json",
+    "$id": "https://charbonnierg.github.io/pytest-broadcaster/latest/schemas/session_finish.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
     "description": "Event emitted when the session is finished.",
     "properties": {
         "event": {
             "const": "session_finish",
             "description": "The event type. Always set to 'session_finish'."
         },
```

### Comparing `pytest_broadcaster-0.8.0/src/schemas/session_result.json` & `pytest_broadcaster-0.9.0/src/schemas/session_result.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/session_start.json` & `pytest_broadcaster-0.9.0/src/schemas/test_case_setup.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6654595404595405%*

 * *Differences: {"'$id'": "'test_case_setup.json'",*

 * * "'description'": "'Pytest Test Case Setup'",*

 * * "'properties'": '{\'event\': {\'const\': \'case_setup\', \'description\': "The event type. Always '*

 * *                 'set to \'case_setup\'."}, \'node_id\': OrderedDict([(\'type\', \'string\'), '*

 * *                 "('description', 'The node ID of the test case.')]), 'start_timestamp': "*

 * *                 "OrderedDict([('type', 'string'), ('format', 'date-time'), ('description', 'Start "*

 * *                 "time of the setup step  […]*

```diff
@@ -1,46 +1,52 @@
 {
-    "$id": "session_start.json",
+    "$id": "test_case_setup.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
-    "description": "Event emitted when the test session is started.",
+    "description": "Pytest Test Case Setup",
     "properties": {
-        "event": {
-            "const": "session_start",
-            "description": "The event type. Always set to `session_start`."
-        },
-        "plugin_version": {
-            "description": "The version of pytest-broadcaster plugin that is used to produce the report.",
-            "type": "string"
+        "duration": {
+            "description": "Duration of the setup step in seconds.",
+            "type": "number"
+        },
+        "error": {
+            "$ref": "test_case_error.json/#",
+            "description": "Error details if the setup step failed."
         },
-        "project": {
-            "$ref": "project.json/#",
-            "description": "The project that is being tested."
+        "event": {
+            "const": "case_setup",
+            "description": "The event type. Always set to 'case_setup'."
         },
-        "pytest_version": {
-            "description": "The version of pytest that is running the tests.",
+        "node_id": {
+            "description": "The node ID of the test case.",
             "type": "string"
         },
-        "python": {
-            "$ref": "python_distribution.json/#",
-            "description": "The Python distribution that is running the tests."
+        "outcome": {
+            "$ref": "outcome.json/#",
+            "description": "Outcome of the setup step."
         },
         "session_id": {
             "description": "The unique if of this test session used to aggregate events together.",
             "type": "string"
         },
-        "timestamp": {
-            "description": "The date and time when the test session was started in ISO 8601 format.",
+        "start_timestamp": {
+            "description": "Start time of the setup step in ISO 8601 format.",
+            "format": "date-time",
+            "type": "string"
+        },
+        "stop_timestamp": {
+            "description": "Stop time of the setup step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         }
     },
     "required": [
         "event",
+        "node_id",
         "session_id",
-        "timestamp",
-        "python",
-        "pytest_version",
-        "plugin_version"
+        "start_timestamp",
+        "stop_timestamp",
+        "duration",
+        "outcome"
     ],
-    "title": "Session Start",
+    "title": "Test Case Setup",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_case.json` & `pytest_broadcaster-0.9.0/src/schemas/test_case.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_case_call.json` & `pytest_broadcaster-0.9.0/src/schemas/test_case_call.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_case_finished.json` & `pytest_broadcaster-0.9.0/src/schemas/test_case_finished.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_case_report.json` & `pytest_broadcaster-0.9.0/src/schemas/test_case_report.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_case_setup.json` & `pytest_broadcaster-0.9.0/src/schemas/test_case_teardown.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7607886904761905%*

 * *Differences: {"'$id'": "'test_case_teardown.json'",*

 * * "'description'": "'Pytest Test Case Teardown'",*

 * * "'properties'": '{\'event\': {\'const\': \'case_teardown\', \'description\': "The event type. '*

 * *                 'Always set to \'case_teardown\'."}, \'start_timestamp\': {\'description\': '*

 * *                 "'Start time of the teardown step in ISO 8601 format.'}, 'stop_timestamp': "*

 * *                 "{'description': 'Stop time of the teardown step in ISO 8601 format.'}, "*

 * *                 "'duration': {'description': ' […]*

```diff
@@ -1,52 +1,52 @@
 {
-    "$id": "test_case_setup.json",
+    "$id": "test_case_teardown.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
-    "description": "Pytest Test Case Setup",
+    "description": "Pytest Test Case Teardown",
     "properties": {
         "duration": {
-            "description": "Duration of the setup step in seconds.",
+            "description": "Duration of the teardown step in seconds.",
             "type": "number"
         },
         "error": {
             "$ref": "test_case_error.json/#",
-            "description": "Error details if the setup step failed."
+            "description": "Error details if the teardown step failed."
         },
         "event": {
-            "const": "case_setup",
-            "description": "The event type. Always set to 'case_setup'."
+            "const": "case_teardown",
+            "description": "The event type. Always set to 'case_teardown'."
         },
         "node_id": {
             "description": "The node ID of the test case.",
             "type": "string"
         },
         "outcome": {
             "$ref": "outcome.json/#",
-            "description": "Outcome of the setup step."
+            "description": "Outcome of the teardown step."
         },
         "session_id": {
             "description": "The unique if of this test session used to aggregate events together.",
             "type": "string"
         },
         "start_timestamp": {
-            "description": "Start time of the setup step in ISO 8601 format.",
+            "description": "Start time of the teardown step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         },
         "stop_timestamp": {
-            "description": "Stop time of the setup step in ISO 8601 format.",
+            "description": "Stop time of the teardown step in ISO 8601 format.",
             "format": "date-time",
             "type": "string"
         }
     },
     "required": [
         "event",
-        "node_id",
         "session_id",
+        "node_id",
         "start_timestamp",
         "stop_timestamp",
         "duration",
         "outcome"
     ],
-    "title": "Test Case Setup",
+    "title": "Test Case Teardown",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_case_teardown.json` & `pytest_broadcaster-0.9.0/src/schemas/traceback.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6428571428571429%*

 * *Differences: {"'$id'": "'traceback.json'",*

 * * "'description'": "'An error traceback.'",*

 * * "'properties'": "{replace: OrderedDict([('entries', OrderedDict([('type', 'array'), "*

 * *                 "('description', 'Traceback frame entries.'), ('items', OrderedDict([('type', "*

 * *                 "'object'), ('required', ['path', 'lineno', 'message']), ('properties', "*

 * *                 "OrderedDict([('path', OrderedDict([('type', 'string'), ('description', 'The file "*

 * *                 "path of this frame entry.')])), ('lineno', Or […]*

```diff
@@ -1,52 +1,38 @@
 {
-    "$id": "test_case_teardown.json",
+    "$id": "traceback.json",
     "$schema": "https://json-schema.org/draft/2019-09/schema",
-    "description": "Pytest Test Case Teardown",
+    "description": "An error traceback.",
     "properties": {
-        "duration": {
-            "description": "Duration of the teardown step in seconds.",
-            "type": "number"
-        },
-        "error": {
-            "$ref": "test_case_error.json/#",
-            "description": "Error details if the teardown step failed."
-        },
-        "event": {
-            "const": "case_teardown",
-            "description": "The event type. Always set to 'case_teardown'."
-        },
-        "node_id": {
-            "description": "The node ID of the test case.",
-            "type": "string"
-        },
-        "outcome": {
-            "$ref": "outcome.json/#",
-            "description": "Outcome of the teardown step."
-        },
-        "session_id": {
-            "description": "The unique if of this test session used to aggregate events together.",
-            "type": "string"
-        },
-        "start_timestamp": {
-            "description": "Start time of the teardown step in ISO 8601 format.",
-            "format": "date-time",
-            "type": "string"
-        },
-        "stop_timestamp": {
-            "description": "Stop time of the teardown step in ISO 8601 format.",
-            "format": "date-time",
-            "type": "string"
+        "entries": {
+            "description": "Traceback frame entries.",
+            "items": {
+                "properties": {
+                    "lineno": {
+                        "description": "The line number of this frame entry.",
+                        "type": "integer"
+                    },
+                    "message": {
+                        "description": "The message of this frame entry.",
+                        "type": "string"
+                    },
+                    "path": {
+                        "description": "The file path of this frame entry.",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "path",
+                    "lineno",
+                    "message"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         }
     },
     "required": [
-        "event",
-        "session_id",
-        "node_id",
-        "start_timestamp",
-        "stop_timestamp",
-        "duration",
-        "outcome"
+        "entries"
     ],
-    "title": "Test Case Teardown",
+    "title": "Traceback",
     "type": "object"
 }
```

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_directory.json` & `pytest_broadcaster-0.9.0/src/schemas/test_directory.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_module.json` & `pytest_broadcaster-0.9.0/src/schemas/test_module.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/test_suite.json` & `pytest_broadcaster-0.9.0/src/schemas/test_suite.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/src/schemas/warning_message.json` & `pytest_broadcaster-0.9.0/src/schemas/warning_message.json`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/call/test_basic.py` & `pytest_broadcaster-0.9.0/tests/call/test_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/call/test_basic_failure.py` & `pytest_broadcaster-0.9.0/tests/call/test_basic_failure.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/call/test_basic_skip.py` & `pytest_broadcaster-0.9.0/tests/call/test_basic_skip.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/call/test_basic_xfail.py` & `pytest_broadcaster-0.9.0/tests/call/test_basic_xfail.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/call/test_skip_within_test.py` & `pytest_broadcaster-0.9.0/tests/call/test_skip_within_test.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/call/test_xfail_within_test.py` & `pytest_broadcaster-0.9.0/tests/call/test_xfail_within_test.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_basic.py` & `pytest_broadcaster-0.9.0/tests/collect/test_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_basic_marker.py` & `pytest_broadcaster-0.9.0/tests/collect/test_basic_marker.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_basic_parametrization.py` & `pytest_broadcaster-0.9.0/tests/collect/test_basic_parametrization.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_basic_suite.py` & `pytest_broadcaster-0.9.0/tests/collect/test_basic_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_errors.py` & `pytest_broadcaster-0.9.0/tests/collect/test_errors.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_errors_third_party.py` & `pytest_broadcaster-0.9.0/tests/collect/test_errors_third_party.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_multi_cases.py` & `pytest_broadcaster-0.9.0/tests/collect/test_multi_cases.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_multi_files.py` & `pytest_broadcaster-0.9.0/tests/collect/test_multi_files.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_multi_suite.py` & `pytest_broadcaster-0.9.0/tests/collect/test_multi_suite.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_nested_directories.py` & `pytest_broadcaster-0.9.0/tests/collect/test_nested_directories.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_nested_markers.py` & `pytest_broadcaster-0.9.0/tests/collect/test_nested_markers.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_warnings.py` & `pytest_broadcaster-0.9.0/tests/collect/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/collect/test_warnings_third_party.py` & `pytest_broadcaster-0.9.0/tests/collect/test_warnings_third_party.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/tests/destination/test_http_webhook.py` & `pytest_broadcaster-0.9.0/tests/destination/test_http_webhook.py`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/LICENSE` & `pytest_broadcaster-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/README.md` & `pytest_broadcaster-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_broadcaster-0.8.0/pyproject.toml` & `pytest_broadcaster-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -68,45 +68,48 @@
 # Serve documentation
 docs = "mkdocs serve"
 # Run test with coverage
 test = { chain = ["__test", "__coverage-html"] }
 # View coverage report
 htmlcov = "python -m http.server 8080 --directory coverage-report"
 # Automate pre-commit
-pre = { chain = ["generate", "__format", "__lint", "test", "__typecheck"] }
+pre = { chain = ["generate", "format", "lint", "test", "typecheck"] }
 # Automate CI
 ci-docs = { chain = ["bootstrap", "diff", "__deploy-docs"] }
 ci = { chain = [
     "bootstrap",
     "diff",
     "__formatcheck",
-    "__lint",
+    "lint",
     "test",
-    "__typecheck",
+    "typecheck",
 ] }
 # Automate project install
 bootstrap = { chain = ["__install-project"] }
+# Run pyright static type checker
+typecheck = { cmd = "pyright", env = { PYRIGHT_PYTHON_FORCE_VERSION = "latest" } }
 # Run code generation
 generate = { chain = ["__generate-models", "__format-models"] }
 # Verify generated code is up-to-date
 diff = { chain = [
     "__remove-previous-check",
     "__generate-models-check",
     "__format-models-check",
     "__generate-models-diff",
 ] }
 # Generate version file
 version = "hatch --quiet build --hooks-only"
+# Run linter
+lint = "rye lint"
+# Run formatter
+format = "rye fmt"
 # Private tasks used for chaining
 __deploy-docs = { cmd = "bash ./scripts/deploy-docs.sh" }
 __test = "coverage run --rcfile=pyproject.toml -m pytest"
 __coverage-html = "coverage html"
-__typecheck = { cmd = "pyright", env = { PYRIGHT_PYTHON_FORCE_VERSION = "latest" } }
-__lint = "rye lint"
-__format = "rye fmt"
 __formatcheck = "rye fmt --check"
 __generate-models = "datamodel-codegen --input src/schemas/ --output src/pytest_broadcaster/models --input-file-type jsonschema --disable-timestamp --output-model-type=dataclasses.dataclass --use-field-description --use-schema-description"
 __generate-models-check = "datamodel-codegen --input src/schemas/ --output check --input-file-type jsonschema --disable-timestamp --output-model-type=dataclasses.dataclass --use-field-description --use-schema-description"
 __generate-models-diff = "diff --exclude __pycache__ -r src/pytest_broadcaster/models check"
 __format-models = "rye fmt src/pytest_broadcaster/models"
 __format-models-check = "rye fmt check"
 __remove-previous-check = "rm -rf check"
@@ -146,13 +149,12 @@
 ]
 [tool.coverage.html]
 directory = "coverage-report"
 
 [tool.pyright]
 pythonVersion = "3.8"
 include = ["tests", "src", "scripts"]
-strict = ["src"]
 exclude = ["**/.venv", "**/node_modules", "**/__pycache__", ".git", "**/build"]
 venv = ".venv"
 venvPath = "."
 typeCheckingMode = "basic"
 reportUnnecessaryTypeIgnoreComment = "warning"
```

### Comparing `pytest_broadcaster-0.8.0/PKG-INFO` & `pytest_broadcaster-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-broadcaster
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pytest plugin to broadcast pytest output to various destinations
 Project-URL: Source, https://github.com/charbonnierg/pytest-broadcaster
 Project-URL: Tracker, https://github.com/charbonnierg/pytest-broadcaster/issues
 Author-email: Guillaume Charbonnier <gu.charbon@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pytest
```

