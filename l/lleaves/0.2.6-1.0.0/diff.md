# Comparing `tmp/lleaves-0.2.6.tar.gz` & `tmp/lleaves-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lleaves/lleaves/dist/tmpvycrhi9q/lleaves-0.2.6.tar", last modified: Sun Jul 10 16:56:14 2022, max compression
+gzip compressed data, was "/home/runner/work/lleaves/lleaves/dist/.tmp-i42ejzto/lleaves-1.0.0.tar", last modified: Wed May 10 10:19:41 2023, max compression
```

## Comparing `lleaves-0.2.6.tar` & `lleaves-1.0.0.tar`

### file list

```diff
@@ -1,97 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/.github/
--rwxr-xr-x   0 runner    (1001) docker     (121)      416 2022-07-10 16:49:36.000000 lleaves-0.2.6/.github/ci.sh
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-07-10 16:49:36.000000 lleaves-0.2.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-07-10 16:49:36.000000 lleaves-0.2.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-07-10 16:49:36.000000 lleaves-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-07-10 16:49:36.000000 lleaves-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-10 16:49:36.000000 lleaves-0.2.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-07-10 16:49:36.000000 lleaves-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-07-10 16:56:14.000000 lleaves-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-07-10 16:49:36.000000 lleaves-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/benchmarks/c_bench/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/c_bench/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/c_bench/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/c_bench/c_bench.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/c_bench/c_bench.h
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/c_bench/gen_binary.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      805 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/c_bench/plot_toplev.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/benchmarks/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/data/gen_npy.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      189 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/data/setup_data.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/train_NYC_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-07-10 16:49:36.000000 lleaves-0.2.6/benchmarks/train_airline_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-07-10 16:49:36.000000 lleaves-0.2.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (121)    29525 2022-07-10 16:49:36.000000 lleaves-0.2.6/docs/assets/pure_categorical.png
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-07-10 16:49:36.000000 lleaves-0.2.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-07-10 16:49:36.000000 lleaves-0.2.6/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-07-10 16:49:36.000000 lleaves-0.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-07-10 16:49:36.000000 lleaves-0.2.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-07-10 16:49:36.000000 lleaves-0.2.6/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves/compiler/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves/compiler/ast/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/ast/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/ast/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/ast/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves/compiler/codegen/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15315 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/codegen/codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/tree_compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/compiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7692 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     7528 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/lleaves.py
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-07-10 16:49:36.000000 lleaves-0.2.6/lleaves/llvm_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-10 16:56:14.000000 lleaves-0.2.6/lleaves.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-10 16:49:36.000000 lleaves-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-10 16:56:14.000000 lleaves-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-07-10 16:49:36.000000 lleaves-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/NYC_taxi/
--rw-r--r--   0 runner    (1001) docker     (121)   324193 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/NYC_taxi/model.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/airline/
--rw-r--r--   0 runner    (1001) docker     (121)   463181 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/airline/model.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (121)   181497 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/boston_housing/model.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/leaf_scan/
--rw-r--r--   0 runner    (1001) docker     (121)     3886 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/leaf_scan/model.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/mixed_categorical/
--rw-r--r--   0 runner    (1001) docker     (121)     4342 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/mixed_categorical/model.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/mtpl2/
--rw-r--r--   0 runner    (1001) docker     (121)  2767972 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/mtpl2/model.txt
--rw-r--r--   0 runner    (1001) docker     (121)   572014 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/mtpl2/model_small.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/multiclass/
--rw-r--r--   0 runner    (1001) docker     (121)    83077 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/multiclass/model.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/pure_categorical/
--rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/pure_categorical/model.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/single_tree/
--rw-r--r--   0 runner    (1001) docker     (121)     4100 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/single_tree/model.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 16:56:14.000000 lleaves-0.2.6/tests/models/tiniest_single_tree/
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/models/tiniest_single_tree/model.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     7888 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_categoricals.py
--rw-r--r--   0 runner    (1001) docker     (121)     3061 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_compile_flags.py
--rw-r--r--   0 runner    (1001) docker     (121)     4010 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_dataprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     5422 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_nans.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-07-10 16:49:36.000000 lleaves-0.2.6/tests/test_tree_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-05-10 10:14:02.000000 lleaves-1.0.0/.github/ci.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 10:14:02.000000 lleaves-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-10 10:14:02.000000 lleaves-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-10 10:14:02.000000 lleaves-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-10 10:14:02.000000 lleaves-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 10:14:02.000000 lleaves-1.0.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 10:14:02.000000 lleaves-1.0.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-10 10:14:02.000000 lleaves-1.0.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 10:14:02.000000 lleaves-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-10 10:19:41.000000 lleaves-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-10 10:14:02.000000 lleaves-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/benchmarks/c_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/c_bench/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/c_bench/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/c_bench/c_bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/c_bench/c_bench.h
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/c_bench/gen_binary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/c_bench/plot_toplev.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/benchmarks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/data/gen_npy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      190 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/data/setup_data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/train_NYC_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 10:14:02.000000 lleaves-1.0.0/benchmarks/train_airline_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 10:14:02.000000 lleaves-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    29525 2023-05-10 10:14:02.000000 lleaves-1.0.0/docs/assets/pure_categorical.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-10 10:14:02.000000 lleaves-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-05-10 10:14:02.000000 lleaves-1.0.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-10 10:14:02.000000 lleaves-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-10 10:14:02.000000 lleaves-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-10 10:14:02.000000 lleaves-1.0.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves/compiler/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/ast/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/ast/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/ast/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves/compiler/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/codegen/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/tree_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/compiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/lleaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-10 10:14:02.000000 lleaves-1.0.0/lleaves/llvm_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 10:19:41.000000 lleaves-1.0.0/lleaves.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 10:14:02.000000 lleaves-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 10:19:41.000000 lleaves-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-10 10:14:02.000000 lleaves-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/NYC_taxi/
+-rw-r--r--   0 runner    (1001) docker     (123)   324193 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/NYC_taxi/model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/airline/
+-rw-r--r--   0 runner    (1001) docker     (123)   463181 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/airline/model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (123)   181497 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/boston_housing/model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/leaf_scan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/leaf_scan/model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/mixed_categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/mixed_categorical/model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/mtpl2/
+-rw-r--r--   0 runner    (1001) docker     (123)  2767972 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/mtpl2/model.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   572014 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/mtpl2/model_small.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/multiclass/
+-rw-r--r--   0 runner    (1001) docker     (123)    83077 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/multiclass/model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/pure_categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/pure_categorical/model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/single_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/single_tree/model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:19:41.000000 lleaves-1.0.0/tests/models/tiniest_single_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/models/tiniest_single_tree/model.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_categoricals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_compile_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_dataprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_nans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-10 10:14:02.000000 lleaves-1.0.0/tests/test_tree_output.py
```

### Comparing `lleaves-0.2.6/.github/workflows/ci.yml` & `lleaves-1.0.0/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 name: CI
 on:
   push:
+    branches: [ master ]
   pull_request:
-    types: [opened, synchronize, reopened]
+  workflow_dispatch:
 
 jobs:
   linux-unittest:
     name: Linux unittest - ${{ matrix.PYTHON_VERSION }}
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
@@ -34,16 +35,16 @@
         with:
           path: ./.hypothesis
           key: hypothesisDB ${{ matrix.PYTHON_VERSION }}
       - name: Run the unittests
         shell: bash -x -l {0}
         run: ./.github/ci.sh ${{ matrix.PYTHON_VERSION }}
       - name: Publish a Python distribution to PyPI
-        if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags') && matrix.PYTHON_VERSION == '3.7'
-        uses: pypa/gh-action-pypi-publish@v1.5.0
+        if: startsWith(github.ref, 'refs/tags') && matrix.PYTHON_VERSION == '3.7'
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
 
   pre-commit-checks:
     name: "Pre-commit checks - Python 3.9"
     runs-on: ubuntu-latest
```

### Comparing `lleaves-0.2.6/.gitignore` & `lleaves-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/.pre-commit-config.yaml` & `lleaves-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/LICENSE` & `lleaves-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/PKG-INFO` & `lleaves-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: lleaves
-Version: 0.2.6
-Summary: LLVM-based compiler for LightGBM models
-Home-page: https://github.com/siboehm/lleaves
-Author: Simon Boehm
-Author-email: simon@siboehm.com
-License: MIT
-Project-URL: Documentation, https://lleaves.readthedocs.io/en/latest/
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # lleaves 🍃
 ![CI](https://github.com/siboehm/lleaves/workflows/CI/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/lleaves/badge/?version=latest)](https://lleaves.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/lleaves)](https://pepy.tech/project/lleaves)
 
 A LLVM-based compiler for LightGBM decision trees.
 
@@ -62,21 +46,33 @@
 |batchsize   | 10,000  | 100,000  | 678,000 |
 |---|---:|---:|---:|
 |LightGBM   | 95.14ms | 992.47ms   | 7034.65ms  |
 |ONNX  Runtime | 38.83ms  | 381.40ms  | 2849.42ms  |
 |Treelite   | 38.15ms | 414.15ms  | 2854.10ms  |
 |``lleaves``  | 5.90ms  | 56.96ms | 388.88ms |
 
-## Advanced usage
-To avoid any Python overhead during prediction you can link directly against the generated binary.
-See `benchmarks/c_bench/` for an example of how to do this.
-The function signature can change between major versions.
+## Advanced Usage
+To avoid expensive recompilation, you can call `lleaves.Model.compile()` and pass a `cache=<filepath>` argument.
+This will store an ELF (Linux) / Mach-O (macOS) file at the given path when the method is first called.
+Subsequent calls of `compile(cache=<same filepath>)` will skip compilation and load the stored binary file instead.
+For more info, see [docs](https://lleaves.readthedocs.io/en/latest/).
+
+To eliminate any Python overhead during inference you can link against this generated binary.
+For an example of how to do this see `benchmarks/c_bench/`.
+The function signature might change between major versions.
 
 ## Development
+High-level explanation of the inner workings of the lleaves compiler: [link](https://siboehm.com/articles/21/lleaves)
 ```bash
 conda env create
 conda activate lleaves
 pip install -e .
 pre-commit install
 ./benchmarks/data/setup_data.sh
 pytest
 ```
+
+Release:
+```
+git tag -a 1.0.0
+git push origin 1.0.0
+```
```

### Comparing `lleaves-0.2.6/README.md` & `lleaves-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: lleaves
+Version: 1.0.0
+Summary: LLVM-based compiler for LightGBM models
+Home-page: https://github.com/siboehm/lleaves
+Author: Simon Boehm
+Author-email: simon@siboehm.com
+License: MIT
+Project-URL: Documentation, https://lleaves.readthedocs.io/en/latest/
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # lleaves 🍃
 ![CI](https://github.com/siboehm/lleaves/workflows/CI/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/lleaves/badge/?version=latest)](https://lleaves.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/lleaves)](https://pepy.tech/project/lleaves)
 
 A LLVM-based compiler for LightGBM decision trees.
 
@@ -46,21 +62,33 @@
 |batchsize   | 10,000  | 100,000  | 678,000 |
 |---|---:|---:|---:|
 |LightGBM   | 95.14ms | 992.47ms   | 7034.65ms  |
 |ONNX  Runtime | 38.83ms  | 381.40ms  | 2849.42ms  |
 |Treelite   | 38.15ms | 414.15ms  | 2854.10ms  |
 |``lleaves``  | 5.90ms  | 56.96ms | 388.88ms |
 
-## Advanced usage
-To avoid any Python overhead during prediction you can link directly against the generated binary.
-See `benchmarks/c_bench/` for an example of how to do this.
-The function signature can change between major versions.
+## Advanced Usage
+To avoid expensive recompilation, you can call `lleaves.Model.compile()` and pass a `cache=<filepath>` argument.
+This will store an ELF (Linux) / Mach-O (macOS) file at the given path when the method is first called.
+Subsequent calls of `compile(cache=<same filepath>)` will skip compilation and load the stored binary file instead.
+For more info, see [docs](https://lleaves.readthedocs.io/en/latest/).
+
+To eliminate any Python overhead during inference you can link against this generated binary.
+For an example of how to do this see `benchmarks/c_bench/`.
+The function signature might change between major versions.
 
 ## Development
+High-level explanation of the inner workings of the lleaves compiler: [link](https://siboehm.com/articles/21/lleaves)
 ```bash
 conda env create
 conda activate lleaves
 pip install -e .
 pre-commit install
 ./benchmarks/data/setup_data.sh
 pytest
 ```
+
+Release:
+```
+git tag -a 1.0.0
+git push origin 1.0.0
+```
```

### Comparing `lleaves-0.2.6/benchmarks/benchmark.py` & `lleaves-1.0.0/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/benchmarks/c_bench/CMakeLists.txt` & `lleaves-1.0.0/benchmarks/c_bench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/benchmarks/c_bench/README.md` & `lleaves-1.0.0/benchmarks/c_bench/README.md`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/benchmarks/c_bench/c_bench.cpp` & `lleaves-1.0.0/benchmarks/c_bench/c_bench.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #include "c_bench.h"
 #include <cnpy.h>
 #include <benchmark/benchmark.h>
 #include <algorithm>
 #include <cstdlib>
 #include <iostream>
 
-static void bm_lleaves(benchmark::State& state) {
+static void bm_lleaves(benchmark::State &state)
+{
   char *model_name = std::getenv("LLEAVES_BENCHMARK_MODEL");
 
   std::ostringstream model_stream;
   model_stream << "../../data/" << model_name << ".npy";
   std::string model_file = model_stream.str();
   cnpy::NpyArray arr = cnpy::npy_load(model_file);
 
   auto *loaded_data = arr.data<double>();
   ulong n_preds = arr.shape[0];
   auto *out = (double *)(malloc(n_preds * sizeof(double)));
 
-  for (auto _ : state){
-      // predict over the whole input array
-      forest_root(loaded_data, out, (int)0, (int)n_preds);
+  for (auto _ : state)
+  {
+    // predict over the whole input array
+    forest_root(loaded_data, out, (int)0, (int)n_preds);
   }
 }
 
-BENCHMARK(bm_lleaves);
+BENCHMARK(bm_lleaves)->Unit(benchmark::kMillisecond);
 BENCHMARK_MAIN();
```

### Comparing `lleaves-0.2.6/benchmarks/c_bench/gen_binary.py` & `lleaves-1.0.0/benchmarks/c_bench/gen_binary.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/benchmarks/c_bench/plot_toplev.sh` & `lleaves-1.0.0/benchmarks/c_bench/plot_toplev.sh`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/benchmarks/data/gen_npy.py` & `lleaves-1.0.0/benchmarks/data/gen_npy.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/benchmarks/train_NYC_model.py` & `lleaves-1.0.0/benchmarks/train_NYC_model.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/benchmarks/train_airline_model.py` & `lleaves-1.0.0/benchmarks/train_airline_model.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/docs/Makefile` & `lleaves-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/docs/assets/pure_categorical.png` & `lleaves-1.0.0/docs/assets/pure_categorical.png`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/docs/conf.py` & `lleaves-1.0.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 sys.path.insert(0, os.path.abspath("../"))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "lleaves"
-copyright = "2021, Simon Boehm"
+copyright = "2023, Simon Boehm"
 author = "Simon Boehm"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `lleaves-0.2.6/docs/development.rst` & `lleaves-1.0.0/docs/development.rst`

 * *Files 21% similar despite different names*

```diff
@@ -114,7 +114,64 @@
 To look at the IR generated by ``lleaves`` there are two useful environment variables:
 
 - Set ``LLEAVES_PRINT_UNOPTIMIZED_IR=1`` to look at the LLVM IR generated by ``lleaves`` before any LLVM compiler
   optimization passes are run.
 - Set ``LLEAVES_PRINT_OPTIMIZED_IR=1`` to look at the final LLVM IR after the LLVM compiler optimization passes.
 - Set ``LLEAVES_PRINT_ASM=1`` to look at the assembly code produced by the compiler.
 
+Interfacing with a Compiled Model in C++
+-------------------
+
+To interface with the compiled model in C++, you need the following steps:
+
+1. Generating Cache Files using Python.
+
+If you already have a trained model file named ``lgbmModel.txt``, the command to read and compile it may look like this.::
+
+    llvm_model = lleaves.Model(model_file="lgbmModel.txt")
+    llvm_model.compile(cache='./lleaves.o')
+    ...
+
+2. Modifying and Moving Relevant Files
+
+- The modifications were made primarily based on this section of code: ``https://github.com/siboehm/lleaves/tree/master/benchmarks/c_bench``
+- Move ``lleaves.o`` to the current directory
+- Modify the ``c_bench.cpp``, like so::
+
+    #include "c_bench.h"
+    #include <vector>
+    #include <iostream>
+    int main()
+    {
+      std::vector<double> data = {8.81351540e+00, -2.74901880e-01, -4.78453119e-02, 2.25956985e+01,
+                                  -2.75495538e-01, -9.12007856e-02, -4.78453119e-02, 1.88485949e+00,
+                                  1.88485949e+00, 1.64226175e-03, 1.64226175e-03};
+
+      double result;
+      forest_root(data.data(), &result, 0, 1);
+      std::cout << "Result: " << result << std::endl;
+      return 0;
+    }
+    ...
+- Due to C++ name mangling, it's important to retain the ``extern C`` function declaration for ``forest_root`` in the header. Else the linker will fail.
+- Modify the ``CMakeLists``, like so::
+
+    cmake_minimum_required(VERSION 3.19)
+    project(c_bench)
+    set(CMAKE_CXX_STANDARD 11)
+    add_executable(c_bench c_bench.cpp)
+    add_dependencies(c_bench run)
+    target_link_libraries(c_bench ${CMAKE_CURRENT_SOURCE_DIR}/lleaves.o)
+    ...
+3. Build the code
+
+- If you are using CMake, you can run the following commands to build and run the program::
+
+    cmake .. && make
+    ./c_bench
+    ...
+
+- If you are using g++, you can run the following commands to build and run the program::
+
+    g++ c_bench.cpp lleaves.o -o c_bench
+    ./c_bench
+    ...
```

### Comparing `lleaves-0.2.6/docs/make.bat` & `lleaves-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves/compiler/ast/nodes.py` & `lleaves-1.0.0/lleaves/compiler/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves/compiler/ast/parser.py` & `lleaves-1.0.0/lleaves/compiler/ast/parser.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves/compiler/ast/scanner.py` & `lleaves-1.0.0/lleaves/compiler/ast/scanner.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves/compiler/codegen/codegen.py` & `lleaves-1.0.0/lleaves/compiler/codegen/codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 LONG = ir.IntType(bits=64)
 ZERO_V = ir.Constant(BOOL, 0)
 FLOAT_POINTER = ir.PointerType(FLOAT)
 DOUBLE_PTR = ir.PointerType(DOUBLE)
 
 
 def iconst(value):
+    assert -(2**31) <= value <= 2**31 - 1
     return ir.Constant(INT, value)
 
 
 def lconst(value):
+    assert -(2**63) <= value <= 2**63 - 1
     return ir.Constant(LONG, value)
 
 
 def fconst(value):
     return ir.Constant(FLOAT, value)
 
 
@@ -162,15 +164,21 @@
     if left_block:
         gen_node(func, left_block, node.left)
     if right_block:
         gen_node(func, right_block, node.right)
 
 
 def _populate_instruction_block(
-    forest, root_func, tree_funcs, setup_block, next_block, eval_obj_func
+    instr_block_idx,
+    forest,
+    root_func,
+    tree_funcs,
+    setup_block,
+    next_block,
+    eval_obj_func,
 ):
     """Generates an instruction_block: loops over all input data and evaluates its chunk of tree_funcs."""
     data_arr, out_arr, start_index, end_index = root_func.args
 
     # -- SETUP BLOCK
     builder = ir.IRBuilder(setup_block)
     start_index = builder.zext(start_index, LONG)
@@ -198,32 +206,38 @@
     iter_mul_nargs = builder.mul(loop_iter_reg, n_args)
     idx = (builder.add(iter_mul_nargs, lconst(i)) for i in range(forest.n_args))
     raw_ptrs = [builder.gep(root_func.args[0], (c,)) for c in idx]
     # cast the categorical inputs to integer
     for feature, ptr in zip(forest.features, raw_ptrs):
         el = builder.load(ptr)
         if feature.is_categorical:
-            args.append(builder.fptosi(el, INT_CAT))
+            # first, check if the value is NaN
+            is_nan = builder.fcmp_ordered("uno", el, dconst(0.0))
+            # if it is, return smallest possible int (will always go right), else cast to int
+            el = builder.select(is_nan, iconst(-(2**31)), builder.fptosi(el, INT_CAT))
+            args.append(el)
         else:
             args.append(el)
     # iterate over each tree, sum up results
     results = [dconst(0.0) for _ in range(forest.n_classes)]
     for func in tree_funcs:
         tree_res = builder.call(func.llvm_function, args)
         results[func.class_id] = builder.fadd(tree_res, results[func.class_id])
     res_idx = builder.mul(lconst(forest.n_classes), loop_iter_reg)
     results_ptr = [
         builder.gep(out_arr, (builder.add(res_idx, lconst(class_idx)),))
         for class_idx in range(forest.n_classes)
     ]
 
-    results = [
-        builder.fadd(result, builder.load(result_ptr))
-        for result, result_ptr in zip(results, results_ptr)
-    ]
+    if instr_block_idx > 0:
+        results = [
+            builder.fadd(result, builder.load(result_ptr))
+            for result, result_ptr in zip(results, results_ptr)
+        ]
+
     if eval_obj_func:
         results = _populate_objective_func_block(
             builder,
             results,
             forest.objective_func,
             forest.objective_func_config,
             forest.raw_score,
@@ -250,14 +264,15 @@
     ]
     term_block = root_func.append_basic_block("term")
     ir.IRBuilder(term_block).ret_void()
     for i, (setup_block, tree_func_chunk) in enumerate(instr_blocks):
         next_block = instr_blocks[i + 1][0] if i < len(instr_blocks) - 1 else term_block
         eval_objective_func = next_block == term_block
         _populate_instruction_block(
+            i,
             forest,
             root_func,
             tree_func_chunk,
             setup_block,
             next_block,
             eval_objective_func,
         )
@@ -335,16 +350,16 @@
 
 def _populate_categorical_node_block(
     func, builder, bitset_comp_builder, node, bitset_comp_block, right_block
 ):
     """Populate block with IR for categorical node"""
     val = func.args[node.split_feature]
 
-    # For categoricals, processing NaNs happens through casting them via fptosi in the Forest root
-    # NaNs become negative max_val, which never exists in the Bitset, so they always go right
+    # For categoricals, processing NaNs happens in the Forest root, by explicitly checking for them
+    # NaNs are converted to negative max_val, which never exists in the Bitset, so they always go right
 
     # Find in bitset
     # First, check value > max categorical
     comp = builder.icmp_unsigned(
         "<",
         val,
         iconst(32 * len(node.cat_threshold)),
```

### Comparing `lleaves-0.2.6/lleaves/compiler/tree_compiler.py` & `lleaves-1.0.0/lleaves/compiler/tree_compiler.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves/compiler/utils.py` & `lleaves-1.0.0/lleaves/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves/data_processing.py` & `lleaves-1.0.0/lleaves/data_processing.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves/lleaves.py` & `lleaves-1.0.0/lleaves/lleaves.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves/llvm_binding.py` & `lleaves-1.0.0/lleaves/llvm_binding.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/lleaves.egg-info/PKG-INFO` & `lleaves-1.0.0/lleaves.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lleaves
-Version: 0.2.6
+Version: 1.0.0
 Summary: LLVM-based compiler for LightGBM models
 Home-page: https://github.com/siboehm/lleaves
 Author: Simon Boehm
 Author-email: simon@siboehm.com
 License: MIT
 Project-URL: Documentation, https://lleaves.readthedocs.io/en/latest/
 Classifier: License :: OSI Approved :: MIT License
@@ -62,21 +62,33 @@
 |batchsize   | 10,000  | 100,000  | 678,000 |
 |---|---:|---:|---:|
 |LightGBM   | 95.14ms | 992.47ms   | 7034.65ms  |
 |ONNX  Runtime | 38.83ms  | 381.40ms  | 2849.42ms  |
 |Treelite   | 38.15ms | 414.15ms  | 2854.10ms  |
 |``lleaves``  | 5.90ms  | 56.96ms | 388.88ms |
 
-## Advanced usage
-To avoid any Python overhead during prediction you can link directly against the generated binary.
-See `benchmarks/c_bench/` for an example of how to do this.
-The function signature can change between major versions.
+## Advanced Usage
+To avoid expensive recompilation, you can call `lleaves.Model.compile()` and pass a `cache=<filepath>` argument.
+This will store an ELF (Linux) / Mach-O (macOS) file at the given path when the method is first called.
+Subsequent calls of `compile(cache=<same filepath>)` will skip compilation and load the stored binary file instead.
+For more info, see [docs](https://lleaves.readthedocs.io/en/latest/).
+
+To eliminate any Python overhead during inference you can link against this generated binary.
+For an example of how to do this see `benchmarks/c_bench/`.
+The function signature might change between major versions.
 
 ## Development
+High-level explanation of the inner workings of the lleaves compiler: [link](https://siboehm.com/articles/21/lleaves)
 ```bash
 conda env create
 conda activate lleaves
 pip install -e .
 pre-commit install
 ./benchmarks/data/setup_data.sh
 pytest
 ```
+
+Release:
+```
+git tag -a 1.0.0
+git push origin 1.0.0
+```
```

### Comparing `lleaves-0.2.6/lleaves.egg-info/SOURCES.txt` & `lleaves-1.0.0/lleaves.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
+CITATION.cff
 LICENSE
 README.md
 environment.yml
 pyproject.toml
 setup.py
 .github/ci.sh
 .github/dependabot.yml
 .github/workflows/ci.yml
+.vscode/settings.json
 benchmarks/__init__.py
 benchmarks/benchmark.py
 benchmarks/train_NYC_model.py
 benchmarks/train_airline_model.py
 benchmarks/c_bench/CMakeLists.txt
 benchmarks/c_bench/README.md
 benchmarks/c_bench/c_bench.cpp
```

### Comparing `lleaves-0.2.6/setup.py` & `lleaves-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/conftest.py` & `lleaves-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/NYC_taxi/model.txt` & `lleaves-1.0.0/tests/models/NYC_taxi/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/airline/model.txt` & `lleaves-1.0.0/tests/models/airline/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/boston_housing/model.txt` & `lleaves-1.0.0/tests/models/boston_housing/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/leaf_scan/model.txt` & `lleaves-1.0.0/tests/models/leaf_scan/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/mixed_categorical/model.txt` & `lleaves-1.0.0/tests/models/mixed_categorical/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/mtpl2/model.txt` & `lleaves-1.0.0/tests/models/mtpl2/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/mtpl2/model_small.txt` & `lleaves-1.0.0/tests/models/mtpl2/model_small.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/multiclass/model.txt` & `lleaves-1.0.0/tests/models/multiclass/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/pure_categorical/model.txt` & `lleaves-1.0.0/tests/models/pure_categorical/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/single_tree/model.txt` & `lleaves-1.0.0/tests/models/single_tree/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/models/tiniest_single_tree/model.txt` & `lleaves-1.0.0/tests/models/tiniest_single_tree/model.txt`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_benchmark.py` & `lleaves-1.0.0/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_categoricals.py` & `lleaves-1.0.0/tests/test_categoricals.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_compile_flags.py` & `lleaves-1.0.0/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_dataprocessing.py` & `lleaves-1.0.0/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_interface.py` & `lleaves-1.0.0/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_nans.py` & `lleaves-1.0.0/tests/test_nans.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_objective_functions.py` & `lleaves-1.0.0/tests/test_objective_functions.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_parallel.py` & `lleaves-1.0.0/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_parsing.py` & `lleaves-1.0.0/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `lleaves-0.2.6/tests/test_tree_output.py` & `lleaves-1.0.0/tests/test_tree_output.py`

 * *Files identical despite different names*

