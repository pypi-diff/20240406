# Comparing `tmp/pulumi_azuredevops-3.1.0a1711735015.tar.gz` & `tmp/pulumi_azuredevops-3.1.0a1712399297.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_azuredevops-3.1.0a1711735015.tar", last modified: Fri Mar 29 18:11:17 2024, max compression
+gzip compressed data, was "pulumi_azuredevops-3.1.0a1712399297.tar", last modified: Sat Apr  6 10:42:17 2024, max compression
```

## Comparing `pulumi_azuredevops-3.1.0a1711735015.tar` & `pulumi_azuredevops-3.1.0a1712399297.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:11:17.833784 pulumi_azuredevops-3.1.0a1711735015/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-03-29 18:11:17.833784 pulumi_azuredevops-3.1.0a1711735015/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:11:17.833784 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/
--rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   159174 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/area_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_auto_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_comment_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_merge_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_status_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16941 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_work_item_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    43565 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    29769 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/build_definition_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/build_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    30632 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/build_folder_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25884 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)    36499 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_branch_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    56723 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_business_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_exclusive_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_required_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:11:17.833784 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/elastic_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/environment_resource_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_agent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_service_endpoint_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_serviceendpoint_azurecr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_serviceendpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    42778 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/git_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/git_repository_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/git_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    29903 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/group_entitlement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    20785 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/iterative_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/library_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   201840 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/pipeline_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    23748 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/project_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/project_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26547 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/project_pipeline_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    21960 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_author_email_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20904 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_case_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    18085 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_check_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_file_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_max_file_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    20181 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_max_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_reserved_names.py
--rw-r--r--   0 runner    (1001) docker     (127)    17453 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/resource_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    24222 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    27945 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    30889 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_azure_ecr.py
--rw-r--r--   0 runner    (1001) docker     (127)    59232 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17330 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    26408 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_generic_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_git_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)    25409 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20052 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_service_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_sonar_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_sonar_qube.py
--rw-r--r--   0 runner    (1001) docker     (127)    23003 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    25768 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_argocd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_externaltfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24637 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
--rw-r--r--   0 runner    (1001) docker     (127)    21103 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)    26010 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25472 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26764 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_maven.py
--rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25867 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_nuget.py
--rw-r--r--   0 runner    (1001) docker     (127)    20117 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23357 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18015 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/servicehook_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30631 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/tagging_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    18618 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/team_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/team_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    21781 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24576 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22441 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/variable_group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26033 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/work_item_query_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/workitem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:11:17.833784 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-03-29 18:11:17.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-03-29 18:11:17.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 18:11:17.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 18:11:17.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-29 18:11:17.000000 pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-29 18:11:11.000000 pulumi_azuredevops-3.1.0a1711735015/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 18:11:17.833784 pulumi_azuredevops-3.1.0a1711735015/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:17.649031 pulumi_azuredevops-3.1.0a1712399297/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-06 10:42:17.649031 pulumi_azuredevops-3.1.0a1712399297/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:17.649031 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/
+-rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   159174 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/area_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_auto_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_comment_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_merge_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_status_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16941 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_work_item_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43565 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29769 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/build_definition_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/build_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30632 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/build_folder_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25884 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36499 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_branch_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56723 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_business_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_exclusive_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_required_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:17.649031 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/elastic_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/environment_resource_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_agent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_service_endpoint_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_serviceendpoint_azurecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_serviceendpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42778 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/git_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/git_repository_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/git_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29903 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/group_entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20785 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/iterative_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/library_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201840 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/pipeline_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23748 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/project_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/project_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26547 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/project_pipeline_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21960 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_author_email_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20904 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_case_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18085 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_check_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_file_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_max_file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20181 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_max_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_reserved_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17417 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/resource_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24222 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27945 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30889 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_azure_ecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59232 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17330 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26408 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_generic_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25409 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20052 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_service_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_sonar_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_sonar_qube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23003 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25768 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_argocd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_externaltfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24637 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21103 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26010 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25472 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26764 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_maven.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25867 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_nuget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20117 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23357 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18015 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/servicehook_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30631 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/tagging_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18618 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/team_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21781 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24576 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22441 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/variable_group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26033 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/work_item_query_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/workitem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:17.649031 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-06 10:42:17.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-06 10:42:17.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:42:17.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 10:42:17.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 10:42:17.000000 pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 10:42:11.000000 pulumi_azuredevops-3.1.0a1712399297/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 10:42:17.649031 pulumi_azuredevops-3.1.0a1712399297/setup.cfg
```

### Comparing `pulumi_azuredevops-3.1.0a1711735015/PKG-INFO` & `pulumi_azuredevops-3.1.0a1712399297/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.1.0a1711735015
+Version: 3.1.0a1712399297
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.1.0a1711735015/README.md` & `pulumi_azuredevops-3.1.0a1712399297/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/__init__.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/_inputs.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/_utilities.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/area_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/area_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_auto_reviewers.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_auto_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_build_validation.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_build_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_comment_resolution.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_comment_resolution.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_merge_types.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_merge_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_min_reviewers.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_min_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_status_check.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_status_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/branch_policy_work_item_linking.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/branch_policy_work_item_linking.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/build_definition.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/build_definition_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/build_definition_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/build_folder.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/build_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/build_folder_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/build_folder_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_approval.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_branch_control.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_branch_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_business_hours.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_business_hours.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_exclusive_lock.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_exclusive_lock.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/check_required_template.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/check_required_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/config/__init__.pyi` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/config/vars.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/elastic_pool.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/elastic_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/environment.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/environment_resource_kubernetes.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/environment_resource_kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_agent_queue.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_agent_queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_area.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_area.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_build_definition.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_client_config.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_environment.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_git_repository.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_git_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_group.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_groups.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_iteration.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_iteration.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_pool.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_pools.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_project.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_projects.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_repositories.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_service_endpoint_github.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_service_endpoint_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_serviceendpoint_azurecr.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_serviceendpoint_azurecr.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_serviceendpoint_npm.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_serviceendpoint_npm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_team.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_teams.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_users.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/get_variable_group.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/get_variable_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 def get_variable_group(name: Optional[str] = None,
                        project_id: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVariableGroupResult:
     """
     Use this data source to access information about existing Variable Groups within Azure DevOps.
 
-    > **Note:** Secret values are masked by service and cannot be obtained through API. [Set secret variables](<https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops&tabs=yaml%!C(MISSING)batch#secret-variables>)
+    > **Note:** Secret values are masked by service and cannot be obtained through API. [Set secret variables](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops&tabs=yaml%2Cbatch#secret-variables)
 
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
@@ -163,15 +163,15 @@
 @_utilities.lift_output_func(get_variable_group)
 def get_variable_group_output(name: Optional[pulumi.Input[str]] = None,
                               project_id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVariableGroupResult]:
     """
     Use this data source to access information about existing Variable Groups within Azure DevOps.
 
-    > **Note:** Secret values are masked by service and cannot be obtained through API. [Set secret variables](<https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops&tabs=yaml%!C(MISSING)batch#secret-variables>)
+    > **Note:** Secret values are masked by service and cannot be obtained through API. [Set secret variables](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops&tabs=yaml%2Cbatch#secret-variables)
 
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
```

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/git.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/git_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/git_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/git_repository_branch.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/git_repository_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/git_repository_file.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/git_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/group.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/group_entitlement.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/group_entitlement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/group_membership.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/iterative_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/iterative_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/library_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/library_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/outputs.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/pipeline_authorization.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/pipeline_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/pool.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/project.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/project_features.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/project_features.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/project_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/project_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/project_pipeline_settings.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/project_pipeline_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/provider.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/queue.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_author_email_pattern.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_author_email_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_case_enforcement.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_case_enforcement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_check_credentials.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_check_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_file_path_pattern.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_file_path_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_max_file_size.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_max_file_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_max_path_length.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_max_path_length.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/repository_policy_reserved_names.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/repository_policy_reserved_names.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/resource_authorization.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/resource_authorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             resource_id=example_service_endpoint_bit_bucket.id,
             authorized=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
-        - [Azure DevOps Service REST API 7.0 - Authorize Definition Resource](<https://docs.microsoft.com/en-us/rest/api/azure/devops/build/resources/authorize%!d(MISSING)efinition%!r(MISSING)esources?view=azure-devops-rest-7.0>)
+        - [Azure DevOps Service REST API 7.0 - Authorize Definition Resource](https://docs.microsoft.com/en-us/rest/api/azure/devops/build/resources/authorize%20definition%20resources?view=azure-devops-rest-7.0)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] authorized: Set to true to allow public access in the project. Type: boolean.
         :param pulumi.Input[int] definition_id: The ID of the build definition to authorize. Type: string.
         :param pulumi.Input[str] project_id: The project ID or project name. Type: string.
         :param pulumi.Input[str] resource_id: The ID of the resource to authorize. Type: string.
@@ -271,15 +271,15 @@
             resource_id=example_service_endpoint_bit_bucket.id,
             authorized=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
-        - [Azure DevOps Service REST API 7.0 - Authorize Definition Resource](<https://docs.microsoft.com/en-us/rest/api/azure/devops/build/resources/authorize%!d(MISSING)efinition%!r(MISSING)esources?view=azure-devops-rest-7.0>)
+        - [Azure DevOps Service REST API 7.0 - Authorize Definition Resource](https://docs.microsoft.com/en-us/rest/api/azure/devops/build/resources/authorize%20definition%20resources?view=azure-devops-rest-7.0)
 
         :param str resource_name: The name of the resource.
         :param ResourceAuthorizationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_artifactory.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_artifactory.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_aws.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_aws.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_azure_dev_ops.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_azure_dev_ops.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_azure_ecr.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_azure_ecr.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_bit_bucket.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_bit_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_docker_registry.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_docker_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_generic.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_generic.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_generic_git.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_generic_git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_git_hub.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_git_hub.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_kubernetes.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_npm.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_npm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_pipeline.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_service_fabric.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_service_fabric.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_sonar_cloud.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_sonar_qube.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_sonar_qube.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/service_endpoint_ssh.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/service_endpoint_ssh.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_argocd.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_argocd.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_externaltfs.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_externaltfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_gcp_terraform.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_gcp_terraform.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_incomingwebhook.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_incomingwebhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jenkins.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jenkins.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_maven.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_maven.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_nexus.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_nexus.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_nuget.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_nuget.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_octopusdeploy.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_octopusdeploy.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/serviceendpoint_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/serviceendpoint_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/servicehook_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/servicehook_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/servicehook_storage_queue_pipelines.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/servicehook_storage_queue_pipelines.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/tagging_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/tagging_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/team.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/team_administrators.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/team_administrators.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/team_members.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/user.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/variable_group.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/variable_group_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/variable_group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/work_item_query_permissions.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/work_item_query_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops/workitem.py` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops/workitem.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops.egg-info/PKG-INFO` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.1.0a1711735015
+Version: 3.1.0a1712399297
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pulumi_azuredevops.egg-info/SOURCES.txt` & `pulumi_azuredevops-3.1.0a1712399297/pulumi_azuredevops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1711735015/pyproject.toml` & `pulumi_azuredevops-3.1.0a1712399297/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_azuredevops"
   description = "A Pulumi package for creating and managing Azure DevOps."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "azuredevops"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.1.0a1711735015"
+  version = "3.1.0a1712399297"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-azuredevops"
 
 [build-system]
```

