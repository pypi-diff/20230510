# Comparing `tmp/iambic_core-0.6.3.tar.gz` & `tmp/iambic_core-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.6.3.tar", max compression
+gzip compressed data, was "iambic_core-0.7.1.tar", max compression
```

## Comparing `iambic_core-0.6.3.tar` & `iambic_core-0.7.1.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0    11356 2023-05-06 19:36:22.982867 iambic_core-0.6.3/LICENSE.md
--rw-r--r--   0        0        0    10551 2023-05-06 19:36:22.982867 iambic_core-0.6.3/README.md
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/__init__.py
--rw-r--r--   0        0        0    20099 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/templates.py
--rw-r--r--   0        0        0     1955 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/utils.py
--rw-r--r--   0        0        0    74846 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-05-06 19:36:23.006868 iambic_core-0.6.3/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/logger.py
--rw-r--r--   0        0        0    24862 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5516 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/parser.py
--rw-r--r--   0        0        0    46094 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/template_generation.py
--rw-r--r--   0        0        0    26626 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/lambda/app.py
--rw-r--r--   0        0        0    13694 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/main.py
--rw-r--r--   0        0        0      664 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/__init__.py
--rw-r--r--   0        0        0     2799 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1753 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     2149 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     2268 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     2483 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    14509 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    33385 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    17683 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13616 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15824 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    17544 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10649 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21304 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24395 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    20623 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22579 2023-05-06 19:36:23.010868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4534 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31619 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35514 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    28137 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1086 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     2973 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10183 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13766 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8515 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8648 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      908 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-05-06 19:36:23.014868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5247 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1154 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9282 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11393 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2685 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1085 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9492 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13610 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      864 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      137 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-05-06 19:36:23.018868 iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     1922 2023-05-06 19:36:23.018868 iambic_core-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 iambic_core-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 23:07:43.595854 iambic_core-0.7.1/LICENSE.md
+-rw-r--r--   0        0        0    10551 2023-05-09 23:07:43.595854 iambic_core-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20099 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/config/templates.py
+-rw-r--r--   0        0        0     3312 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/config/utils.py
+-rw-r--r--   0        0        0    77079 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/logger.py
+-rw-r--r--   0        0        0    24862 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5516 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/parser.py
+-rw-r--r--   0        0        0    46094 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    26626 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/lambda/app.py
+-rw-r--r--   0        0        0    13921 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2799 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2149 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2268 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2483 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     1902 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    16350 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    33385 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    17683 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13616 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.619855 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15824 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    17544 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10649 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21304 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24395 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    20623 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22579 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     4534 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31619 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35514 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    28498 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0     1086 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     2973 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10183 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    13766 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8515 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8648 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      908 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14549 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5247 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1154 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-05-09 23:07:43.623854 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9282 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11393 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2685 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1085 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9492 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13610 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      864 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      977 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      137 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-05-09 23:07:43.627855 iambic_core-0.7.1/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     1922 2023-05-09 23:07:43.627855 iambic_core-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 iambic_core-0.7.1/PKG-INFO
```

### Comparing `iambic_core-0.6.3/LICENSE.md` & `iambic_core-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/README.md` & `iambic_core-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/config/dynamic_config.py` & `iambic_core-0.7.1/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/config/wizard.py` & `iambic_core-0.7.1/iambic/config/wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,18 @@
     Config,
     ExtendsConfig,
     ExtendsConfigKey,
     load_config,
     process_config,
 )
 from iambic.config.utils import (
+    aws_cf_parse_key_value_string,
     check_and_update_resource_limit,
     resolve_config_template_path,
+    validate_aws_cf_input_tags,
 )
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.parser import load_templates
 from iambic.core.template_generation import get_existing_template_map
@@ -52,14 +54,15 @@
 from iambic.plugins.v0_1_0.aws.iam.role.models import (
     AWS_IAM_ROLE_TEMPLATE_TYPE,
     AwsIamRoleTemplate,
 )
 from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
 from iambic.plugins.v0_1_0.aws.models import (
     ARN_RE,
+    IAMBIC_HUB_ROLE_NAME,
     IAMBIC_SPOKE_ROLE_NAME,
     AWSAccount,
     AWSIdentityCenter,
     AWSOrganization,
     BaseAWSOrgRule,
     Partition,
     get_hub_role_arn,
@@ -110,15 +113,14 @@
         None
 
     Returns:
         None
     """
     # Warning: This appears to work fine in a real terminal,
     # but not VSCode's Debug Terminal
-
     r, _, _ = select.select([sys.stdin], [], [], 0)
     while r:
         # If there is input waiting, read and discard it.
         sys.stdin.readline()
         r, _, _ = select.select([sys.stdin], [], [], 0)
 
 
@@ -334,25 +336,26 @@
         )
         if questionary.confirm("Proceed?").unsafe_ask():
             log.info("Exiting...")
             sys.exit(0)
 
 
 class ConfigurationWizard:
-    def __init__(self, repo_dir: str):
+    def __init__(self, repo_dir: str, is_more_options: bool = False):
         # TODO: Handle the case where the config file exists but is not valid
         self.existing_role_template_map = {}
         self.aws_account_map = {}
         self.repo_dir = repo_dir
         self._has_cf_permissions = None
         self._cf_role_arn = None
         self._assume_as_arn = None
         self.caller_identity = {}
         self.profile_name = ""
         self._default_region = None
+        self._is_more_options = is_more_options
 
         asyncio.run(self.set_config_details())
         check_and_update_resource_limit(self.config)
         log.debug("Starting configuration wizard", config_path=self.config_path)
 
     @property
     def has_cf_permissions(self):
@@ -798,14 +801,15 @@
         requires_sync = bool(
             not is_hub_account
             and (
                 len(self.config.aws.accounts)
                 > self.config.aws.min_accounts_required_for_wildcard_included_accounts
             )
         )
+        assume_as_arn = self.assume_as_arn
 
         if is_hub_account:
             account_id = self.hub_account_id
             account_name = set_required_text_value(
                 "What is the name of the AWS Account?"
             )
             default_region = self.aws_default_region
@@ -820,14 +824,16 @@
 
             if not questionary.confirm("Proceed?").unsafe_ask():
                 log.info(
                     "Unable to add the AWS Account without creating the required roles."
                 )
                 return
 
+            role_arn = set_aws_role_arn(account_id)
+
         else:
             if requires_sync:
                 click.echo(
                     "\nAdding this account will require a sync to be run.\n"
                     "This is to apply any matching templates to the account if the resource does not already exist.\n"
                     "Then, the account resources will be imported into Iambic."
                 )
@@ -850,15 +856,14 @@
                 log.info("AWS Account already exists in the configuration")
                 return
 
             default_region = set_aws_region(
                 "What region should IAMbic use?", self.aws_default_region
             )
             role_arn = set_aws_role_arn(account_id)
-            assume_as_arn = self.assume_as_arn
 
             click.echo(
                 "\nIAMbic requires Hub and Spoke roles to be created which is deployed using CloudFormation.\n"
                 "To review the templates used or deploy them manually, the template used can be found here:\n"
                 "https://github.com/noqdev/iambic/blob/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml\n"
                 "If you have already manually deployed the templates, answer yes to proceed.\n"
                 "IAMbic will validate that your stacks have been deployed successfully and will not attempt to replace them."
@@ -878,57 +883,69 @@
             return
 
         if is_hub_account and not profile_name:
             profile_name = self.profile_name
         elif not is_hub_account:
             profile_name = None
 
+        hub_role_name, spoke_role_name, tags = self.set_aws_cf_customization()
+
         cf_client = session.client("cloudformation", region_name=default_region)
 
         if is_hub_account:
             created_successfully = asyncio.run(
                 create_iambic_role_stacks(
                     cf_client=cf_client,
                     hub_account_id=account_id,
                     assume_as_arn=assume_as_arn,
                     role_arn=role_arn,
                     read_only=read_only,
+                    hub_role_stack_name=hub_role_name,
+                    hub_role_name=hub_role_name,
+                    spoke_role_stack_name=spoke_role_name,
+                    spoke_role_name=spoke_role_name,
+                    tags=tags,
                 )
             )
             if not created_successfully:
                 log.error("Failed to create the required IAMbic roles. Exiting.")
                 sys.exit(0)
         else:
             created_successfully = asyncio.run(
                 create_spoke_role_stack(
                     cf_client=cf_client,
                     hub_account_id=account_id,
                     role_arn=role_arn,
                     read_only=read_only,
+                    hub_role_stack_name=hub_role_name,
+                    hub_role_name=hub_role_name,
+                    spoke_role_stack_name=spoke_role_name,
+                    spoke_role_name=spoke_role_name,
+                    tags=tags,
                 )
             )
             if not created_successfully:
                 log.error(
                     "Failed to create the required IAMbic role. Account not added."
                 )
                 return
 
         iambic_managed = (
             IambicManaged.IMPORT_ONLY if read_only else IambicManaged.READ_AND_WRITE
         )
         account = AWSAccount(
             account_id=account_id,
             account_name=account_name,
-            spoke_role_arn=get_spoke_role_arn(account_id),
+            spoke_role_arn=get_spoke_role_arn(account_id, role_name=spoke_role_name),
             iambic_managed=iambic_managed,
             aws_profile=profile_name,
             default_region=default_region,
         )
         if is_hub_account:
-            account.hub_role_arn = get_hub_role_arn(account_id)
+            account.hub_role_arn = get_hub_role_arn(account_id, role_name=hub_role_name)
         # account.partition = set_aws_account_partition(account.partition)
 
         confirm_command_exe("AWS Account", Operation.ADDED, requires_sync=requires_sync)
 
         self.config.aws.accounts.append(account)
 
         if is_hub_account:
@@ -1170,40 +1187,48 @@
             "If you have already manually deployed the templates, answer yes to proceed.\n"
             "IAMbic will validate that your stacks have been deployed successfully and will not attempt to replace them."
         )
         if not questionary.confirm("Proceed?").unsafe_ask():
             log.info("Unable to add the AWS Org without creating the required roles.")
             return
 
+        hub_role_name, spoke_role_name, tags = self.set_aws_cf_customization()
+
         created_successfully = asyncio.run(
             create_iambic_role_stacks(
                 cf_client=session.client(
                     "cloudformation", region_name=self.aws_default_region
                 ),
                 hub_account_id=account_id,
                 assume_as_arn=assume_as_arn,
                 role_arn=cf_role_arn,
                 org_client=session.client(
                     "organizations", region_name=self.aws_default_region
                 ),
                 read_only=read_only,
+                hub_role_stack_name=hub_role_name,
+                hub_role_name=hub_role_name,
+                spoke_role_stack_name=spoke_role_name,
+                spoke_role_name=spoke_role_name,
+                tags=tags,
             )
         )
         if not created_successfully:
             log.error("Failed to create the required IAMbic roles. Exiting.")
             sys.exit(0)
 
         aws_org = AWSOrganization(
             org_id=org_id,
             org_account_id=account_id,
             default_rule=BaseAWSOrgRule(),
-            hub_role_arn=get_hub_role_arn(account_id),
+            hub_role_arn=get_hub_role_arn(account_id, role_name=hub_role_name),
             aws_profile=profile_name,
             spoke_role_is_read_only=read_only,
             default_region=self.aws_default_region,
+            preferred_spoke_role_name=spoke_role_name,
         )
         if self.config.aws.spoke_role_is_read_only:
             aws_org.default_rule.iambic_managed = IambicManaged.IMPORT_ONLY
         else:
             aws_org.default_rule.iambic_managed = IambicManaged.READ_AND_WRITE
 
         self.config.aws.organizations.append(aws_org)
@@ -1781,14 +1806,38 @@
                 repo_dir=self.repo_dir,
                 repo_name=repo_name,
                 commit_email=commit_email,
                 assume_role_arn=self.config.aws.hub_role_arn,
                 region=region,
             )
 
+    def set_aws_cf_customization(self):
+        hub_role_name = IAMBIC_HUB_ROLE_NAME
+        spoke_role_name = IAMBIC_SPOKE_ROLE_NAME
+        if self._is_more_options:
+            input_hub_role_name = questionary.text(
+                "(Optional) Iambic Hub Role Name: ",
+                default="",
+            ).unsafe_ask()
+            input_spoke_role_name = questionary.text(
+                "(Optional) Iambic Spoke Role Name: ",
+                default="",
+            ).unsafe_ask()
+            if input_hub_role_name:
+                hub_role_name = input_hub_role_name
+            if input_spoke_role_name:
+                spoke_role_name = input_spoke_role_name
+        unparse_tags = questionary.text(
+            "Add Tags (leave blank or `team=ops_team, cost_center=engineering`): ",
+            default="",
+            validate=validate_aws_cf_input_tags,
+        ).ask()
+        tags = aws_cf_parse_key_value_string(unparse_tags)
+        return hub_role_name, spoke_role_name, tags
+
     def configuration_wizard_change_detection_setup(self, aws_org: AWSOrganization):
         click.echo(
             "\nTo setup change detection for iambic it requires creating CloudFormation stacks "
             "and a CloudFormation stack set.\n"
             "To review the templates used or deploy them manually, the IdentityRule templates used can be found here:\n"
             "https://github.com/noqdev/iambic/tree/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates\n"
             "If you have already manually deployed the templates, answer yes to proceed.\n"
```

### Comparing `iambic_core-0.6.3/iambic/core/aio_utils/__init__.py` & `iambic_core-0.7.1/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/exceptions.py` & `iambic_core-0.7.1/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/git.py` & `iambic_core-0.7.1/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/iambic_enum.py` & `iambic_core-0.7.1/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/iambic_plugin.py` & `iambic_core-0.7.1/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/logger.py` & `iambic_core-0.7.1/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/models.py` & `iambic_core-0.7.1/iambic/core/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/noq_json.py` & `iambic_core-0.7.1/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/parser.py` & `iambic_core-0.7.1/iambic/core/parser.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/template_generation.py` & `iambic_core-0.7.1/iambic/core/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/core/utils.py` & `iambic_core-0.7.1/iambic/core/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.7.1/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.7.1/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.7.1/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/github/templates/iambic-import.yml` & `iambic_core-0.7.1/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/github/utils.py` & `iambic_core-0.7.1/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/lambda/app.py` & `iambic_core-0.7.1/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/main.py` & `iambic_core-0.7.1/iambic/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,15 +457,23 @@
     "-d",
     "repo_dir",
     required=False,
     type=click.Path(exists=True),
     default=os.getenv("IAMBIC_REPO_DIR"),
     help="The repo directory. Example: ~/iambic-templates",
 )
-def setup(repo_dir: str):
+@click.option(
+    "--more-options",
+    "is_more_options",
+    is_flag=True,
+    hidden=True,
+    default=False,
+    help="If enabled, wizard will ask more questions",
+)
+def setup(repo_dir: str, is_more_options: bool):
     ctx.command = Command.APPLY
-    ConfigurationWizard(repo_dir).run()
+    ConfigurationWizard(repo_dir, is_more_options=is_more_options).run()
 
 
 if __name__ == "__main__":
     init_writable_directory()
     cli()
```

### Comparing `iambic_core-0.6.3/iambic/output/__init__.py` & `iambic_core-0.7.1/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/output/filters.py` & `iambic_core-0.7.1/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/output/models.py` & `iambic_core-0.7.1/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.7.1/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.7.1/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.7.1/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/output/text.py` & `iambic_core-0.7.1/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/README.md` & `iambic_core-0.7.1/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -318,118 +318,179 @@
 
 
 async def create_spoke_role_stack_set(
     cf_client,
     org_client,
     hub_account_id: str,
     read_only=False,
+    stack_set_name=IAMBIC_SPOKE_ROLE_NAME,
+    hub_role_name=IAMBIC_HUB_ROLE_NAME,
+    spoke_role_name=IAMBIC_SPOKE_ROLE_NAME,
+    tags=None,
 ) -> bool:
+    """Create stack instances in the member accounts.
+    This does not have special handling for delegated
+    administrator membership account.
+    TODO: If the org has delegated administrator account,
+    the IambicHubRole should be installed on delegated
+    administrator account.
+    """
     region = cf_client.meta.region_name
     org_roots = await legacy_paginated_search(
         org_client.list_roots, response_key="Roots"
     )
 
+    kwargs = {}
+
+    if tags:
+        kwargs["Tags"] = tags
+
     return await create_stack_set(
         cf_client,
-        stack_set_name="IambicSpokeRole",
+        stack_set_name=stack_set_name,
         template_body=get_iambic_spoke_role_template_body(read_only=read_only),
         parameters=[
             {
                 "ParameterKey": "HubRoleArn",
-                "ParameterValue": get_hub_role_arn(hub_account_id),
+                "ParameterValue": get_hub_role_arn(
+                    hub_account_id, role_name=hub_role_name
+                ),
             },
-            {"ParameterKey": "SpokeRoleName", "ParameterValue": IAMBIC_SPOKE_ROLE_NAME},
+            {"ParameterKey": "SpokeRoleName", "ParameterValue": spoke_role_name},
         ],
         deployment_targets={
             "OrganizationalUnitIds": [root["Id"] for root in org_roots],
             "AccountFilterType": "NONE",
         },
         deployment_regions=[region],
         operation_preferences={
             "RegionConcurrencyType": "PARALLEL",
             "MaxConcurrentCount": 10,
             "FailureToleranceCount": 10,
         },
         Capabilities=["CAPABILITY_NAMED_IAM"],
+        **kwargs,
     )
 
 
 async def create_spoke_role_stack(
     cf_client,
     hub_account_id: str,
     role_arn: str = None,
     read_only=False,
+    stack_name=IAMBIC_SPOKE_ROLE_NAME,
+    hub_role_name=IAMBIC_HUB_ROLE_NAME,
+    spoke_role_name=IAMBIC_SPOKE_ROLE_NAME,
+    tags=None,
 ) -> bool:
     additional_kwargs = {"RoleARN": role_arn} if role_arn else {}
+    if tags:
+        additional_kwargs["Tags"] = tags
     return await create_stack(
         cf_client,
-        stack_name="IambicSpokeRole",
+        stack_name=stack_name,
         template_body=get_iambic_spoke_role_template_body(read_only=read_only),
         parameters=[
             {
                 "ParameterKey": "HubRoleArn",
-                "ParameterValue": get_hub_role_arn(hub_account_id),
+                "ParameterValue": get_hub_role_arn(
+                    hub_account_id, role_name=hub_role_name
+                ),
             },
             {
                 "ParameterKey": "SpokeRoleName",
-                "ParameterValue": IAMBIC_SPOKE_ROLE_NAME,
+                "ParameterValue": spoke_role_name,
             },
         ],
         Capabilities=["CAPABILITY_NAMED_IAM"],
         **additional_kwargs,
     )
 
 
-async def create_hub_role_stack(
+async def create_hub_account_stacks(
     cf_client,
     hub_account_id: str,
     assume_as_arn: str,
     role_arn: str = None,
+    read_only=False,
+    stack_name=IAMBIC_HUB_ROLE_NAME,
+    hub_role_name=IAMBIC_HUB_ROLE_NAME,
+    spoke_role_name=IAMBIC_SPOKE_ROLE_NAME,
+    tags=None,
 ) -> bool:
+    """Create IambicHubRole and IambicSpokeRole in hub account"""
     additional_kwargs = {"RoleARN": role_arn} if role_arn else {}
+    if tags:
+        additional_kwargs["Tags"] = tags
+
     stack_created = await create_stack(
         cf_client,
-        stack_name="IambicHubRole",
+        stack_name=stack_name,
         template_body=get_iambic_hub_role_template_body(),
         parameters=[
-            {"ParameterKey": "HubRoleName", "ParameterValue": IAMBIC_HUB_ROLE_NAME},
+            {"ParameterKey": "HubRoleName", "ParameterValue": hub_role_name},
             {
                 "ParameterKey": "SpokeRoleName",
-                "ParameterValue": IAMBIC_SPOKE_ROLE_NAME,
+                "ParameterValue": spoke_role_name,
             },
             {"ParameterKey": "AssumeAsArn", "ParameterValue": assume_as_arn},
         ],
         Capabilities=["CAPABILITY_NAMED_IAM"],
         **additional_kwargs,
     )
     if stack_created:
-        return await create_spoke_role_stack(cf_client, hub_account_id, role_arn)
+        return await create_spoke_role_stack(
+            cf_client,
+            hub_account_id,
+            role_arn,
+            read_only=read_only,
+            stack_name=spoke_role_name,
+            hub_role_name=hub_role_name,
+            spoke_role_name=spoke_role_name,
+        )
 
     return stack_created
 
 
 async def create_iambic_role_stacks(
     cf_client,
     hub_account_id: str,
     assume_as_arn: str,
     role_arn: str = None,
     org_client=None,
     read_only=False,
+    hub_role_stack_name=IAMBIC_HUB_ROLE_NAME,
+    hub_role_name=IAMBIC_HUB_ROLE_NAME,
+    spoke_role_stack_name=IAMBIC_SPOKE_ROLE_NAME,
+    spoke_role_name=IAMBIC_SPOKE_ROLE_NAME,
+    tags=None,
 ) -> bool:
-    hub_role_created = await create_hub_role_stack(
+    hub_role_created = await create_hub_account_stacks(
         cf_client,
         hub_account_id,
         assume_as_arn,
         role_arn,
+        read_only=read_only,
+        stack_name=hub_role_stack_name,
+        hub_role_name=hub_role_name,
+        spoke_role_name=spoke_role_name,
+        tags=tags,
     )
     region = cf_client.meta.region_name
     if hub_role_created and org_client:
         log.info(
             f"WARNING: Do not exit; creating stack instances.\n"
             f"You can check the progress here:\n"
-            f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacksets/IambicSpokeRole/stacks\n"
+            f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacksets/{spoke_role_name}/stacks\n"
         )
         return await create_spoke_role_stack_set(
-            cf_client, org_client, hub_account_id, read_only=read_only
+            cf_client,
+            org_client,
+            hub_account_id,
+            read_only=read_only,
+            stack_set_name=spoke_role_stack_name,
+            hub_role_name=hub_role_name,
+            spoke_role_name=spoke_role_name,
+            tags=tags,
         )
 
     return hub_role_created
```

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,24 @@
 
 ARN_RE = r"(^arn:([^:]*):([^:]*):([^:]*):(|\*|[\d]{12}|cloudfront|aws|{{var.account_id}}):(.+)$)|^\*$"
 
 IAMBIC_HUB_ROLE_NAME = "IambicHubRole"
 IAMBIC_SPOKE_ROLE_NAME = "IambicSpokeRole"
 
 
-def get_hub_role_arn(account_id: str) -> str:
-    return f"arn:aws:iam::{account_id}:role/{IAMBIC_HUB_ROLE_NAME}"
+def get_hub_role_arn(account_id: str, role_name=None) -> str:
+    if not role_name:
+        role_name = IAMBIC_HUB_ROLE_NAME
+    return f"arn:aws:iam::{account_id}:role/{role_name}"
 
 
-def get_spoke_role_arn(account_id: str) -> str:
-    return f"arn:aws:iam::{account_id}:role/{IAMBIC_SPOKE_ROLE_NAME}"
+def get_spoke_role_arn(account_id: str, role_name=None) -> str:
+    if not role_name:
+        role_name = IAMBIC_SPOKE_ROLE_NAME
+    return f"arn:aws:iam::{account_id}:role/{role_name}"
 
 
 @yaml_object(yaml)
 class Partition(Enum):
     AWS = "aws"
     AWS_GOV = "aws-us-gov"
     AWS_CHINA = "aws-cn"
@@ -584,14 +588,18 @@
     hub_role_arn: str = Field(
         description="The role arn to assume into when making calls to the account",
     )
     spoke_role_is_read_only: bool = Field(
         False,
         description="if true, the spoke role will be limited to read-only permissions",
     )
+    preferred_spoke_role_name: Optional[str] = Field(
+        IAMBIC_SPOKE_ROLE_NAME,
+        description="SpokeRoleName use across organization",
+    )
 
     async def _create_org_account_instance(
         self, account: dict, session: boto3.Session
     ) -> Optional[AWSAccount]:
         """Create an AWSAccount instance from an AWS Organization account and account dict
 
         Evaluate rules to determine if the account should be added to the config and if it is a read-only account.
@@ -618,15 +626,17 @@
         aws_account = AWSAccount(
             account_id=account_id,
             account_name=account_name,
             org_id=self.org_id,
             variables=account["variables"],
             identity_center_details=identity_center_details,
             iambic_managed=account_rule.iambic_managed,
-            spoke_role_arn=get_spoke_role_arn(account_id),
+            spoke_role_arn=get_spoke_role_arn(
+                account_id, role_name=self.preferred_spoke_role_name
+            ),
             hub_session_info=dict(boto3_session=session),
             default_region=region_name,
             boto3_session_map={},
         )
         try:
             await aws_account.get_boto3_session()
             return aws_account
```

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.7.1/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/request_handler/expire_resources.py` & `iambic_core-0.7.1/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/request_handler/git_apply.py` & `iambic_core-0.7.1/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/request_handler/git_plan.py` & `iambic_core-0.7.1/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.7.1/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.7.1/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.6.3/pyproject.toml` & `iambic_core-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.6.3"
+version = "0.7.1"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.6.3/PKG-INFO` & `iambic_core-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.6.3
+Version: 0.7.1
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

