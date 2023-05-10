# Comparing `tmp/sarus_data_spec_public-3.2.1.dev0.tar.gz` & `tmp/sarus_data_spec_public-3.2.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.2.1.dev0.tar", last modified: Tue May  2 11:55:46 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.2.1.dev2.tar", last modified: Tue May  9 08:13:15 2023, max compression
```

## Comparing `sarus_data_spec_public-3.2.1.dev0.tar` & `sarus_data_spec_public-3.2.1.dev2.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.590237 sarus_data_spec_public-3.2.1.dev0/
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-02 11:55:46.590237 sarus_data_spec_public-3.2.1.dev0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.538236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.540236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5582 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9892 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.541236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3622 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.542236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18711 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.543236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.546236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)    13941 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8284 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.547236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    28802 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.548236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8138 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.549236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2172 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.550236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.550236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.551236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.554236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11465 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)     7945 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.555236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    71070 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    26225 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.560236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38861 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     6429 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6041 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    18290 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6107 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.564236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)    10320 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.566236 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3127 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.587237 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     6521 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   107770 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38135 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    73431 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28800 2023-05-02 11:55:36.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43542 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17816 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.588237 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31051 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   136116 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    35527 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:55:46.590237 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7837 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-02 11:55:46.000000 sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5833 2023-05-02 11:55:46.592237 sarus_data_spec_public-3.2.1.dev0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2023-05-02 11:55:24.000000 sarus_data_spec_public-3.2.1.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.868536 sarus_data_spec_public-3.2.1.dev2/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-09 08:13:15.868536 sarus_data_spec_public-3.2.1.dev2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.811532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      830 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.813532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5582 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.814532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3622 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.815532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18711 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.817532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.819532 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11044 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)    19230 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.821533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    28802 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.821533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8823 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.823533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.823533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.824533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.825533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.829533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11465 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)     7943 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.830533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    73352 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    26225 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.835533 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38861 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6920 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    18360 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6107 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.840534 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-09 08:12:52.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/select_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)    10320 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.841534 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.864535 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)    24833 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14459 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    91981 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32903 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)    18816 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)   107770 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38135 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)    74241 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    29134 2023-05-09 08:13:05.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43542 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    16850 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.865536 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31051 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   136116 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    35669 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 08:13:15.868536 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7837 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-09 08:13:15.000000 sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2023-05-09 08:13:15.869536 sarus_data_spec_public-3.2.1.dev2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2023-05-09 08:12:53.000000 sarus_data_spec_public-3.2.1.dev2/setup.py
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.2.1.dev0'
+VERSION: Final[str] = '3.2.1.dev2'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/conversion.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/arrow/type.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import sarus_data_spec.typing as st
 
 INTBASE_TO_ARROW = {
     st.IntegerBase.INT64: pa.int64(),
     st.IntegerBase.INT32: pa.int32(),
     st.IntegerBase.INT16: pa.int16(),
     st.IntegerBase.INT8: pa.int8(),
+    st.IntegerBase.UINT64: pa.uint64(),
+    st.IntegerBase.UINT32: pa.uint32(),
+    st.IntegerBase.UINT16: pa.uint16(),
+    st.IntegerBase.UINT8: pa.uint8(),
 }
 
 IDBASE_TO_ARROW = {
     st.IdBase.INT64: pa.int64(),
     st.IdBase.INT32: pa.int32(),
     st.IdBase.INT16: pa.int16(),
     st.IdBase.INT8: pa.int8(),
@@ -256,14 +260,22 @@
         return sdt.Integer(base=st.IntegerBase.INT8)
     if pa.types.is_int16(type):
         return sdt.Integer(base=st.IntegerBase.INT16)
     if pa.types.is_int32(type):
         return sdt.Integer(base=st.IntegerBase.INT32)
     if pa.types.is_int64(type):
         return sdt.Integer(base=st.IntegerBase.INT64)
+    if pa.types.is_uint8(type):
+        return sdt.Integer(base=st.IntegerBase.UINT8)
+    if pa.types.is_uint16(type):
+        return sdt.Integer(base=st.IntegerBase.UINT16)
+    if pa.types.is_uint32(type):
+        return sdt.Integer(base=st.IntegerBase.UINT32)
+    if pa.types.is_uint64(type):
+        return sdt.Integer(base=st.IntegerBase.UINT64)
 
     # Floats
     if pa.types.is_float16(type):
         return sdt.Float(base=st.FloatBase.FLOAT16)
     if pa.types.is_float32(type):
         return sdt.Float(base=st.FloatBase.FLOAT32)
     if pa.types.is_float64(type):
@@ -312,15 +324,15 @@
             }
         )
     if pa.types.is_list(type):
         list_type = t.cast(pa.ListType, type)
         return sdt.List(
             type=type_from_arrow(list_type.value_type, nullable=False)
         )
-    raise NotImplementedError('Type not implemented')
+    raise NotImplementedError(f'Type {type} not implemented')
 
 
 def type_from_arrow(
     arrow_type: pa.DataType,
     nullable: bool,
 ) -> st.Type:
     if nullable and not (pa.types.is_null(arrow_type)):
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/base.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/config/privacy_properties.yaml` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/config/privacy_properties.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/constants.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/signature.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from sarus_data_spec.arrow.admin_utils import (
     async_admin_data,
     validate_admin_data,
 )
 from sarus_data_spec.dataspec_validator.parameter_kind import (
     DATASET,
     DATASPEC,
-    PEP,
     PEP_DATASET,
     SCALAR,
     STATIC,
     ParameterCondition,
     is_accepted,
 )
 from sarus_data_spec.manager.ops.processor.external.utils import (
@@ -42,14 +41,64 @@
         self.name = name
         self.condition = condition
         self.annotation = annotation
         self.default = default
         self.predicate = predicate
 
 
+class SarusParameterArray(SarusParameter):
+    """Class representing a variable number of positional arguments.
+
+    This is used to represent `*args` in signatures.
+
+    If used, it must be the first argument to a signature. All positional
+    arguments are captured by it.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        annotation: t.Any,
+        condition: ParameterCondition = STATIC | DATASPEC,
+        predicate: t.Callable[[t.Any], bool] = lambda _: True,
+    ):
+        super().__init__(
+            name=name,
+            annotation=annotation,
+            default=DefautValue.NO_DEFAULT,
+            condition=condition,
+            predicate=predicate,
+        )
+
+
+class SarusParameterMapping(SarusParameter):
+    """Class representing a variable number of named arguments.
+
+    This is used to represent `**kwargs` in signatures.
+
+    If used it must be the last argument to a signature. All remaining keyword
+    arguments are captured by it.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        annotation: t.Any,
+        condition: ParameterCondition = STATIC | DATASPEC,
+        predicate: t.Callable[[t.Any], bool] = lambda _: True,
+    ):
+        super().__init__(
+            name=name,
+            annotation=annotation,
+            default=DefautValue.NO_DEFAULT,
+            condition=condition,
+            predicate=predicate,
+        )
+
+
 class SarusSignature:
     """A Signature is a list of Parameters."""
 
     def __init__(self, *parameters: SarusParameter):
         self._parameters = list(parameters)
         self._parameter_map = {param.name: param for param in parameters}
 
@@ -77,27 +126,85 @@
         kwargs = {**py_kwargs, **ds_kwargs}
         args = [pos_args[i] for i in range(len(pos_args))]
         args_types = [ds_types.get(pos) for pos in range(len(args))]
         kwargs_types = {name: ds_types.get(name) for name in kwargs.keys()}
 
         # Pair arguments serialized in protobuf with the signature's
         # parameters
-        bound_args = [
-            SarusBoundArgument(self.parameters()[i], arg, args_types[i])
-            for i, arg in enumerate(args)
-        ]
-
-        bound_kwargs = [
-            SarusBoundArgument(
-                param, kwargs[param.name], kwargs_types[param.name]
+        if len(self.parameters()) > 0:
+            has_param_array = isinstance(
+                self.parameters()[0], SarusParameterArray
             )
-            for param in self.parameters()
-            if param.name in kwargs
-        ]
+            has_param_mapping = isinstance(
+                self.parameters()[-1], SarusParameterMapping
+            )
+        else:
+            has_param_array = False
+            has_param_mapping = False
+
+        if has_param_array:
+            # All positional arguments are captured by the array
+            param_array = self.parameters()[0]
+            bound_args = [
+                SarusBoundArgument(
+                    SarusParameter(
+                        name=f"{param_array.name}_{i}",
+                        annotation=param_array.annotation,
+                        default=param_array.default,
+                        condition=param_array.condition,
+                        predicate=param_array.predicate,
+                    ),
+                    arg,
+                    args_types[i],
+                    positional_only=True,
+                )
+                for i, arg in enumerate(args)
+            ]
+        else:
+            bound_args = [
+                SarusBoundArgument(self.parameters()[i], arg, args_types[i])
+                for i, arg in enumerate(args)
+            ]
+
+        if not has_param_mapping:
+            bound_kwargs = [
+                SarusBoundArgument(
+                    param, kwargs[param.name], kwargs_types[param.name]
+                )
+                for param in self.parameters()
+                if param.name in kwargs
+            ]
+        else:
+            # Capture all kwargs described in the signature
+            bound_kwargs = [
+                SarusBoundArgument(
+                    param, kwargs[param.name], kwargs_types[param.name]
+                )
+                for param in self.parameters()[:-1]
+                if param.name in kwargs
+            ]
+            # Remaining kwargs are bound to the parameter mapping
+            param_mapping = self.parameters()[-1]
+            already_bound_kwargs = [arg.name() for arg in bound_kwargs]
+            bound_kwargs += [
+                SarusBoundArgument(
+                    SarusParameter(
+                        name=name,
+                        annotation=param_mapping.annotation,
+                        condition=param_mapping.condition,
+                        predicate=param_mapping.predicate,
+                    ),
+                    value,
+                    kwargs_types[name],
+                )
+                for name, value in kwargs.items()
+                if name not in already_bound_kwargs
+            ]
 
+        # Check that all arguments have a unique name
         bound_arguments = bound_args + bound_kwargs
         bound_args_names = [bound_arg.name() for bound_arg in bound_arguments]
         if len(set(bound_args_names)) != len(bound_args_names):
             raise ValueError(
                 "An argument was specified more than "
                 "once in an external transform."
             )
@@ -107,24 +214,32 @@
             SarusBoundArgument(param, param.default)
             for param in self.parameters()
             if param.name not in bound_args_names
             and param.default != DefautValue.NO_DEFAULT
         ]
         bound_arguments += default_bound_args
 
-        if len(bound_arguments) != len(self.parameters()):
+        # Check number of arguments
+        if (
+            not has_param_array
+            and not has_param_mapping
+            and len(bound_arguments) != len(self.parameters())
+        ):
             raise ValueError(
                 "Invalid number of parameters serialized in external"
                 f" transform. Expected {len(self.parameters())}, "
                 f"got {len(bound_arguments)}."
             )
 
         # reorder arguments
-        arg_map = {arg.name(): arg for arg in bound_arguments}
-        bound_arguments = [arg_map[param.name] for param in self.parameters()]
+        if not has_param_array and not has_param_mapping:
+            arg_map = {arg.name(): arg for arg in bound_arguments}
+            bound_arguments = [
+                arg_map[param.name] for param in self.parameters()
+            ]
 
         return SarusBoundSignature(bound_arguments)
 
     def bind_dataspec(self, dataspec: st.DataSpec) -> SarusBoundSignature:
         if not dataspec.is_transformed():
             raise ValueError("Cannot bind a non transformed dataspec.")
 
@@ -173,30 +288,34 @@
     Args:
         parameter (SarusParameter):
             The Sarus parameter describing what is accepted.
         value (t.Union[st.DataSpec, t.Any]):
             The value as defined by the computation graph.
         kind (t.Optional[str]):
             The Python type a Dataset should be casted to.
+        positional_only (bool):
+            The argument is positional only and the name should be ignored.
     """
 
     dataset_types = {
         str(_type): t.cast(t.Type, _type)
         for _type in t.get_args(st.DatasetCastable)
     }
 
     def __init__(
         self,
         parameter: SarusParameter,
         value: t.Union[st.DataSpec, t.Any],
         kind: t.Optional[str] = None,
+        positional_only: bool = False,
     ):
         self.parameter = parameter
         self._value = value
         self.kind = kind
+        self.positional_only = positional_only
 
     def name(self) -> str:
         return self.parameter.name
 
     def static_value(self) -> t.Any:
         return self._value
 
@@ -215,35 +334,29 @@
                     return DATASET
             else:
                 return SCALAR
         else:
             return STATIC
 
     def pep_token(self) -> t.Optional[str]:
-        parameter_kind = self.parameter_kind()
-        if PEP.isin(parameter_kind):
-            dataset = t.cast(st.Dataset, self.static_value())
-            return dataset.pep_token()
+        if isinstance(self.static_value(), st.DataSpec):
+            dataspec = t.cast(st.DataSpec, self.static_value())
+            return dataspec.pep_token()
         else:
             return None
 
     def is_pep(self) -> bool:
         return self.pep_token() is not None
 
     def is_public(self) -> bool:
-        parameter_kind = self.parameter_kind()
-        if STATIC.isin(parameter_kind):
-            return True
-        elif DATASPEC.isin(parameter_kind):
+        if isinstance(self.static_value(), st.DataSpec):
             dataspec = t.cast(st.DataSpec, self.static_value())
             return dataspec.is_public()
         else:
-            raise ValueError(
-                f"Cannot determine if {parameter_kind} is public."
-            )
+            return True
 
     def static_validation(self) -> None:
         """Check that the argument is compatible with the parameter"""
         parameter_kind = self.parameter_kind()
         if not is_accepted(self.parameter.condition, parameter_kind):
             raise TypeError(
                 f"Expected parameter {self.name()} to be "
@@ -273,26 +386,27 @@
                 )
 
     async def dynamic_validation(self) -> None:
         ...
 
     async def collect(self) -> t.Any:
         """Evaluate the argument before calling the data function."""
-        parameter_kind = self.parameter_kind()
-        if DATASET.isin(parameter_kind):
-            dataset = t.cast(st.Dataset, self.static_value())
-            if self.kind is None:
-                raise ValueError(
-                    f"Parameter {self.name()} is a Dataset, but no type "
-                    "to cast to is defined."
-                )
-            return dataset.to(self.dataset_types[self.kind])
-        elif SCALAR.isin(parameter_kind):
-            scalar = t.cast(st.Scalar, self.static_value())
-            return scalar.value()
+        if isinstance(self.static_value(), st.DataSpec):
+            ds = t.cast(st.DataSpec, self.static_value())
+            if ds.prototype() == sp.Dataset:
+                dataset = t.cast(st.Dataset, self.static_value())
+                if self.kind is None:
+                    raise ValueError(
+                        f"Parameter {self.name()} is a Dataset, but no type "
+                        "to cast to is defined."
+                    )
+                return dataset.to(self.dataset_types[self.kind])
+            else:
+                scalar = t.cast(st.Scalar, ds)
+                return scalar.value()
         else:
             return self.static_value()
 
     async def admin_data(self) -> t.Optional[pa.Table]:
         if not self.is_pep():
             return None
 
@@ -326,45 +440,90 @@
         remove ForwardRefs.
         """
         for arg in self.arguments:
             await arg.dynamic_validation()
 
     def static_kwargs(self) -> t.Dict[str, t.Any]:
         """Return non evaluated arguments."""
+        assert not any([arg.positional_only for arg in self.arguments])
         return {
             arg.parameter.name: arg.static_value() for arg in self.arguments
         }
 
     def static_args(self) -> t.List[t.Any]:
         """Return non evaluated arguments."""
         return [arg.static_value() for arg in self.arguments]
 
     async def collect_kwargs(self) -> t.Dict[str, t.Any]:
         """Evaluate arguments for calling the data function."""
+        assert not any([arg.positional_only for arg in self.arguments])
         return {
             arg.parameter.name: await arg.collect() for arg in self.arguments
         }
 
     async def collect_args(self) -> t.List[t.Any]:
         """Evaluate arguments for calling the data function."""
         return [await arg.collect() for arg in self.arguments]
 
     async def collect_kwargs_method(
         self,
     ) -> t.Tuple[t.Any, t.Dict[str, t.Any]]:
-        """Evaluate the arguments but separate the first argument from the
-        rest. This is useful to evaluate a method.
+        """Evaluate the arguments.
+
+        Return a tuple (self, kwargs)
         """
+        assert not any([arg.positional_only for arg in self.arguments])
         first_value = await self.arguments[0].collect()
         other_values = {
             arg.parameter.name: await arg.collect()
             for arg in self.arguments[1:]
         }
         return first_value, other_values
 
+    async def collect_method(
+        self,
+    ) -> t.Tuple[t.Any, t.List[t.Any], t.Dict[str, t.Any]]:
+        """Evaluate the arguments.
+
+        Return a tuple (self, args, kwargs).
+        """
+        first_value = await self.arguments[0].collect()
+        positional_values = [
+            await arg.collect()
+            for arg in self.arguments[1:]
+            if arg.positional_only
+        ]
+        keyword_values = {
+            arg.name(): await arg.collect()
+            for arg in self.arguments[1:]
+            if not arg.positional_only
+        }
+
+        return first_value, positional_values, keyword_values
+
+    async def collect(
+        self,
+    ) -> t.Tuple[t.List[t.Any], t.Dict[str, t.Any]]:
+        """Evaluate the arguments.
+
+        Return a tuple (args, kwargs).
+        """
+        positional_values = [
+            await arg.collect()
+            for arg in self.arguments
+            if arg.positional_only
+        ]
+        keyword_values = {
+            arg.name(): await arg.collect()
+            for arg in self.arguments
+            if not arg.positional_only
+        }
+
+        return positional_values, keyword_values
+
     def pep_token(self) -> t.Optional[str]:
         """Compute the PEP token of the inputs.
 
         A PEP token exists if:
           - all input dataspecs are PEP or PUBLIC
           - there must be at least one input PEP dataspec
           - if there are more that one input PEP dataspecs, all PEP inputs must
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/json_serialisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,23 @@
                 '_type': 'class',
                 'data': {'"name"': obj.__name__, '"module"': obj.__module__},
             }
         elif isinstance(obj, pd.api.extensions.ExtensionDtype):
             return {'_type': 'dtype', 'data': str(obj)}
         elif isinstance(obj, slice):
             return {'_type': 'slice', 'data': (obj.start, obj.stop, obj.step)}
+        elif isinstance(obj, range):
+            return {
+                '_type': 'range',
+                'data': {
+                    '"start"': obj.start,
+                    '"stop"': obj.stop,
+                    '"step"': obj.step,
+                },
+            }
         return super().default(obj)
 
     def encode_obj(self, obj: Any) -> Any:
         if isinstance(obj, tuple):
             return {
                 '_type': 'tuple',
                 'data': [self.encode_obj(v) for v in obj],
@@ -183,14 +192,16 @@
                             raise ValueError("Decoded object is not a type")
                     else:
                         raise ValueError("Invalid module name")
                 elif obj['_type'] == 'dtype':
                     return pd.api.types.pandas_dtype(data)
                 elif obj['_type'] == 'slice':
                     return slice(*data)
+                elif obj['_type'] == 'range':
+                    return range(data['start'], data['stop'], data['step'])
             return {self.decode(k): self.decode_obj(v) for k, v in obj.items()}
         elif isinstance(obj, list):
             return [self.decode_obj(v) for v in obj]
         return obj
 
     @classmethod
     def decode_bytes(cls, b: bytes, *args: Any, **kwargs: Any) -> Any:
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,27 +134,28 @@
         dataspec: st.DataSpec,
     ) -> st.Status:
         """The DataSpec already has an Error status.
         In this case, we clear the statuses so that the
         task can be relaunched in the future.
         """
         status = self.status(dataspec)
-        assert status
-        stage = status.task(self.task_name)
-        assert stage
-        should_clear = status_error_policy(stage=stage)
-        if should_clear:
-            stt.clear_task(dataspec=dataspec, task=self.task_name)
-            return await self.complete_task(dataspec=dataspec)
-        raise stt.DataSpecErrorStatus(
-            (
-                stage.properties()["relaunch"] == str(True),
-                stage.properties()["message"],
+        if status is not None:
+            stage = status.task(self.task_name)
+            assert stage
+            should_clear = status_error_policy(stage=stage)
+            if should_clear:
+                status.clear_task(self.task_name)
+                return await self.complete_task(dataspec=dataspec)
+            raise stt.DataSpecErrorStatus(
+                (
+                    stage.properties()["relaunch"] == str(True),
+                    stage.properties()["message"],
+                )
             )
-        )
+        return await self.complete_task(dataspec=dataspec)
 
     async def wait_for_computation(
         self,
         dataspec: st.DataSpec,
         current_stage: str,
         timeout: int = 300,
         max_delay: int = 10,
@@ -176,14 +177,28 @@
                 total_wait += delay
                 delay = min(2 * delay, max_delay, timeout - total_wait)
             else:
                 break
         assert stage
         return stage
 
+    def force_launch(self, dataspec: st.DataSpec) -> None:
+        """Method to force launch when an existing
+        status with relaunch=true exists. it creates
+        a new status without the task in question
+        and calls launch task"""
+        status = self.status(dataspec=dataspec)
+        if status is not None:
+            stage = status.task(self.task_name)
+            assert stage
+            should_clear = status_error_policy(stage=stage)
+            if should_clear:
+                status.clear_task(self.task_name)
+                self.launch_task(dataspec=dataspec)
+
 
 class ErrorCatchingAsyncIterator:
     """Wrap an AsyncIterator and catches potential errors.
 
     When an error occurs, this sets the Dataspec status to error
     accordingly.
     """
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from numpy.typing import ArrayLike, DTypeLike
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC, STATIC
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusParameter,
+    SarusParameterArray,
     SarusSignature,
 )
 
 from .external_op import ExternalOpImplementation
 
 Casting = Literal["no", "equiv", "safe", "same_kind", "unsafe"]
 Order = Literal["K", "A", "C", "F"]
@@ -243,24 +244,23 @@
         kwargs = await signature.collect_kwargs()
         return np.std(**kwargs)
 
 
 class np_rand(ExternalOpImplementation):
     _transform_id = "numpy.NP_RAND"
     _signature = SarusSignature(
-        SarusParameter(
+        SarusParameterArray(
             name="size",
             annotation=Optional[Union[int, List[int]]],
-            default=None,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
-        return np.random.random_sample(**kwargs)
+        sizes = await signature.collect_args()
+        return np.random.random_sample(sizes)
 
 
 # ------ METHODS ------
 class np_astype(ExternalOpImplementation):
     _transform_id = "numpy.NP_ASTYPE"
     _signature = SarusSignature(
         SarusParameter(
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -558,14 +558,16 @@
             annotation=str,
             default="raise",
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> t.Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["axis"]
         return this.drop(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         axis = signature["axis"].static_value()
         if axis in [0, 'columns']:
             return PEPKind.PEP
         else:
@@ -606,14 +608,17 @@
             default=False,
             predicate=lambda x: x is False,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> t.Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["subset"]
+            del kwargs["thresh"]
         return this.dropna(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         axis = signature["axis"].static_value()
         if axis in [0, 'columns']:
             return PEPKind.PEP
         else:
@@ -986,14 +991,16 @@
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["axis"]
         return this.add(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_sub(ExternalOpImplementation):
@@ -1025,14 +1032,16 @@
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["axis"]
         return this.sub(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_reset_index(ExternalOpImplementation):
@@ -1080,14 +1089,17 @@
         #     annotation=Optional[Union[Hashable, Sequence[Hashable]]],
         #     default=None,
         # ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["col_level"]
+            del kwargs["col_fill"]
         return this.reset_index(**kwargs)
 
 
 class pd_min(ExternalOpImplementation):
     _transform_id = "pandas.PD_MIN"
     _signature = SarusSignature(
         SarusParameter(
@@ -1276,14 +1288,17 @@
         #     annotation=Literal["single", "table"],
         #     default="single",
         # ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["axis"]
+            del kwargs["numeric_only"]
         return this.quantile(**kwargs)
 
 
 class pd_reindex(ExternalOpImplementation):
     _transform_id = "pandas.PD_REINDEX"
     _signature = SarusSignature(
         SarusParameter(
@@ -1373,14 +1388,17 @@
             annotation=bool,
             default=False,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["axis"]
+            del kwargs["numeric_only"]
         return this.count(**kwargs)
 
 
 class pd_transpose(ExternalOpImplementation):
     _transform_id = "pandas.PD_TRANSPOSE"
     _signature = SarusSignature(
         SarusParameter(
@@ -1433,14 +1451,16 @@
             annotation=bool,
             default=True,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["subset"]
         return this.value_counts(**kwargs)
 
 
 class pd_to_dict(ExternalOpImplementation):
     _transform_id = "pandas.PD_TO_DICT"
     _signature = SarusSignature(
         SarusParameter(
@@ -1501,14 +1521,18 @@
             annotation=Optional[Literal["expand", "reduce", "broadcast"]],
             default=None,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["axis"]
+            del kwargs["result_type"]
+            del kwargs["raw"]
         return this.apply(**kwargs)
 
 
 class pd_skew(ExternalOpImplementation):
     _transform_id = "pandas.PD_SKEW"
     _signature = SarusSignature(
         SarusParameter(
@@ -1665,14 +1689,17 @@
             annotation=ValueKeyFunc,
             default=None,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["axis"]
+            del kwargs["by"]
         return this.sort_values(**kwargs)
 
 
 class pd_drop_duplicates(ExternalOpImplementation):
     _transform_id = "pandas.PD_DROP_DUPLICATES"
     _signature = SarusSignature(
         SarusParameter(
@@ -1701,23 +1728,26 @@
             annotation=bool,
             default=False,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["subset"]
+            del kwargs["ignore_index"]
         return this.drop_duplicates(**kwargs)
 
 
 class pd_corr(ExternalOpImplementation):
     _transform_id = "pandas.PD_CORR"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
-            annotation=Union[pd.DataFrame, pd.Series],
+            annotation=pd.DataFrame,
             condition=DATASPEC,
         ),
         SarusParameter(
             name="method",
             annotation=CorrelationMethod,
             default="pearson",
         ),
@@ -1735,14 +1765,48 @@
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
         return this.corr(**kwargs)
 
 
+class pd_corr_series(ExternalOpImplementation):
+    _transform_id = "pandas.PD_CORR_SERIES"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=pd.Series,
+        ),
+        SarusParameter(
+            name="other",
+            annotation=pd.Series,
+        ),
+        SarusParameter(
+            name="method",
+            annotation=CorrelationMethod,
+            default="pearson",
+        ),
+        SarusParameter(
+            name="min_periods",
+            annotation=int,
+            default=1,
+        ),
+        # > 1.3.5
+        # SarusParameter(
+        #     name="numeric_only",
+        #     annotation=bool,
+        #     default=False,
+        # ),
+    )
+
+    async def call(self, signature: SarusBoundSignature) -> Any:
+        this, kwargs = await signature.collect_kwargs_method()
+        return this.corr(**kwargs)
+
+
 # ------ DataFrame & Series PROPERTIES ------
 class pd_shape(ExternalOpImplementation):
     _transform_id = "pandas.PD_SHAPE"
     _dp_equivalent_id = "pandas.PD_SHAPE_DP"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -2121,14 +2185,16 @@
             annotation=bool,
             default=True,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
+        if signature["this"].python_type() == str(pd.Series):
+            del kwargs["axis"]
         return this.nunique(**kwargs)
 
 
 class pd_rolling(ExternalOpImplementation):
     _transform_id = "pandas.PD_ROLLING"
     _signature = SarusSignature(
         SarusParameter(
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,33 @@
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
         fitted_model = this.fit(**kwargs)
         return fitted_model
 
 
+class sk_fit_y(ExternalOpImplementation):
+    _transform_id = "sklearn.SK_FIT_Y"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=BaseEstimator,
+        ),
+        SarusParameter(
+            name="y",
+            annotation=Union[npt.ArrayLike, spmatrix],
+        ),
+    )
+
+    async def call(self, signature: SarusBoundSignature) -> Any:
+        this, kwargs = await signature.collect_kwargs_method()
+        fitted_model = this.fit(**kwargs)
+        return fitted_model
+
+
 class sk_predict(ExternalOpImplementation):
     _transform_id = "sklearn.SK_PREDICT"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=BaseEstimator,
         ),
@@ -111,16 +130,16 @@
         SarusParameter(
             name="X",
             annotation=Union[npt.ArrayLike, spmatrix],
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
-        return this.transform(**kwargs)
+        (this, X) = await signature.collect_args()
+        return this.transform(X)
 
 
 class sk_inverse_transform(ExternalOpImplementation):
     _transform_id = "sklearn.SK_INVERSE_TRANSFORM"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -129,16 +148,16 @@
         SarusParameter(
             name="X",
             annotation=Union[npt.ArrayLike, spmatrix],
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
-        return this.inverse_transform(**kwargs)
+        this, X = await signature.collect_args()
+        return this.inverse_transform(X)
 
 
 class sk_score(ExternalOpImplementation):
     _transform_id = "sklearn.SK_SCORE"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import numpy.typing as npt
 import pandas as pd
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC, STATIC
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusParameter,
+    SarusParameterArray,
     SarusSignature,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from scipy.sparse import spmatrix
@@ -147,15 +148,15 @@
         kwargs = await signature.collect_kwargs()
         return model_selection.cross_val_score(**kwargs)
 
 
 class sk_train_test_split(ExternalOpImplementation):
     _transform_id = "sklearn.SK_TRAIN_TEST_SPLIT"
     _signature = SarusSignature(
-        SarusParameter(
+        SarusParameterArray(
             name="arrays",
             annotation=Sequence[
                 Union[List, np.ndarray, spmatrix, pd.DataFrame]
             ],
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
@@ -182,15 +183,15 @@
             name="stratify",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
-        arrays, kwargs = await signature.collect_kwargs_method()
+        arrays, kwargs = await signature.collect()
         return model_selection.train_test_split(*arrays, **kwargs)
 
 
 class sk_time_series_split(ExternalOpImplementation):
     _transform_id = "sklearn.SK_TIME_SERIES_SPLIT"
     _signature = SarusSignature(
         SarusParameter(
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Any, Dict, List, Optional
 
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusParameter,
+    SarusParameterArray,
+    SarusParameterMapping,
     SarusSignature,
 )
 from sarus_data_spec.dataspec_validator.typing import PEPKind
 
 from .external_op import ExternalOpImplementation
 
 
@@ -534,37 +536,37 @@
         (this,) = await signature.collect_args()
         return float(this)
 
 
 class _list(ExternalOpImplementation):
     _transform_id = "std.LIST"
     _signature = SarusSignature(
-        SarusParameter(
-            name="this",
+        SarusParameterArray(
+            name="elem",
             annotation=Any,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
-        return list(this)
+        elems = await signature.collect_args()
+        return list(elems)
 
 
 class _dict(ExternalOpImplementation):
     _transform_id = "std.DICT"
     _signature = SarusSignature(
-        SarusParameter(
-            name="this",
+        SarusParameterMapping(
+            name="elem",
             annotation=Any,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
-        return dict(this)
+        _, elems = await signature.collect()
+        return dict(**elems)
 
 
 class _slice(ExternalOpImplementation):
     _transform_id = "std.SLICE"
     _signature = SarusSignature(
         SarusParameter(
             name="start",
@@ -587,37 +589,37 @@
         (start, stop, step) = await signature.collect_args()
         return slice(start, stop, step)
 
 
 class _set(ExternalOpImplementation):
     _transform_id = "std.SET"
     _signature = SarusSignature(
-        SarusParameter(
-            name="this",
+        SarusParameterArray(
+            name="elem",
             annotation=Any,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
-        return set(this)
+        elems = await signature.collect_args()
+        return set(elems)
 
 
 class _tuple(ExternalOpImplementation):
     _transform_id = "std.TUPLE"
     _signature = SarusSignature(
-        SarusParameter(
-            name="this",
+        SarusParameterArray(
+            name="elem",
             annotation=Any,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
-        return tuple(this)
+        elems = await signature.collect_args()
+        return tuple(elems)
 
 
 class keys(ExternalOpImplementation):
     _transform_id = "std.KEYS"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/select_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/path.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type.proto`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,18 @@
     int64 max = 3;
     repeated int64 possible_values = 4;
     enum Base {
       INT64 = 0;
       INT32 = 1;
       INT16 = 2;
       INT8 = 3;
+      UINT64 = 4;
+      UINT32 = 5;
+      UINT16 = 6;
+      UINT8 = 7;
     }
   }
 
   message Enum {
     Base base = 1;
     bool ordered = 2;
     repeated NameValue name_values = 3;
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='sarus_data_spec/protobuf/type.proto',
   package='sarus_data_spec',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n#sarus_data_spec/protobuf/type.proto\x12\x0fsarus_data_spec\x1a(sarus_data_spec/protobuf/predicate.proto\x1a#sarus_data_spec/protobuf/path.proto\"\xcb\x18\n\x04Type\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04null\x18\x03 \x01(\x0b\x32\x1a.sarus_data_spec.Type.NullH\x00\x12*\n\x04unit\x18\x04 \x01(\x0b\x32\x1a.sarus_data_spec.Type.UnitH\x00\x12\x30\n\x07\x62oolean\x18\x05 \x01(\x0b\x32\x1d.sarus_data_spec.Type.BooleanH\x00\x12\x30\n\x07integer\x18\x06 \x01(\x0b\x32\x1d.sarus_data_spec.Type.IntegerH\x00\x12*\n\x04\x65num\x18\x07 \x01(\x0b\x32\x1a.sarus_data_spec.Type.EnumH\x00\x12,\n\x05\x66loat\x18\x08 \x01(\x0b\x32\x1b.sarus_data_spec.Type.FloatH\x00\x12*\n\x04text\x18\t \x01(\x0b\x32\x1a.sarus_data_spec.Type.TextH\x00\x12,\n\x05\x62ytes\x18\n \x01(\x0b\x32\x1b.sarus_data_spec.Type.BytesH\x00\x12.\n\x06struct\x18\x0b \x01(\x0b\x32\x1c.sarus_data_spec.Type.StructH\x00\x12,\n\x05union\x18\x0c \x01(\x0b\x32\x1b.sarus_data_spec.Type.UnionH\x00\x12\x32\n\x08optional\x18\r \x01(\x0b\x32\x1e.sarus_data_spec.Type.OptionalH\x00\x12*\n\x04list\x18\x0e \x01(\x0b\x32\x1a.sarus_data_spec.Type.ListH\x00\x12,\n\x05\x61rray\x18\x0f \x01(\x0b\x32\x1b.sarus_data_spec.Type.ArrayH\x00\x12\x32\n\x08\x64\x61tetime\x18\x10 \x01(\x0b\x32\x1e.sarus_data_spec.Type.DatetimeH\x00\x12\x38\n\x0b\x63onstrained\x18\x11 \x01(\x0b\x32!.sarus_data_spec.Type.ConstrainedH\x00\x12\x36\n\nhypothesis\x18\x12 \x01(\x0b\x32 .sarus_data_spec.Type.HypothesisH\x00\x12&\n\x02id\x18\x13 \x01(\x0b\x32\x18.sarus_data_spec.Type.IdH\x00\x12*\n\x04\x64\x61te\x18\x14 \x01(\x0b\x32\x1a.sarus_data_spec.Type.DateH\x00\x12*\n\x04time\x18\x15 \x01(\x0b\x32\x1a.sarus_data_spec.Type.TimeH\x00\x12\x32\n\x08\x64uration\x18\x16 \x01(\x0b\x32\x1e.sarus_data_spec.Type.DurationH\x00\x12\x39\n\nproperties\x18\x02 \x03(\x0b\x32%.sarus_data_spec.Type.PropertiesEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x06\n\x04Null\x1a\x06\n\x04Unit\x1a\t\n\x07\x42oolean\x1a\xa1\x01\n\x07Integer\x12\x30\n\x04\x62\x61se\x18\x01 \x01(\x0e\x32\".sarus_data_spec.Type.Integer.Base\x12\x0b\n\x03min\x18\x02 \x01(\x03\x12\x0b\n\x03max\x18\x03 \x01(\x03\x12\x17\n\x0fpossible_values\x18\x04 \x03(\x03\"1\n\x04\x42\x61se\x12\t\n\x05INT64\x10\x00\x12\t\n\x05INT32\x10\x01\x12\t\n\x05INT16\x10\x02\x12\x08\n\x04INT8\x10\x03\x1a\xde\x01\n\x04\x45num\x12-\n\x04\x62\x61se\x18\x01 \x01(\x0e\x32\x1f.sarus_data_spec.Type.Enum.Base\x12\x0f\n\x07ordered\x18\x02 \x01(\x08\x12\x39\n\x0bname_values\x18\x03 \x03(\x0b\x32$.sarus_data_spec.Type.Enum.NameValue\x1a(\n\tNameValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03\"1\n\x04\x42\x61se\x12\t\n\x05INT64\x10\x00\x12\t\n\x05INT32\x10\x01\x12\t\n\x05INT16\x10\x02\x12\x08\n\x04INT8\x10\x03\x1a\x99\x01\n\x05\x46loat\x12.\n\x04\x62\x61se\x18\x01 \x01(\x0e\x32 .sarus_data_spec.Type.Float.Base\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x17\n\x0fpossible_values\x18\x04 \x03(\x01\"-\n\x04\x42\x61se\x12\x0b\n\x07\x46LOAT64\x10\x00\x12\x0b\n\x07\x46LOAT32\x10\x01\x12\x0b\n\x07\x46LOAT16\x10\x02\x1a\x31\n\x04Text\x12\x10\n\x08\x65ncoding\x18\x01 \x01(\t\x12\x17\n\x0fpossible_values\x18\x02 \x03(\t\x1a\x07\n\x05\x42ytes\x1ax\n\x06Struct\x12\x32\n\x06\x66ields\x18\x01 \x03(\x0b\x32\".sarus_data_spec.Type.Struct.Field\x1a:\n\x05\x46ield\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x04type\x18\x02 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1av\n\x05Union\x12\x31\n\x06\x66ields\x18\x01 \x03(\x0b\x32!.sarus_data_spec.Type.Union.Field\x1a:\n\x05\x46ield\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x04type\x18\x02 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x08Optional\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a=\n\x04List\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12\x10\n\x08max_size\x18\x02 \x01(\x03\x1a;\n\x05\x41rray\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12\r\n\x05shape\x18\x02 \x03(\x03\x1a\xb0\x01\n\x08\x44\x61tetime\x12\x0e\n\x06\x66ormat\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x02 \x01(\t\x12\x0b\n\x03max\x18\x03 \x01(\t\x12\x17\n\x0fpossible_values\x18\x04 \x03(\t\x12\x31\n\x04\x62\x61se\x18\x05 \x01(\x0e\x32#.sarus_data_spec.Type.Datetime.Base\".\n\x04\x42\x61se\x12\x0c\n\x08INT64_NS\x10\x00\x12\x0c\n\x08INT64_MS\x10\x01\x12\n\n\x06STRING\x10\x02\x1a\x97\x01\n\x04\x44\x61te\x12\x0e\n\x06\x66ormat\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x02 \x01(\t\x12\x0b\n\x03max\x18\x03 \x01(\t\x12\x17\n\x0fpossible_values\x18\x04 \x03(\t\x12-\n\x04\x62\x61se\x18\x05 \x01(\x0e\x32\x1f.sarus_data_spec.Type.Date.Base\"\x1d\n\x04\x42\x61se\x12\t\n\x05INT32\x10\x00\x12\n\n\x06STRING\x10\x01\x1a\xb6\x01\n\x04Time\x12\x0e\n\x06\x66ormat\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x02 \x01(\t\x12\x0b\n\x03max\x18\x03 \x01(\t\x12\x17\n\x0fpossible_values\x18\x04 \x03(\t\x12-\n\x04\x62\x61se\x18\x05 \x01(\x0e\x32\x1f.sarus_data_spec.Type.Time.Base\"<\n\x04\x42\x61se\x12\x0c\n\x08INT64_NS\x10\x00\x12\x0c\n\x08INT32_MS\x10\x01\x12\n\n\x06STRING\x10\x02\x12\x0c\n\x08INT64_US\x10\x03\x1aK\n\x08\x44uration\x12\x0c\n\x04unit\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x02 \x01(\x03\x12\x0b\n\x03max\x18\x03 \x01(\x03\x12\x17\n\x0fpossible_values\x18\x04 \x03(\x03\x1a\x62\n\x0b\x43onstrained\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12.\n\nconstraint\x18\x02 \x01(\x0b\x32\x1a.sarus_data_spec.Predicate\x1a\x82\x01\n\nHypothesis\x12\x36\n\x05types\x18\x02 \x03(\x0b\x32\'.sarus_data_spec.Type.Hypothesis.Scored\x1a<\n\x06Scored\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12\r\n\x05score\x18\x02 \x01(\x01\x1a\xb5\x01\n\x02Id\x12+\n\x04\x62\x61se\x18\x01 \x01(\x0e\x32\x1d.sarus_data_spec.Type.Id.Base\x12\x0e\n\x06unique\x18\x02 \x01(\x08\x12(\n\treference\x18\x03 \x01(\x0b\x32\x15.sarus_data_spec.Path\"H\n\x04\x42\x61se\x12\t\n\x05INT64\x10\x00\x12\t\n\x05INT32\x10\x01\x12\t\n\x05INT16\x10\x02\x12\x08\n\x04INT8\x10\x03\x12\n\n\x06STRING\x10\x04\x12\t\n\x05\x42YTES\x10\x05\x42\x06\n\x04typeb\x06proto3'
+  serialized_pb=b'\n#sarus_data_spec/protobuf/type.proto\x12\x0fsarus_data_spec\x1a(sarus_data_spec/protobuf/predicate.proto\x1a#sarus_data_spec/protobuf/path.proto\"\xfa\x18\n\x04Type\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x04null\x18\x03 \x01(\x0b\x32\x1a.sarus_data_spec.Type.NullH\x00\x12*\n\x04unit\x18\x04 \x01(\x0b\x32\x1a.sarus_data_spec.Type.UnitH\x00\x12\x30\n\x07\x62oolean\x18\x05 \x01(\x0b\x32\x1d.sarus_data_spec.Type.BooleanH\x00\x12\x30\n\x07integer\x18\x06 \x01(\x0b\x32\x1d.sarus_data_spec.Type.IntegerH\x00\x12*\n\x04\x65num\x18\x07 \x01(\x0b\x32\x1a.sarus_data_spec.Type.EnumH\x00\x12,\n\x05\x66loat\x18\x08 \x01(\x0b\x32\x1b.sarus_data_spec.Type.FloatH\x00\x12*\n\x04text\x18\t \x01(\x0b\x32\x1a.sarus_data_spec.Type.TextH\x00\x12,\n\x05\x62ytes\x18\n \x01(\x0b\x32\x1b.sarus_data_spec.Type.BytesH\x00\x12.\n\x06struct\x18\x0b \x01(\x0b\x32\x1c.sarus_data_spec.Type.StructH\x00\x12,\n\x05union\x18\x0c \x01(\x0b\x32\x1b.sarus_data_spec.Type.UnionH\x00\x12\x32\n\x08optional\x18\r \x01(\x0b\x32\x1e.sarus_data_spec.Type.OptionalH\x00\x12*\n\x04list\x18\x0e \x01(\x0b\x32\x1a.sarus_data_spec.Type.ListH\x00\x12,\n\x05\x61rray\x18\x0f \x01(\x0b\x32\x1b.sarus_data_spec.Type.ArrayH\x00\x12\x32\n\x08\x64\x61tetime\x18\x10 \x01(\x0b\x32\x1e.sarus_data_spec.Type.DatetimeH\x00\x12\x38\n\x0b\x63onstrained\x18\x11 \x01(\x0b\x32!.sarus_data_spec.Type.ConstrainedH\x00\x12\x36\n\nhypothesis\x18\x12 \x01(\x0b\x32 .sarus_data_spec.Type.HypothesisH\x00\x12&\n\x02id\x18\x13 \x01(\x0b\x32\x18.sarus_data_spec.Type.IdH\x00\x12*\n\x04\x64\x61te\x18\x14 \x01(\x0b\x32\x1a.sarus_data_spec.Type.DateH\x00\x12*\n\x04time\x18\x15 \x01(\x0b\x32\x1a.sarus_data_spec.Type.TimeH\x00\x12\x32\n\x08\x64uration\x18\x16 \x01(\x0b\x32\x1e.sarus_data_spec.Type.DurationH\x00\x12\x39\n\nproperties\x18\x02 \x03(\x0b\x32%.sarus_data_spec.Type.PropertiesEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x06\n\x04Null\x1a\x06\n\x04Unit\x1a\t\n\x07\x42oolean\x1a\xd0\x01\n\x07Integer\x12\x30\n\x04\x62\x61se\x18\x01 \x01(\x0e\x32\".sarus_data_spec.Type.Integer.Base\x12\x0b\n\x03min\x18\x02 \x01(\x03\x12\x0b\n\x03max\x18\x03 \x01(\x03\x12\x17\n\x0fpossible_values\x18\x04 \x03(\x03\"`\n\x04\x42\x61se\x12\t\n\x05INT64\x10\x00\x12\t\n\x05INT32\x10\x01\x12\t\n\x05INT16\x10\x02\x12\x08\n\x04INT8\x10\x03\x12\n\n\x06UINT64\x10\x04\x12\n\n\x06UINT32\x10\x05\x12\n\n\x06UINT16\x10\x06\x12\t\n\x05UINT8\x10\x07\x1a\xde\x01\n\x04\x45num\x12-\n\x04\x62\x61se\x18\x01 \x01(\x0e\x32\x1f.sarus_data_spec.Type.Enum.Base\x12\x0f\n\x07ordered\x18\x02 \x01(\x08\x12\x39\n\x0bname_values\x18\x03 \x03(\x0b\x32$.sarus_data_spec.Type.Enum.NameValue\x1a(\n\tNameValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03\"1\n\x04\x42\x61se\x12\t\n\x05INT64\x10\x00\x12\t\n\x05INT32\x10\x01\x12\t\n\x05INT16\x10\x02\x12\x08\n\x04INT8\x10\x03\x1a\x99\x01\n\x05\x46loat\x12.\n\x04\x62\x61se\x18\x01 \x01(\x0e\x32 .sarus_data_spec.Type.Float.Base\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x17\n\x0fpossible_values\x18\x04 \x03(\x01\"-\n\x04\x42\x61se\x12\x0b\n\x07\x46LOAT64\x10\x00\x12\x0b\n\x07\x46LOAT32\x10\x01\x12\x0b\n\x07\x46LOAT16\x10\x02\x1a\x31\n\x04Text\x12\x10\n\x08\x65ncoding\x18\x01 \x01(\t\x12\x17\n\x0fpossible_values\x18\x02 \x03(\t\x1a\x07\n\x05\x42ytes\x1ax\n\x06Struct\x12\x32\n\x06\x66ields\x18\x01 \x03(\x0b\x32\".sarus_data_spec.Type.Struct.Field\x1a:\n\x05\x46ield\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x04type\x18\x02 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1av\n\x05Union\x12\x31\n\x06\x66ields\x18\x01 \x03(\x0b\x32!.sarus_data_spec.Type.Union.Field\x1a:\n\x05\x46ield\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x04type\x18\x02 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x08Optional\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a=\n\x04List\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12\x10\n\x08max_size\x18\x02 \x01(\x03\x1a;\n\x05\x41rray\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12\r\n\x05shape\x18\x02 \x03(\x03\x1a\xb0\x01\n\x08\x44\x61tetime\x12\x0e\n\x06\x66ormat\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x02 \x01(\t\x12\x0b\n\x03max\x18\x03 \x01(\t\x12\x17\n\x0fpossible_values\x18\x04 \x03(\t\x12\x31\n\x04\x62\x61se\x18\x05 \x01(\x0e\x32#.sarus_data_spec.Type.Datetime.Base\".\n\x04\x42\x61se\x12\x0c\n\x08INT64_NS\x10\x00\x12\x0c\n\x08INT64_MS\x10\x01\x12\n\n\x06STRING\x10\x02\x1a\x97\x01\n\x04\x44\x61te\x12\x0e\n\x06\x66ormat\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x02 \x01(\t\x12\x0b\n\x03max\x18\x03 \x01(\t\x12\x17\n\x0fpossible_values\x18\x04 \x03(\t\x12-\n\x04\x62\x61se\x18\x05 \x01(\x0e\x32\x1f.sarus_data_spec.Type.Date.Base\"\x1d\n\x04\x42\x61se\x12\t\n\x05INT32\x10\x00\x12\n\n\x06STRING\x10\x01\x1a\xb6\x01\n\x04Time\x12\x0e\n\x06\x66ormat\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x02 \x01(\t\x12\x0b\n\x03max\x18\x03 \x01(\t\x12\x17\n\x0fpossible_values\x18\x04 \x03(\t\x12-\n\x04\x62\x61se\x18\x05 \x01(\x0e\x32\x1f.sarus_data_spec.Type.Time.Base\"<\n\x04\x42\x61se\x12\x0c\n\x08INT64_NS\x10\x00\x12\x0c\n\x08INT32_MS\x10\x01\x12\n\n\x06STRING\x10\x02\x12\x0c\n\x08INT64_US\x10\x03\x1aK\n\x08\x44uration\x12\x0c\n\x04unit\x18\x01 \x01(\t\x12\x0b\n\x03min\x18\x02 \x01(\x03\x12\x0b\n\x03max\x18\x03 \x01(\x03\x12\x17\n\x0fpossible_values\x18\x04 \x03(\x03\x1a\x62\n\x0b\x43onstrained\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12.\n\nconstraint\x18\x02 \x01(\x0b\x32\x1a.sarus_data_spec.Predicate\x1a\x82\x01\n\nHypothesis\x12\x36\n\x05types\x18\x02 \x03(\x0b\x32\'.sarus_data_spec.Type.Hypothesis.Scored\x1a<\n\x06Scored\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12\r\n\x05score\x18\x02 \x01(\x01\x1a\xb5\x01\n\x02Id\x12+\n\x04\x62\x61se\x18\x01 \x01(\x0e\x32\x1d.sarus_data_spec.Type.Id.Base\x12\x0e\n\x06unique\x18\x02 \x01(\x08\x12(\n\treference\x18\x03 \x01(\x0b\x32\x15.sarus_data_spec.Path\"H\n\x04\x42\x61se\x12\t\n\x05INT64\x10\x00\x12\t\n\x05INT32\x10\x01\x12\t\n\x05INT16\x10\x02\x12\x08\n\x04INT8\x10\x03\x12\n\n\x06STRING\x10\x04\x12\t\n\x05\x42YTES\x10\x05\x42\x06\n\x04typeb\x06proto3'
   ,
   dependencies=[sarus__data__spec_dot_protobuf_dot_predicate__pb2.DESCRIPTOR,sarus__data__spec_dot_protobuf_dot_path__pb2.DESCRIPTOR,])
 
 
 
 _TYPE_INTEGER_BASE = _descriptor.EnumDescriptor(
   name='Base',
@@ -50,19 +50,39 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='INT8', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='UINT64', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='UINT32', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='UINT16', index=6, number=6,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='UINT8', index=7, number=7,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
   serialized_start=1358,
-  serialized_end=1407,
+  serialized_end=1454,
 )
 _sym_db.RegisterEnumDescriptor(_TYPE_INTEGER_BASE)
 
 _TYPE_ENUM_BASE = _descriptor.EnumDescriptor(
   name='Base',
   full_name='sarus_data_spec.Type.Enum.Base',
   filename=None,
@@ -118,16 +138,16 @@
       name='FLOAT16', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1743,
-  serialized_end=1788,
+  serialized_start=1790,
+  serialized_end=1835,
 )
 _sym_db.RegisterEnumDescriptor(_TYPE_FLOAT_BASE)
 
 _TYPE_DATETIME_BASE = _descriptor.EnumDescriptor(
   name='Base',
   full_name='sarus_data_spec.Type.Datetime.Base',
   filename=None,
@@ -148,16 +168,16 @@
       name='STRING', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2396,
-  serialized_end=2442,
+  serialized_start=2443,
+  serialized_end=2489,
 )
 _sym_db.RegisterEnumDescriptor(_TYPE_DATETIME_BASE)
 
 _TYPE_DATE_BASE = _descriptor.EnumDescriptor(
   name='Base',
   full_name='sarus_data_spec.Type.Date.Base',
   filename=None,
@@ -173,16 +193,16 @@
       name='STRING', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2567,
-  serialized_end=2596,
+  serialized_start=2614,
+  serialized_end=2643,
 )
 _sym_db.RegisterEnumDescriptor(_TYPE_DATE_BASE)
 
 _TYPE_TIME_BASE = _descriptor.EnumDescriptor(
   name='Base',
   full_name='sarus_data_spec.Type.Time.Base',
   filename=None,
@@ -208,16 +228,16 @@
       name='INT64_US', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2721,
-  serialized_end=2781,
+  serialized_start=2768,
+  serialized_end=2828,
 )
 _sym_db.RegisterEnumDescriptor(_TYPE_TIME_BASE)
 
 _TYPE_ID_BASE = _descriptor.EnumDescriptor(
   name='Base',
   full_name='sarus_data_spec.Type.Id.Base',
   filename=None,
@@ -253,16 +273,16 @@
       name='BYTES', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3203,
-  serialized_end=3275,
+  serialized_start=3250,
+  serialized_end=3322,
 )
 _sym_db.RegisterEnumDescriptor(_TYPE_ID_BASE)
 
 
 _TYPE_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
   full_name='sarus_data_spec.Type.PropertiesEntry',
@@ -419,15 +439,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1246,
-  serialized_end=1407,
+  serialized_end=1454,
 )
 
 _TYPE_ENUM_NAMEVALUE = _descriptor.Descriptor(
   name='NameValue',
   full_name='sarus_data_spec.Type.Enum.NameValue',
   filename=None,
   file=DESCRIPTOR,
@@ -456,16 +476,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1541,
-  serialized_end=1581,
+  serialized_start=1588,
+  serialized_end=1628,
 )
 
 _TYPE_ENUM = _descriptor.Descriptor(
   name='Enum',
   full_name='sarus_data_spec.Type.Enum',
   filename=None,
   file=DESCRIPTOR,
@@ -502,16 +522,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1410,
-  serialized_end=1632,
+  serialized_start=1457,
+  serialized_end=1679,
 )
 
 _TYPE_FLOAT = _descriptor.Descriptor(
   name='Float',
   full_name='sarus_data_spec.Type.Float',
   filename=None,
   file=DESCRIPTOR,
@@ -555,16 +575,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1635,
-  serialized_end=1788,
+  serialized_start=1682,
+  serialized_end=1835,
 )
 
 _TYPE_TEXT = _descriptor.Descriptor(
   name='Text',
   full_name='sarus_data_spec.Type.Text',
   filename=None,
   file=DESCRIPTOR,
@@ -593,16 +613,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1790,
-  serialized_end=1839,
+  serialized_start=1837,
+  serialized_end=1886,
 )
 
 _TYPE_BYTES = _descriptor.Descriptor(
   name='Bytes',
   full_name='sarus_data_spec.Type.Bytes',
   filename=None,
   file=DESCRIPTOR,
@@ -617,16 +637,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1841,
-  serialized_end=1848,
+  serialized_start=1888,
+  serialized_end=1895,
 )
 
 _TYPE_STRUCT_FIELD = _descriptor.Descriptor(
   name='Field',
   full_name='sarus_data_spec.Type.Struct.Field',
   filename=None,
   file=DESCRIPTOR,
@@ -655,16 +675,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1912,
-  serialized_end=1970,
+  serialized_start=1959,
+  serialized_end=2017,
 )
 
 _TYPE_STRUCT = _descriptor.Descriptor(
   name='Struct',
   full_name='sarus_data_spec.Type.Struct',
   filename=None,
   file=DESCRIPTOR,
@@ -686,16 +706,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1850,
-  serialized_end=1970,
+  serialized_start=1897,
+  serialized_end=2017,
 )
 
 _TYPE_UNION_FIELD = _descriptor.Descriptor(
   name='Field',
   full_name='sarus_data_spec.Type.Union.Field',
   filename=None,
   file=DESCRIPTOR,
@@ -724,16 +744,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1912,
-  serialized_end=1970,
+  serialized_start=1959,
+  serialized_end=2017,
 )
 
 _TYPE_UNION = _descriptor.Descriptor(
   name='Union',
   full_name='sarus_data_spec.Type.Union',
   filename=None,
   file=DESCRIPTOR,
@@ -755,16 +775,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1972,
-  serialized_end=2090,
+  serialized_start=2019,
+  serialized_end=2137,
 )
 
 _TYPE_OPTIONAL = _descriptor.Descriptor(
   name='Optional',
   full_name='sarus_data_spec.Type.Optional',
   filename=None,
   file=DESCRIPTOR,
@@ -786,16 +806,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2092,
-  serialized_end=2139,
+  serialized_start=2139,
+  serialized_end=2186,
 )
 
 _TYPE_LIST = _descriptor.Descriptor(
   name='List',
   full_name='sarus_data_spec.Type.List',
   filename=None,
   file=DESCRIPTOR,
@@ -824,16 +844,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2141,
-  serialized_end=2202,
+  serialized_start=2188,
+  serialized_end=2249,
 )
 
 _TYPE_ARRAY = _descriptor.Descriptor(
   name='Array',
   full_name='sarus_data_spec.Type.Array',
   filename=None,
   file=DESCRIPTOR,
@@ -862,16 +882,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2204,
-  serialized_end=2263,
+  serialized_start=2251,
+  serialized_end=2310,
 )
 
 _TYPE_DATETIME = _descriptor.Descriptor(
   name='Datetime',
   full_name='sarus_data_spec.Type.Datetime',
   filename=None,
   file=DESCRIPTOR,
@@ -922,16 +942,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2266,
-  serialized_end=2442,
+  serialized_start=2313,
+  serialized_end=2489,
 )
 
 _TYPE_DATE = _descriptor.Descriptor(
   name='Date',
   full_name='sarus_data_spec.Type.Date',
   filename=None,
   file=DESCRIPTOR,
@@ -982,16 +1002,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2445,
-  serialized_end=2596,
+  serialized_start=2492,
+  serialized_end=2643,
 )
 
 _TYPE_TIME = _descriptor.Descriptor(
   name='Time',
   full_name='sarus_data_spec.Type.Time',
   filename=None,
   file=DESCRIPTOR,
@@ -1042,16 +1062,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2599,
-  serialized_end=2781,
+  serialized_start=2646,
+  serialized_end=2828,
 )
 
 _TYPE_DURATION = _descriptor.Descriptor(
   name='Duration',
   full_name='sarus_data_spec.Type.Duration',
   filename=None,
   file=DESCRIPTOR,
@@ -1094,16 +1114,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2783,
-  serialized_end=2858,
+  serialized_start=2830,
+  serialized_end=2905,
 )
 
 _TYPE_CONSTRAINED = _descriptor.Descriptor(
   name='Constrained',
   full_name='sarus_data_spec.Type.Constrained',
   filename=None,
   file=DESCRIPTOR,
@@ -1132,16 +1152,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2860,
-  serialized_end=2958,
+  serialized_start=2907,
+  serialized_end=3005,
 )
 
 _TYPE_HYPOTHESIS_SCORED = _descriptor.Descriptor(
   name='Scored',
   full_name='sarus_data_spec.Type.Hypothesis.Scored',
   filename=None,
   file=DESCRIPTOR,
@@ -1170,16 +1190,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3031,
-  serialized_end=3091,
+  serialized_start=3078,
+  serialized_end=3138,
 )
 
 _TYPE_HYPOTHESIS = _descriptor.Descriptor(
   name='Hypothesis',
   full_name='sarus_data_spec.Type.Hypothesis',
   filename=None,
   file=DESCRIPTOR,
@@ -1201,16 +1221,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2961,
-  serialized_end=3091,
+  serialized_start=3008,
+  serialized_end=3138,
 )
 
 _TYPE_ID = _descriptor.Descriptor(
   name='Id',
   full_name='sarus_data_spec.Type.Id',
   filename=None,
   file=DESCRIPTOR,
@@ -1247,16 +1267,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3094,
-  serialized_end=3275,
+  serialized_start=3141,
+  serialized_end=3322,
 )
 
 _TYPE = _descriptor.Descriptor(
   name='Type',
   full_name='sarus_data_spec.Type',
   filename=None,
   file=DESCRIPTOR,
@@ -1431,15 +1451,15 @@
     _descriptor.OneofDescriptor(
       name='type', full_name='sarus_data_spec.Type.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
   serialized_start=136,
-  serialized_end=3283,
+  serialized_end=3330,
 )
 
 _TYPE_PROPERTIESENTRY.containing_type = _TYPE
 _TYPE_NULL.containing_type = _TYPE
 _TYPE_UNIT.containing_type = _TYPE
 _TYPE_BOOLEAN.containing_type = _TYPE
 _TYPE_INTEGER.fields_by_name['base'].enum_type = _TYPE_INTEGER_BASE
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,27 @@
             V = typing.NewType('V', builtins.int)
         class _BaseEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Base.V], builtins.type):
             DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
             INT64 = Type.Integer.Base.V(0)
             INT32 = Type.Integer.Base.V(1)
             INT16 = Type.Integer.Base.V(2)
             INT8 = Type.Integer.Base.V(3)
+            UINT64 = Type.Integer.Base.V(4)
+            UINT32 = Type.Integer.Base.V(5)
+            UINT16 = Type.Integer.Base.V(6)
+            UINT8 = Type.Integer.Base.V(7)
 
         INT64 = Type.Integer.Base.V(0)
         INT32 = Type.Integer.Base.V(1)
         INT16 = Type.Integer.Base.V(2)
         INT8 = Type.Integer.Base.V(3)
+        UINT64 = Type.Integer.Base.V(4)
+        UINT32 = Type.Integer.Base.V(5)
+        UINT16 = Type.Integer.Base.V(6)
+        UINT8 = Type.Integer.Base.V(7)
 
         BASE_FIELD_NUMBER: builtins.int
         MIN_FIELD_NUMBER: builtins.int
         MAX_FIELD_NUMBER: builtins.int
         POSSIBLE_VALUES_FIELD_NUMBER: builtins.int
         base: global___Type.Integer.Base.V = ...
         min: builtins.int = ...
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/size.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/status.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from datetime import datetime
 from functools import partial
-from typing import Callable, List, Mapping, Optional, Type, cast
+from typing import Callable, Mapping, Optional, Type, cast
 import logging
 import typing as t
 
 from sarus_data_spec import typing as st
 from sarus_data_spec.base import Base, Referring
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.manager.typing import Manager
@@ -309,38 +309,14 @@
 
     if status.task(task=task) is None:
         return None
 
     return status
 
 
-def last_statuses(
-    dataspec: st.DataSpec, task: t.Optional[str] = None
-) -> List[st.Status]:
-    """Return a list composed by the last status of every
-    DataSpec's manager."""
-    managers = dataspec.storage().type_name(sp.type_name(sp.Manager))
-    statuses = []
-    for manager in managers:
-        stt = last_status(
-            dataspec,
-            cast(
-                Optional[Manager],
-                manager,
-            ),
-        )
-        if stt is not None:
-            if task is not None:
-                if stt.task(task) is not None:
-                    statuses.append(stt)
-            else:
-                statuses.append(stt)
-    return statuses
-
-
 class Stage(Base[sp.Status.Stage]):
     """A simple wrapper type to simplify protobuf usage"""
 
     def accept(self, visitor: st.StageVisitor) -> None:
         dispatch: Callable[[], None] = {
             'pending': visitor.pending,
             'processing': visitor.processing,
@@ -462,23 +438,14 @@
         dataspec,
         task_stages={task: error_stage(properties=properties)},
         properties=None,
         manager=manager,
     )
 
 
-def clear_task(dataspec: st.DataSpec, task: str) -> None:
-    """This methods creates a new status for each manager
-    where the specified task has been cleared"""
-
-    statuses = last_statuses(dataspec)
-    for manager_status in statuses:
-        manager_status.clear_task(task)
-
-
 def update_last(
     status: st.Referring[ProtobufWithUUIDAndDatetime],
     task_stages: Optional[Mapping[str, st.Stage]],
     properties: Optional[Mapping[str, str]],
 ) -> t.Tuple[st.Referring[ProtobufWithUUIDAndDatetime], bool]:
     """Returns whether the update should be done, ie transitions
     are respected and the status that can be updated in case"""
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/type.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -870,14 +870,18 @@
 
 
 class IntegerBase(Enum):
     INT64 = sp.Type.Integer.INT64
     INT32 = sp.Type.Integer.INT32
     INT16 = sp.Type.Integer.INT16
     INT8 = sp.Type.Integer.INT8
+    UINT64 = sp.Type.Integer.UINT64
+    UINT32 = sp.Type.Integer.UINT32
+    UINT16 = sp.Type.Integer.UINT16
+    UINT8 = sp.Type.Integer.UINT8
 
 
 class FloatBase(Enum):
     FLOAT64 = sp.Type.Float.FLOAT64
     FLOAT32 = sp.Type.Float.FLOAT32
     FLOAT16 = sp.Type.Float.FLOAT16
```

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.2.1.dev2/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/setup.cfg` & `sarus_data_spec_public-3.2.1.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.2.1.dev0/setup.py` & `sarus_data_spec_public-3.2.1.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.2.1.dev0')
+    setup(version='3.2.1.dev2')
```

