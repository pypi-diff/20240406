# Comparing `tmp/fusio-sdk-5.0.2.tar.gz` & `tmp/fusio-sdk-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusio-sdk-5.0.2.tar", last modified: Sun Mar 31 22:10:47 2024, max compression
+gzip compressed data, was "fusio-sdk-5.0.3.tar", last modified: Sat Apr  6 19:28:29 2024, max compression
```

## Comparing `fusio-sdk-5.0.2.tar` & `fusio-sdk-5.0.3.tar`

### file list

```diff
@@ -1,273 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:10:47.929044 fusio-sdk-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-31 22:10:47.929044 fusio-sdk-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:10:47.929044 fusio-sdk-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:10:47.885043 fusio-sdk-5.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:10:47.929044 fusio-sdk-5.0.2/src/fusio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-31 22:10:47.000000 fusio-sdk-5.0.2/src/fusio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-03-31 22:10:47.000000 fusio-sdk-5.0.2/src/fusio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:10:47.000000 fusio-sdk-5.0.2/src/fusio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 22:10:47.000000 fusio-sdk-5.0.2/src/fusio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-31 22:10:47.000000 fusio-sdk-5.0.2/src/fusio_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:10:47.929044 fusio-sdk-5.0.2/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/authorization_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_account_change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_execute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_execute_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_execute_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_execute_response_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_execute_response_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_action_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_audit_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_audit_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_audit_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_category_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_category_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_category_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_category_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_config_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_config_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_config_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_introspection_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_introspection_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_introspection_entity_row.py
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_connection_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_cronjob.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_cronjob_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_cronjob_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_cronjob_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_cronjob_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_cronjob_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_dashboard_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_event_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_event_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_generator_index_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_generator_index_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_generator_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_generator_provider_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_generator_provider_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_generator_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_identity_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_identity_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_identity_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_identity_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_identity_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_log_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_log_error_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_marketplace_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_marketplace_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_marketplace_collection_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_marketplace_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_marketplace_local_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_marketplace_remote_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_marketplace_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_operation_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_operation_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_operation_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_operation_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_operation_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_operation_throws.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_operation_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_page_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_page_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_rate_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_rate_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_rate_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_rate_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_rate_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_role_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_role_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_schema_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_schema_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_schema_preview_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_schema_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_schema_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope_category_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_scope_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_sdk_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_sdk_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_sdk_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_sdk_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_statistic_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_statistic_chart_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_statistic_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    18570 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_statistic_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_tenant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_trash_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_trash_data_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_trash_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_trash_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_trash_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_user_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/backend_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_form_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_form_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_form_element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_form_element_select.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_form_element_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_form_element_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_form_element_text_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_message_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_authorize_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_authorize_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_authorize_response_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_grant_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_grant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_payment_checkout_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_payment_checkout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_payment_portal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_payment_portal_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_token_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_token_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_token_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_password_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_user_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/consumer_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/passthru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_about.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_about_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_about_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_meta_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_route.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_route_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_route_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_schema_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-31 22:10:44.000000 fusio-sdk-5.0.2/src/sdk/system_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:28:29.866751 fusio-sdk-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-06 19:28:29.866751 fusio-sdk-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-06 19:28:26.000000 fusio-sdk-5.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:28:29.866751 fusio-sdk-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:28:29.814751 fusio-sdk-5.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:28:29.866751 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:28:29.862751 fusio-sdk-5.0.3/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/authorization_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_account_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_response_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_audit_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_audit_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_audit_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_config_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_config_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_config_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_introspection_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_introspection_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_introspection_entity_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_index_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_index_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_provider_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log_error_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_collection_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_local_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_throws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_preview_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_category_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_sdk_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_sdk_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_sdk_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_sdk_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_statistic_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_statistic_chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_statistic_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18570 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_statistic_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_tenant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_data_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_text_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_message_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_authorize_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_authorize_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_authorize_response_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_grant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_grant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_checkout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_portal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_portal_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_password_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/passthru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_about_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_about_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_meta_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_o_auth_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_route_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_route_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_schema_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_tag.py
```

### Comparing `fusio-sdk-5.0.2/LICENSE` & `fusio-sdk-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/PKG-INFO` & `fusio-sdk-5.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusio-sdk
-Version: 5.0.2
+Version: 5.0.3
 Summary: SDK to talk to the Fusio REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-sdk-python
 Project-URL: Issues, https://github.com/apioo/fusio-sdk-sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusio-sdk-5.0.2/README.md` & `fusio-sdk-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/pyproject.toml` & `fusio-sdk-5.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fusio-sdk"
-version = "5.0.2"
+version = "5.0.3"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "SDK to talk to the Fusio REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `fusio-sdk-5.0.2/src/fusio_sdk.egg-info/PKG-INFO` & `fusio-sdk-5.0.3/src/fusio_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusio-sdk
-Version: 5.0.2
+Version: 5.0.3
 Summary: SDK to talk to the Fusio REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-sdk-python
 Project-URL: Issues, https://github.com/apioo/fusio-sdk-sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusio-sdk-5.0.2/src/fusio_sdk.egg-info/SOURCES.txt` & `fusio-sdk-5.0.3/src/fusio_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -253,14 +253,15 @@
 src/sdk/passthru.py
 src/sdk/system_about.py
 src/sdk/system_about_apps.py
 src/sdk/system_about_link.py
 src/sdk/system_connection_tag.py
 src/sdk/system_health_check.py
 src/sdk/system_meta_tag.py
+src/sdk/system_o_auth_configuration.py
 src/sdk/system_payment_tag.py
 src/sdk/system_route.py
 src/sdk/system_route_method.py
 src/sdk/system_route_path.py
 src/sdk/system_schema.py
 src/sdk/system_schema_form.py
 src/sdk/system_schema_type_schema.py
```

### Comparing `fusio-sdk-5.0.2/src/sdk/authorization_tag.py` & `fusio-sdk-5.0.3/src/sdk/authorization_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_account_change_password.py` & `fusio-sdk-5.0.3/src/sdk/backend_account_change_password.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
 class BackendAccountChangePassword:
-    old_password: str = field(metadata=config(field_name="oldPassword"))
-    new_password: str = field(metadata=config(field_name="newPassword"))
-    verify_password: str = field(metadata=config(field_name="verifyPassword"))
+    old_password: str = field(default=None, metadata=config(field_name="oldPassword"))
+    new_password: str = field(default=None, metadata=config(field_name="newPassword"))
+    verify_password: str = field(default=None, metadata=config(field_name="verifyPassword"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_account_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_account_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_action.py` & `fusio-sdk-5.0.3/src/sdk/backend_action.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from backend_action_config import BackendActionConfig
 from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendAction:
-    id: int = field(metadata=config(field_name="id"))
-    status: int = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    _class: str = field(metadata=config(field_name="class"))
-    async: bool = field(metadata=config(field_name="async"))
-    config: BackendActionConfig = field(metadata=config(field_name="config"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    _class: str = field(default=None, metadata=config(field_name="class"))
+    async: bool = field(default=None, metadata=config(field_name="async"))
+    config: BackendActionConfig = field(default=None, metadata=config(field_name="config"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_action_execute_request.py` & `fusio-sdk-5.0.3/src/sdk/backend_log.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """
-backend_action_execute_request automatically generated by SDKgen please do not edit this file manually
+backend_log automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_action_execute_request_body import BackendActionExecuteRequestBody
+from typing import List
+from backend_log_error import BackendLogError
 @dataclass_json
 @dataclass
-class BackendActionExecuteRequest:
-    method: str = field(metadata=config(field_name="method"))
-    uri_fragments: str = field(metadata=config(field_name="uriFragments"))
-    parameters: str = field(metadata=config(field_name="parameters"))
-    headers: str = field(metadata=config(field_name="headers"))
-    body: BackendActionExecuteRequestBody = field(metadata=config(field_name="body"))
+class BackendLog:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    ip: str = field(default=None, metadata=config(field_name="ip"))
+    user_agent: str = field(default=None, metadata=config(field_name="userAgent"))
+    method: str = field(default=None, metadata=config(field_name="method"))
+    path: str = field(default=None, metadata=config(field_name="path"))
+    header: str = field(default=None, metadata=config(field_name="header"))
+    body: str = field(default=None, metadata=config(field_name="body"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
+    errors: List[BackendLogError] = field(default=None, metadata=config(field_name="errors"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_action_execute_response.py` & `fusio-sdk-5.0.3/src/sdk/backend_action_execute_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from backend_action_execute_response_headers import BackendActionExecuteResponseHeaders
 from backend_action_execute_response_body import BackendActionExecuteResponseBody
 @dataclass_json
 @dataclass
 class BackendActionExecuteResponse:
-    status_code: int = field(metadata=config(field_name="statusCode"))
-    headers: BackendActionExecuteResponseHeaders = field(metadata=config(field_name="headers"))
-    body: BackendActionExecuteResponseBody = field(metadata=config(field_name="body"))
+    status_code: int = field(default=None, metadata=config(field_name="statusCode"))
+    headers: BackendActionExecuteResponseHeaders = field(default=None, metadata=config(field_name="headers"))
+    body: BackendActionExecuteResponseBody = field(default=None, metadata=config(field_name="body"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_action_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_action_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_app.py` & `fusio-sdk-5.0.3/src/sdk/backend_identity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 """
-backend_app automatically generated by SDKgen please do not edit this file manually
+backend_identity automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
-from common_metadata import CommonMetadata
-from backend_token import BackendToken
+from backend_identity_config import BackendIdentityConfig
 @dataclass_json
 @dataclass
-class BackendApp:
-    id: int = field(metadata=config(field_name="id"))
-    user_id: int = field(metadata=config(field_name="userId"))
-    status: int = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    url: str = field(metadata=config(field_name="url"))
-    parameters: str = field(metadata=config(field_name="parameters"))
-    app_key: str = field(metadata=config(field_name="appKey"))
-    app_secret: str = field(metadata=config(field_name="appSecret"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    tokens: List[BackendToken] = field(metadata=config(field_name="tokens"))
+class BackendIdentity:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    app_id: int = field(default=None, metadata=config(field_name="appId"))
+    role_id: int = field(default=None, metadata=config(field_name="roleId"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    icon: str = field(default=None, metadata=config(field_name="icon"))
+    _class: str = field(default=None, metadata=config(field_name="class"))
+    config: BackendIdentityConfig = field(default=None, metadata=config(field_name="config"))
+    allow_create: bool = field(default=None, metadata=config(field_name="allowCreate"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_app_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_app_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_audit.py` & `fusio-sdk-5.0.3/src/sdk/consumer_page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """
-backend_audit automatically generated by SDKgen please do not edit this file manually
+consumer_page automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_app import BackendApp
-from backend_user import BackendUser
-from backend_audit_object import BackendAuditObject
+from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendAudit:
-    id: int = field(metadata=config(field_name="id"))
-    app: BackendApp = field(metadata=config(field_name="app"))
-    user: BackendUser = field(metadata=config(field_name="user"))
-    event: str = field(metadata=config(field_name="event"))
-    ip: str = field(metadata=config(field_name="ip"))
-    message: str = field(metadata=config(field_name="message"))
-    content: BackendAuditObject = field(metadata=config(field_name="content"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+class ConsumerPage:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    title: str = field(default=None, metadata=config(field_name="title"))
+    slug: str = field(default=None, metadata=config(field_name="slug"))
+    content: str = field(default=None, metadata=config(field_name="content"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_audit_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_audit_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_category_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_category_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_config.py` & `fusio-sdk-5.0.3/src/sdk/consumer_scope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
-backend_config automatically generated by SDKgen please do not edit this file manually
+consumer_scope automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import Any
+from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendConfig:
-    id: int = field(metadata=config(field_name="id"))
-    type: int = field(metadata=config(field_name="type"))
-    name: str = field(metadata=config(field_name="name"))
-    description: str = field(metadata=config(field_name="description"))
-    value: Any = field(metadata=config(field_name="value"))
+class ConsumerScope:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    description: str = field(default=None, metadata=config(field_name="description"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_config_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_config_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_connection.py` & `fusio-sdk-5.0.3/src/sdk/backend_dashboard_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
-backend_connection automatically generated by SDKgen please do not edit this file manually
+backend_dashboard_user automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_connection_config import BackendConnectionConfig
-from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendConnection:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    _class: str = field(metadata=config(field_name="class"))
-    config: BackendConnectionConfig = field(metadata=config(field_name="config"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendDashboardUser:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: str = field(default=None, metadata=config(field_name="status"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_connection_introspection_entity.py` & `fusio-sdk-5.0.3/src/sdk/backend_connection_introspection_entity.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
 from backend_connection_introspection_entity_row import BackendConnectionIntrospectionEntityRow
 @dataclass_json
 @dataclass
 class BackendConnectionIntrospectionEntity:
-    name: str = field(metadata=config(field_name="name"))
-    headers: List[str] = field(metadata=config(field_name="headers"))
-    rows: List[BackendConnectionIntrospectionEntityRow] = field(metadata=config(field_name="rows"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    headers: List[str] = field(default=None, metadata=config(field_name="headers"))
+    rows: List[BackendConnectionIntrospectionEntityRow] = field(default=None, metadata=config(field_name="rows"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_connection_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_connection_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_cronjob.py` & `fusio-sdk-5.0.3/src/sdk/backend_scope.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
-backend_cronjob automatically generated by SDKgen please do not edit this file manually
+backend_scope automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
+from backend_scope_operation import BackendScopeOperation
 from common_metadata import CommonMetadata
-from backend_cronjob_error import BackendCronjobError
 @dataclass_json
 @dataclass
-class BackendCronjob:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    cron: str = field(metadata=config(field_name="cron"))
-    action: str = field(metadata=config(field_name="action"))
-    execute_date: datetime.datetime = field(metadata=config(field_name="executeDate"))
-    exit_code: int = field(metadata=config(field_name="exitCode"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
-    errors: List[BackendCronjobError] = field(metadata=config(field_name="errors"))
+class BackendScope:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    description: str = field(default=None, metadata=config(field_name="description"))
+    operations: List[BackendScopeOperation] = field(default=None, metadata=config(field_name="operations"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_cronjob_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_cronjob_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_dashboard.py` & `fusio-sdk-5.0.3/src/sdk/backend_dashboard.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from backend_dashboard_apps import BackendDashboardApps
 from backend_dashboard_requests import BackendDashboardRequests
 from backend_dashboard_users import BackendDashboardUsers
 from backend_dashboard_transactions import BackendDashboardTransactions
 @dataclass_json
 @dataclass
 class BackendDashboard:
-    errors_per_operation: BackendStatisticChart = field(metadata=config(field_name="errorsPerOperation"))
-    incoming_requests: BackendStatisticChart = field(metadata=config(field_name="incomingRequests"))
-    incoming_transactions: BackendStatisticChart = field(metadata=config(field_name="incomingTransactions"))
-    most_used_operations: BackendStatisticChart = field(metadata=config(field_name="mostUsedOperations"))
-    time_per_operation: BackendStatisticChart = field(metadata=config(field_name="timePerOperation"))
-    latest_apps: BackendDashboardApps = field(metadata=config(field_name="latestApps"))
-    latest_requests: BackendDashboardRequests = field(metadata=config(field_name="latestRequests"))
-    latest_users: BackendDashboardUsers = field(metadata=config(field_name="latestUsers"))
-    latest_transactions: BackendDashboardTransactions = field(metadata=config(field_name="latestTransactions"))
+    errors_per_operation: BackendStatisticChart = field(default=None, metadata=config(field_name="errorsPerOperation"))
+    incoming_requests: BackendStatisticChart = field(default=None, metadata=config(field_name="incomingRequests"))
+    incoming_transactions: BackendStatisticChart = field(default=None, metadata=config(field_name="incomingTransactions"))
+    most_used_operations: BackendStatisticChart = field(default=None, metadata=config(field_name="mostUsedOperations"))
+    time_per_operation: BackendStatisticChart = field(default=None, metadata=config(field_name="timePerOperation"))
+    latest_apps: BackendDashboardApps = field(default=None, metadata=config(field_name="latestApps"))
+    latest_requests: BackendDashboardRequests = field(default=None, metadata=config(field_name="latestRequests"))
+    latest_users: BackendDashboardUsers = field(default=None, metadata=config(field_name="latestUsers"))
+    latest_transactions: BackendDashboardTransactions = field(default=None, metadata=config(field_name="latestTransactions"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_dashboard_request.py` & `fusio-sdk-5.0.3/src/sdk/backend_event.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
-backend_dashboard_request automatically generated by SDKgen please do not edit this file manually
+backend_event automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendDashboardRequest:
-    id: int = field(metadata=config(field_name="id"))
-    path: str = field(metadata=config(field_name="path"))
-    ip: str = field(metadata=config(field_name="ip"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+class BackendEvent:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    description: str = field(default=None, metadata=config(field_name="description"))
+    schema: str = field(default=None, metadata=config(field_name="schema"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_dashboard_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_dashboard_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_dashboard_transaction.py` & `fusio-sdk-5.0.3/src/sdk/backend_statistic_count.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """
-backend_dashboard_transaction automatically generated by SDKgen please do not edit this file manually
+backend_statistic_count automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
-class BackendDashboardTransaction:
-    id: int = field(metadata=config(field_name="id"))
-    status: str = field(metadata=config(field_name="status"))
-    provider: str = field(metadata=config(field_name="provider"))
-    transaction_id: str = field(metadata=config(field_name="transactionId"))
-    amount: float = field(metadata=config(field_name="amount"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+class BackendStatisticCount:
+    count: int = field(default=None, metadata=config(field_name="count"))
+    _from: datetime.datetime = field(default=None, metadata=config(field_name="from"))
+    to: datetime.datetime = field(default=None, metadata=config(field_name="to"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_dashboard_user.py` & `fusio-sdk-5.0.3/src/sdk/common_form_element.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-backend_dashboard_user automatically generated by SDKgen please do not edit this file manually
+common_form_element automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
-class BackendDashboardUser:
-    id: int = field(metadata=config(field_name="id"))
-    status: str = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+class CommonFormElement:
+    element: str = field(default=None, metadata=config(field_name="element"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    title: str = field(default=None, metadata=config(field_name="title"))
+    help: str = field(default=None, metadata=config(field_name="help"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_event.py` & `fusio-sdk-5.0.3/src/sdk/common_collection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
-backend_event automatically generated by SDKgen please do not edit this file manually
+common_collection automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
+from typing import List
 @dataclass_json
 @dataclass
-class BackendEvent:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    description: str = field(metadata=config(field_name="description"))
-    schema: str = field(metadata=config(field_name="schema"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class CommonCollection:
+    total_results: int = field(default=None, metadata=config(field_name="totalResults"))
+    start_index: int = field(default=None, metadata=config(field_name="startIndex"))
+    items_per_page: int = field(default=None, metadata=config(field_name="itemsPerPage"))
+    entry: List[T] = field(default=None, metadata=config(field_name="entry"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_event_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_event_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_generator_provider.py` & `fusio-sdk-5.0.3/src/sdk/backend_generator_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
 from backend_generator_provider_config import BackendGeneratorProviderConfig
 @dataclass_json
 @dataclass
 class BackendGeneratorProvider:
-    path: str = field(metadata=config(field_name="path"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    public: bool = field(metadata=config(field_name="public"))
-    config: BackendGeneratorProviderConfig = field(metadata=config(field_name="config"))
+    path: str = field(default=None, metadata=config(field_name="path"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    public: bool = field(default=None, metadata=config(field_name="public"))
+    config: BackendGeneratorProviderConfig = field(default=None, metadata=config(field_name="config"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_generator_provider_changelog.py` & `fusio-sdk-5.0.3/src/sdk/backend_generator_provider_changelog.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 from typing import List
 from backend_schema import BackendSchema
 from backend_action import BackendAction
 from backend_operation import BackendOperation
 @dataclass_json
 @dataclass
 class BackendGeneratorProviderChangelog:
-    schemas: List[BackendSchema] = field(metadata=config(field_name="schemas"))
-    actions: List[BackendAction] = field(metadata=config(field_name="actions"))
-    operations: List[BackendOperation] = field(metadata=config(field_name="operations"))
+    schemas: List[BackendSchema] = field(default=None, metadata=config(field_name="schemas"))
+    actions: List[BackendAction] = field(default=None, metadata=config(field_name="actions"))
+    operations: List[BackendOperation] = field(default=None, metadata=config(field_name="operations"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_generator_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_generator_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_identity.py` & `fusio-sdk-5.0.3/src/sdk/backend_dashboard_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 """
-backend_identity automatically generated by SDKgen please do not edit this file manually
+backend_dashboard_request automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_identity_config import BackendIdentityConfig
 @dataclass_json
 @dataclass
-class BackendIdentity:
-    id: int = field(metadata=config(field_name="id"))
-    app_id: int = field(metadata=config(field_name="appId"))
-    role_id: int = field(metadata=config(field_name="roleId"))
-    name: str = field(metadata=config(field_name="name"))
-    icon: str = field(metadata=config(field_name="icon"))
-    _class: str = field(metadata=config(field_name="class"))
-    config: BackendIdentityConfig = field(metadata=config(field_name="config"))
-    allow_create: bool = field(metadata=config(field_name="allowCreate"))
+class BackendDashboardRequest:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    path: str = field(default=None, metadata=config(field_name="path"))
+    ip: str = field(default=None, metadata=config(field_name="ip"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_identity_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_identity_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_log.py` & `fusio-sdk-5.0.3/src/sdk/backend_cronjob.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-backend_log automatically generated by SDKgen please do not edit this file manually
+backend_cronjob automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_log_error import BackendLogError
+from common_metadata import CommonMetadata
+from backend_cronjob_error import BackendCronjobError
 @dataclass_json
 @dataclass
-class BackendLog:
-    id: int = field(metadata=config(field_name="id"))
-    ip: str = field(metadata=config(field_name="ip"))
-    user_agent: str = field(metadata=config(field_name="userAgent"))
-    method: str = field(metadata=config(field_name="method"))
-    path: str = field(metadata=config(field_name="path"))
-    header: str = field(metadata=config(field_name="header"))
-    body: str = field(metadata=config(field_name="body"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
-    errors: List[BackendLogError] = field(metadata=config(field_name="errors"))
+class BackendCronjob:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    cron: str = field(default=None, metadata=config(field_name="cron"))
+    action: str = field(default=None, metadata=config(field_name="action"))
+    execute_date: datetime.datetime = field(default=None, metadata=config(field_name="executeDate"))
+    exit_code: int = field(default=None, metadata=config(field_name="exitCode"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
+    errors: List[BackendCronjobError] = field(default=None, metadata=config(field_name="errors"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_log_error.py` & `fusio-sdk-5.0.3/src/sdk/backend_cronjob_error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
-backend_log_error automatically generated by SDKgen please do not edit this file manually
+backend_cronjob_error automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
-class BackendLogError:
-    id: int = field(metadata=config(field_name="id"))
-    message: int = field(metadata=config(field_name="message"))
-    trace: str = field(metadata=config(field_name="trace"))
-    file: str = field(metadata=config(field_name="file"))
-    line: int = field(metadata=config(field_name="line"))
+class BackendCronjobError:
+    message: str = field(default=None, metadata=config(field_name="message"))
+    trace: str = field(default=None, metadata=config(field_name="trace"))
+    file: str = field(default=None, metadata=config(field_name="file"))
+    line: int = field(default=None, metadata=config(field_name="line"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_log_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_log_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_marketplace_app.py` & `fusio-sdk-5.0.3/src/sdk/consumer_plan.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
-backend_marketplace_app automatically generated by SDKgen please do not edit this file manually
+consumer_plan automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendMarketplaceApp:
-    version: str = field(metadata=config(field_name="version"))
-    description: str = field(metadata=config(field_name="description"))
-    screenshot: str = field(metadata=config(field_name="screenshot"))
-    website: str = field(metadata=config(field_name="website"))
-    download_url: str = field(metadata=config(field_name="downloadUrl"))
-    sha_hash: str = field(metadata=config(field_name="sha1Hash"))
-    start_url: str = field(metadata=config(field_name="startUrl"))
+class ConsumerPlan:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    description: str = field(default=None, metadata=config(field_name="description"))
+    price: float = field(default=None, metadata=config(field_name="price"))
+    points: int = field(default=None, metadata=config(field_name="points"))
+    period: int = field(default=None, metadata=config(field_name="period"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_marketplace_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_marketplace_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_operation.py` & `fusio-sdk-5.0.3/src/sdk/backend_plan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 """
-backend_operation automatically generated by SDKgen please do not edit this file manually
+backend_plan automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_operation_parameters import BackendOperationParameters
-from backend_operation_throws import BackendOperationThrows
 from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendOperation:
-    id: int = field(metadata=config(field_name="id"))
-    status: int = field(metadata=config(field_name="status"))
-    active: bool = field(metadata=config(field_name="active"))
-    public: bool = field(metadata=config(field_name="public"))
-    stability: int = field(metadata=config(field_name="stability"))
-    description: str = field(metadata=config(field_name="description"))
-    http_method: str = field(metadata=config(field_name="httpMethod"))
-    http_path: str = field(metadata=config(field_name="httpPath"))
-    http_code: int = field(metadata=config(field_name="httpCode"))
-    name: str = field(metadata=config(field_name="name"))
-    parameters: BackendOperationParameters = field(metadata=config(field_name="parameters"))
-    incoming: str = field(metadata=config(field_name="incoming"))
-    outgoing: str = field(metadata=config(field_name="outgoing"))
-    throws: BackendOperationThrows = field(metadata=config(field_name="throws"))
-    action: str = field(metadata=config(field_name="action"))
-    costs: int = field(metadata=config(field_name="costs"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendPlan:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    description: str = field(default=None, metadata=config(field_name="description"))
+    price: float = field(default=None, metadata=config(field_name="price"))
+    points: int = field(default=None, metadata=config(field_name="points"))
+    period: int = field(default=None, metadata=config(field_name="period"))
+    external_id: str = field(default=None, metadata=config(field_name="externalId"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_operation_schema.py` & `fusio-sdk-5.0.3/src/sdk/backend_role.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
-backend_operation_schema automatically generated by SDKgen please do not edit this file manually
+backend_role automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from typing import List
 @dataclass_json
 @dataclass
-class BackendOperationSchema:
-    description: str = field(metadata=config(field_name="description"))
-    type: str = field(metadata=config(field_name="type"))
-    format: str = field(metadata=config(field_name="format"))
-    enum: str = field(metadata=config(field_name="enum"))
+class BackendRole:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    category_id: int = field(default=None, metadata=config(field_name="categoryId"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_operation_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_operation_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_page.py` & `fusio-sdk-5.0.3/src/sdk/backend_rate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
-backend_page automatically generated by SDKgen please do not edit this file manually
+backend_rate automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from typing import List
+from backend_rate_allocation import BackendRateAllocation
 from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendPage:
-    id: int = field(metadata=config(field_name="id"))
-    status: int = field(metadata=config(field_name="status"))
-    title: str = field(metadata=config(field_name="title"))
-    slug: str = field(metadata=config(field_name="slug"))
-    content: str = field(metadata=config(field_name="content"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendRate:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    priority: int = field(default=None, metadata=config(field_name="priority"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    rate_limit: int = field(default=None, metadata=config(field_name="rateLimit"))
+    timespan: datetime.timedelta = field(default=None, metadata=config(field_name="timespan"))
+    allocation: List[BackendRateAllocation] = field(default=None, metadata=config(field_name="allocation"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_page_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_page_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_plan.py` & `fusio-sdk-5.0.3/src/sdk/backend_user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
-backend_plan automatically generated by SDKgen please do not edit this file manually
+backend_user automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
+from backend_app import BackendApp
 from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendPlan:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    description: str = field(metadata=config(field_name="description"))
-    price: float = field(metadata=config(field_name="price"))
-    points: int = field(metadata=config(field_name="points"))
-    period: int = field(metadata=config(field_name="period"))
-    external_id: str = field(metadata=config(field_name="externalId"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendUser:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    role_id: int = field(default=None, metadata=config(field_name="roleId"))
+    plan_id: int = field(default=None, metadata=config(field_name="planId"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    email: str = field(default=None, metadata=config(field_name="email"))
+    points: int = field(default=None, metadata=config(field_name="points"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    apps: List[BackendApp] = field(default=None, metadata=config(field_name="apps"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_plan_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_plan_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_rate.py` & `fusio-sdk-5.0.3/src/sdk/consumer_transaction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
-backend_rate automatically generated by SDKgen please do not edit this file manually
+consumer_transaction automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
-from backend_rate_allocation import BackendRateAllocation
-from common_metadata import CommonMetadata
+from consumer_plan import ConsumerPlan
 @dataclass_json
 @dataclass
-class BackendRate:
-    id: int = field(metadata=config(field_name="id"))
-    priority: int = field(metadata=config(field_name="priority"))
-    name: str = field(metadata=config(field_name="name"))
-    rate_limit: int = field(metadata=config(field_name="rateLimit"))
-    timespan: datetime.timedelta = field(metadata=config(field_name="timespan"))
-    allocation: List[BackendRateAllocation] = field(metadata=config(field_name="allocation"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class ConsumerTransaction:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    user_id: int = field(default=None, metadata=config(field_name="userId"))
+    plan_id: int = field(default=None, metadata=config(field_name="planId"))
+    plan: ConsumerPlan = field(default=None, metadata=config(field_name="plan"))
+    transaction_id: str = field(default=None, metadata=config(field_name="transactionId"))
+    amount: float = field(default=None, metadata=config(field_name="amount"))
+    points: float = field(default=None, metadata=config(field_name="points"))
+    period_start: datetime.datetime = field(default=None, metadata=config(field_name="periodStart"))
+    period_end: datetime.datetime = field(default=None, metadata=config(field_name="periodEnd"))
+    insert_date: datetime.datetime = field(default=None, metadata=config(field_name="insertDate"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_rate_allocation.py` & `fusio-sdk-5.0.3/src/sdk/backend_rate_allocation.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
 class BackendRateAllocation:
-    id: int = field(metadata=config(field_name="id"))
-    operation_id: int = field(metadata=config(field_name="operationId"))
-    user_id: int = field(metadata=config(field_name="userId"))
-    plan_id: int = field(metadata=config(field_name="planId"))
-    app_id: int = field(metadata=config(field_name="appId"))
-    authenticated: bool = field(metadata=config(field_name="authenticated"))
+    id: int = field(default=None, metadata=config(field_name="id"))
+    operation_id: int = field(default=None, metadata=config(field_name="operationId"))
+    user_id: int = field(default=None, metadata=config(field_name="userId"))
+    plan_id: int = field(default=None, metadata=config(field_name="planId"))
+    app_id: int = field(default=None, metadata=config(field_name="appId"))
+    authenticated: bool = field(default=None, metadata=config(field_name="authenticated"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_rate_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_rate_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_role.py` & `fusio-sdk-5.0.3/src/sdk/consumer_user_register.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
-backend_role automatically generated by SDKgen please do not edit this file manually
+consumer_user_register automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
 @dataclass_json
 @dataclass
-class BackendRole:
-    id: int = field(metadata=config(field_name="id"))
-    category_id: int = field(metadata=config(field_name="categoryId"))
-    name: str = field(metadata=config(field_name="name"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
+class ConsumerUserRegister:
+    name: str = field(default=None, metadata=config(field_name="name"))
+    email: str = field(default=None, metadata=config(field_name="email"))
+    password: str = field(default=None, metadata=config(field_name="password"))
+    captcha: str = field(default=None, metadata=config(field_name="captcha"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_role_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_role_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_schema.py` & `fusio-sdk-5.0.3/src/sdk/backend_log_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """
-backend_schema automatically generated by SDKgen please do not edit this file manually
+backend_log_error automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_schema_source import BackendSchemaSource
-from backend_schema_form import BackendSchemaForm
-from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendSchema:
-    id: int = field(metadata=config(field_name="id"))
-    status: int = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    source: BackendSchemaSource = field(metadata=config(field_name="source"))
-    form: BackendSchemaForm = field(metadata=config(field_name="form"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendLogError:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    message: int = field(default=None, metadata=config(field_name="message"))
+    trace: str = field(default=None, metadata=config(field_name="trace"))
+    file: str = field(default=None, metadata=config(field_name="file"))
+    line: int = field(default=None, metadata=config(field_name="line"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_schema_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_schema_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_scope.py` & `fusio-sdk-5.0.3/src/sdk/backend_operation_schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
-backend_scope automatically generated by SDKgen please do not edit this file manually
+backend_operation_schema automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
-from backend_scope_operation import BackendScopeOperation
-from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendScope:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    description: str = field(metadata=config(field_name="description"))
-    operations: List[BackendScopeOperation] = field(metadata=config(field_name="operations"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendOperationSchema:
+    description: str = field(default=None, metadata=config(field_name="description"))
+    type: str = field(default=None, metadata=config(field_name="type"))
+    format: str = field(default=None, metadata=config(field_name="format"))
+    enum: str = field(default=None, metadata=config(field_name="enum"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_scope_category.py` & `fusio-sdk-5.0.3/src/sdk/backend_scope_category.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
 from backend_scope_category_scope import BackendScopeCategoryScope
 @dataclass_json
 @dataclass
 class BackendScopeCategory:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    scopes: List[BackendScopeCategoryScope] = field(metadata=config(field_name="scopes"))
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    scopes: List[BackendScopeCategoryScope] = field(default=None, metadata=config(field_name="scopes"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_scope_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_scope_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_sdk_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_sdk_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_statistic_chart.py` & `fusio-sdk-5.0.3/src/sdk/backend_statistic_chart.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
 from backend_statistic_chart_data import BackendStatisticChartData
 @dataclass_json
 @dataclass
 class BackendStatisticChart:
-    labels: List[str] = field(metadata=config(field_name="labels"))
-    data: List[BackendStatisticChartData] = field(metadata=config(field_name="data"))
-    series: List[str] = field(metadata=config(field_name="series"))
+    labels: List[str] = field(default=None, metadata=config(field_name="labels"))
+    data: List[BackendStatisticChartData] = field(default=None, metadata=config(field_name="data"))
+    series: List[str] = field(default=None, metadata=config(field_name="series"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_statistic_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_statistic_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_tenant_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_tenant_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_token.py` & `fusio-sdk-5.0.3/src/sdk/consumer_app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
-backend_token automatically generated by SDKgen please do not edit this file manually
+consumer_app automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
+from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendToken:
-    id: int = field(metadata=config(field_name="id"))
-    status: int = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    ip: str = field(metadata=config(field_name="ip"))
-    expire: datetime.datetime = field(metadata=config(field_name="expire"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+class ConsumerApp:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    user_id: int = field(default=None, metadata=config(field_name="userId"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    url: str = field(default=None, metadata=config(field_name="url"))
+    app_key: str = field(default=None, metadata=config(field_name="appKey"))
+    app_secret: str = field(default=None, metadata=config(field_name="appSecret"))
+    date: str = field(default=None, metadata=config(field_name="date"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_token_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_token_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_transaction.py` & `fusio-sdk-5.0.3/src/sdk/backend_audit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
-backend_transaction automatically generated by SDKgen please do not edit this file manually
+backend_audit automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from backend_app import BackendApp
+from backend_user import BackendUser
+from backend_audit_object import BackendAuditObject
 @dataclass_json
 @dataclass
-class BackendTransaction:
-    id: int = field(metadata=config(field_name="id"))
-    user_id: int = field(metadata=config(field_name="userId"))
-    plan_id: int = field(metadata=config(field_name="planId"))
-    transaction_id: str = field(metadata=config(field_name="transactionId"))
-    amount: float = field(metadata=config(field_name="amount"))
-    points: float = field(metadata=config(field_name="points"))
-    period_start: datetime.datetime = field(metadata=config(field_name="periodStart"))
-    period_end: datetime.datetime = field(metadata=config(field_name="periodEnd"))
-    insert_date: datetime.datetime = field(metadata=config(field_name="insertDate"))
+class BackendAudit:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    app: BackendApp = field(default=None, metadata=config(field_name="app"))
+    user: BackendUser = field(default=None, metadata=config(field_name="user"))
+    event: str = field(default=None, metadata=config(field_name="event"))
+    ip: str = field(default=None, metadata=config(field_name="ip"))
+    message: str = field(default=None, metadata=config(field_name="message"))
+    content: BackendAuditObject = field(default=None, metadata=config(field_name="content"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_transaction_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_transaction_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_trash_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_trash_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_user.py` & `fusio-sdk-5.0.3/src/sdk/backend_dashboard_transaction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 """
-backend_user automatically generated by SDKgen please do not edit this file manually
+backend_dashboard_transaction automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
-from backend_app import BackendApp
-from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendUser:
-    id: int = field(metadata=config(field_name="id"))
-    role_id: int = field(metadata=config(field_name="roleId"))
-    plan_id: int = field(metadata=config(field_name="planId"))
-    status: int = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    email: str = field(metadata=config(field_name="email"))
-    points: int = field(metadata=config(field_name="points"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    apps: List[BackendApp] = field(metadata=config(field_name="apps"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+class BackendDashboardTransaction:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: str = field(default=None, metadata=config(field_name="status"))
+    provider: str = field(default=None, metadata=config(field_name="provider"))
+    transaction_id: str = field(default=None, metadata=config(field_name="transactionId"))
+    amount: float = field(default=None, metadata=config(field_name="amount"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_user_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_user_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_webhook.py` & `fusio-sdk-5.0.3/src/sdk/consumer_webhook.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-backend_webhook automatically generated by SDKgen please do not edit this file manually
+consumer_webhook automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_webhook_response import BackendWebhookResponse
+from consumer_webhook_response import ConsumerWebhookResponse
 @dataclass_json
 @dataclass
-class BackendWebhook:
-    id: int = field(metadata=config(field_name="id"))
-    event_id: int = field(metadata=config(field_name="eventId"))
-    user_id: int = field(metadata=config(field_name="userId"))
-    name: str = field(metadata=config(field_name="name"))
-    endpoint: str = field(metadata=config(field_name="endpoint"))
-    responses: List[BackendWebhookResponse] = field(metadata=config(field_name="responses"))
+class ConsumerWebhook:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    event: str = field(default=None, metadata=config(field_name="event"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    endpoint: str = field(default=None, metadata=config(field_name="endpoint"))
+    responses: List[ConsumerWebhookResponse] = field(default=None, metadata=config(field_name="responses"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_webhook_response.py` & `fusio-sdk-5.0.3/src/sdk/consumer_user_jwt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
-backend_webhook_response automatically generated by SDKgen please do not edit this file manually
+consumer_user_jwt automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
-class BackendWebhookResponse:
-    id: int = field(metadata=config(field_name="id"))
-    status: int = field(metadata=config(field_name="status"))
-    code: int = field(metadata=config(field_name="code"))
-    attempts: int = field(metadata=config(field_name="attempts"))
-    error: str = field(metadata=config(field_name="error"))
-    execute_date: datetime.datetime = field(metadata=config(field_name="executeDate"))
+class ConsumerUserJWT:
+    token: str = field(default=None, metadata=config(field_name="token"))
+    expires_in: int = field(default=None, metadata=config(field_name="expires_in"))
+    refresh_token: str = field(default=None, metadata=config(field_name="refresh_token"))
+    scope: str = field(default=None, metadata=config(field_name="scope"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/backend_webhook_tag.py` & `fusio-sdk-5.0.3/src/sdk/backend_webhook_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/client.py` & `fusio-sdk-5.0.3/src/sdk/client.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/common_collection.py` & `fusio-sdk-5.0.3/src/sdk/consumer_webhook_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
-common_collection automatically generated by SDKgen please do not edit this file manually
+consumer_webhook_response automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
 @dataclass_json
 @dataclass
-class CommonCollection:
-    total_results: int = field(metadata=config(field_name="totalResults"))
-    start_index: int = field(metadata=config(field_name="startIndex"))
-    items_per_page: int = field(metadata=config(field_name="itemsPerPage"))
-    entry: List[T] = field(metadata=config(field_name="entry"))
+class ConsumerWebhookResponse:
+    status: int = field(default=None, metadata=config(field_name="status"))
+    code: int = field(default=None, metadata=config(field_name="code"))
+    attempts: str = field(default=None, metadata=config(field_name="attempts"))
+    execute_date: str = field(default=None, metadata=config(field_name="executeDate"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/common_form_container.py` & `fusio-sdk-5.0.3/src/sdk/common_form_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from common_form_element_input import CommonFormElementInput
 from common_form_element_select import CommonFormElementSelect
 from common_form_element_tag import CommonFormElementTag
 from common_form_element_text_area import CommonFormElementTextArea
 @dataclass_json
 @dataclass
 class CommonFormContainer:
-    element: List[Union[CommonFormElementInput, CommonFormElementSelect, CommonFormElementTag, CommonFormElementTextArea]] = field(metadata=config(field_name="element"))
+    element: List[Union[CommonFormElementInput, CommonFormElementSelect, CommonFormElementTag, CommonFormElementTextArea]] = field(default=None, metadata=config(field_name="element"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/common_form_element_select.py` & `fusio-sdk-5.0.3/src/sdk/common_form_element_select.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 from dataclasses_json import dataclass_json, config
 from typing import List
 from common_form_element import CommonFormElement
 from common_form_element_select_option import CommonFormElementSelectOption
 @dataclass_json
 @dataclass
 class CommonFormElementSelect(CommonFormElement):
-    options: List[CommonFormElementSelectOption] = field(metadata=config(field_name="options"))
+    options: List[CommonFormElementSelectOption] = field(default=None, metadata=config(field_name="options"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_account_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_account_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_app.py` & `fusio-sdk-5.0.3/src/sdk/backend_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 """
-consumer_app automatically generated by SDKgen please do not edit this file manually
+backend_page automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
 from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class ConsumerApp:
-    id: int = field(metadata=config(field_name="id"))
-    user_id: int = field(metadata=config(field_name="userId"))
-    status: int = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    url: str = field(metadata=config(field_name="url"))
-    app_key: str = field(metadata=config(field_name="appKey"))
-    app_secret: str = field(metadata=config(field_name="appSecret"))
-    date: str = field(metadata=config(field_name="date"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendPage:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    title: str = field(default=None, metadata=config(field_name="title"))
+    slug: str = field(default=None, metadata=config(field_name="slug"))
+    content: str = field(default=None, metadata=config(field_name="content"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_app_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_app_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_authorize_meta.py` & `fusio-sdk-5.0.3/src/sdk/consumer_grant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
-consumer_authorize_meta automatically generated by SDKgen please do not edit this file manually
+consumer_grant automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
-from consumer_scope import ConsumerScope
+from consumer_app import ConsumerApp
 @dataclass_json
 @dataclass
-class ConsumerAuthorizeMeta:
-    name: str = field(metadata=config(field_name="name"))
-    url: str = field(metadata=config(field_name="url"))
-    scopes: List[ConsumerScope] = field(metadata=config(field_name="scopes"))
+class ConsumerGrant:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    app: ConsumerApp = field(default=None, metadata=config(field_name="app"))
+    create_date: datetime.datetime = field(default=None, metadata=config(field_name="createDate"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_authorize_request.py` & `fusio-sdk-5.0.3/src/sdk/consumer_authorize_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
 class ConsumerAuthorizeRequest:
-    response_type: str = field(metadata=config(field_name="responseType"))
-    client_id: str = field(metadata=config(field_name="clientId"))
-    redirect_uri: str = field(metadata=config(field_name="redirectUri"))
-    scope: str = field(metadata=config(field_name="scope"))
-    state: str = field(metadata=config(field_name="state"))
-    allow: bool = field(metadata=config(field_name="allow"))
+    response_type: str = field(default=None, metadata=config(field_name="responseType"))
+    client_id: str = field(default=None, metadata=config(field_name="clientId"))
+    redirect_uri: str = field(default=None, metadata=config(field_name="redirectUri"))
+    scope: str = field(default=None, metadata=config(field_name="scope"))
+    state: str = field(default=None, metadata=config(field_name="state"))
+    allow: bool = field(default=None, metadata=config(field_name="allow"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_authorize_response.py` & `fusio-sdk-5.0.3/src/sdk/consumer_authorize_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from consumer_authorize_response_token import ConsumerAuthorizeResponseToken
 @dataclass_json
 @dataclass
 class ConsumerAuthorizeResponse:
-    type: str = field(metadata=config(field_name="type"))
-    token: ConsumerAuthorizeResponseToken = field(metadata=config(field_name="token"))
-    code: str = field(metadata=config(field_name="code"))
-    redirect_uri: str = field(metadata=config(field_name="redirectUri"))
+    type: str = field(default=None, metadata=config(field_name="type"))
+    token: ConsumerAuthorizeResponseToken = field(default=None, metadata=config(field_name="token"))
+    code: str = field(default=None, metadata=config(field_name="code"))
+    redirect_uri: str = field(default=None, metadata=config(field_name="redirectUri"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_authorize_response_token.py` & `fusio-sdk-5.0.3/src/sdk/consumer_user_plan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
-consumer_authorize_response_token automatically generated by SDKgen please do not edit this file manually
+consumer_user_plan automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
-class ConsumerAuthorizeResponseToken:
-    access_token: str = field(metadata=config(field_name="access_token"))
-    token_type: str = field(metadata=config(field_name="token_type"))
-    expires_in: str = field(metadata=config(field_name="expires_in"))
-    scope: str = field(metadata=config(field_name="scope"))
+class ConsumerUserPlan:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    price: int = field(default=None, metadata=config(field_name="price"))
+    points: int = field(default=None, metadata=config(field_name="points"))
+    period: int = field(default=None, metadata=config(field_name="period"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_event.py` & `fusio-sdk-5.0.3/src/sdk/backend_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
-consumer_event automatically generated by SDKgen please do not edit this file manually
+backend_config automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
+from typing import Any
 @dataclass_json
 @dataclass
-class ConsumerEvent:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    description: str = field(metadata=config(field_name="description"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendConfig:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    type: int = field(default=None, metadata=config(field_name="type"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    description: str = field(default=None, metadata=config(field_name="description"))
+    value: Any = field(default=None, metadata=config(field_name="value"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_event_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_event_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_grant_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_grant_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_identity_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_identity_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_log.py` & `fusio-sdk-5.0.3/src/sdk/consumer_log.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
 class ConsumerLog:
-    id: int = field(metadata=config(field_name="id"))
-    app_id: int = field(metadata=config(field_name="appId"))
-    ip: str = field(metadata=config(field_name="ip"))
-    user_agent: str = field(metadata=config(field_name="userAgent"))
-    method: str = field(metadata=config(field_name="method"))
-    path: str = field(metadata=config(field_name="path"))
-    header: str = field(metadata=config(field_name="header"))
-    body: str = field(metadata=config(field_name="body"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+    id: int = field(default=None, metadata=config(field_name="id"))
+    app_id: int = field(default=None, metadata=config(field_name="appId"))
+    ip: str = field(default=None, metadata=config(field_name="ip"))
+    user_agent: str = field(default=None, metadata=config(field_name="userAgent"))
+    method: str = field(default=None, metadata=config(field_name="method"))
+    path: str = field(default=None, metadata=config(field_name="path"))
+    header: str = field(default=None, metadata=config(field_name="header"))
+    body: str = field(default=None, metadata=config(field_name="body"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_log_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_log_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_page.py` & `fusio-sdk-5.0.3/src/sdk/consumer_authorize_response_token.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
-consumer_page automatically generated by SDKgen please do not edit this file manually
+consumer_authorize_response_token automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class ConsumerPage:
-    id: int = field(metadata=config(field_name="id"))
-    title: str = field(metadata=config(field_name="title"))
-    slug: str = field(metadata=config(field_name="slug"))
-    content: str = field(metadata=config(field_name="content"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class ConsumerAuthorizeResponseToken:
+    access_token: str = field(default=None, metadata=config(field_name="access_token"))
+    token_type: str = field(default=None, metadata=config(field_name="token_type"))
+    expires_in: str = field(default=None, metadata=config(field_name="expires_in"))
+    scope: str = field(default=None, metadata=config(field_name="scope"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_page_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_page_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_payment_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_payment_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_plan.py` & `fusio-sdk-5.0.3/src/sdk/backend_webhook_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
-consumer_plan automatically generated by SDKgen please do not edit this file manually
+backend_webhook_response automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class ConsumerPlan:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    description: str = field(metadata=config(field_name="description"))
-    price: float = field(metadata=config(field_name="price"))
-    points: int = field(metadata=config(field_name="points"))
-    period: int = field(metadata=config(field_name="period"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendWebhookResponse:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    code: int = field(default=None, metadata=config(field_name="code"))
+    attempts: int = field(default=None, metadata=config(field_name="attempts"))
+    error: str = field(default=None, metadata=config(field_name="error"))
+    execute_date: datetime.datetime = field(default=None, metadata=config(field_name="executeDate"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_plan_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_plan_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_scope.py` & `fusio-sdk-5.0.3/src/sdk/backend_marketplace_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
-consumer_scope automatically generated by SDKgen please do not edit this file manually
+backend_marketplace_app automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class ConsumerScope:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    description: str = field(metadata=config(field_name="description"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
+class BackendMarketplaceApp:
+    version: str = field(default=None, metadata=config(field_name="version"))
+    description: str = field(default=None, metadata=config(field_name="description"))
+    screenshot: str = field(default=None, metadata=config(field_name="screenshot"))
+    website: str = field(default=None, metadata=config(field_name="website"))
+    download_url: str = field(default=None, metadata=config(field_name="downloadUrl"))
+    sha_hash: str = field(default=None, metadata=config(field_name="sha1Hash"))
+    start_url: str = field(default=None, metadata=config(field_name="startUrl"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_scope_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_scope_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_token.py` & `fusio-sdk-5.0.3/src/sdk/consumer_app_create.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
-consumer_token automatically generated by SDKgen please do not edit this file manually
+consumer_app_create automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
 @dataclass_json
 @dataclass
-class ConsumerToken:
-    id: int = field(metadata=config(field_name="id"))
-    status: int = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    ip: str = field(metadata=config(field_name="ip"))
-    expire: datetime.date = field(metadata=config(field_name="expire"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+class ConsumerAppCreate:
+    name: str = field(default=None, metadata=config(field_name="name"))
+    url: str = field(default=None, metadata=config(field_name="url"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_token_access_token.py` & `fusio-sdk-5.0.3/src/sdk/consumer_identity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
-consumer_token_access_token automatically generated by SDKgen please do not edit this file manually
+consumer_identity automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
-class ConsumerTokenAccessToken:
-    access_token: str = field(metadata=config(field_name="access_token"))
-    token_type: str = field(metadata=config(field_name="token_type"))
-    expires_in: int = field(metadata=config(field_name="expires_in"))
-    refresh_token: str = field(metadata=config(field_name="refresh_token"))
-    scope: str = field(metadata=config(field_name="scope"))
+class ConsumerIdentity:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    icon: str = field(default=None, metadata=config(field_name="icon"))
+    redirect: str = field(default=None, metadata=config(field_name="redirect"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_token_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_token_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_transaction.py` & `fusio-sdk-5.0.3/src/sdk/consumer_token_access_token.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 """
-consumer_transaction automatically generated by SDKgen please do not edit this file manually
+consumer_token_access_token automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from consumer_plan import ConsumerPlan
 @dataclass_json
 @dataclass
-class ConsumerTransaction:
-    id: int = field(metadata=config(field_name="id"))
-    user_id: int = field(metadata=config(field_name="userId"))
-    plan_id: int = field(metadata=config(field_name="planId"))
-    plan: ConsumerPlan = field(metadata=config(field_name="plan"))
-    transaction_id: str = field(metadata=config(field_name="transactionId"))
-    amount: float = field(metadata=config(field_name="amount"))
-    points: float = field(metadata=config(field_name="points"))
-    period_start: datetime.datetime = field(metadata=config(field_name="periodStart"))
-    period_end: datetime.datetime = field(metadata=config(field_name="periodEnd"))
-    insert_date: datetime.datetime = field(metadata=config(field_name="insertDate"))
+class ConsumerTokenAccessToken:
+    access_token: str = field(default=None, metadata=config(field_name="access_token"))
+    token_type: str = field(default=None, metadata=config(field_name="token_type"))
+    expires_in: int = field(default=None, metadata=config(field_name="expires_in"))
+    refresh_token: str = field(default=None, metadata=config(field_name="refresh_token"))
+    scope: str = field(default=None, metadata=config(field_name="scope"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_transaction_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_transaction_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_user_account.py` & `fusio-sdk-5.0.3/src/sdk/consumer_user_account.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from dataclasses_json import dataclass_json, config
 from typing import List
 from consumer_user_plan import ConsumerUserPlan
 from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class ConsumerUserAccount:
-    id: int = field(metadata=config(field_name="id"))
-    plan_id: int = field(metadata=config(field_name="planId"))
-    status: int = field(metadata=config(field_name="status"))
-    name: str = field(metadata=config(field_name="name"))
-    email: str = field(metadata=config(field_name="email"))
-    points: int = field(metadata=config(field_name="points"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    plans: List[ConsumerUserPlan] = field(metadata=config(field_name="plans"))
-    metadata: CommonMetadata = field(metadata=config(field_name="metadata"))
-    date: datetime.datetime = field(metadata=config(field_name="date"))
+    id: int = field(default=None, metadata=config(field_name="id"))
+    plan_id: int = field(default=None, metadata=config(field_name="planId"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    email: str = field(default=None, metadata=config(field_name="email"))
+    points: int = field(default=None, metadata=config(field_name="points"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    plans: List[ConsumerUserPlan] = field(default=None, metadata=config(field_name="plans"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_user_plan.py` & `fusio-sdk-5.0.3/src/sdk/backend_schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
-consumer_user_plan automatically generated by SDKgen please do not edit this file manually
+backend_schema automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from backend_schema_source import BackendSchemaSource
+from backend_schema_form import BackendSchemaForm
+from common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class ConsumerUserPlan:
-    id: int = field(metadata=config(field_name="id"))
-    name: str = field(metadata=config(field_name="name"))
-    price: int = field(metadata=config(field_name="price"))
-    points: int = field(metadata=config(field_name="points"))
-    period: int = field(metadata=config(field_name="period"))
+class BackendSchema:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    source: BackendSchemaSource = field(default=None, metadata=config(field_name="source"))
+    form: BackendSchemaForm = field(default=None, metadata=config(field_name="form"))
+    metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_user_register.py` & `fusio-sdk-5.0.3/src/sdk/consumer_token.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """
-consumer_user_register automatically generated by SDKgen please do not edit this file manually
+consumer_token automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from typing import List
 @dataclass_json
 @dataclass
-class ConsumerUserRegister:
-    name: str = field(metadata=config(field_name="name"))
-    email: str = field(metadata=config(field_name="email"))
-    password: str = field(metadata=config(field_name="password"))
-    captcha: str = field(metadata=config(field_name="captcha"))
+class ConsumerToken:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    ip: str = field(default=None, metadata=config(field_name="ip"))
+    expire: datetime.date = field(default=None, metadata=config(field_name="expire"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_webhook.py` & `fusio-sdk-5.0.3/src/sdk/consumer_token_create.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
-consumer_webhook automatically generated by SDKgen please do not edit this file manually
+consumer_token_create automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from consumer_webhook_response import ConsumerWebhookResponse
 @dataclass_json
 @dataclass
-class ConsumerWebhook:
-    id: int = field(metadata=config(field_name="id"))
-    status: int = field(metadata=config(field_name="status"))
-    event: str = field(metadata=config(field_name="event"))
-    name: str = field(metadata=config(field_name="name"))
-    endpoint: str = field(metadata=config(field_name="endpoint"))
-    responses: List[ConsumerWebhookResponse] = field(metadata=config(field_name="responses"))
+class ConsumerTokenCreate:
+    name: str = field(default=None, metadata=config(field_name="name"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    expire: datetime.date = field(default=None, metadata=config(field_name="expire"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_webhook_response.py` & `fusio-sdk-5.0.3/src/sdk/backend_token.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """
-consumer_webhook_response automatically generated by SDKgen please do not edit this file manually
+backend_token automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from typing import List
 @dataclass_json
 @dataclass
-class ConsumerWebhookResponse:
-    status: int = field(metadata=config(field_name="status"))
-    code: int = field(metadata=config(field_name="code"))
-    attempts: str = field(metadata=config(field_name="attempts"))
-    execute_date: str = field(metadata=config(field_name="executeDate"))
+class BackendToken:
+    id: int = field(default=None, metadata=config(field_name="id"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    name: str = field(default=None, metadata=config(field_name="name"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    ip: str = field(default=None, metadata=config(field_name="ip"))
+    expire: datetime.datetime = field(default=None, metadata=config(field_name="expire"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/consumer_webhook_tag.py` & `fusio-sdk-5.0.3/src/sdk/consumer_webhook_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/system_about.py` & `fusio-sdk-5.0.3/src/sdk/system_about.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from dataclasses_json import dataclass_json, config
 from typing import List
 from system_about_apps import SystemAboutApps
 from system_about_link import SystemAboutLink
 @dataclass_json
 @dataclass
 class SystemAbout:
-    api_version: str = field(metadata=config(field_name="apiVersion"))
-    title: str = field(metadata=config(field_name="title"))
-    description: str = field(metadata=config(field_name="description"))
-    terms_of_service: str = field(metadata=config(field_name="termsOfService"))
-    contact_name: str = field(metadata=config(field_name="contactName"))
-    contact_url: str = field(metadata=config(field_name="contactUrl"))
-    contact_email: str = field(metadata=config(field_name="contactEmail"))
-    license_name: str = field(metadata=config(field_name="licenseName"))
-    license_url: str = field(metadata=config(field_name="licenseUrl"))
-    payment_currency: str = field(metadata=config(field_name="paymentCurrency"))
-    categories: List[str] = field(metadata=config(field_name="categories"))
-    scopes: List[str] = field(metadata=config(field_name="scopes"))
-    apps: SystemAboutApps = field(metadata=config(field_name="apps"))
-    links: List[SystemAboutLink] = field(metadata=config(field_name="links"))
+    api_version: str = field(default=None, metadata=config(field_name="apiVersion"))
+    title: str = field(default=None, metadata=config(field_name="title"))
+    description: str = field(default=None, metadata=config(field_name="description"))
+    terms_of_service: str = field(default=None, metadata=config(field_name="termsOfService"))
+    contact_name: str = field(default=None, metadata=config(field_name="contactName"))
+    contact_url: str = field(default=None, metadata=config(field_name="contactUrl"))
+    contact_email: str = field(default=None, metadata=config(field_name="contactEmail"))
+    license_name: str = field(default=None, metadata=config(field_name="licenseName"))
+    license_url: str = field(default=None, metadata=config(field_name="licenseUrl"))
+    payment_currency: str = field(default=None, metadata=config(field_name="paymentCurrency"))
+    categories: List[str] = field(default=None, metadata=config(field_name="categories"))
+    scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    apps: SystemAboutApps = field(default=None, metadata=config(field_name="apps"))
+    links: List[SystemAboutLink] = field(default=None, metadata=config(field_name="links"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/system_connection_tag.py` & `fusio-sdk-5.0.3/src/sdk/system_connection_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/system_meta_tag.py` & `fusio-sdk-5.0.3/src/sdk/system_meta_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sdkgen
 from requests import RequestException
 
 from common_message_exception import CommonMessageException
 from passthru import Passthru
 from system_about import SystemAbout
 from system_health_check import SystemHealthCheck
+from system_o_auth_configuration import SystemOAuthConfiguration
 from system_route import SystemRoute
 from system_schema import SystemSchema
 
 class SystemMetaTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
@@ -71,14 +72,38 @@
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     pass
+
+    def get_o_auth_configuration(self) -> SystemOAuthConfiguration:
+        try:
+            path_params = {}
+
+            query_params = {}
+
+            query_struct_names = []
+
+            url = self.parser.url("/system/oauth-authorization-server", path_params)
+
+            headers = {}
+
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+
+            if response.status_code >= 200 and response.status_code < 300:
+                return SystemOAuthConfiguration.from_json(response.content)
+
+
+            raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
+        except RequestException as e:
+            raise sdkgen.ClientException("An unknown error occurred: " + str(e))
+
+    pass
 
     def get_health(self) -> SystemHealthCheck:
         try:
             path_params = {}
 
             query_params = {}
```

### Comparing `fusio-sdk-5.0.2/src/sdk/system_payment_tag.py` & `fusio-sdk-5.0.3/src/sdk/system_payment_tag.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.2/src/sdk/system_schema.py` & `fusio-sdk-5.0.3/src/sdk/system_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from system_schema_type_schema import SystemSchemaTypeSchema
 from system_schema_form import SystemSchemaForm
 @dataclass_json
 @dataclass
 class SystemSchema:
-    schema: SystemSchemaTypeSchema = field(metadata=config(field_name="schema"))
-    form: SystemSchemaForm = field(metadata=config(field_name="form"))
+    schema: SystemSchemaTypeSchema = field(default=None, metadata=config(field_name="schema"))
+    form: SystemSchemaForm = field(default=None, metadata=config(field_name="form"))
```

### Comparing `fusio-sdk-5.0.2/src/sdk/system_tag.py` & `fusio-sdk-5.0.3/src/sdk/system_tag.py`

 * *Files identical despite different names*

