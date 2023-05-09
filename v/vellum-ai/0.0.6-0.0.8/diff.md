# Comparing `tmp/vellum_ai-0.0.6.tar.gz` & `tmp/vellum_ai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.0.6.tar", max compression
+gzip compressed data, was "vellum_ai-0.0.8.tar", max compression
```

## Comparing `vellum_ai-0.0.6.tar` & `vellum_ai-0.0.8.tar`

### file list

```diff
@@ -1,61 +1,71 @@
--rw-r--r--   0        0        0      413 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2675 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/__init__.py
--rw-r--r--   0        0        0     8763 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/client.py
--rw-r--r--   0        0        0      348 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      498 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/environment.py
--rw-r--r--   0        0        0        0 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/py.typed
--rw-r--r--   0        0        0      148 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0     5769 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/model_versions/__init__.py
--rw-r--r--   0        0        0     2282 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/model_versions/client.py
--rw-r--r--   0        0        0     3891 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/__init__.py
--rw-r--r--   0        0        0      830 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/block_type_enum.py
--rw-r--r--   0        0        0      825 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/chat_message_request.py
--rw-r--r--   0        0        0      645 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/chat_message_role.py
--rw-r--r--   0        0        0     1117 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/document.py
--rw-r--r--   0        0        0     1268 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1745 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      639 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      831 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0      929 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1514 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1246 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1326 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0      992 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      840 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0     1012 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      435 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0      483 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_type_enum.py
--rw-r--r--   0        0        0     1241 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_build_config.py
--rw-r--r--   0        0        0     1021 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_exec_config_parameters.py
--rw-r--r--   0        0        0     1421 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_exec_config_read.py
--rw-r--r--   0        0        0     2056 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_read.py
--rw-r--r--   0        0        0      895 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_read_status_enum.py
--rw-r--r--   0        0        0      934 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_sandbox_snapshot.py
--rw-r--r--   0        0        0      890 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0      891 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      939 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0      835 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0      934 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/prompt_template_block.py
--rw-r--r--   0        0        0      860 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/prompt_template_block_data.py
--rw-r--r--   0        0        0      986 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/prompt_template_block_properties.py
--rw-r--r--   0        0        0     1039 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/provider_enum.py
--rw-r--r--   0        0        0      829 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0      881 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0     1486 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0      952 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1157 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_result.py
--rw-r--r--   0        0        0      834 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0      961 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     2009 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0      351 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/slim_document_status_enum.py
--rw-r--r--   0        0        0     1778 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      772 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0      763 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      837 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 vellum_ai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2980 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/README.md
+-rw-r--r--   0        0        0      433 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3041 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/__init__.py
+-rw-r--r--   0        0        0     9151 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/client.py
+-rw-r--r--   0        0        0      348 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      498 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/environment.py
+-rw-r--r--   0        0        0        0 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/py.typed
+-rw-r--r--   0        0        0      172 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0     5769 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/model_versions/__init__.py
+-rw-r--r--   0        0        0     2282 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/model_versions/client.py
+-rw-r--r--   0        0        0       65 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/resources/sandboxes/__init__.py
+-rw-r--r--   0        0        0     3633 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/resources/sandboxes/client.py
+-rw-r--r--   0        0        0     4425 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/block_type_enum.py
+-rw-r--r--   0        0        0      818 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/chat_message.py
+-rw-r--r--   0        0        0      825 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/chat_message_request.py
+-rw-r--r--   0        0        0      645 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/chat_message_role.py
+-rw-r--r--   0        0        0     1117 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/document.py
+-rw-r--r--   0        0        0     1268 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1745 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      639 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      831 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0      929 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1514 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1246 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1326 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0      992 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      840 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0     1012 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      435 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0      483 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_type_enum.py
+-rw-r--r--   0        0        0     1241 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_build_config.py
+-rw-r--r--   0        0        0     1021 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_exec_config_parameters.py
+-rw-r--r--   0        0        0     1469 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_exec_config_read.py
+-rw-r--r--   0        0        0     2056 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_read.py
+-rw-r--r--   0        0        0      895 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_read_status_enum.py
+-rw-r--r--   0        0        0     1052 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_sandbox_snapshot.py
+-rw-r--r--   0        0        0      890 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0      891 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      939 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0      835 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0      946 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/prompt_template_block.py
+-rw-r--r--   0        0        0      860 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/prompt_template_block_data.py
+-rw-r--r--   0        0        0      950 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/prompt_template_block_properties.py
+-rw-r--r--   0        0        0     1039 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/provider_enum.py
+-rw-r--r--   0        0        0      943 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/sandbox_input.py
+-rw-r--r--   0        0        0      972 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/sandbox_input_request.py
+-rw-r--r--   0        0        0      802 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/sandbox_metric_input_params.py
+-rw-r--r--   0        0        0      809 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/sandbox_metric_input_params_request.py
+-rw-r--r--   0        0        0     1096 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/sandbox_scenario.py
+-rw-r--r--   0        0        0      829 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0      881 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0     1486 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0      952 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1157 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0      834 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0      961 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     2009 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0      351 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/slim_document_status_enum.py
+-rw-r--r--   0        0        0     1778 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      772 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0      468 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/type_enum.py
+-rw-r--r--   0        0        0      763 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      837 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 vellum_ai-0.0.8/PKG-INFO
```

### Comparing `vellum_ai-0.0.6/src/vellum/__init__.py` & `vellum_ai-0.0.8/src/vellum/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .environment import VellumEnvironment
-from .resources import documents, model_versions
+from .resources import documents, model_versions, sandboxes
 from .types import (
     BlockTypeEnum,
+    ChatMessage,
     ChatMessageRequest,
     ChatMessageRole,
     Document,
     DocumentDocumentToDocumentIndex,
     EnrichedNormalizedCompletion,
     FinishReasonEnum,
     GenerateErrorResponse,
@@ -30,31 +31,38 @@
     NormalizedTokenLogProbs,
     PaginatedSlimDocumentList,
     ProcessingStateEnum,
     PromptTemplateBlock,
     PromptTemplateBlockData,
     PromptTemplateBlockProperties,
     ProviderEnum,
+    SandboxInput,
+    SandboxInputRequest,
+    SandboxMetricInputParams,
+    SandboxMetricInputParamsRequest,
+    SandboxScenario,
     SearchErrorResponse,
     SearchFiltersRequest,
     SearchRequestOptionsRequest,
     SearchResponse,
     SearchResult,
     SearchResultMergingRequest,
     SearchWeightsRequest,
     SlimDocument,
     SlimDocumentStatusEnum,
     SubmitCompletionActualRequest,
     SubmitCompletionActualsErrorResponse,
+    TypeEnum,
     UploadDocumentErrorResponse,
     UploadDocumentResponse,
 )
 
 __all__ = [
     "BlockTypeEnum",
+    "ChatMessage",
     "ChatMessageRequest",
     "ChatMessageRole",
     "Document",
     "DocumentDocumentToDocumentIndex",
     "EnrichedNormalizedCompletion",
     "FinishReasonEnum",
     "GenerateErrorResponse",
@@ -77,24 +85,31 @@
     "NormalizedTokenLogProbs",
     "PaginatedSlimDocumentList",
     "ProcessingStateEnum",
     "PromptTemplateBlock",
     "PromptTemplateBlockData",
     "PromptTemplateBlockProperties",
     "ProviderEnum",
+    "SandboxInput",
+    "SandboxInputRequest",
+    "SandboxMetricInputParams",
+    "SandboxMetricInputParamsRequest",
+    "SandboxScenario",
     "SearchErrorResponse",
     "SearchFiltersRequest",
     "SearchRequestOptionsRequest",
     "SearchResponse",
     "SearchResult",
     "SearchResultMergingRequest",
     "SearchWeightsRequest",
     "SlimDocument",
     "SlimDocumentStatusEnum",
     "SubmitCompletionActualRequest",
     "SubmitCompletionActualsErrorResponse",
+    "TypeEnum",
     "UploadDocumentErrorResponse",
     "UploadDocumentResponse",
     "VellumEnvironment",
     "documents",
     "model_versions",
+    "sandboxes",
 ]
```

### Comparing `vellum_ai-0.0.6/src/vellum/client.py` & `vellum_ai-0.0.8/src/vellum/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from .core.api_error import ApiError
 from .core.jsonable_encoder import jsonable_encoder
 from .core.remove_none_from_headers import remove_none_from_headers
 from .environment import VellumEnvironment
 from .resources.documents.client import AsyncDocumentsClient, DocumentsClient
 from .resources.model_versions.client import AsyncModelVersionsClient, ModelVersionsClient
+from .resources.sandboxes.client import AsyncSandboxesClient, SandboxesClient
 from .types.generate_options_request import GenerateOptionsRequest
 from .types.generate_request import GenerateRequest
 from .types.generate_response import GenerateResponse
 from .types.search_request_options_request import SearchRequestOptionsRequest
 from .types.search_response import SearchResponse
 from .types.submit_completion_actual_request import SubmitCompletionActualRequest
 
@@ -108,14 +109,18 @@
     def documents(self) -> DocumentsClient:
         return DocumentsClient(environment=self._environment, api_key=self.api_key)
 
     @cached_property
     def model_versions(self) -> ModelVersionsClient:
         return ModelVersionsClient(environment=self._environment, api_key=self.api_key)
 
+    @cached_property
+    def sandboxes(self) -> SandboxesClient:
+        return SandboxesClient(environment=self._environment, api_key=self.api_key)
+
 
 class AsyncVellum:
     def __init__(self, *, environment: VellumEnvironment = VellumEnvironment.PRODUCTION, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
     async def generate(
@@ -203,7 +208,11 @@
     @cached_property
     def documents(self) -> AsyncDocumentsClient:
         return AsyncDocumentsClient(environment=self._environment, api_key=self.api_key)
 
     @cached_property
     def model_versions(self) -> AsyncModelVersionsClient:
         return AsyncModelVersionsClient(environment=self._environment, api_key=self.api_key)
+
+    @cached_property
+    def sandboxes(self) -> AsyncSandboxesClient:
+        return AsyncSandboxesClient(environment=self._environment, api_key=self.api_key)
```

### Comparing `vellum_ai-0.0.6/src/vellum/core/datetime_utils.py` & `vellum_ai-0.0.8/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.0.8/src/vellum/core/jsonable_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 (e.g. datetimes to strings, Pydantic models to dicts).
 
 Taken from FastAPI, and made a bit simpler
 https://github.com/tiangolo/fastapi/blob/master/fastapi/encoders.py
 """
 
 import dataclasses
+import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
 from pydantic import BaseModel
 from pydantic.json import ENCODERS_BY_TYPE
 
+from .datetime_utils import serialize_datetime
+
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
@@ -56,14 +59,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
+    if isinstance(obj, dt.date):
+        return str(obj)
+    if isinstance(obj, dt.datetime):
+        return serialize_datetime(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
```

### Comparing `vellum_ai-0.0.6/src/vellum/resources/documents/client.py` & `vellum_ai-0.0.8/src/vellum/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/resources/model_versions/client.py` & `vellum_ai-0.0.8/src/vellum/resources/model_versions/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/__init__.py` & `vellum_ai-0.0.8/src/vellum/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .block_type_enum import BlockTypeEnum
+from .chat_message import ChatMessage
 from .chat_message_request import ChatMessageRequest
 from .chat_message_role import ChatMessageRole
 from .document import Document
 from .document_document_to_document_index import DocumentDocumentToDocumentIndex
 from .enriched_normalized_completion import EnrichedNormalizedCompletion
 from .finish_reason_enum import FinishReasonEnum
 from .generate_error_response import GenerateErrorResponse
@@ -27,30 +28,37 @@
 from .normalized_token_log_probs import NormalizedTokenLogProbs
 from .paginated_slim_document_list import PaginatedSlimDocumentList
 from .processing_state_enum import ProcessingStateEnum
 from .prompt_template_block import PromptTemplateBlock
 from .prompt_template_block_data import PromptTemplateBlockData
 from .prompt_template_block_properties import PromptTemplateBlockProperties
 from .provider_enum import ProviderEnum
+from .sandbox_input import SandboxInput
+from .sandbox_input_request import SandboxInputRequest
+from .sandbox_metric_input_params import SandboxMetricInputParams
+from .sandbox_metric_input_params_request import SandboxMetricInputParamsRequest
+from .sandbox_scenario import SandboxScenario
 from .search_error_response import SearchErrorResponse
 from .search_filters_request import SearchFiltersRequest
 from .search_request_options_request import SearchRequestOptionsRequest
 from .search_response import SearchResponse
 from .search_result import SearchResult
 from .search_result_merging_request import SearchResultMergingRequest
 from .search_weights_request import SearchWeightsRequest
 from .slim_document import SlimDocument
 from .slim_document_status_enum import SlimDocumentStatusEnum
 from .submit_completion_actual_request import SubmitCompletionActualRequest
 from .submit_completion_actuals_error_response import SubmitCompletionActualsErrorResponse
+from .type_enum import TypeEnum
 from .upload_document_error_response import UploadDocumentErrorResponse
 from .upload_document_response import UploadDocumentResponse
 
 __all__ = [
     "BlockTypeEnum",
+    "ChatMessage",
     "ChatMessageRequest",
     "ChatMessageRole",
     "Document",
     "DocumentDocumentToDocumentIndex",
     "EnrichedNormalizedCompletion",
     "FinishReasonEnum",
     "GenerateErrorResponse",
@@ -73,21 +81,27 @@
     "NormalizedTokenLogProbs",
     "PaginatedSlimDocumentList",
     "ProcessingStateEnum",
     "PromptTemplateBlock",
     "PromptTemplateBlockData",
     "PromptTemplateBlockProperties",
     "ProviderEnum",
+    "SandboxInput",
+    "SandboxInputRequest",
+    "SandboxMetricInputParams",
+    "SandboxMetricInputParamsRequest",
+    "SandboxScenario",
     "SearchErrorResponse",
     "SearchFiltersRequest",
     "SearchRequestOptionsRequest",
     "SearchResponse",
     "SearchResult",
     "SearchResultMergingRequest",
     "SearchWeightsRequest",
     "SlimDocument",
     "SlimDocumentStatusEnum",
     "SubmitCompletionActualRequest",
     "SubmitCompletionActualsErrorResponse",
+    "TypeEnum",
     "UploadDocumentErrorResponse",
     "UploadDocumentResponse",
 ]
```

### Comparing `vellum_ai-0.0.6/src/vellum/types/chat_message_request.py` & `vellum_ai-0.0.8/src/vellum/types/chat_message_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/chat_message_role.py` & `vellum_ai-0.0.8/src/vellum/types/chat_message_role.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/document.py` & `vellum_ai-0.0.8/src/vellum/types/document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.0.8/src/vellum/types/document_document_to_document_index.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.0.8/src/vellum/types/enriched_normalized_completion.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/finish_reason_enum.py` & `vellum_ai-0.0.8/src/vellum/types/finish_reason_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/generate_error_response.py` & `vellum_ai-0.0.8/src/vellum/types/generate_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/generate_options_request.py` & `vellum_ai-0.0.8/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/generate_request.py` & `vellum_ai-0.0.8/src/vellum/types/generate_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/generate_response.py` & `vellum_ai-0.0.8/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/generate_result.py` & `vellum_ai-0.0.8/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/generate_result_data.py` & `vellum_ai-0.0.8/src/vellum/types/generate_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/generate_result_error.py` & `vellum_ai-0.0.8/src/vellum/types/generate_result_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/indexing_state_enum.py` & `vellum_ai-0.0.8/src/vellum/types/indexing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/model_version_build_config.py` & `vellum_ai-0.0.8/src/vellum/types/model_version_build_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/model_version_exec_config_parameters.py` & `vellum_ai-0.0.8/src/vellum/types/model_version_exec_config_parameters.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/model_version_exec_config_read.py` & `vellum_ai-0.0.8/src/vellum/types/model_version_exec_config_read.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 class ModelVersionExecConfigRead(pydantic.BaseModel):
     parameters: ModelVersionExecConfigParameters = pydantic.Field(
         description=("The generation parameters that are passed to the LLM provider at runtime.\n")
     )
     input_variables: typing.List[str] = pydantic.Field(
         description=("Names of the template variables specified in the prompt template.\n")
     )
-    prompt_template: str = pydantic.Field(
+    prompt_template: typing.Optional[str] = pydantic.Field(
         description=("The template used to generate prompts for this model version.\n")
     )
     prompt_block_data: typing.Optional[PromptTemplateBlockData]
+    prompt_syntax_version: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.6/src/vellum/types/model_version_read.py` & `vellum_ai-0.0.8/src/vellum/types/model_version_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/model_version_read_status_enum.py` & `vellum_ai-0.0.8/src/vellum/types/model_version_read_status_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/model_version_sandbox_snapshot.py` & `vellum_ai-0.0.8/src/vellum/types/search_result.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .document import Document
 
 
-class ModelVersionSandboxSnapshot(pydantic.BaseModel):
-    id: str = pydantic.Field(description=("The ID of the sandbox snapshot.\n"))
-    prompt_index: int = pydantic.Field(description=("The index of the prompt in the sandbox snapshot.\n"))
+class SearchResult(pydantic.BaseModel):
+    document: Document = pydantic.Field(
+        description=("The document that contains the chunk that matched the search query.\n")
+    )
+    text: str = pydantic.Field(description=("The text of the chunk that matched the search query.\n"))
+    keywords: typing.List[str]
+    score: float = pydantic.Field(description=("A score representing how well the chunk matches the search query.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.6/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.0.8/src/vellum/types/normalized_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.0.8/src/vellum/types/normalized_token_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.0.8/src/vellum/types/paginated_slim_document_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/processing_state_enum.py` & `vellum_ai-0.0.8/src/vellum/types/processing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/prompt_template_block.py` & `vellum_ai-0.0.8/src/vellum/types/prompt_template_block.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from ..core.datetime_utils import serialize_datetime
 from .block_type_enum import BlockTypeEnum
 from .prompt_template_block_properties import PromptTemplateBlockProperties
 
 
 class PromptTemplateBlock(pydantic.BaseModel):
+    id: str
     block_type: BlockTypeEnum
     properties: PromptTemplateBlockProperties
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.0.6/src/vellum/types/prompt_template_block_data.py` & `vellum_ai-0.0.8/src/vellum/types/prompt_template_block_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/prompt_template_block_properties.py` & `vellum_ai-0.0.8/src/vellum/types/prompt_template_block_properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 from ..core.datetime_utils import serialize_datetime
 from .chat_message_role import ChatMessageRole
 
 
 class PromptTemplateBlockProperties(pydantic.BaseModel):
     chat_role: typing.Optional[ChatMessageRole]
-    text: typing.Optional[str]
-    variable_name: typing.Optional[str]
+    template: typing.Optional[str]
     blocks: typing.Optional[typing.List[typing.Dict[str, typing.Any]]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.0.6/src/vellum/types/provider_enum.py` & `vellum_ai-0.0.8/src/vellum/types/provider_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/search_error_response.py` & `vellum_ai-0.0.8/src/vellum/types/search_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/search_filters_request.py` & `vellum_ai-0.0.8/src/vellum/types/search_filters_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.0.8/src/vellum/types/search_request_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/search_response.py` & `vellum_ai-0.0.8/src/vellum/types/search_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/search_result.py` & `vellum_ai-0.0.8/src/vellum/types/search_result_merging_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,24 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document import Document
 
 
-class SearchResult(pydantic.BaseModel):
-    document: Document = pydantic.Field(
-        description=("The document that contains the chunk that matched the search query.\n")
-    )
-    text: str = pydantic.Field(description=("The text of the chunk that matched the search query.\n"))
-    keywords: typing.List[str]
-    score: float = pydantic.Field(description=("A score representing how well the chunk matches the search query.\n"))
+class SearchResultMergingRequest(pydantic.BaseModel):
+    enabled: bool = pydantic.Field(description=("Whether to enable merging results\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.6/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.0.8/src/vellum/types/upload_document_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class SearchResultMergingRequest(pydantic.BaseModel):
-    enabled: bool = pydantic.Field(description=("Whether to enable merging results\n"))
+class UploadDocumentResponse(pydantic.BaseModel):
+    document_id: str = pydantic.Field(description=("The ID of the newly created document.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.6/src/vellum/types/search_weights_request.py` & `vellum_ai-0.0.8/src/vellum/types/search_weights_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/slim_document.py` & `vellum_ai-0.0.8/src/vellum/types/slim_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.0.8/src/vellum/types/submit_completion_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.0.8/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.0.8/src/vellum/types/upload_document_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.6/src/vellum/types/upload_document_response.py` & `vellum_ai-0.0.8/src/vellum/types/chat_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .chat_message_role import ChatMessageRole
 
 
-class UploadDocumentResponse(pydantic.BaseModel):
-    document_id: str = pydantic.Field(description=("The ID of the newly created document.\n"))
+class ChatMessage(pydantic.BaseModel):
+    text: str
+    role: ChatMessageRole
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

