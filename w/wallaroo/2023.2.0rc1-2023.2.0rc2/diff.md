# Comparing `tmp/wallaroo-2023.2.0rc1.tar.gz` & `tmp/wallaroo-2023.2.0rc2.tar.gz`

## Comparing `wallaroo-2023.2.0rc1.tar` & `wallaroo-2023.2.0rc2.tar`

### file list

```diff
@@ -1,1478 +1,1480 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/.DS_Store
--rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/.coverage
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/Dockerfile
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/Makefile
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/README.md
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/_version.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/mypy.ini
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/pytest.ini
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/requirements.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/.gitignore
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/make.bat
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/autoscaling.ipynb
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/conf.py
--rw-r--r--   0        0        0    16542 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/core-abstractions.ipynb
--rw-r--r--   0        0        0    97557 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/email.png
--rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/experiments.ipynb
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/index.rst
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/jupyter.md
--rw-r--r--   0        0        0  1202751 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model-insights.ipynb
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion.rst
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion_keras.ipynb
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion_sklearn.ipynb
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion_xgboost.ipynb
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/models.ipynb
--rw-r--r--   0        0        0    36022 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/monitoring.ipynb
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/overview.md
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/python-processing.ipynb
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/sdk.rst
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/single-sign-on.md
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/standalone-mode.ipynb
--rw-r--r--   0        0        0    16569 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/workspaces.ipynb
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/BikeShareRegressor.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/demand_curve.pickle
--rw-r--r--   0        0        0    55124 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/isolet_xgboost_model.pickle
--rw-r--r--   0        0        0   339061 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/pytorch_bikesharingmodel.pt
--rw-r--r--   0        0        0    16201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/sentiment_model.zip
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/doc_app.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/index.html
--rw-r--r--   0        0        0  2325894 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/search.js
--rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo.html
--rw-r--r--   0        0        0    45048 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/ModelConversion.html
--rw-r--r--   0        0        0    37610 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/assay.html
--rw-r--r--   0        0        0    92157 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/assay_config.html
--rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/auth.html
--rw-r--r--   0        0        0    41365 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/checks.html
--rw-r--r--   0        0        0    86995 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/client.html
--rw-r--r--   0        0        0    25318 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/comment.html
--rw-r--r--   0        0        0    28571 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/connection.html
--rw-r--r--   0        0        0    20833 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/datasizeunit.html
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/deployment.html
--rw-r--r--   0        0        0    33510 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/deployment_config.html
--rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/engine_config.html
--rw-r--r--   0        0        0    61794 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/explainability.html
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/expression.html
--rw-r--r--   0        0        0    33076 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/framework.html
--rw-r--r--   0        0        0    17152 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/functions.html
--rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/graphql.html
--rw-r--r--   0        0        0    25039 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/inference_decode.html
--rw-r--r--   0        0        0    23185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/inference_result.html
--rw-r--r--   0        0        0    23071 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/logs.html
--rw-r--r--   0        0        0    35292 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/model.html
--rw-r--r--   0        0        0    25359 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/model_config.html
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/models.html
--rw-r--r--   0        0        0    23083 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/notify.html
--rw-r--r--   0        0        0    39062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/object.html
--rw-r--r--   0        0        0    37539 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/orchestration.html
--rw-r--r--   0        0        0    70395 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/pipeline.html
--rw-r--r--   0        0        0    99309 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/pipeline_config.html
--rw-r--r--   0        0        0    27690 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/pipeline_variant.html
--rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/queries.html
--rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/records.html
--rw-r--r--   0        0        0    22344 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/standalone_client.html
--rw-r--r--   0        0        0    26746 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/tag.html
--rw-r--r--   0        0        0    26135 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/task.html
--rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/unwrap.html
--rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/user.html
--rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/user_type.html
--rw-r--r--   0        0        0    24899 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/utils.html
--rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/version.html
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/visibility.html
--rw-r--r--   0        0        0    30345 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client.html
--rw-r--r--   0        0        0    30487 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/workspace.html
--rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/graphql/Assays.html
--rw-r--r--   0        0        0    17176 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/graphql/Workspaces.html
--rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/graphql/explainability.html
--rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/graphql/models.html
--rw-r--r--   0        0        0    17164 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/graphql/orch.html
--rw-r--r--   0        0        0    17174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/graphql/pipelines.html
--rw-r--r--   0        0        0    17166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/graphql/tasks.html
--rw-r--r--   0        0        0    31550 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/records/convert_keras_model.html
--rw-r--r--   0        0        0    17186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/records/graphql_queries.html
--rw-r--r--   0        0        0    42591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/records/telemetry_body.html
--rw-r--r--   0        0        0    22224 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/records/telemetry_error.html
--rw-r--r--   0        0        0    30662 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/records/v1_metric_response.html
--rw-r--r--   0        0        0    22631 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/records/v1_tls_response.html
--rw-r--r--   0        0        0    35762 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api.html
--rw-r--r--   0        0        0    91511 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/client.html
--rw-r--r--   0        0        0   251776 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models.html
--rw-r--r--   0        0        0    57883 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/types.html
--rw-r--r--   0        0        0    34852 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin.html
--rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay.html
--rw-r--r--   0        0        0    35695 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability.html
--rw-r--r--   0        0        0    34792 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc.html
--rw-r--r--   0        0        0    35222 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model.html
--rw-r--r--   0        0        0    34996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline.html
--rw-r--r--   0        0        0    34842 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau.html
--rw-r--r--   0        0        0    35099 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task.html
--rw-r--r--   0        0        0    34932 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user.html
--rw-r--r--   0        0        0    35100 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace.html
--rw-r--r--   0        0        0   103915 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.html
--rw-r--r--   0        0        0   103903 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.html
--rw-r--r--   0        0        0    96536 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.html
--rw-r--r--   0        0        0    94546 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.html
--rw-r--r--   0        0        0    94354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.html
--rw-r--r--   0        0        0   102532 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.html
--rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_results.html
--rw-r--r--   0        0        0    98489 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.html
--rw-r--r--   0        0        0   101224 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.html
--rw-r--r--   0        0        0   102809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.html
--rw-r--r--   0        0        0    97798 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.html
--rw-r--r--   0        0        0   104246 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.html
--rw-r--r--   0        0        0   105823 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.html
--rw-r--r--   0        0        0   101555 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.html
--rw-r--r--   0        0        0   101740 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.html
--rw-r--r--   0        0        0   101327 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.html
--rw-r--r--   0        0        0    90484 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.html
--rw-r--r--   0        0        0    95036 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.html
--rw-r--r--   0        0        0   106882 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.html
--rw-r--r--   0        0        0   104529 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.html
--rw-r--r--   0        0        0    77244 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.html
--rw-r--r--   0        0        0   101018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.html
--rw-r--r--   0        0        0    96704 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.html
--rw-r--r--   0        0        0    96492 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.html
--rw-r--r--   0        0        0   100867 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.html
--rw-r--r--   0        0        0    97263 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.html
--rw-r--r--   0        0        0   117840 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.html
--rw-r--r--   0        0        0    98796 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.html
--rw-r--r--   0        0        0    99321 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.html
--rw-r--r--   0        0        0    99309 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.html
--rw-r--r--   0        0        0    97607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.html
--rw-r--r--   0        0        0    97511 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.html
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.html
--rw-r--r--   0        0        0   100741 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.html
--rw-r--r--   0        0        0    98851 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.html
--rw-r--r--   0        0        0    97387 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_id.html
--rw-r--r--   0        0        0    98563 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status.html
--rw-r--r--   0        0        0   101796 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status_and_workspace.html
--rw-r--r--   0        0        0    99500 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_workspace.html
--rw-r--r--   0        0        0    90132 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_update.html
--rw-r--r--   0        0        0    97111 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.html
--rw-r--r--   0        0        0    97527 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.html
--rw-r--r--   0        0        0    97283 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.html
--rw-r--r--   0        0        0    96571 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.html
--rw-r--r--   0        0        0    98574 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.html
--rw-r--r--   0        0        0    97932 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.html
--rw-r--r--   0        0        0    97500 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.html
--rw-r--r--   0        0        0   100083 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.html
--rw-r--r--   0        0        0    99319 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.html
--rw-r--r--   0        0        0    80018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.html
--rw-r--r--   0        0        0    75031 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.html
--rw-r--r--   0        0        0    80018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.html
--rw-r--r--   0        0        0    75031 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.html
--rw-r--r--   0        0        0   247398 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.html
--rw-r--r--   0        0        0    77057 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.html
--rw-r--r--   0        0        0    76000 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    76698 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.html
--rw-r--r--   0        0        0    89869 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    76792 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.html
--rw-r--r--   0        0        0    90314 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   137892 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.html
--rw-r--r--   0        0        0    48283 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    49047 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    47768 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    45477 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.html
--rw-r--r--   0        0        0    81740 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.html
--rw-r--r--   0        0        0    45501 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.html
--rw-r--r--   0        0        0   108406 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.html
--rw-r--r--   0        0        0    72211 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.html
--rw-r--r--   0        0        0   116441 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.html
--rw-r--r--   0        0        0    82564 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.html
--rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.html
--rw-r--r--   0        0        0   255712 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.html
--rw-r--r--   0        0        0    78641 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.html
--rw-r--r--   0        0        0    77371 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    78282 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.html
--rw-r--r--   0        0        0    91786 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    78376 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.html
--rw-r--r--   0        0        0    92231 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   141854 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    48924 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    49737 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    48409 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46020 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    83506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    46044 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   110939 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.html
--rw-r--r--   0        0        0    87219 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.html
--rw-r--r--   0        0        0   225352 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.html
--rw-r--r--   0        0        0   179675 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.html
--rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.html
--rw-r--r--   0        0        0    49043 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.html
--rw-r--r--   0        0        0   146962 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    49751 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    50627 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    49236 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46721 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    85788 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    46745 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   178307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.html
--rw-r--r--   0        0        0    49565 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.html
--rw-r--r--   0        0        0    78631 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.html
--rw-r--r--   0        0        0   110252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.html
--rw-r--r--   0        0        0    68384 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_200_item.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.html
--rw-r--r--   0        0        0   104659 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_json_body.html
--rw-r--r--   0        0        0   220093 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item.html
--rw-r--r--   0        0        0   176239 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary.html
--rw-r--r--   0        0        0    49288 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary_aggregation.html
--rw-r--r--   0        0        0    48549 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_status.html
--rw-r--r--   0        0        0   144127 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    50133 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    48777 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46332 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    84522 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    46356 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   174871 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary.html
--rw-r--r--   0        0        0    49106 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary_aggregation.html
--rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_400.html
--rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_401.html
--rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_500.html
--rw-r--r--   0        0        0    74300 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.html
--rw-r--r--   0        0        0   268583 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.html
--rw-r--r--   0        0        0    78193 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.html
--rw-r--r--   0        0        0    76983 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    77834 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.html
--rw-r--r--   0        0        0    91242 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    77928 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.html
--rw-r--r--   0        0        0    91687 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   140730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    49541 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    48227 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    83006 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    45890 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   110339 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.html
--rw-r--r--   0        0        0   267313 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.html
--rw-r--r--   0        0        0    80673 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.html
--rw-r--r--   0        0        0    79130 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    80314 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.html
--rw-r--r--   0        0        0    94247 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    80408 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.html
--rw-r--r--   0        0        0    94692 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   146937 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.html
--rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    50623 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    49232 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46717 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.html
--rw-r--r--   0        0        0    85772 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.html
--rw-r--r--   0        0        0    46741 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.html
--rw-r--r--   0        0        0   114192 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.html
--rw-r--r--   0        0        0    69546 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.html
--rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.html
--rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.html
--rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.html
--rw-r--r--   0        0        0   257261 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.html
--rw-r--r--   0        0        0    78865 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.html
--rw-r--r--   0        0        0    77565 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    78506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.html
--rw-r--r--   0        0        0    92058 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    78600 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.html
--rw-r--r--   0        0        0    92503 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   142416 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.html
--rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    49835 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    48500 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46097 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.html
--rw-r--r--   0        0        0    83756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.html
--rw-r--r--   0        0        0    46121 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.html
--rw-r--r--   0        0        0   111299 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.html
--rw-r--r--   0        0        0   224337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.html
--rw-r--r--   0        0        0   178975 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.html
--rw-r--r--   0        0        0    49652 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.html
--rw-r--r--   0        0        0    48941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.html
--rw-r--r--   0        0        0   146375 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    49656 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    50525 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    49141 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46640 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    85522 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    46664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   177607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.html
--rw-r--r--   0        0        0    49470 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.html
--rw-r--r--   0        0        0    76814 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.html
--rw-r--r--   0        0        0    77468 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.html
--rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.html
--rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.html
--rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.html
--rw-r--r--   0        0        0   156808 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.html
--rw-r--r--   0        0        0    79738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.html
--rw-r--r--   0        0        0    69201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.html
--rw-r--r--   0        0        0   159996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.html
--rw-r--r--   0        0        0    96970 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.html
--rw-r--r--   0        0        0    96196 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.html
--rw-r--r--   0        0        0    69367 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.html
--rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.html
--rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.html
--rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.html
--rw-r--r--   0        0        0    74075 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.html
--rw-r--r--   0        0        0    68703 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.html
--rw-r--r--   0        0        0    74305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.html
--rw-r--r--   0        0        0    68869 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.html
--rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.html
--rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.html
--rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.html
--rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.html
--rw-r--r--   0        0        0    68703 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.html
--rw-r--r--   0        0        0    74445 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.html
--rw-r--r--   0        0        0    76003 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.html
--rw-r--r--   0        0        0    71398 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.html
--rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.html
--rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.html
--rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.html
--rw-r--r--   0        0        0    69712 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.html
--rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.html
--rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.html
--rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.html
--rw-r--r--   0        0        0    74738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.html
--rw-r--r--   0        0        0    69878 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.html
--rw-r--r--   0        0        0    84036 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.html
--rw-r--r--   0        0        0    68211 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.html
--rw-r--r--   0        0        0    70842 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.html
--rw-r--r--   0        0        0   110748 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.html
--rw-r--r--   0        0        0   114100 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.html
--rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.html
--rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.html
--rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.html
--rw-r--r--   0        0        0    71360 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.html
--rw-r--r--   0        0        0    81687 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.html
--rw-r--r--   0        0        0    99356 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.html
--rw-r--r--   0        0        0    83498 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.html
--rw-r--r--   0        0        0   115258 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.html
--rw-r--r--   0        0        0   105405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.html
--rw-r--r--   0        0        0    46114 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.html
--rw-r--r--   0        0        0    86971 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.html
--rw-r--r--   0        0        0    85711 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.html
--rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.html
--rw-r--r--   0        0        0    78923 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.html
--rw-r--r--   0        0        0    88601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.html
--rw-r--r--   0        0        0    87371 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.html
--rw-r--r--   0        0        0    90725 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.html
--rw-r--r--   0        0        0    80112 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.html
--rw-r--r--   0        0        0    45522 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.html
--rw-r--r--   0        0        0   119549 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.html
--rw-r--r--   0        0        0    70280 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.html
--rw-r--r--   0        0        0   107861 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.html
--rw-r--r--   0        0        0    75696 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.html
--rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.html
--rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.html
--rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.html
--rw-r--r--   0        0        0    96500 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.html
--rw-r--r--   0        0        0    68859 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.html
--rw-r--r--   0        0        0    83809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.html
--rw-r--r--   0        0        0   155198 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.html
--rw-r--r--   0        0        0    69238 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.html
--rw-r--r--   0        0        0    83368 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.html
--rw-r--r--   0        0        0    72567 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.html
--rw-r--r--   0        0        0    83727 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.html
--rw-r--r--   0        0        0    67694 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.html
--rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.html
--rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.html
--rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.html
--rw-r--r--   0        0        0    83009 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.html
--rw-r--r--   0        0        0    75223 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.html
--rw-r--r--   0        0        0    91489 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.html
--rw-r--r--   0        0        0    73642 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.html
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.html
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.html
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.html
--rw-r--r--   0        0        0    72867 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.html
--rw-r--r--   0        0        0   146363 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.html
--rw-r--r--   0        0        0    79269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.html
--rw-r--r--   0        0        0   143833 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.html
--rw-r--r--   0        0        0    48904 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.html
--rw-r--r--   0        0        0    72317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.html
--rw-r--r--   0        0        0    51426 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.html
--rw-r--r--   0        0        0   122335 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.html
--rw-r--r--   0        0        0   142755 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.html
--rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.html
--rw-r--r--   0        0        0    71968 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.html
--rw-r--r--   0        0        0    51212 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.html
--rw-r--r--   0        0        0    72505 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.html
--rw-r--r--   0        0        0    73018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.html
--rw-r--r--   0        0        0    78096 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.html
--rw-r--r--   0        0        0   141171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.html
--rw-r--r--   0        0        0    48445 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.html
--rw-r--r--   0        0        0    71464 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.html
--rw-r--r--   0        0        0    50897 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.html
--rw-r--r--   0        0        0    87540 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.html
--rw-r--r--   0        0        0   143811 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.html
--rw-r--r--   0        0        0    48900 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.html
--rw-r--r--   0        0        0    72304 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.html
--rw-r--r--   0        0        0    51422 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.html
--rw-r--r--   0        0        0    47341 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.html
--rw-r--r--   0        0        0    71728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.html
--rw-r--r--   0        0        0    67391 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.html
--rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.html
--rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.html
--rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.html
--rw-r--r--   0        0        0    72120 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.html
--rw-r--r--   0        0        0    67727 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.html
--rw-r--r--   0        0        0    79001 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.html
--rw-r--r--   0        0        0    76665 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.html
--rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.html
--rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.html
--rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.html
--rw-r--r--   0        0        0    81109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.html
--rw-r--r--   0        0        0    74260 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.html
--rw-r--r--   0        0        0    79975 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.html
--rw-r--r--   0        0        0    70389 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.html
--rw-r--r--   0        0        0    72475 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.html
--rw-r--r--   0        0        0    88028 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.html
--rw-r--r--   0        0        0   109802 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.html
--rw-r--r--   0        0        0    71831 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.html
--rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.html
--rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.html
--rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.html
--rw-r--r--   0        0        0    72851 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.html
--rw-r--r--   0        0        0   126961 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.html
--rw-r--r--   0        0        0   110890 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.html
--rw-r--r--   0        0        0    72361 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.html
--rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.html
--rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.html
--rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.html
--rw-r--r--   0        0        0    71840 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_json_body.html
--rw-r--r--   0        0        0    75030 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200.html
--rw-r--r--   0        0        0   279449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task.html
--rw-r--r--   0        0        0   235836 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item.html
--rw-r--r--   0        0        0    72127 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_error_data.html
--rw-r--r--   0        0        0    72293 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_output_data.html
--rw-r--r--   0        0        0    46678 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_0.html
--rw-r--r--   0        0        0    46642 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_1.html
--rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_2.html
--rw-r--r--   0        0        0    46786 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_3.html
--rw-r--r--   0        0        0    46726 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_4.html
--rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_5.html
--rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_6.html
--rw-r--r--   0        0        0    78265 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_7.html
--rw-r--r--   0        0        0    45405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_0.html
--rw-r--r--   0        0        0    45429 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_1.html
--rw-r--r--   0        0        0    74928 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_2.html
--rw-r--r--   0        0        0    45357 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_0.html
--rw-r--r--   0        0        0    45321 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_1.html
--rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_2.html
--rw-r--r--   0        0        0    45465 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_3.html
--rw-r--r--   0        0        0    45405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_4.html
--rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_5.html
--rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_6.html
--rw-r--r--   0        0        0    74928 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_7.html
--rw-r--r--   0        0        0    45455 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_0.html
--rw-r--r--   0        0        0    45575 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_1.html
--rw-r--r--   0        0        0    45491 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_2.html
--rw-r--r--   0        0        0    75329 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_3.html
--rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_400.html
--rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_401.html
--rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_500.html
--rw-r--r--   0        0        0   169074 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body.html
--rw-r--r--   0        0        0    46366 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_0.html
--rw-r--r--   0        0        0    46330 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_1.html
--rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_2.html
--rw-r--r--   0        0        0    46474 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_3.html
--rw-r--r--   0        0        0    46414 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_4.html
--rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_5.html
--rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_6.html
--rw-r--r--   0        0        0    77476 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_7.html
--rw-r--r--   0        0        0    87286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200.html
--rw-r--r--   0        0        0   129638 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item.html
--rw-r--r--   0        0        0    47034 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_0.html
--rw-r--r--   0        0        0    47058 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_1.html
--rw-r--r--   0        0        0    79041 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_2.html
--rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_400.html
--rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_401.html
--rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_500.html
--rw-r--r--   0        0        0   154233 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body.html
--rw-r--r--   0        0        0    45434 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_0.html
--rw-r--r--   0        0        0    45398 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_1.html
--rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_2.html
--rw-r--r--   0        0        0    45542 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_3.html
--rw-r--r--   0        0        0    45482 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_4.html
--rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_5.html
--rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_6.html
--rw-r--r--   0        0        0    75122 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_7.html
--rw-r--r--   0        0        0    83570 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200.html
--rw-r--r--   0        0        0   123274 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item.html
--rw-r--r--   0        0        0    46102 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_0.html
--rw-r--r--   0        0        0    46126 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_1.html
--rw-r--r--   0        0        0    76687 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_2.html
--rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_400.html
--rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_401.html
--rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_500.html
--rw-r--r--   0        0        0    73401 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_json_body.html
--rw-r--r--   0        0        0    84383 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200.html
--rw-r--r--   0        0        0   219068 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item.html
--rw-r--r--   0        0        0    46333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_0.html
--rw-r--r--   0        0        0    46357 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_1.html
--rw-r--r--   0        0        0    77269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_2.html
--rw-r--r--   0        0        0    46285 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_0.html
--rw-r--r--   0        0        0    46249 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_1.html
--rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_2.html
--rw-r--r--   0        0        0    46393 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_3.html
--rw-r--r--   0        0        0    46333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_4.html
--rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_5.html
--rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_6.html
--rw-r--r--   0        0        0    77269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_7.html
--rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_400.html
--rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_401.html
--rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_500.html
--rw-r--r--   0        0        0   129869 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body.html
--rw-r--r--   0        0        0    69164 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_additional_data.html
--rw-r--r--   0        0        0    68285 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_error_data.html
--rw-r--r--   0        0        0    50899 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_status.html
--rw-r--r--   0        0        0    74827 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200.html
--rw-r--r--   0        0        0   164435 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data.html
--rw-r--r--   0        0        0    45272 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_0.html
--rw-r--r--   0        0        0    45236 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_1.html
--rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_2.html
--rw-r--r--   0        0        0    45380 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_3.html
--rw-r--r--   0        0        0    45320 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_4.html
--rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_5.html
--rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_6.html
--rw-r--r--   0        0        0    74708 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_7.html
--rw-r--r--   0        0        0    76620 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_500.html
--rw-r--r--   0        0        0   102591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.html
--rw-r--r--   0        0        0    68109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.html
--rw-r--r--   0        0        0    72650 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.html
--rw-r--r--   0        0        0    73154 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.html
--rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.html
--rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.html
--rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.html
--rw-r--r--   0        0        0    74934 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.html
--rw-r--r--   0        0        0    83034 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.html
--rw-r--r--   0        0        0   112145 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.html
--rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.html
--rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.html
--rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.html
--rw-r--r--   0        0        0    73182 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.html
--rw-r--r--   0        0        0    84128 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.html
--rw-r--r--   0        0        0    83709 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.html
--rw-r--r--   0        0        0    88686 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.html
--rw-r--r--   0        0        0    74176 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.html
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/pdoc_templates/frame.html.jinja2
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/pdoc_templates/module.html.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/__init__.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/reusable_responders.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/status_samples.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_assay.py
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_assay_config.py
--rw-r--r--   0        0        0    26551 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_auth.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_checks.py
--rw-r--r--   0        0        0    49739 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_client.py
--rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_comment.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_connection.py
--rw-r--r--   0        0        0    30118 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_deployment.py
--rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_deployment_config.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_engine_config.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_explainability.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_import.py
--rw-r--r--   0        0        0    21694 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_inference_result.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_log_entries.py
--rw-r--r--   0        0        0    20229 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_model.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_model_config.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_models.py
--rw-r--r--   0        0        0    20956 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_pipeline.py
--rw-r--r--   0        0        0    31774 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_pipeline_config.py
--rw-r--r--   0        0        0    14056 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_pipeline_variant.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_tag.py
--rw-r--r--   0        0        0    14900 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/test_workspace.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/testutil.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/.DS_Store
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/ccfraud_output.json
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/day5_output.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/dev_smoke_test.arrow
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/dev_smoke_test.pandas.json
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/dev_smoke_test.txt
--rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/lazyadam_output.json
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/pipeline_output.json
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/sample_batched_inference_result.json
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/sample_inference_result.arrow
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/sample_inference_result.json
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/sample_inference_result.pandas.json
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/sample_logged_inference_result.json
--rw-r--r--   0        0        0    32666 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/sample_logs.arrow
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/outputs/some_output.json
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_aggregate_function/aggregate.json
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_bounds_expression/bounds.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_bounds_expression/gauges.json
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_model_drift/drift.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_model_drift/gauges.json
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_values_expression/gauges.json
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_values_expression/values.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/default_model_config.yaml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/experiment_model_config.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_batch_config_pipeline/model_config.yaml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_batch_config_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/model_config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/model_config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/model_config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/post_model_config.yaml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/pre_model_config.yaml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/wl_model_config.yaml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/challenger.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/control.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/control.yaml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/model2.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/model3.yaml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_simple_pipeline/model_config.yaml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_simple_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_single_alert/alert.json
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_single_validation/single_validation.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_validate/single_validation.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_validation_placement/checked_pipeline.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/ModelConversion.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/__init__.py
--rw-r--r--   0        0        0    17522 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/assay.py
--rw-r--r--   0        0        0    28003 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/assay_config.py
--rw-r--r--   0        0        0    27397 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/auth.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/checks.py
--rw-r--r--   0        0        0    80813 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/client.py
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/comment.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/connection.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/datasizeunit.py
--rw-r--r--   0        0        0    30989 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/deployment.py
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/deployment_config.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/engine_config.py
--rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/explainability.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/expression.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/framework.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/functions.py
--rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/inference_decode.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/inference_result.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/logs.py
--rw-r--r--   0        0        0    17966 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/model.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/model_config.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/models.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/notify.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/object.py
--rw-r--r--   0        0        0    12348 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/orchestration.py
--rw-r--r--   0        0        0    36887 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/pipeline.py
--rw-r--r--   0        0        0    26383 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/pipeline_config.py
--rw-r--r--   0        0        0     8286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/pipeline_variant.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/queries.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/standalone_client.py
--rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/tag.py
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/task.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/unwrap.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/user.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/user_type.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/utils.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/version.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/visibility.py
--rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/workspace.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateConnection.graphql
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateDefaultUserWorkspace.graphql
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateDeployment.graphql
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreatePipelineWithDefinition.graphql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateTag.graphql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateWorkspace.graphql
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateWorkspaceBare.graphql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateWorkspaceConnection.graphql
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/DeleteConnection.graphql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/DeleteWorkspaceConnection.graphql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/DeleteWorkspaceUser.graphql
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetConfiguredModelById.graphql
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetConfiguredModelByTaskId.graphql
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetConnection.graphql
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetConnectionById.graphql
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetDeploymentForPipeline.graphql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModel.graphql
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModelById.graphql
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModelByTaskId.graphql
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModelConfigs.graphql
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModels.graphql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineAndWorkspace.graphql
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineByIdForCopying.graphql
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineByName.graphql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineVersion.graphql
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineVersionDeploymentDetails.graphql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelinesForModels.graphql
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertConfiguredModel.graphql
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertDeploymentModelConfig.graphql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertDeploymentModelConfigMultiple.graphql
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertDeploymentPipelineVersion.graphql
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertModel.graphql
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertModelConfig.graphql
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertModelConfigFull.graphql
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertWorkspaceUser.graphql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListConnections.graphql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListDeployments.graphql
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListModelConversions.graphql
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListModels.graphql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListPipelines.graphql
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListWorkspaces.graphql
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ModelByName.graphql
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/PipelineModels.graphql
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/PipelineVariantById.graphql
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/README.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Undeploy.graphql
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/UpdateModel.graphql
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/UpdateModelConversionMetaData.graphql
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/UserDefaultWorkspace.graphql
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/WorkspaceById.graphql
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/WorkspaceByName.graphql
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/WorkspaceListConnections.graphql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/WorkspaceNameById.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/AssaySetActive.graphql
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/CreateAssay.graphql
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/FilterAssays.graphql
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/GetAssayResults.graphql
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/ListAssays.graphql
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/ListAssaysWithPipeline.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/DeleteUsersFromWorkspace.graphql
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/GetUserWorkspacePermission.graphql
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/ListWorkspaceUsers.graphql
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/ListWorkspacesByUser.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetDeploymentPipelineVersion.graphql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetExplainabilityConfig.graphql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetExplainabilityConfigByReferencePipelineVersion.graphql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetExplainabilityRequest.graphql
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetPipelineByPipelineVersion.graphql
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetPipelineVersionVersion.graphql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/ListExplainabilityConfigs.graphql
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/ListExplainabilityConfigsByPipeline.graphql
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/ListExplainabilityRequests.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/GetLatestModelConfig.graphql
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/GetModel.graphql
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/GetModelVersions.graphql
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/GetModels.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/GetOrchestration.graphql
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/GetOrchestrationByTaskId.graphql
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/InsertOrchestration.graphql
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/ListOrchestrations.graphql
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/UpdateOrchestration.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/__init__.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/pipelines/GetPipelineDefinitionByNameAndVersion.graphql
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/pipelines/PipelineModelsFlat.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/pipelines/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/GetTaskById.graphql
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/GetTasksByStatus.graphql
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/GetTasksByStatusAndWorkspaceId.graphql
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/InsertTask.graphql
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/ListTasks.graphql
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/README.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/SetTaskKilled.graphql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/StartTaskRun.graphql
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/UpdateTask.graphql
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/UpdateTaskStatus.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/records/README.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/records/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/records/convert_keras_model.py
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/records/graphql_queries.py
--rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/records/telemetry_body.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/records/telemetry_error.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/records/v1_metric_response.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/records/v1_tls_response.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/__init__.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/client.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/errors.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/types.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/__init__.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.py
--rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/__init__.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.py
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.py
--rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.py
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/__init__.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_add_to_workspace.py
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_create.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_delete.py
--rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get.py
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get_by_id.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_list.py
--rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_remove_from_workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/__init__.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.py
--rw-r--r--   0        0        0     7982 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.py
--rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.py
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/__init__.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/__init__.py
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.py
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.py
--rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.py
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.py
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.py
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/__init__.py
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/get_by_id.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/list_.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/__init__.py
--rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.py
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_logs.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_version.py
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/__init__.py
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/__init__.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/cron_job.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_by_id1.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/kill.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/list1.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/network_service.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/oneshot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/__init__.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.py
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/__init__.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.py
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.py
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.py
--rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.py
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.py
--rw-r--r--   0        0        0    58651 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/__init__.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/arbex_status.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.py
--rw-r--r--   0        0        0    11372 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.py
--rw-r--r--   0        0        0     9367 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.py
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body_next.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.py
--rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.py
--rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.py
--rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.py
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.py
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_json_body.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_200.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_400.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_401.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_500.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body_details.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_200.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_400.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_401.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_500.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_json_body.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_400.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_401.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_500.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_json_body.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200_details.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_400.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_401.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_404.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_500.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_json_body.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200_details.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_400.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_401.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_404.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_500.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_json_body.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item_details.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_400.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_401.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_500.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_json_body.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_400.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_401.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_500.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_exec.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body_json.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request_json.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_response_201.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/event_base.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/event_base_extra_env_vars.py
--rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.py
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200_input_data.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_request.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_response.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_task_by_id_request.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/insert_task_response.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_request.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202_input_data.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_orchestrations_request.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_tasks_request.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_exec.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_request.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_request_json.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_response_201.py
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request_json.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_response_201.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/orchestration.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/orchestration_status.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body_order.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200_records.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200_status.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_400.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_401.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_500.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_json_body.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200_definition.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_400.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_401.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_500.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.py
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/task.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/task_input_data.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_request.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_response.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.py
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateConnection.graphql
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateDefaultUserWorkspace.graphql
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateDeployment.graphql
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreatePipelineWithDefinition.graphql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateTag.graphql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateWorkspace.graphql
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateWorkspaceBare.graphql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/CreateWorkspaceConnection.graphql
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/DeleteConnection.graphql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/DeleteWorkspaceConnection.graphql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/DeleteWorkspaceUser.graphql
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetConfiguredModelById.graphql
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetConfiguredModelByTaskId.graphql
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetConnection.graphql
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetConnectionById.graphql
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetDeploymentForPipeline.graphql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModel.graphql
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModelById.graphql
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModelByTaskId.graphql
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModelConfigs.graphql
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetModels.graphql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineAndWorkspace.graphql
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineByIdForCopying.graphql
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineByName.graphql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineVersion.graphql
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineVersionDeploymentDetails.graphql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelinesForModels.graphql
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertConfiguredModel.graphql
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertDeploymentModelConfig.graphql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertDeploymentModelConfigMultiple.graphql
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertDeploymentPipelineVersion.graphql
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertModel.graphql
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertModelConfig.graphql
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertModelConfigFull.graphql
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/InsertWorkspaceUser.graphql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListConnections.graphql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListDeployments.graphql
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListModelConversions.graphql
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListModels.graphql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListPipelines.graphql
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ListWorkspaces.graphql
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/ModelByName.graphql
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/PipelineModels.graphql
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/PipelineVariantById.graphql
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/README.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Undeploy.graphql
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/UpdateModel.graphql
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/UpdateModelConversionMetaData.graphql
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/UserDefaultWorkspace.graphql
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/WorkspaceById.graphql
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/WorkspaceByName.graphql
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/WorkspaceListConnections.graphql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/WorkspaceNameById.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/AssaySetActive.graphql
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/CreateAssay.graphql
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/FilterAssays.graphql
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/GetAssayResults.graphql
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/ListAssays.graphql
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/ListAssaysWithPipeline.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/DeleteUsersFromWorkspace.graphql
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/GetUserWorkspacePermission.graphql
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/ListWorkspaceUsers.graphql
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/ListWorkspacesByUser.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/Workspaces/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetDeploymentPipelineVersion.graphql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetExplainabilityConfig.graphql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetExplainabilityConfigByReferencePipelineVersion.graphql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetExplainabilityRequest.graphql
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetPipelineByPipelineVersion.graphql
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/GetPipelineVersionVersion.graphql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/ListExplainabilityConfigs.graphql
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/ListExplainabilityConfigsByPipeline.graphql
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/ListExplainabilityRequests.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/GetLatestModelConfig.graphql
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/GetModel.graphql
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/GetModelVersions.graphql
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/GetModels.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/models/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/GetOrchestration.graphql
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/GetOrchestrationByTaskId.graphql
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/InsertOrchestration.graphql
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/ListOrchestrations.graphql
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/UpdateOrchestration.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/orch/__init__.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/pipelines/GetPipelineDefinitionByNameAndVersion.graphql
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/pipelines/PipelineModelsFlat.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/pipelines/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/GetTaskById.graphql
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/GetTasksByStatus.graphql
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/GetTasksByStatusAndWorkspaceId.graphql
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/InsertTask.graphql
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/ListTasks.graphql
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/README.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/SetTaskKilled.graphql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/StartTaskRun.graphql
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/UpdateTask.graphql
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/UpdateTaskStatus.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/.gitignore
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/public_README.md
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/.DS_Store
+-rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/.coverage
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/Dockerfile
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/Makefile
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/README.md
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/_version.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/mypy.ini
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/pytest.ini
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/requirements.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/.gitignore
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/make.bat
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/autoscaling.ipynb
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/conf.py
+-rw-r--r--   0        0        0    16542 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/core-abstractions.ipynb
+-rw-r--r--   0        0        0    97557 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/email.png
+-rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/experiments.ipynb
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/index.rst
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/jupyter.md
+-rw-r--r--   0        0        0  1202751 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model-insights.ipynb
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion.rst
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion_keras.ipynb
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion_sklearn.ipynb
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion_xgboost.ipynb
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/models.ipynb
+-rw-r--r--   0        0        0    36022 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/monitoring.ipynb
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/overview.md
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/python-processing.ipynb
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/sdk.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/single-sign-on.md
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/standalone-mode.ipynb
+-rw-r--r--   0        0        0    16569 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/workspaces.ipynb
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/BikeShareRegressor.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/demand_curve.pickle
+-rw-r--r--   0        0        0    55124 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/isolet_xgboost_model.pickle
+-rw-r--r--   0        0        0   339061 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/pytorch_bikesharingmodel.pt
+-rw-r--r--   0        0        0    16201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/sentiment_model.zip
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/doc_app.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/index.html
+-rw-r--r--   0        0        0  2325894 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/search.js
+-rw-r--r--   0        0        0    17126 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo.html
+-rw-r--r--   0        0        0    45048 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/ModelConversion.html
+-rw-r--r--   0        0        0    37610 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/assay.html
+-rw-r--r--   0        0        0    92157 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/assay_config.html
+-rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/auth.html
+-rw-r--r--   0        0        0    41365 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/checks.html
+-rw-r--r--   0        0        0    86995 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/client.html
+-rw-r--r--   0        0        0    25318 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/comment.html
+-rw-r--r--   0        0        0    28571 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/connection.html
+-rw-r--r--   0        0        0    20833 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/datasizeunit.html
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/deployment.html
+-rw-r--r--   0        0        0    33510 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/deployment_config.html
+-rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/engine_config.html
+-rw-r--r--   0        0        0    61794 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/explainability.html
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/expression.html
+-rw-r--r--   0        0        0    33076 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/framework.html
+-rw-r--r--   0        0        0    17152 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/functions.html
+-rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/graphql.html
+-rw-r--r--   0        0        0    25039 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/inference_decode.html
+-rw-r--r--   0        0        0    23185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/inference_result.html
+-rw-r--r--   0        0        0    23071 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/logs.html
+-rw-r--r--   0        0        0    35292 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/model.html
+-rw-r--r--   0        0        0    25359 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/model_config.html
+-rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/models.html
+-rw-r--r--   0        0        0    23083 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/notify.html
+-rw-r--r--   0        0        0    39062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/object.html
+-rw-r--r--   0        0        0    37539 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/orchestration.html
+-rw-r--r--   0        0        0    70395 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/pipeline.html
+-rw-r--r--   0        0        0    99309 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/pipeline_config.html
+-rw-r--r--   0        0        0    27690 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/pipeline_variant.html
+-rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/queries.html
+-rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/records.html
+-rw-r--r--   0        0        0    22344 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/standalone_client.html
+-rw-r--r--   0        0        0    26746 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/tag.html
+-rw-r--r--   0        0        0    26135 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/task.html
+-rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/unwrap.html
+-rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/user.html
+-rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/user_type.html
+-rw-r--r--   0        0        0    24899 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/utils.html
+-rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/version.html
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/visibility.html
+-rw-r--r--   0        0        0    30345 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client.html
+-rw-r--r--   0        0        0    30487 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/workspace.html
+-rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/graphql/Assays.html
+-rw-r--r--   0        0        0    17176 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/graphql/Workspaces.html
+-rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/graphql/explainability.html
+-rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/graphql/models.html
+-rw-r--r--   0        0        0    17164 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/graphql/orch.html
+-rw-r--r--   0        0        0    17174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/graphql/pipelines.html
+-rw-r--r--   0        0        0    17166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/graphql/tasks.html
+-rw-r--r--   0        0        0    31550 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/records/convert_keras_model.html
+-rw-r--r--   0        0        0    17186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/records/graphql_queries.html
+-rw-r--r--   0        0        0    42591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/records/telemetry_body.html
+-rw-r--r--   0        0        0    22224 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/records/telemetry_error.html
+-rw-r--r--   0        0        0    30662 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/records/v1_metric_response.html
+-rw-r--r--   0        0        0    22631 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/records/v1_tls_response.html
+-rw-r--r--   0        0        0    35762 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api.html
+-rw-r--r--   0        0        0    91511 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/client.html
+-rw-r--r--   0        0        0   251776 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models.html
+-rw-r--r--   0        0        0    57883 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/types.html
+-rw-r--r--   0        0        0    34852 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin.html
+-rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay.html
+-rw-r--r--   0        0        0    35695 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability.html
+-rw-r--r--   0        0        0    34792 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc.html
+-rw-r--r--   0        0        0    35222 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model.html
+-rw-r--r--   0        0        0    34996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline.html
+-rw-r--r--   0        0        0    34842 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau.html
+-rw-r--r--   0        0        0    35099 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task.html
+-rw-r--r--   0        0        0    34932 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user.html
+-rw-r--r--   0        0        0    35100 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace.html
+-rw-r--r--   0        0        0   103915 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.html
+-rw-r--r--   0        0        0   103903 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.html
+-rw-r--r--   0        0        0    96536 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.html
+-rw-r--r--   0        0        0    94546 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.html
+-rw-r--r--   0        0        0    94354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.html
+-rw-r--r--   0        0        0   102532 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.html
+-rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_results.html
+-rw-r--r--   0        0        0    98489 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.html
+-rw-r--r--   0        0        0   101224 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.html
+-rw-r--r--   0        0        0   102809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.html
+-rw-r--r--   0        0        0    97798 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.html
+-rw-r--r--   0        0        0   104246 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.html
+-rw-r--r--   0        0        0   105823 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.html
+-rw-r--r--   0        0        0   101555 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.html
+-rw-r--r--   0        0        0   101740 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.html
+-rw-r--r--   0        0        0   101327 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.html
+-rw-r--r--   0        0        0    90484 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.html
+-rw-r--r--   0        0        0    95036 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.html
+-rw-r--r--   0        0        0   106882 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.html
+-rw-r--r--   0        0        0   104529 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.html
+-rw-r--r--   0        0        0    77244 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.html
+-rw-r--r--   0        0        0   101018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.html
+-rw-r--r--   0        0        0    96704 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.html
+-rw-r--r--   0        0        0    96492 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.html
+-rw-r--r--   0        0        0   100867 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.html
+-rw-r--r--   0        0        0    97263 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.html
+-rw-r--r--   0        0        0   117840 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.html
+-rw-r--r--   0        0        0    98796 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.html
+-rw-r--r--   0        0        0    99321 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.html
+-rw-r--r--   0        0        0    99309 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.html
+-rw-r--r--   0        0        0    97607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.html
+-rw-r--r--   0        0        0    97511 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.html
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.html
+-rw-r--r--   0        0        0   100741 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.html
+-rw-r--r--   0        0        0    98851 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.html
+-rw-r--r--   0        0        0    97387 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_id.html
+-rw-r--r--   0        0        0    98563 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status.html
+-rw-r--r--   0        0        0   101796 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status_and_workspace.html
+-rw-r--r--   0        0        0    99500 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_workspace.html
+-rw-r--r--   0        0        0    90132 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_update.html
+-rw-r--r--   0        0        0    97111 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.html
+-rw-r--r--   0        0        0    97527 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.html
+-rw-r--r--   0        0        0    97283 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.html
+-rw-r--r--   0        0        0    96571 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.html
+-rw-r--r--   0        0        0    98574 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.html
+-rw-r--r--   0        0        0    97932 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.html
+-rw-r--r--   0        0        0    97500 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.html
+-rw-r--r--   0        0        0   100083 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.html
+-rw-r--r--   0        0        0    99319 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.html
+-rw-r--r--   0        0        0    80018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.html
+-rw-r--r--   0        0        0    75031 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.html
+-rw-r--r--   0        0        0    80018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.html
+-rw-r--r--   0        0        0    75031 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.html
+-rw-r--r--   0        0        0   247398 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.html
+-rw-r--r--   0        0        0    77057 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.html
+-rw-r--r--   0        0        0    76000 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    76698 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.html
+-rw-r--r--   0        0        0    89869 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    76792 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.html
+-rw-r--r--   0        0        0    90314 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   137892 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.html
+-rw-r--r--   0        0        0    48283 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    49047 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    47768 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    45477 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    81740 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.html
+-rw-r--r--   0        0        0    45501 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   108406 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.html
+-rw-r--r--   0        0        0    72211 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.html
+-rw-r--r--   0        0        0   116441 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.html
+-rw-r--r--   0        0        0    82564 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.html
+-rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.html
+-rw-r--r--   0        0        0   255712 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.html
+-rw-r--r--   0        0        0    78641 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.html
+-rw-r--r--   0        0        0    77371 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    78282 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.html
+-rw-r--r--   0        0        0    91786 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    78376 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.html
+-rw-r--r--   0        0        0    92231 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   141854 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    48924 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    49737 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    48409 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46020 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    83506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    46044 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   110939 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.html
+-rw-r--r--   0        0        0    87219 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.html
+-rw-r--r--   0        0        0   225352 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.html
+-rw-r--r--   0        0        0   179675 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.html
+-rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.html
+-rw-r--r--   0        0        0    49043 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.html
+-rw-r--r--   0        0        0   146962 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    49751 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    50627 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    49236 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46721 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    85788 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    46745 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   178307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.html
+-rw-r--r--   0        0        0    49565 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.html
+-rw-r--r--   0        0        0    78631 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.html
+-rw-r--r--   0        0        0   110252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.html
+-rw-r--r--   0        0        0    68384 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_200_item.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.html
+-rw-r--r--   0        0        0   104659 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_json_body.html
+-rw-r--r--   0        0        0   220093 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item.html
+-rw-r--r--   0        0        0   176239 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary.html
+-rw-r--r--   0        0        0    49288 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary_aggregation.html
+-rw-r--r--   0        0        0    48549 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_status.html
+-rw-r--r--   0        0        0   144127 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    50133 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    48777 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46332 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    84522 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    46356 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   174871 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary.html
+-rw-r--r--   0        0        0    49106 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary_aggregation.html
+-rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_400.html
+-rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_401.html
+-rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_500.html
+-rw-r--r--   0        0        0    74300 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.html
+-rw-r--r--   0        0        0   268583 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.html
+-rw-r--r--   0        0        0    78193 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.html
+-rw-r--r--   0        0        0    76983 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    77834 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.html
+-rw-r--r--   0        0        0    91242 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    77928 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.html
+-rw-r--r--   0        0        0    91687 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   140730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    49541 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    48227 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    83006 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    45890 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   110339 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.html
+-rw-r--r--   0        0        0   267313 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.html
+-rw-r--r--   0        0        0    80673 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.html
+-rw-r--r--   0        0        0    79130 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    80314 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.html
+-rw-r--r--   0        0        0    94247 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    80408 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.html
+-rw-r--r--   0        0        0    94692 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   146937 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.html
+-rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    50623 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    49232 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46717 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    85772 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.html
+-rw-r--r--   0        0        0    46741 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   114192 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.html
+-rw-r--r--   0        0        0    69546 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.html
+-rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.html
+-rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.html
+-rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.html
+-rw-r--r--   0        0        0   257261 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.html
+-rw-r--r--   0        0        0    78865 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.html
+-rw-r--r--   0        0        0    77565 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    78506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.html
+-rw-r--r--   0        0        0    92058 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    78600 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.html
+-rw-r--r--   0        0        0    92503 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   142416 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.html
+-rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    49835 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    48500 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46097 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    83756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.html
+-rw-r--r--   0        0        0    46121 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   111299 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.html
+-rw-r--r--   0        0        0   224337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.html
+-rw-r--r--   0        0        0   178975 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.html
+-rw-r--r--   0        0        0    49652 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.html
+-rw-r--r--   0        0        0    48941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.html
+-rw-r--r--   0        0        0   146375 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    49656 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    50525 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    49141 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46640 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    85522 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    46664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   177607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.html
+-rw-r--r--   0        0        0    49470 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.html
+-rw-r--r--   0        0        0    76814 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.html
+-rw-r--r--   0        0        0    77468 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.html
+-rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.html
+-rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.html
+-rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.html
+-rw-r--r--   0        0        0   156808 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.html
+-rw-r--r--   0        0        0    79738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.html
+-rw-r--r--   0        0        0    69201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.html
+-rw-r--r--   0        0        0   159996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.html
+-rw-r--r--   0        0        0    96970 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.html
+-rw-r--r--   0        0        0    96196 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.html
+-rw-r--r--   0        0        0    69367 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.html
+-rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.html
+-rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.html
+-rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.html
+-rw-r--r--   0        0        0    74075 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.html
+-rw-r--r--   0        0        0    68703 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.html
+-rw-r--r--   0        0        0    74305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.html
+-rw-r--r--   0        0        0    68869 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.html
+-rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.html
+-rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.html
+-rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.html
+-rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.html
+-rw-r--r--   0        0        0    68703 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.html
+-rw-r--r--   0        0        0    74445 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.html
+-rw-r--r--   0        0        0    76003 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.html
+-rw-r--r--   0        0        0    71398 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.html
+-rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.html
+-rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.html
+-rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.html
+-rw-r--r--   0        0        0    69712 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.html
+-rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.html
+-rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.html
+-rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.html
+-rw-r--r--   0        0        0    74738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.html
+-rw-r--r--   0        0        0    69878 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.html
+-rw-r--r--   0        0        0    84036 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.html
+-rw-r--r--   0        0        0    68211 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.html
+-rw-r--r--   0        0        0    70842 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.html
+-rw-r--r--   0        0        0   110748 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.html
+-rw-r--r--   0        0        0   114100 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.html
+-rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.html
+-rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.html
+-rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.html
+-rw-r--r--   0        0        0    71360 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.html
+-rw-r--r--   0        0        0    81687 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.html
+-rw-r--r--   0        0        0    99356 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.html
+-rw-r--r--   0        0        0    83498 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.html
+-rw-r--r--   0        0        0   115258 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.html
+-rw-r--r--   0        0        0   105405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.html
+-rw-r--r--   0        0        0    46114 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.html
+-rw-r--r--   0        0        0    86971 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.html
+-rw-r--r--   0        0        0    85711 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.html
+-rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.html
+-rw-r--r--   0        0        0    78923 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.html
+-rw-r--r--   0        0        0    88601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.html
+-rw-r--r--   0        0        0    87371 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.html
+-rw-r--r--   0        0        0    90725 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.html
+-rw-r--r--   0        0        0    80112 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.html
+-rw-r--r--   0        0        0    45522 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.html
+-rw-r--r--   0        0        0   119549 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.html
+-rw-r--r--   0        0        0    70280 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.html
+-rw-r--r--   0        0        0   107861 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.html
+-rw-r--r--   0        0        0    75696 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.html
+-rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.html
+-rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.html
+-rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.html
+-rw-r--r--   0        0        0    96500 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.html
+-rw-r--r--   0        0        0    68859 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.html
+-rw-r--r--   0        0        0    83809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.html
+-rw-r--r--   0        0        0   155198 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.html
+-rw-r--r--   0        0        0    69238 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.html
+-rw-r--r--   0        0        0    83368 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.html
+-rw-r--r--   0        0        0    72567 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.html
+-rw-r--r--   0        0        0    83727 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.html
+-rw-r--r--   0        0        0    67694 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.html
+-rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.html
+-rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.html
+-rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.html
+-rw-r--r--   0        0        0    83009 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.html
+-rw-r--r--   0        0        0    75223 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.html
+-rw-r--r--   0        0        0    91489 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.html
+-rw-r--r--   0        0        0    73642 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.html
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.html
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.html
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.html
+-rw-r--r--   0        0        0    72867 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.html
+-rw-r--r--   0        0        0   146363 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.html
+-rw-r--r--   0        0        0    79269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.html
+-rw-r--r--   0        0        0   143833 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.html
+-rw-r--r--   0        0        0    48904 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.html
+-rw-r--r--   0        0        0    72317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.html
+-rw-r--r--   0        0        0    51426 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.html
+-rw-r--r--   0        0        0   122335 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.html
+-rw-r--r--   0        0        0   142755 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.html
+-rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.html
+-rw-r--r--   0        0        0    71968 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.html
+-rw-r--r--   0        0        0    51212 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.html
+-rw-r--r--   0        0        0    72505 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.html
+-rw-r--r--   0        0        0    73018 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.html
+-rw-r--r--   0        0        0    78096 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.html
+-rw-r--r--   0        0        0   141171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.html
+-rw-r--r--   0        0        0    48445 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.html
+-rw-r--r--   0        0        0    71464 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.html
+-rw-r--r--   0        0        0    50897 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.html
+-rw-r--r--   0        0        0    87540 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.html
+-rw-r--r--   0        0        0   143811 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.html
+-rw-r--r--   0        0        0    48900 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.html
+-rw-r--r--   0        0        0    72304 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.html
+-rw-r--r--   0        0        0    51422 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.html
+-rw-r--r--   0        0        0    47341 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.html
+-rw-r--r--   0        0        0    71728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.html
+-rw-r--r--   0        0        0    67391 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.html
+-rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.html
+-rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.html
+-rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.html
+-rw-r--r--   0        0        0    72120 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.html
+-rw-r--r--   0        0        0    67727 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.html
+-rw-r--r--   0        0        0    79001 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.html
+-rw-r--r--   0        0        0    76665 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.html
+-rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.html
+-rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.html
+-rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.html
+-rw-r--r--   0        0        0    81109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.html
+-rw-r--r--   0        0        0    74260 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.html
+-rw-r--r--   0        0        0    79975 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.html
+-rw-r--r--   0        0        0    70389 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.html
+-rw-r--r--   0        0        0    72475 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.html
+-rw-r--r--   0        0        0    88028 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.html
+-rw-r--r--   0        0        0   109802 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.html
+-rw-r--r--   0        0        0    71831 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.html
+-rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.html
+-rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.html
+-rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.html
+-rw-r--r--   0        0        0    72851 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.html
+-rw-r--r--   0        0        0   126961 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.html
+-rw-r--r--   0        0        0   110890 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.html
+-rw-r--r--   0        0        0    72361 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.html
+-rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.html
+-rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.html
+-rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.html
+-rw-r--r--   0        0        0    71840 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_json_body.html
+-rw-r--r--   0        0        0    75030 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200.html
+-rw-r--r--   0        0        0   279449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task.html
+-rw-r--r--   0        0        0   235836 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item.html
+-rw-r--r--   0        0        0    72127 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_error_data.html
+-rw-r--r--   0        0        0    72293 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_output_data.html
+-rw-r--r--   0        0        0    46678 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_0.html
+-rw-r--r--   0        0        0    46642 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_1.html
+-rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_2.html
+-rw-r--r--   0        0        0    46786 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_3.html
+-rw-r--r--   0        0        0    46726 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_4.html
+-rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_5.html
+-rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_6.html
+-rw-r--r--   0        0        0    78265 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_7.html
+-rw-r--r--   0        0        0    45405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_0.html
+-rw-r--r--   0        0        0    45429 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_1.html
+-rw-r--r--   0        0        0    74928 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_2.html
+-rw-r--r--   0        0        0    45357 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_0.html
+-rw-r--r--   0        0        0    45321 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_1.html
+-rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_2.html
+-rw-r--r--   0        0        0    45465 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_3.html
+-rw-r--r--   0        0        0    45405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_4.html
+-rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_5.html
+-rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_6.html
+-rw-r--r--   0        0        0    74928 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_7.html
+-rw-r--r--   0        0        0    45455 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_0.html
+-rw-r--r--   0        0        0    45575 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_1.html
+-rw-r--r--   0        0        0    45491 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_2.html
+-rw-r--r--   0        0        0    75329 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_3.html
+-rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_400.html
+-rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_401.html
+-rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_500.html
+-rw-r--r--   0        0        0   169074 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body.html
+-rw-r--r--   0        0        0    46366 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_0.html
+-rw-r--r--   0        0        0    46330 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_1.html
+-rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_2.html
+-rw-r--r--   0        0        0    46474 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_3.html
+-rw-r--r--   0        0        0    46414 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_4.html
+-rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_5.html
+-rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_6.html
+-rw-r--r--   0        0        0    77476 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_7.html
+-rw-r--r--   0        0        0    87286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200.html
+-rw-r--r--   0        0        0   129638 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item.html
+-rw-r--r--   0        0        0    47034 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_0.html
+-rw-r--r--   0        0        0    47058 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_1.html
+-rw-r--r--   0        0        0    79041 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_2.html
+-rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_400.html
+-rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_401.html
+-rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_500.html
+-rw-r--r--   0        0        0   154233 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body.html
+-rw-r--r--   0        0        0    45434 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_0.html
+-rw-r--r--   0        0        0    45398 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_1.html
+-rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_2.html
+-rw-r--r--   0        0        0    45542 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_3.html
+-rw-r--r--   0        0        0    45482 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_4.html
+-rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_5.html
+-rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_6.html
+-rw-r--r--   0        0        0    75122 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_7.html
+-rw-r--r--   0        0        0    83570 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200.html
+-rw-r--r--   0        0        0   123274 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item.html
+-rw-r--r--   0        0        0    46102 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_0.html
+-rw-r--r--   0        0        0    46126 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_1.html
+-rw-r--r--   0        0        0    76687 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_2.html
+-rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_400.html
+-rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_401.html
+-rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_500.html
+-rw-r--r--   0        0        0    73401 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_json_body.html
+-rw-r--r--   0        0        0    84383 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200.html
+-rw-r--r--   0        0        0   219068 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item.html
+-rw-r--r--   0        0        0    46333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_0.html
+-rw-r--r--   0        0        0    46357 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_1.html
+-rw-r--r--   0        0        0    77269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_2.html
+-rw-r--r--   0        0        0    46285 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_0.html
+-rw-r--r--   0        0        0    46249 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_1.html
+-rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_2.html
+-rw-r--r--   0        0        0    46393 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_3.html
+-rw-r--r--   0        0        0    46333 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_4.html
+-rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_5.html
+-rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_6.html
+-rw-r--r--   0        0        0    77269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_7.html
+-rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_400.html
+-rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_401.html
+-rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_500.html
+-rw-r--r--   0        0        0   129869 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body.html
+-rw-r--r--   0        0        0    69164 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_additional_data.html
+-rw-r--r--   0        0        0    68285 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_error_data.html
+-rw-r--r--   0        0        0    50899 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_status.html
+-rw-r--r--   0        0        0    74827 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200.html
+-rw-r--r--   0        0        0   164435 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data.html
+-rw-r--r--   0        0        0    45272 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_0.html
+-rw-r--r--   0        0        0    45236 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_1.html
+-rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_2.html
+-rw-r--r--   0        0        0    45380 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_3.html
+-rw-r--r--   0        0        0    45320 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_4.html
+-rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_5.html
+-rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_6.html
+-rw-r--r--   0        0        0    74708 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_7.html
+-rw-r--r--   0        0        0    76620 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_500.html
+-rw-r--r--   0        0        0   102591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.html
+-rw-r--r--   0        0        0    68109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.html
+-rw-r--r--   0        0        0    72650 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.html
+-rw-r--r--   0        0        0    73154 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.html
+-rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.html
+-rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.html
+-rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.html
+-rw-r--r--   0        0        0    74934 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.html
+-rw-r--r--   0        0        0    83034 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.html
+-rw-r--r--   0        0        0   112145 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.html
+-rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.html
+-rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.html
+-rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.html
+-rw-r--r--   0        0        0    73182 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.html
+-rw-r--r--   0        0        0    84128 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.html
+-rw-r--r--   0        0        0    83709 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.html
+-rw-r--r--   0        0        0    88686 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.html
+-rw-r--r--   0        0        0    74176 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.html
+-rw-r--r--   0        0        0    32122 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/logs/pipeline-logs-1.arrow
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/pdoc_templates/frame.html.jinja2
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/pdoc_templates/module.html.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/__init__.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/reusable_responders.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/status_samples.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_assay.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_assay_config.py
+-rw-r--r--   0        0        0    26551 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_auth.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_checks.py
+-rw-r--r--   0        0        0    49739 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_client.py
+-rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_comment.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_connection.py
+-rw-r--r--   0        0        0    29940 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_deployment.py
+-rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_deployment_config.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_engine_config.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_explainability.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_import.py
+-rw-r--r--   0        0        0    21694 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_inference_result.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_log_entries.py
+-rw-r--r--   0        0        0    20326 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_model.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_model_config.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_models.py
+-rw-r--r--   0        0        0    21947 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_pipeline.py
+-rw-r--r--   0        0        0    31774 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_pipeline_config.py
+-rw-r--r--   0        0        0    14056 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_pipeline_variant.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_tag.py
+-rw-r--r--   0        0        0    14900 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/test_workspace.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/testutil.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/.DS_Store
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/ccfraud_output.json
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/day5_output.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/dev_smoke_test.arrow
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/dev_smoke_test.pandas.json
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/dev_smoke_test.txt
+-rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/lazyadam_output.json
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/pipeline_output.json
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/sample_batched_inference_result.json
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/sample_inference_result.arrow
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/sample_inference_result.json
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/sample_inference_result.pandas.json
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/sample_logged_inference_result.json
+-rw-r--r--   0        0        0    32666 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/sample_logs.arrow
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/some_output.json
+-rw-r--r--   0        0        0    32122 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/test_logs-1.arrow
+-rw-r--r--   0        0        0    32122 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/outputs/logs/pipeline-logs-1.arrow
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_aggregate_function/aggregate.json
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_bounds_expression/bounds.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_bounds_expression/gauges.json
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_model_drift/drift.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_model_drift/gauges.json
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_values_expression/gauges.json
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_values_expression/values.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/default_model_config.yaml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/experiment_model_config.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_batch_config_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_batch_config_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/post_model_config.yaml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/pre_model_config.yaml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/wl_model_config.yaml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/challenger.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/control.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/control.yaml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/model2.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/model3.yaml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_simple_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_simple_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_single_alert/alert.json
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_single_validation/single_validation.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_validate/single_validation.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_validation_placement/checked_pipeline.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/ModelConversion.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/__init__.py
+-rw-r--r--   0        0        0    17522 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/assay.py
+-rw-r--r--   0        0        0    28003 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/assay_config.py
+-rw-r--r--   0        0        0    27397 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/auth.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/checks.py
+-rw-r--r--   0        0        0    81099 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/client.py
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/comment.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/connection.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/datasizeunit.py
+-rw-r--r--   0        0        0    30957 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/deployment.py
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/deployment_config.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/engine_config.py
+-rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/explainability.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/expression.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/framework.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/functions.py
+-rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/inference_decode.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/inference_result.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/logs.py
+-rw-r--r--   0        0        0    17966 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/model.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/model_config.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/models.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/notify.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/object.py
+-rw-r--r--   0        0        0    12348 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/orchestration.py
+-rw-r--r--   0        0        0    37337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/pipeline.py
+-rw-r--r--   0        0        0    26383 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/pipeline_config.py
+-rw-r--r--   0        0        0     8286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/pipeline_variant.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/queries.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/standalone_client.py
+-rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/tag.py
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/task.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/unwrap.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/user.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/user_type.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/utils.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/version.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/visibility.py
+-rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/workspace.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateConnection.graphql
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateDefaultUserWorkspace.graphql
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateDeployment.graphql
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreatePipelineWithDefinition.graphql
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateTag.graphql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateWorkspace.graphql
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateWorkspaceBare.graphql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateWorkspaceConnection.graphql
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/DeleteConnection.graphql
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/DeleteWorkspaceConnection.graphql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/DeleteWorkspaceUser.graphql
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetConfiguredModelById.graphql
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetConfiguredModelByTaskId.graphql
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetConnection.graphql
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetConnectionById.graphql
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetDeploymentForPipeline.graphql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModel.graphql
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModelById.graphql
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModelByTaskId.graphql
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModelConfigs.graphql
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModels.graphql
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineAndWorkspace.graphql
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineByIdForCopying.graphql
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineByName.graphql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineVersion.graphql
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineVersionDeploymentDetails.graphql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelinesForModels.graphql
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertConfiguredModel.graphql
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertDeploymentModelConfig.graphql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertDeploymentModelConfigMultiple.graphql
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertDeploymentPipelineVersion.graphql
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertModel.graphql
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertModelConfig.graphql
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertModelConfigFull.graphql
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertWorkspaceUser.graphql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListConnections.graphql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListDeployments.graphql
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListModelConversions.graphql
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListModels.graphql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListPipelines.graphql
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListWorkspaces.graphql
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ModelByName.graphql
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/PipelineModels.graphql
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/PipelineVariantById.graphql
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/README.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Undeploy.graphql
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/UpdateModel.graphql
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/UpdateModelConversionMetaData.graphql
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/UserDefaultWorkspace.graphql
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/WorkspaceById.graphql
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/WorkspaceByName.graphql
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/WorkspaceListConnections.graphql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/WorkspaceNameById.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/AssaySetActive.graphql
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/CreateAssay.graphql
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/FilterAssays.graphql
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/GetAssayResults.graphql
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/ListAssays.graphql
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/ListAssaysWithPipeline.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/DeleteUsersFromWorkspace.graphql
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/GetUserWorkspacePermission.graphql
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/ListWorkspaceUsers.graphql
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/ListWorkspacesByUser.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetDeploymentPipelineVersion.graphql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetExplainabilityConfig.graphql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetExplainabilityConfigByReferencePipelineVersion.graphql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetExplainabilityRequest.graphql
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetPipelineByPipelineVersion.graphql
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetPipelineVersionVersion.graphql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/ListExplainabilityConfigs.graphql
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/ListExplainabilityConfigsByPipeline.graphql
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/ListExplainabilityRequests.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/GetLatestModelConfig.graphql
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/GetModel.graphql
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/GetModelVersions.graphql
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/GetModels.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/GetOrchestration.graphql
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/GetOrchestrationByTaskId.graphql
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/InsertOrchestration.graphql
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/ListOrchestrations.graphql
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/UpdateOrchestration.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/__init__.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/pipelines/GetPipelineDefinitionByNameAndVersion.graphql
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/pipelines/PipelineModelsFlat.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/pipelines/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/GetTaskById.graphql
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/GetTasksByStatus.graphql
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/GetTasksByStatusAndWorkspaceId.graphql
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/InsertTask.graphql
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/ListTasks.graphql
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/README.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/SetTaskKilled.graphql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/StartTaskRun.graphql
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/UpdateTask.graphql
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/UpdateTaskStatus.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/records/README.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/records/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/records/convert_keras_model.py
+-rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/records/graphql_queries.py
+-rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/records/telemetry_body.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/records/telemetry_error.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/records/v1_metric_response.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/records/v1_tls_response.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/__init__.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/client.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/errors.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/types.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/__init__.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.py
+-rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/__init__.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.py
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.py
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.py
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/__init__.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_add_to_workspace.py
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_create.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_delete.py
+-rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get.py
+-rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get_by_id.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_list.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_remove_from_workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/__init__.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.py
+-rw-r--r--   0        0        0     7982 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.py
+-rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.py
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/__init__.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/__init__.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.py
+-rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.py
+-rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.py
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/__init__.py
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/get_by_id.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/list_.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/__init__.py
+-rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_logs.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_version.py
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/__init__.py
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/__init__.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/cron_job.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_by_id1.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/kill.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/list1.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/network_service.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/oneshot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/__init__.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.py
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/__init__.py
+-rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.py
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.py
+-rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.py
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.py
+-rw-r--r--   0        0        0    58594 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/arbex_status.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.py
+-rw-r--r--   0        0        0    11372 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.py
+-rw-r--r--   0        0        0     9367 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body_next.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.py
+-rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.py
+-rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.py
+-rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.py
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.py
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_json_body.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_200.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_400.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_401.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_500.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body_details.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_200.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_400.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_401.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_500.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_json_body.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_400.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_401.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_500.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_json_body.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200_details.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_400.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_401.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_404.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_500.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_json_body.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200_details.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_400.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_401.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_404.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_500.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_json_body.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item_details.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_400.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_401.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_500.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_json_body.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_400.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_401.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_500.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_exec.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body_json.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request_json.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_response_201.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/event_base.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/event_base_extra_env_vars.py
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.py
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200_input_data.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_request.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_response.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_task_by_id_request.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/insert_task_response.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_request.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202_input_data.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_orchestrations_request.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_tasks_request.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_exec.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_request.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_request_json.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_response_201.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request_json.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_response_201.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/orchestration.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/orchestration_status.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body_order.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200_records.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200_status.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_400.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_401.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_500.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_json_body.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200_definition.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_400.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_401.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_500.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.py
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/task.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/task_input_data.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_request.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_response.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.py
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateConnection.graphql
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateDefaultUserWorkspace.graphql
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateDeployment.graphql
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreatePipelineWithDefinition.graphql
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateTag.graphql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateWorkspace.graphql
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateWorkspaceBare.graphql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/CreateWorkspaceConnection.graphql
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/DeleteConnection.graphql
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/DeleteWorkspaceConnection.graphql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/DeleteWorkspaceUser.graphql
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetConfiguredModelById.graphql
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetConfiguredModelByTaskId.graphql
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetConnection.graphql
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetConnectionById.graphql
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetDeploymentForPipeline.graphql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModel.graphql
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModelById.graphql
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModelByTaskId.graphql
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModelConfigs.graphql
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetModels.graphql
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineAndWorkspace.graphql
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineByIdForCopying.graphql
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineByName.graphql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineVersion.graphql
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineVersionDeploymentDetails.graphql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelinesForModels.graphql
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertConfiguredModel.graphql
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertDeploymentModelConfig.graphql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertDeploymentModelConfigMultiple.graphql
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertDeploymentPipelineVersion.graphql
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertModel.graphql
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertModelConfig.graphql
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertModelConfigFull.graphql
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/InsertWorkspaceUser.graphql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListConnections.graphql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListDeployments.graphql
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListModelConversions.graphql
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListModels.graphql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListPipelines.graphql
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ListWorkspaces.graphql
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/ModelByName.graphql
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/PipelineModels.graphql
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/PipelineVariantById.graphql
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/README.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Undeploy.graphql
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/UpdateModel.graphql
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/UpdateModelConversionMetaData.graphql
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/UserDefaultWorkspace.graphql
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/WorkspaceById.graphql
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/WorkspaceByName.graphql
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/WorkspaceListConnections.graphql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/WorkspaceNameById.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/AssaySetActive.graphql
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/CreateAssay.graphql
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/FilterAssays.graphql
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/GetAssayResults.graphql
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/ListAssays.graphql
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/ListAssaysWithPipeline.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/DeleteUsersFromWorkspace.graphql
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/GetUserWorkspacePermission.graphql
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/ListWorkspaceUsers.graphql
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/ListWorkspacesByUser.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/Workspaces/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetDeploymentPipelineVersion.graphql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetExplainabilityConfig.graphql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetExplainabilityConfigByReferencePipelineVersion.graphql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetExplainabilityRequest.graphql
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetPipelineByPipelineVersion.graphql
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/GetPipelineVersionVersion.graphql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/ListExplainabilityConfigs.graphql
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/ListExplainabilityConfigsByPipeline.graphql
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/ListExplainabilityRequests.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/GetLatestModelConfig.graphql
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/GetModel.graphql
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/GetModelVersions.graphql
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/GetModels.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/models/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/GetOrchestration.graphql
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/GetOrchestrationByTaskId.graphql
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/InsertOrchestration.graphql
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/ListOrchestrations.graphql
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/UpdateOrchestration.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/orch/__init__.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/pipelines/GetPipelineDefinitionByNameAndVersion.graphql
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/pipelines/PipelineModelsFlat.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/pipelines/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/GetTaskById.graphql
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/GetTasksByStatus.graphql
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/GetTasksByStatusAndWorkspaceId.graphql
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/InsertTask.graphql
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/ListTasks.graphql
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/README.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/SetTaskKilled.graphql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/StartTaskRun.graphql
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/UpdateTask.graphql
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/UpdateTaskStatus.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/.gitignore
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/public_README.md
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 wallaroo-2023.2.0rc2/PKG-INFO
```

### Comparing `wallaroo-2023.2.0rc1/.DS_Store` & `wallaroo-2023.2.0rc2/.DS_Store`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/.coverage` & `wallaroo-2023.2.0rc2/.coverage`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/Dockerfile` & `wallaroo-2023.2.0rc2/Dockerfile`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/Makefile` & `wallaroo-2023.2.0rc2/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 	python3 -m pip install hatch==1.7.0
 
 # This is a convenience for unit tests that will symlink into the SDK and need its dependencies.
 install-sdk-requirements: ensure_hatch
 	python3 -m hatch -e default dep show requirements | xargs python3 -m pip install
 
 build-sdk: clean generate-openapi ensure_hatch
-	SETUPTOOLS_SCM_PRETEND_VERSION="${SDK_VERSION}rc1" python3 -m hatch build
+	SETUPTOOLS_SCM_PRETEND_VERSION="${SDK_VERSION}rc2" python3 -m hatch build
 
 image: build-sdk
 	$(DOCKER) build \
 	-t $(SDK_IMAGE):$(TAG) -t $(SDK_IMAGE):latest \
 	--cache-to=type=registry,ref=$(SDK_IMAGE):cache,mode=max \
 	--cache-from=type=registry,ref=$(SDK_IMAGE):cache \
 	--label "org.opencontainers.image.revision=$(REVISION)" \
```

### Comparing `wallaroo-2023.2.0rc1/README.md` & `wallaroo-2023.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/requirements.txt` & `wallaroo-2023.2.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/Makefile` & `wallaroo-2023.2.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/make.bat` & `wallaroo-2023.2.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/autoscaling.ipynb` & `wallaroo-2023.2.0rc2/docs/source/autoscaling.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/conf.py` & `wallaroo-2023.2.0rc2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/core-abstractions.ipynb` & `wallaroo-2023.2.0rc2/docs/source/core-abstractions.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/email.png` & `wallaroo-2023.2.0rc2/docs/source/email.png`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/experiments.ipynb` & `wallaroo-2023.2.0rc2/docs/source/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/index.rst` & `wallaroo-2023.2.0rc2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/jupyter.md` & `wallaroo-2023.2.0rc2/docs/source/jupyter.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model-insights.ipynb` & `wallaroo-2023.2.0rc2/docs/source/model-insights.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model_conversion.rst` & `wallaroo-2023.2.0rc2/docs/source/model_conversion.rst`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model_conversion_keras.ipynb` & `wallaroo-2023.2.0rc2/docs/source/model_conversion_keras.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model_conversion_sklearn.ipynb` & `wallaroo-2023.2.0rc2/docs/source/model_conversion_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model_conversion_xgboost.ipynb` & `wallaroo-2023.2.0rc2/docs/source/model_conversion_xgboost.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/models.ipynb` & `wallaroo-2023.2.0rc2/docs/source/models.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/monitoring.ipynb` & `wallaroo-2023.2.0rc2/docs/source/monitoring.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/python-processing.ipynb` & `wallaroo-2023.2.0rc2/docs/source/python-processing.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/sdk.rst` & `wallaroo-2023.2.0rc2/docs/source/sdk.rst`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/standalone-mode.ipynb` & `wallaroo-2023.2.0rc2/docs/source/standalone-mode.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/workspaces.ipynb` & `wallaroo-2023.2.0rc2/docs/source/workspaces.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/BikeShareRegressor.py` & `wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/BikeShareRegressor.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/isolet_xgboost_model.pickle` & `wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/isolet_xgboost_model.pickle`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/pytorch_bikesharingmodel.pt` & `wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/pytorch_bikesharingmodel.pt`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/docs/source/model_conversion_resources/sentiment_model.zip` & `wallaroo-2023.2.0rc2/docs/source/model_conversion_resources/sentiment_model.zip`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/search.js` & `wallaroo-2023.2.0rc2/html/search.js`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo.html` & `wallaroo-2023.2.0rc2/html/wallaroo.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/ModelConversion.html` & `wallaroo-2023.2.0rc2/html/wallaroo/ModelConversion.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/assay.html` & `wallaroo-2023.2.0rc2/html/wallaroo/assay.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/assay_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/assay_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/auth.html` & `wallaroo-2023.2.0rc2/html/wallaroo/auth.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/checks.html` & `wallaroo-2023.2.0rc2/html/wallaroo/checks.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/client.html` & `wallaroo-2023.2.0rc2/html/wallaroo/client.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/comment.html` & `wallaroo-2023.2.0rc2/html/wallaroo/comment.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/connection.html` & `wallaroo-2023.2.0rc2/html/wallaroo/connection.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/datasizeunit.html` & `wallaroo-2023.2.0rc2/html/wallaroo/datasizeunit.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/deployment.html` & `wallaroo-2023.2.0rc2/html/wallaroo/deployment.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/deployment_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/deployment_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/engine_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/engine_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/explainability.html` & `wallaroo-2023.2.0rc2/html/wallaroo/explainability.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/expression.html` & `wallaroo-2023.2.0rc2/html/wallaroo/expression.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/framework.html` & `wallaroo-2023.2.0rc2/html/wallaroo/framework.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/functions.html` & `wallaroo-2023.2.0rc2/html/wallaroo/functions.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/graphql.html` & `wallaroo-2023.2.0rc2/html/wallaroo/graphql.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/inference_decode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/inference_decode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/inference_result.html` & `wallaroo-2023.2.0rc2/html/wallaroo/inference_result.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/logs.html` & `wallaroo-2023.2.0rc2/html/wallaroo/logs.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/model.html` & `wallaroo-2023.2.0rc2/html/wallaroo/model.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/model_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/model_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/models.html` & `wallaroo-2023.2.0rc2/html/wallaroo/models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/notify.html` & `wallaroo-2023.2.0rc2/html/wallaroo/notify.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/object.html` & `wallaroo-2023.2.0rc2/html/wallaroo/object.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/orchestration.html` & `wallaroo-2023.2.0rc2/html/wallaroo/orchestration.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/pipeline.html` & `wallaroo-2023.2.0rc2/html/wallaroo/pipeline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/pipeline_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/pipeline_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/pipeline_variant.html` & `wallaroo-2023.2.0rc2/html/wallaroo/pipeline_variant.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/queries.html` & `wallaroo-2023.2.0rc2/html/wallaroo/queries.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/records.html` & `wallaroo-2023.2.0rc2/html/wallaroo/records.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/standalone_client.html` & `wallaroo-2023.2.0rc2/html/wallaroo/standalone_client.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/tag.html` & `wallaroo-2023.2.0rc2/html/wallaroo/tag.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/task.html` & `wallaroo-2023.2.0rc2/html/wallaroo/task.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/unwrap.html` & `wallaroo-2023.2.0rc2/html/wallaroo/unwrap.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/user.html` & `wallaroo-2023.2.0rc2/html/wallaroo/user.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/user_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/user_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/utils.html` & `wallaroo-2023.2.0rc2/html/wallaroo/utils.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/version.html` & `wallaroo-2023.2.0rc2/html/wallaroo/version.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/visibility.html` & `wallaroo-2023.2.0rc2/html/wallaroo/visibility.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/workspace.html` & `wallaroo-2023.2.0rc2/html/wallaroo/workspace.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/graphql/Assays.html` & `wallaroo-2023.2.0rc2/html/wallaroo/graphql/Assays.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/graphql/Workspaces.html` & `wallaroo-2023.2.0rc2/html/wallaroo/graphql/Workspaces.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/graphql/explainability.html` & `wallaroo-2023.2.0rc2/html/wallaroo/graphql/explainability.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/graphql/models.html` & `wallaroo-2023.2.0rc2/html/wallaroo/graphql/models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/graphql/orch.html` & `wallaroo-2023.2.0rc2/html/wallaroo/graphql/orch.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/graphql/pipelines.html` & `wallaroo-2023.2.0rc2/html/wallaroo/graphql/pipelines.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/graphql/tasks.html` & `wallaroo-2023.2.0rc2/html/wallaroo/graphql/tasks.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/records/convert_keras_model.html` & `wallaroo-2023.2.0rc2/html/wallaroo/records/convert_keras_model.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/records/graphql_queries.html` & `wallaroo-2023.2.0rc2/html/wallaroo/records/graphql_queries.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/records/telemetry_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/records/telemetry_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/records/telemetry_error.html` & `wallaroo-2023.2.0rc2/html/wallaroo/records/telemetry_error.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/records/v1_metric_response.html` & `wallaroo-2023.2.0rc2/html/wallaroo/records/v1_metric_response.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/records/v1_tls_response.html` & `wallaroo-2023.2.0rc2/html/wallaroo/records/v1_tls_response.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/client.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/client.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/types.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/types.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_results.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_results.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_id.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_id.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status_and_workspace.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status_and_workspace.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_workspace.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_workspace.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_update.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_update.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_error_data.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_error_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_output_data.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_output_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_3.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_4.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_5.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_6.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_7.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_3.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_4.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_5.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_6.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_7.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_3.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_3.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_4.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_5.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_6.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_7.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_3.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_4.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_5.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_6.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_7.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_3.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_4.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_5.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_6.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_7.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_additional_data.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_additional_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_error_data.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_error_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_status.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_0.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_1.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_2.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_3.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_4.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_5.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_6.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_7.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.html` & `wallaroo-2023.2.0rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/pdoc_templates/frame.html.jinja2` & `wallaroo-2023.2.0rc2/pdoc_templates/frame.html.jinja2`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/reusable_responders.py` & `wallaroo-2023.2.0rc2/unit_tests/reusable_responders.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/status_samples.py` & `wallaroo-2023.2.0rc2/unit_tests/status_samples.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_assay.py` & `wallaroo-2023.2.0rc2/unit_tests/test_assay.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_assay_config.py` & `wallaroo-2023.2.0rc2/unit_tests/test_assay_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_auth.py` & `wallaroo-2023.2.0rc2/unit_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_checks.py` & `wallaroo-2023.2.0rc2/unit_tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_client.py` & `wallaroo-2023.2.0rc2/unit_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_comment.py` & `wallaroo-2023.2.0rc2/unit_tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_connection.py` & `wallaroo-2023.2.0rc2/unit_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_deployment.py` & `wallaroo-2023.2.0rc2/unit_tests/test_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
                 got_value = getattr(deployment, method_name)()
                 if want_value is not None:
                     self.assertEqual(want_value, got_value)
                 self.assertEqual(1, len(responses.calls))
                 responses.reset()
 
     @responses.activate
+    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "false"})
     def test_infer_on_pipeline(self):
         responses.add(
             responses.POST,
             url="http://engine-lb.some-pipeline-1:29502/pipelines/some-pipeline",
             json=SAMPLE_INFERENCE_RESULT,
         )
         responses.add(
@@ -213,14 +214,15 @@
         with self.assertRaises(TypeError):
             deployment.infer("foo")
 
         with self.assertRaises(TypeError):
             deployment.infer([])
 
     @responses.activate
+    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "false"})
     def test_infer_from_file(self):
         responses.add(
             responses.POST,
             url="http://engine-lb.some-pipeline-1:29502/pipelines/some-pipeline",
             json=SAMPLE_INFERENCE_RESULT,
         )
         responses.add(
@@ -284,15 +286,14 @@
             input = []
             json.dump(input, f)
             f.flush()
             with self.assertRaises(TypeError):
                 deployment.infer_from_file(f.name)
 
     @responses.activate
-    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "true"})
     def test_infer_from_file_with_arrow(self):
 
         responses.add(
             responses.POST,
             url="http://engine-lb.some-pipeline-1:29502/pipelines/some-pipeline",
             body=SAMPLE_ARROW_INFERENCE_RESPONSE,
         )
@@ -360,15 +361,14 @@
 
         self.assertEqual(
             list(fixed.columns)[:4],
             ["time", "in.text_input", "out._model_split", "out.banjori"],
         )
 
     @responses.activate
-    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "true"})
     def test_infer_from_file_with_pandas_records(self):
         result_df = pd.DataFrame.from_records(SAMPLE_PANDAS_RECORDS_INFERENCE_RESPONSE)
 
         responses.add(
             responses.POST,
             url="http://engine-lb.some-pipeline-1:29502/pipelines/some-pipeline",
             json=SAMPLE_PANDAS_RECORDS_INFERENCE_RESPONSE,
@@ -406,15 +406,14 @@
 
         output_df = deployment.infer_from_file(SAMPLE_PANDAS_RECORDS_FILE)
         self.assertIsInstance(output_df, pd.DataFrame)
         self.assertEqual(type(output_df["time"][0]), pd.Timestamp)
         self.assertEqual(type(output_df["check_failures"][0]), numpy.int64)
 
     @responses.activate
-    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "true"})
     def test_infer_from_file_with_invalid_file_type(self):
 
         deployment = Deployment(
             client=self.test_client,
             data={
                 "id": 1,
                 "deploy_id": "some-pipeline",
@@ -434,15 +433,14 @@
                 ],
             },
         )
         with self.assertRaises(TypeError):
             output = deployment.infer_from_file("unit_tests/outputs/dev_smoke_test.txt")
 
     @responses.activate
-    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "True"})
     def test_infer_with_arrow(self):
         with pa.ipc.open_file("unit_tests/outputs/dev_smoke_test.arrow") as source:
             table = source.read_all()
 
         responses.add(
             responses.POST,
             url="http://engine-lb.some-pipeline-1:29502/pipelines/some-pipeline",
@@ -484,15 +482,14 @@
             deployment.infer(123)
 
         with self.assertRaises(TypeError):
             deployment.infer("foo")
 
 
     @responses.activate
-    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "True"})
     def test_infer_with_pandas_records(self):
         data_df = pd.DataFrame.from_records(SAMPLE_PANDAS_RECORDS_INFERENCE_RESPONSE)
 
         responses.add(
             responses.POST,
             url="http://engine-lb.some-pipeline-1:29502/pipelines/some-pipeline",
             json=SAMPLE_PANDAS_RECORDS_INFERENCE_RESPONSE,
```

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_deployment_config.py` & `wallaroo-2023.2.0rc2/unit_tests/test_deployment_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_engine_config.py` & `wallaroo-2023.2.0rc2/unit_tests/test_engine_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_explainability.py` & `wallaroo-2023.2.0rc2/unit_tests/test_explainability.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_inference_result.py` & `wallaroo-2023.2.0rc2/unit_tests/test_inference_result.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_log_entries.py` & `wallaroo-2023.2.0rc2/unit_tests/test_log_entries.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_model.py` & `wallaroo-2023.2.0rc2/unit_tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from wallaroo.deployment import WaitForDeployError
 from wallaroo.pipeline import Pipeline
 from wallaroo.model import Model
 from wallaroo.tag import Tag
 
 import datetime
 from io import StringIO
+import os
 import responses
 from responses import matchers
 import time
 import unittest
+from unittest import mock
 from unittest.mock import patch
 import respx
 
 from . import status_samples
 from . import testutil
 from .reusable_responders import (
     add_deploy_responder,
@@ -489,14 +491,15 @@
             with patch("sys.stderr", new_callable=StringIO) as stderr:
                 success_deployment.undeploy()
                 outvalue = stdout.getvalue()
                 self.assertEqual(stdout.getvalue(), " ok\n")
                 self.assertEqual(stderr.getvalue(), "")
 
     @responses.activate
+    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "false"})
     def test_logs(self):
         responses.add(
             responses.GET,
             f"{self.test_client.api_endpoint}/v1/logs/topic/model-x-inference",
             status=200,
             json={
                 "partitions": {
```

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_model_config.py` & `wallaroo-2023.2.0rc2/unit_tests/test_model_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_models.py` & `wallaroo-2023.2.0rc2/unit_tests/test_models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_pipeline.py` & `wallaroo-2023.2.0rc2/unit_tests/test_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -332,14 +332,15 @@
                 got_value = getattr(pipeline, method_name)()
                 if want_value is not None:
                     self.assertEqual(want_value, got_value)
                 self.assertEqual(1, len(responses.calls))
                 responses.reset()
 
     @responses.activate
+    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "false"})
     def test_logs(self):
         self.add_get_topic_name_responder()
         self.add_user_workspace_responder()
 
         responses.add(
             responses.GET,
             f"http://api-lb:8080/v1/logs/topic/workspace-1-pipeline-x-inference",
@@ -364,15 +365,14 @@
             },
             match=[responses.matchers.json_params_matcher({"testing-1": 10, "testing-2": 10})],
         )
 
         self.assertEqual(len(self.pipeline.logs(20)), 1)
 
     @responses.activate
-    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "true"})
     def test_logs_with_arrow(self):
         params = {
                     "page_size": 100,
                     "order": "desc",
                     "dataset[]": "*",
                     "dataset.exclude[]": "metadata",
                     "dataset.separator": ".",
@@ -382,15 +382,14 @@
         self.add_get_records_responder(params)
         log_table = self.pipeline.logs(limit=100, arrow=True)
         
         self.assertIsInstance(log_table, pa.Table)
         log_table.equals(arrow_logs)
 
     @responses.activate
-    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "true"})
     def test_export_logs_to_arrow_file(self):
         start_datetime = datetime.datetime.utcnow()
         end_datetime = datetime.datetime.utcnow()
         params = {
             "time.start": start_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "time.end": end_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "dataset[]": "*",
@@ -403,15 +402,36 @@
         self.pipeline.export_logs(directory="unit_tests/outputs", file_prefix="test_logs", start_datetime=start_datetime,
                                   end_datetime=end_datetime, arrow=True)
         with pa.ipc.open_file("unit_tests/outputs/test_logs-1.arrow") as file_reader:
             entries = file_reader.read_all()
         arrow_logs.equals(entries, check_metadata=True)
 
     @responses.activate
-    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "true"})
+    def test_export_logs_without_user_provided_filepath(self):
+        start_datetime = datetime.datetime.utcnow()
+        end_datetime = datetime.datetime.utcnow()
+        params = {
+            "time.start": start_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
+            "time.end": end_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
+            "dataset[]": "*",
+            "dataset.exclude[]": "metadata",
+            "dataset.separator": ".",
+        }
+        self.add_get_topic_name_responder()
+        self.add_get_records_responder(params)
+        cwd = os.getcwd()
+        # we don't want to be writing test related files outside this directory
+        os.chdir("unit_tests/outputs")
+        self.pipeline.export_logs(start_datetime=start_datetime, end_datetime=end_datetime, arrow=True)
+        with pa.ipc.open_file("logs/pipeline-logs-1.arrow") as file_reader:
+            entries = file_reader.read_all()
+        arrow_logs.equals(entries, check_metadata=True)
+        os.chdir(cwd)
+
+    @responses.activate
     def test_get_pipeline_logs_by_time(self):
         start_datetime = datetime.datetime.utcnow()
         end_datetime = datetime.datetime.utcnow()
         params = {
             "time.start": start_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "time.end": end_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "dataset[]": "*",
@@ -423,14 +443,15 @@
         self.add_get_records_responder(params)
 
         log_table = self.pipeline.logs(start_datetime=start_datetime, end_datetime=end_datetime, arrow=True)
         self.assertIsInstance(log_table, pa.Table)
         log_table.equals(arrow_logs)
 
     @responses.activate
+    @mock.patch.dict(os.environ, {"ARROW_ENABLED": "false"})
     def test_log_time_shift(self):
         workspace_id = 1
         self.add_get_topic_name_responder()
         self.add_user_workspace_responder()
         responses.add(
             responses.POST,
             "http://api-lb:8080/v1/graphql",
```

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_pipeline_config.py` & `wallaroo-2023.2.0rc2/unit_tests/test_pipeline_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_pipeline_variant.py` & `wallaroo-2023.2.0rc2/unit_tests/test_pipeline_variant.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_tag.py` & `wallaroo-2023.2.0rc2/unit_tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/test_workspace.py` & `wallaroo-2023.2.0rc2/unit_tests/test_workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/testutil.py` & `wallaroo-2023.2.0rc2/unit_tests/testutil.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/.DS_Store` & `wallaroo-2023.2.0rc2/unit_tests/outputs/.DS_Store`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/ccfraud_output.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/ccfraud_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/day5_output.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/day5_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/dev_smoke_test.arrow` & `wallaroo-2023.2.0rc2/unit_tests/outputs/dev_smoke_test.arrow`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/dev_smoke_test.pandas.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/dev_smoke_test.pandas.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/dev_smoke_test.txt` & `wallaroo-2023.2.0rc2/unit_tests/outputs/dev_smoke_test.txt`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/lazyadam_output.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/lazyadam_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/pipeline_output.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/pipeline_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/sample_batched_inference_result.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/sample_batched_inference_result.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/sample_inference_result.arrow` & `wallaroo-2023.2.0rc2/unit_tests/outputs/sample_inference_result.arrow`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/sample_inference_result.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/sample_inference_result.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/sample_inference_result.pandas.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/sample_inference_result.pandas.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/sample_logged_inference_result.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/sample_logged_inference_result.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/sample_logs.arrow` & `wallaroo-2023.2.0rc2/unit_tests/outputs/sample_logs.arrow`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/outputs/some_output.json` & `wallaroo-2023.2.0rc2/unit_tests/outputs/some_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_aggregate_function/aggregate.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_aggregate_function/aggregate.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_bounds_expression/bounds.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_bounds_expression/bounds.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_bounds_expression/gauges.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_bounds_expression/gauges.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_model_drift/drift.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_model_drift/drift.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_model_drift/gauges.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_model_drift/gauges.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_values_expression/gauges.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_values_expression/gauges.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_checks/test_values_expression/values.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_checks/test_values_expression/values.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/model_config.yaml` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/model_config.yaml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/model_config.yaml` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/model_config.yaml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/model_config.yaml` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/model_config.yaml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_single_alert/alert.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_single_alert/alert.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_single_validation/single_validation.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_single_validation/single_validation.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_validate/single_validation.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_validate/single_validation.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/unit_tests/snapshots/test_pipeline_config/test_validation_placement/checked_pipeline.json` & `wallaroo-2023.2.0rc2/unit_tests/snapshots/test_pipeline_config/test_validation_placement/checked_pipeline.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/ModelConversion.py` & `wallaroo-2023.2.0rc2/wallaroo/ModelConversion.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/assay.py` & `wallaroo-2023.2.0rc2/wallaroo/assay.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/assay_config.py` & `wallaroo-2023.2.0rc2/wallaroo/assay_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/auth.py` & `wallaroo-2023.2.0rc2/wallaroo/auth.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/checks.py` & `wallaroo-2023.2.0rc2/wallaroo/checks.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/client.py` & `wallaroo-2023.2.0rc2/wallaroo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,14 @@
 DEFAULT_MODEL_CONVERSION_TIMEOUT = 60 * 10  # 10 minutes
 DEFAULT_MODEL_CONVERSION_PYTHON_VERSION = "3.8"
 
 DEFAULT_RECORDS_LIMIT = 100
 DEFAULT_RECORDS_BY_TIME_LIMIT = 1_000_000
 DEFAULT_MAX_DATA_SIZE = 100  # type: float
 DEFAULT_MAX_DATA_UNIT = DataSizeUnit.MiB
-DEFAULT_LOGS_DIRECTORY = "logs"
-DEFAULT_LOGS_FILE_PREFIX = "pipeline-logs"
 
 
 class Client(object):
     """Client handle to a Wallaroo platform instance.
 
     Objects of this class serve as the entrypoint to Wallaroo platform
     functionality.
@@ -1434,28 +1432,22 @@
         return size, unit
 
     def _export_logs(
         self,
         base: str,
         params: Dict[str, Any],
         headers: Dict[str, str],
-        directory: Optional[str] = None,
-        file_prefix: Optional[str] = None,
+        directory: str,
+        file_prefix: str,
         data_size_limit: Optional[str] = None,
         limit: Optional[int] = None,
         arrow: Optional[bool] = False,
     ) -> None:
         iterator = {}  # type: Dict[str, Any]
 
-        if directory is None:
-            directory = DEFAULT_LOGS_DIRECTORY
-        if not os.path.exists(directory):
-            os.makedirs(directory)
-        if file_prefix is None:
-            file_prefix = DEFAULT_LOGS_FILE_PREFIX
         chronological_order = (
             "oldest" if "time.start" and "time.end" in params else "newest"
         )
         data_size, data_unit = (
             self._validate_file_size_input(data_size_limit)
             if data_size_limit
             else (DEFAULT_MAX_DATA_SIZE, DEFAULT_MAX_DATA_UNIT)
@@ -1468,15 +1460,15 @@
         schema_changed = False
         end_time = None
         previous_end_time = None
 
         while iterator is not None:
             response = self._get_next_records(params, iterator, headers, base)
             logs_table, iterator, status = self._extract_logs_from_response(response)
-            if logs_table is None:
+            if logs_table.num_rows == 0:
                 break
             if schema is not None and schema != logs_table.schema:
                 schema_changed = True
                 writer.close()
                 writer = None
 
             if writer is None:
@@ -1556,15 +1548,15 @@
             limit=limit,
             start_datetime=start_datetime,
             end_datetime=end_datetime,
             dataset=dataset,
             dataset_exclude=dataset_exclude,
             dataset_separator=dataset_separator,
         )
-        if file_prefix is not None:
+        if file_prefix is not None and directory is not None:
             self._export_logs(
                 base=base,
                 directory=directory,
                 file_prefix=file_prefix,
                 data_size_limit=data_size_limit,
                 params=params,
                 headers=headers,
@@ -2093,18 +2085,28 @@
         return Orchestration.list_orchestrations(self)
 
     def upload_orchestration(
         self, bytes_buffer: Optional[bytes] = None, path: Optional[str] = None
     ):
         """Upload a file to be packaged and used as an Orchestration.
 
+        The uploaded artifact must be a ZIP file which contains:
+
+        * User code. If `main.py` exists, then that will be used as the task entrypoint. Otherwise,
+          the first `main.py` found in any subdirectory will be used as the entrypoint.
+        * Optional: A standard Python `requirements.txt` for any dependencies to be provided in the
+          task environment. The Wallaroo SDK will already be present and should not be mentioned.
+          Multiple `requirements.txt` files are not allowed.
+        * Optional: Any other artifacts desired for runtime, including data or code.
+
         :param Optional[str] path: The path to the file on your filesystem that will be uploaded as an Orchestration.
         :param Optional[str] file_name: An optional filename to describe your Orchestration when using the bytes_buffer param.
         :param Optional[bytes] bytes_buffer: The raw bytes to upload to be used Orchestration. Cannot be used with the `path` param.
         :return: The Orchestration that was uploaded.
+
         """
         return Orchestration.upload(self, bytes_buffer=bytes_buffer, path=path)
 
     def list_tasks(self):
         """List all Tasks in the current Workspace.
 
         :return: A List containing Task objects."""
```

### Comparing `wallaroo-2023.2.0rc1/wallaroo/comment.py` & `wallaroo-2023.2.0rc2/wallaroo/comment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/connection.py` & `wallaroo-2023.2.0rc2/wallaroo/connection.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/datasizeunit.py` & `wallaroo-2023.2.0rc2/wallaroo/datasizeunit.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/deployment.py` & `wallaroo-2023.2.0rc2/wallaroo/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from .wallaroo_ml_ops_api_client.types import UNSET
 
 if TYPE_CHECKING:
     from .client import Client
     from .model import Model
     from .pipeline_variant import PipelineVariant
 
-ARROW_ENABLED = "ARROW_ENABLED"
 ARROW_HEADER = "application/vnd.apache.arrow.file"
 ARROW_FORMAT = "arrow"
 PANDAS_RECORDS_HEADER = "application/json; format=pandas-records"
 PANDAS_RECORDS_FORMAT = "pandas-records"
 JSON_HEADER = "application/json"
 CUSTOM_JSON_FORMAT = "custom-json"
```

### Comparing `wallaroo-2023.2.0rc1/wallaroo/deployment_config.py` & `wallaroo-2023.2.0rc2/wallaroo/deployment_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/engine_config.py` & `wallaroo-2023.2.0rc2/wallaroo/engine_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/explainability.py` & `wallaroo-2023.2.0rc2/wallaroo/explainability.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/framework.py` & `wallaroo-2023.2.0rc2/wallaroo/framework.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/inference_decode.py` & `wallaroo-2023.2.0rc2/wallaroo/inference_decode.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/inference_result.py` & `wallaroo-2023.2.0rc2/wallaroo/inference_result.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/logs.py` & `wallaroo-2023.2.0rc2/wallaroo/logs.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/model.py` & `wallaroo-2023.2.0rc2/wallaroo/model.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/model_config.py` & `wallaroo-2023.2.0rc2/wallaroo/model_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/models.py` & `wallaroo-2023.2.0rc2/wallaroo/models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/notify.py` & `wallaroo-2023.2.0rc2/wallaroo/notify.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/object.py` & `wallaroo-2023.2.0rc2/wallaroo/object.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/orchestration.py` & `wallaroo-2023.2.0rc2/wallaroo/orchestration.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/pipeline.py` & `wallaroo-2023.2.0rc2/wallaroo/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import os
 import pathlib
 import sys
 import time
 from dataclasses import asdict
 from typing import (
     TYPE_CHECKING,
     Iterable,
@@ -42,14 +43,17 @@
     # Imports that happen below in methods to fix circular import dependency
     # issues need to also be specified here to satisfy mypy type checking.
     from .client import Client
     from .deployment import Deployment
     from .pipeline_variant import PipelineVariant
     from .tag import Tag
 
+DEFAULT_LOGS_DIRECTORY = "logs"
+DEFAULT_LOGS_FILE_PREFIX = "pipeline-logs"
+
 
 def update_timestamp(f):
     def _inner(self, *args, **kwargs):
         results = f(self, *args, **kwargs)
         if isinstance(results, list):
             self._last_infer_time = max(
                 # could be arbitrary json if not InferenceResult, which may not have "time" in results
@@ -470,14 +474,24 @@
         """
         topic = self.get_topic_name()
 
         if valid is False:
             topic += "-failures"
         assert self.client is not None
 
+        if directory is None:
+            directory = DEFAULT_LOGS_DIRECTORY
+        if not os.path.exists(directory):
+            try:
+                os.makedirs(directory)
+            except OSError as e:
+                raise Exception(f"Error while creating directory: {e}")
+        if file_prefix is None:
+            file_prefix = DEFAULT_LOGS_FILE_PREFIX
+
         self.client.get_logs(
             topic=topic,
             limit=limit,
             start_datetime=start_datetime,
             end_datetime=end_datetime,
             dataset=dataset,
             dataset_exclude=dataset_exclude,
```

### Comparing `wallaroo-2023.2.0rc1/wallaroo/pipeline_config.py` & `wallaroo-2023.2.0rc2/wallaroo/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/pipeline_variant.py` & `wallaroo-2023.2.0rc2/wallaroo/pipeline_variant.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/queries.py` & `wallaroo-2023.2.0rc2/wallaroo/queries.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/standalone_client.py` & `wallaroo-2023.2.0rc2/wallaroo/standalone_client.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/tag.py` & `wallaroo-2023.2.0rc2/wallaroo/tag.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/task.py` & `wallaroo-2023.2.0rc2/wallaroo/task.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/user.py` & `wallaroo-2023.2.0rc2/wallaroo/user.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/utils.py` & `wallaroo-2023.2.0rc2/wallaroo/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 MODELS_ENABLED = "MODELS_ENABLED"
 
 DEFAULT_ARROW_FILE_SUFFIX = "arrow"
 DEFAULT_JSON_FILE_SUFFIX = "json"
 
 
 def is_arrow_enabled():
-    return os.getenv(ARROW_ENABLED, "false").lower() == "true"
+    return os.getenv(ARROW_ENABLED, "true").lower() == "true"
 
 
 def is_models_enabled():
     return os.getenv(MODELS_ENABLED, "false").lower() == "true"
 
 
 def flatten_np_array_columns(df, col):
```

### Comparing `wallaroo-2023.2.0rc1/wallaroo/workspace.py` & `wallaroo-2023.2.0rc2/wallaroo/workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/CreateDefaultUserWorkspace.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/CreateDefaultUserWorkspace.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/CreateDeployment.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/CreateDeployment.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/CreatePipelineWithDefinition.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/CreatePipelineWithDefinition.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/GetPipelineByName.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/GetPipelineByName.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/InsertConfiguredModel.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/InsertConfiguredModel.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/InsertModel.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/InsertModel.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/InsertModelConfigFull.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/InsertModelConfigFull.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/PipelineVariantById.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/PipelineVariantById.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/UpdateModel.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/UpdateModel.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/UpdateModelConversionMetaData.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/UpdateModelConversionMetaData.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/CreateAssay.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/CreateAssay.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/Assays/ListAssays.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/Assays/ListAssays.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/InsertTask.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/InsertTask.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/README.md` & `wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/README.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/graphql/tasks/UpdateTask.graphql` & `wallaroo-2023.2.0rc2/wallaroo/graphql/tasks/UpdateTask.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/records/README.md` & `wallaroo-2023.2.0rc2/wallaroo/records/README.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/records/convert_keras_model.py` & `wallaroo-2023.2.0rc2/wallaroo/records/convert_keras_model.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/records/graphql_queries.py` & `wallaroo-2023.2.0rc2/wallaroo/records/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/records/telemetry_body.py` & `wallaroo-2023.2.0rc2/wallaroo/records/telemetry_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/records/telemetry_error.py` & `wallaroo-2023.2.0rc2/wallaroo/records/telemetry_error.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/records/v1_metric_response.py` & `wallaroo-2023.2.0rc2/wallaroo/records/v1_metric_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/records/v1_tls_response.py` & `wallaroo-2023.2.0rc2/wallaroo/records/v1_tls_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/client.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/client.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/types.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/types.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_add_to_workspace.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_add_to_workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_create.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_create.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_delete.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_delete.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get_by_id.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get_by_id.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_list.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_remove_from_workspace.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_remove_from_workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/get_by_id.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/get_by_id.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/list_.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/list_.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/upload.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/upload.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_logs.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_logs.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_version.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_version.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/cron_job.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/cron_job.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_by_id1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_by_id1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/kill.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/kill.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/list1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/list1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/network_service.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/network_service.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/oneshot.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/oneshot.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/__init__.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,14 @@
 from .models_upload_stream_response_401 import ModelsUploadStreamResponse401
 from .models_upload_stream_response_500 import ModelsUploadStreamResponse500
 from .models_upload_stream_visibility import ModelsUploadStreamVisibility
 from .network_service_exec import NetworkServiceExec
 from .network_service_request import NetworkServiceRequest
 from .network_service_request_json import NetworkServiceRequestJson
 from .network_service_response_201 import NetworkServiceResponse201
-from .oneshot_exec import OneshotExec
 from .oneshot_request import OneshotRequest
 from .oneshot_request_json import OneshotRequestJson
 from .oneshot_response_201 import OneshotResponse201
 from .orchestration import Orchestration
 from .orchestration_status import OrchestrationStatus
 from .pipelines_copy_pipeline_json_body import PipelinesCopyPipelineJsonBody
 from .pipelines_copy_pipeline_json_body_engine_config import \
@@ -965,15 +964,14 @@
     "ModelsUploadStreamResponse401",
     "ModelsUploadStreamResponse500",
     "ModelsUploadStreamVisibility",
     "NetworkServiceExec",
     "NetworkServiceRequest",
     "NetworkServiceRequestJson",
     "NetworkServiceResponse201",
-    "OneshotExec",
     "OneshotRequest",
     "OneshotRequestJson",
     "OneshotResponse201",
     "Orchestration",
     "OrchestrationStatus",
     "PipelinesCopyPipelineJsonBody",
     "PipelinesCopyPipelineJsonBodyEngineConfig",
```

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body_next.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body_next.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body_details.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200_details.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_404.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_404.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200_details.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_404.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_404.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item_details.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_exec.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_exec.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body_json.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body_json.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request_json.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request_json.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_response_201.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_response_201.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/event_base.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/event_base.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/event_base_extra_env_vars.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/event_base_extra_env_vars.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200_input_data.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200_input_data.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_response.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_task_by_id_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_task_by_id_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/insert_task_response.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/insert_task_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202_input_data.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202_input_data.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_orchestrations_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_orchestrations_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_tasks_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_tasks_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_exec.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_exec.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_request_json.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_request_json.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_response_201.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_response_201.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request_json.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request_json.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_response_201.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_response_201.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/orchestration.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/orchestration.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200_records.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_200_records.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200_definition.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200_definition.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/task.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/task.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/task_input_data.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/task_input_data.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_request.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_response.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.py` & `wallaroo-2023.2.0rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/public_README.md` & `wallaroo-2023.2.0rc2/public_README.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/pyproject.toml` & `wallaroo-2023.2.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.0rc1/PKG-INFO` & `wallaroo-2023.2.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallaroo
-Version: 2023.2.0rc1
+Version: 2023.2.0rc2
 Summary: Wallaroo.ai model management API client
 Project-URL: Homepage, https://www.wallaroo.ai/
 Author-email: "Wallaroo.ai" <hello@wallaroo.ai>
 License: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

