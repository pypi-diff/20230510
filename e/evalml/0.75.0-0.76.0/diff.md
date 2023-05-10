# Comparing `tmp/evalml-0.75.0.tar.gz` & `tmp/evalml-0.76.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-zhlwywqf/evalml-0.75.0.tar", last modified: Tue May  2 17:20:46 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-khmpqtc9/evalml-0.76.0.tar", last modified: Wed May 10 14:56:56 2023, max compression
```

## Comparing `evalml-0.75.0.tar` & `evalml-0.76.0.tar`

### file list

```diff
@@ -1,444 +1,444 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/
--rw-r--r--   0 root         (0) root         (0)     1513 2023-05-02 17:20:32.000000 evalml-0.75.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8233 2023-05-02 17:20:46.000000 evalml-0.75.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4824 2023-05-02 17:20:32.000000 evalml-0.75.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/
--rw-r--r--   0 root         (0) root         (0)      763 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/automl/
--rw-r--r--   0 root         (0) root         (0)      412 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/automl/automl_algorithm/
--rw-r--r--   0 root         (0) root         (0)      318 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11921 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_algorithm/automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    29145 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_algorithm/default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    21384 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_algorithm/iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    79617 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/automl_search.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/automl/engine/
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6902 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/cf_engine.py
--rw-r--r--   0 root         (0) root         (0)     6907 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/dask_engine.py
--rw-r--r--   0 root         (0) root         (0)    15405 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/engine_base.py
--rw-r--r--   0 root         (0) root         (0)     5060 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/engine/sequential_engine.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/progress.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/automl/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/data_checks/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11989 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_action.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_action_code.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     3156 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_message.py
--rw-r--r--   0 root         (0) root         (0)     6580 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_message_code.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_check_message_type.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/data_checks.py
--rw-r--r--   0 root         (0) root         (0)    25088 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/default_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    11488 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    20762 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)    11843 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    17159 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9500 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6213 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7242 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8124 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8205 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/data_checks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/demos/
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/__init__.py
--rw-r--r--   0 root         (0) root         (0)      605 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/churn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/demos/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     1103 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/diabetes.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/fraud.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/weather.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/demos/wine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/exceptions/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5886 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/exceptions/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/model_family/
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_family/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_family/model_family.py
--rw-r--r--   0 root         (0) root         (0)      910 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_family/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/model_understanding/
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
--rw-r--r--   0 root         (0) root         (0)    18388 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/_partial_dependence_utils.py
--rw-r--r--   0 root         (0) root         (0)     8990 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)     8042 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/force_plots.py
--rw-r--r--   0 root         (0) root         (0)    15125 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/metrics.py
--rw-r--r--   0 root         (0) root         (0)    27420 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/partial_dependence_functions.py
--rw-r--r--   0 root         (0) root         (0)    13556 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/permutation_importance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13317 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/_algorithms.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
--rw-r--r--   0 root         (0) root         (0)    36936 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15630 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/prediction_explanations/explainers.py
--rw-r--r--   0 root         (0) root         (0)    22293 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/model_understanding/visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/objectives/
--rw-r--r--   0 root         (0) root         (0)     1543 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     3392 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/fraud_cost.py
--rw-r--r--   0 root         (0) root         (0)     1780 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/multiclass_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/objective_base.py
--rw-r--r--   0 root         (0) root         (0)      406 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/regression_objective.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/sensitivity_low_alert.py
--rw-r--r--   0 root         (0) root         (0)    33865 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/standard_metrics.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/time_series_regression_objective.py
--rw-r--r--   0 root         (0) root         (0)     6835 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/objectives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/
--rw-r--r--   0 root         (0) root         (0)     1928 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4893 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/binary_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/binary_classification_pipeline_mixin.py
--rw-r--r--   0 root         (0) root         (0)     7845 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    40232 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/component_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/
--rw-r--r--   0 root         (0) root         (0)     1935 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10149 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/component_base.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/component_base_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/estimators/
--rw-r--r--   0 root         (0) root         (0)      964 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/
--rw-r--r--   0 root         (0) root         (0)     1445 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3656 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8797 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4811 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
--rw-r--r--   0 root         (0) root         (0)     5042 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8530 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/
--rw-r--r--   0 root         (0) root         (0)     1685 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13466 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4996 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7329 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7295 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
--rw-r--r--   0 root         (0) root         (0)     9356 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5128 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/
--rw-r--r--   0 root         (0) root         (0)     1478 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6235 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/column_selectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/
--rw-r--r--   0 root         (0) root         (0)      439 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
--rw-r--r--   0 root         (0) root         (0)    13779 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    12206 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/
--rw-r--r--   0 root         (0) root         (0)      599 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     5285 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
--rw-r--r--   0 root         (0) root         (0)     3116 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8253 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/imputer.py
--rw-r--r--   0 root         (0) root         (0)     4640 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     6187 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5357 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    11389 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5899 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    15805 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
--rw-r--r--   0 root         (0) root         (0)     3213 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8673 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
--rw-r--r--   0 root         (0) root         (0)     6461 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)    17526 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5354 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
--rw-r--r--   0 root         (0) root         (0)     7283 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/oversampler.py
--rw-r--r--   0 root         (0) root         (0)     8265 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/samplers/undersampler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/pipelines/components/transformers/scalers/
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/scalers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/transformers/transformer.py
--rw-r--r--   0 root         (0) root         (0)    18498 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/components/utils.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/multiclass_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    33022 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/pipeline_meta.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    17176 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/time_series_classification_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    15747 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/time_series_pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    12880 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/time_series_regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    53306 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/preprocessing/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/
--rw-r--r--   0 root         (0) root         (0)      367 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/no_split.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     5599 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/time_series_split.py
--rw-r--r--   0 root         (0) root         (0)     3669 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/data_splitters/training_validation_split.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/preprocessing/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/problem_types/
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/problem_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/problem_types/problem_types.py
--rw-r--r--   0 root         (0) root         (0)     6085 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/problem_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/automl_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5757 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/dask_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9622 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
--rw-r--r--   0 root         (0) root         (0)    17604 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
--rw-r--r--   0 root         (0) root         (0)    14529 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
--rw-r--r--   0 root         (0) root         (0)   179549 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38707 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38820 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_classification.py
--rw-r--r--   0 root         (0) root         (0)    15745 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
--rw-r--r--   0 root         (0) root         (0)     8716 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_regression.py
--rw-r--r--   0 root         (0) root         (0)     7055 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
--rw-r--r--   0 root         (0) root         (0)    12934 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_automl_utils.py
--rw-r--r--   0 root         (0) root         (0)    32956 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7793 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_engine_base.py
--rw-r--r--   0 root         (0) root         (0)    36749 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_search.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_search_iterative.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/automl_tests/test_time_series_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/component_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27084 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    11644 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    15261 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6678 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8548 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_column_selector_transformers.py
--rw-r--r--   0 root         (0) root         (0)    64838 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_components.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1370 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     7573 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
--rw-r--r--   0 root         (0) root         (0)     4797 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_en_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_en_regressor.py
--rw-r--r--   0 root         (0) root         (0)    15118 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_estimators.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6226 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_feature_selectors.py
--rw-r--r--   0 root         (0) root         (0)    14950 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_featuretools.py
--rw-r--r--   0 root         (0) root         (0)     9627 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
--rw-r--r--   0 root         (0) root         (0)    25736 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_imputer.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_knn_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2979 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     8017 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_label_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_lda.py
--rw-r--r--   0 root         (0) root         (0)    13414 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_lgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     9754 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_lgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8111 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_lsa.py
--rw-r--r--   0 root         (0) root         (0)    20457 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     9988 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_nullable_types_replacer.py
--rw-r--r--   0 root         (0) root         (0)    26816 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_one_hot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    25966 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)    19941 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_oversampler.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_pca.py
--rw-r--r--   0 root         (0) root         (0)    12025 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5021 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)    23430 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)    18269 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)    10542 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8928 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_target_encoder.py
--rw-r--r--   0 root         (0) root         (0)     9398 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    30311 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    24722 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_time_series_imputer.py
--rw-r--r--   0 root         (0) root         (0)     9937 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     6246 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_undersampler.py
--rw-r--r--   0 root         (0) root         (0)     9766 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3980 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2792 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/component_tests/test_xgboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)    80070 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     9729 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/tips.csv
--rw-r--r--   0 root         (0) root         (0)    61194 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data/titanic.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/data_checks_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24199 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_action.py
--rw-r--r--   0 root         (0) root         (0)    20667 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_message.py
--rw-r--r--   0 root         (0) root         (0)    29212 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    19715 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)    12185 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    30182 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    26417 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8238 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5609 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)    18212 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4898 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/data_checks_tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/demo_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/demo_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/demo_tests/test_datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/dependency_update_check/
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
--rw-r--r--   0 root         (0) root         (0)      642 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/dependency_update_check/minimum_requirements.txt
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10709 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
--rw-r--r--   0 root         (0) root         (0)     5184 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/integration_tests/test_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)     7110 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/integration_tests/test_time_series_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/model_family_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_family_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_family_tests/test_model_family.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14158 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
--rw-r--r--   0 root         (0) root         (0)    67430 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
--rw-r--r--   0 root         (0) root         (0)     9790 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
--rw-r--r--   0 root         (0) root         (0)    19357 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15261 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)    14744 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)    26774 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    98520 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
--rw-r--r--   0 root         (0) root         (0)    29313 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
--rw-r--r--   0 root         (0) root         (0)    26181 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/model_understanding_tests/test_visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/objective_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_fraud_detection.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_objectives.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_sla.py
--rw-r--r--   0 root         (0) root         (0)    27155 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/objective_tests/test_standard_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
--rw-r--r--   0 root         (0) root         (0)     4688 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3652 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
--rw-r--r--   0 root         (0) root         (0)    94308 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_component_graph.py
--rw-r--r--   0 root         (0) root         (0)     8969 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_graphs.py
--rw-r--r--   0 root         (0) root         (0)    49985 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
--rw-r--r--   0 root         (0) root         (0)   101164 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     5622 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    70356 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/test_no_split.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     3849 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/test_split_data.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/problem_type_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/problem_type_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6537 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/problem_type_tests/test_problem_types.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/test_all_test_dirs_included.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/tuner_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/tuner_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/tuner_tests/test_random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     9170 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/tuner_tests/test_skopt_tuner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tests/utils_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3993 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    30486 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)    12628 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tests/utils_tests/test_woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/tuners/
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     4675 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/skopt_tuner.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/tuner.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/tuners/tuner_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml/utils/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/base_meta.py
--rw-r--r--   0 root         (0) root         (0)     6540 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    26270 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     7066 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/update_checker.py
--rw-r--r--   0 root         (0) root         (0)     6346 2023-05-02 17:20:32.000000 evalml-0.75.0/evalml/utils/woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8233 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20684 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1283 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-02 17:20:46.000000 evalml-0.75.0/evalml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5078 2023-05-02 17:20:32.000000 evalml-0.75.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 17:20:46.000000 evalml-0.75.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-05-10 14:56:39.000000 evalml-0.76.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-05-10 14:56:56.000000 evalml-0.76.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-05-10 14:56:39.000000 evalml-0.76.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/automl/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/automl/automl_algorithm/
+-rw-r--r--   0 root         (0) root         (0)      318 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11921 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_algorithm/automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    29145 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_algorithm/default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    21384 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_algorithm/iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    86362 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_search.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/automl/engine/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6902 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)    15405 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/engine_base.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/sequential_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/progress.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/data_checks/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11989 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_action_code.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_message_code.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    25088 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/default_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11488 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    20762 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    11843 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    17159 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8124 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4569 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8205 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/demos/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      605 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/churn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/demos/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/diabetes.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/fraud.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/weather.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/wine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/exceptions/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/model_family/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_family/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_family/model_family.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_family/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/model_understanding/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
+-rw-r--r--   0 root         (0) root         (0)    18388 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/_partial_dependence_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    15125 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    27420 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/partial_dependence_functions.py
+-rw-r--r--   0 root         (0) root         (0)    13556 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/permutation_importance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
+-rw-r--r--   0 root         (0) root         (0)    36936 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15630 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/explainers.py
+-rw-r--r--   0 root         (0) root         (0)    22293 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/objectives/
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/fraud_cost.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/multiclass_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/objective_base.py
+-rw-r--r--   0 root         (0) root         (0)      406 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/sensitivity_low_alert.py
+-rw-r--r--   0 root         (0) root         (0)    33866 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/standard_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/time_series_regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)    15394 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/binary_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/binary_classification_pipeline_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     7845 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    40232 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/component_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10149 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/component_base.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/component_base_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/estimators/
+-rw-r--r--   0 root         (0) root         (0)      964 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8797 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4811 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8530 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13466 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7329 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5128 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/column_selectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    13779 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    12206 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     5285 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8253 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/imputer.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    11389 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5899 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    15805 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
+-rw-r--r--   0 root         (0) root         (0)     6461 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)    17526 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     7283 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     8265 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/undersampler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/scalers/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/scalers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/transformer.py
+-rw-r--r--   0 root         (0) root         (0)    18498 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/multiclass_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    33202 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/pipeline_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    17176 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/time_series_classification_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    15747 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/time_series_pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)    12880 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/time_series_regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    53306 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/no_split.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/time_series_split.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/training_validation_split.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/problem_types/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/problem_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/problem_types/problem_types.py
+-rw-r--r--   0 root         (0) root         (0)     6085 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/problem_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/automl_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/dask_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9622 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
+-rw-r--r--   0 root         (0) root         (0)    17604 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)    14529 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)   185850 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    38707 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    38820 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_classification.py
+-rw-r--r--   0 root         (0) root         (0)    15745 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_regression.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
+-rw-r--r--   0 root         (0) root         (0)    12934 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    32956 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7793 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_engine_base.py
+-rw-r--r--   0 root         (0) root         (0)    36749 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_search.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_search_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_time_series_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/component_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27084 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    11644 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6678 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8548 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_column_selector_transformers.py
+-rw-r--r--   0 root         (0) root         (0)    64838 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_components.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_en_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_en_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    15118 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_estimators.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_feature_selectors.py
+-rw-r--r--   0 root         (0) root         (0)    14950 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     9627 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
+-rw-r--r--   0 root         (0) root         (0)    25736 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_knn_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     8017 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_lda.py
+-rw-r--r--   0 root         (0) root         (0)    13414 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_lgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     9754 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_lgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_lsa.py
+-rw-r--r--   0 root         (0) root         (0)    20457 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     9988 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_nullable_types_replacer.py
+-rw-r--r--   0 root         (0) root         (0)    26816 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_one_hot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    25966 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    19941 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_pca.py
+-rw-r--r--   0 root         (0) root         (0)    12025 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    23430 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    18269 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)    10542 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_target_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     9398 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    30311 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    24722 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_time_series_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     6246 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_undersampler.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3980 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_xgboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    80078 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     9729 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/tips.csv
+-rw-r--r--   0 root         (0) root         (0)    61194 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/titanic.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/data_checks_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24199 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)    29212 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    19715 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    12185 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    30182 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    26417 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8238 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    18212 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4898 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/demo_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/demo_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/demo_tests/test_datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/dependency_update_check/
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/dependency_update_check/minimum_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/integration_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/integration_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10709 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/integration_tests/test_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/integration_tests/test_time_series_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/model_family_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_family_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_family_tests/test_model_family.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14158 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)    67430 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
+-rw-r--r--   0 root         (0) root         (0)     9790 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    19357 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)    14744 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)    26774 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    98520 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
+-rw-r--r--   0 root         (0) root         (0)    29313 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
+-rw-r--r--   0 root         (0) root         (0)    26181 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/objective_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_fraud_detection.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)    13953 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_objectives.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_sla.py
+-rw-r--r--   0 root         (0) root         (0)    27155 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_standard_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
+-rw-r--r--   0 root         (0) root         (0)     4688 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
+-rw-r--r--   0 root         (0) root         (0)    94308 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_component_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8969 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_graphs.py
+-rw-r--r--   0 root         (0) root         (0)    49985 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
+-rw-r--r--   0 root         (0) root         (0)   101489 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    70356 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/test_no_split.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/test_split_data.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/problem_type_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/problem_type_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/problem_type_tests/test_problem_types.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/test_all_test_dirs_included.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/tuner_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/tuner_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/tuner_tests/test_random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     9170 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/tuner_tests/test_skopt_tuner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/utils_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    30486 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12628 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tuners/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     4675 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/skopt_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/tuner.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/tuner_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/utils/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/base_meta.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    26270 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7066 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/update_checker.py
+-rw-r--r--   0 root         (0) root         (0)     6346 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20684 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-05-10 14:56:39.000000 evalml-0.76.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 14:56:56.000000 evalml-0.76.0/setup.cfg
```

### Comparing `evalml-0.75.0/LICENSE` & `evalml-0.76.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/PKG-INFO` & `evalml-0.76.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.75.0
+Version: 0.76.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.75.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.76.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.75.0/README.md` & `evalml-0.76.0/README.md`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/__init__.py` & `evalml-0.76.0/evalml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", FutureWarning)
     warnings.simplefilter("ignore", DeprecationWarning)
     import skopt
 warnings.filterwarnings("ignore", category=FutureWarning)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
-__version__ = "0.75.0"
+__version__ = "0.76.0"
```

### Comparing `evalml-0.75.0/evalml/automl/automl_algorithm/automl_algorithm.py` & `evalml-0.76.0/evalml/automl/automl_algorithm/automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/automl_algorithm/default_algorithm.py` & `evalml-0.76.0/evalml/automl/automl_algorithm/default_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/automl_algorithm/iterative_algorithm.py` & `evalml-0.76.0/evalml/automl/automl_algorithm/iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/automl_search.py` & `evalml-0.76.0/evalml/automl/automl_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,25 +27,33 @@
 from evalml.automl.utils import (
     AutoMLConfig,
     check_all_pipeline_names_unique,
     get_best_sampler_for_data,
     get_default_primary_search_objective,
     make_data_splitter,
 )
-from evalml.data_checks import DataCheckMessageType, DefaultDataChecks
+from evalml.data_checks import (
+    ClassImbalanceDataCheck,
+    DataCheckMessageType,
+    DefaultDataChecks,
+)
 from evalml.exceptions import (
     AutoMLSearchException,
     PipelineNotFoundError,
     PipelineScoreError,
 )
 from evalml.model_family import ModelFamily
 from evalml.objectives import (
+    get_default_recommendation_objectives,
     get_non_core_objectives,
     get_objective,
     get_optimization_objectives,
+    normalize_objectives,
+    organize_objectives,
+    recommendation_score,
 )
 from evalml.pipelines import (
     BinaryClassificationPipeline,
     ComponentGraph,
     MulticlassClassificationPipeline,
     RegressionPipeline,
 )
@@ -426,14 +434,20 @@
         verbose (boolean): Whether or not to display semi-real-time updates to stdout while search is running. Defaults to False.
 
         timing (boolean): Whether or not to write pipeline search times to the logger. Defaults to False.
         exclude_featurizers (list[str]): A list of featurizer components to exclude from the pipelines built by search.
             Valid options are "DatetimeFeaturizer", "EmailFeaturizer", "URLFeaturizer", "NaturalLanguageFeaturizer", "TimeSeriesFeaturizer"
 
         holdout_set_size (float): The size of the holdout set that AutoML search will take for datasets larger than 500 rows. If set to 0, holdout set will not be taken regardless of number of rows. Must be between 0 and 1, exclusive. Defaults to 0.1.
+
+        use_recommendation (bool): Whether or not to use a recommendation score to rank pipelines instead of optimization objective. Defaults to False.
+
+        include_recommendation (list[str]): A list of objectives to include beyond the defaults in the recommendation score. Defaults to None.
+
+        exclude_recommendation (list[str]): A list of objectives to exclude from the defaults in the recommendation score. Defaults to None.
     """
 
     _MAX_NAME_LEN = 40
 
     # Minimum number of rows dataset must have before a holdout set is used to rank pipelines.
     _HOLDOUT_SET_MIN_ROWS = 500
 
@@ -473,14 +487,17 @@
         _pipelines_per_batch=5,
         automl_algorithm="default",
         engine="sequential",
         verbose=False,
         timing=False,
         exclude_featurizers=None,
         holdout_set_size=0,
+        use_recommendation=False,
+        include_recommendation=None,
+        exclude_recommendation=None,
     ):
         self.verbose = verbose
         if verbose:
             self.logger = get_logger(f"{__name__}.verbose")
         else:
             self.logger = logging.getLogger(__name__)
         self.timing = timing
@@ -515,78 +532,24 @@
             )
 
         if is_time_series(self.problem_type):
             warnings.warn(
                 "Time series support in evalml is still in beta, which means we are still actively building "
                 "its core features. Please be mindful of that when running search().",
             )
+
         self.errors = {}
         self._SLEEP_TIME = 0.1
         self.tuner_class = tuner_class or SKOptTuner
         self.start_iteration_callback = start_iteration_callback
         self.add_result_callback = add_result_callback
         self.error_callback = error_callback or log_error_callback
         self.data_splitter = data_splitter
         self.optimize_thresholds = optimize_thresholds
         self.ensembling = ensembling
-        if objective == "auto":
-            objective = get_default_primary_search_objective(self.problem_type.value)
-        objective = get_objective(objective, return_instance=False)
-        self.objective = self._validate_objective(objective)
-        self.alternate_thresholding_objective = None
-        if (
-            is_binary(self.problem_type)
-            and self.optimize_thresholds
-            and self.objective.score_needs_proba
-        ):
-            self.alternate_thresholding_objective = get_objective(
-                alternate_thresholding_objective,
-                return_instance=True,
-            )
-        if (
-            self.alternate_thresholding_objective is not None
-            and self.alternate_thresholding_objective.score_needs_proba
-        ):
-            raise ValueError(
-                "Alternate thresholding objective must be a tuneable objective and cannot need probabilities!",
-            )
-        if self.data_splitter is not None and not issubclass(
-            self.data_splitter.__class__,
-            BaseCrossValidator,
-        ):
-            raise ValueError("Not a valid data splitter")
-        if not objective.is_defined_for_problem_type(self.problem_type):
-            raise ValueError(
-                "Given objective {} is not compatible with a {} problem.".format(
-                    self.objective.name,
-                    self.problem_type.value,
-                ),
-            )
-        if additional_objectives is None:
-            additional_objectives = get_optimization_objectives(self.problem_type)
-            # if our main objective is part of default set of objectives for problem_type, remove it
-            existing_main_objective = next(
-                (
-                    obj
-                    for obj in additional_objectives
-                    if obj.name == self.objective.name
-                ),
-                None,
-            )
-            if existing_main_objective is not None:
-                additional_objectives.remove(existing_main_objective)
-        else:
-            additional_objectives = [get_objective(o) for o in additional_objectives]
-        additional_objectives = [
-            self._validate_objective(obj) for obj in additional_objectives
-        ]
-        self.additional_objectives = additional_objectives
-        self.objective_name_to_class = {
-            o.name: o for o in [self.objective] + self.additional_objectives
-        }
 
         if not isinstance(max_time, (int, float, str, type(None))):
             raise TypeError(
                 f"Parameter max_time must be a float, int, string or None. Received {type(max_time)} with value {str(max_time)}..",
             )
         if isinstance(max_time, (int, float)) and max_time < 0:
             raise ValueError(
@@ -646,15 +609,14 @@
         self.allowed_component_graphs = allowed_component_graphs
         self.allowed_model_families = allowed_model_families
         self.allow_long_running_models = allow_long_running_models
         self._start = 0.0
         self._baseline_cv_scores = {}
         self.show_batch_output = False
 
-        self._validate_problem_type()
         self.problem_configuration = self._validate_problem_configuration(
             problem_configuration,
         )
         self._train_best_pipeline = train_best_pipeline
         self._best_pipeline = None
         self._searched = False
 
@@ -676,14 +638,15 @@
                 self.logger.info(
                     f"Created a holdout dataset with {len(X_holdout)} rows. Training dataset has {len(X_train)} rows.",
                 )
             else:
                 self.logger.info(
                     f"Dataset size is too small to create holdout set. Minimum dataset size is {self._HOLDOUT_SET_MIN_ROWS} rows, X_train has {len(X_train)} rows. Holdout set evaluation is disabled.",
                 )
+
         # Set holdout data in AutoML search if provided as parameter
         self.X_train = infer_feature_types(X_train)
         self.y_train = infer_feature_types(y_train)
         self.X_holdout = (
             infer_feature_types(X_holdout) if X_holdout is not None else None
         )
         self.y_holdout = (
@@ -695,14 +658,19 @@
                 "AutoMLSearch will use mean CV score to rank pipelines.",
             )
         else:
             self.logger.info(
                 "AutoMLSearch will use the holdout set to score and rank pipelines.",
             )
 
+        if self.data_splitter is not None and not issubclass(
+            self.data_splitter.__class__,
+            BaseCrossValidator,
+        ):
+            raise ValueError("Not a valid data splitter")
         default_data_splitter = make_data_splitter(
             self.X_train,
             self.y_train,
             self.problem_type,
             self.problem_configuration,
             n_splits=3,
             shuffle=True,
@@ -723,14 +691,114 @@
                     {"use_covariates": Categorical([False])},
                 )
             elif not user_arima_hyperparams:
                 self.search_parameters[ARIMARegressor.name] = {
                     "use_covariates": Categorical([False]),
                 }
 
+        def _is_imbalanced(X, y, problem_type):
+            if problem_type != ProblemTypes.MULTICLASS:
+                return False
+            imbalance_data_check = ClassImbalanceDataCheck()
+            results = imbalance_data_check.validate(X, y)
+            return bool(len(results))
+
+        recommendation_objectives = {}
+        if use_recommendation:
+            imbalanced = _is_imbalanced(self.X_train, self.y_train, self.problem_type)
+            default_objectives = get_default_recommendation_objectives(problem_type)
+            if include_recommendation is not None:
+                if not isinstance(include_recommendation, list):
+                    raise ValueError(
+                        "Objectives to include from the recommendation score should be a list",
+                    )
+                for include_objective in include_recommendation:
+                    include_objective = get_objective(include_objective)
+                    if include_objective.name in default_objectives:
+                        self.logger.warning(
+                            f"Objective to include {include_objective} is already one of the default objectives being evaluated. No behavior will be changed.",
+                        )
+            if exclude_recommendation is not None and not isinstance(
+                exclude_recommendation,
+                list,
+            ):
+                raise ValueError(
+                    "Objectives to exclude from the recommendation score should be a list",
+                )
+            recommendation_objectives = organize_objectives(
+                self.problem_type,
+                include_recommendation,
+                exclude_recommendation,
+                imbalanced,
+            )
+        self.use_recommendation = use_recommendation
+        self.recommendation_objectives = recommendation_objectives
+
+        if objective == "auto":
+            objective = get_default_primary_search_objective(self.problem_type.value)
+        objective = get_objective(objective, return_instance=False)
+        self.objective = self._validate_objective(objective)
+        self.alternate_thresholding_objective = None
+        if (
+            is_binary(self.problem_type)
+            and self.optimize_thresholds
+            and self.objective.score_needs_proba
+        ):
+            self.alternate_thresholding_objective = get_objective(
+                alternate_thresholding_objective,
+                return_instance=True,
+            )
+        if (
+            self.alternate_thresholding_objective is not None
+            and self.alternate_thresholding_objective.score_needs_proba
+        ):
+            raise ValueError(
+                "Alternate thresholding objective must be a tuneable objective and cannot need probabilities!",
+            )
+        if not objective.is_defined_for_problem_type(self.problem_type):
+            raise ValueError(
+                "Given objective {} is not compatible with a {} problem.".format(
+                    self.objective.name,
+                    self.problem_type.value,
+                ),
+            )
+        if additional_objectives is None:
+            additional_objectives = get_optimization_objectives(self.problem_type)
+            # if our main objective is part of default set of objectives for problem_type, remove it
+            existing_main_objective = next(
+                (
+                    obj
+                    for obj in additional_objectives
+                    if obj.name == self.objective.name
+                ),
+                None,
+            )
+            if existing_main_objective is not None:
+                additional_objectives.remove(existing_main_objective)
+        else:
+            additional_objectives = [get_objective(o) for o in additional_objectives]
+        additional_objectives = [
+            self._validate_objective(obj) for obj in additional_objectives
+        ]
+        additional_objective_names = [
+            objective.name for objective in additional_objectives
+        ]
+        for recommendation_obj in self.recommendation_objectives:
+            if (
+                recommendation_obj not in additional_objective_names
+                and recommendation_obj != existing_main_objective.name
+            ):
+                additional_objectives.append(get_objective(recommendation_obj))
+        self.additional_objectives = additional_objectives
+        self.objective_name_to_class = {
+            o.name: o for o in [self.objective] + self.additional_objectives
+        }
+
+        self._validate_problem_type()
+
         self.search_iteration_plot = None
         self._interrupted = False
         internal_search_parameters = copy.copy(self.search_parameters)
 
         if self.problem_configuration:
             internal_search_parameters.update({"pipeline": self.problem_configuration})
 
@@ -1626,18 +1694,106 @@
         rankings_df = pd.DataFrame(self._results["pipeline_results"].values())
         rankings_df = rankings_df[pipeline_results_cols]
         rankings_df.insert(
             2,
             "search_order",
             pd.Series(self._results["search_order"]),
         )  # place search_order after pipeline_name
-        rankings_df.sort_values("ranking_score", ascending=ascending, inplace=True)
+
+        ranking_column = "ranking_score"
+        if self.use_recommendation:
+            recommendation_scores = self.get_recommendation_scores()
+            ranking_column = "recommendation_score"
+            ascending = False
+            rankings_df.insert(
+                3,
+                "recommendation_score",
+                pd.Series(recommendation_scores.values()),
+            )
+
+        rankings_df.sort_values(ranking_column, ascending=ascending, inplace=True)
         rankings_df.reset_index(drop=True, inplace=True)
         return rankings_df
 
+    def get_recommendation_scores(
+        self,
+        priority=None,
+        custom_weights=None,
+        use_pipeline_names=False,
+    ):
+        """Calculates recommendation scores for all pipelines in the search results.
+
+        Args:
+            priority (str): An optional name of a priority objective that should be given heavier weight (of 0.5)
+                than the other objectives contributing to the score. Defaults to None, where all objectives are
+                weighted equally.
+            custom_weights (dict[str,float]): A dictionary mapping objective names to corresponding weights between 0 and 1.
+                Should not be used at the same time as prioritized_objective. Defaults to None.
+            use_pipeline_names (bool): Whether or not to return the pipeline names instead of ids as the keys
+                to the recommendation score dictionary. Defaults to False.
+
+        Returns:
+            A dictionary mapping pipeline IDs to recommendation scores
+        """
+
+        def _get_scores_and_max_min(objectives_to_evaluate):
+            all_scores = {}
+            max_scores = {objective: 0 for objective in objectives_to_evaluate}
+            min_scores = {objective: 0 for objective in objectives_to_evaluate}
+
+            for pl_id, pl_results in self._results["pipeline_results"].items():
+                ranking_results = pl_results["ranking_additional_objectives"]
+                for objective in objectives_to_evaluate:
+                    objective_obj = get_objective(objective)
+                    if (
+                        objective_obj.is_bounded_like_percentage
+                        or objective_obj.name == "R2"
+                    ):
+                        continue
+                    max_scores[objective] = max(
+                        max_scores[objective],
+                        ranking_results[objective],
+                    )
+                    min_scores[objective] = min(
+                        min_scores[objective],
+                        ranking_results[objective],
+                    )
+                all_scores[pl_id] = {
+                    objective: ranking_results[objective]
+                    for objective in objectives_to_evaluate
+                }
+            return all_scores, max_scores, min_scores
+
+        if len(self.recommendation_objectives) == 0:
+            self.recommendation_objectives = get_default_recommendation_objectives(
+                self.problem_type,
+            )
+        all_scores, max_scores, min_scores = _get_scores_and_max_min(
+            self.recommendation_objectives,
+        )
+        recommendation_scores = {}
+        for pipeline_id, pipeline_scores in all_scores.items():
+            rescaled_scores = normalize_objectives(
+                pipeline_scores,
+                max_scores,
+                min_scores,
+            )
+            score = recommendation_score(
+                rescaled_scores,
+                priority,
+                custom_weights,
+            )
+            recommendation_scores[pipeline_id] = score
+        if use_pipeline_names:
+            recommendation_scores = {
+                self.get_pipeline(pipeline_id).estimator.name: score
+                for pipeline_id, score in recommendation_scores.items()
+            }
+        return recommendation_scores
+
     @property
     def best_pipeline(self):
         """Returns a trained instance of the best pipeline and parameters found during automl search. If `train_best_pipeline` is set to False, returns an untrained pipeline instance.
 
         Returns:
             PipelineBase: A trained instance of the best pipeline and parameters found during automl search. If `train_best_pipeline` is set to False, returns an untrained pipeline instance.
```

### Comparing `evalml-0.75.0/evalml/automl/callbacks.py` & `evalml-0.76.0/evalml/automl/callbacks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/engine/cf_engine.py` & `evalml-0.76.0/evalml/automl/engine/cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/engine/dask_engine.py` & `evalml-0.76.0/evalml/automl/engine/dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/engine/engine_base.py` & `evalml-0.76.0/evalml/automl/engine/engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/engine/sequential_engine.py` & `evalml-0.76.0/evalml/automl/engine/sequential_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/pipeline_search_plots.py` & `evalml-0.76.0/evalml/automl/pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/progress.py` & `evalml-0.76.0/evalml/automl/progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/automl/utils.py` & `evalml-0.76.0/evalml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/__init__.py` & `evalml-0.76.0/evalml/data_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/class_imbalance_data_check.py` & `evalml-0.76.0/evalml/data_checks/class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/data_check.py` & `evalml-0.76.0/evalml/data_checks/data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/data_check_action.py` & `evalml-0.76.0/evalml/data_checks/data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/data_check_action_code.py` & `evalml-0.76.0/evalml/data_checks/data_check_action_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/data_check_action_option.py` & `evalml-0.76.0/evalml/data_checks/data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/data_check_message.py` & `evalml-0.76.0/evalml/data_checks/data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/data_check_message_code.py` & `evalml-0.76.0/evalml/data_checks/data_check_message_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/data_checks.py` & `evalml-0.76.0/evalml/data_checks/data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/datetime_format_data_check.py` & `evalml-0.76.0/evalml/data_checks/datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/default_data_checks.py` & `evalml-0.76.0/evalml/data_checks/default_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/id_columns_data_check.py` & `evalml-0.76.0/evalml/data_checks/id_columns_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/invalid_target_data_check.py` & `evalml-0.76.0/evalml/data_checks/invalid_target_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/multicollinearity_data_check.py` & `evalml-0.76.0/evalml/data_checks/multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/no_variance_data_check.py` & `evalml-0.76.0/evalml/data_checks/no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/null_data_check.py` & `evalml-0.76.0/evalml/data_checks/null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/outliers_data_check.py` & `evalml-0.76.0/evalml/data_checks/outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/sparsity_data_check.py` & `evalml-0.76.0/evalml/data_checks/sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/target_distribution_data_check.py` & `evalml-0.76.0/evalml/data_checks/target_distribution_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/target_leakage_data_check.py` & `evalml-0.76.0/evalml/data_checks/target_leakage_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/ts_parameters_data_check.py` & `evalml-0.76.0/evalml/data_checks/ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/ts_splitting_data_check.py` & `evalml-0.76.0/evalml/data_checks/ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/uniqueness_data_check.py` & `evalml-0.76.0/evalml/data_checks/uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/data_checks/utils.py` & `evalml-0.76.0/evalml/data_checks/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/breast_cancer.py` & `evalml-0.76.0/evalml/demos/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/churn.py` & `evalml-0.76.0/evalml/demos/churn.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/data/churn.csv` & `evalml-0.76.0/evalml/demos/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/data/daily-min-temperatures.csv` & `evalml-0.76.0/evalml/demos/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/data/fraud_transactions.csv.gz` & `evalml-0.76.0/evalml/demos/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/diabetes.py` & `evalml-0.76.0/evalml/demos/diabetes.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/fraud.py` & `evalml-0.76.0/evalml/demos/fraud.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/weather.py` & `evalml-0.76.0/evalml/demos/weather.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/demos/wine.py` & `evalml-0.76.0/evalml/demos/wine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/exceptions/__init__.py` & `evalml-0.76.0/evalml/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/exceptions/exceptions.py` & `evalml-0.76.0/evalml/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_family/model_family.py` & `evalml-0.76.0/evalml/model_family/model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_family/utils.py` & `evalml-0.76.0/evalml/model_family/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/__init__.py` & `evalml-0.76.0/evalml/model_understanding/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py` & `evalml-0.76.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/_partial_dependence_utils.py` & `evalml-0.76.0/evalml/model_understanding/_partial_dependence_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/decision_boundary.py` & `evalml-0.76.0/evalml/model_understanding/decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/feature_explanations.py` & `evalml-0.76.0/evalml/model_understanding/feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/force_plots.py` & `evalml-0.76.0/evalml/model_understanding/force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/metrics.py` & `evalml-0.76.0/evalml/model_understanding/metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/partial_dependence_functions.py` & `evalml-0.76.0/evalml/model_understanding/partial_dependence_functions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/permutation_importance.py` & `evalml-0.76.0/evalml/model_understanding/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/prediction_explanations/_algorithms.py` & `evalml-0.76.0/evalml/model_understanding/prediction_explanations/_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py` & `evalml-0.76.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/prediction_explanations/_user_interface.py` & `evalml-0.76.0/evalml/model_understanding/prediction_explanations/_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/prediction_explanations/explainers.py` & `evalml-0.76.0/evalml/model_understanding/prediction_explanations/explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/model_understanding/visualizations.py` & `evalml-0.76.0/evalml/model_understanding/visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/objectives/__init__.py` & `evalml-0.76.0/evalml/objectives/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,18 @@
     RecallMacro,
     RecallMicro,
     RecallWeighted,
 )
 from evalml.objectives.utils import (
     get_objective,
     get_core_objectives,
+    get_default_recommendation_objectives,
     get_all_objective_names,
     get_non_core_objectives,
     get_core_objective_names,
     get_optimization_objectives,
     get_ranking_objectives,
+    normalize_objectives,
+    organize_objectives,
     ranking_only_objectives,
+    recommendation_score,
 )
```

### Comparing `evalml-0.75.0/evalml/objectives/binary_classification_objective.py` & `evalml-0.76.0/evalml/objectives/binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/objectives/cost_benefit_matrix.py` & `evalml-0.76.0/evalml/objectives/cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/objectives/fraud_cost.py` & `evalml-0.76.0/evalml/objectives/fraud_cost.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/objectives/lead_scoring.py` & `evalml-0.76.0/evalml/objectives/lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/objectives/objective_base.py` & `evalml-0.76.0/evalml/objectives/objective_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/objectives/sensitivity_low_alert.py` & `evalml-0.76.0/evalml/objectives/sensitivity_low_alert.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/objectives/standard_metrics.py` & `evalml-0.76.0/evalml/objectives/standard_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -796,15 +796,15 @@
         >>> np.testing.assert_almost_equal(MAE().objective_function(y_true, y_pred), 0.2727272)
     """
 
     name = "MAE"
     greater_is_better = False
     score_needs_proba = False
     perfect_score = 0.0
-    is_bounded_like_percentage = True  # Range [0, Inf)
+    is_bounded_like_percentage = False  # Range [0, Inf)
     expected_range = [0, float("inf")]
 
     def objective_function(self, y_true, y_predicted, X=None, sample_weight=None):
         """Objective function for mean absolute error for regression."""
         return metrics.mean_absolute_error(
             y_true,
             y_predicted,
```

### Comparing `evalml-0.75.0/evalml/pipelines/__init__.py` & `evalml-0.76.0/evalml/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/binary_classification_pipeline.py` & `evalml-0.76.0/evalml/pipelines/binary_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/binary_classification_pipeline_mixin.py` & `evalml-0.76.0/evalml/pipelines/binary_classification_pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/classification_pipeline.py` & `evalml-0.76.0/evalml/pipelines/classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/component_graph.py` & `evalml-0.76.0/evalml/pipelines/component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/__init__.py` & `evalml-0.76.0/evalml/pipelines/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/component_base.py` & `evalml-0.76.0/evalml/pipelines/components/component_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/component_base_meta.py` & `evalml-0.76.0/evalml/pipelines/components/component_base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py` & `evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/__init__.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/__init__.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/estimator.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/__init__.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/et_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py` & `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/__init__.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/column_selectors.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/column_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/encoders/label_encoder.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/encoders/label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/encoders/target_encoder.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/encoders/target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/__init__.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/__init__.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/imputer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/target_imputer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/target_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/__init__.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/lsa.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/samplers/base_sampler.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/samplers/oversampler.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/samplers/oversampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/samplers/undersampler.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/samplers/undersampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/transformers/transformer.py` & `evalml-0.76.0/evalml/pipelines/components/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/components/utils.py` & `evalml-0.76.0/evalml/pipelines/components/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/multiclass_classification_pipeline.py` & `evalml-0.76.0/evalml/pipelines/multiclass_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/pipeline_base.py` & `evalml-0.76.0/evalml/pipelines/pipeline_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import inspect
 import logging
 import os
 import sys
 import traceback
 from abc import ABC, abstractmethod
 from collections import OrderedDict
+from io import BytesIO
+from typing import Union
 
 import cloudpickle
 import numpy as np
 import pandas as pd
 
 from evalml.exceptions import ObjectiveCreationError, PipelineScoreError
 from evalml.objectives import get_objective
@@ -624,23 +626,26 @@
             file_path (str): Location to save file.
             pickle_protocol (int): The pickle data stream format.
         """
         with open(file_path, "wb") as f:
             cloudpickle.dump(self, f, protocol=pickle_protocol)
 
     @staticmethod
-    def load(file_path):
+    def load(file_path: Union[str, BytesIO]):
         """Loads pipeline at file path.
 
         Args:
-            file_path (str): Location to load file.
+            file_path (str|BytesIO): load filepath or a BytesIO object.
 
         Returns:
             PipelineBase object
         """
+        if isinstance(file_path, BytesIO):
+            return cloudpickle.load(file_path)
+
         with open(file_path, "rb") as f:
             return cloudpickle.load(f)
 
     def clone(self):
         """Constructs a new pipeline with the same components, parameters, and random seed.
 
         Returns:
```

### Comparing `evalml-0.75.0/evalml/pipelines/pipeline_meta.py` & `evalml-0.76.0/evalml/pipelines/pipeline_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/regression_pipeline.py` & `evalml-0.76.0/evalml/pipelines/regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/time_series_classification_pipelines.py` & `evalml-0.76.0/evalml/pipelines/time_series_classification_pipelines.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/time_series_pipeline_base.py` & `evalml-0.76.0/evalml/pipelines/time_series_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/time_series_regression_pipeline.py` & `evalml-0.76.0/evalml/pipelines/time_series_regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/pipelines/utils.py` & `evalml-0.76.0/evalml/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/preprocessing/data_splitters/no_split.py` & `evalml-0.76.0/evalml/preprocessing/data_splitters/no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/preprocessing/data_splitters/sk_splitters.py` & `evalml-0.76.0/evalml/preprocessing/data_splitters/sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/preprocessing/data_splitters/time_series_split.py` & `evalml-0.76.0/evalml/preprocessing/data_splitters/time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/preprocessing/data_splitters/training_validation_split.py` & `evalml-0.76.0/evalml/preprocessing/data_splitters/training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/preprocessing/utils.py` & `evalml-0.76.0/evalml/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/problem_types/problem_types.py` & `evalml-0.76.0/evalml/problem_types/problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/problem_types/utils.py` & `evalml-0.76.0/evalml/problem_types/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/dask_test_utils.py` & `evalml-0.76.0/evalml/tests/automl_tests/dask_test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py` & `evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py` & `evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py` & `evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_automl.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_automl.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from evalml.automl.utils import (
     _LARGE_DATA_PERCENT_VALIDATION,
     _LARGE_DATA_ROW_THRESHOLD,
     get_default_primary_search_objective,
 )
 from evalml.exceptions import (
     AutoMLSearchException,
+    ObjectiveNotFoundError,
     ParameterNotUsedWarning,
     PipelineNotFoundError,
     PipelineNotYetFittedError,
     PipelineScoreError,
 )
 from evalml.model_family import ModelFamily
 from evalml.objectives import (
@@ -47,14 +48,15 @@
     CostBenefitMatrix,
     FraudCost,
     RegressionObjective,
 )
 from evalml.objectives.utils import (
     get_all_objective_names,
     get_core_objectives,
+    get_default_recommendation_objectives,
     get_non_core_objectives,
     get_objective,
 )
 from evalml.pipelines import (
     BinaryClassificationPipeline,
     ComponentGraph,
     MulticlassClassificationPipeline,
@@ -3155,29 +3157,37 @@
     assert search.objective not in only_positive
     assert all([obj not in only_positive for obj in search.additional_objectives])
 
 
 @pytest.mark.parametrize("non_core_objective", get_non_core_objectives())
 def test_automl_validate_objective(non_core_objective, X_y_regression):
     X, y = X_y_regression
+    problem_configuration = {
+        "time_index": "Date",
+        "gap": 0,
+        "max_delay": 0,
+        "forecast_horizon": 2,
+    }
 
     with pytest.raises(ValueError, match="is not allowed in AutoML!"):
         AutoMLSearch(
             X_train=X,
             y_train=y,
             problem_type=non_core_objective.problem_types[0],
             objective=non_core_objective.name,
+            problem_configuration=problem_configuration,
         )
 
     with pytest.raises(ValueError, match="is not allowed in AutoML!"):
         AutoMLSearch(
             X_train=X,
             y_train=y,
             problem_type=non_core_objective.problem_types[0],
             additional_objectives=[non_core_objective.name],
+            problem_configuration=problem_configuration,
         )
 
 
 def test_automl_pipeline_params_simple(AutoMLTestEnv, X_y_binary):
     X, y = X_y_binary
     params = {
         "Imputer": {"numeric_impute_strategy": "most_frequent"},
@@ -5476,7 +5486,207 @@
     assert "holdout_score" in automl.rankings
     assert "holdout_score" in automl.full_rankings
     assert_series_equal(
         automl.rankings["holdout_score"],
         automl.rankings["ranking_score"],
         check_names=False,
     )
+
+
+def test_get_recommendation_scores(X_y_binary):
+    X, y = X_y_binary
+
+    # Test that we can still get recommendation scores without setting use_recommendation
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type="binary",
+    )
+    automl.search()
+
+    scores = automl.get_recommendation_scores()
+    assert isinstance(scores, dict)
+    assert scores.keys() == automl.results["pipeline_results"].keys()
+
+    # check that the output scores are between 0 and 100
+    for score in scores.values():
+        assert 0 <= score <= 100
+
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type="regression",
+        use_recommendation=True,
+        include_recommendation=["MedianAE", "MaxError"],
+        exclude_recommendation=["MAE"],
+    )
+    automl.search()
+
+    scores = automl.get_recommendation_scores(
+        priority="MaxError",
+    )
+    for score in scores.values():
+        assert 0 <= score <= 100
+    for pipeline_id in scores.keys():
+        assert isinstance(pipeline_id, int)
+
+    scores = automl.get_recommendation_scores(use_pipeline_names=True)
+    for pipeline_name in scores.keys():
+        assert isinstance(pipeline_name, str)
+
+
+def test_recommendation_score_argument_errors(X_y_binary, caplog):
+    caplog.clear()
+    X, y = X_y_binary
+
+    with pytest.raises(
+        ValueError,
+        match="Objectives to include from the recommendation score should be a list",
+    ):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type="binary",
+            use_recommendation=True,
+            include_recommendation="Not a list",
+        )
+    with pytest.raises(
+        ValueError,
+        match="Objectives to exclude from the recommendation score should be a list",
+    ):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type="binary",
+            use_recommendation=True,
+            exclude_recommendation="Not a list",
+        )
+    with pytest.raises(ObjectiveNotFoundError, match="not a valid Objective!"):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type="binary",
+            use_recommendation=True,
+            include_recommendation=["Does not exist"],
+        )
+    with pytest.raises(ValueError, match="not defined for binary"):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type="binary",
+            use_recommendation=True,
+            include_recommendation=["R2"],
+        )
+    with pytest.raises(ValueError, match="Cannot exclude objective"):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type="binary",
+            use_recommendation=True,
+            exclude_recommendation=["Precision"],
+        )
+    AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type="binary",
+        use_recommendation=True,
+        include_recommendation=["F1"],
+    )
+    assert "already one of the default objectives" in caplog.text
+
+
+def test_recommendation_include_non_optimization(X_y_binary):
+    X, y = X_y_binary
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type="binary",
+        use_recommendation=True,
+        include_recommendation=["Recall"],
+    )
+    assert "Recall" in automl.recommendation_objectives
+    assert get_objective("Recall") in automl.additional_objectives
+
+
+@pytest.mark.parametrize("imbalanced_data", [True, False])
+def test_use_recommendation_score_imbalanced(
+    imbalanced_data,
+    mock_imbalanced_data_X_y,
+    X_y_multi,
+):
+    if imbalanced_data:
+        X, y = mock_imbalanced_data_X_y("multiclass", "none", "small")
+        X = X[
+            :-300
+        ]  # Make the dataset more imbalanced, so that the data check flags it
+        y = y[:-300]
+    else:
+        X, y = X_y_multi
+
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type="multiclass",
+        use_recommendation=True,
+    )
+    objectives = get_default_recommendation_objectives(
+        "multiclass",
+        imbalanced=imbalanced_data,
+    )
+    assert automl.recommendation_objectives == objectives
+
+
+@pytest.mark.parametrize("use_recommendation", [False, True])
+def test_use_recommendation_score(AutoMLTestEnv, X_y_binary, use_recommendation):
+    X, y = X_y_binary
+
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type="binary",
+        use_recommendation=use_recommendation,
+    )
+    env = AutoMLTestEnv("binary")
+    objectives = get_default_recommendation_objectives("binary")
+    with env.test_context(
+        score_return_value={objective: 0.75 for objective in objectives},
+    ):
+        automl.search()
+    if not use_recommendation:
+        assert "recommendation_score" not in automl.rankings
+    else:
+        assert "recommendation_score" in automl.rankings
+
+
+def test_recommendation_score_include_exclude(AutoMLTestEnv, X_y_binary):
+    X, y = X_y_binary
+
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type="binary",
+        use_recommendation=True,
+    )
+    env = AutoMLTestEnv("binary")
+    objectives = get_default_recommendation_objectives("binary")
+    with env.test_context(
+        score_return_value={objective: 0.75 for objective in objectives},
+    ):
+        automl.search()
+    default_rankings = automl.rankings["recommendation_score"]
+
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type="binary",
+        use_recommendation=True,
+        include_recommendation=["Precision"],
+        exclude_recommendation=["F1", "AUC"],
+    )
+    objectives.update({"Precision"})
+    objectives = objectives - {"F1", "AUC"}
+    with env.test_context(
+        score_return_value={objective: 0.75 for objective in objectives},
+    ):
+        automl.search()
+    custom_rankings = automl.rankings["recommendation_score"]
+    assert all(default_rankings != custom_rankings)
```

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_automl_algorithm.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_classification.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_regression.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_automl_utils.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_automl_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_default_algorithm.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_default_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_engine_base.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_iterative_algorithm.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_iterative_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_pipeline_search_plots.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_progress.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_search.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_search_iterative.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_search_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/automl_tests/test_time_series_split.py` & `evalml-0.76.0/evalml/tests/automl_tests/test_time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py` & `evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py` & `evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py` & `evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_arima_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_arima_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_baseline_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_baseline_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_catboost_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_catboost_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_column_selector_transformers.py` & `evalml-0.76.0/evalml/tests/component_tests/test_column_selector_transformers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_components.py` & `evalml-0.76.0/evalml/tests/component_tests/test_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_datetime_featurizer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_decision_tree_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_decision_tree_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_drop_rows_transformer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_en_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_en_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_en_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_en_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_estimators.py` & `evalml-0.76.0/evalml/tests/component_tests/test_estimators.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_et_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_et_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_feature_selectors.py` & `evalml-0.76.0/evalml/tests/component_tests/test_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_featuretools.py` & `evalml-0.76.0/evalml/tests/component_tests/test_featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py` & `evalml-0.76.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_imputer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_knn_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_knn_imputer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_knn_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_label_encoder.py` & `evalml-0.76.0/evalml/tests/component_tests/test_label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_lda.py` & `evalml-0.76.0/evalml/tests/component_tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_lgbm_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_lgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_lgbm_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_lgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_log_transformer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_lsa.py` & `evalml-0.76.0/evalml/tests/component_tests/test_lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_natural_language_featurizer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_nullable_types_replacer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_nullable_types_replacer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_one_hot_encoder.py` & `evalml-0.76.0/evalml/tests/component_tests/test_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_ordinal_encoder.py` & `evalml-0.76.0/evalml/tests/component_tests/test_ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_oversampler.py` & `evalml-0.76.0/evalml/tests/component_tests/test_oversampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_pca.py` & `evalml-0.76.0/evalml/tests/component_tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_per_column_imputer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_prophet_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_simple_imputer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_simple_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_standard_scaler.py` & `evalml-0.76.0/evalml/tests/component_tests/test_standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_svm_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_svm_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_target_encoder.py` & `evalml-0.76.0/evalml/tests/component_tests/test_target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_target_imputer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_target_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_time_series_featurizer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_time_series_imputer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_time_series_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_time_series_regularizer.py` & `evalml-0.76.0/evalml/tests/component_tests/test_time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_undersampler.py` & `evalml-0.76.0/evalml/tests/component_tests/test_undersampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_utils.py` & `evalml-0.76.0/evalml/tests/component_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_xgboost_classifier.py` & `evalml-0.76.0/evalml/tests/component_tests/test_xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/component_tests/test_xgboost_regressor.py` & `evalml-0.76.0/evalml/tests/component_tests/test_xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/conftest.py` & `evalml-0.76.0/evalml/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1748,38 +1748,39 @@
 
         Args:
             problem_type (str): Either 'binary' or 'multiclass'
             categorical_columns (str): Determines how many categorical cols to use. Either 'all', 'some', or 'none'.
             size (str): Either 'large' or 'small'. 'large' returns a dataset of size 21,000, while 'small' returns a size of 4200
         """
         multiplier = 5 if size == "large" else 1
+        if problem_type == "binary":
+            targets = [0] * 3500 + [1] * 700
+        else:
+            targets = [0] * 3000 + [1] * 600 + [2] * 600
+        targets *= multiplier
+        y = ww.init_series(pd.Series(targets))
+
         col_names = [f"col_{i}" for i in range(100)]
         # generate X to be all int values
         X_dict = {
-            col_name: [i % (j + 1) for i in range(1, 100)]
+            col_name: [i % (j + 1) for i in range(1, len(y) + 1)]
             for j, col_name in enumerate(col_names)
         }
         X = pd.DataFrame(X_dict)
         if categorical_columns == "all":
             X.ww.init(logical_types={col_name: "Categorical" for col_name in col_names})
         elif categorical_columns == "some":
             X.ww.init(
                 logical_types={
                     col_name: "Categorical"
                     for col_name in col_names[: len(col_names) // 2]
                 },
             )
         else:
             X.ww.init()
-        if problem_type == "binary":
-            targets = [0] * 3500 + [1] * 700
-        else:
-            targets = [0] * 3000 + [1] * 600 + [2] * 600
-        targets *= multiplier
-        y = ww.init_series(pd.Series(targets))
         return X, y
 
     return _imbalanced_data_X_y
 
 
 class _AutoMLTestEnv:
     """A test environment that makes it easy to test automl behavior with patched pipeline computations.
```

### Comparing `evalml-0.75.0/evalml/tests/data/churn.csv` & `evalml-0.76.0/evalml/tests/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data/daily-min-temperatures.csv` & `evalml-0.76.0/evalml/tests/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data/fraud_transactions.csv.gz` & `evalml-0.76.0/evalml/tests/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data/tips.csv` & `evalml-0.76.0/evalml/tests/data/tips.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data/titanic.csv` & `evalml-0.76.0/evalml/tests/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_action.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_action_option.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_check_message.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_data_checks.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_null_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_outliers_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/data_checks_tests/test_utils.py` & `evalml-0.76.0/evalml/tests/data_checks_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/demo_tests/test_datasets.py` & `evalml-0.76.0/evalml/tests/demo_tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt` & `evalml-0.76.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt`

 * *Files 24% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 pyzmq==25.0.2
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
 scipy==1.9.1
 seaborn==0.12.2
 shap==0.41.0
 sktime==0.17.0
-statsmodels==0.13.5
+statsmodels==0.14.0
 texttable==1.6.7
 tomli==2.0.1
 vowpalwabbit==9.8.0
 woodwork==0.23.0
 xgboost==1.7.5
```

### Comparing `evalml-0.75.0/evalml/tests/dependency_update_check/minimum_requirements.txt` & `evalml-0.76.0/evalml/tests/dependency_update_check/minimum_requirements.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt` & `evalml-0.76.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py` & `evalml-0.76.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/integration_tests/test_nullable_types.py` & `evalml-0.76.0/evalml/tests/integration_tests/test_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/integration_tests/test_time_series_integration.py` & `evalml-0.76.0/evalml/tests/integration_tests/test_time_series_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_family_tests/test_model_family.py` & `evalml-0.76.0/evalml/tests/model_family_tests/test_model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/test_decision_boundary.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/test_decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/test_feature_explanations.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/test_feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/test_metrics.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/test_partial_dependence.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/test_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/test_permutation_importance.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/model_understanding_tests/test_visualizations.py` & `evalml-0.76.0/evalml/tests/model_understanding_tests/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/objective_tests/test_binary_classification_objective.py` & `evalml-0.76.0/evalml/tests/objective_tests/test_binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py` & `evalml-0.76.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/objective_tests/test_fraud_detection.py` & `evalml-0.76.0/evalml/tests/objective_tests/test_fraud_detection.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/objective_tests/test_lead_scoring.py` & `evalml-0.76.0/evalml/tests/objective_tests/test_lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/objective_tests/test_sla.py` & `evalml-0.76.0/evalml/tests/objective_tests/test_sla.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/objective_tests/test_standard_metrics.py` & `evalml-0.76.0/evalml/tests/objective_tests/test_standard_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/test_component_graph.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/test_component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/test_graphs.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/test_pipeline_utils.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/test_pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/test_pipelines.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/test_pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import io
 import os
 import pickle
 import re
+from typing import Union
 from unittest.mock import patch
 
 import cloudpickle
 import numpy as np
 import pandas as pd
 import pytest
 import woodwork as ww
@@ -123,21 +125,34 @@
     class TestPipelineWithoutComponentGraph(PipelineBase):
         pass
 
     with pytest.raises(TypeError):
         TestPipelineWithoutComponentGraph(parameters={})
 
 
-def test_serialization(X_y_binary, tmpdir, logistic_regression_binary_pipeline):
+@pytest.mark.parametrize("filetype", ["str", "BytesIO"])
+def test_serialization(
+    X_y_binary, tmpdir, logistic_regression_binary_pipeline, filetype
+):
     X, y = X_y_binary
     path = os.path.join(str(tmpdir), "pipe.pkl")
     pipeline = logistic_regression_binary_pipeline
     pipeline.fit(X, y)
+
     pipeline.save(path)
-    assert pipeline.score(X, y, ["precision"]) == PipelineBase.load(path).score(
+    data_path: Union[str, io.BytesIO]
+
+    data_path = path
+
+    if filetype == "BytesIO":
+        with open(path, "rb") as f:
+            file_contents = f.read()
+        data_path = io.BytesIO(file_contents)
+
+    assert pipeline.score(X, y, ["precision"]) == PipelineBase.load(data_path).score(
         X,
         y,
         ["precision"],
     )
 
 
 @patch("cloudpickle.dump")
```

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py` & `evalml-0.76.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/preprocessing_tests/test_no_split.py` & `evalml-0.76.0/evalml/tests/preprocessing_tests/test_no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/preprocessing_tests/test_sk_splitters.py` & `evalml-0.76.0/evalml/tests/preprocessing_tests/test_sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/preprocessing_tests/test_split_data.py` & `evalml-0.76.0/evalml/tests/preprocessing_tests/test_split_data.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/preprocessing_tests/test_training_validation_split.py` & `evalml-0.76.0/evalml/tests/preprocessing_tests/test_training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/problem_type_tests/test_problem_types.py` & `evalml-0.76.0/evalml/tests/problem_type_tests/test_problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/test_all_test_dirs_included.py` & `evalml-0.76.0/evalml/tests/test_all_test_dirs_included.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/tuner_tests/test_grid_search_tuner.py` & `evalml-0.76.0/evalml/tests/tuner_tests/test_grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/tuner_tests/test_random_search_tuner.py` & `evalml-0.76.0/evalml/tests/tuner_tests/test_random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/tuner_tests/test_skopt_tuner.py` & `evalml-0.76.0/evalml/tests/tuner_tests/test_skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/utils_tests/test_cli_utils.py` & `evalml-0.76.0/evalml/tests/utils_tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/utils_tests/test_gen_utils.py` & `evalml-0.76.0/evalml/tests/utils_tests/test_gen_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/utils_tests/test_logger.py` & `evalml-0.76.0/evalml/tests/utils_tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/utils_tests/test_nullable_type_utils.py` & `evalml-0.76.0/evalml/tests/utils_tests/test_nullable_type_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tests/utils_tests/test_woodwork_utils.py` & `evalml-0.76.0/evalml/tests/utils_tests/test_woodwork_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tuners/grid_search_tuner.py` & `evalml-0.76.0/evalml/tuners/grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tuners/random_search_tuner.py` & `evalml-0.76.0/evalml/tuners/random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tuners/skopt_tuner.py` & `evalml-0.76.0/evalml/tuners/skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/tuners/tuner.py` & `evalml-0.76.0/evalml/tuners/tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/utils/__init__.py` & `evalml-0.76.0/evalml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/utils/base_meta.py` & `evalml-0.76.0/evalml/utils/base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/utils/cli_utils.py` & `evalml-0.76.0/evalml/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/utils/gen_utils.py` & `evalml-0.76.0/evalml/utils/gen_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/utils/logger.py` & `evalml-0.76.0/evalml/utils/logger.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/utils/nullable_type_utils.py` & `evalml-0.76.0/evalml/utils/nullable_type_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml/utils/woodwork_utils.py` & `evalml-0.76.0/evalml/utils/woodwork_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml.egg-info/PKG-INFO` & `evalml-0.76.0/evalml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.75.0
+Version: 0.76.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.75.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.76.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.75.0/evalml.egg-info/SOURCES.txt` & `evalml-0.76.0/evalml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.75.0/evalml.egg-info/requires.txt` & `evalml-0.76.0/evalml.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-numpy>=1.21.0
+numpy<=1.23.5,>=1.21.0
 pandas>=1.5.0
 scipy>=1.5.0
 scikit-learn>=1.2.2
 scikit-optimize>=0.9.0
 pyzmq>=20.0.0
 colorama>=0.4.4
 cloudpickle>=1.5.0
```

### Comparing `evalml-0.75.0/pyproject.toml` & `evalml-0.76.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 maintainers = [
     {name="Alteryx, Inc.", email="open_source_support@alteryx.com"}
 ]
 keywords = ["data science", "machine learning", "optimization", "automl"]
 license = {file = "LICENSE"}
 requires-python = ">=3.8,<4"
 dependencies = [
-    "numpy >= 1.21.0",
+    "numpy >= 1.21.0, <=1.23.5",
     "pandas >= 1.5.0",
     "scipy >= 1.5.0",
     "scikit-learn >= 1.2.2",
     "scikit-optimize >= 0.9.0",
     "pyzmq >= 20.0.0",
     "colorama >= 0.4.4",
     "cloudpickle >= 1.5.0",
```

