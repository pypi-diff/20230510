# Comparing `tmp/pulumi_azuredevops-2.8.0.tar.gz` & `tmp/pulumi_azuredevops-2.8.0a1683661270.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_azuredevops-2.8.0.tar", last modified: Tue May  9 21:03:48 2023, max compression
+gzip compressed data, was "pulumi_azuredevops-2.8.0a1683661270.tar", last modified: Tue May  9 19:47:38 2023, max compression
```

## Comparing `pulumi_azuredevops-2.8.0.tar` & `pulumi_azuredevops-2.8.0a1683661270.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.573485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/
--rw-r--r--   0 runner    (1001) docker     (123)    24455 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   147060 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.573485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/area_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_auto_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_comment_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    16839 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_merge_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_status_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_work_item_linking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.573485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38702 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    44955 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38457 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build_definition_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/build_folder_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32736 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/check_branch_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    52960 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/check_business_hours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.573485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.573485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21750 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/project_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.573485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/entitlement/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/entitlement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/entitlement/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_agent_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_build_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_service_endpoint_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_variable_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/git_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/git_repository_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/git_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    29921 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/group_membership.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    30141 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/iterative_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)   189015 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/pipeline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/pipeline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24694 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/pipeline/variable_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19196 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/project_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/project_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/project_pipeline_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    22877 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_author_email_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_case_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_check_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_file_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_max_file_size.py
--rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_max_path_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_reserved_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/resource_authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/security/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/security/resource_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    22356 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    30733 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_azure_ecr.py
--rw-r--r--   0 runner    (1001) docker     (123)    39015 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18522 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_generic_git.py
--rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_git_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    18919 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    26154 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_service_fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_sonar_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_sonar_qube.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38745 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    27750 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/git_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_argocd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17775 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_externaltfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    25176 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19604 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/servicehook_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/tagging_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/team_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/variable_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/work_item_query_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops/workitem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:48.573485 pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:03:48.577485 pulumi_azuredevops-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-09 21:03:48.000000 pulumi_azuredevops-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.406342 pulumi_azuredevops-2.8.0a1683661270/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/
+-rw-r--r--   0 runner    (1001) docker     (123)    24455 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147060 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/area_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_auto_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_comment_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16839 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_merge_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_status_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_work_item_linking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38702 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44955 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38457 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_definition_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_folder_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32736 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/check_branch_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52960 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/check_business_hours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21750 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/project_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/entitlement/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/entitlement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/entitlement/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_agent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_service_endpoint_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_repository_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29921 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/group_membership.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30141 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/iterative_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189015 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24694 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/variable_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19196 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_pipeline_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22877 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_author_email_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_case_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_check_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_file_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_max_file_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_max_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_reserved_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/resource_authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/security/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/security/resource_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22356 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30733 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_ecr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39015 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18522 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_generic_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18919 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26154 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_service_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_sonar_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_sonar_qube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38745 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27750 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_argocd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17775 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_externaltfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25176 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19604 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/servicehook_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/tagging_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/work_item_query_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/workitem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:47:38.406342 pulumi_azuredevops-2.8.0a1683661270/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/setup.py
```

### Comparing `pulumi_azuredevops-2.8.0/PKG-INFO` & `pulumi_azuredevops-2.8.0a1683661270/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 2.8.0
+Version: 2.8.0a1683661270
 Summary: A Pulumi package for creating and managing Azure DevOps.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi azuredevops
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_azuredevops-2.8.0/README.md` & `pulumi_azuredevops-2.8.0a1683661270/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/__init__.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/_utilities.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/get_pool.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/get_pools.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/pool.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/agent/queue.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/area_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/area_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_auto_reviewers.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_auto_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_build_validation.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_build_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_comment_resolution.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_comment_resolution.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_merge_types.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_merge_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_min_reviewers.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_min_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_status_check.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_status_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/branch_policy_work_item_linking.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_work_item_linking.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/build/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/build/build_definition.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/build/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/build_definition.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/build_definition_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_definition_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/build_folder.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/build_folder_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_folder_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/check_branch_control.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/check_branch_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/check_business_hours.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/check_business_hours.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/config/vars.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/get_client_config.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/get_project.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/get_projects.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/project.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/core/project_features.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/project_features.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/entitlement/user.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/entitlement/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/environment.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_agent_queue.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_agent_queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_area.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_area.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_build_definition.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_client_config.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_git_repository.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_git_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_groups.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_iteration.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_iteration.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_pool.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_pools.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_project.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_projects.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_repositories.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_service_endpoint_azure_rm.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_service_endpoint_github.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_service_endpoint_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_team.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_teams.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_users.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/get_variable_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/git.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/git_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/git_repository_branch.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_repository_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/git_repository_file.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/group_membership.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/get_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/get_users.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/group_membership.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/identities/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/iterative_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/iterative_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/pipeline/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/pipeline/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/pipeline/variable_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/branch_policy_build_validation.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/branch_policy_build_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/branch_policy_min_reviewers.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/branch_policy_min_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/policy/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/pool.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/project.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/project_features.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_features.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/project_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/project_pipeline_settings.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_pipeline_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/provider.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/queue.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/get_repositories.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/git.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_author_email_pattern.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_author_email_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_case_enforcement.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_case_enforcement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_check_credentials.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_check_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_file_path_pattern.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_file_path_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_max_file_size.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_max_file_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_max_path_length.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_max_path_length.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/repository_policy_reserved_names.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_reserved_names.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/resource_authorization.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/resource_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/security/resource_authorization.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/security/resource_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_artifactory.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_artifactory.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_aws.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_aws.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_azure_dev_ops.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_dev_ops.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_azure_ecr.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_ecr.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_azure_rm.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_bit_bucket.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_bit_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_docker_registry.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_docker_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_generic.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_generic.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_generic_git.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_generic_git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_git_hub.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_git_hub.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_kubernetes.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_npm.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_npm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_pipeline.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_service_fabric.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_service_fabric.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_sonar_cloud.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_sonar_qube.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_sonar_qube.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/service_endpoint_ssh.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_ssh.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/azure_rm.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/bit_bucket.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/bit_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/docker_registry.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/docker_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/git_hub.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/git_hub.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/kubernetes.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_argocd.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_argocd.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_externaltfs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_externaltfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_incomingwebhook.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_incomingwebhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_octopusdeploy.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_octopusdeploy.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/serviceendpoint_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/servicehook_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/servicehook_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/tagging_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/tagging_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/team.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/team_administrators.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team_administrators.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/team_members.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/user.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/variable_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/work_item_query_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/work_item_query_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops/workitem.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/workitem.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/PKG-INFO` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-azuredevops
-Version: 2.8.0
+Version: 2.8.0a1683661270
 Summary: A Pulumi package for creating and managing Azure DevOps.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi azuredevops
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_azuredevops-2.8.0/pulumi_azuredevops.egg-info/SOURCES.txt` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.8.0/setup.py` & `pulumi_azuredevops-2.8.0a1683661270/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.8.0"
-PLUGIN_VERSION = "2.8.0"
+VERSION = "2.8.0a1683661270"
+PLUGIN_VERSION = "2.8.0-alpha.1683661270+aa6c7d3b"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'azuredevops', PLUGIN_VERSION])
         except OSError as error:
```

