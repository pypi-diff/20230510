# Comparing `tmp/gpt_index-0.6.3.tar.gz` & `tmp/gpt_index-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_index-0.6.3.tar", last modified: Wed May 10 00:04:45 2023, max compression
+gzip compressed data, was "gpt_index-0.6.4.tar", last modified: Wed May 10 00:12:10 2023, max compression
```

## Comparing `gpt_index-0.6.3.tar` & `gpt_index-0.6.4.tar`

### file list

```diff
@@ -1,459 +1,459 @@
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.056131 gpt_index-0.6.3/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1064 2023-03-07 02:41:00.000000 gpt_index-0.6.3/LICENSE
--rw-r--r--   0 jerryliu   (501) staff       (20)       72 2023-05-09 08:32:50.000000 gpt_index-0.6.3/MANIFEST.in
--rw-r--r--   0 jerryliu   (501) staff       (20)     4253 2023-05-10 00:04:45.055824 gpt_index-0.6.3/PKG-INFO
--rw-r--r--   0 jerryliu   (501) staff       (20)     4026 2023-05-09 08:32:50.000000 gpt_index-0.6.3/README.md
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.002419 gpt_index-0.6.3/gpt_index.egg-info/
--rw-r--r--   0 jerryliu   (501) staff       (20)     4253 2023-05-10 00:04:44.000000 gpt_index-0.6.3/gpt_index.egg-info/PKG-INFO
--rw-r--r--   0 jerryliu   (501) staff       (20)    14058 2023-05-10 00:04:44.000000 gpt_index-0.6.3/gpt_index.egg-info/SOURCES.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)        1 2023-05-10 00:04:44.000000 gpt_index-0.6.3/gpt_index.egg-info/dependency_links.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)      112 2023-05-10 00:04:44.000000 gpt_index-0.6.3/gpt_index.egg-info/requires.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       18 2023-05-10 00:04:44.000000 gpt_index-0.6.3/gpt_index.egg-info/top_level.txt
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.004140 gpt_index-0.6.3/llama_index/
--rw-r--r--   0 jerryliu   (501) staff       (20)        6 2023-05-09 23:59:50.000000 gpt_index-0.6.3/llama_index/VERSION
--rw-r--r--   0 jerryliu   (501) staff       (20)     4719 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      322 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/async_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.004727 gpt_index-0.6.3/llama_index/callbacks/
--rw-r--r--   0 jerryliu   (501) staff       (20)      196 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/callbacks/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3068 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/callbacks/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5526 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1073 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/callbacks/schema.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.005065 gpt_index-0.6.3/llama_index/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)      232 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      171 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/composability/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3777 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      313 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/constants.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.005870 gpt_index-0.6.3/llama_index/data_structs/
--rw-r--r--   0 jerryliu   (501) staff       (20)      400 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/data_structs/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9458 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/data_structs/data_structs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2292 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/data_structs/document_summary.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6221 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/data_structs/node.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      904 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/data_structs/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3638 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/data_structs/struct_type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1025 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/data_structs/table.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.006585 gpt_index-0.6.3/llama_index/embeddings/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/embeddings/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7721 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/embeddings/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1164 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/embeddings/google.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1109 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/embeddings/langchain.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9925 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/embeddings/openai.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      559 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/embeddings/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.007046 gpt_index-0.6.3/llama_index/evaluation/
--rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/evaluation/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    12080 2023-05-09 23:55:00.000000 gpt_index-0.6.3/llama_index/evaluation/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5341 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      544 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/img_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.008538 gpt_index-0.6.3/llama_index/indices/
--rw-r--r--   0 jerryliu   (501) staff       (20)      542 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9742 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      856 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.008780 gpt_index-0.6.3/llama_index/indices/common/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.009244 gpt_index-0.6.3/llama_index/indices/common/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8471 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      776 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2676 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.009482 gpt_index-0.6.3/llama_index/indices/common_tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7971 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.009738 gpt_index-0.6.3/llama_index/indices/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)      180 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3950 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.010109 gpt_index-0.6.3/llama_index/indices/document_summary/
--rw-r--r--   0 jerryliu   (501) staff       (20)      382 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6018 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/document_summary/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8686 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.010592 gpt_index-0.6.3/llama_index/indices/empty/
--rw-r--r--   0 jerryliu   (501) staff       (20)      198 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/empty/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2145 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/empty/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1173 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.011430 gpt_index-0.6.3/llama_index/indices/keyword_table/
--rw-r--r--   0 jerryliu   (501) staff       (20)      656 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8539 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      650 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6484 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      844 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2264 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.011780 gpt_index-0.6.3/llama_index/indices/knowledge_graph/
--rw-r--r--   0 jerryliu   (501) staff       (20)      254 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9043 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10428 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.012147 gpt_index-0.6.3/llama_index/indices/list/
--rw-r--r--   0 jerryliu   (501) staff       (20)      295 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/list/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3299 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/list/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4195 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/list/retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3608 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/loading.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.012933 gpt_index-0.6.3/llama_index/indices/postprocessor/
--rw-r--r--   0 jerryliu   (501) staff       (20)      888 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1749 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11715 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8830 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5026 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      445 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8489 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.013734 gpt_index-0.6.3/llama_index/indices/query/
--rw-r--r--   0 jerryliu   (501) staff       (20)      137 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/query/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1934 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/query/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3386 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.014214 gpt_index-0.6.3/llama_index/indices/query/query_transform/
--rw-r--r--   0 jerryliu   (501) staff       (20)      281 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8904 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5920 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8058 2023-05-09 23:55:00.000000 gpt_index-0.6.3/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1248 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/query/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1292 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/registry.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.014953 gpt_index-0.6.3/llama_index/indices/response/
--rw-r--r--   0 jerryliu   (501) staff       (20)      419 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/response/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    24768 2023-05-09 23:54:57.000000 gpt_index-0.6.3/llama_index/indices/response/response_builder.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/response/type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3643 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/service_context.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.015994 gpt_index-0.6.3/llama_index/indices/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      622 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2109 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/struct_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5765 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2208 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5409 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6142 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7158 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.016982 gpt_index-0.6.3/llama_index/indices/tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)      616 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1606 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5853 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/tree/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7188 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/tree/inserter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4660 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15309 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1399 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2002 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.017513 gpt_index-0.6.3/llama_index/indices/vector_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      260 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8300 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/vector_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4349 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.018197 gpt_index-0.6.3/llama_index/langchain_helpers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       39 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.018803 gpt_index-0.6.3/llama_index/langchain_helpers/agents/
--rw-r--r--   0 jerryliu   (501) staff       (20)      514 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2994 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      837 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2211 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      252 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7675 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3287 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    18172 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.019638 gpt_index-0.6.3/llama_index/llm_predictor/
--rw-r--r--   0 jerryliu   (501) staff       (20)      359 2023-05-09 23:55:00.000000 gpt_index-0.6.3/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10841 2023-05-09 23:54:57.000000 gpt_index-0.6.3/llama_index/llm_predictor/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4282 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8095 2023-05-09 23:55:00.000000 gpt_index-0.6.3/llama_index/llm_predictor/huggingface.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2274 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.020040 gpt_index-0.6.3/llama_index/logger/
--rw-r--r--   0 jerryliu   (501) staff       (20)       95 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/logger/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      995 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/logger/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.020551 gpt_index-0.6.3/llama_index/node_parser/
--rw-r--r--   0 jerryliu   (501) staff       (20)      184 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/node_parser/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      527 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/node_parser/interface.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3582 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/node_parser/node_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1818 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/node_parser/simple.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.020801 gpt_index-0.6.3/llama_index/optimization/
--rw-r--r--   0 jerryliu   (501) staff       (20)      144 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/optimization/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4301 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.021390 gpt_index-0.6.3/llama_index/output_parsers/
--rw-r--r--   0 jerryliu   (501) staff       (20)      230 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/output_parsers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      611 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/output_parsers/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2742 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1828 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/output_parsers/langchain.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1345 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/output_parsers/selection.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.021608 gpt_index-0.6.3/llama_index/playground/
--rw-r--r--   0 jerryliu   (501) staff       (20)      202 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/playground/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6471 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/playground/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.022720 gpt_index-0.6.3/llama_index/prompts/
--rw-r--r--   0 jerryliu   (501) staff       (20)       87 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/prompts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6633 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/prompts/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1969 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1134 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10843 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/prompts/default_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1120 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/prompts/prompt_type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7685 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/prompts/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/py.typed
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.023645 gpt_index-0.6.3/llama_index/query_engine/
--rw-r--r--   0 jerryliu   (501) staff       (20)      635 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/query_engine/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3569 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5811 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6997 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4587 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2964 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.027260 gpt_index-0.6.3/llama_index/readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)     3043 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      659 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.027490 gpt_index-0.6.3/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 jerryliu   (501) staff       (20)      145 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2111 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3755 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/chroma.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3308 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/database.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3456 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/deeplake.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4981 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/discord_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7769 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/download.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2392 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/elasticsearch.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2510 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/faiss.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.029344 gpt_index-0.6.3/llama_index/readers/file/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8535 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1342 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/base_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1629 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1318 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3180 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4106 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/image_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3222 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1027 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3616 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3162 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3945 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3357 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1770 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.029910 gpt_index-0.6.3/llama_index/readers/github_readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11730 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15889 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5473 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.030330 gpt_index-0.6.3/llama_index/readers/google_readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5659 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4989 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3708 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/json.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.030675 gpt_index-0.6.3/llama_index/readers/make_com/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1693 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1261 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/mbox.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2307 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/metal.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4588 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2608 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/mongo.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5541 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5679 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/notion.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1601 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/obsidian.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2766 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6920 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/qdrant.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.030974 gpt_index-0.6.3/llama_index/readers/schema/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/schema/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1214 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/schema/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7892 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/slack.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.031278 gpt_index-0.6.3/llama_index/readers/steamship/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3498 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1042 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/string_iterable.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1918 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/twitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.032026 gpt_index-0.6.3/llama_index/readers/weaviate/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7760 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/weaviate/client.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3986 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1867 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7987 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/web.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      981 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/wikipedia.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1255 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.032692 gpt_index-0.6.3/llama_index/response/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/response/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2036 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/response/notebook_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1490 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/response/pprint_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3068 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/response/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/response/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.032965 gpt_index-0.6.3/llama_index/retrievers/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1258 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/retrievers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1063 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2792 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/schema.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.033622 gpt_index-0.6.3/llama_index/selectors/
--rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/selectors/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7082 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2438 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/selectors/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2235 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/selectors/types.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.033899 gpt_index-0.6.3/llama_index/storage/
--rw-r--r--   0 jerryliu   (501) staff       (20)      124 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.034853 gpt_index-0.6.3/llama_index/storage/docstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)      536 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4825 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1408 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      762 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/docstore/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2658 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2529 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/docstore/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      915 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.035583 gpt_index-0.6.3/llama_index/storage/index_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      301 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2209 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1341 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1811 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      873 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/index_store/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      635 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.036098 gpt_index-0.6.3/llama_index/storage/kvstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)      187 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4061 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2580 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      973 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/kvstore/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4460 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/storage/storage_context.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.036724 gpt_index-0.6.3/llama_index/token_counter/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/token_counter/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4664 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      722 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2874 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/token_counter/token_counter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/token_counter/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.037087 gpt_index-0.6.3/llama_index/tools/
--rw-r--r--   0 jerryliu   (501) staff       (20)      162 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/tools/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1557 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/tools/query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      366 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/tools/types.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.037551 gpt_index-0.6.3/llama_index/tts/
--rw-r--r--   0 jerryliu   (501) staff       (20)      154 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/tts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2589 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/tts/bark.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      631 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/tts/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1282 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/tts/elevenlabs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)       81 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5847 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.039784 gpt_index-0.6.3/llama_index/vector_stores/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1308 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5181 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3942 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/chroma.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8629 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4451 2023-05-09 23:55:00.000000 gpt_index-0.6.3/llama_index/vector_stores/faiss.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3903 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3523 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/metal.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15763 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8360 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7184 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11372 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6504 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2111 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5370 2023-05-09 23:55:00.000000 gpt_index-0.6.3/llama_index/vector_stores/simple.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2285 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3379 2023-05-09 08:32:50.000000 gpt_index-0.6.3/llama_index/vector_stores/weaviate.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      276 2023-04-01 01:19:55.000000 gpt_index-0.6.3/pyproject.toml
--rw-r--r--   0 jerryliu   (501) staff       (20)       38 2023-05-10 00:04:45.056178 gpt_index-0.6.3/setup.cfg
--rw-r--r--   0 jerryliu   (501) staff       (20)     1192 2023-05-09 08:32:50.000000 gpt_index-0.6.3/setup.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.040243 gpt_index-0.6.3/tests/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.040625 gpt_index-0.6.3/tests/callbacks/
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/callbacks/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2975 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1966 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/conftest.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.041015 gpt_index-0.6.3/tests/embeddings/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/embeddings/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3002 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/embeddings/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.042068 gpt_index-0.6.3/tests/indices/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/indices/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.042292 gpt_index-0.6.3/tests/indices/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      993 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/composability/test_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1023 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/conftest.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.042700 gpt_index-0.6.3/tests/indices/document_summary/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/document_summary/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1340 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/document_summary/test_index.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      367 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.043028 gpt_index-0.6.3/tests/indices/empty/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/indices/empty/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      548 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/empty/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.043645 gpt_index-0.6.3/tests/indices/keyword_table/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6259 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1185 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1010 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.044230 gpt_index-0.6.3/tests/indices/knowledge_graph/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      381 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6415 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3900 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.044588 gpt_index-0.6.3/tests/indices/list/
--rw-r--r--   0 jerryliu   (501) staff       (20)       34 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/list/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6487 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/list/test_index.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1480 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.044972 gpt_index-0.6.3/tests/indices/postprocessor/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-03 06:27:55.000000 gpt_index-0.6.3/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    13872 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/postprocessor/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.045716 gpt_index-0.6.3/tests/indices/query/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/indices/query/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1832 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/query/conftest.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.046227 gpt_index-0.6.3/tests/indices/query/query_transform/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      267 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      787 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6649 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/query/test_compose.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    13016 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2196 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.047093 gpt_index-0.6.3/tests/indices/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/indices/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1195 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/struct_store/conftest.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11931 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/struct_store/test_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1234 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/struct_store/test_pandas.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3901 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5540 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/test_loading.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2007 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/test_loading_graph.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1940 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/test_node_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7178 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/test_prompt_helper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      463 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/test_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.047960 gpt_index-0.6.3/tests/indices/tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/indices/tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      992 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/tree/conftest.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4444 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7789 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/tree/test_index.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1332 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.049900 gpt_index-0.6.3/tests/indices/vector_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/indices/vector_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      767 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/conftest.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1153 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1056 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2960 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1630 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/test_lancedb.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1984 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/test_milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4134 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1726 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5027 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6554 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1546 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/test_weaviate.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1773 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.050206 gpt_index-0.6.3/tests/langchain_helpers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/langchain_helpers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3426 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.050615 gpt_index-0.6.3/tests/llm_predictor/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/llm_predictor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3174 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.050962 gpt_index-0.6.3/tests/logger/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/logger/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1244 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/logger/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.052033 gpt_index-0.6.3/tests/mock_utils/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/mock_utils/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8147 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/mock_utils/mock_predict.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2253 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1141 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      739 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.052312 gpt_index-0.6.3/tests/optimization/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/optimization/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2466 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/optimization/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.052731 gpt_index-0.6.3/tests/output_parsers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/output_parsers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1507 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/output_parsers/test_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      972 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.053119 gpt_index-0.6.3/tests/playground/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-04-01 01:19:55.000000 gpt_index-0.6.3/tests/playground/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3494 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/playground/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.053404 gpt_index-0.6.3/tests/prompts/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/prompts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4655 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/prompts/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.054049 gpt_index-0.6.3/tests/readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11334 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/readers/test_file.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1773 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/readers/test_json.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1732 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/readers/test_mongo.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      339 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.054280 gpt_index-0.6.3/tests/selectors/
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/selectors/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1261 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.054616 gpt_index-0.6.3/tests/storage/
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/storage/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      548 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/storage/conftest.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.054967 gpt_index-0.6.3/tests/storage/docstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/storage/docstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2115 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2137 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      959 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/storage/test_storage_context.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3016 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/test_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.055198 gpt_index-0.6.3/tests/token_predictor/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-03-07 02:41:00.000000 gpt_index-0.6.3/tests/token_predictor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1940 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/token_predictor/test_base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-10 00:04:45.055539 gpt_index-0.6.3/tests/vector_stores/
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/vector_stores/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4975 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1002 2023-05-09 08:32:50.000000 gpt_index-0.6.3/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.064128 gpt_index-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 00:11:50.000000 gpt_index-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 00:11:50.000000 gpt_index-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-10 00:12:10.060128 gpt_index-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-10 00:11:50.000000 gpt_index-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.016127 gpt_index-0.6.4/gpt_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-10 00:12:09.000000 gpt_index-0.6.4/gpt_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-05-10 00:12:10.000000 gpt_index-0.6.4/gpt_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:12:09.000000 gpt_index-0.6.4/gpt_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 00:12:09.000000 gpt_index-0.6.4/gpt_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 00:12:09.000000 gpt_index-0.6.4/gpt_index.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.020127 gpt_index-0.6.4/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.020127 gpt_index-0.6.4/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/callbacks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.020127 gpt_index-0.6.4/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.020127 gpt_index-0.6.4/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/data_structs/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.020127 gpt_index-0.6.4/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.024128 gpt_index-0.6.4/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.028128 gpt_index-0.6.4/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.028128 gpt_index-0.6.4/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.028128 gpt_index-0.6.4/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.028128 gpt_index-0.6.4/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.028128 gpt_index-0.6.4/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.028128 gpt_index-0.6.4/llama_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24768 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.028128 gpt_index-0.6.4/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.028128 gpt_index-0.6.4/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/vector_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/llm_predictor/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/output_parsers/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.032128 gpt_index-0.6.4/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.036128 gpt_index-0.6.4/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.036128 gpt_index-0.6.4/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.036128 gpt_index-0.6.4/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.040128 gpt_index-0.6.4/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.044128 gpt_index-0.6.4/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.044128 gpt_index-0.6.4/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.044128 gpt_index-0.6.4/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.044128 gpt_index-0.6.4/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.044128 gpt_index-0.6.4/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.044128 gpt_index-0.6.4/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.048128 gpt_index-0.6.4/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/tools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.048128 gpt_index-0.6.4/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.048128 gpt_index-0.6.4/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-10 00:11:50.000000 gpt_index-0.6.4/llama_index/vector_stores/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-10 00:11:50.000000 gpt_index-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 00:12:10.064128 gpt_index-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-10 00:11:50.000000 gpt_index-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.048128 gpt_index-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.048128 gpt_index-0.6.4/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.052128 gpt_index-0.6.4/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/postprocessor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.056128 gpt_index-0.6.4/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.056128 gpt_index-0.6.4/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.056128 gpt_index-0.6.4/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.056128 gpt_index-0.6.4/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.056128 gpt_index-0.6.4/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/test_lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/test_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/test_weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.056128 gpt_index-0.6.4/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.056128 gpt_index-0.6.4/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:12:10.060128 gpt_index-0.6.4/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-10 00:11:50.000000 gpt_index-0.6.4/tests/vector_stores/test_weaviate.py
```

### Comparing `gpt_index-0.6.3/LICENSE` & `gpt_index-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/PKG-INFO` & `gpt_index-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_index
-Version: 0.6.3
+Version: 0.6.4
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.3/README.md` & `gpt_index-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/gpt_index.egg-info/PKG-INFO` & `gpt_index-0.6.4/gpt_index.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-index
-Version: 0.6.3
+Version: 0.6.4
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.3/gpt_index.egg-info/SOURCES.txt` & `gpt_index-0.6.4/gpt_index.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/__init__.py` & `gpt_index-0.6.4/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/callbacks/base.py` & `gpt_index-0.6.4/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/callbacks/llama_debug.py` & `gpt_index-0.6.4/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/callbacks/schema.py` & `gpt_index-0.6.4/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/composability/joint_qa_summary.py` & `gpt_index-0.6.4/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/data_structs/data_structs.py` & `gpt_index-0.6.4/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/data_structs/document_summary.py` & `gpt_index-0.6.4/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/data_structs/node.py` & `gpt_index-0.6.4/llama_index/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/data_structs/registry.py` & `gpt_index-0.6.4/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/data_structs/struct_type.py` & `gpt_index-0.6.4/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/data_structs/table.py` & `gpt_index-0.6.4/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/embeddings/base.py` & `gpt_index-0.6.4/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/embeddings/google.py` & `gpt_index-0.6.4/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/embeddings/langchain.py` & `gpt_index-0.6.4/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/embeddings/openai.py` & `gpt_index-0.6.4/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/embeddings/utils.py` & `gpt_index-0.6.4/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/evaluation/base.py` & `gpt_index-0.6.4/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/evaluation/dataset_generation.py` & `gpt_index-0.6.4/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/img_utils.py` & `gpt_index-0.6.4/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/__init__.py` & `gpt_index-0.6.4/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/base.py` & `gpt_index-0.6.4/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/base_retriever.py` & `gpt_index-0.6.4/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/common/struct_store/base.py` & `gpt_index-0.6.4/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/common/struct_store/schema.py` & `gpt_index-0.6.4/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/common/struct_store/sql.py` & `gpt_index-0.6.4/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/common_tree/base.py` & `gpt_index-0.6.4/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/composability/graph.py` & `gpt_index-0.6.4/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/document_summary/base.py` & `gpt_index-0.6.4/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/document_summary/retrievers.py` & `gpt_index-0.6.4/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/empty/base.py` & `gpt_index-0.6.4/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/empty/retrievers.py` & `gpt_index-0.6.4/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/keyword_table/__init__.py` & `gpt_index-0.6.4/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/keyword_table/base.py` & `gpt_index-0.6.4/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/keyword_table/rake_base.py` & `gpt_index-0.6.4/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/keyword_table/retrievers.py` & `gpt_index-0.6.4/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/keyword_table/simple_base.py` & `gpt_index-0.6.4/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/keyword_table/utils.py` & `gpt_index-0.6.4/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/knowledge_graph/base.py` & `gpt_index-0.6.4/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/knowledge_graph/retrievers.py` & `gpt_index-0.6.4/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/list/base.py` & `gpt_index-0.6.4/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/list/retrievers.py` & `gpt_index-0.6.4/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/loading.py` & `gpt_index-0.6.4/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/postprocessor/__init__.py` & `gpt_index-0.6.4/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/postprocessor/cohere_rerank.py` & `gpt_index-0.6.4/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/postprocessor/node.py` & `gpt_index-0.6.4/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/postprocessor/node_recency.py` & `gpt_index-0.6.4/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/postprocessor/pii.py` & `gpt_index-0.6.4/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/prompt_helper.py` & `gpt_index-0.6.4/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/query/base.py` & `gpt_index-0.6.4/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/query/embedding_utils.py` & `gpt_index-0.6.4/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/query/query_transform/base.py` & `gpt_index-0.6.4/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/query/query_transform/prompts.py` & `gpt_index-0.6.4/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/query/response_synthesis.py` & `gpt_index-0.6.4/llama_index/indices/query/response_synthesis.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/query/schema.py` & `gpt_index-0.6.4/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/registry.py` & `gpt_index-0.6.4/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/response/response_builder.py` & `gpt_index-0.6.4/llama_index/indices/response/response_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/service_context.py` & `gpt_index-0.6.4/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/struct_store/__init__.py` & `gpt_index-0.6.4/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/struct_store/base.py` & `gpt_index-0.6.4/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/struct_store/container_builder.py` & `gpt_index-0.6.4/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/struct_store/pandas.py` & `gpt_index-0.6.4/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/struct_store/pandas_query.py` & `gpt_index-0.6.4/llama_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/struct_store/sql.py` & `gpt_index-0.6.4/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/struct_store/sql_query.py` & `gpt_index-0.6.4/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/tree/__init__.py` & `gpt_index-0.6.4/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/tree/all_leaf_retriever.py` & `gpt_index-0.6.4/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/tree/base.py` & `gpt_index-0.6.4/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/tree/inserter.py` & `gpt_index-0.6.4/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `gpt_index-0.6.4/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/tree/select_leaf_retriever.py` & `gpt_index-0.6.4/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/tree/tree_root_retriever.py` & `gpt_index-0.6.4/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/utils.py` & `gpt_index-0.6.4/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/vector_store/base.py` & `gpt_index-0.6.4/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/indices/vector_store/retrievers.py` & `gpt_index-0.6.4/llama_index/indices/vector_store/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/langchain_helpers/agents/__init__.py` & `gpt_index-0.6.4/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/langchain_helpers/agents/agents.py` & `gpt_index-0.6.4/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/langchain_helpers/agents/toolkits.py` & `gpt_index-0.6.4/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/langchain_helpers/agents/tools.py` & `gpt_index-0.6.4/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/langchain_helpers/memory_wrapper.py` & `gpt_index-0.6.4/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/langchain_helpers/sql_wrapper.py` & `gpt_index-0.6.4/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/langchain_helpers/text_splitter.py` & `gpt_index-0.6.4/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/llm_predictor/base.py` & `gpt_index-0.6.4/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/llm_predictor/chatgpt.py` & `gpt_index-0.6.4/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/llm_predictor/huggingface.py` & `gpt_index-0.6.4/llama_index/llm_predictor/huggingface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/llm_predictor/structured.py` & `gpt_index-0.6.4/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/logger/base.py` & `gpt_index-0.6.4/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/node_parser/interface.py` & `gpt_index-0.6.4/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/node_parser/node_utils.py` & `gpt_index-0.6.4/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/node_parser/simple.py` & `gpt_index-0.6.4/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/optimization/optimizer.py` & `gpt_index-0.6.4/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/output_parsers/base.py` & `gpt_index-0.6.4/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/output_parsers/guardrails.py` & `gpt_index-0.6.4/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/output_parsers/langchain.py` & `gpt_index-0.6.4/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/output_parsers/selection.py` & `gpt_index-0.6.4/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/playground/base.py` & `gpt_index-0.6.4/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/prompts/base.py` & `gpt_index-0.6.4/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/prompts/chat_prompts.py` & `gpt_index-0.6.4/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/prompts/default_prompt_selectors.py` & `gpt_index-0.6.4/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/prompts/default_prompts.py` & `gpt_index-0.6.4/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/prompts/prompt_type.py` & `gpt_index-0.6.4/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/prompts/prompts.py` & `gpt_index-0.6.4/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/query_engine/__init__.py` & `gpt_index-0.6.4/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/query_engine/graph_query_engine.py` & `gpt_index-0.6.4/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/query_engine/multistep_query_engine.py` & `gpt_index-0.6.4/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/query_engine/retriever_query_engine.py` & `gpt_index-0.6.4/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/query_engine/router_query_engine.py` & `gpt_index-0.6.4/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/query_engine/transform_query_engine.py` & `gpt_index-0.6.4/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/__init__.py` & `gpt_index-0.6.4/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/base.py` & `gpt_index-0.6.4/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/chatgpt_plugin/base.py` & `gpt_index-0.6.4/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/chroma.py` & `gpt_index-0.6.4/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/database.py` & `gpt_index-0.6.4/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/deeplake.py` & `gpt_index-0.6.4/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/discord_reader.py` & `gpt_index-0.6.4/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/download.py` & `gpt_index-0.6.4/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/elasticsearch.py` & `gpt_index-0.6.4/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/faiss.py` & `gpt_index-0.6.4/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/base.py` & `gpt_index-0.6.4/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/base_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/docs_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/epub_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/image_caption_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/image_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/image_vision_llm_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/ipynb_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/markdown_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/mbox_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/slides_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/tabular_parser.py` & `gpt_index-0.6.4/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/file/video_audio.py` & `gpt_index-0.6.4/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/github_readers/github_api_client.py` & `gpt_index-0.6.4/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/github_readers/github_repository_reader.py` & `gpt_index-0.6.4/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/github_readers/utils.py` & `gpt_index-0.6.4/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/google_readers/gdocs.py` & `gpt_index-0.6.4/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/google_readers/gsheets.py` & `gpt_index-0.6.4/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/json.py` & `gpt_index-0.6.4/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/make_com/wrapper.py` & `gpt_index-0.6.4/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/mbox.py` & `gpt_index-0.6.4/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/metal.py` & `gpt_index-0.6.4/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/milvus.py` & `gpt_index-0.6.4/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/mongo.py` & `gpt_index-0.6.4/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/myscale.py` & `gpt_index-0.6.4/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/notion.py` & `gpt_index-0.6.4/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/obsidian.py` & `gpt_index-0.6.4/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/pinecone.py` & `gpt_index-0.6.4/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/qdrant.py` & `gpt_index-0.6.4/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/schema/base.py` & `gpt_index-0.6.4/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/slack.py` & `gpt_index-0.6.4/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/steamship/file_reader.py` & `gpt_index-0.6.4/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/string_iterable.py` & `gpt_index-0.6.4/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/twitter.py` & `gpt_index-0.6.4/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/weaviate/client.py` & `gpt_index-0.6.4/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/weaviate/reader.py` & `gpt_index-0.6.4/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/weaviate/utils.py` & `gpt_index-0.6.4/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/web.py` & `gpt_index-0.6.4/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/wikipedia.py` & `gpt_index-0.6.4/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/readers/youtube_transcript.py` & `gpt_index-0.6.4/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/response/notebook_utils.py` & `gpt_index-0.6.4/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/response/pprint_utils.py` & `gpt_index-0.6.4/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/response/schema.py` & `gpt_index-0.6.4/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/retrievers/__init__.py` & `gpt_index-0.6.4/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/retrievers/transform_retriever.py` & `gpt_index-0.6.4/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/schema.py` & `gpt_index-0.6.4/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/selectors/llm_selectors.py` & `gpt_index-0.6.4/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/selectors/prompts.py` & `gpt_index-0.6.4/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/selectors/types.py` & `gpt_index-0.6.4/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/docstore/__init__.py` & `gpt_index-0.6.4/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/docstore/keyval_docstore.py` & `gpt_index-0.6.4/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/docstore/mongo_docstore.py` & `gpt_index-0.6.4/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/docstore/registry.py` & `gpt_index-0.6.4/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/docstore/simple_docstore.py` & `gpt_index-0.6.4/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/docstore/types.py` & `gpt_index-0.6.4/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/docstore/utils.py` & `gpt_index-0.6.4/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/index_store/keyval_index_store.py` & `gpt_index-0.6.4/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/index_store/mongo_index_store.py` & `gpt_index-0.6.4/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/index_store/simple_index_store.py` & `gpt_index-0.6.4/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/index_store/types.py` & `gpt_index-0.6.4/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/index_store/utils.py` & `gpt_index-0.6.4/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/kvstore/mongodb_kvstore.py` & `gpt_index-0.6.4/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/kvstore/simple_kvstore.py` & `gpt_index-0.6.4/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/kvstore/types.py` & `gpt_index-0.6.4/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/storage/storage_context.py` & `gpt_index-0.6.4/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/token_counter/mock_chain_wrapper.py` & `gpt_index-0.6.4/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/token_counter/mock_embed_model.py` & `gpt_index-0.6.4/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/token_counter/token_counter.py` & `gpt_index-0.6.4/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/token_counter/utils.py` & `gpt_index-0.6.4/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/tools/query_engine.py` & `gpt_index-0.6.4/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/tts/bark.py` & `gpt_index-0.6.4/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/tts/base.py` & `gpt_index-0.6.4/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/tts/elevenlabs.py` & `gpt_index-0.6.4/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/utils.py` & `gpt_index-0.6.4/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/__init__.py` & `gpt_index-0.6.4/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/chatgpt_plugin.py` & `gpt_index-0.6.4/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/chroma.py` & `gpt_index-0.6.4/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/deeplake.py` & `gpt_index-0.6.4/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/faiss.py` & `gpt_index-0.6.4/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/lancedb.py` & `gpt_index-0.6.4/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/metal.py` & `gpt_index-0.6.4/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/milvus.py` & `gpt_index-0.6.4/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/myscale.py` & `gpt_index-0.6.4/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/opensearch.py` & `gpt_index-0.6.4/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/pinecone.py` & `gpt_index-0.6.4/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/qdrant.py` & `gpt_index-0.6.4/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/registry.py` & `gpt_index-0.6.4/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/simple.py` & `gpt_index-0.6.4/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/types.py` & `gpt_index-0.6.4/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/llama_index/vector_stores/weaviate.py` & `gpt_index-0.6.4/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/setup.py` & `gpt_index-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/callbacks/test_llama_debug.py` & `gpt_index-0.6.4/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/conftest.py` & `gpt_index-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/embeddings/test_base.py` & `gpt_index-0.6.4/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/composability/test_utils.py` & `gpt_index-0.6.4/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/conftest.py` & `gpt_index-0.6.4/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/document_summary/test_index.py` & `gpt_index-0.6.4/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/empty/test_base.py` & `gpt_index-0.6.4/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/keyword_table/test_base.py` & `gpt_index-0.6.4/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/keyword_table/test_retrievers.py` & `gpt_index-0.6.4/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/keyword_table/test_utils.py` & `gpt_index-0.6.4/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/knowledge_graph/test_base.py` & `gpt_index-0.6.4/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/knowledge_graph/test_retrievers.py` & `gpt_index-0.6.4/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/list/test_index.py` & `gpt_index-0.6.4/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/list/test_retrievers.py` & `gpt_index-0.6.4/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/postprocessor/test_base.py` & `gpt_index-0.6.4/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/query/conftest.py` & `gpt_index-0.6.4/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/query/query_transform/test_base.py` & `gpt_index-0.6.4/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/query/test_compose.py` & `gpt_index-0.6.4/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/query/test_compose_vector.py` & `gpt_index-0.6.4/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/query/test_query_bundle.py` & `gpt_index-0.6.4/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/struct_store/conftest.py` & `gpt_index-0.6.4/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/struct_store/test_base.py` & `gpt_index-0.6.4/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/struct_store/test_pandas.py` & `gpt_index-0.6.4/tests/indices/struct_store/test_pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/struct_store/test_sql_query.py` & `gpt_index-0.6.4/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/test_loading.py` & `gpt_index-0.6.4/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/test_loading_graph.py` & `gpt_index-0.6.4/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/test_node_utils.py` & `gpt_index-0.6.4/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/test_prompt_helper.py` & `gpt_index-0.6.4/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/tree/conftest.py` & `gpt_index-0.6.4/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/tree/test_embedding_retriever.py` & `gpt_index-0.6.4/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/tree/test_index.py` & `gpt_index-0.6.4/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/tree/test_retrievers.py` & `gpt_index-0.6.4/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/conftest.py` & `gpt_index-0.6.4/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/mock_faiss.py` & `gpt_index-0.6.4/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/mock_services.py` & `gpt_index-0.6.4/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/test_faiss.py` & `gpt_index-0.6.4/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/test_lancedb.py` & `gpt_index-0.6.4/tests/indices/vector_store/test_lancedb.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/test_milvus.py` & `gpt_index-0.6.4/tests/indices/vector_store/test_milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/test_myscale.py` & `gpt_index-0.6.4/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/test_pinecone.py` & `gpt_index-0.6.4/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/test_retrievers.py` & `gpt_index-0.6.4/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/test_simple.py` & `gpt_index-0.6.4/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/test_weaviate.py` & `gpt_index-0.6.4/tests/indices/vector_store/test_weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/indices/vector_store/utils.py` & `gpt_index-0.6.4/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/langchain_helpers/test_text_splitter.py` & `gpt_index-0.6.4/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/llm_predictor/test_base.py` & `gpt_index-0.6.4/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/logger/test_base.py` & `gpt_index-0.6.4/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/mock_utils/mock_predict.py` & `gpt_index-0.6.4/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/mock_utils/mock_prompts.py` & `gpt_index-0.6.4/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/mock_utils/mock_text_splitter.py` & `gpt_index-0.6.4/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/mock_utils/mock_utils.py` & `gpt_index-0.6.4/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/optimization/test_base.py` & `gpt_index-0.6.4/tests/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/output_parsers/test_base.py` & `gpt_index-0.6.4/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/output_parsers/test_selection.py` & `gpt_index-0.6.4/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/playground/test_base.py` & `gpt_index-0.6.4/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/prompts/test_base.py` & `gpt_index-0.6.4/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/readers/test_file.py` & `gpt_index-0.6.4/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/readers/test_json.py` & `gpt_index-0.6.4/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/readers/test_mongo.py` & `gpt_index-0.6.4/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/selectors/test_llm_selectors.py` & `gpt_index-0.6.4/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/storage/conftest.py` & `gpt_index-0.6.4/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/storage/docstore/test_mongo_docstore.py` & `gpt_index-0.6.4/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/storage/docstore/test_simple_docstore.py` & `gpt_index-0.6.4/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/storage/test_storage_context.py` & `gpt_index-0.6.4/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/test_utils.py` & `gpt_index-0.6.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/token_predictor/test_base.py` & `gpt_index-0.6.4/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/vector_stores/test_qdrant.py` & `gpt_index-0.6.4/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.3/tests/vector_stores/test_weaviate.py` & `gpt_index-0.6.4/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

