# Comparing `tmp/sec-certs-0.1.3.tar.gz` & `tmp/sec-certs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sec-certs-0.1.3.tar", last modified: Tue Jan 10 14:55:15 2023, max compression
+gzip compressed data, was "sec-certs-0.1.4.tar", last modified: Wed May 10 12:00:38 2023, max compression
```

## Comparing `sec-certs-0.1.3.tar` & `sec-certs-0.1.4.tar`

### file list

```diff
@@ -1,236 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.374113 sec-certs-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.342113 sec-certs-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-10 14:55:03.000000 sec-certs-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-01-10 14:55:03.000000 sec-certs-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-01-10 14:55:03.000000 sec-certs-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-01-10 14:55:03.000000 sec-certs-0.1.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-10 14:55:03.000000 sec-certs-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-01-10 14:55:15.374113 sec-certs-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-01-10 14:55:03.000000 sec-certs-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-10 14:55:03.000000 sec-certs-0.1.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/data/cert_id_eval/
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/cert_id_eval/duplicate_ids.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/cert_id_eval/missing_ids.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/cert_id_eval/random.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/cert_id_eval/random_references.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/cert_id_eval/truth.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.350113 sec-certs-0.1.3/data/cpe_eval/
--rw-r--r--   0 runner    (1001) docker     (123)   176434 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/cpe_eval/manual_cpe_labels.json
--rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/cpe_eval/random.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/label_studio_interface.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.350113 sec-certs-0.1.3/data/old_manual_cpe_labels/
--rw-r--r--   0 runner    (1001) docker     (123)  1552011 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/old_manual_cpe_labels/cc.json
--rw-r--r--   0 runner    (1001) docker     (123)  1467792 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/old_manual_cpe_labels/fips.json
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.350113 sec-certs-0.1.3/data/sar_correlations/
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/sar_correlations/all_certs_sar_cve_corr.csv
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/sar_correlations/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.342113 sec-certs-0.1.3/data/validation_test_split/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.354113 sec-certs-0.1.3/data/validation_test_split/cc/
--rw-r--r--   0 runner    (1001) docker     (123)    55394 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/validation_test_split/cc/test.json
--rw-r--r--   0 runner    (1001) docker     (123)    55394 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/validation_test_split/cc/validation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.354113 sec-certs-0.1.3/data/validation_test_split/fips/
--rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/validation_test_split/fips/test.json
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-01-10 14:55:03.000000 sec-certs-0.1.3/data/validation_test_split/fips/validation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.354113 sec-certs-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.354113 sec-certs-0.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    41751 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/_static/logo_badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/_static/logo_badge.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.354113 sec-certs-0.1.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/api/dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/api/model.md
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/api/sample.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/code_of_conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-10 14:55:03.000000 sec-certs-0.1.3/docs/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.354113 sec-certs-0.1.3/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.354113 sec-certs-0.1.3/notebooks/cc/
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/cc/cert_id_eval.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/cc/cpe_eval.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    44390 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/cc/references.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/cc/temporal_trends.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/cc/vulnerabilities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.358113 sec-certs-0.1.3/notebooks/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/examples/cc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/examples/fips.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/examples/fips_iut.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/examples/fips_mip.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/examples/model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   104006 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/final_run.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.358113 sec-certs-0.1.3/notebooks/fips/
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/fips/in_process.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/fips/references.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/fips/temporal_trends.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   132824 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/fips/vulnerabilities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/latex_plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-01-10 14:55:03.000000 sec-certs-0.1.3/notebooks/ocr.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-01-10 14:55:03.000000 sec-certs-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.358113 sec-certs-0.1.3/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-01-10 14:55:03.000000 sec-certs-0.1.3/requirements/compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-01-10 14:55:03.000000 sec-certs-0.1.3/requirements/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-01-10 14:55:03.000000 sec-certs-0.1.3/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-01-10 14:55:03.000000 sec-certs-0.1.3/requirements/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-10 14:55:03.000000 sec-certs-0.1.3/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 14:55:15.374113 sec-certs-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.342113 sec-certs-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.358113 sec-certs-0.1.3/src/sec_certs/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-10 14:55:15.000000 sec-certs-0.1.3/src/sec_certs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/cert_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.358113 sec-certs-0.1.3/src/sec_certs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/config/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/config/settings-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/config/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.362113 sec-certs-0.1.3/src/sec_certs/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68659 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/cpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/cve.py
--rw-r--r--   0 runner    (1001) docker     (123)    23134 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/fips.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/fips_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/fips_iut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/fips_mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/json_path_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/dataset/protection_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.362113 sec-certs-0.1.3/src/sec_certs/model/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/model/cpe_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/model/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/model/reference_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/model/sar_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/model/transitive_vulnerability_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27743 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.362113 sec-certs-0.1.3/src/sec_certs/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41468 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/cc_certificate_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/cc_maintenance_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/cpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/cve.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/fips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/fips_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/fips_iut.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/fips_mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/protection_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/sample/sar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.362113 sec-certs-0.1.3/src/sec_certs/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/serialization/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/serialization/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.366113 sec-certs-0.1.3/src/sec_certs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39050 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21953 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/parallel_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/sanitization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-10 14:55:03.000000 sec-certs-0.1.3/src/sec_certs/utils/tqdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.358113 sec-certs-0.1.3/src/sec_certs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-01-10 14:55:15.000000 sec-certs-0.1.3/src/sec_certs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-01-10 14:55:15.000000 sec-certs-0.1.3/src/sec_certs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 14:55:15.000000 sec-certs-0.1.3/src/sec_certs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-10 14:55:15.000000 sec-certs-0.1.3/src/sec_certs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-10 14:55:15.000000 sec-certs-0.1.3/src/sec_certs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-10 14:55:15.000000 sec-certs-0.1.3/src/sec_certs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.366113 sec-certs-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.366113 sec-certs-0.1.3/tests/cc/
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/cc/test_cc_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/cc/test_cc_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/cc/test_cc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/cc/test_cc_maintenance_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/cc/test_cc_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/cc/test_cc_schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.366113 sec-certs-0.1.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/tests/data/cc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.366113 sec-certs-0.1.3/tests/data/cc/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.366113 sec-certs-0.1.3/tests/data/cc/analysis/auxillary_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/auxillary_datasets/cpe_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/auxillary_datasets/cve_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/cc_full_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/tests/data/cc/analysis/certs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/tests/data/cc/analysis/certs/reports/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.366113 sec-certs-0.1.3/tests/data/cc/analysis/certs/reports/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)  1174271 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/cc/analysis/certs/reports/txt/
--rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/tests/data/cc/analysis/certs/targets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/cc/analysis/certs/targets/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)   615034 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/cc/analysis/certs/targets/txt/
--rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt
--rw-r--r--   0 runner    (1001) docker     (123)    53839 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/reference_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)   103359 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/transitive_vulnerability_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/analysis/vulnerable_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/cc/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/certificate/fictional_cert.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/cc/dataset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/tests/data/cc/dataset/auxillary_datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/cc/dataset/auxillary_datasets/maintenances/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/dataset/auxillary_datasets/maintenances/maintenance_updates.json
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/dataset/cc_products_active.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31505 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/dataset/cc_products_active.html
--rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt
--rw-r--r--   0 runner    (1001) docker     (123)    72568 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/cc/dataset/toy_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.346113 sec-certs-0.1.3/tests/data/fips/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/fips/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/certificate/fictional_cert.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/fips/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/dataset/alg_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)    45964 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/dataset/fips_modules_active.html
--rw-r--r--   0 runner    (1001) docker     (123)    54952 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/dataset/fips_modules_historical.html
--rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/dataset/fips_modules_revoked.html
--rw-r--r--   0 runner    (1001) docker     (123)    60283 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt
--rw-r--r--   0 runner    (1001) docker     (123)    75714 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/dataset/toy_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.370113 sec-certs-0.1.3/tests/data/fips/iut/
--rw-r--r--   0 runner    (1001) docker     (123)    72808 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html
--rw-r--r--   0 runner    (1001) docker     (123)    81803 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.374113 sec-certs-0.1.3/tests/data/fips/mip/
--rw-r--r--   0 runner    (1001) docker     (123)   104771 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html
--rw-r--r--   0 runner    (1001) docker     (123)    85900 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html
--rw-r--r--   0 runner    (1001) docker     (123)   150298 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/data/settings_tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:55:15.374113 sec-certs-0.1.3/tests/fips/
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/fips/test_fips_algorithm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/fips/test_fips_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/fips/test_fips_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/fips/test_fips_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/fips/test_fips_iut.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/fips/test_fips_mip.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/test_cpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-01-10 14:55:03.000000 sec-certs-0.1.3/tests/test_cve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.684648 sec-certs-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.640648 sec-certs-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-10 12:00:28.000000 sec-certs-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-10 12:00:28.000000 sec-certs-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-10 12:00:28.000000 sec-certs-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-10 12:00:28.000000 sec-certs-0.1.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-10 12:00:28.000000 sec-certs-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-10 12:00:38.684648 sec-certs-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-10 12:00:28.000000 sec-certs-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-10 12:00:28.000000 sec-certs-0.1.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/data/cert_id_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/duplicate_ids.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/missing_ids.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/random.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/random_references.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cert_id_eval/truth.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.648648 sec-certs-0.1.4/data/cpe_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)   176434 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cpe_eval/manual_cpe_labels.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/cpe_eval/random.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.652648 sec-certs-0.1.4/data/information_retrieval_split/
+-rw-r--r--   0 runner    (1001) docker     (123)   117213 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    85352 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/sampled_images.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72860 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/information_retrieval_split/valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/label_studio_interface.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.652648 sec-certs-0.1.4/data/old_manual_cpe_labels/
+-rw-r--r--   0 runner    (1001) docker     (123)  1552011 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/old_manual_cpe_labels/cc.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1467792 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/old_manual_cpe_labels/fips.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/data/reference_annotations_split/
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/reference_annotations_split/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/reference_annotations_split/train.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/reference_annotations_split/valid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/data/sar_correlations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/sar_correlations/all_certs_sar_cve_corr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/sar_correlations/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/data/validation_test_split/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/data/validation_test_split/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)    55394 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/validation_test_split/cc/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55394 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/validation_test_split/cc/validation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/data/validation_test_split/fips/
+-rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/validation_test_split/fips/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-10 12:00:28.000000 sec-certs-0.1.4/data/validation_test_split/fips/validation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.656648 sec-certs-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    41751 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logo_badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logo_badge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   363422 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/_static/logolink_OP_VVV_hor_barva_eng.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/api/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/api/model.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/api/sample.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/code_of_conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-10 12:00:28.000000 sec-certs-0.1.4/docs/user_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/notebooks/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/cert_id_eval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/cpe_eval.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/notebooks/cc/reference_annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/reference_annotations/train_validation_test_split.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42619 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/references.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/temporal_trends.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/cc/vulnerabilities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.660648 sec-certs-0.1.4/notebooks/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/cc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   337372 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/est_solution.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/fips.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/fips_iut.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/fips_mip.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/notebooks/examples/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    29981 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/img/boxplot_validity.png
+-rw-r--r--   0 runner    (1001) docker     (123)   134946 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/img/cves_n_days_after_certification.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/examples/model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   104006 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/final_run.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/notebooks/fips/
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/fips/in_process.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/fips/references.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/fips/temporal_trends.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   132824 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/fips/vulnerabilities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/latex_plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-10 12:00:28.000000 sec-certs-0.1.4/notebooks/ocr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-10 12:00:28.000000 sec-certs-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-05-10 12:00:28.000000 sec-certs-0.1.4/requirements/compile.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-05-10 12:00:28.000000 sec-certs-0.1.4/requirements/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-10 12:00:28.000000 sec-certs-0.1.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-10 12:00:28.000000 sec-certs-0.1.4/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 12:00:28.000000 sec-certs-0.1.4/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:00:38.684648 sec-certs-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/src/sec_certs/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/cert_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.668648 sec-certs-0.1.4/src/sec_certs/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39043 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/cc_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/cpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/cve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25690 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/fips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/fips_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/fips_iut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/fips_mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/json_path_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/dataset/protection_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.668648 sec-certs-0.1.4/src/sec_certs/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/cc_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/cpe_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/fips_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/reference_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/sar_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/model/transitive_vulnerability_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27743 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.672649 sec-certs-0.1.4/src/sec_certs/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42917 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cc_certificate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cc_maintenance_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65455 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cc_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/cve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/fips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/fips_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/fips_iut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/fips_mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/protection_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/sample/sar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.672649 sec-certs-0.1.4/src/sec_certs/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/serialization/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/serialization/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.672649 sec-certs-0.1.4/src/sec_certs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38410 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/nvd_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/parallel_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/sanitization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 12:00:28.000000 sec-certs-0.1.4/src/sec_certs/utils/tqdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.664648 sec-certs-0.1.4/src/sec_certs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 12:00:38.000000 sec-certs-0.1.4/src/sec_certs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.672649 sec-certs-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_maintenance_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/cc/test_cc_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/cc_full_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/cc/analysis/certs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)  1174271 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.676648 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)   615034 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    53839 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/reference_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)   103359 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/transitive_vulnerability_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/analysis/vulnerable_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/cc/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/certificate/fictional_cert.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/cc/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/cc/dataset/auxiliary_datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/cc/dataset/auxiliary_datasets/maintenances/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/auxiliary_datasets/maintenances/maintenance_updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/cc_products_active.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    31505 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/cc_products_active.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    72568 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/cc/dataset/toy_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/cpe_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    88427 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/cpe_match_feed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31329 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/cve_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/common/settings_tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.644648 sec-certs-0.1.4/tests/data/fips/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/fips/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/certificate/fictional_cert.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.680648 sec-certs-0.1.4/tests/data/fips/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/alg_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45964 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_active.html
+-rw-r--r--   0 runner    (1001) docker     (123)    54952 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_historical.html
+-rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_revoked.html
+-rw-r--r--   0 runner    (1001) docker     (123)    60283 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    75670 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/dataset/toy_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.684648 sec-certs-0.1.4/tests/data/fips/iut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/iut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72808 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html
+-rw-r--r--   0 runner    (1001) docker     (123)    81803 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.684648 sec-certs-0.1.4/tests/data/fips/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104771 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html
+-rw-r--r--   0 runner    (1001) docker     (123)    85900 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html
+-rw-r--r--   0 runner    (1001) docker     (123)   150298 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:00:38.684648 sec-certs-0.1.4/tests/fips/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_algorithm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_iut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/fips/test_fips_mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_cpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_cve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_cve_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-10 12:00:28.000000 sec-certs-0.1.4/tests/test_nvd_dataset_builder.py
```

### Comparing `sec-certs-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `sec-certs-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `sec-certs-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/.github/workflows/docs.yml` & `sec-certs-0.1.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/.github/workflows/release.yml` & `sec-certs-0.1.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/.github/workflows/tests.yml` & `sec-certs-0.1.4/.github/workflows/tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,18 @@
       - name: Install Poppler
         run: sudo apt-get install -y build-essential libpoppler-cpp-dev pkg-config python3-dev
       - uses: actions/checkout@v3
       - name: Setup python
         uses: actions/setup-python@v4
         with:
           python-version: "3.8"
+          cache: "pip"
+          cache-dependency-path: |
+            requirements/requirements.txt
+            requirements/test_requirements.txt
       - name: Install python dependencies
         run: |
           pip install -r requirements/requirements.txt
           pip install -r requirements/test_requirements.txt
       - name: Install sec-certs
         run: |
           pip install -e .
```

### Comparing `sec-certs-0.1.3/.gitignore` & `sec-certs-0.1.4/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -112,16 +112,19 @@
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
+# ruff
+.ruff_cache
+
 # log
 cert_processing_log.txt
 ./cc_processing_log.txt
 
 # Experiment results produced by notebooks
 notebooks/cc/results/
 
 # Default directory for dataset
-/dataset
+/dataset
```

### Comparing `sec-certs-0.1.3/CODE_OF_CONDUCT.md` & `sec-certs-0.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/CONTRIBUTING.md` & `sec-certs-0.1.4/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,44 +29,42 @@
 - `setuptools-scm` will automatically, upon editable/real install of a package, infer its version and write it to `sec_certs/_version.py`. This file is not indexed as well. See more at [setuptools-scm GitHub](https://github.com/pypa/setuptools_scm)
 - On publishing a release, the tool is automatically published to [PyPi](https://pypi.org/project/sec-certs/) and [DockerHub](https://hub.docker.com/repository/docker/seccerts/sec-certs).
 
 Note on single-sourcing the package version: More can be read [here](https://packaging.python.org/en/latest/guides/single-sourcing-package-version/). The downside of our approach is that `.git` folder and editable/real install is needed to infer the version of the package. Releases can be infered without installing the project.
 
 ### Currently, the release process is as follows
 
-1. Create a release from GitHub UI. Include release notes, add proper version tag and publish the release (or create it from scratch with new tag).
-2. This will automatically update PyPi and DockerHub packages.
+1. Update dependencies with `pre-commit autoupdate`, pin new versions of linters into `pyproject.toml` and run `cd requirements && ./compile.sh`.
+2. Create a release from GitHub UI. Include release notes, add proper version tag and publish the release (or create it from scratch with new tag).
+3. This will automatically update PyPi and DockerHub packages.
 
 
 ## Quality assurance
 
 All commits shall pass the lint pipeline of the following tools:
 
 - Mypy (see [pyproject.toml](https://github.com/crocs-muni/sec-certs/blob/main/pyproject.toml) for settings)
 - Black (see [pyproject.toml](https://github.com/crocs-muni/sec-certs/blob/main/pyproject.toml) for settings)
-- isort (see [pyproject.toml](https://github.com/crocs-muni/sec-certs/blob/main/pyproject.toml) for settings)
-- Flake8 (see [.flake8](https://github.com/crocs-muni/sec-certs/blob/main/.flake8) for settings)
+- Ruff (see [pyproject.toml](https://github.com/crocs-muni/sec-certs/blob/main/pyproject.toml) for settings)
 - PyUpgrade
 
-These tools can be installed via [dev_requirements.txt](https://github.com/crocs-muni/sec-certs/blob/main/dev_requirements.txt) You can use [pre-commit](https://pre-commit.com/) tool register git hook that will evalute these checks prior to any commit and abort the commit for you. Note that the pre-commit is not meant to automatically fix the issues, just warn you.
+These tools can be installed via [dev_requirements.txt](https://github.com/crocs-muni/sec-certs/blob/main/dev_requirements.txt) You can use [pre-commit](https://pre-commit.com/) tool to register git hook that will evalute these checks prior to any commit and abort the commit for you. Note that the pre-commit is not meant to automatically fix the issues, just warn you.
 
 It should thus suffice to:
 
 ```bash
 pip3 install -r ./dev_requirements.txt &&
 pre-commit install &&
 pre-commit run --all-files
 ```
 
 To ivoke the tools manually, you can, in the repository root, use:
 - Mypy: `mypy .`
 - Black: `black --check .` (without the flag to reformat)
-- isort: `isort --check-only .` (without the flag to actually fix the issue)
-- Flake8: `flake8 .`
-- PyUpgrade: `pyupgrade --py38-plus 'find ./sec_certs/ -name "*.py" -type f'`
+- Ruff: `ruff ." (or with `--fix` flag to apply fixes)
 
 ## Documentation
 
 Every public method of a module that can be leveraged as an API by user should be documented. The docstrng style should
 be `sphinx-oneline`.
 
 The documentation is built using `sphinx` with `mnyst` extension that allows for markdown files. Folder `notebooks/examples` is symbolically linked to `/docs` and its contents will be automatically parsed. These notebooks are supposed to be runnable from Binder.
```

### Comparing `sec-certs-0.1.3/Dockerfile` & `sec-certs-0.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/LICENSE` & `sec-certs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/PKG-INFO` & `sec-certs-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-certs
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for data scraping and analysis of security certificates from Common Criteria and FIPS 140-2/3 frameworks
 Author: Jan Jancar, Petr Svenda, Jiri Michalik, Stanislav Bobon
 Author-email: Adam Janovsky <adamjanovsky@mail.muni.cz>
 License: MIT
 Project-URL: Homepage, https://seccerts.org
 Project-URL: GitHub, https://github.com/crocs-muni/sec-certs/
 Project-URL: Documentation, https://seccerts.org/docs
@@ -79,7 +79,13 @@
 
 # Get certificates from 2015 and newer
 df_2015_and_newer = df.loc[df.year_from > 2014]
 
 # Plot distribution of years of certification
 df.year_from.value_counts().sort_index().plot.line()
 ```
+
+## Authors
+
+This work is being done at [CRoCS MUNI](https://crocs.fi.muni.cz/) by Adam Janovsky, Jan Jancar, Petr Svenda, Jiri Michalik, Lukasz Chmielewski and other contributors. This work was supported by the Internal grant agency of Masaryk University, CZ.02.2.69/0.0/0.0/19_073/0016943.
+
+![](docs/_static/logolink_OP_VVV_hor_barva_eng.jpg)
```

### Comparing `sec-certs-0.1.3/README.md` & `sec-certs-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -53,7 +53,13 @@
 
 # Get certificates from 2015 and newer
 df_2015_and_newer = df.loc[df.year_from > 2014]
 
 # Plot distribution of years of certification
 df.year_from.value_counts().sort_index().plot.line()
 ```
+
+## Authors
+
+This work is being done at [CRoCS MUNI](https://crocs.fi.muni.cz/) by Adam Janovsky, Jan Jancar, Petr Svenda, Jiri Michalik, Lukasz Chmielewski and other contributors. This work was supported by the Internal grant agency of Masaryk University, CZ.02.2.69/0.0/0.0/19_073/0016943.
+
+![](docs/_static/logolink_OP_VVV_hor_barva_eng.jpg)
```

### Comparing `sec-certs-0.1.3/data/cert_id_eval/duplicate_ids.csv` & `sec-certs-0.1.4/data/cert_id_eval/duplicate_ids.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/cert_id_eval/missing_ids.csv` & `sec-certs-0.1.4/data/cert_id_eval/missing_ids.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/cert_id_eval/random.csv` & `sec-certs-0.1.4/data/cert_id_eval/random.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/cert_id_eval/random_references.csv` & `sec-certs-0.1.4/data/cert_id_eval/random_references.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/cert_id_eval/truth.csv` & `sec-certs-0.1.4/data/cert_id_eval/truth.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/cpe_eval/manual_cpe_labels.json` & `sec-certs-0.1.4/data/cpe_eval/manual_cpe_labels.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/cpe_eval/random.csv` & `sec-certs-0.1.4/data/cpe_eval/random.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/label_studio_interface.txt` & `sec-certs-0.1.4/data/label_studio_interface.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/old_manual_cpe_labels/cc.json` & `sec-certs-0.1.4/data/old_manual_cpe_labels/cc.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/old_manual_cpe_labels/fips.json` & `sec-certs-0.1.4/data/old_manual_cpe_labels/fips.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/sar_correlations/all_certs_sar_cve_corr.csv` & `sec-certs-0.1.4/data/sar_correlations/all_certs_sar_cve_corr.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/sar_correlations/readme.md` & `sec-certs-0.1.4/data/sar_correlations/readme.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv` & `sec-certs-0.1.4/data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/validation_test_split/cc/test.json` & `sec-certs-0.1.4/data/validation_test_split/cc/test.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/validation_test_split/cc/validation.json` & `sec-certs-0.1.4/data/validation_test_split/cc/validation.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/validation_test_split/fips/test.json` & `sec-certs-0.1.4/data/validation_test_split/fips/test.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/data/validation_test_split/fips/validation.json` & `sec-certs-0.1.4/data/validation_test_split/fips/validation.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/Makefile` & `sec-certs-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/_static/logo.png` & `sec-certs-0.1.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/_static/logo.svg` & `sec-certs-0.1.4/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/_static/logo_badge.png` & `sec-certs-0.1.4/docs/_static/logo_badge.png`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/_static/logo_badge.svg` & `sec-certs-0.1.4/docs/_static/logo_badge.svg`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/api/dataset.md` & `sec-certs-0.1.4/docs/api/dataset.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/api/model.md` & `sec-certs-0.1.4/docs/api/model.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/conf.py` & `sec-certs-0.1.4/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # import sys
 # sys.path.insert(0, os.path.abspath("."))
 from importlib.metadata import version as get_version
 
 # -- Project information -----------------------------------------------------
 
 project = "sec-certs"
-copyright = "2020-2022"
+copyright = "CRoCS MUNI | 2020-2023"
 
 # Note thas this inference won't work from Docker: https://github.com/pypa/setuptools_scm/#usage-from-docker
 release = ".".join(get_version("sec-certs").split(".")[:3])
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -59,14 +59,14 @@
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 html_logo = "_static/logo.png"
 html_favicon = "_static/logo_badge.png"
 
 html_theme_options = {
-    "repository_url": "https://anonymous.4open.science/r/sec-certs-7A92",
+    "repository_url": "https://github.com/crocs-muni/sec-certs",
     "repository_branch": "main",
     "launch_buttons": {"binderhub_url": "https://mybinder.org"},
     "use_fullscreen_button": False,
 }
 
 myst_heading_anchors = 3
```

### Comparing `sec-certs-0.1.3/docs/index.md` & `sec-certs-0.1.4/docs/index.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 # Sec-certs documentation
 
-```{warning}
-This documentation was anonymized but may still contain occasional links back to the non-anonymous GitHub repository.
-```
-
-
 Welcome to the technical documentation of *sec-certs* tool for the data analysis of products certified with Common Criteria or FIPS 140 frameworks. If you're looking for general description of the tool, its use cases and capabilites, we refer you to [sec-certs homepage](https://seccerts.org/). If you are looking for more advanced knowledge, e.g. how to mine your own data, how to extend the tool, and so forth, this is the right place.
 
 There are three main parts of this documentation. *User's guide* describes high-level use of our tool. Driven by this knowledge, you can progress to *Notebook examples* that showcase some of the API that we use in the form of Jupyter notebooks. The documentation also contains some of the modules documented with `autodoc`, see *API reference*. Still, some dark corners of our codebase are not documented. To inspect the code directly, see the [sec_certs](https://github.com/crocs-muni/sec-certs/tree/main/src/sec_certs) module. If you want, you can run the notebooks as they are stored in the [project repository](https://github.com/crocs-muni/sec-certs/tree/main/notebooks). If you are interested in contributing to our project or in other aspects of our development, you can consult the relevant *GitHub artifacts*
 
 ```{button-ref} quickstart
 :align: center
 :color: primary
@@ -22,31 +17,33 @@
 
 ```{toctree}
 :hidden:
 :caption: Navigation
 :maxdepth: 1
 Seccerts homepage <https://seccerts.org/>
 Seccerts docs <https://seccerts.org/docs>
-GitHub repo <https://anonymous.4open.science/r/sec-certs-7A92/>
+GitHub repo <https://github.com/crocs-muni/sec-certs>
 Seccerts PyPi <https://pypi.org/project/sec-certs/>
 ```
 
 ```{toctree}
 :hidden: True
 :caption: User's guide
 :maxdepth: 1
 installation.md
 quickstart.md
 configuration.md
+user_guide.md
 ```
 
 ```{toctree}
 :caption: Notebook examples
 :hidden: True
 :maxdepth: 1
+notebooks/examples/est_solution.ipynb
 notebooks/examples/cc.ipynb
 notebooks/examples/fips.ipynb
 notebooks/examples/model.ipynb
 notebooks/examples/fips_iut.ipynb
 notebooks/examples/fips_mip.ipynb
 ```
```

### Comparing `sec-certs-0.1.3/docs/installation.md` & `sec-certs-0.1.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/make.bat` & `sec-certs-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/docs/quickstart.md` & `sec-certs-0.1.4/docs/quickstart.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 ::::{tab-set}
 
 :::{tab-item} Common Criteria
 1. Install the latest version with `pip install -U sec-certs && python -m spacy download en_core_web_sm` (see [installation](installation.md)).
 2. In your Python interpreter, type
 ```python
-from sec_certs.dataset import CCDataset
+from sec_certs.dataset.cc import CCDataset
 
 dset = CCDataset.from_web_latest()
 ```
 to obtain to obtain freshly processed dataset from [seccerts.org](https://seccerts.org).
 
 3. Play with the dataset. See [example notebook](./notebooks/examples/cc.ipynb).
 :::
 
 :::{tab-item} FIPS 140
 1. Install the latest version with `pip install -U sec-certs && python -m spacy download en_core_web_sm` (see [installation](installation.md)).
 2. In your Python interpreter, type
 ```python
-from sec_certs.dataset import FIPSDataset
+from sec_certs.dataset.fips import FIPSDataset
 
 dset = FIPSDataset.from_web_latest()
 ```
 to obtain to obtain freshly processed dataset from [seccerts.org](https://seccerts.org).
 
 3. Play with the dataset. See [example notebook](./notebooks/examples/fips.ipynb).
 :::
```

### Comparing `sec-certs-0.1.3/notebooks/cc/cert_id_eval.ipynb` & `sec-certs-0.1.4/notebooks/cc/cert_id_eval.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/cc/cpe_eval.ipynb` & `sec-certs-0.1.4/notebooks/cc/cpe_eval.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923511904761905%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1, 'source': {insert: [(2, 'import json\\n'), (3, 'import "*

 * *            "tempfile')], delete: [2]}}, 3: {'execution_count': 2, 'outputs': {0: {'name': "*

 * *            "'stderr', 'text': ['Downloading CC Dataset: 100%|██████████| 139M/139M [00:15<00:00, "*

 * *            "9.61MB/s] \\n']}}, 'source': {insert: [(13, 'with tempfile.TemporaryDirectory() as "*

 * *            "tmp_dir:\\n'), (14, '    dset.root_dir = tmp_dir\\n'), (15, '    dset.certs = "*

 * *            "{x.dgst: x for x i […]*

```diff
@@ -7,40 +7,41 @@
                 "## Manual CPE matching evaluation\n",
                 "\n",
                 "This notebook assists the manual matching evaluation"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from sec_certs.dataset import CCDataset\n",
                 "import pandas as pd\n",
-                "import json"
+                "import json\n",
+                "import tempfile"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Prepare the input data for label studio"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
+                    "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Max CPE matches: 37\n"
+                        "Downloading CC Dataset: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 139M/139M [00:15<00:00, 9.61MB/s] \n"
                     ]
                 }
             ],
             "source": [
                 "dset = CCDataset.from_web_latest()\n",
                 "df = dset.to_pandas()\n",
                 "\n",
@@ -50,17 +51,18 @@
                 "# It may be handy to display max number of assigned cpe matches here\n",
                 "eval_certs[\"n_cpes\"] = eval_certs.cpe_matches.map(len)\n",
                 "max_n_cpes = eval_certs.n_cpes.max()\n",
                 "print(f\"Max CPE matches: {max_n_cpes}\")\n",
                 "\n",
                 "# Now you may want to adjust the key `cpe_n_max_matches` config in sec_certs/config/settings.yml according to max_n_cpes\n",
                 "# This helps to avoid clutter in label studio interface\n",
-                "\n",
-                "dset.certs = {x.dgst: x for x in dset if x.dgst in eval_certs.index.tolist()}\n",
-                "dset.to_label_studio_json(\"./label_studio_input_data.json\")"
+                "with tempfile.TemporaryDirectory() as tmp_dir:\n",
+                "    dset.root_dir = tmp_dir\n",
+                "    dset.certs = {x.dgst: x for x in dset if x.dgst in eval_certs.index.tolist()}\n",
+                "    dset.to_label_studio_json(\"./label_studio_input_data.json\", update_json=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "`Now you import this data to label studio and label it`"
@@ -71,15 +73,15 @@
             "metadata": {},
             "source": [
                 "## Load the data from label studio and show the results"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Evaluated 607 CPE matches in 100 certificates\n",
```

### Comparing `sec-certs-0.1.3/notebooks/cc/references.ipynb` & `sec-certs-0.1.4/notebooks/cc/references.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921084640300034%*

 * *Differences: {"'cells'": "{1: {'execution_count': None}, 2: {'execution_count': None, 'outputs': []}, 3: "*

 * *            "{'execution_count': None}, 6: {'execution_count': None, 'outputs': []}, 7: "*

 * *            "{'execution_count': None, 'outputs': [], 'source': {insert: [(4, '    if "*

 * *            "pd.isnull(referencing):\\n')], delete: [6, 4]}}, 9: {'execution_count': None}, 10: "*

 * *            "{'execution_count': None, 'outputs': [], 'source': {insert: [(4, "*

 * *            '\'exploded["ref_category"] = exploded.directly_re […]*

```diff
@@ -15,15 +15,15 @@
                 "\n",
                 "The notebook has two parts, an analysis part and a network visualization part.\n",
                 "But first some common initialization and data loading."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
@@ -69,37 +69,29 @@
                 "#sns.set_context(\"notebook\")  # Set to \"paper\" for use in paper :)\n",
                 "\n",
                 "#plt.rcParams['figure.figsize'] = (10, 6)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Downloading CC Dataset: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 135M/135M [00:26<00:00, 5.34MB/s]\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "# Initialize\n",
                 "dset = CCDataset.from_web_latest()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = dset.to_pandas()\n",
                 "df_id_rich = df.loc[df.cert_id.notnull()].copy()"
             ]
         },
@@ -122,33 +114,22 @@
                 "\n",
                 "- From the numbers follows that whenever a certificate is directly referencing some else, it also indirectly references some else\n",
                 "- We have more outgoing references than ingoing references, which kinda makes sense. You don't have to be aware that some other cert references you"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 },
                 "scrolled": true
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\\newcommand{\\numCcAllDirectReferencing}{1500}\n",
-                        "\\newcommand{\\numCcAllNotDirectReferencing}{3641}\n",
-                        "\\newcommand{\\numCcWithIdDirectReferencing}{1500}\n",
-                        "\\newcommand{\\numCcWithIdNotDirectReferencing}{3565}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "df[\"has_outgoing_direct_references\"] = df.directly_referencing.notnull()\n",
                 "df[\"has_incoming_direct_references\"] = df.directly_referenced_by.notnull()\n",
                 "df[\"has_outgoing_indirect_references\"] = df.indirectly_referencing.notnull()\n",
                 "df[\"has_incoming_indirect_references\"] = df.indirectly_referenced_by.notnull()\n",
                 "\n",
                 "#df.loc[:, [\"directly_referenced_by\", \"indirectly_referenced_by\", \"directly_referencing\", \"indirectly_referencing\"]].notnull().describe()\n",
@@ -165,48 +146,38 @@
                 "print(f\"\\\\newcommand{{\\\\numCcWithIdNotDirectReferencing}}{{{len(df_id_rich) - df_id_rich.has_outgoing_direct_references.sum()}}}\")\n",
                 "\n",
                 "#df_id_rich.loc[:, [\"directly_referenced_by\", \"indirectly_referenced_by\", \"directly_referencing\", \"indirectly_referencing\"]].notnull().describe()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\\newcommand{\\numCCActiveDirectReferencing}{545}\n",
-                        "\\newcommand{\\numCCActiveDirectReferencingArchived}{169}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "print(f\"\\\\newcommand{{\\\\numCCActiveDirectReferencing}}{{{df_id_rich.loc[df_id_rich.status == 'active'].has_outgoing_direct_references.sum()}}}\")\n",
                 "\n",
                 "archived_cert_id_list = set(df_id_rich[df_id_rich.status == \"archived\"].cert_id)\n",
                 "def contains_archived_cert_reference(referencing):\n",
-                "    if referencing is np.nan:\n",
+                "    if pd.isnull(referencing):\n",
                 "        return False\n",
-                "    \n",
                 "    return bool(archived_cert_id_list.intersection(referencing))\n",
                 "print(f\"\\\\newcommand{{\\\\numCCActiveDirectReferencingArchived}}{{{df_id_rich[df_id_rich.status == 'active'].directly_referencing.apply(contains_archived_cert_reference).sum()}}}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Plot direct references per category"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
@@ -225,39 +196,27 @@
                 "    )\n",
                 "    countplot.tick_params(axis=\"x\", rotation=90)\n",
                 "    countplot.legend(title=' '.join(col.split('_')), bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.0)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\\newcommand{\\numCCDirectRefsSameCategory}{2133}\n",
-                        "\\newcommand{\\numCCDirectRefsOtherCategory}{192}\n",
-                        "\\newcommand{\\numCCDirectRefs}{2325}\n",
-                        "\\newcommand{\\numCCDirectRefsFromSmartcards}{1896}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "cert_id_to_category_mapping = dict(zip(df.cert_id, df.category))\n",
                 "cert_id_to_category_mapping[np.NaN] = \"No references\"\n",
                 "\n",
                 "exploded = df_id_rich.loc[:, [\"category\", \"directly_referencing\"]].explode(\"directly_referencing\")\n",
-                "\n",
-                "exploded[\"ref_category\"] = exploded.directly_referencing.map(cert_id_to_category_mapping)\n",
+                "exploded[\"ref_category\"] = exploded.directly_referencing.map(lambda x: cert_id_to_category_mapping[x] if pd.notnull(x) else np.nan)\n",
                 "exploded = exploded.loc[exploded.ref_category.notnull()]\n",
                 "\n",
                 "exploded_with_refs = exploded.loc[exploded.ref_category != \"No references\"]\n",
                 "print(f\"\\\\newcommand{{\\\\numCCDirectRefsSameCategory}}{{{(exploded_with_refs.category == exploded_with_refs.ref_category).sum()}}}\")\n",
                 "print(f\"\\\\newcommand{{\\\\numCCDirectRefsOtherCategory}}{{{(exploded_with_refs.category != exploded_with_refs.ref_category).sum()}}}\")\n",
                 "print(f\"\\\\newcommand{{\\\\numCCDirectRefs}}{{{len(exploded_with_refs)}}}\")\n",
                 "print(f\"\\\\newcommand{{\\\\numCCDirectRefsFromSmartcards}}{{{(exploded_with_refs.category == 'ICs, Smart Cards and Smart Card-Related Devices and Systems').sum()}}}\")\n",
@@ -282,15 +241,15 @@
             "metadata": {},
             "source": [
                 "### Plot direct references per scheme"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
@@ -316,29 +275,21 @@
             "metadata": {},
             "source": [
                 "### Number of certificates referencing archived certificates"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Number of certificates that reference some archived certificate: 933\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "def references_archived_cert(references):\n",
                 "    if pd.isnull(references):\n",
                 "        return False\n",
                 "\n",
                 "    return any([x in cert_ids] for x in references)\n",
                 "\n",
@@ -369,15 +320,15 @@
             "metadata": {},
             "source": [
                 "### Count scheme references"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
@@ -402,26 +353,17 @@
                 "figure.savefig(\"scheme_references.pdf\", bbox_inches=\"tight\")\n",
                 "figure.savefig(\"scheme_references.pgf\", bbox_inches=\"tight\")\n",
                 "plt.close(figure)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\\newcommand{\\numCCUSReferencing}{4}\n",
-                        "\\newcommand{\\numCCUS}{959}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "print(f\"\\\\newcommand{{\\\\numCCUSReferencing}}{{{len(df_id_rich.loc[(df_id_rich.scheme == 'US') & (df_id_rich.directly_referencing.notnull())])}}}\")\n",
                 "print(f\"\\\\newcommand{{\\\\numCCUS}}{{{len(df_id_rich.loc[(df_id_rich.scheme == 'US')])}}}\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -430,15 +372,15 @@
                 "### Temporal evolution of references\n",
                 "\n",
                 "Shows plot with relative number of certificates for a given year that reference some other certificate"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": null,
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
@@ -1190,35 +1132,27 @@
                 "    df: DataFrame, labels: ndarray, side: str\n",
                 ") -> Tuple[Dict, float64]:\n",
                 "    \"\"\"Determine positions of label patches and total widths\"\"\"\n",
                 "    widths: Dict = defaultdict()\n",
                 "    for i, label in enumerate(labels):\n",
                 "        label_widths = {}\n",
                 "        label_widths[side] = df[df[side] == label][side + \"Weight\"].sum()\n",
-                "        print(\"a\")\n",
                 "        if i == 0:\n",
                 "            label_widths[\"bottom\"] = 0\n",
                 "            label_widths[\"top\"] = label_widths[side]\n",
                 "        else:\n",
                 "            bottom_width = widths[labels[i - 1]][\"top\"]\n",
                 "            weighted_sum = 0.05 * df[side + \"Weight\"].sum()\n",
                 "            label_widths[\"bottom\"] = bottom_width + weighted_sum\n",
                 "            label_widths[\"top\"] = label_widths[\"bottom\"] + label_widths[side]\n",
                 "            topEdge = label_widths[\"top\"]\n",
                 "        widths[label] = label_widths\n",
                 "        LOGGER.debug(\"%s position of '%s' : %s\", side, label, label_widths)\n",
                 "    return widths, topEdge\n"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.8.13 ('venv': venv)",
             "language": "python",
             "name": "python3"
```

### Comparing `sec-certs-0.1.3/notebooks/cc/temporal_trends.ipynb` & `sec-certs-0.1.4/notebooks/cc/temporal_trends.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/cc/vulnerabilities.ipynb` & `sec-certs-0.1.4/notebooks/cc/vulnerabilities.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991122883232948%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(9, \'sns.set_style("whitegrid")\\n\'), (16, \'import '*

 * *            "tempfile\\n'), (17, 'from sec_certs.dataset import CCDataset, "*

 * *            "CCDatasetMaintenanceUpdates, CVEDataset, CPEDataset\\n'), (33, "*

 * *            "'RESULTS_DIR.mkdir(exist_ok=True)')], delete: [33, 17, 16, 9]}}, 3: {'source': "*

 * *            "{insert: [(1, '# dset: CCDataset = "*

 * *            'CCDataset.from_json("/path/to/cc_dataset.json")\\n\'), (2, \'# '*

 * *            '#dset.process_maintenance_ […]*

```diff
@@ -20,23 +20,23 @@
                 "import matplotlib.pyplot as plt\n",
                 "import pandas as pd\n",
                 "import seaborn as sns\n",
                 "from tqdm.notebook import tqdm\n",
                 "\n",
                 "from sec_certs.cert_rules import cc_rules\n",
                 "\n",
-                "plt.style.use(\"seaborn-whitegrid\")\n",
+                "sns.set_style(\"whitegrid\")\n",
                 "sns.set_palette(\"deep\")\n",
                 "sns.set_context(\"notebook\")  # Set to \"paper\" for use in paper :)\n",
                 "\n",
                 "import itertools\n",
                 "import warnings\n",
                 "from pathlib import Path\n",
-                "\n",
-                "from sec_certs.dataset import CCDataset, CPEDataset, CVEDataset, CCDatasetMaintenanceUpdates\n",
+                "import tempfile\n",
+                "from sec_certs.dataset import CCDataset, CCDatasetMaintenanceUpdates, CVEDataset, CPEDataset\n",
                 "from sec_certs.utils.pandas import (\n",
                 "    compute_cve_correlations,\n",
                 "    compute_maintenances_that_come_after_vulns,\n",
                 "    discover_sar_families,\n",
                 "    expand_df_with_cve_cols,\n",
                 "    filter_to_cves_within_validity_period,\n",
                 "    get_sar_level_from_set,\n",
@@ -44,15 +44,15 @@
                 "    move_fixing_mu_to_directory,\n",
                 "    prepare_cwe_df,\n",
                 ")\n",
                 "\n",
                 "warnings.simplefilter(action=\"ignore\", category=pd.errors.PerformanceWarning)\n",
                 "\n",
                 "RESULTS_DIR = Path(\"./results\")\n",
-                "RESULTS_DIR.mkdir(exist_ok=True)\n"
+                "RESULTS_DIR.mkdir(exist_ok=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Retrieve necessary objects from sec-certs"
@@ -61,24 +61,29 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Local instantiation\n",
-                "dset: CCdataset = CCDataset.from_web_latest()\n",
-                "# dset.process_maintenance_updates() # Run this only once, can take ~10 minutes to finnish, fully processes maintenance updates\n",
-                "main_dset = CCDatasetMaintenanceUpdates.from_json(dset.mu_dataset_path)\n",
-                "cve_dset: CVEDataset = dset._prepare_cve_dataset()\n",
-                "cpe_dset: CPEDataset = dset._prepare_cpe_dataset()\n",
+                "# dset: CCDataset = CCDataset.from_json(\"/path/to/cc_dataset.json\")\n",
+                "# #dset.process_maintenance_updates() # Run this only once, can take ~10 minutes to finnish, fully processes mainten#ance updates\n",
+                "# main_dset = CCDatasetMaintenanceUpdates.from_json(dset.mu_dataset_path) # TODO: Recover me\n",
+                "# cve_dset: CVEDataset = dset._prepare_cve_dataset()\n",
+                "# cpe_dset: CPEDataset = dset._prepare_cpe_dataset()\n",
                 "\n",
                 "# Remote instantiation\n",
-                "# dset: CCDataset = CCDataset.from_web_latest()\n",
-                "# # main_dset: CDatasetMaintenanceUpdates = CCDatasetMaintenanceUpdates.from_web_latest()\n",
-                "# cve_dset: CVEDataset = CVEDataset.from_web()"
+                "with tempfile.TemporaryDirectory() as tmp_dir:\n",
+                "    dset: CCDataset = CCDataset.from_web_latest()\n",
+                "    dset.root_dir = tmp_dir\n",
+                "    main_dset: CCDatasetMaintenanceUpdates = CCDatasetMaintenanceUpdates.from_web_latest()\n",
+                "    dset._prepare_cpe_dataset()\n",
+                "    dset._prepare_cve_dataset()\n",
+                "    cve_dset = dset.auxiliary_datasets.cve_dset\n",
+                "    cpe_dset = dset.auxiliary_datasets.cpe_dset"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Dataset preprocessing\n",
@@ -108,35 +113,36 @@
                 "    main_dates = main_dset.get_maintenance_dates_df()\n",
                 "    df = pd.concat([df, main_dates], axis=\"columns\")\n",
                 "\n",
                 "# Expand DataFrame with CVEs that affect some certificate\n",
                 "cves = list(itertools.chain.from_iterable(x.heuristics.related_cves for x in dset if x.heuristics.related_cves))\n",
                 "cve_dict = {x: cve_dset[x] for x in cves}\n",
                 "cve_dset.cves = cve_dict  # Limit cve_dset to CVEs relevant to some certificate\n",
+                "\n",
                 "df = expand_df_with_cve_cols(df, cve_dset)\n",
                 "\n",
                 "df_cves_within_validity_period = filter_to_cves_within_validity_period(\n",
                 "    df.loc[(df.not_valid_before.notnull()) & (df.not_valid_after.notnull())].copy(), cve_dset\n",
                 ")\n",
                 "df_cves_within_validity_period = expand_df_with_cve_cols(df_cves_within_validity_period, cve_dset)\n",
                 "\n",
                 "df_cpe_rich = df.loc[~df.cpe_matches.isnull()].copy()\n",
-                "df_cve_rich = df.loc[df.n_cves > 0].copy()\n"
+                "df_cve_rich = df.loc[df.n_cves > 0].copy()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Take a look at columns related to CVEs\n",
                 "df.loc[\n",
                 "    ~df.related_cves.isna(), [\"related_cves\", \"cve_published_dates\", \"earliest_cve\", \"worst_cve_score\", \"avg_cve_score\"]\n",
-                "]\n"
+                "]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Plots\n",
@@ -231,14 +237,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# TODO: The number of evaluated families is suspiciously low. Must investigate before recomputing results.\n",
                 "# This limits analysis to SAR families that are popular-enough (>100 CVE-rich certs, second-most-popular value with >= 40 instances)\n",
                 "cve_rich = df_cves_within_validity_period.loc[df_cves_within_validity_period.related_cves.notnull()].copy()\n",
                 "families = discover_sar_families(cve_rich.extracted_sars)\n",
                 "\n",
                 "for family in tqdm(families):\n",
                 "    cve_rich[family] = cve_rich.extracted_sars.map(lambda x: get_sar_level_from_set(x, family))\n",
                 "\n",
@@ -274,15 +281,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df_corr\n"
+                "df_cves_within_validity_period"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Time from CVE to maintenance update\n",
@@ -343,15 +350,15 @@
                 "        \"related_cves\",\n",
                 "        \"not_valid_before\",\n",
                 "        \"not_valid_after\",\n",
                 "        \"cve_published_dates\",\n",
                 "        \"maintenance_dates\",\n",
                 "        \"earliest_maintenance_after_vuln\",\n",
                 "    ],\n",
-                "].to_csv(\"/Users/adam/Downloads/vulns_before_mu.csv\")\n"
+                "].to_csv(RESULTS_DIR / \"vulns_before_mu.csv\")\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -495,15 +502,15 @@
                 "        (df_cve_rich.year_from < 2022) & (df_cve_rich.n_cves < n_cves_top_20_certs) & (~df_cve_rich.eal.isna()),\n",
                 "        [\"related_cves\", \"eal\", \"category\"],\n",
                 "    ]\n",
                 "    .explode(\"related_cves\")\n",
                 "    .rename(columns={\"related_cves\": \"cve_id\"})\n",
                 ")\n",
                 "cves[\"published_date\"] = cves.cve_id.map(lambda x: cve_dset[x].published_date).dt.tz_localize(None).dt.normalize()\n",
-                "cves[\"base_score\"] = cves.cve_id.map(lambda x: cve_dset[x].impact.base_score)\n",
+                "cves[\"base_score\"] = cves.cve_id.map(lambda x: cve_dset[x].metrics.base_score)\n",
                 "cves = cves.drop_duplicates()\n",
                 "\n",
                 "g = sns.relplot(\n",
                 "    data=cves,\n",
                 "    x=\"published_date\",\n",
                 "    y=\"base_score\",\n",
                 "    hue=\"eal\",\n",
```

### Comparing `sec-certs-0.1.3/notebooks/examples/cc.ipynb` & `sec-certs-0.1.4/notebooks/examples/cc.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/examples/fips.ipynb` & `sec-certs-0.1.4/notebooks/examples/fips.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/examples/fips_iut.ipynb` & `sec-certs-0.1.4/notebooks/examples/fips_iut.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/examples/fips_mip.ipynb` & `sec-certs-0.1.4/notebooks/examples/fips_mip.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/examples/model.ipynb` & `sec-certs-0.1.4/notebooks/examples/model.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/final_run.ipynb` & `sec-certs-0.1.4/notebooks/final_run.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/fips/in_process.ipynb` & `sec-certs-0.1.4/notebooks/fips/in_process.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782657657657657%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, 'from itertools import takewhile\\n'), (1, 'from "*

 * *            "operator import itemgetter\\n'), (2, '\\n'), (6, 'from sec_certs.model.fips_matching "*

 * *            "import FIPSProcessMatcher\\n'), (7, 'from sec_certs.dataset.fips import "*

 * *            "FIPSDataset\\n'), (8, 'from sec_certs.configuration import config\\n'), (13, 'from "*

 * *            "tqdm import tqdm\\n')], delete: [11, 8, 6]}}, 7: {'source': {insert: [(5, 'for "*

 * *            "snapshot in tqdm(sorted(iut […]*

```diff
@@ -3,35 +3,53 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4d7d7d8c",
             "metadata": {},
             "outputs": [],
             "source": [
+                "from itertools import takewhile\n",
+                "from operator import itemgetter\n",
+                "\n",
                 "from sec_certs.dataset.fips_mip import MIPDataset\n",
                 "from sec_certs.dataset.fips_iut import IUTDataset\n",
                 "from sec_certs.sample.fips_mip import MIPStatus\n",
+                "from sec_certs.model.fips_matching import FIPSProcessMatcher\n",
+                "from sec_certs.dataset.fips import FIPSDataset\n",
+                "from sec_certs.configuration import config\n",
                 "import pandas as pd\n",
                 "import seaborn as sns\n",
                 "import matplotlib.pyplot as plt\n",
-                "import math\n",
                 "import numpy as np\n",
-                "import tqdm\n",
+                "from tqdm import tqdm\n",
                 "import matplotlib.ticker as mtick\n",
                 "import warnings\n",
-                "from pathlib import Path\n",
                 "\n",
                 "plt.style.use(\"seaborn-whitegrid\")\n",
                 "sns.set_palette(\"deep\")\n",
                 "sns.set_context(\"notebook\") # Set to \"paper\" for use in paper :)\n",
                 "\n",
                 "warnings.simplefilter(action='ignore', category=pd.errors.PerformanceWarning)"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false,
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
+            "outputs": [],
+            "source": [
+                "fips = FIPSDataset.from_web_latest()\n"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "bd5f0fd6",
             "metadata": {},
             "source": [
                 "## IUT dataset"
             ]
         },
@@ -93,18 +111,18 @@
             "outputs": [],
             "source": [
                 "def iut_key(entry):\n",
                 "    return entry.module_name, entry.vendor_name, entry.standard\n",
                 "\n",
                 "iut_first_seen = {}\n",
                 "iut_last_seen = {}\n",
-                "for snapshot in sorted(iut_dset.snapshots, key=lambda x: x.timestamp):\n",
+                "for snapshot in tqdm(sorted(iut_dset.snapshots, key=lambda x: x.timestamp)):\n",
                 "    snapshot_date = snapshot.timestamp.date()\n",
                 "    for entry in snapshot.entries:\n",
-                "        entry_key = entry #iut_key(entry) # or entry here\n",
+                "        entry_key = entry # iut_key(entry) # or entry here\n",
                 "        if entry_key not in iut_first_seen:\n",
                 "            iut_first_seen[entry_key] = snapshot_date\n",
                 "        if entry_key not in iut_last_seen or iut_last_seen[entry_key] < snapshot_date:\n",
                 "            iut_last_seen[entry_key] = snapshot_date\n",
                 "\n",
                 "#iut_local_df = pd.DataFrame([(entry[0], entry[1], entry[2], iut_first_seen[entry], iut_last_seen[entry], iut_last_seen[entry] == snapshot_date) for entry in iut_first_seen.keys()], columns=(\"name\", \"vendor\", \"standard\", \"first_seen\", \"last_seen\", \"present\"))\n",
                 "iut_local_df = pd.DataFrame([(entry.module_name, entry.vendor_name, entry.standard, entry.iut_date, iut_first_seen[entry], iut_last_seen[entry], iut_last_seen[entry] == snapshot_date) for entry in iut_first_seen.keys()], columns=(\"name\", \"vendor\", \"standard\", \"iut_date\", \"first_seen\", \"last_seen\", \"present\"))\n",
@@ -179,14 +197,41 @@
             "outputs": [],
             "source": [
                 "iut_local_df.vendor.value_counts()"
             ]
         },
         {
             "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false,
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
+            "source": [
+                "### IUT - Certificate mapping"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false,
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
+            "outputs": [],
+            "source": [
+                "first_snapshot = iut_dset.snapshots[-1]\n",
+                "matches = FIPSProcessMatcher.match_snapshot(first_snapshot, fips)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "cbc02977",
             "metadata": {},
             "source": [
                 "## MIP dataset"
             ]
         },
         {
@@ -334,14 +379,41 @@
             "source": [
                 "with sns.plotting_context(\"notebook\", font_scale=0.75):\n",
                 "    g = sns.FacetGrid(mip_local_df.loc[~mip_local_df.present], col=\"status\", hue=\"standard\", col_wrap=2, height=2, ylim=(0,300))\n",
                 "    g.map(sns.histplot, \"seen_for\")\n",
                 "    g.set_titles(\"{col_name}\")\n",
                 "    plt.show()"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "collapsed": false,
+                "pycharm": {
+                    "name": "#%% md\n"
+                }
+            },
+            "source": [
+                "### MIP - Certificate matching"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "collapsed": false,
+                "pycharm": {
+                    "name": "#%%\n"
+                }
+            },
+            "outputs": [],
+            "source": [
+                "first_snapshot = mip_dset.snapshots[-1]\n",
+                "matches = FIPSProcessMatcher.match_snapshot(first_snapshot, fips)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.8.13 ('venv': venv)",
             "language": "python",
             "name": "python3"
```

### Comparing `sec-certs-0.1.3/notebooks/fips/references.ipynb` & `sec-certs-0.1.4/notebooks/fips/references.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/fips/temporal_trends.ipynb` & `sec-certs-0.1.4/notebooks/fips/temporal_trends.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/fips/vulnerabilities.ipynb` & `sec-certs-0.1.4/notebooks/fips/vulnerabilities.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/latex_plotting.ipynb` & `sec-certs-0.1.4/notebooks/latex_plotting.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/notebooks/ocr.ipynb` & `sec-certs-0.1.4/notebooks/ocr.ipynb`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/pyproject.toml` & `sec-certs-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -54,85 +54,98 @@
     "ipywidgets",
     "spacy",
     "pkgconfig",
     "seaborn",
     "pySankeyBeta",
     "scipy>=1.9.0",
     "networkx",
+    "pydantic",
   ]
 
   [project.optional-dependencies]
     dev = [
-      "mypy",
+      "black==23.1.0",
+      "ruff==0.0.239",
+      "mypy==1.0.0",
       "types-PyYAML",
       "types-python-dateutil",
       "types-requests",
       "pytest",
       "pytest-cov",
       "pytest-monitor",
       "pytest-profiling",
-      "black",
-      "isort",
-      "flake8",
       "pre-commit",
       "pip-tools",
       "sphinx",
       "myst-nb>=0.14",
       "sphinx-book-theme",
       "sphinx-design",
       "sphinx-copybutton",
-      "pyupgrade",
-      "flake8-future-annotations",
       "ipython!=8.7.0",
     ]
     test = ["pytest", "coverage", "pytest-cov"]
 
   [project.urls]
     Homepage = "https://seccerts.org"
     GitHub = "https://github.com/crocs-muni/sec-certs/"
     Documentation = "https://seccerts.org/docs"
 
   [project.scripts]
     sec-certs = "sec_certs.cli:main"
 
-[tool.setuptools.package-data]
-  "*" = ["*.yaml", "*.json"]
+[tool.ruff]
+  select = [
+    "I",   # isort
+    "E",   # pycodestyle
+    "W",   # pycodestyle
+    "F",   # pyflakes
+    "C90", # mccabe
+    "UP",  # pyupgrade
+    "PTH", # enforce pathlib usage
+    "C4",  # comprehensions
+    "SIM",
+  ]
+  ignore = [
+    "E501", # line-length, should be handled by black
+  ]
+  src = ["src", "tests"]
+  line-length = 120
+  target-version = "py38"
+
+  [tool.ruff.mccabe]
+    max-complexity = 10
+
+  [tool.setuptools.package-data]
+    "*" = ["*.yaml", "*.json"]
 
 
 [tool.setuptools_scm]
   write_to = "src/sec_certs/_version.py"
   version_scheme = "no-guess-dev"
 
 [tool.black]
   line-length = 120
-  exclude = '''
+  force-exclude = '''
 /(
     \.git
   | \.mypy_cache
   | \.tox
   | venv
-  | certsvenv
   | \.venv
   | _build
   | buck-out
   | build
   | dist
   | src/sec_certs/_version.py
+  | docs
+  | .ipynb_checkpoints
+  | .eggs
 )/
 '''
 
-[tool.isort]
-  multi_line_output = 3
-  include_trailing_comma = true
-  force_grid_wrap = 0
-  use_parentheses = true
-  ensure_newline_before_comments = true
-  line_length = 120
-  skip = ["certsvenv", "build"]
-
 [tool.mypy]
   plugins = ["numpy.typing.mypy_plugin"]
   ignore_missing_imports = true
   exclude = "build/"
 
 [tool.pytest.ini_options]
   markers = ["slow: marks tests as slow (deselect with '-m \"not slow\"')"]
```

### Comparing `sec-certs-0.1.3/requirements/dev_requirements.txt` & `sec-certs-0.1.4/requirements/dev_requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     # via ipython
 beautifulsoup4==4.11.1
     # via
     #   pydata-sphinx-theme
     #   sec-certs (./../pyproject.toml)
 billiard==4.0.2
     # via sec-certs (./../pyproject.toml)
-black==22.10.0
+black==23.1.0
     # via sec-certs (./../pyproject.toml)
 blis==0.7.9
     # via thinc
 build==0.9.0
     # via pip-tools
 catalogue==2.0.8
     # via
@@ -81,20 +81,14 @@
     # via pytest
 executing==1.2.0
     # via stack-data
 fastjsonschema==2.16.2
     # via nbformat
 filelock==3.8.2
     # via virtualenv
-flake8==6.0.0
-    # via
-    #   flake8-future-annotations
-    #   sec-certs (./../pyproject.toml)
-flake8-future-annotations==1.0.0
-    # via sec-certs (./../pyproject.toml)
 fonttools==4.38.0
     # via matplotlib
 gprof2dot==2022.7.29
     # via pytest-profiling
 greenlet==2.0.1
     # via sqlalchemy
 html5lib==1.1
@@ -115,24 +109,22 @@
 iniconfig==1.1.1
     # via pytest
 ipykernel==6.19.1
     # via
     #   ipywidgets
     #   myst-nb
     #   sec-certs (./../pyproject.toml)
-ipython==8.6.0
+ipython==8.10.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
     #   sec-certs (./../pyproject.toml)
 ipywidgets==8.0.3
     # via sec-certs (./../pyproject.toml)
-isort==5.10.1
-    # via sec-certs (./../pyproject.toml)
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via
     #   myst-parser
     #   spacy
     #   sphinx
@@ -158,43 +150,41 @@
     # via matplotlib
 langcodes==3.3.0
     # via spacy
 lxml==4.9.1
     # via
     #   pikepdf
     #   sec-certs (./../pyproject.toml)
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
     # via
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.1
     # via jinja2
 matplotlib==3.6.2
     # via
     #   pysankeybeta
     #   seaborn
     #   sec-certs (./../pyproject.toml)
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
-mccabe==0.7.0
-    # via flake8
 mdit-py-plugins==0.3.3
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 memory-profiler==0.61.0
     # via pytest-monitor
 murmurhash==1.0.9
     # via
     #   preshed
     #   spacy
     #   thinc
-mypy==0.991
+mypy==1.0.0
     # via sec-certs (./../pyproject.toml)
 mypy-extensions==0.4.3
     # via
     #   black
     #   mypy
 myst-nb==0.17.1
     # via sec-certs (./../pyproject.toml)
@@ -230,14 +220,15 @@
     #   seaborn
     #   sec-certs (./../pyproject.toml)
     #   spacy
     #   tabula-py
     #   thinc
 packaging==22.0
     # via
+    #   black
     #   build
     #   deprecation
     #   ipykernel
     #   matplotlib
     #   pikepdf
     #   pydata-sphinx-theme
     #   pytest
@@ -297,27 +288,23 @@
     #   ipykernel
     #   memory-profiler
     #   pytest-monitor
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pycodestyle==2.10.0
-    # via flake8
 pycryptodome==3.16.0
     # via pypdf
 pydantic==1.10.2
     # via
     #   confection
     #   spacy
     #   thinc
 pydata-sphinx-theme==0.8.1
     # via sphinx-book-theme
-pyflakes==3.0.1
-    # via flake8
 pygments==2.13.0
     # via
     #   ipython
     #   sphinx
 pyparsing==3.0.9
     # via matplotlib
 pypdf[crypto]==3.2.1
@@ -344,16 +331,14 @@
     #   matplotlib
     #   pandas
     #   sec-certs (./../pyproject.toml)
 pytz==2022.6
     # via
     #   babel
     #   pandas
-pyupgrade==3.3.1
-    # via sec-certs (./../pyproject.toml)
 pyyaml==6.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   myst-parser
     #   pre-commit
     #   sec-certs (./../pyproject.toml)
@@ -366,14 +351,16 @@
     # via sec-certs (./../pyproject.toml)
 requests==2.28.1
     # via
     #   pytest-monitor
     #   sec-certs (./../pyproject.toml)
     #   spacy
     #   sphinx
+ruff==0.0.239
+    # via sec-certs (./../pyproject.toml)
 scikit-learn==1.2.0
     # via sec-certs (./../pyproject.toml)
 scipy==1.9.3
     # via
     #   scikit-learn
     #   sec-certs (./../pyproject.toml)
 seaborn==0.12.1
@@ -440,16 +427,14 @@
     # via sec-certs (./../pyproject.toml)
 tabulate==0.9.0
     # via jupyter-cache
 thinc==8.1.5
     # via spacy
 threadpoolctl==3.1.0
     # via scikit-learn
-tokenize-rt==5.0.0
-    # via pyupgrade
 toml==0.10.2
     # via pre-commit
 tomli==2.0.1
     # via
     #   black
     #   build
     #   coverage
```

### Comparing `sec-certs-0.1.3/requirements/requirements.txt` & `sec-certs-0.1.4/requirements/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     # via requests
 importlib-resources==5.10.1
     # via jsonschema
 ipykernel==6.19.1
     # via
     #   ipywidgets
     #   sec-certs (./../pyproject.toml)
-ipython==8.7.0
+ipython==8.10.0
     # via
     #   ipykernel
     #   ipywidgets
 ipywidgets==8.0.3
     # via sec-certs (./../pyproject.toml)
 jedi==0.18.2
     # via ipython
```

### Comparing `sec-certs-0.1.3/requirements/test_requirements.txt` & `sec-certs-0.1.4/requirements/test_requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # via jsonschema
 iniconfig==1.1.1
     # via pytest
 ipykernel==6.19.1
     # via
     #   ipywidgets
     #   sec-certs (./../pyproject.toml)
-ipython==8.7.0
+ipython==8.10.0
     # via
     #   ipykernel
     #   ipywidgets
 ipywidgets==8.0.3
     # via sec-certs (./../pyproject.toml)
 jedi==0.18.2
     # via ipython
```

### Comparing `sec-certs-0.1.3/src/sec_certs/__init__.py` & `sec-certs-0.1.4/src/sec_certs/__init__.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/src/sec_certs/cert_rules.py` & `sec-certs-0.1.4/src/sec_certs/cert_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,29 +201,27 @@
 FIPS_LIST_OF_TABLES = re.compile(r"^(?:(?:[Tt]able\s|[Ll]ist\s)(?:[Oo]f\s))[Tt]ables[\s\S]+?\f", re.MULTILINE)
 
 
 def _load():
     script_dir = Path(__file__).parent
     filepath = script_dir / "rules.yaml"
     with Path(filepath).open("r") as file:
-        loaded = yaml.load(file, Loader=yaml.FullLoader)
-    return loaded
+        return yaml.load(file, Loader=yaml.FullLoader)
 
 
-def _process(obj):
+def _process(obj: dict | list):
     if isinstance(obj, dict):
         return {k: _process(v) for k, v in obj.items()}
-    elif isinstance(obj, list):
-        return [
-            re.compile(
-                REGEXEC_SEP_START + MATCH_START + rule + MATCH_END + REGEXEC_SEP_END,
-                re.MULTILINE,
-            )
-            for rule in obj
-        ]
+    return [
+        re.compile(
+            REGEXEC_SEP_START + MATCH_START + rule + MATCH_END + REGEXEC_SEP_END,
+            re.MULTILINE,
+        )
+        for rule in obj
+    ]
 
 
 rules = _load()
 
 cc_rules = {}
 for rule_group in rules["cc_rules"]:
     cc_rules[rule_group] = _process(rules[rule_group])
```

### Comparing `sec-certs-0.1.3/src/sec_certs/cli.py` & `sec-certs-0.1.4/src/sec_certs/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 import sys
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
 from typing import Callable
 
 import click
+from pydantic import ValidationError
 
-from sec_certs.config.configuration import config
-from sec_certs.dataset import CCDataset, FIPSDataset
+from sec_certs.configuration import config
+from sec_certs.dataset.cc import CCDataset
 from sec_certs.dataset.dataset import Dataset
+from sec_certs.dataset.fips import FIPSDataset
 from sec_certs.utils.helpers import warn_if_missing_poppler, warn_if_missing_tesseract
 
 logger = logging.getLogger(__name__)
 
 EXIT_CODE_NOK: int = 1
 EXIT_CODE_OK: int = 0
 
@@ -59,15 +61,14 @@
 
 def build_or_load_dataset(
     framework: str,
     inputpath: Path | None,
     to_build: bool,
     outputpath: Path | None,
 ) -> CCDataset | FIPSDataset:
-
     constructor: type[CCDataset] | type[FIPSDataset] = CCDataset if framework == "cc" else FIPSDataset
     dset: CCDataset | FIPSDataset
 
     if to_build:
         if not outputpath:
             outputpath = DEFAULT_OUTPUTPATH
         if inputpath:
@@ -99,17 +100,17 @@
 
     return dset
 
 
 steps = [
     ProcessingStep(
         "process-aux-dsets",
-        "process_auxillary_datasets",
+        "process_auxiliary_datasets",
         preconditions=["meta_sources_parsed"],
-        precondition_error_msg="Error: You want to process the auxillary datasets, but the data from cert. framework website was not parsed. You must use 'build' action first.",
+        precondition_error_msg="Error: You want to process the auxiliary datasets, but the data from cert. framework website was not parsed. You must use 'build' action first.",
         pre_callback_func=None,
     ),
     ProcessingStep(
         "download",
         "download_all_artifacts",
         preconditions=["meta_sources_parsed"],
         precondition_error_msg="Error: You want to download all artifacts, but the data from the cert. framework website was not parsed. You must use 'build' action first.",
@@ -121,15 +122,15 @@
         preconditions=["artifacts_downloaded"],
         precondition_error_msg="Error: You want to convert pdfs -> txt, but the pdfs were not downloaded. You must use 'download' action first.",
         pre_callback_func=warn_missing_libs,
     ),
     ProcessingStep(
         "analyze",
         "analyze_certificates",
-        preconditions=["pdfs_converted", "auxillary_datasets_processed"],
+        preconditions=["pdfs_converted", "auxiliary_datasets_processed"],
         precondition_error_msg="Error: You want to process txt documents of certificates, but pdfs were not converted. You must use 'convert' action first.",
         pre_callback_func=None,
     ),
 ]
 
 
 @click.command()
@@ -154,15 +155,15 @@
 )
 @click.option(
     "-c",
     "--config",
     "configpath",
     default=None,
     type=click.Path(file_okay=True, dir_okay=False, writable=True, readable=True),
-    help="Path to your own config yaml file that will override the default one.",
+    help="Path to your own config yaml file that will override the default config.",
 )
 @click.option(
     "-i",
     "--input",
     "inputpath",
     type=click.Path(file_okay=True, dir_okay=False, writable=True, readable=True),
     help="If set, the actions will be performed on a CC dataset loaded from JSON from the input path.",
@@ -173,33 +174,33 @@
     actions: list[str],
     outputpath: Path | None,
     configpath: Path | None,
     inputpath: Path | None,
     quiet: bool,
 ):
     try:
+        if configpath:
+            try:
+                config.load_from_yaml(configpath)
+            except FileNotFoundError:
+                click.echo("Error: Bad path to configuration file", err=True)
+                sys.exit(EXIT_CODE_NOK)
+            except (ValueError, ValidationError) as e:
+                click.echo(f"Error: Bad format of configuration file: {e}", err=True)
+                sys.exit(EXIT_CODE_NOK)
+
         file_handler = logging.FileHandler(config.log_filepath)
         stream_handler = logging.StreamHandler(sys.stderr)
         formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         file_handler.setFormatter(formatter)
         stream_handler.setFormatter(formatter)
         handlers: list[logging.StreamHandler] = [file_handler] if quiet else [file_handler, stream_handler]
         logging.basicConfig(level=logging.INFO, handlers=handlers)
         start = datetime.now()
 
-        if configpath:
-            try:
-                config.load(configpath)
-            except FileNotFoundError:
-                click.echo("Error: Bad path to configuration file", err=True)
-                sys.exit(EXIT_CODE_NOK)
-            except ValueError as e:
-                click.echo(f"Error: Bad format of configuration file: {e}", err=True)
-                sys.exit(EXIT_CODE_NOK)
-
         actions_set = (
             {"build", "process-aux-dsets", "download", "convert", "analyze"} if "all" in actions else set(actions)
         )
 
         dset = build_or_load_dataset(framework, inputpath, "build" in actions_set, outputpath)
         aux_dsets_to_handle = "PP, Maintenance updates" if framework == "cc" else "Algorithms"
         aux_dsets_to_handle += "CPE, CVE"
```

### Comparing `sec-certs-0.1.3/src/sec_certs/constants.py` & `sec-certs-0.1.4/src/sec_certs/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import re
 from pathlib import Path
+from typing import Final
 
 DUMMY_NONEXISTING_PATH = Path("/this/is/dummy/nonexisting/path")
 
 RESPONSE_OK = 200
 RETURNCODE_OK = "ok"
 RETURNCODE_NOK = "nok"
-REQUEST_TIMEOUT = 10
+REQUEST_TIMEOUT = 20
+
+INCREMENTAL_NVD_UPDATE_MAX_INTERVAL_DAYS: Final[int] = 120
 
 MIN_CORRECT_CERT_SIZE = 5000
 
 MIN_FIPS_HTML_SIZE = 64000
 
 MIN_CC_HTML_SIZE = 5000000
 MIN_CC_CSV_SIZE = 700000
@@ -62,60 +65,74 @@
 GARBAGE_LINES_THRESHOLD = 30
 GARBAGE_SIZE_THRESHOLD = 1000
 GARBAGE_AVG_LLEN_THRESHOLD = 10
 GARBAGE_EVERY_SECOND_CHAR_THRESHOLD = 15
 GARBAGE_ALPHA_CHARS_THRESHOLD = 0.5
 
 CC_AUSTRALIA_BASE_URL = "https://www.cyber.gov.au"
-CC_AUSTRALIA_CERTIFIED_URL = (
-    CC_AUSTRALIA_BASE_URL + "/acsc/view-all-content/programs/australian-information-security-evaluation-program"
+CC_AUSTRALIA_INEVAL_URL = (
+    CC_AUSTRALIA_BASE_URL
+    + "/resources-business-and-government/assessment-and-evaluation-programs/australian-information-security-evaluation-program-aisep"
 )
 CC_CANADA_CERTIFIED_URL = "https://www.cyber.gc.ca/en/tools-services/common-criteria/certified-products"
 CC_CANADA_INEVAL_URL = "https://www.cyber.gc.ca/en/tools-services/common-criteria/products-evaluation"
 CC_ANSSI_BASE_URL = "https://www.ssi.gouv.fr"
 CC_ANSSI_CERTIFIED_URL = CC_ANSSI_BASE_URL + "/en/products/certified-products/"
 CC_BSI_BASE_URL = "https://www.bsi.bund.de/"
-CC_BSI_CERTIFIED_URL = CC_BSI_BASE_URL + "EN2021/Topics/Certification/certified_products/certified_products_node.html"
-CC_INDIA_CERTIFIED_URL = "https://www.commoncriteria-india.gov.in/product-certified"
-CC_INDIA_ARCHIVED_URL = "https://www.commoncriteria-india.gov.in/archived-prod-cer"
+CC_BSI_CERTIFIED_URL = (
+    CC_BSI_BASE_URL
+    + "EN/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/Zertifizierung-und-Anerkennung/Listen/Zertifizierte-Produkte-nach-CC/zertifizierte-produkte-nach-cc_node.html"
+)
+CC_INDIA_BASE_URL = "https://www.commoncriteria-india.gov.in"
+CC_INDIA_CERTIFIED_URL = CC_INDIA_BASE_URL + "/Products-Certified"
+CC_INDIA_ARCHIVED_URL = CC_INDIA_BASE_URL + "/Products-Archived"
 CC_ITALY_BASE_URL = "https://www.ocsi.gov.it"
 CC_ITALY_CERTIFIED_URL = CC_ITALY_BASE_URL + "/index.php/elenchi-certificazioni/prodotti-certificati.html"
 CC_ITALY_INEVAL_URL = CC_ITALY_BASE_URL + "/index.php/elenchi-certificazioni/in-corso-di-valutazione.html"
-CC_JAPAN_BASE_URL = "https://www.ipa.go.jp/security/jisec/jisec_e"
+CC_JAPAN_BASE_URL = "https://www.ipa.go.jp/en/security/jisec"
 CC_JAPAN_CERT_BASE_URL = CC_JAPAN_BASE_URL + "/certified_products"
-CC_JAPAN_CERTIFIED_URL = CC_JAPAN_BASE_URL + "/certified_products/certfy_list_e31.html"
-CC_JAPAN_ARCHIVED_URL = CC_JAPAN_BASE_URL + "/certified_products/certfy_list_e_archive.html"
-CC_JAPAN_INEVAL_URL = CC_JAPAN_BASE_URL + "/prdct_in_eval.html"
+CC_JAPAN_CERTIFIED_SW_URL = CC_JAPAN_BASE_URL + "/software/certified-cert/index.html"
+CC_JAPAN_CERTIFIED_HW_URL = CC_JAPAN_BASE_URL + "/hardware/certified-cert/index.html"
+CC_JAPAN_ARCHIVED_SW_URL = CC_JAPAN_BASE_URL + "/software/certified-cert/archive.html"
+CC_JAPAN_INEVAL_URL = CC_JAPAN_BASE_URL + "/prdct-in-eval/in_eval_list.html"
 CC_MALAYSIA_BASE_URL = "https://iscb.cybersecurity.my"
 CC_MALAYSIA_CERTIFIED_URL = (
-    CC_MALAYSIA_BASE_URL + "/en/index.php/certification/product-certification/mycc/certified-products-and-systems"
+    CC_MALAYSIA_BASE_URL + "/index.php/certification/product-certification/mycc/certified-products-and-systems"
 )
 CC_MALAYSIA_INEVAL_URL = (
     CC_MALAYSIA_BASE_URL
-    + "/en/index.php/certification/product-certification/mycc/list-of-products-and-systems-under-evaluation-or-maintenance"
+    + "/index.php/certification/product-certification/mycc/list-of-products-and-systems-under-evaluation-or-maintenance"
 )
 CC_NETHERLANDS_BASE_URL = "https://www.tuv-nederland.nl/common-criteria"
 CC_NETHERLANDS_CERTIFIED_URL = CC_NETHERLANDS_BASE_URL + "/certificates.html"
 CC_NETHERLANDS_INEVAL_URL = CC_NETHERLANDS_BASE_URL + "/ongoing-certifications.html"
-CC_NORWAY_CERTIFIED_URL = "https://sertit.no/certified-products/category1919.html"
-CC_NORWAY_ARCHIVED_URL = "https://sertit.no/certified-products/product-archive/"
-CC_KOREA_EN_URL = "https://itscc.kr/main/main.do?accessMode=home_en"
-CC_KOREA_CERTIFIED_URL = "https://itscc.kr/certprod/list.do"
-CC_KOREA_PRODUCT_URL = "https://itscc.kr/certprod/view.do?product_id={}&product_class=1"
+CC_NORWAY_BASE_URL = "https://sertit.no"
+CC_NORWAY_CERTIFIED_URL = CC_NORWAY_BASE_URL + "/certified-products/category1919.html"
+CC_NORWAY_ARCHIVED_URL = CC_NORWAY_BASE_URL + "/certified-products/product-archive/"
+CC_KOREA_BASE_URL = "https://itscc.kr"
+CC_KOREA_EN_URL = CC_KOREA_BASE_URL + "/main/main.do?accessMode=home_en"
+CC_KOREA_CERTIFIED_URL = CC_KOREA_BASE_URL + "/certprod/list.do"
+CC_KOREA_PRODUCT_URL = CC_KOREA_BASE_URL + "/certprod/view.do?product_id={}&product_class=1"
 CC_SINGAPORE_BASE_URL = "https://www.csa.gov.sg"
 CC_SINGAPORE_CERTIFIED_URL = (
     CC_SINGAPORE_BASE_URL + "/Programmes/certification-and-labelling-schemes/csa-common-criteria/product-list"
 )
 CC_SINGAPORE_ARCHIVED_URL = (
     CC_SINGAPORE_BASE_URL + "/Programmes/certification-and-labelling-schemes/csa-common-criteria/product-archives"
 )
+CC_SINGAPORE_API_URL = CC_SINGAPORE_BASE_URL + "/api/CsaCommonProductCriteria/getProduct"
+CC_SINGAPORE_INEVAL_URL = (
+    CC_SINGAPORE_BASE_URL
+    + "/our-programmes/certification-and-labelling-schemes/singapore-common-criteria-scheme/product-list/in-evaluation"
+)
 CC_SPAIN_BASE_URL = "https://oc.ccn.cni.es"
 CC_SPAIN_CERTIFIED_URL = CC_SPAIN_BASE_URL + "/en/certified-products/certified-products"
 CC_SWEDEN_BASE_URL = "https://www.fmv.se"
 CC_SWEDEN_CERTIFIED_URL = CC_SWEDEN_BASE_URL + "/verksamhet/ovrig-verksamhet/csec/certifikat-utgivna-av-csec/"
 CC_SWEDEN_INEVAL_URL = CC_SWEDEN_BASE_URL + "/verksamhet/ovrig-verksamhet/csec/pagaende-certifieringar/"
 CC_SWEDEN_ARCHIVED_URL = CC_SWEDEN_BASE_URL + "/verksamhet/ovrig-verksamhet/csec/arkiverade-certifikat-aldre-an-5-ar/"
 CC_TURKEY_ARCHIVED_URL = "https://statik.tse.org.tr/upload/tr/dosya/icerikyonetimi/3300/03112021143434-2.pdf"
 CC_USA_BASE_URL = "https://www.niap-ccevs.org"
+CC_USA_PRODUCT_URL = CC_USA_BASE_URL + "/Product/"
 CC_USA_CERTIFIED_URL = CC_USA_BASE_URL + "/Product/PCL.cfm"
 CC_USA_INEVAL_URL = CC_USA_BASE_URL + "/Product/PINE.cfm"
 CC_USA_ARCHIVED_URL = CC_USA_BASE_URL + "/Product/Archived.cfm"
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/__init__.py` & `sec-certs-0.1.4/src/sec_certs/dataset/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-"""This package exposes Datasets of various Samples, both primary (Common Criteria, FIPS) and auxillary (CVEs, CPEs, ...)"""
+"""This package exposes Datasets of various Samples, both primary (Common Criteria, FIPS) and auxiliary (CVEs, CPEs, ...)"""
 
-from sec_certs.dataset.cc import CCDataset, CCDatasetMaintenanceUpdates, CCSchemeDataset
+from sec_certs.dataset.cc import CCDataset, CCDatasetMaintenanceUpdates
+from sec_certs.dataset.cc_scheme import CCSchemeDataset
 from sec_certs.dataset.cpe import CPEDataset
 from sec_certs.dataset.cve import CVEDataset
 from sec_certs.dataset.fips import FIPSDataset
 from sec_certs.dataset.fips_algorithm import FIPSAlgorithmDataset
 from sec_certs.dataset.fips_iut import IUTDataset
 from sec_certs.dataset.fips_mip import MIPDataset
 from sec_certs.dataset.protection_profile import ProtectionProfileDataset
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/cpe.py` & `sec-certs-0.1.4/src/sec_certs/dataset/cve.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,197 +1,182 @@
 from __future__ import annotations
 
-import copy
 import itertools
 import logging
 import tempfile
-import xml.etree.ElementTree as ET
-import zipfile
+from datetime import datetime
 from pathlib import Path
-from typing import ClassVar, Iterator
+from typing import Any, ClassVar
 
+import numpy as np
 import pandas as pd
 
+import sec_certs.configuration as config_module
 from sec_certs import constants
-from sec_certs.dataset.cve import CVEDataset
 from sec_certs.dataset.json_path_dataset import JSONPathDataset
-from sec_certs.sample.cpe import CPE, cached_cpe
-from sec_certs.serialization.json import ComplexSerializableType, serialize
+from sec_certs.sample.cpe import CPE
+from sec_certs.sample.cve import CVE
+from sec_certs.serialization.json import ComplexSerializableType
 from sec_certs.utils import helpers
 from sec_certs.utils.tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 
 
-class CPEDataset(JSONPathDataset, ComplexSerializableType):
-    """
-    Dataset of CPE records. Includes look-up dictionaries for fast search.
-    """
-
-    CPE_XML_BASENAME: ClassVar[str] = "official-cpe-dictionary_v2.3.xml"
-    CPE_URL: ClassVar[str] = "https://nvd.nist.gov/feeds/xml/cpe/dictionary/" + CPE_XML_BASENAME + ".zip"
+class CVEDataset(JSONPathDataset, ComplexSerializableType):
+    CVE_URL: ClassVar[str] = "https://nvd.nist.gov/feeds/json/cve/1.1/nvdcve-1.1-"
+    CPE_MATCH_FEED_URL: ClassVar[str] = "https://nvd.nist.gov/feeds/json/cpematch/1.0/nvdcpematch-1.0.json.zip"
 
     def __init__(
         self,
-        was_enhanced_with_vuln_cpes: bool,
-        cpes: dict[str, CPE],
+        cves: dict[str, CVE] = {},
         json_path: str | Path = constants.DUMMY_NONEXISTING_PATH,
+        last_update_timestamp: datetime = datetime.fromtimestamp(0),
     ):
-        self.was_enhanced_with_vuln_cpes = was_enhanced_with_vuln_cpes
-        self.cpes = cpes
+        self.cves = cves
         self.json_path = Path(json_path)
+        self._cpe_uri_to_cve_ids_lookup: dict[str, set[str]] = {}
+        self._cves_with_vulnerable_configurations: list[CVE] = []
+        self.last_update_timestamp = last_update_timestamp
 
-        self.vendor_to_versions: dict[str, set[str]] = dict()
-        self.vendor_version_to_cpe: dict[tuple[str, str], set[CPE]] = dict()
-        self.title_to_cpes: dict[str, set[CPE]] = dict()
-        self.vendors: set[str] = set()
-
-        self.build_lookup_dicts()
+    def __iter__(self):
+        yield from self.cves.values()
 
-    def __iter__(self) -> Iterator[CPE]:
-        yield from self.cpes.values()
+    def __getitem__(self, item: str) -> CVE:
+        return self.cves.__getitem__(item.upper())
 
-    def __getitem__(self, item: str) -> CPE:
-        return self.cpes.__getitem__(item.lower())
-
-    def __setitem__(self, key: str, value: CPE) -> None:
-        self.cpes.__setitem__(key.lower(), value)
+    def __setitem__(self, key: str, value: CVE):
+        self.cves.__setitem__(key.upper(), value)
 
     def __len__(self) -> int:
-        return len(self.cpes)
-
-    def __contains__(self, item: CPE) -> bool:
-        if not isinstance(item, CPE):
-            raise ValueError(f"{item} is not of CPE class")
-        return item.uri in self.cpes.keys() and self.cpes[item.uri] == item
+        return len(self.cves)
 
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, CPEDataset) and self.cpes == other.cpes
+    def __eq__(self, other: object):
+        return isinstance(other, CVEDataset) and self.cves == other.cves
 
     @property
     def serialized_attributes(self) -> list[str]:
-        return ["was_enhanced_with_vuln_cpes", "cpes"]
+        return ["last_update_timestamp", "cves"]
 
-    def build_lookup_dicts(self) -> None:
-        """
-        Will build look-up dictionaries that are used for fast matching.
-        """
-        logger.info("CPE dataset: building lookup dictionaries.")
-        self.vendor_to_versions = {x.vendor: set() for x in self}
-        self.vendor_version_to_cpe = dict()
-        self.title_to_cpes = dict()
-        self.vendors = set(self.vendor_to_versions.keys())
-        for cpe in self:
-            self.vendor_to_versions[cpe.vendor].add(cpe.version)
-            if (cpe.vendor, cpe.version) not in self.vendor_version_to_cpe:
-                self.vendor_version_to_cpe[(cpe.vendor, cpe.version)] = {cpe}
-            else:
-                self.vendor_version_to_cpe[(cpe.vendor, cpe.version)].add(cpe)
-
-            if cpe.title:
-                if cpe.title not in self.title_to_cpes:
-                    self.title_to_cpes[cpe.title] = {cpe}
-                else:
-                    self.title_to_cpes[cpe.title].add(cpe)
+    @classmethod
+    def from_dict(cls, dct: dict[str, Any]) -> CVEDataset:
+        dct["last_update_timestamp"] = datetime.fromisoformat(dct["last_update_timestamp"])
+        return cls(**dct)
+
+    @property
+    def look_up_dicts_built(self) -> bool:
+        return bool(self._cpe_uri_to_cve_ids_lookup)
 
     @classmethod
-    def from_web(cls, json_path: str | Path = constants.DUMMY_NONEXISTING_PATH) -> CPEDataset:
+    def from_web(cls, json_path: str | Path = constants.DUMMY_NONEXISTING_PATH) -> CVEDataset:
         """
-        Creates CPEDataset from NIST resources published on-line
+        Creates CVEDataset from NIST resources published on-line
 
         :param Union[str, Path] json_path: Path to store the dataset to
-        :return CPEDataset: The resulting dataset
+        :return CVEDataset: The resulting dataset
         """
         with tempfile.TemporaryDirectory() as tmp_dir:
-            xml_path = Path(tmp_dir) / cls.CPE_XML_BASENAME
-            zip_path = Path(tmp_dir) / (cls.CPE_XML_BASENAME + ".zip")
-            helpers.download_file(cls.CPE_URL, zip_path)
-
-            with zipfile.ZipFile(zip_path, "r") as zip_ref:
-                zip_ref.extractall(tmp_dir)
-
-            return cls._from_xml(xml_path, json_path)
-
-    @classmethod
-    def _from_xml(cls, xml_path: str | Path, json_path: str | Path = constants.DUMMY_NONEXISTING_PATH) -> CPEDataset:
-        logger.info("Loading CPE dataset from XML.")
-        root = ET.parse(xml_path).getroot()
-        dct = {}
-        for cpe_item in root.findall("{http://cpe.mitre.org/dictionary/2.0}cpe-item"):
-            found_title = cpe_item.find("{http://cpe.mitre.org/dictionary/2.0}title")
-            if found_title is None:
-                raise RuntimeError(
-                    "Title is not found during building CPE dataset from xml - this should not be happening"
-                )
-            title = found_title.text
-
-            found_cpe_uri = cpe_item.find("{http://scap.nist.gov/schema/cpe-extension/2.3}cpe23-item")
-            if found_cpe_uri is None:
-                raise RuntimeError(
-                    "CPE uri is not found during building CPE dataset from xml - this should not be happening"
+            dset_path = Path(tmp_dir) / "cve_dataset.json.gz"
+            if (
+                not helpers.download_file(
+                    config_module.config.cve_latest_snapshot,
+                    dset_path,
+                    progress_bar_desc="Downloading CVEDataset from web",
                 )
-            cpe_uri = found_cpe_uri.attrib["name"]
-
-            dct[cpe_uri] = cached_cpe(cpe_uri, title)
-
-        return cls(False, dct, json_path)
+                == constants.RESPONSE_OK
+            ):
+                raise RuntimeError(f"Could not download CVEDataset from {config_module.config.cve_latest_snapshot}.")
+            dset = cls.from_json(dset_path, is_compressed=True)
 
-    def to_pandas(self) -> pd.DataFrame:
-        """
-        Turns the dataset into pandas DataFrame. Each CPE record forms a row.
+        dset.json_path = json_path
+        dset.to_json()
+        return dset
+
+    def _get_cves_with_criteria_configurations(self) -> None:
+        """
+        Method filters the subset of CVE dataset thah contain at least one CPE criteria configuration in the CVE.
+        """
+        self._cves_with_vulnerable_configurations = [cve for cve in self if cve.vulnerable_criteria_configurations]
+
+    def _expand_criteria_configurations(self, matching_dict: dict, relevant_cpe_uris: set[str] | None = None) -> None:
+        indices_to_delete = []
+        cve: CVE
+        for index, cve in enumerate(
+            tqdm(self._cves_with_vulnerable_configurations, desc="Expanding and filtering criteria configurations")
+        ):
+            can_be_matched = []
+            for configuration in cve.vulnerable_criteria_configurations:
+                configuration.expand_and_filter(matching_dict, relevant_cpe_uris)
+                can_be_matched.append(not any(len(component) == 0 for component in configuration._expanded_components))
+            if not any(can_be_matched):
+                indices_to_delete.append(index)
 
-        :return pd.DataFrame: the resulting DataFrame
-        """
-        df = pd.DataFrame([x.pandas_tuple for x in self], columns=CPE.pandas_columns)
-        df = df.set_index("uri")
-        return df
+        for index in sorted(indices_to_delete, reverse=True):
+            del self._cves_with_vulnerable_configurations[index]
 
-    @serialize
-    def enhance_with_cpes_from_cve_dataset(self, cve_dset: CVEDataset | str | Path) -> None:
-        """
-        Some CPEs are present only in the CVEDataset and are missing from the CPE Dataset.
-        This method goes through the provided CVEDataset and enriches self with CPEs from
-        the CVEDataset.
-
-        :param Union[CVEDataset, str, Path] cve_dset: CVEDataset of a path to it.
-        """
+    def build_lookup_dict(
+        self,
+        cpe_match_feed: dict,
+        limit_to_cpes: set[CPE] = set(),
+    ):
+        self._cpe_uri_to_cve_ids_lookup = {}
+        cpe_uris_of_interest = {x.uri for x in limit_to_cpes} if limit_to_cpes else None
+        self._get_cves_with_criteria_configurations()
+        self._expand_criteria_configurations(cpe_match_feed, cpe_uris_of_interest)
+
+        logger.info("Building lookup dictionaries.")
+        cve: CVE
+        for cve in tqdm(self, desc="Building-up lookup dictionaries for fast CVE matching"):
+            vulnerable_cpe_uris: set[str] = set()
+            for x in cve.vulnerable_criteria:
+                if x.criteria_id not in cpe_match_feed["match_strings"]:
+                    # This happens when there's no `matches` key in the original dict. In such case, the whole key got
+                    # discarded. Statistically, approx. 13% of criteria match to no CPEs and are used solely as criteria.
+                    continue
+                matches = cpe_match_feed["match_strings"][x.criteria_id]["matches"]
+                vulnerable_cpe_uris = vulnerable_cpe_uris.union(x["cpeName"] for x in matches)
 
-        def _adding_condition(
-            considered_cpe: CPE,
-            vndr_item_lookup: set[tuple[str, str]],
-            vndr_item_version_lookup: set[tuple[str, str, str]],
-        ) -> bool:
             if (
-                considered_cpe.version == constants.CPE_VERSION_NA
-                and (considered_cpe.vendor, considered_cpe.item_name) not in vndr_item_lookup
+                cpe_uris_of_interest
+                and not cve.vulnerable_criteria_configurations
+                and not any(x in cpe_uris_of_interest for x in vulnerable_cpe_uris)
             ):
-                return True
-            elif (
-                considered_cpe.version != constants.CPE_VERSION_NA
-                and (considered_cpe.vendor, considered_cpe.item_name, considered_cpe.version)
-                not in vndr_item_version_lookup
-            ):
-                return True
-            return False
-
-        if isinstance(cve_dset, (str, Path)):
-            cve_dset = CVEDataset.from_json(cve_dset)
+                continue
 
-        if not isinstance(cve_dset, CVEDataset):
-            raise RuntimeError("Conversion of CVE dataset did not work.")
-        all_cpes_in_cve_dset = set(itertools.chain.from_iterable(cve.vulnerable_cpes for cve in cve_dset))
-
-        old_len = len(self.cpes)
-
-        # We only enrich if tuple (vendor, item_name) is not already in the dataset
-        vendor_item_lookup = {(cpe.vendor, cpe.item_name) for cpe in self}
-        vendor_item_version_lookup = {(cpe.vendor, cpe.item_name, cpe.version) for cpe in self}
-        for cpe in tqdm(all_cpes_in_cve_dset, desc="Enriching CPE dataset with new CPEs"):
-            if _adding_condition(cpe, vendor_item_lookup, vendor_item_version_lookup):
-                new_cpe = copy.deepcopy(cpe)
-                new_cpe.start_version = None
-                new_cpe.end_version = None
-                self[new_cpe.uri] = new_cpe
-        self.build_lookup_dicts()
+            for cpe_uri in vulnerable_cpe_uris:
+                if not cpe_uris_of_interest or cpe_uri in cpe_uris_of_interest:
+                    self._cpe_uri_to_cve_ids_lookup.setdefault(cpe_uri, set()).add(cve.cve_id)
+
+    def _get_cves_from_exactly_matched_cpes(self, cpe_uris: set[str]) -> set[str]:
+        return set(
+            itertools.chain.from_iterable([self._cpe_uri_to_cve_ids_lookup.get(cpe_uri, set()) for cpe_uri in cpe_uris])
+        )
+
+    def _get_cves_from_criteria_configurations(self, cpe_uris: set[str]) -> set[str]:
+        return {
+            cve.cve_id
+            for cve in self._cves_with_vulnerable_configurations
+            if any(configuration.matches(cpe_uris) for configuration in cve.vulnerable_criteria_configurations)
+        }
+
+    def get_cves_from_matched_cpe_uris(self, cpe_uris: set[str]) -> set[str]:
+        """
+        Method returns the set of CVEs which are matched to the set of CPE uris.
+        """
+        return {
+            *self._get_cves_from_exactly_matched_cpes(cpe_uris),
+            *self._get_cves_from_criteria_configurations(cpe_uris),
+        }
 
-        logger.info(f"Enriched the CPE dataset with {len(self.cpes) - old_len} new CPE records.")
-        self.was_enhanced_with_vuln_cpes = True
+    def to_pandas(self) -> pd.DataFrame:
+        df = pd.DataFrame([x.pandas_tuple for x in self], columns=CVE.pandas_columns)
+        df.cwe_ids = df.cwe_ids.map(lambda x: x if x else np.nan)
+        return df.set_index("cve_id")
+
+    def enhance_with_nvd_data(self, data: dict[str, Any]) -> CVEDataset:
+        self.last_update_timestamp = datetime.fromisoformat(data["timestamp"])
+        for vuln in data["vulnerabilities"]:
+            # https://nvd.nist.gov/vuln/vulnerability-status#divNvdStatus
+            if vuln["cve"]["vulnStatus"] in {"Analyzed", "Modified"}:
+                cve = CVE.from_nist_dict(vuln["cve"])
+                self[cve.cve_id] = cve
+        return self
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/cve.py` & `sec-certs-0.1.4/src/sec_certs/utils/pdf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,219 +1,280 @@
 from __future__ import annotations
 
-import datetime
 import glob
-import itertools
-import json
 import logging
-import shutil
-import tempfile
-import zipfile
+import subprocess
+from datetime import datetime, timedelta, timezone
+from functools import reduce
 from pathlib import Path
-from typing import ClassVar
+from tempfile import TemporaryDirectory
+from typing import Any
 
-import numpy as np
-import pandas as pd
+import pdftotext
+import pikepdf
 
-import sec_certs.constants as constants
-import sec_certs.utils.helpers as helpers
-from sec_certs.dataset.json_path_dataset import JSONPathDataset
-from sec_certs.sample.cpe import CPE, cached_cpe
-from sec_certs.sample.cve import CVE
-from sec_certs.serialization.json import ComplexSerializableType
-from sec_certs.utils.parallel_processing import process_parallel
-from sec_certs.utils.tqdm import tqdm
+from sec_certs import constants
+from sec_certs.constants import (
+    GARBAGE_ALPHA_CHARS_THRESHOLD,
+    GARBAGE_AVG_LLEN_THRESHOLD,
+    GARBAGE_EVERY_SECOND_CHAR_THRESHOLD,
+    GARBAGE_LINES_THRESHOLD,
+    GARBAGE_SIZE_THRESHOLD,
+)
 
 logger = logging.getLogger(__name__)
+logging.getLogger("pypdf").setLevel(logging.ERROR)
 
 
-class CVEDataset(JSONPathDataset, ComplexSerializableType):
-    CVE_URL: ClassVar[str] = "https://nvd.nist.gov/feeds/json/cve/1.1/nvdcve-1.1-"
-    CPE_MATCH_FEED_URL: ClassVar[str] = "https://nvd.nist.gov/feeds/json/cpematch/1.0/nvdcpematch-1.0.json.zip"
-
-    def __init__(self, cves: dict[str, CVE], json_path: str | Path = constants.DUMMY_NONEXISTING_PATH):
-        self.cves = cves
-        self.json_path = Path(json_path)
-        self.cpe_to_cve_ids_lookup: dict[str, set[str]] = dict()
-
-    @property
-    def serialized_attributes(self) -> list[str]:
-        return ["cves"]
-
-    def __iter__(self):
-        yield from self.cves.values()
-
-    def __getitem__(self, item: str) -> CVE:
-        return self.cves.__getitem__(item.upper())
-
-    def __setitem__(self, key: str, value: CVE):
-        self.cves.__setitem__(key.lower(), value)
-
-    def __len__(self) -> int:
-        return len(self.cves)
-
-    def __eq__(self, other: object):
-        return isinstance(other, CVEDataset) and self.cves == other.cves
-
-    def build_lookup_dict(self, use_nist_mapping: bool = True, nist_matching_filepath: Path | None = None):
-        """
-        Builds look-up dictionary CPE -> Set[CVE]
-        Developer's note: There are 3 CPEs that are present in the cpe matching feed, but are badly processed by CVE
-        feed, in which case they won't be found as a key in the dictionary. We intentionally ignore those. Feel free
-        to add corner cases and manual fixes. According to our investigation, the suffereing CPEs are:
-            - CPE(uri='cpe:2.3:a:arubanetworks:airwave:*:*:*:*:*:*:*:*', title=None, version='*', vendor='arubanetworks', item_name='airwave', start_version=None, end_version=('excluding', '8.2.0.0'))
-            - CPE(uri='cpe:2.3:a:bayashi:dopvcomet\\*:0009:b:*:*:*:*:*:*', title=None, version='0009', vendor='bayashi', item_name='dopvcomet\\*', start_version=None, end_version=None)
-            - CPE(uri='cpe:2.3:a:bayashi:dopvstar\\*:0091:*:*:*:*:*:*:*', title=None, version='0091', vendor='bayashi', item_name='dopvstar\\*', start_version=None, end_version=None)
-        """
-        self.cpe_to_cve_ids_lookup = dict()
-        self.cves = {x.cve_id.upper(): x for x in self}
-
-        logger.info("Getting CPE matching dictionary from NIST.gov")
-
-        if use_nist_mapping:
-            matching_dict = self.get_nist_cpe_matching_dict(nist_matching_filepath)
-
-        cve: CVE
-        for cve in tqdm(self, desc="Building-up lookup dictionaries for fast CVE matching"):
-            # See note above, we use matching_dict.get(cpe, []) instead of matching_dict[cpe] as would be expected
-            if use_nist_mapping:
-                vulnerable_configurations = list(
-                    itertools.chain.from_iterable(matching_dict.get(cpe, []) for cpe in cve.vulnerable_cpes)
-                )
-            else:
-                vulnerable_configurations = cve.vulnerable_cpes
-            for cpe in vulnerable_configurations:
-                if cpe.uri not in self.cpe_to_cve_ids_lookup:
-                    self.cpe_to_cve_ids_lookup[cpe.uri] = {cve.cve_id}
-                else:
-                    self.cpe_to_cve_ids_lookup[cpe.uri].add(cve.cve_id)
-
-    @classmethod
-    def download_cves(cls, output_path_str: str, start_year: int, end_year: int):
-        output_path = Path(output_path_str)
-        if not output_path.exists():
-            output_path.mkdir()
-
-        urls = [cls.CVE_URL + str(x) + ".json.zip" for x in range(start_year, end_year + 1)]
-
-        logger.info(f"Identified {len(urls)} CVE files to fetch from nist.gov. Downloading them into {output_path}")
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            outpaths = [Path(tmp_dir) / Path(x).name.rstrip(".zip") for x in urls]
-            responses = helpers.download_parallel(urls, outpaths, "Downloading CVEs resources from NVD")
-
-            for o, r in zip(outpaths, responses):
-                if r == constants.RESPONSE_OK:
-                    with zipfile.ZipFile(o, "r") as zip_handle:
-                        zip_handle.extractall(output_path)
-
-    @classmethod
-    def from_nist_json(cls, input_path: str) -> CVEDataset:
-        with Path(input_path).open("r") as handle:
-            data = json.load(handle)
-        cves = [CVE.from_nist_dict(x) for x in data["CVE_Items"]]
-        return cls({x.cve_id: x for x in cves})
-
-    @classmethod
-    def from_web(
-        cls,
-        start_year: int = 2002,
-        end_year: int = datetime.datetime.now().year,
-        json_path: str | Path = constants.DUMMY_NONEXISTING_PATH,
-    ):
-        logger.info("Building CVE dataset from nist.gov website.")
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            cls.download_cves(tmp_dir, start_year, end_year)
-            json_files = glob.glob(tmp_dir + "/*.json")
-
-            all_cves = dict()
-            logger.info("Downloaded required resources. Building CVEDataset from jsons.")
-            results = process_parallel(
-                cls.from_nist_json,
-                json_files,
-                use_threading=False,
-                progress_bar_desc="Building CVEDataset from jsons",
+def repair_pdf(file: Path) -> None:
+    """
+    Some pdfs can't be opened by PyPDF2 - opening them with pikepdf and then saving them fixes this issue.
+    By opening this file in a pdf reader, we can already extract number of pages.
+
+    :param file: file name
+    :return: number of pages in pdf file
+    """
+    pdf = pikepdf.Pdf.open(file, allow_overwriting_input=True)
+    pdf.save(file)
+
+
+def ocr_pdf_file(pdf_path: Path) -> str:
+    """
+    OCR a PDF file and return its text contents, uses `pdftoppm` and `tesseract`.
+
+    :param pdf_path: The PDF file to OCR.
+    :return: The text contents.
+    """
+    with TemporaryDirectory() as tmpdir:
+        tmppath = Path(tmpdir)
+        ppm = subprocess.run(
+            ["pdftoppm", pdf_path, tmppath / "image"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+        )
+        if ppm.returncode != 0:
+            raise ValueError(f"pdftoppm failed: {ppm.returncode}")
+        for ppm_path in map(Path, glob.glob(str(tmppath / "image*.ppm"))):
+            base = ppm_path.with_suffix("")
+            tes = subprocess.run(
+                ["tesseract", "-l", "eng+deu+fra", ppm_path, base], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
             )
-            for r in results:
-                all_cves.update(r.cves)
-
-        return cls(all_cves, json_path)
+            if tes.returncode != 0:
+                raise ValueError(f"tesseract failed: {tes.returncode}")
 
-    def get_cve_ids_for_cpe_uri(self, cpe_uri: str) -> set[str] | None:
-        return self.cpe_to_cve_ids_lookup.get(cpe_uri, None)
+        contents = ""
 
-    def filter_related_cpes(self, relevant_cpes: set[CPE]):
-        """
-        Since each of the CVEs is related to many CPEs, the dataset size explodes (serialized). For certificates,
-        only CPEs within sample dataset are relevant. This function modifies all CVE elements. Specifically, it
-        deletes all CPE records unless they are part of relevant_cpe_uris.
-        :param relevant_cpes: List of relevant CPEs to keep in CVE dataset.
-        """
-        total_deleted_cpes = 0
-        cve_ids_to_delete = []
-        for cve in self:
-            n_cpes_orig = len(cve.vulnerable_cpes)
-            cve.vulnerable_cpes = list(filter(lambda x: x in relevant_cpes, cve.vulnerable_cpes))
-            total_deleted_cpes += n_cpes_orig - len(cve.vulnerable_cpes)
-            if not cve.vulnerable_cpes:
-                cve_ids_to_delete.append(cve.cve_id)
-
-        for cve_id in cve_ids_to_delete:
-            del self.cves[cve_id]
-        logger.info(
-            f"Totally deleted {total_deleted_cpes} irrelevant CPEs and {len(cve_ids_to_delete)} CVEs from CVEDataset."
-        )
+        txt_paths = [x for x in tmppath.iterdir() if x.is_file() and "image-" in x.stem and x.suffix == ".txt"]
+        txt_paths = sorted(txt_paths, key=lambda txt_path: int(txt_path.stem.split("-")[1]))
 
-    def to_pandas(self) -> pd.DataFrame:
-        df = pd.DataFrame([x.pandas_tuple for x in self], columns=CVE.pandas_columns)
-        df.cwe_ids = df.cwe_ids.map(lambda x: x if x else np.nan)
-        return df.set_index("cve_id")
-
-    def get_nist_cpe_matching_dict(self, input_filepath: Path | None) -> dict[CPE, list[CPE]]:
-        """
-        Computes dictionary that maps complex CPEs to list of simple CPEs.
-        """
-
-        def parse_key_cpe(field: dict) -> CPE:
-            start_version = None
-            if "versionStartIncluding" in field:
-                start_version = ("including", field["versionStartIncluding"])
-            elif "versionStartExcluding" in field:
-                start_version = ("excluding", field["versionStartExcluding"])
-
-            end_version = None
-            if "versionEndIncluding" in field:
-                end_version = ("including", field["versionEndIncluding"])
-            elif "versionEndExcluding" in field:
-                end_version = ("excluding", field["versionEndExcluding"])
-
-            return cached_cpe(field["cpe23Uri"], start_version=start_version, end_version=end_version)
-
-        def parse_values_cpe(field: dict) -> list[CPE]:
-            return [cached_cpe(x["cpe23Uri"]) for x in field["cpe_name"]]
-
-        logger.debug("Attempting to get NIST mapping file.")
-        if not input_filepath or not input_filepath.is_file():
-            logger.debug("NIST mapping file not available, going to download.")
-            with tempfile.TemporaryDirectory() as tmp_dir:
-                filename = Path(self.CPE_MATCH_FEED_URL).name
-                download_path = Path(tmp_dir) / filename
-                unzipped_path = Path(tmp_dir) / filename.rstrip(".zip")
-                helpers.download_file(self.CPE_MATCH_FEED_URL, download_path)
-
-                with zipfile.ZipFile(download_path, "r") as zip_handle:
-                    zip_handle.extractall(tmp_dir)
-                with unzipped_path.open("r") as handle:
-                    match_data = json.load(handle)
-                if input_filepath:
-                    logger.debug(f"Copying attained NIST mapping file to {input_filepath}")
-                    shutil.move(str(unzipped_path), str(input_filepath))
+        for txt_path in txt_paths:
+            with txt_path.open("r", encoding="utf-8") as f:
+                contents += f.read()
+    return contents
+
+
+def convert_pdf_file(pdf_path: Path, txt_path: Path) -> tuple[bool, bool]:
+    """
+    Convert a PDF tile to text and save it on the `txt_path`.
+
+    :param pdf_path: Path to the to-be-converted PDF file.
+    :param txt_path: Path to the resulting text file.
+    :return: A tuple of two results, whether OCR was done and what the complete result
+             was (OK/NOK).
+    """
+    txt = None
+    ok = False
+    ocr = False
+    try:
+        with pdf_path.open("rb") as pdf_handle:
+            pdf = pdftotext.PDF(pdf_handle, "", True)  # No password, Raw=True
+            txt = "".join(pdf)
+    except Exception as e:
+        logger.error(f"Error when converting pdf->txt: {e}")
+
+    if txt is None or text_is_garbage(txt):
+        logger.warning(f"Detected garbage during conversion of {pdf_path}")
+        ocr = True
+        try:
+            txt = ocr_pdf_file(pdf_path)
+            logger.info(f"OCR OK for {pdf_path}")
+        except Exception as e:
+            logger.error(f"Error during OCR of {pdf_path}, using garbage: {e}")
+
+    if txt is not None:
+        ok = True
+        with txt_path.open("w", encoding="utf-8") as txt_handle:
+            txt_handle.write(txt)
+
+    return ocr, ok
+
+
+def parse_pdf_date(dateval: bytes | None) -> datetime | None:
+    """
+    Parse PDF metadata date format:
+
+    ```
+        parse_pdf_date(b"D:20110617082321-04'00'")
+    ```
+    into
+    ```
+        datetime.datetime(2011, 6, 17, 8, 23, 21, tzinfo=datetime.timezone(datetime.timedelta(days=-1, seconds=72000)))
+    ```
+
+    :param dateval: The date as in the PDF metadata.
+    :return: The parsed datetime, if successful, else `None`.
+    """
+    if dateval is None:
+        return None
+    clean = dateval.decode("utf-8").replace("D:", "")
+    tz = None
+    tzoff = None
+    if "+" in clean:
+        clean, tz = clean.split("+")
+        tzoff = 1
+    if "-" in clean:
+        clean, tz = clean.split("-")
+        tzoff = -1
+    elif "Z" in clean:
+        clean, tz = clean.split("Z")
+        tzoff = 1
+    try:
+        res_datetime = datetime.strptime(clean, "%Y%m%d%H%M%S")
+        if tz and tzoff:
+            tz_datetime = datetime.strptime(tz, "%H'%M'")
+            delta = tzoff * timedelta(hours=tz_datetime.hour, minutes=tz_datetime.minute)
+            res_tz = timezone(delta)
+            res_datetime = res_datetime.replace(tzinfo=res_tz)
+        return res_datetime
+    except ValueError:
+        return None
+
+
+def extract_pdf_metadata(filepath: Path) -> tuple[str, dict[str, Any] | None]:  # noqa: C901
+    """
+    Extract PDF metadata, such as the number of pages, author, title, etc.
+
+    :param filepath: THe path to the PDF.
+    :return: A tuple of the result code (see constants) and the metadata dictionary.
+    """
+    from pypdf import PdfReader
+    from pypdf.generic import (
+        BooleanObject,
+        ByteStringObject,
+        FloatObject,
+        IndirectObject,
+        NumberObject,
+        TextStringObject,
+    )
+
+    def map_metadata_value(val, nope_out=False):
+        if isinstance(val, BooleanObject):
+            val = val.value
+        elif isinstance(val, FloatObject):
+            val = float(val)
+        elif isinstance(val, NumberObject):
+            val = int(val)
+        elif isinstance(val, IndirectObject) and not nope_out:
+            # Let's make sure to nope out in case of cycles
+            val = map_metadata_value(val.get_object(), nope_out=True)
+        elif isinstance(val, TextStringObject):
+            val = str(val)
+        elif isinstance(val, ByteStringObject):
+            try:
+                val = val.decode("utf-8")
+            except UnicodeDecodeError:
+                val = str(val)
         else:
-            with input_filepath.open("r") as handle:
-                match_data = json.load(handle)
-
-        mapping_dict = dict()
-        for match in tqdm(match_data["matches"], desc="parsing cpe matching (by NIST) dictionary"):
-            key = parse_key_cpe(match)
-            value = parse_values_cpe(match)
-            mapping_dict[key] = value if value else [key]
+            val = str(val)
+        return val
 
-        return mapping_dict
+    def resolve_indirect(val, bound=10):
+        if isinstance(val, list) and bound:
+            return [resolve_indirect(v, bound - 1) for v in val]
+        if isinstance(val, IndirectObject) and bound:
+            return resolve_indirect(val.get_object(), bound - 1)
+        return val
+
+    metadata: dict[str, Any] = {}
+
+    try:
+        metadata["pdf_file_size_bytes"] = filepath.stat().st_size
+        with filepath.open("rb") as handle:
+            pdf = PdfReader(handle, strict=False)
+            metadata["pdf_is_encrypted"] = pdf.is_encrypted
+
+        # see https://stackoverflow.com/questions/26242952/pypdf-2-decrypt-not-working
+        if metadata["pdf_is_encrypted"]:
+            pikepdf.open(filepath, allow_overwriting_input=True).save()
+
+        with filepath.open("rb") as handle:
+            pdf = PdfReader(handle, strict=False)
+            metadata["pdf_number_of_pages"] = len(pdf.pages)
+            pdf_document_info = pdf.metadata
+
+            if pdf_document_info is None:
+                raise ValueError("PDF metadata unavailable")
+
+            for key, val in pdf_document_info.items():
+                metadata[str(key)] = map_metadata_value(val)
+
+            # Get the hyperlinks in the PDF
+            annots = [page.get("/Annots", []) for page in pdf.pages]
+            annots = reduce(lambda x, y: x + y, map(resolve_indirect, annots))
+            links = set()
+            for annot in annots:
+                try:
+                    A = resolve_indirect(annot.get("/A", {}))
+                    link = resolve_indirect(A.get("/URI"))
+                    if link:
+                        links.add(map_metadata_value(link))
+                except Exception:
+                    pass
+            metadata["pdf_hyperlinks"] = links
+
+    except Exception as e:
+        relative_filepath = "/".join(str(filepath).split("/")[-4:])
+        error_msg = f"Failed to read metadata of {relative_filepath}, error: {e}"
+        logger.error(error_msg)
+        return error_msg, None
+
+    return constants.RETURNCODE_OK, metadata
+
+
+def text_is_garbage(text: str) -> bool:
+    """
+    Detect whether the given text is "garbage". A series of tests is applied,
+    using the number of lines, average line length, total size, every second character on a line
+    and the ratio of alphanumeric characters.
+
+    :param text: The tested text.
+    :return: Whether the text is a "garbage" result of pdftotext conversion.
+    """
+    size = len(text)
+    content_len = 0
+    lines = 0
+    every_second = 0
+    alpha_len = len("".join(filter(str.isalpha, text)))
+    for line in text.splitlines():
+        content_len += len(line)
+        lines += 1
+        if len(set(line[1::2])) > 1:
+            every_second += 1
+
+    avg_line_len = content_len / lines if lines else 0
+    alpha = alpha_len / size if size else 0
+
+    # If number of lines is small, this is garbage.
+    if lines < GARBAGE_LINES_THRESHOLD:
+        return True
+    # If the file size is small, this is garbage.
+    if size < GARBAGE_SIZE_THRESHOLD:
+        return True
+    # If the average length of a line is small, this is garbage.
+    if avg_line_len < GARBAGE_AVG_LLEN_THRESHOLD:
+        return True
+    # If there a small amount of lines that have more than one character at every second character, this is garbage.
+    # This detects the ANSSI spacing issues.
+    if every_second < GARBAGE_EVERY_SECOND_CHAR_THRESHOLD:
+        return True
+    # If there is a small ratio of alphanumeric chars to all chars, this is garbage.
+    if alpha < GARBAGE_ALPHA_CHARS_THRESHOLD:
+        return True
+    return False
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/dataset.py` & `sec-certs-0.1.4/src/sec_certs/dataset/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,85 @@
 from __future__ import annotations
 
+import gzip
 import itertools
 import json
 import logging
 import re
 import shutil
 import tempfile
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Generic, Iterator, TypeVar, cast
 
 import pandas as pd
 
-import sec_certs.constants as constants
-import sec_certs.utils.helpers as helpers
-from sec_certs.config.configuration import config
+from sec_certs import constants
+from sec_certs.configuration import config
 from sec_certs.dataset.cpe import CPEDataset
 from sec_certs.dataset.cve import CVEDataset
 from sec_certs.model.cpe_matching import CPEClassifier
 from sec_certs.sample.certificate import Certificate
 from sec_certs.sample.cpe import CPE
 from sec_certs.serialization.json import ComplexSerializableType, get_class_fullname, serialize
+from sec_certs.utils import helpers
+from sec_certs.utils.nvd_dataset_builder import CpeMatchNvdDatasetBuilder, CpeNvdDatasetBuilder, CveNvdDatasetBuilder
 from sec_certs.utils.tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
-class AuxillaryDatasets:
+class AuxiliaryDatasets:
     cpe_dset: CPEDataset | None = None
     cve_dset: CVEDataset | None = None
 
 
 CertSubType = TypeVar("CertSubType", bound=Certificate)
-AuxillaryDatasetsSubType = TypeVar("AuxillaryDatasetsSubType", bound=AuxillaryDatasets)
+AuxiliaryDatasetsSubType = TypeVar("AuxiliaryDatasetsSubType", bound=AuxiliaryDatasets)
 DatasetSubType = TypeVar("DatasetSubType", bound="Dataset")
 
 
-class Dataset(Generic[CertSubType, AuxillaryDatasetsSubType], ComplexSerializableType, ABC):
+class Dataset(Generic[CertSubType, AuxiliaryDatasetsSubType], ComplexSerializableType, ABC):
     """
     Base class for dataset of certificates from CC and FIPS 140 schemes. Layouts public
     functions, the processing pipeline and common operations on the dataset and certs.
     """
 
     @dataclass
     class DatasetInternalState(ComplexSerializableType):
         meta_sources_parsed: bool = False
         artifacts_downloaded: bool = False
         pdfs_converted: bool = False
-        auxillary_datasets_processed: bool = False
+        auxiliary_datasets_processed: bool = False
         certs_analyzed: bool = False
 
-        def __bool__(self):
-            return any(vars(self))
-
     def __init__(
         self,
-        certs: dict[str, CertSubType] = dict(),
+        certs: dict[str, CertSubType] = {},
         root_dir: str | Path = constants.DUMMY_NONEXISTING_PATH,
         name: str | None = None,
         description: str = "",
         state: DatasetInternalState | None = None,
-        auxillary_datasets: AuxillaryDatasetsSubType | None = None,
+        auxiliary_datasets: AuxiliaryDatasetsSubType | None = None,
     ):
         self.certs = certs
 
         self.timestamp = datetime.now()
         self.sha256_digest = "not implemented"
         self.name = name if name else type(self).__name__.lower() + "_dataset"
         self.description = description if description else "No description provided"
         self.state = state if state else self.DatasetInternalState()
 
-        if not auxillary_datasets:
-            self.auxillary_datasets = AuxillaryDatasets()
+        if not auxiliary_datasets:
+            self.auxiliary_datasets = AuxiliaryDatasets()
         else:
-            self.auxillary_datasets = auxillary_datasets
+            self.auxiliary_datasets = auxiliary_datasets
 
         self.root_dir = Path(root_dir)
 
     @property
     def root_dir(self) -> Path:
         """
         Directory that will hold the serialized dataset files.
@@ -104,38 +103,42 @@
     def web_dir(self) -> Path:
         """
         Path to certification-artifacts posted on web.
         """
         return self.root_dir / "web"
 
     @property
-    def auxillary_datasets_dir(self) -> Path:
+    def auxiliary_datasets_dir(self) -> Path:
         """
-        Path to directory with auxillary datasets.
+        Path to directory with auxiliary datasets.
         """
-        return self.root_dir / "auxillary_datasets"
+        return self.root_dir / "auxiliary_datasets"
 
     @property
     def certs_dir(self) -> Path:
         """
         Returns directory that holds files associated with certificates
         """
         return self.root_dir / "certs"
 
     @property
     def cpe_dataset_path(self) -> Path:
-        return self.auxillary_datasets_dir / "cpe_dataset.json"
+        return self.auxiliary_datasets_dir / "cpe_dataset.json"
+
+    @property
+    def cpe_match_json_path(self) -> Path:
+        return self.auxiliary_datasets_dir / "cpe_match_feed.json"
 
     @property
     def cve_dataset_path(self) -> Path:
-        return self.auxillary_datasets_dir / "cve_dataset.json"
+        return self.auxiliary_datasets_dir / "cve_dataset.json"
 
     @property
     def nist_cve_cpe_matching_dset_path(self) -> Path:
-        return self.auxillary_datasets_dir / "nvdcpematch-1.0.json"
+        return self.auxiliary_datasets_dir / "nvdcpematch-1.0.json"
 
     @property
     def json_path(self) -> Path:
         return self.root_dir / (self.name + ".json")
 
     def __contains__(self, item: object) -> bool:
         if not isinstance(item, Certificate):
@@ -194,25 +197,25 @@
         if len(dset) != (claimed := dct["n_certs"]):
             logger.error(
                 f"The actual number of certs in dataset ({len(dset)}) does not match the claimed number ({claimed})."
             )
         return dset
 
     @classmethod
-    def from_json(cls: type[DatasetSubType], input_path: str | Path) -> DatasetSubType:
-        dset = cast("DatasetSubType", ComplexSerializableType.from_json(input_path))
+    def from_json(cls: type[DatasetSubType], input_path: str | Path, is_compressed: bool = False) -> DatasetSubType:
+        dset = cast("DatasetSubType", ComplexSerializableType.from_json(input_path, is_compressed))
         dset._root_dir = Path(input_path).parent.absolute()
         dset._set_local_paths()
         return dset
 
     def _set_local_paths(self) -> None:
-        if self.auxillary_datasets.cpe_dset:
-            self.auxillary_datasets.cpe_dset.json_path = self.cpe_dataset_path
-        if self.auxillary_datasets.cve_dset:
-            self.auxillary_datasets.cve_dset.json_path = self.cve_dataset_path
+        if self.auxiliary_datasets.cpe_dset:
+            self.auxiliary_datasets.cpe_dset.json_path = self.cpe_dataset_path
+        if self.auxiliary_datasets.cve_dset:
+            self.auxiliary_datasets.cve_dset.json_path = self.cve_dataset_path
 
     def move_dataset(self, new_root_dir: str | Path) -> None:
         """
         Moves all dataset files to `new_root_dir` and adjusts all paths internally. Deletes the artifacts from the original location.
         :param str | Path new_root_dir: path to directory where the new dataset shall be stored.
         """
         new_root_dir = Path(new_root_dir)
@@ -245,23 +248,27 @@
 
     @abstractmethod
     def get_certs_from_web(self) -> None:
         raise NotImplementedError("Not meant to be implemented by the base class.")
 
     @serialize
     @abstractmethod
-    def process_auxillary_datasets(self, download_fresh: bool = False) -> None:
+    def process_auxiliary_datasets(self, download_fresh: bool = False) -> None:
         """
-        Processes all auxillary datasets (CPE, CVE, ...) that are required during computation.
+        Processes all auxiliary datasets (CPE, CVE, ...) that are required during computation.
         """
-        logger.info("Processing auxillary datasets.")
-        self.auxillary_datasets_dir.mkdir(parents=True, exist_ok=True)
-        self.auxillary_datasets.cpe_dset = self._prepare_cpe_dataset(download_fresh)
-        self.auxillary_datasets.cve_dset = self._prepare_cve_dataset(download_fresh_cves=download_fresh)
-        self.state.auxillary_datasets_processed = True
+        logger.info("Processing auxiliary datasets.")
+        self.auxiliary_datasets_dir.mkdir(parents=True, exist_ok=True)
+        self.auxiliary_datasets.cpe_dset = self._prepare_cpe_dataset(download_fresh)
+        self.auxiliary_datasets.cve_dset = self._prepare_cve_dataset(download_fresh)
+
+        if download_fresh or not self.cpe_match_json_path.exists():
+            self._prepare_cpe_match_dict(download_fresh=download_fresh)
+
+        self.state.auxiliary_datasets_processed = True
 
     @serialize
     def download_all_artifacts(self, fresh: bool = True) -> None:
         """
         Downloads all artifacts related to certification in the given scheme.
         """
         if not self.state.meta_sources_parsed:
@@ -307,17 +314,17 @@
             - Computes various heuristics on the certificates.
         """
         if not self.state.pdfs_converted:
             logger.info(
                 "Attempting run analysis of txt files while not having the pdf->txt conversion done. Returning."
             )
             return
-        if not self.state.auxillary_datasets_processed:
+        if not self.state.auxiliary_datasets_processed:
             logger.info(
-                "Attempting to run analysis of certifies while not having the auxillary datasets processed. Returning."
+                "Attempting to run analysis of certifies while not having the auxiliary datasets processed. Returning."
             )
 
         logger.info("Analyzing certificates.")
         self._analyze_certificates_body()
         self.state.certs_analyzed = True
 
     def _analyze_certificates_body(self) -> None:
@@ -339,107 +346,156 @@
     def _compute_references(self) -> None:
         raise NotImplementedError("Not meant to be implemented by the base class.")
 
     @abstractmethod
     def _compute_transitive_vulnerabilities(self) -> None:
         raise NotImplementedError("Not meant to be implemented by the base class.")
 
-    def _prepare_cpe_dataset(self, download_fresh_cpes: bool = False) -> CPEDataset:
-        logger.info("Preparing CPE dataset.")
-        if not self.auxillary_datasets_dir.exists():
-            self.auxillary_datasets_dir.mkdir(parents=True)
+    def _prepare_cpe_dataset(self, download_fresh: bool = False) -> CPEDataset:
+        if not self.auxiliary_datasets_dir.exists():
+            self.auxiliary_datasets_dir.mkdir(parents=True)
+
+        if self.cpe_dataset_path.exists():
+            logger.info("Preparing CPEDataset from json.")
+            cpe_dataset = CPEDataset.from_json(self.cpe_dataset_path)
+        else:
+            cpe_dataset = CPEDataset(json_path=self.cpe_dataset_path)
+            download_fresh = True
 
-        if not self.cpe_dataset_path.exists() or download_fresh_cpes is True:
-            cpe_dataset = CPEDataset.from_web(self.cpe_dataset_path)
+        if download_fresh:
+            if config.preferred_source_nvd_datasets == "api":
+                logger.info("Fetching new CPE records from NVD API.")
+                with CpeNvdDatasetBuilder(api_key=config.nvd_api_key) as builder:
+                    cpe_dataset = builder.build_dataset(cpe_dataset)
+            else:
+                logger.info("Preparing CPEDataset from seccerts.org.")
+                cpe_dataset = CPEDataset.from_web(self.cpe_dataset_path)
             cpe_dataset.to_json()
-        else:
-            cpe_dataset = CPEDataset.from_json(str(self.cpe_dataset_path))
 
         return cpe_dataset
 
-    def _prepare_cve_dataset(
-        self, download_fresh_cves: bool = False, use_nist_cpe_matching_dict: bool = True
-    ) -> CVEDataset:
-        logger.info("Preparing CVE dataset.")
-        if not self.auxillary_datasets_dir.exists():
-            self.auxillary_datasets_dir.mkdir(parents=True)
+    def _prepare_cve_dataset(self, download_fresh: bool = False) -> CVEDataset:
+        if not self.auxiliary_datasets_dir.exists():
+            logger.info("Loading CVEDataset from json.")
+            self.auxiliary_datasets_dir.mkdir(parents=True)
 
-        if not self.cve_dataset_path.exists() or download_fresh_cves is True:
-            cve_dataset = CVEDataset.from_web(json_path=self.cve_dataset_path)
-            cve_dataset.to_json()
-        else:
+        if self.cve_dataset_path.exists():
+            logger.info("Preparing CVEDataset from json.")
             cve_dataset = CVEDataset.from_json(self.cve_dataset_path)
+        else:
+            cve_dataset = CVEDataset(json_path=self.cve_dataset_path)
+            download_fresh = True
+
+        if download_fresh:
+            if config.preferred_source_nvd_datasets == "api":
+                logger.info("Fetching new CVE records from NVD API.")
+                with CveNvdDatasetBuilder(api_key=config.nvd_api_key) as builder:
+                    cve_dataset = builder.build_dataset(cve_dataset)
+            else:
+                logger.info("Preparing CVEDataset from seccerts.org")
+                cve_dataset = CVEDataset.from_web(self.cve_dataset_path)
+            cve_dataset.to_json()
 
-        cve_dataset.build_lookup_dict(use_nist_cpe_matching_dict, self.nist_cve_cpe_matching_dset_path)
         return cve_dataset
 
+    def _prepare_cpe_match_dict(self, download_fresh: bool = False) -> dict:
+        if self.cpe_match_json_path.exists():
+            logger.info("Preparing CPE Match feed from json.")
+            with self.cpe_match_json_path.open("r") as handle:
+                cpe_match_dict = json.load(handle)
+        else:
+            cpe_match_dict = CpeMatchNvdDatasetBuilder._init_new_dataset()
+            download_fresh = True
+
+        if download_fresh:
+            if config.preferred_source_nvd_datasets == "api":
+                logger.info("Fetchnig CPE Match feed from NVD APi.")
+                with CpeMatchNvdDatasetBuilder(api_key=config.nvd_api_key) as builder:
+                    cpe_match_dict = builder.build_dataset(cpe_match_dict)
+            else:
+                logger.info("Preparing CPE Match feed from seccerts.org.")
+                with tempfile.TemporaryDirectory() as tmp_dir:
+                    dset_path = Path(tmp_dir) / "cpe_match_feed.json.gz"
+                    if (
+                        not helpers.download_file(
+                            config.cpe_match_latest_snapshot,
+                            dset_path,
+                            progress_bar_desc="Downloading CPE Match feed from web",
+                        )
+                        == constants.RESPONSE_OK
+                    ):
+                        raise RuntimeError(
+                            f"Could not download CPE Match feed from {config.cpe_match_latest_snapshot}."
+                        )
+                    with gzip.open(str(dset_path)) as handle:
+                        json_str = handle.read().decode("utf-8")
+                        cpe_match_dict = json.loads(json_str)
+            with self.cpe_match_json_path.open("w") as handle:
+                json.dump(cpe_match_dict, handle, indent=4)
+
+        return cpe_match_dict
+
     @serialize
-    def compute_cpe_heuristics(self, download_fresh_cpes: bool = False) -> CPEClassifier:
+    def compute_cpe_heuristics(self) -> CPEClassifier:
         """
         Computes matching CPEs for the certificates.
         """
         WINDOWS_WEAK_CPES: set[CPE] = {
-            CPE("cpe:2.3:o:microsoft:windows:-:*:*:*:*:*:x64:*", "Microsoft Windows on X64", None, None),
-            CPE("cpe:2.3:o:microsoft:windows:-:*:*:*:*:*:x86:*", "Microsoft Windows on X86", None, None),
+            CPE("", "cpe:2.3:o:microsoft:windows:-:*:*:*:*:*:x64:*", "Microsoft Windows on X64"),
+            CPE("", "cpe:2.3:o:microsoft:windows:-:*:*:*:*:*:x86:*", "Microsoft Windows on X86"),
         }
 
         def filter_condition(cpe: CPE) -> bool:
             """
             Filters out very weak CPE matches that don't improve our database.
             """
             if (
                 cpe.title
                 and (cpe.version == "-" or cpe.version == "*")
                 and not any(char.isdigit() for char in cpe.title)
             ):
                 return False
-            elif (
+            if (
                 not cpe.title
                 and cpe.item_name
                 and (cpe.version == "-" or cpe.version == "*")
                 and not any(char.isdigit() for char in cpe.item_name)
             ):
                 return False
-            elif re.match(constants.RELEASE_CANDIDATE_REGEX, cpe.update):
+            if re.match(constants.RELEASE_CANDIDATE_REGEX, cpe.update):
                 return False
-            elif cpe in WINDOWS_WEAK_CPES:
+            if cpe in WINDOWS_WEAK_CPES:
                 return False
             return True
 
         logger.info("Computing heuristics: Finding CPE matches for certificates")
-        if not self.auxillary_datasets.cpe_dset or download_fresh_cpes:
-            self.auxillary_datasets.cpe_dset = self._prepare_cpe_dataset(download_fresh_cpes)
-
-        # Temporarily disabled, see: https://github.com/crocs-muni/sec-certs/issues/173
-        # if not cpe_dset.was_enhanced_with_vuln_cpes:
-        #     self.auxillary_datasets.cve_dset = self._prepare_cve_dataset(download_fresh_cves=False)
-        #     self.auxillary_datasets.cpe_dset.enhance_with_cpes_from_cve_dataset(cve_dset)  # this also calls build_lookup_dicts() on cpe_dset
-        # else:
-        #     self.auxillary_datasets.cpe_dset.build_lookup_dicts()
+        if not self.auxiliary_datasets.cpe_dset:
+            self.auxiliary_datasets.cpe_dset = self._prepare_cpe_dataset()
 
         clf = CPEClassifier(config.cpe_matching_threshold, config.cpe_n_max_matches)
-        clf.fit([x for x in self.auxillary_datasets.cpe_dset if filter_condition(x)])
+        clf.fit([x for x in self.auxiliary_datasets.cpe_dset if filter_condition(x)])
 
         cert: CertSubType
         for cert in tqdm(self, desc="Predicting CPE matches with the classifier"):
             cert.compute_heuristics_version()
 
             cert.heuristics.cpe_matches = (
                 clf.predict_single_cert(cert.manufacturer, cert.name, cert.heuristics.extracted_versions)
                 if cert.name
                 else None
             )
 
         return clf
 
+    @serialize
     def to_label_studio_json(self, output_path: str | Path) -> None:
         cpe_dset = self._prepare_cpe_dataset()
 
         lst = []
-        for cert in [x for x in cast(Iterator[Certificate], self) if x.heuristics.cpe_matches]:
+        for cert in [x for x in self if x.heuristics.cpe_matches]:
             dct = {"text": cert.label_studio_title}
             candidates = [cpe_dset[x].title for x in cert.heuristics.cpe_matches]
             candidates += ["No good match"] * (config.cpe_n_max_matches - len(candidates))
             options = ["option_" + str(x) for x in range(1, config.cpe_n_max_matches)]
             dct.update({o: c for o, c in zip(options, candidates)})
             lst.append(dct)
 
@@ -448,38 +504,37 @@
 
     @serialize
     def load_label_studio_labels(self, input_path: str | Path) -> set[str]:
         with Path(input_path).open("r") as handle:
             data = json.load(handle)
 
         cpe_dset = self._prepare_cpe_dataset()
+        title_to_cpes_dict = cpe_dset.get_title_to_cpes_dict()
         labeled_cert_digests: set[str] = set()
 
         logger.info("Translating label studio matches into their CPE representations and assigning to certificates.")
         for annotation in tqdm(data, desc="Translating label studio matches"):
-            cpe_candidate_keys = {
-                key for key in annotation.keys() if "option_" in key and annotation[key] != "No good match"
-            }
+            cpe_candidate_keys = {key for key in annotation if "option_" in key and annotation[key] != "No good match"}
 
             if "verified_cpe_match" not in annotation:
                 incorrect_keys: set[str] = set()
             elif isinstance(annotation["verified_cpe_match"], str):
                 incorrect_keys = {annotation["verified_cpe_match"]}
             else:
                 incorrect_keys = set(annotation["verified_cpe_match"]["choices"])
 
             incorrect_keys = {x.lstrip("$") for x in incorrect_keys}
             predicted_annotations = {annotation[x] for x in cpe_candidate_keys - incorrect_keys}
 
             cpes: set[CPE] = set()
             for x in predicted_annotations:
-                if x not in cpe_dset.title_to_cpes:
+                if x not in title_to_cpes_dict:
                     logger.error(f"{x} not in dataset")
                 else:
-                    to_update = cpe_dset.title_to_cpes[x]
+                    to_update = title_to_cpes_dict[x]
                     if to_update and not cpes:
                         cpes = to_update
                     elif to_update and cpes:
                         cpes.update(to_update)
 
             # distinguish between FIPS and CC
             if "\n" in annotation["text"]:
@@ -503,55 +558,58 @@
             if not cert.heuristics.cpe_matches and cert.heuristics.verified_cpe_matches:
                 cert.heuristics.cpe_matches = cert.heuristics.verified_cpe_matches
             elif cert.heuristics.cpe_matches and cert.heuristics.verified_cpe_matches:
                 cert.heuristics.cpe_matches = set(cert.heuristics.cpe_matches).union(
                     set(cert.heuristics.verified_cpe_matches)
                 )
 
+    def _get_all_cpes_in_dataset(self) -> set[CPE]:
+        if not self.auxiliary_datasets.cpe_dset:
+            raise ValueError(
+                "Cannot retrieve all cpes in dataset when cpe_dset is not set. You can prepare it with obj._prepare_cpe_dataset()"
+            )
+
+        cpe_matches = [
+            [self.auxiliary_datasets.cpe_dset.cpes[y] for y in x.heuristics.cpe_matches]
+            for x in self
+            if x.heuristics.cpe_matches
+        ]
+        return set(itertools.chain.from_iterable(cpe_matches))
+
     @serialize
-    def compute_related_cves(
-        self,
-        download_fresh_cves: bool = False,
-        use_nist_cpe_matching_dict: bool = True,
-    ) -> None:
+    def compute_related_cves(self) -> None:
         """
         Computes CVEs for the certificates, given their CPE matches.
         """
-        logger.info("Retrieving related CVEs to verified CPE matches")
-        if download_fresh_cves or not self.auxillary_datasets.cve_dset:
-            self.auxillary_datasets.cve_dset = self._prepare_cve_dataset(
-                download_fresh_cves, use_nist_cpe_matching_dict
-            )
-
         logger.info("Computing heuristics: CVEs in certificates.")
+
+        if not self.auxiliary_datasets.cpe_dset:
+            self.auxiliary_datasets.cpe_dset = self._prepare_cpe_dataset()
+
+        if not self.auxiliary_datasets.cve_dset:
+            self.auxiliary_datasets.cve_dset = self._prepare_cve_dataset()
+
+        if not self.auxiliary_datasets.cve_dset.look_up_dicts_built:
+            cpe_match_dict = self._prepare_cpe_match_dict()
+            all_cpes = self._get_all_cpes_in_dataset()
+            self.auxiliary_datasets.cve_dset.build_lookup_dict(cpe_match_dict, all_cpes)
+
         self.enrich_automated_cpes_with_manual_labels()
         cpe_rich_certs = [x for x in cast(Iterator[Certificate], self) if x.heuristics.cpe_matches]
 
         if not cpe_rich_certs:
             logger.error(
                 "No certificates with verified CPE match detected. You must run dset.manually_verify_cpe_matches() first. Returning."
             )
             return
 
-        relevant_cpes = set(itertools.chain.from_iterable(x.heuristics.cpe_matches for x in cpe_rich_certs))
-        self.auxillary_datasets.cve_dset.filter_related_cpes(relevant_cpes)
-
         cert: Certificate
         for cert in tqdm(cpe_rich_certs, desc="Computing related CVES"):
-            if cert.heuristics.cpe_matches:
-                related_cves = [
-                    self.auxillary_datasets.cve_dset.get_cve_ids_for_cpe_uri(x) for x in cert.heuristics.cpe_matches
-                ]
-                related_cves = list(filter(lambda x: x is not None, related_cves))
-                if related_cves:
-                    cert.heuristics.related_cves = set(
-                        itertools.chain.from_iterable(x for x in related_cves if x is not None)
-                    )
-            else:
-                cert.heuristics.related_cves = None
+            related_cves = self.auxiliary_datasets.cve_dset.get_cves_from_matched_cpe_uris(cert.heuristics.cpe_matches)
+            cert.heuristics.related_cves = related_cves if related_cves else None
 
         n_vulnerable = len([x for x in cpe_rich_certs if x.heuristics.related_cves])
         n_vulnerabilities = sum([len(x.heuristics.related_cves) for x in cpe_rich_certs if x.heuristics.related_cves])
         logger.info(
             f"In total, we identified {n_vulnerabilities} vulnerabilities in {n_vulnerable} vulnerable certificates."
         )
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/fips.py` & `sec-certs-0.1.4/src/sec_certs/dataset/fips.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,58 +8,58 @@
 from typing import Final
 
 import numpy as np
 import pandas as pd
 from bs4 import BeautifulSoup, NavigableString
 
 from sec_certs import constants
-from sec_certs.config.configuration import config
+from sec_certs.configuration import config
 from sec_certs.dataset.cpe import CPEDataset
 from sec_certs.dataset.cve import CVEDataset
-from sec_certs.dataset.dataset import AuxillaryDatasets, Dataset
+from sec_certs.dataset.dataset import AuxiliaryDatasets, Dataset
 from sec_certs.dataset.fips_algorithm import FIPSAlgorithmDataset
 from sec_certs.model.reference_finder import ReferenceFinder
 from sec_certs.model.transitive_vulnerability_finder import TransitiveVulnerabilityFinder
 from sec_certs.sample.fips import FIPSCertificate
 from sec_certs.serialization.json import ComplexSerializableType, serialize
 from sec_certs.utils import helpers
 from sec_certs.utils import parallel_processing as cert_processing
 from sec_certs.utils.helpers import fips_dgst
 
 logger = logging.getLogger(__name__)
 
 
-class FIPSAuxillaryDatasets(AuxillaryDatasets):
+class FIPSAuxiliaryDatasets(AuxiliaryDatasets):
     cpe_dset: CPEDataset | None = None
     cve_dset: CVEDataset | None = None
     algorithm_dset: FIPSAlgorithmDataset | None = None
 
 
-class FIPSDataset(Dataset[FIPSCertificate, FIPSAuxillaryDatasets], ComplexSerializableType):
+class FIPSDataset(Dataset[FIPSCertificate, FIPSAuxiliaryDatasets], ComplexSerializableType):
     """
     Class for processing of FIPSCertificate samples. Inherits from `ComplexSerializableType` and base abstract `Dataset` class.
     """
 
     def __init__(
         self,
-        certs: dict[str, FIPSCertificate] = dict(),
+        certs: dict[str, FIPSCertificate] = {},
         root_dir: str | Path = constants.DUMMY_NONEXISTING_PATH,
         name: str | None = None,
         description: str = "",
         state: Dataset.DatasetInternalState | None = None,
-        auxillary_datasets: FIPSAuxillaryDatasets | None = None,
+        auxiliary_datasets: FIPSAuxiliaryDatasets | None = None,
     ):
         self.certs = certs
         self.timestamp = datetime.datetime.now()
         self.sha256_digest = "not implemented"
         self.name = name if name else type(self).__name__ + " dataset"
         self.description = description if description else datetime.datetime.now().strftime("%d/%m/%Y %H:%M:%S")
         self.state = state if state else self.DatasetInternalState()
-        self.auxillary_datasets: FIPSAuxillaryDatasets = (
-            auxillary_datasets if auxillary_datasets else FIPSAuxillaryDatasets()
+        self.auxiliary_datasets: FIPSAuxiliaryDatasets = (
+            auxiliary_datasets if auxiliary_datasets else FIPSAuxiliaryDatasets()
         )
 
         self.root_dir = Path(root_dir)
 
     LIST_OF_CERTS_HTML: Final[dict[str, str]] = {
         "fips_modules_active.html": constants.FIPS_ACTIVE_MODULES_URL,
         "fips_modules_historical.html": constants.FIPS_HISTORICAL_MODULES_URL,
@@ -80,15 +80,15 @@
 
     @property
     def module_dir(self) -> Path:
         return self.certs_dir / "modules"
 
     @property
     def algorithm_dataset_path(self) -> Path:
-        return self.auxillary_datasets_dir / "algorithms.json"
+        return self.auxiliary_datasets_dir / "algorithms.json"
 
     def __getitem__(self, item: str) -> FIPSCertificate:
         try:
             return super().__getitem__(item)
         except KeyError:
             return super().__getitem__(fips_dgst(item))
 
@@ -183,51 +183,51 @@
             certs_to_process,
             progress_bar_desc="Converting policies to pdf",
         )
 
     def _download_html_resources(self) -> None:
         logger.info("Downloading HTML files that list FIPS certificates.")
         html_urls = list(FIPSDataset.LIST_OF_CERTS_HTML.values())
-        html_paths = [self.web_dir / x for x in FIPSDataset.LIST_OF_CERTS_HTML.keys()]
+        html_paths = [self.web_dir / x for x in FIPSDataset.LIST_OF_CERTS_HTML]
         helpers.download_parallel(html_urls, html_paths)
 
     def _get_all_certs_from_html_sources(self) -> list[FIPSCertificate]:
         return list(
             itertools.chain.from_iterable(
-                self._get_certificates_from_html(self.web_dir / x) for x in self.LIST_OF_CERTS_HTML.keys()
+                self._get_certificates_from_html(self.web_dir / x) for x in self.LIST_OF_CERTS_HTML
             )
         )
 
     def _get_certificates_from_html(self, html_file: Path) -> list[FIPSCertificate]:
-        with open(html_file, encoding="utf-8") as handle:
+        with html_file.open("r", encoding="utf-8") as handle:
             html = BeautifulSoup(handle.read(), "html5lib")
 
         table = [x for x in html.find(id="searchResultsTable").tbody.contents if x != "\n"]
         cert_ids: set[str] = set()
 
         for entry in table:
             if isinstance(entry, NavigableString):
                 continue
             cert_id = entry.find("a").text
             if cert_id not in cert_ids:
                 cert_ids.add(cert_id)
 
-        return [FIPSCertificate(cert_id) for cert_id in cert_ids]
+        return [FIPSCertificate(int(cert_id)) for cert_id in cert_ids]
 
     @classmethod
     def from_web_latest(cls) -> FIPSDataset:
         """
         Fetches the fresh snapshot of FIPSDataset from mirror.
         """
         return cls.from_web(config.fips_latest_snapshot, "Downloading FIPS Dataset", "fips_latest_dataset.json")
 
     def _set_local_paths(self) -> None:
         super()._set_local_paths()
-        if self.auxillary_datasets.algorithm_dset:
-            self.auxillary_datasets.algorithm_dset.json_path = self.algorithm_dataset_path
+        if self.auxiliary_datasets.algorithm_dset:
+            self.auxiliary_datasets.algorithm_dset.json_path = self.algorithm_dataset_path
 
         cert: FIPSCertificate
         for cert in self.certs.values():
             cert.set_local_paths(self.policies_pdf_dir, self.policies_txt_dir, self.module_dir)
 
     @serialize
     def get_certs_from_web(self, to_download: bool = True, keep_metadata: bool = True) -> None:
@@ -243,17 +243,17 @@
         if not keep_metadata:
             shutil.rmtree(self.web_dir)
 
         self._set_local_paths()
         self.state.meta_sources_parsed = True
 
     @serialize
-    def process_auxillary_datasets(self, download_fresh: bool = False) -> None:
-        super().process_auxillary_datasets(download_fresh)
-        self.auxillary_datasets.algorithm_dset = self._prepare_algorithm_dataset(download_fresh)
+    def process_auxiliary_datasets(self, download_fresh: bool = False) -> None:
+        super().process_auxiliary_datasets(download_fresh)
+        self.auxiliary_datasets.algorithm_dset = self._prepare_algorithm_dataset(download_fresh)
 
     def _prepare_algorithm_dataset(self, download_fresh_algs: bool = False) -> FIPSAlgorithmDataset:
         logger.info("Preparing FIPSAlgorithm dataset.")
         if not self.algorithm_dataset_path.exists() or download_fresh_algs:
             alg_dset = FIPSAlgorithmDataset.from_web(self.algorithm_dataset_path)
             alg_dset.to_json()
         else:
@@ -280,45 +280,45 @@
             use_threading=False,
             progress_bar_desc="Extracting security policy metadata",
         )
         self.update_with_certs(processed_certs)
 
     def _compute_transitive_vulnerabilities(self) -> None:
         logger.info("Computing heuristics: Computing transitive vulnerabilities in referenc(ed/ing) certificates.")
-        transitive_cve_finder = TransitiveVulnerabilityFinder(lambda cert: cert.cert_id)
+        transitive_cve_finder = TransitiveVulnerabilityFinder(lambda cert: str(cert.cert_id))
         transitive_cve_finder.fit(self.certs, lambda cert: cert.heuristics.policy_processed_references)
 
         for dgst in self.certs:
             transitive_cve = transitive_cve_finder.predict_single_cert(dgst)
             self.certs[dgst].heuristics.direct_transitive_cves = transitive_cve.direct_transitive_cves
             self.certs[dgst].heuristics.indirect_transitive_cves = transitive_cve.indirect_transitive_cves
 
     def _prune_reference_candidates(self) -> None:
         for cert in self:
             cert.prune_referenced_cert_ids()
 
         # Previously, a following procedure was used to prune reference_candidates:
-        #   - A set of algorithms was obtained via self.auxillary_datasets.algorithm_dset.get_algorithms_by_id(reference_candidate)
+        #   - A set of algorithms was obtained via self.auxiliary_datasets.algorithm_dset.get_algorithms_by_id(reference_candidate)
         #   - If any of these algorithms had the same vendor as the reference_candidate, the candidate was rejected
         #   - The rationale is that if an ID appears in a certificate s.t. an algorithm with the same ID was produced by the same vendor, the reference likely refers to alg.
         #   - Such reference should then be discarded.
         #   - We are uncertain of the effectivity of such measure, disabling it for now.
 
     def _compute_references(self, keep_unknowns: bool = False) -> None:
         logger.info("Computing heuristics: Recovering references between certificates")
         self._prune_reference_candidates()
 
         policy_reference_finder = ReferenceFinder()
         policy_reference_finder.fit(
-            self.certs, lambda cert: cert.cert_id, lambda cert: cert.heuristics.policy_prunned_references
+            self.certs, lambda cert: str(cert.cert_id), lambda cert: cert.heuristics.policy_prunned_references
         )
 
         module_reference_finder = ReferenceFinder()
         module_reference_finder.fit(
-            self.certs, lambda cert: cert.cert_id, lambda cert: cert.heuristics.module_prunned_references
+            self.certs, lambda cert: str(cert.cert_id), lambda cert: cert.heuristics.module_prunned_references
         )
 
         for cert in self:
             cert.heuristics.policy_processed_references = policy_reference_finder.predict_single_cert(
                 cert.dgst, keep_unknowns
             )
             cert.heuristics.module_processed_references = module_reference_finder.predict_single_cert(
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/fips_algorithm.py` & `sec-certs-0.1.4/src/sec_certs/dataset/fips_algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 from typing import Iterator
 
 import pandas as pd
 from bs4 import BeautifulSoup
 
 from sec_certs import constants
 from sec_certs.dataset.json_path_dataset import JSONPathDataset
-from sec_certs.sample import FIPSAlgorithm
+from sec_certs.sample.fips_algorithm import FIPSAlgorithm
 from sec_certs.serialization.json import ComplexSerializableType
 from sec_certs.utils import helpers
 
 logger = logging.getLogger(__name__)
 
 
 class FIPSAlgorithmDataset(JSONPathDataset, ComplexSerializableType):
-    def __init__(
-        self, algs: dict[str, FIPSAlgorithm] = dict(), json_path: str | Path = constants.DUMMY_NONEXISTING_PATH
-    ):
+    def __init__(self, algs: dict[str, FIPSAlgorithm] = {}, json_path: str | Path = constants.DUMMY_NONEXISTING_PATH):
         self.algs = algs
         self.json_path = Path(json_path)
-        self.alg_number_to_algs: dict[str, set[FIPSAlgorithm]] = dict()
+        self.alg_number_to_algs: dict[str, set[FIPSAlgorithm]] = {}
 
         self._build_lookup_dicts()
 
     @property
     def serialized_attributes(self) -> list[str]:
         return ["algs"]
 
@@ -44,15 +42,15 @@
 
     def __len__(self) -> int:
         return len(self.algs)
 
     def __contains__(self, item: FIPSAlgorithm) -> bool:
         if not isinstance(item, FIPSAlgorithm):
             raise ValueError(f"{item} is not of FIPSAlgorithm class")
-        return item.dgst in self.algs.keys() and self.algs[item.dgst] == item
+        return item.dgst in self.algs and self.algs[item.dgst] == item
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, FIPSAlgorithmDataset) and self.algs == other.algs
 
     @classmethod
     def from_web(cls, json_path: str | Path = constants.DUMMY_NONEXISTING_PATH) -> FIPSAlgorithmDataset:
         with TemporaryDirectory() as tmp_dir:
@@ -105,17 +103,15 @@
                 row["alg_number"], row["alg_type"], row["Vendor"], row["Implementation"], row["Validation Date"]
             ),
             axis=1,
         )
         return set(df["alg"])
 
     def to_pandas(self) -> pd.DataFrame:
-        df = pd.DataFrame([x.pandas_tuple for x in self], columns=FIPSAlgorithm.pandas_columns)
-        df = df.set_index("dgst")
-        return df
+        return pd.DataFrame([x.pandas_tuple for x in self], columns=FIPSAlgorithm.pandas_columns).set_index("dgst")
 
     def _build_lookup_dicts(self) -> None:
         for alg in self:
             if alg.alg_number not in self.alg_number_to_algs:
                 self.alg_number_to_algs[alg.alg_number] = {alg}
             else:
                 self.alg_number_to_algs[alg.alg_number].add(alg)
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/fips_iut.py` & `sec-certs-0.1.4/src/sec_certs/dataset/fips_iut.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Iterator, Mapping
 
 import requests
 
 from sec_certs import constants
-from sec_certs.config.configuration import config
+from sec_certs.configuration import config
 from sec_certs.dataset.dataset import logger
 from sec_certs.dataset.json_path_dataset import JSONPathDataset
 from sec_certs.sample.fips_iut import IUTSnapshot
 from sec_certs.serialization.json import ComplexSerializableType
 from sec_certs.utils.tqdm import tqdm
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/json_path_dataset.py` & `sec-certs-0.1.4/src/sec_certs/dataset/json_path_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
-import json
 import logging
 import shutil
 from abc import ABC
 from pathlib import Path
 
-from sec_certs.serialization.json import ComplexSerializableType, CustomJSONDecoder, get_class_fullname
+from sec_certs.serialization.json import ComplexSerializableType, get_class_fullname
 
 logger = logging.getLogger(__name__)
 
 
 class JSONPathDataset(ComplexSerializableType, ABC):
     _json_path: Path
 
@@ -35,12 +34,11 @@
             shutil.move(str(self.json_path), str(new_json_path))
             self.json_path = new_json_path
         else:
             self.json_path = new_json_path
             self.to_json()
 
     @classmethod
-    def from_json(cls, input_path: str | Path):
-        with Path(input_path).open("r") as handle:
-            dset = json.load(handle, cls=CustomJSONDecoder)
+    def from_json(cls, input_path: str | Path, is_compressed: bool = False):
+        dset = super().from_json(input_path, is_compressed)
         dset.json_path = Path(input_path)
         return dset
```

### Comparing `sec-certs-0.1.3/src/sec_certs/dataset/protection_profile.py` & `sec-certs-0.1.4/src/sec_certs/dataset/protection_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import json
 import logging
 import shutil
 import tempfile
 from dataclasses import dataclass
 from pathlib import Path
 
-import sec_certs.utils.helpers as helpers
 from sec_certs import constants
-from sec_certs.config.configuration import config
+from sec_certs.configuration import config
 from sec_certs.sample.protection_profile import ProtectionProfile
 from sec_certs.serialization.json import get_class_fullname
+from sec_certs.utils import helpers
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ProtectionProfileDataset:
     pps: dict[tuple[str, str | None], ProtectionProfile]
@@ -79,15 +79,14 @@
                 logger.warning(f"Duplicate entry in PP dataset: {(item.pp_name, item.pp_link)}")
             dct[(item.pp_name, item.pp_link)] = item
 
         return cls(dct)
 
     @classmethod
     def from_web(cls, store_dataset_path: Path | None = None):
-
         logger.info(f"Downloading static PP dataset from: {config.pp_latest_snapshot}")
         if not store_dataset_path:
             tmp = tempfile.TemporaryDirectory()
             store_dataset_path = Path(tmp.name) / "pp_dataset.json"
 
         helpers.download_file(config.pp_latest_snapshot, store_dataset_path)
         obj = cls.from_json(store_dataset_path)
```

### Comparing `sec-certs-0.1.3/src/sec_certs/model/__init__.py` & `sec-certs-0.1.4/src/sec_certs/model/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 """
 This package exposes model (mostly transformers and classifiers) that apply complex transformations. These are to be
 leveraged by members of Dataset package and are directly applied on members of Sample class (or on built-in objects).
 """
 
+from sec_certs.model.cc_matching import CCSchemeMatcher
 from sec_certs.model.cpe_matching import CPEClassifier
+from sec_certs.model.fips_matching import FIPSProcessMatcher
 from sec_certs.model.reference_finder import ReferenceFinder
 from sec_certs.model.sar_transformer import SARTransformer
 from sec_certs.model.transitive_vulnerability_finder import TransitiveVulnerabilityFinder
 
-__all__ = ["CPEClassifier", "ReferenceFinder", "TransitiveVulnerabilityFinder", "SARTransformer"]
+__all__ = [
+    "CPEClassifier",
+    "CCSchemeMatcher",
+    "FIPSProcessMatcher",
+    "ReferenceFinder",
+    "TransitiveVulnerabilityFinder",
+    "SARTransformer",
+]
```

### Comparing `sec-certs-0.1.3/src/sec_certs/model/cpe_matching.py` & `sec-certs-0.1.4/src/sec_certs/model/cpe_matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,45 @@
 
 import itertools
 import logging
 import operator
 import re
 from typing import Pattern
 
-import spacy
 from rapidfuzz import fuzz
-from sklearn.base import BaseEstimator
 
 from sec_certs import cert_rules, constants
 from sec_certs.sample.cpe import CPE
+from sec_certs.utils.strings import (
+    discard_trademark_symbols,
+    fully_sanitize_string,
+    lemmatize_product_name,
+    load_spacy_model,
+    standardize_version_in_cert_name,
+)
 from sec_certs.utils.tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 
 
-class CPEClassifier(BaseEstimator):
+class CPEClassifier:
     """
     Class that can predict CPE matches for certificate instances.
-    Adheres to sklearn BaseEstimator interface.
+    Adheres to sklearn `sklearn.base.BaseEstimator` interface.
     Fit method is called on list of CPEs and build two look-up dictionaries, see description of attributes.
     """
 
     vendor_to_versions_: dict[str, set[str]]  # Key: CPE vendor, Value: versions of all CPE records of that vendor
     vendor_version_to_cpe_: dict[tuple[str, str], set[CPE]]  # Key: (CPE vendor, version), Value: CPEs (vendor, version)
     vendors_: set[str]
 
     def __init__(self, match_threshold: int = 80, n_max_matches: int = 10, spacy_model_to_use: str = "en_core_web_sm"):
         self.match_threshold = match_threshold
         self.n_max_matches = n_max_matches
-        self.nlp = spacy.load(spacy_model_to_use, disable=["parser", "ner"])
+        self.nlp = load_spacy_model(spacy_model_to_use)
 
     def fit(self, X: list[CPE], y: list[str] | None = None) -> CPEClassifier:
         """
         Just creates look-up structures from provided list of CPEs
 
         :param List[CPE] X: List of CPEs that can be matched with predict()
         :param Optional[List[str]] y: will be ignored, specified to adhere to sklearn BaseEstimator interface, defaults to None
@@ -62,22 +67,19 @@
         - vendors_: Just aggregates set of vendors, used for prunning later on.
 
         :param List[CPE] X: List of CPEs that will be used to build the dictionaries
         """
         sufficiently_long_cpes = self._filter_short_cpes(X)
         self.vendor_to_versions_ = {x.vendor: set() for x in sufficiently_long_cpes}
         self.vendors_ = set(self.vendor_to_versions_.keys())
-        self.vendor_version_to_cpe_ = dict()
+        self.vendor_version_to_cpe_ = {}
 
         for cpe in tqdm(sufficiently_long_cpes, desc="Fitting the CPE classifier"):
             self.vendor_to_versions_[cpe.vendor].add(cpe.version)
-            if (cpe.vendor, cpe.version) not in self.vendor_version_to_cpe_:
-                self.vendor_version_to_cpe_[(cpe.vendor, cpe.version)] = {cpe}
-            else:
-                self.vendor_version_to_cpe_[(cpe.vendor, cpe.version)].add(cpe)
+            self.vendor_version_to_cpe_.setdefault((cpe.vendor, cpe.version), set()).add(cpe)
 
     def predict(self, X: list[tuple[str, str, str]]) -> list[set[str] | None]:
         """
         Will predict CPE uris for List of Tuples (vendor, product name, identified versions in product name)
 
         :param List[Tuple[str, str, str]] X: tuples (vendor, product name, identified versions in product name)
         :return List[Optional[Set[str]]]: List of CPE uris that correspond to given input, None if nothing was found.
@@ -105,17 +107,17 @@
         :param Optional[str] vendor: manufacturer of the certificate
         :param str product_name: name of the certificate
         :param Set[str] versions: List of versions that appear in the certificate name
         :param bool relax_version: See step 6 above., defaults to False
         :param bool relax_title: See step 7 above, defaults to False
         :return Optional[Set[str]]: Set of matching CPE uris, None if no matches found
         """
-        lemmatized_product_name = self._lemmatize_product_name(product_name)
+        lemmatized_product_name = lemmatize_product_name(self.nlp, product_name)
         candidate_vendors = self._get_candidate_list_of_vendors(
-            CPEClassifier._discard_trademark_symbols(vendor).lower() if vendor else vendor
+            discard_trademark_symbols(vendor).lower() if vendor else vendor
         )
         candidates = self._get_candidate_cpe_matches(candidate_vendors, versions)
         candidates = self._filter_candidates_by_platform(candidates, product_name)
         candidates = self._filter_candidates_by_update(candidates, lemmatized_product_name)
 
         ratings = [
             self._compute_best_match(cpe, lemmatized_product_name, candidate_vendors, versions, relax_title=relax_title)
@@ -144,28 +146,28 @@
         """
         Update means `service pack` or `release`.
         """
 
         def filter_condition(regex: Pattern, cpe: CPE, min_value: int, soft: bool = True):
             if matches := re.findall(regex, cpe.update):
                 return int(re.findall(r"\d+", matches[0])[0]) >= min_value
-            return True if soft else False
+            return soft
 
         update_regexes = [cert_rules.SERVICE_PACK_RE, cert_rules.RELEASE_RE]
 
         for update_regex in update_regexes:
             if matches := re.findall(update_regex, cert_title):
                 min_value = min([int(re.findall(r"\d+", x)[0]) for x in matches])
                 soft = not any(re.search(update_regex, cpe.update + str(cpe.title)) for cpe in cpes)
                 return [x for x in cpes if filter_condition(update_regex, x, min_value, soft)]
 
         return cpes
 
     def _filter_candidates_by_platform(self, cpes: list[CPE], cert_title: str) -> list[CPE]:
-        def filter_condition(cpe: CPE, cert_platforms: set[str]):
+        def filter_condition(cpe: CPE, cert_platforms: set[str]) -> bool:
             if not cert_platforms and cpe.target_hw == "*":
                 return True
             if cert_platforms and cpe.target_hw == "*":
                 return any(re.search(cert_rules.PLATFORM_REGEXES[x], str(cpe.title)) for x in cert_platforms)
             if not cert_platforms and cpe.target_hw != "*":
                 return False
             if cert_platforms and cpe.target_hw != "*":
@@ -176,16 +178,17 @@
                 ]
                 assert len(target_hw_platforms) <= 1
                 can_return_true = any(
                     re.search(cert_rules.PLATFORM_REGEXES[x], cpe.target_hw + str(cpe.title)) for x in cert_platforms
                 )
                 if not target_hw_platforms:
                     return can_return_true
-                else:
-                    return can_return_true and target_hw_platforms[0] in cert_platforms
+
+                return can_return_true and target_hw_platforms[0] in cert_platforms
+            return True
 
         crt_platforms = {
             platform for platform, regex in cert_rules.PLATFORM_REGEXES.items() if re.search(regex, cert_title)
         }
         return [x for x in cpes if filter_condition(x, crt_platforms)]
 
     def _compute_best_match(
@@ -206,36 +209,36 @@
         :param Optional[Set[str]] candidate_vendors: vendors that appear in the certificate
         :param Set[str] versions: versions that appear in the certificate
         :param bool relax_title: if to relax title or not, defaults to False
         :return float: Maximal value of the four string similarities discussed above.
         """
         if relax_title:
             sanitized_title = (
-                CPEClassifier._fully_sanitize_string(cpe.title)
+                fully_sanitize_string(cpe.title)
                 if cpe.title
-                else CPEClassifier._fully_sanitize_string(
+                else fully_sanitize_string(
                     cpe.vendor + " " + cpe.item_name + " " + cpe.version + " " + cpe.update + " " + cpe.target_hw
                 )
             )
         else:
             if cpe.title:
-                sanitized_title = CPEClassifier._fully_sanitize_string(cpe.title)
+                sanitized_title = fully_sanitize_string(cpe.title)
             else:
                 return 0
 
         # Sometimes, sanitization shortens CPE title to very short length. E.g., CPEs in Japanese unicode symbols that get all deteled.
         if len(sanitized_title) < 5:
             return 0
 
-        sanitized_item_name = CPEClassifier._fully_sanitize_string(cpe.item_name)
+        sanitized_item_name = fully_sanitize_string(cpe.item_name)
         sanitized_cpe_stripped_manufacturer = re.sub(r"\b" + rf"{cpe.vendor}" + r"\b", "", sanitized_title)
-        standard_version_product_name = self._standardize_version_in_cert_name(product_name, versions)
+        standard_version_product_name = standardize_version_in_cert_name(product_name, versions)
 
         # The expression below is currently unused, it could assist with some matches though
-        # cert_stripped = CPEClassifier._strip_manufacturer_and_version(product_name, candidate_vendors, versions)
+        # cert_stripped = strip_manufacturer_and_version(product_name, candidate_vendors, versions)
 
         # On some ratings, we require 100 match regardless of the treshold in settings.
         ratings = [
             fuzz.token_set_ratio(product_name, sanitized_title),
             fuzz.token_set_ratio(standard_version_product_name, sanitized_title),
             fuzz.partial_token_sort_ratio(product_name, sanitized_title, score_cutoff=100),
             fuzz.partial_token_sort_ratio(standard_version_product_name, sanitized_title, score_cutoff=100),
@@ -250,42 +253,14 @@
                 fuzz.partial_ratio(product_name, sanitized_cpe_stripped_manufacturer, score_cutoff=100),
                 fuzz.token_set_ratio(product_name, sanitized_item_name, score_cutoff=100),
                 fuzz.partial_ratio(product_name, sanitized_item_name, score_cutoff=100),
             ]
 
         return max(ratings)
 
-    @staticmethod
-    def _fully_sanitize_string(string: str) -> str:
-        return CPEClassifier._replace_special_chars_with_space(
-            CPEClassifier._discard_trademark_symbols(string.lower())
-        ).strip()
-
-    @staticmethod
-    def _replace_special_chars_with_space(string: str) -> str:
-        return re.sub(r"[^a-zA-Z0-9 \n\.]", " ", string)
-
-    @staticmethod
-    def _discard_trademark_symbols(string: str) -> str:
-        return string.replace("®", "").replace("™", "")
-
-    @staticmethod
-    def _strip_manufacturer_and_version(string: str, manufacturers: set[str] | None, versions: set[str]) -> str:
-        to_strip = versions | manufacturers if manufacturers else versions
-        for x in to_strip:
-            string = string.lower().replace(CPEClassifier._replace_special_chars_with_space(x.lower()), " ").strip()
-        return string
-
-    @staticmethod
-    def _standardize_version_in_cert_name(string: str, detected_versions: set[str]) -> str:
-        for ver in detected_versions:
-            version_regex = r"(" + r"(\bversion)\s*" + ver + r"+) | (\bv\s*" + ver + r"+)"
-            string = re.sub(version_regex, " " + ver + " ", string, flags=re.IGNORECASE)
-        return string
-
     def _process_manufacturer(self, manufacturer: str, result: set) -> set[str]:
         tokenized = manufacturer.split()
         if tokenized[0] in self.vendors_:
             result.add(tokenized[0])
         if len(tokenized) > 1 and tokenized[0] + tokenized[1] in self.vendors_:
             result.add(tokenized[0] + tokenized[1])
 
@@ -319,15 +294,15 @@
         splits = re.compile(r"[,/]").findall(manufacturer)
 
         if splits:
             vendor_tokens = set(
                 itertools.chain.from_iterable([x.strip() for x in manufacturer.split(s)] for s in splits)
             )
             result_aux = [self._get_candidate_list_of_vendors(x) for x in vendor_tokens]
-            result_used = set(set(itertools.chain.from_iterable(x for x in result_aux if x)))
+            result_used = set(itertools.chain.from_iterable(x for x in result_aux if x))
             return result_used if result_used else set()
 
         if manufacturer in self.vendors_:
             result.add(manufacturer)
 
         return self._process_manufacturer(manufacturer, result)
 
@@ -343,18 +318,15 @@
         :return Optional[List[Tuple[str, str]]]: List of tuples (cpe_vendor, cpe_version) that can be used in the lookup table to search the CPE dataset.
         """
 
         def is_cpe_version_among_cert_versions(cpe_version: str | None, cert_versions: set[str]) -> bool:
             def simple_startswith(seeked_version: str, checked_string: str) -> bool:
                 if seeked_version == checked_string:
                     return True
-                else:
-                    return (
-                        checked_string.startswith(seeked_version) and not checked_string[len(seeked_version)].isdigit()
-                    )
+                return checked_string.startswith(seeked_version) and not checked_string[len(seeked_version)].isdigit()
 
             if not cpe_version:
                 return False
             just_numbers = r"(\d{1,5})(\.\d{1,5})"
 
             # This assures that on cert version with at least two tokens, we don't match only one-token CPE.
             # E.g. cert with version 7.6 must not match CPE record of version 7
@@ -393,12 +365,7 @@
         """
         candidate_vendor_version_pairs = self._get_candidate_vendor_version_pairs(candidate_vendors, candidate_versions)
         return (
             list(itertools.chain.from_iterable(self.vendor_version_to_cpe_[x] for x in candidate_vendor_version_pairs))
             if candidate_vendor_version_pairs
             else []
         )
-
-    def _lemmatize_product_name(self, product_name: str) -> str:
-        if not product_name:
-            return product_name
-        return " ".join([token.lemma_ for token in self.nlp(CPEClassifier._fully_sanitize_string(product_name))])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sec-certs-0.1.3/src/sec_certs/model/evaluation.py` & `sec-certs-0.1.4/src/sec_certs/model/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import json
 import logging
 from pathlib import Path
 
 import numpy as np
 
-import sec_certs.utils.helpers as helpers
 from sec_certs.dataset.cpe import CPEDataset
 from sec_certs.sample.cc import CCCertificate
 from sec_certs.sample.fips import FIPSCertificate
 from sec_certs.serialization.json import CustomJSONEncoder
+from sec_certs.utils import helpers
 
 logger = logging.getLogger(__name__)
 
 
 def get_validation_dgsts(filepath: str | Path) -> set[str]:
     with Path(filepath).open("r") as handle:
         return set(json.load(handle))
```

### Comparing `sec-certs-0.1.3/src/sec_certs/model/reference_finder.py` & `sec-certs-0.1.4/src/sec_certs/model/reference_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class ReferenceFinder:
     """
     The class assigns references of other certificate instances for each instance.
     Adheres to sklearn BaseEstimator interface.
     The fit is called on a dictionary of certificates, builds a hashmap of references, and assigns references for each certificate in the dictionary.
     """
 
-    def __init__(self):
+    def __init__(self: ReferenceFinder) -> None:
         self.references: ReferencesType = {}
         self.id_mapping: IDMapping = {}
         self._fitted: bool = False
 
     def _create_id_mapping(self, certificates: Certificates, id_func: IDLookupFunc) -> None:
         """
         Create the ID mapping of certificate IDs to certificate digests.
```

### Comparing `sec-certs-0.1.3/src/sec_certs/model/sar_transformer.py` & `sec-certs-0.1.4/src/sec_certs/model/sar_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 import logging
 from typing import Dict, Iterable, cast
 
-from sklearn.base import BaseEstimator, TransformerMixin
-
 from sec_certs.sample.cc import CCCertificate
 from sec_certs.sample.sar import SAR, SAR_DICT_KEY
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Right now we ignore number of ocurrences for final SAR selection. If we keep it this way, we can discard that variable
-class SARTransformer(BaseEstimator, TransformerMixin):
+class SARTransformer:
     """
     Class for transforming SARs defined in st_keywords and report_keywords dictionaries into SAR objects.
-    This class implements sklearn transformer interface, so fit_transform() can be called on it.
+    This class implements `sklearn.base.Transformer` interface, so fit_transform() can be called on it.
     """
 
     def fit(self, certificates: Iterable[CCCertificate]) -> SARTransformer:
         """
         Just returns self, no fitting needed
 
         :param Iterable[CCCertificate] certificates: Unused parameter
         :return SARTransformer: return self
         """
         return self
 
+    def fit_transform(self, X, y=None, **fit_params):
+        return self.fit(X).transform(X)
+
     def transform(self, certificates: Iterable[CCCertificate]) -> list[set[SAR] | None]:
         """
         Just a wrapper around transform_single_cert() called on an iterable of CCCertificate.
 
         :param Iterable[CCCertificate] certificates: Iterable of CCCertificate objects to perform the extraction on.
         :return List[Optional[Set[SAR]]]: Returns List of results from transform_single_cert().
         """
@@ -124,15 +125,15 @@
 
         Only SARs with recovered level are considered, e.g. ASE_REQ.2 is valid string while ASE_REQ is not.
 
         :param dct: _description_
         :param dgst: DIgest of the processed certificate.
         :return: _description_
         """
-        sars: dict[str, tuple[SAR, int]] = dict()
+        sars: dict[str, tuple[SAR, int]] = {}
         for sar_class, class_matches in dct.items():
             for sar_string, n_occurences in class_matches.items():
                 try:
                     candidate = SAR.from_string(sar_string)
                 except ValueError as e:
                     logger.debug(f"Badly formatted SAR string {sar_string}, skipping: {e}")
                     continue
```

### Comparing `sec-certs-0.1.3/src/sec_certs/model/transitive_vulnerability_finder.py` & `sec-certs-0.1.4/src/sec_certs/model/transitive_vulnerability_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
     def _fill_dataset_cert_ids_counter(self) -> None:
         self._cert_id_counter = Counter([self._id_func(x) for x in self.certificates.values()])
 
     def _get_cert_transitive_cves(
         self, cert: CertSubType, reference_type: ReferenceType, ref_func: ReferenceLookupFunc
     ) -> set[str] | None:
-
         references = (
             ref_func(cert).directly_referenced_by
             if reference_type == ReferenceType.DIRECT
             else ref_func(cert).indirectly_referenced_by
         )
 
         if not references:
@@ -94,15 +93,15 @@
 
             if not cert_id:
                 continue
             if self._cert_id_counter[cert_id] > 1:
                 thrown_away_cert_counter += 1
                 continue
 
-            self.vulnerabilities[cert.dgst] = dict()
+            self.vulnerabilities[cert.dgst] = {}
             self.vulnerabilities[cert.dgst][ReferenceType.DIRECT.value] = self._get_cert_transitive_cves(
                 cert, ReferenceType.DIRECT, ref_func
             )
             self.vulnerabilities[cert.dgst][ReferenceType.INDIRECT.value] = self._get_cert_transitive_cves(
                 cert, ReferenceType.INDIRECT, ref_func
             )
```

### Comparing `sec-certs-0.1.3/src/sec_certs/rules.yaml` & `sec-certs-0.1.4/src/sec_certs/rules.yaml`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/__init__.py` & `sec-certs-0.1.4/src/sec_certs/sample/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """This package holds mostly data objects of primary interest (Common Criteria, FIPS), or assisting objects
 like CPE, CVE, etc. The objects mostly hold data and allow for serialization, but can also perform some basic transformations.
 """
 
 from sec_certs.sample.cc import CCCertificate
 from sec_certs.sample.cc_certificate_id import CertificateId
 from sec_certs.sample.cc_maintenance_update import CCMaintenanceUpdate
-from sec_certs.sample.cpe import CPE, cached_cpe
+from sec_certs.sample.cpe import CPE
 from sec_certs.sample.cve import CVE
 from sec_certs.sample.fips import FIPSCertificate
 from sec_certs.sample.fips_algorithm import FIPSAlgorithm
 from sec_certs.sample.fips_iut import IUTEntry, IUTSnapshot
 from sec_certs.sample.fips_mip import MIPEntry, MIPSnapshot, MIPStatus
 from sec_certs.sample.protection_profile import ProtectionProfile
 from sec_certs.sample.sar import SAR
 
 __all__ = [
     "CertificateId",
     "CCMaintenanceUpdate",
     "CCCertificate",
     "CPE",
-    "cached_cpe",
+    "CPEConfiguration",
     "CVE",
     "FIPSCertificate",
     "FIPSAlgorithm",
     "IUTEntry",
     "IUTSnapshot",
     "MIPEntry",
     "MIPSnapshot",
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/cc.py` & `sec-certs-0.1.4/src/sec_certs/sample/cc.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 import numpy as np
 import requests
 from bs4 import Tag
 
 import sec_certs.utils.extract
 import sec_certs.utils.pdf
 import sec_certs.utils.sanitization
-from sec_certs import constants as constants
+from sec_certs import constants
 from sec_certs.cert_rules import SARS_IMPLIED_FROM_EAL, cc_rules, rules, security_level_csv_scan
 from sec_certs.sample.cc_certificate_id import canonicalize
-from sec_certs.sample.certificate import Certificate
+from sec_certs.sample.certificate import Certificate, References, logger
 from sec_certs.sample.certificate import Heuristics as BaseHeuristics
 from sec_certs.sample.certificate import PdfData as BasePdfData
-from sec_certs.sample.certificate import References, logger
 from sec_certs.sample.protection_profile import ProtectionProfile
 from sec_certs.sample.sar import SAR
 from sec_certs.serialization.json import ComplexSerializableType
 from sec_certs.serialization.pandas import PandasSerializableType
 from sec_certs.utils import helpers
 from sec_certs.utils.extract import normalize_match_string
 
@@ -113,18 +112,18 @@
         report_extract_ok: bool  # Whether report extraction went OK
 
         st_pdf_hash: str | None
         report_pdf_hash: str | None
         st_txt_hash: str | None
         report_txt_hash: str | None
 
-        st_pdf_path: Path
-        report_pdf_path: Path
-        st_txt_path: Path
-        report_txt_path: Path
+        _st_pdf_path: Path | None = None
+        _report_pdf_path: Path | None = None
+        _st_txt_path: Path | None = None
+        _report_txt_path: Path | None = None
 
         def __init__(
             self,
             st_download_ok: bool = False,
             report_download_ok: bool = False,
             st_convert_garbage: bool = False,
             report_convert_garbage: bool = False,
@@ -148,14 +147,54 @@
             self.report_extract_ok = report_extract_ok
             self.st_pdf_hash = st_pdf_hash
             self.report_pdf_hash = report_pdf_hash
             self.st_txt_hash = st_txt_hash
             self.report_txt_hash = report_txt_hash
 
         @property
+        def st_pdf_path(self) -> Path:
+            if not self._st_pdf_path:
+                raise ValueError(f"st_pdf_path not set on {type(self)}")
+            return self._st_pdf_path
+
+        @st_pdf_path.setter
+        def st_pdf_path(self, pth: str | Path | None) -> None:
+            self._st_pdf_path = Path(pth) if pth else None
+
+        @property
+        def report_pdf_path(self) -> Path:
+            if not self._report_pdf_path:
+                raise ValueError(f"report_pdf_path not set on {type(self)}")
+            return self._report_pdf_path
+
+        @report_pdf_path.setter
+        def report_pdf_path(self, pth: str | Path | None) -> None:
+            self._report_pdf_path = Path(pth) if pth else None
+
+        @property
+        def st_txt_path(self) -> Path:
+            if not self._st_txt_path:
+                raise ValueError(f"st_txt_path not set on {type(self)}")
+            return self._st_txt_path
+
+        @st_txt_path.setter
+        def st_txt_path(self, pth: str | Path | None) -> None:
+            self._st_txt_path = Path(pth) if pth else None
+
+        @property
+        def report_txt_path(self) -> Path:
+            if not self._report_txt_path:
+                raise ValueError(f"report_txt_path not set on {type(self)}")
+            return self._report_txt_path
+
+        @report_txt_path.setter
+        def report_txt_path(self, pth: str | Path | None) -> None:
+            self._report_txt_path = Path(pth) if pth else None
+
+        @property
         def serialized_attributes(self) -> list[str]:
             return [
                 "st_download_ok",
                 "report_download_ok",
                 "st_convert_garbage",
                 "report_convert_garbage",
                 "st_convert_ok",
@@ -394,14 +433,15 @@
         cert_lab: list[str] | None = field(default=None)
         cert_id: str | None = field(default=None)
         st_references: References = field(default_factory=References)
         report_references: References = field(default_factory=References)
         extracted_sars: set[SAR] | None = field(default=None)
         direct_transitive_cves: set[str] | None = field(default=None)
         indirect_transitive_cves: set[str] | None = field(default=None)
+        scheme_data: dict[str, Any] | None = field(default=None)
 
         @property
         def serialized_attributes(self) -> list[str]:
             return copy.deepcopy(super().serialized_attributes)
 
     pandas_columns: ClassVar[list[str]] = [
         "dgst",
@@ -468,17 +508,17 @@
         self.not_valid_after = sec_certs.utils.sanitization.sanitize_date(not_valid_after)
         self.report_link = sec_certs.utils.sanitization.sanitize_link(report_link)
         self.st_link = sec_certs.utils.sanitization.sanitize_link(st_link)
         self.cert_link = sec_certs.utils.sanitization.sanitize_link(cert_link)
         self.manufacturer_web = sec_certs.utils.sanitization.sanitize_link(manufacturer_web)
         self.protection_profiles = protection_profiles
         self.maintenance_updates = maintenance_updates
-        self.state = self.InternalState() if not state else state
-        self.pdf_data = self.PdfData() if not pdf_data else pdf_data
-        self.heuristics: CCCertificate.Heuristics = self.Heuristics() if not heuristics else heuristics
+        self.state = state if state else self.InternalState()
+        self.pdf_data = pdf_data if pdf_data else self.PdfData()
+        self.heuristics: CCCertificate.Heuristics = heuristics if heuristics else self.Heuristics()
 
     @property
     def dgst(self) -> str:
         """
         Computes the primary key of the sample using first 16 bytes of SHA-256 digest
         """
         if not (self.name is not None and self.report_link is not None and self.category is not None):
@@ -503,15 +543,15 @@
 
     @property
     def actual_sars(self) -> set[SAR] | None:
         """
         Computes actual SARs. First, SARs implied by EAL are computed. Then, these are augmented with heuristically extracted SARs
         :return Optional[Set[SAR]]: Set of actual SARs of a certificate, None if empty
         """
-        sars = dict()
+        sars = {}
         if self.eal:
             sars = {x[0]: SAR(x[0], x[1]) for x in SARS_IMPLIED_FROM_EAL[self.eal[:4]]}
 
         if self.heuristics.extracted_sars:
             for sar in self.heuristics.extracted_sars:
                 if sar not in sars or sar.level > sars[sar.family].level:
                     sars[sar.family] = sar
@@ -751,21 +791,21 @@
         Sets paths to files given the requested directories
 
         :param Optional[Union[str, Path]] report_pdf_dir: Directory where pdf reports shall be stored
         :param Optional[Union[str, Path]] st_pdf_dir: Directory where pdf security targets shall be stored
         :param Optional[Union[str, Path]] report_txt_dir: Directory where txt reports shall be stored
         :param Optional[Union[str, Path]] st_txt_dir: Directory where txt security targets shall be stored
         """
-        if report_pdf_dir is not None:
+        if report_pdf_dir:
             self.state.report_pdf_path = Path(report_pdf_dir) / (self.dgst + ".pdf")
-        if st_pdf_dir is not None:
+        if st_pdf_dir:
             self.state.st_pdf_path = Path(st_pdf_dir) / (self.dgst + ".pdf")
-        if report_txt_dir is not None:
+        if report_txt_dir:
             self.state.report_txt_path = Path(report_txt_dir) / (self.dgst + ".txt")
-        if st_txt_dir is not None:
+        if st_txt_dir:
             self.state.st_txt_path = Path(st_txt_dir) / (self.dgst + ".txt")
 
     @staticmethod
     def download_pdf_report(cert: CCCertificate) -> CCCertificate:
         """
         Downloads pdf of certification report given the certificate. Staticmethod to allow for parallelization.
 
@@ -791,19 +831,18 @@
     def download_pdf_st(cert: CCCertificate) -> CCCertificate:
         """
         Downloads pdf of security target given the certificate. Staticmethod to allow for parallelization.
 
         :param CCCertificate cert: cert to download the pdf security target for
         :return CCCertificate: returns the modified certificate with updated state
         """
-        exit_code: str | int
-        if not cert.st_link:
-            exit_code = "No link"
-        else:
-            exit_code = helpers.download_file(cert.st_link, cert.state.st_pdf_path)
+        exit_code: str | int = (
+            helpers.download_file(cert.st_link, cert.state.st_pdf_path) if cert.st_link else "No link"
+        )
+
         if exit_code != requests.codes.ok:
             error_msg = f"failed to download ST from {cert.st_link}, code: {exit_code}"
             logger.error(f"Cert dgst: {cert.dgst} " + error_msg)
             cert.state.st_download_ok = False
         else:
             cert.state.st_download_ok = True
             cert.state.st_pdf_hash = helpers.get_sha256_filepath(cert.state.st_pdf_path)
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/cc_certificate_id.py` & `sec-certs-0.1.4/src/sec_certs/sample/cc_certificate_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
     scheme: str
     raw: str
 
     def _canonical_fr(self) -> str:
         new_cert_id = self.clean
         rules = [
-            "(?:Rapport de certification|Certification Report) ([0-9]+[/-_][0-9]+(?:v[1-9])?(?:[_/-][MSR][0-9]+)?)",
-            "(?:ANSS[Ii]|DCSSI)(?:-CC)?[- ]([0-9]+[/-_][0-9]+(?:v[1-9])?(?:[_/-][MSR][0-9]+)?)",
-            "([0-9]+[/-_][0-9]+(?:v[1-9])?(?:[_/-][MSR][0-9]+)?)",
+            "(?:Rapport de certification|Certification Report) ([0-9]+[/-_][0-9]+(?:[vV][1-9])?(?:[_/-][MSR][0-9]+)?)",
+            "(?:ANSS[Ii]|DCSSI)(?:-CC)?[- ]([0-9]+[/-_][0-9]+(?:[vV][1-9])?(?:[_/-][MSR][0-9]+)?)",
+            "([0-9]+[/-_][0-9]+(?:[vV][1-9])?(?:[_/-][MSR][0-9]+)?)",
         ]
         for rule in rules:
             if match := re.match(rule, new_cert_id):
-                return "ANSSI-CC-" + match.group(1).replace("_", "/")
+                return "ANSSI-CC-" + match.group(1).replace("_", "/").replace("V", "v")
 
         return new_cert_id
 
     def _canonical_de(self) -> str:
         def extract_parts(bsi_parts: list[str]) -> tuple:
             cert_num = None
             cert_version = None
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/cc_maintenance_update.py` & `sec-certs-0.1.4/src/sec_certs/sample/cc_maintenance_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import logging
 from datetime import date
 from typing import ClassVar
 
-import sec_certs.utils.helpers as helpers
 from sec_certs.sample.cc import CCCertificate
 from sec_certs.serialization.json import ComplexSerializableType
+from sec_certs.utils import helpers
 
 logger = logging.getLogger(__name__)
 
 
 class CCMaintenanceUpdate(CCCertificate, ComplexSerializableType):
     pandas_columns: ClassVar[list[str]] = [
         "dgst",
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/certificate.py` & `sec-certs-0.1.4/src/sec_certs/sample/certificate.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 @dataclass
 class References(ComplexSerializableType):
     directly_referenced_by: set[str] | None = field(default=None)
     indirectly_referenced_by: set[str] | None = field(default=None)
     directly_referencing: set[str] | None = field(default=None)
     indirectly_referencing: set[str] | None = field(default=None)
 
+    def __bool__(self):
+        return any(getattr(self, x) for x in vars(self))
+
 
 class Heuristics:
     cpe_matches: set[str] | None
     related_cves: set[str] | None
 
 
 class PdfData:
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/fips.py` & `sec-certs-0.1.4/src/sec_certs/sample/fips.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,31 +8,25 @@
 from typing import Any, Callable, ClassVar, Final, Literal
 
 import dateutil
 import numpy as np
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup, Tag
-from tabula import read_pdf
 
-import sec_certs.constants as constants
-import sec_certs.utils.extract
-import sec_certs.utils.helpers as helpers
-import sec_certs.utils.pdf
-import sec_certs.utils.pdf as pdf
-import sec_certs.utils.tables as tables
+from sec_certs import constants
 from sec_certs.cert_rules import FIPS_ALGS_IN_TABLE, fips_rules
-from sec_certs.config.configuration import config
-from sec_certs.sample.certificate import Certificate
+from sec_certs.configuration import config
+from sec_certs.sample.certificate import Certificate, References, logger
 from sec_certs.sample.certificate import Heuristics as BaseHeuristics
 from sec_certs.sample.certificate import PdfData as BasePdfData
-from sec_certs.sample.certificate import References, logger
 from sec_certs.sample.cpe import CPE
 from sec_certs.serialization.json import ComplexSerializableType
 from sec_certs.serialization.pandas import PandasSerializableType
+from sec_certs.utils import extract, helpers, pdf, tables
 from sec_certs.utils.helpers import fips_dgst
 
 
 class FIPSHTMLParser:
     def __init__(self, soup: BeautifulSoup):
         self._soup = soup
 
@@ -65,15 +59,15 @@
             return normalized_key, normalized_entry
 
         entries = details_div.find_all("div", class_="row padrow")
         entries = zip(
             [x.find("div", class_="col-md-3") for x in entries], [x.find("div", class_="col-md-9") for x in entries]
         )
         entries = [(FIPSHTMLParser.normalize_string(key.text), entry) for key, entry in entries]
-        entries = [parse_single_detail_entry(*x) for x in entries if x[0] in DETAILS_KEY_NORMALIZATION_DICT.keys()]
+        entries = [parse_single_detail_entry(*x) for x in entries if x[0] in DETAILS_KEY_NORMALIZATION_DICT]
         entries = {x: y for x, y in entries}
 
         if "caveat" in entries:
             entries["mentioned_certs"] = FIPSHTMLParser.get_mentioned_certs_from_caveat(entries["caveat"])
 
         # Temporarily disabled, as this isn't extracting anything useful. Only UNKNOWN#1-9 algs were extracted over whole dataset.
         # if "description" in entries:
@@ -126,29 +120,45 @@
 
     @staticmethod
     def get_algs_from_description(description: str) -> set[str]:
         return {m.group() for m in re.finditer(FIPS_ALGS_IN_TABLE, description)}
 
     @staticmethod
     def parse_algorithms(algorithms_div: Tag) -> dict[str, set[str]]:
-        rows = algorithms_div.find("tbody").find_all("tr")
-        dct: dict[str, set[str]] = dict()
-        for row in rows:
-            cells = row.find_all("td")
-            dct[cells[0].text] = {m.group() for m in re.finditer(FIPS_ALGS_IN_TABLE, cells[1].text)}
+        dct: dict[str, set[str]] = {}
+        table = algorithms_div.find("tbody")
+        # Two types of organization on the CMVP website:
+        #  - One is a table with algo references in text
+        #  - Other is just divs for rows, one per algo
+        if table:
+            rows = table.find_all("tr")
+            for row in rows:
+                cells = row.find_all("td")
+                dct[str(cells[0].text)] = {m.group() for m in re.finditer(FIPS_ALGS_IN_TABLE, cells[1].text)}
+        else:
+            rows = algorithms_div.find_all("div", class_="col-md-12")
+            for row in rows:
+                dct[str(row.find("div", class_="col-md-3").text)] = {
+                    str(row.find("div", class_="col-md-4").text).strip()
+                }
         return dct
 
     @staticmethod
+    def normalize_type(mod_type: Tag) -> str:
+        tag_text = str(mod_type.text).strip()
+        return "-".join(s.capitalize() for s in tag_text.split("-"))
+
+    @staticmethod
     def normalize_string(string: str) -> str:
         return " ".join(string.split())
 
     @staticmethod
     def parse_tested_configurations(tested_configurations: Tag) -> list[str] | None:
         configurations = [y.text for y in tested_configurations.find_all("li")]
-        return configurations if not configurations == ["N/A"] else None
+        return None if configurations == ["N/A"] else configurations
 
     @staticmethod
     def normalize_embodiment(embodiment_element: Tag) -> str:
         text = FIPSHTMLParser.normalize_string(embodiment_element.text)
         embodiment_normalization_dict = {
             "Multi-chip embedded": "Multi-Chip Embedded",
             "Multi-chip Standalone": "Multi-Chip Stand Alone",
@@ -185,14 +195,15 @@
     "date_sunset": lambda x: dateutil.parser.parse(x.text).date(),
     "algorithms": getattr(FIPSHTMLParser, "parse_algorithms"),
     "tested_conf": getattr(FIPSHTMLParser, "parse_tested_configurations"),
     "exceptions": lambda x: [y.text for y in x.find_all("li")],
     "status": lambda x: FIPSHTMLParser.normalize_string(x.text).lower(),
     "level": lambda x: int(FIPSHTMLParser.normalize_string(x.text)),
     "embodiment": getattr(FIPSHTMLParser, "normalize_embodiment"),
+    "module_type": getattr(FIPSHTMLParser, "normalize_type"),
 }
 
 
 class FIPSCertificate(
     Certificate["FIPSCertificate", "FIPSCertificate.Heuristics", "FIPSCertificate.PdfData"],
     PandasSerializableType,
     ComplexSerializableType,
@@ -244,17 +255,17 @@
 
         module_extract_ok: bool
         policy_extract_ok: bool
 
         policy_pdf_hash: str | None
         policy_txt_hash: str | None
 
-        policy_pdf_path: Path
-        policy_txt_path: Path
-        module_html_path: Path
+        _policy_pdf_path: Path | None = None
+        _policy_txt_path: Path | None = None
+        _module_html_path: Path | None = None
 
         def __init__(
             self,
             module_download_ok: bool = False,
             policy_download_ok: bool = False,
             policy_convert_garbage: bool = False,
             policy_convert_ok: bool = False,
@@ -269,14 +280,44 @@
             self.policy_convert_ok = policy_convert_ok
             self.module_extract_ok = module_extract_ok
             self.policy_extract_ok = policy_extract_ok
             self.policy_pdf_hash = policy_pdf_hash
             self.policy_txt_hash = policy_txt_hash
 
         @property
+        def policy_pdf_path(self) -> Path:
+            if not self._policy_pdf_path:
+                raise ValueError(f"policy_pdf_path not set on {type(self)}")
+            return self._policy_pdf_path
+
+        @policy_pdf_path.setter
+        def policy_pdf_path(self, pth: str | Path | None) -> None:
+            self._policy_pdf_path = Path(pth) if pth else None
+
+        @property
+        def policy_txt_path(self) -> Path:
+            if not self._policy_txt_path:
+                raise ValueError(f"policy_txt_path not set on {type(self)}")
+            return self._policy_txt_path
+
+        @policy_txt_path.setter
+        def policy_txt_path(self, pth: str | Path | None) -> None:
+            self._policy_txt_path = Path(pth) if pth else None
+
+        @property
+        def module_html_path(self) -> Path:
+            if not self._module_html_path:
+                raise ValueError(f"module_html_path not set on {type(self)}")
+            return self._module_html_path
+
+        @module_html_path.setter
+        def module_html_path(self, pth: str | Path | None) -> None:
+            self._module_html_path = Path(pth) if pth else None
+
+        @property
         def serialized_attributes(self) -> list[str]:
             return [
                 "module_download_ok",
                 "policy_download_ok",
                 "policy_convert_garbage",
                 "policy_convert_ok",
                 "module_extract_ok",
@@ -385,16 +426,16 @@
         keywords: dict = field(default_factory=dict)
         policy_metadata: dict[str, Any] = field(default_factory=dict)
 
         @property
         def certlike_algorithm_numbers(self) -> set[str]:
             """Returns numbers of certificates from keywords["fips_certlike"]["Certlike"]"""
             if self.keywords and "fips_certlike" in self.keywords:
-                fips_certlike = self.keywords["fips_certlike"].get("Certlike", dict())
-                matches = {re.search(r"#\s{0,1}\d{1,4}", x) for x in fips_certlike.keys()}
+                fips_certlike = self.keywords["fips_certlike"].get("Certlike", {})
+                matches = {re.search(r"#\s{0,1}\d{1,4}", x) for x in fips_certlike}
                 return {"".join([x for x in match.group() if x.isdigit()]) for match in matches if match}
             else:
                 return set()
 
     @dataclass(eq=True)
     class Heuristics(BaseHeuristics, ComplexSerializableType):
         """
@@ -459,15 +500,15 @@
             + "\n"
             + "FW version: "
             + str(self.web_data.fw_versions)
         )
 
     def __init__(
         self,
-        cert_id: str,
+        cert_id: int,
         web_data: FIPSCertificate.WebData | None = None,
         pdf_data: FIPSCertificate.PdfData | None = None,
         heuristics: FIPSCertificate.Heuristics | None = None,
         state: InternalState | None = None,
     ):
         super().__init__()
 
@@ -539,17 +580,15 @@
         return cert
 
     @staticmethod
     def convert_policy_pdf(cert: FIPSCertificate) -> FIPSCertificate:
         """
         Converts policy pdf -> txt
         """
-        ocr_done, ok_result = sec_certs.utils.pdf.convert_pdf_file(
-            cert.state.policy_pdf_path, cert.state.policy_txt_path
-        )
+        ocr_done, ok_result = pdf.convert_pdf_file(cert.state.policy_pdf_path, cert.state.policy_txt_path)
 
         # If OCR was done and the result was garbage
         cert.state.policy_convert_garbage = ocr_done
         # And put the whole result into convert_ok
         cert.state.policy_convert_ok = ok_result
 
         if not ok_result:
@@ -561,41 +600,43 @@
         return cert
 
     @staticmethod
     def extract_policy_pdf_metadata(cert: FIPSCertificate) -> FIPSCertificate:
         """
         Extract the PDF metadata from the security policy.
         """
-        _, metadata = sec_certs.utils.pdf.extract_pdf_metadata(cert.state.policy_pdf_path)
+        _, metadata = pdf.extract_pdf_metadata(cert.state.policy_pdf_path)
 
         if metadata:
             cert.pdf_data.policy_metadata = metadata
         else:
-            cert.pdf_data.policy_metadata = dict()
+            cert.pdf_data.policy_metadata = {}
             cert.state.policy_extract_ok = False
         return cert
 
     @staticmethod
     def extract_policy_pdf_keywords(cert: FIPSCertificate) -> FIPSCertificate:
         """
         Extract keywords from policy document
         """
-        keywords = sec_certs.utils.extract.extract_keywords(cert.state.policy_txt_path, fips_rules)
+        keywords = extract.extract_keywords(cert.state.policy_txt_path, fips_rules)
         if not keywords:
             cert.state.policy_extract_ok = False
         else:
             cert.pdf_data.keywords = keywords
         return cert
 
     @staticmethod
     def get_algorithms_from_policy_tables(cert: FIPSCertificate):
         """
         Retrieves IDs of algorithms from tables inside security policy pdfs.
         External library is used to handle this.
         """
+        from tabula import read_pdf
+
         if table_rich_page_numbers := tables.find_pages_with_tables(cert.state.policy_txt_path):
             pdf.repair_pdf(cert.state.policy_pdf_path)
             try:
                 tabular_data = read_pdf(cert.state.policy_pdf_path, pages=list(table_rich_page_numbers), silent=True)
                 cert.heuristics.algorithms |= set(
                     itertools.chain.from_iterable(
                         tables.get_algs_from_table(df.to_string())
@@ -614,15 +655,15 @@
         heuristics.prunned_module_references and heuristics.prunned_policy_references. These variables are further
         processed and Reference objects are created from them.
         """
         html_module_ids = set(self.web_data.mentioned_certs.keys()) if self.web_data.mentioned_certs else set()
         self.heuristics.module_prunned_references = self._prune_reference_ids_variable(html_module_ids)
 
         if self.pdf_data.keywords:
-            pdf_policy_ids = set(self.pdf_data.keywords["fips_cert_id"].get("Cert", dict()).keys())
+            pdf_policy_ids = set(self.pdf_data.keywords["fips_cert_id"].get("Cert", {}).keys())
             pdf_policy_ids = {"".join([y for y in x if y.isdigit()]) for x in pdf_policy_ids}
         else:
             pdf_policy_ids = set()
 
         self.heuristics.policy_prunned_references = self._prune_reference_ids_variable(pdf_policy_ids)
 
     def compute_heuristics_version(self) -> None:
@@ -642,13 +683,11 @@
         """
         Prunnes cert_ids from variable "attribute_to_prune", return result. Steps:
             0. Consider only ids != self.cert_id
             1. Consider only ids > config.always_false_positive_fips_cert_id_threshold
             2. Consider only ids s.t. they don't appear in self.heuristics.algorithms
             3. Consider only ids s.t. they don't appear in self.pdf_data.keywords["fips_certlike"]["Certlike"]
         """
-        prunned = {x for x in attribute_to_prune if x != self.cert_id}
+        prunned = {x for x in attribute_to_prune if x != str(self.cert_id)}
         prunned = {x for x in prunned if int(x) > config.always_false_positive_fips_cert_id_threshold}
         prunned = {x for x in prunned if x not in self.heuristics.algorithm_numbers}
-        prunned = {x for x in prunned if x not in self.pdf_data.certlike_algorithm_numbers}
-
-        return prunned
+        return {x for x in prunned if x not in self.pdf_data.certlike_algorithm_numbers}
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/fips_algorithm.py` & `sec-certs-0.1.4/src/sec_certs/sample/fips_algorithm.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/fips_iut.py` & `sec-certs-0.1.4/src/sec_certs/sample/fips_iut.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tempfile import NamedTemporaryFile
 from typing import Iterator, Mapping
 
 import requests
 from bs4 import BeautifulSoup, Tag
 
 from sec_certs import constants
-from sec_certs.config.configuration import config
+from sec_certs.configuration import config
 from sec_certs.serialization.json import ComplexSerializableType
 from sec_certs.utils.helpers import to_utc
 
 
 @dataclass(frozen=True)
 class IUTEntry(ComplexSerializableType):
     module_name: str
@@ -97,15 +97,15 @@
         entries = {
             IUTEntry(
                 str(line[0].string),
                 str(line[1].string),
                 str(line[2].string),
                 datetime.strptime(str(line[3].string), "%m/%d/%Y").date(),
             )
-            for line in map(lambda tr: tr.find_all("td"), lines)
+            for line in (tr.find_all("td") for tr in lines)
         }
 
         # Parse footer
         footer = soup.find(id="IUTFooter")
         displayed: int | None
         not_displayed: int | None
         total: int | None
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/fips_mip.py` & `sec-certs-0.1.4/src/sec_certs/sample/fips_mip.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,91 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from datetime import date, datetime
 from enum import Enum
+from functools import total_ordering
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Iterator, Mapping
 
 import requests
 from bs4 import BeautifulSoup, Tag
 
 from sec_certs import constants
-from sec_certs.config.configuration import config
+from sec_certs.configuration import config
 from sec_certs.constants import FIPS_MIP_STATUS_RE
 from sec_certs.serialization.json import ComplexSerializableType
 from sec_certs.utils.helpers import to_utc
 
 logger = logging.getLogger(__name__)
 
 
+@total_ordering
 class MIPStatus(Enum):
     IN_REVIEW = "In Review"
     REVIEW_PENDING = "Review Pending"
     COORDINATION = "Coordination"
     FINALIZATION = "Finalization"
 
+    def __lt__(self, other):
+        if self.__class__ == other.__class__:
+            mb = list(MIPStatus.__members__.keys())
+            return mb.index(self.name) < mb.index(other.name)
+        raise NotImplementedError
 
-@dataclass(frozen=True)
+
+@dataclass(frozen=True, order=True)
 class MIPEntry(ComplexSerializableType):
     module_name: str
     vendor_name: str
     standard: str
-    status: MIPStatus | None
+    status: MIPStatus
     status_since: date | None
 
-    def to_dict(self) -> dict[str, str | MIPStatus | None | date | None]:
+    def to_dict(self) -> dict[str, str | MIPStatus | date | None]:
         return {
             **self.__dict__,
-            "status": self.status.value if self.status else None,
+            "status": self.status.value,
             "status_since": self.status_since.isoformat() if self.status_since else None,
         }
 
     @classmethod
     def from_dict(cls, dct: Mapping) -> MIPEntry:
         return cls(
             dct["module_name"],
             dct["vendor_name"],
             dct["standard"],
-            MIPStatus(dct["status"]) if dct["status"] else None,
+            MIPStatus(dct["status"]),
             date.fromisoformat(dct["status_since"]) if dct.get("status_since") else None,
         )
 
 
 @dataclass
+class MIPFlow(ComplexSerializableType):
+    module_name: str
+    vendor_name: str
+    standard: str
+    state_changes: list[tuple[date, MIPStatus]]
+
+    def to_dict(self) -> dict[str, str | list]:
+        return {**self.__dict__, "state_changes": [(dt.isoformat(), status.value) for dt, status in self.state_changes]}
+
+    @classmethod
+    def from_dict(cls, dct: Mapping) -> MIPFlow:
+        return cls(
+            dct["module_name"],
+            dct["vendor_name"],
+            dct["standard"],
+            [(date.fromisoformat(dt), MIPStatus(status)) for dt, status in dct["state_changes"]],
+        )
+
+
+@dataclass
 class MIPSnapshot(ComplexSerializableType):
     entries: set[MIPEntry]
     timestamp: datetime
     last_updated: date
     displayed: int
     not_displayed: int
     total: int
@@ -91,77 +119,76 @@
 
     @classmethod
     def _extract_entries_1(cls, lines):
         """Works until 2020.10.28 (including)."""
         entries = set()
         for tr in lines:
             tds = tr.find_all("td")
-            status = None
             if "mip-highlight" in tds[-1]["class"]:
                 status = MIPStatus.FINALIZATION
             elif "mip-highlight" in tds[-2]["class"]:
                 status = MIPStatus.COORDINATION
             elif "mip-highlight" in tds[-3]["class"]:
                 status = MIPStatus.REVIEW_PENDING
             elif "mip-highlight" in tds[-4]["class"]:
                 status = MIPStatus.IN_REVIEW
+            else:
+                raise ValueError("Cannot parse MIP status line.")
             entries.add(MIPEntry(str(tds[0].string), str(tds[1].string), str(tds[2].string), status, None))
         return entries
 
     @classmethod
     def _extract_entries_2(cls, lines):
         """Works until 2021.04.20 (including)."""
         return {
             MIPEntry(
                 str(line[0].string), str(line[1].string), str(line[2].string), MIPStatus(str(line[3].string)), None
             )
-            for line in map(lambda tr: tr.find_all("td"), lines)
+            for line in (tr.find_all("td") for tr in lines)
         }
 
     @classmethod
     def _extract_entries_3(cls, lines):
         """Works until 2022.03.23 (including)."""
         return {
             MIPEntry(
                 str(line[0].string),
-                str(" ".join(line[1].find_all(text=True, recursive=False)).strip()),
+                str(" ".join(line[1].find_all(string=True, recursive=False)).strip()),
                 str(line[2].string),
                 MIPStatus(str(line[3].string)),
                 None,
             )
-            for line in map(lambda tr: tr.find_all("td"), lines)
+            for line in (tr.find_all("td") for tr in lines)
         }
 
     @classmethod
     def _extract_entries_4(cls, lines):
         """Works now."""
         entries = set()
-        for line in map(lambda tr: tr.find_all("td"), lines):
+        for line in (tr.find_all("td") for tr in lines):
             module_name = str(line[0].string)
-            vendor_name = str(" ".join(line[1].find_all(text=True, recursive=False)).strip())
+            vendor_name = str(" ".join(line[1].find_all(string=True, recursive=False)).strip())
             standard = str(line[2].string)
             status_line = FIPS_MIP_STATUS_RE.match(str(line[3].string))
             if status_line is None:
                 raise ValueError("Cannot parse MIP status line.")
             status = MIPStatus(status_line.group("status"))
             since = datetime.strptime(status_line.group("since"), "%m/%d/%Y").date()
             entries.add(MIPEntry(module_name, vendor_name, standard, status, since))
         return entries
 
     @classmethod
     def _extract_entries(cls, lines, snapshot_date):
         if snapshot_date <= datetime(2020, 10, 28):
-            entries = cls._extract_entries_1(lines)
-        elif snapshot_date <= datetime(2021, 4, 20):
-            entries = cls._extract_entries_2(lines)
-        elif snapshot_date <= datetime(2022, 3, 23):
-            entries = cls._extract_entries_3(lines)
-        else:
-            entries = cls._extract_entries_4(lines)
-        return entries
+            return cls._extract_entries_1(lines)
+        if snapshot_date <= datetime(2021, 4, 20):
+            return cls._extract_entries_2(lines)
+        if snapshot_date <= datetime(2022, 3, 23):
+            return cls._extract_entries_3(lines)
+        return cls._extract_entries_4(lines)
 
     @classmethod
     def from_page(cls, content: bytes, snapshot_date: datetime) -> MIPSnapshot:
         """
         Get a MIP snapshot from a HTML dump of the FIPS website.
         """
         if not content:
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/protection_profile.py` & `sec-certs-0.1.4/src/sec_certs/sample/protection_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import copy
 import logging
 from dataclasses import dataclass
 from typing import Any
 
-import sec_certs.utils.sanitization as sanitization
 from sec_certs.serialization.json import ComplexSerializableType
+from sec_certs.utils import sanitization
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class ProtectionProfile(ComplexSerializableType):
     """
```

### Comparing `sec-certs-0.1.3/src/sec_certs/sample/sar.py` & `sec-certs-0.1.4/src/sec_certs/sample/sar.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "AGD": "Guidance documents",
     "ALC": "Life-cycle support",
     "ATE": "Tests",
     "AVA": "Vulnerability assessment",
     "ACO": "Comoposition",
 }
 
-SAR_CLASSES = {x for x in SAR_CLASS_MAPPING}
+SAR_CLASSES = set(SAR_CLASS_MAPPING)
 SAR_DICT_KEY = "cc_sar"
 
 
 @dataclass(frozen=True, eq=True)
 class SAR(ComplexSerializableType):
     family: str
     level: int
```

### Comparing `sec-certs-0.1.3/src/sec_certs/serialization/json.py` & `sec-certs-0.1.4/src/sec_certs/serialization/json.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import copy
+import gzip
 import json
-from datetime import date
+from datetime import date, datetime
 from functools import wraps
 from pathlib import Path
 from typing import Any, Callable, TypeVar
 
 from sec_certs import constants
 
 T = TypeVar("T", bound="ComplexSerializableType")
@@ -40,15 +41,20 @@
     @classmethod
     def from_dict(cls: type[T], dct: dict) -> T:
         try:
             return cls(**dct)
         except TypeError as e:
             raise TypeError(f"Dict: {dct} on {cls.__mro__}") from e
 
-    def to_json(self, output_path: str | Path | None = None) -> None:
+    def to_json(self, output_path: str | Path | None = None, compress: bool = False) -> None:
+        """
+        Serializes `ComplexSerializableType` instance to json file.
+        :param str | Path | None output_path: path where the file will be stored. If None, `obj.json_path` access is attempted, defaults to None
+        :param bool compress: if True, will be compress with gzip, defaults to False
+        """
         if not output_path and (not hasattr(self, "json_path") or not self.json_path):  # type: ignore
             raise SerializationError(
                 f"The object {self} of type {self.__class__} does not have json_path attribute set but to_json() was called without an argument."
             )
         if not output_path:
             output_path = self.json_path  # type: ignore
             if self.json_path == constants.DUMMY_NONEXISTING_PATH:  # type: ignore
@@ -56,29 +62,41 @@
             if hasattr(self, "root_dir") and self.root_dir == constants.DUMMY_NONEXISTING_PATH:  # type: ignore
                 raise SerializationError(f"root_dir attribute for '{get_class_fullname(self)}' was not yet set.")
 
         if Path(output_path).is_dir():  # type: ignore
             raise SerializationError("output path for json cannot be directory.")
 
         # false positive MyPy warning, cannot be None
-        with Path(output_path).open("w") as handle:  # type: ignore
-            json.dump(self, handle, indent=4, cls=CustomJSONEncoder, ensure_ascii=False)
+        if compress:
+            with gzip.open(str(output_path), "wt", encoding="utf-8") as handle:  # type: ignore
+                json.dump(self, handle, indent=4, cls=CustomJSONEncoder, ensure_ascii=False)
+        else:
+            with Path(output_path).open("w") as handle:  # type: ignore
+                json.dump(self, handle, indent=4, cls=CustomJSONEncoder, ensure_ascii=False)
 
     @classmethod
-    def from_json(cls: type[T], input_path: str | Path) -> T:
-        input_path = Path(input_path)
-        with input_path.open("r") as handle:
-            obj = json.load(handle, cls=CustomJSONDecoder)
-        return obj
+    def from_json(cls: type[T], input_path: str | Path, is_compressed: bool = False) -> T:
+        """
+        Will load `ComplexSerializableType` from json.
+        :param str | Path input_path: path to load the file from
+        :param bool is_compressed: if True, will decompress .gz first, defaults to False
+        :return T: the deserialized object
+        """
+        if is_compressed:
+            with gzip.open(str(input_path), "rt", encoding="utf-8") as handle:
+                return json.load(handle, cls=CustomJSONDecoder)
+        else:
+            with Path(input_path).open("r") as handle:
+                return json.load(handle, cls=CustomJSONDecoder)
 
 
 # Decorator for serialization
 def serialize(func: Callable):
     @wraps(func)
-    def inner_func(*args, **kwargs):
+    def _serialize(*args, **kwargs):
         if not args or not issubclass(type(args[0]), ComplexSerializableType):
             raise ValueError(
                 "@serialize decorator is to be used only on instance methods of ComplexSerializableType child classes."
             )
 
         if hasattr(args[0], "_root_dir") and args[0]._root_dir == constants.DUMMY_NONEXISTING_PATH:
             raise SerializationError(
@@ -87,40 +105,39 @@
 
         update_json = kwargs.pop("update_json", True)
         result = func(*args, **kwargs)
         if update_json:
             args[0].to_json()
         return result
 
-    return inner_func
+    return _serialize
 
 
 def get_class_fullname(obj: Any) -> str:
-    if isinstance(obj, type):
-        klass = obj
-    else:
-        klass = obj.__class__
+    klass = obj if isinstance(obj, type) else obj.__class__
     module = klass.__module__
     if module == "builtins":
         return klass.__qualname__
     return module + "." + klass.__qualname__
 
 
 class CustomJSONEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, ComplexSerializableType):
             return {**{"_type": get_class_fullname(obj)}, **obj.to_dict()}
         if isinstance(obj, dict):
             return obj
         if isinstance(obj, set):
-            return {"_type": "Set", "elements": sorted(list(obj))}
+            return {"_type": "Set", "elements": sorted(obj)}
         if isinstance(obj, frozenset):
-            return sorted(list(obj))
+            return sorted(obj)
         if isinstance(obj, date):
             return str(obj)
+        if isinstance(obj, datetime):
+            return obj.isoformat()
         if isinstance(obj, Path):
             return str(obj)
         return super().default(obj)
 
 
 class CustomJSONDecoder(json.JSONDecoder):
     """
@@ -132,14 +149,14 @@
     def __init__(self, *args, **kwargs):
         json.JSONDecoder.__init__(self, object_hook=self.object_hook, *args, **kwargs)
         self.serializable_complex_types = {get_class_fullname(x): x for x in ComplexSerializableType.__subclasses__()}
 
     def object_hook(self, obj):
         if "_type" in obj and obj["_type"] == "Set":
             return set(obj["elements"])
-        if "_type" in obj and obj["_type"] in self.serializable_complex_types.keys():
+        if "_type" in obj and obj["_type"] in self.serializable_complex_types:
             complex_type = obj.pop("_type")
             return self.serializable_complex_types[complex_type].from_dict(obj)
-        elif "_type" in obj:
+        if "_type" in obj:
             raise SerializationError(f"JSONDecoder doesn't know how to handle {obj}")
 
         return obj
```

### Comparing `sec-certs-0.1.3/src/sec_certs/utils/extract.py` & `sec-certs-0.1.4/src/sec_certs/utils/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import logging
 import os
 import re
 from collections import Counter
 from enum import Enum
 from pathlib import Path
-from typing import Any, Iterator
+from typing import Any
 
 import numpy as np
 
-from sec_certs import constants as constants
+from sec_certs import constants
 from sec_certs.cert_rules import REGEXEC_SEP, cc_rules
 from sec_certs.constants import FILE_ERRORS_STRATEGY, LINE_SEPARATOR, MAX_ALLOWED_MATCH_LENGTH
 
 logger = logging.getLogger(__name__)
 
 
 def search_only_headers_anssi(filepath: Path):  # noqa: C901
@@ -581,19 +581,14 @@
         error_msg = f"Failed to parse Canada headers from frontpage: {filepath}; {e}"
         logger.error(error_msg)
         return error_msg, None
 
     return constants.RETURNCODE_OK, items_found
 
 
-def search_files(folder: str | Path) -> Iterator[str]:
-    for root, _, files in os.walk(str(folder)):
-        yield from [os.path.join(root, x) for x in files]
-
-
 def flatten_matches(dct: dict) -> dict:
     """
     Function to flatten dictionary of matches.
 
     Turns
     ```
         {"a": {"cc": 3}, "b": {}, "d": {"dd": 4, "cc": 2}}
@@ -659,21 +654,21 @@
 
     try:
         whole_text, whole_text_with_newlines, was_unicode_decode_error = load_text_file(filepath, -1, LINE_SEPARATOR)
 
         def extract(rules):
             if isinstance(rules, dict):
                 return {k: extract(v) for k, v in rules.items()}
-            elif isinstance(rules, list):
+            if isinstance(rules, list):
                 matches = [extract(rule) for rule in rules]
                 c = Counter()
                 for match_list in matches:
                     c += Counter(match_list)
                 return dict(c)
-            elif isinstance(rules, re.Pattern):
+            if isinstance(rules, re.Pattern):
                 rule = rules
                 matches = []
                 for match in rule.finditer(whole_text):
                     match = match.group("match")
                     match = normalize_match_string(match)
 
                     match_len = len(match)
@@ -715,15 +710,15 @@
         try:
             lines = f.readlines()
         except UnicodeDecodeError:
             was_unicode_decode_error = True
             logger.warning("UnicodeDecodeError, opening as utf8")
 
     if was_unicode_decode_error:
-        with open(file_name, encoding="utf8", errors=FILE_ERRORS_STRATEGY) as f2:
+        with Path(file_name).open("r", encoding="utf8", errors=FILE_ERRORS_STRATEGY) as f2:
             # coding failure, try line by line
             line = " "
             while line:
                 try:
                     line = f2.readline()
                     lines.append(line)
                 except UnicodeDecodeError:
@@ -742,31 +737,39 @@
         whole_text += line
         whole_text += line_separator
         lines_included += 1
 
     return whole_text, whole_text_with_newlines, was_unicode_decode_error
 
 
-def load_cert_html_file(file_name: str) -> str:
-    with open(file_name, errors=FILE_ERRORS_STRATEGY) as f:
-        try:
-            return f.read()
-        except UnicodeDecodeError:
-            logger.warning("UnicodeDecodeError, opening as utf8")
+def rules_get_subset(desired_path: str) -> dict:
+    """
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
-    with open(file_name, encoding="utf8", errors=FILE_ERRORS_STRATEGY) as f2:
-        try:
-            return f2.read()
-        except UnicodeDecodeError:
-            logger.error(f"Failed to read file {file_name}")
-    return ""
 
 
-def rules_get_subset(desired_path: str) -> dict:
-    """
     Recursively applies cc_certs.get(key) on tokens from desired_path,
     returns the keys of the inner-most layer.
     """
     dct = cc_rules
     for token in desired_path.split("."):
         dct = dct[token]
     return dct
```

### Comparing `sec-certs-0.1.3/src/sec_certs/utils/helpers.py` & `sec-certs-0.1.4/src/sec_certs/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pathlib import Path
 from typing import Any, Collection
 
 import numpy as np
 import pkgconfig
 import requests
 
-import sec_certs.constants as constants
+from sec_certs import constants
 from sec_certs.utils import parallel_processing
 from sec_certs.utils.tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 
 
 def download_file(
@@ -40,20 +40,19 @@
                 unit_divisor=1024,
                 desc=progress_bar_desc,
             )
         else:
             ctx = nullcontext
 
         if r.status_code == requests.codes.ok:
-            with ctx() as pbar:
-                with output.open("wb") as f:
-                    for data in r.iter_content(1024):
-                        f.write(data)
-                        if show_progress_bar:
-                            pbar.update(len(data))
+            with ctx() as pbar, output.open("wb") as f:
+                for data in r.iter_content(1024):
+                    f.write(data)
+                    if show_progress_bar:
+                        pbar.update(len(data))
 
             return r.status_code
     except requests.exceptions.Timeout:
         return requests.codes.timeout
     except Exception as e:
         logger.error(f"Failed to download from {url}; {e}")
         return constants.RETURNCODE_NOK
@@ -93,25 +92,23 @@
 
 
 def to_utc(timestamp: datetime) -> datetime:
     offset = timestamp.utcoffset()
     if offset is None:
         return timestamp
     timestamp -= offset
-    timestamp = timestamp.replace(tzinfo=None)
-    return timestamp
+    return timestamp.replace(tzinfo=None)
 
 
 def is_in_dict(target_dict: dict, path: str) -> bool:
     current_level = target_dict
     for item in path:
         if item not in current_level:
             return False
-        else:
-            current_level = current_level[item]
+        current_level = current_level[item]
     return True
 
 
 def compute_heuristics_version(cert_name: str) -> set[str]:
     """
     Will extract possible versions from the name of sample
     """
```

### Comparing `sec-certs-0.1.3/src/sec_certs/utils/pandas.py` & `sec-certs-0.1.4/src/sec_certs/utils/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     return list(families)
 
 
 def get_sar_level_from_set(sars: set[SAR], sar_family: str) -> int | None:
     """
     Given a set of SARs and a family name, will return level of the seeked SAR from the set.
     """
-    family_sars_dict = {x.family: x for x in sars} if (sars and not pd.isnull(sars)) else dict()
+    family_sars_dict = {x.family: x for x in sars} if (sars and not pd.isnull(sars)) else {}
     if sar_family not in family_sars_dict.keys():
         return None
     return family_sars_dict[sar_family].level
 
 
 def compute_cve_correlations(
     df: pd.DataFrame,
@@ -248,15 +248,14 @@
     Filters the column `related_cves` in `cc_df` DataFrame to CVEs that were published within validity period of the
     studied certificate.
     """
 
     def filter_cves(
         cve_dset: CVEDataset, cves: set[str], not_valid_before: pd.Timestamp, not_valid_after: pd.Timestamp
     ) -> set[str] | float:
-
         # Mypy is complaining, but the Optional date is resolved at the beginning of the and condition
         result: set[str] = {
             x
             for x in cves
             if cve_dset[x].published_date
             and not_valid_before < pd.Timestamp(cve_dset[x].published_date.date())  # type: ignore
             and not_valid_after > pd.Timestamp(cve_dset[x].published_date.date())  # type: ignore
@@ -282,33 +281,32 @@
     )
 
     return cc_df
 
 
 def expand_df_with_cve_cols(df: pd.DataFrame, cve_dset: CVEDataset) -> pd.DataFrame:
     df = df.copy()
-
-    df["n_cves"] = df.related_cves.map(lambda x: len(x) if x is not np.nan else 0)
+    df["n_cves"] = df.related_cves.map(lambda x: 0 if pd.isna(x) else len(x))
     df["cve_published_dates"] = df.related_cves.map(
-        lambda x: [cve_dset[y].published_date.date() for y in x] if x is not np.nan else np.nan  # type: ignore
+        lambda x: [cve_dset[y].published_date.date() for y in x] if not pd.isna(x) else np.nan  # type: ignore
     )
 
     df["earliest_cve"] = df.cve_published_dates.map(lambda x: min(x) if isinstance(x, list) else np.nan)
     df["worst_cve_score"] = df.related_cves.map(
-        lambda x: max([cve_dset[cve].impact.base_score for cve in x]) if x is not np.nan else np.nan
+        lambda x: max([cve_dset[cve].metrics.base_score for cve in x]) if not pd.isna(x) else np.nan
     )
 
     """
     Note: Technically, CVE can have 0 base score. This happens when the CVE is discarded from the database.
     This could skew the results. During May 2022 analysis, we encountered a single CVE with such score.
     Therefore, we do not treat this case.
     To properly treat this, the average should be taken across CVEs with >0 base_socre.
     """
     df["avg_cve_score"] = df.related_cves.map(
-        lambda x: np.mean([cve_dset[cve].impact.base_score for cve in x]) if x is not np.nan else np.nan
+        lambda x: np.mean([cve_dset[cve].metrics.base_score for cve in x]) if not pd.isna(x) else np.nan
     )
     return df
 
 
 def prepare_cwe_df(
     cc_df: pd.DataFrame, cve_dset: CVEDataset, fine_grained: bool = False
 ) -> tuple[pd.DataFrame, pd.DataFrame]:
```

### Comparing `sec-certs-0.1.3/src/sec_certs/utils/parallel_processing.py` & `sec-certs-0.1.4/src/sec_certs/utils/parallel_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from __future__ import annotations
 
 import time
 from multiprocessing import cpu_count
-from multiprocessing.pool import ThreadPool
+from multiprocessing.pool import Pool, ThreadPool
 from typing import Any, Callable, Iterable
 
-from billiard.pool import Pool
-
-from sec_certs.config.configuration import config
+from sec_certs.configuration import config
 from sec_certs.utils.tqdm import tqdm
 
 
 def process_parallel(
     func: Callable,
     items: Iterable,
     max_workers: int = config.n_threads,
     callback: Callable | None = None,
     use_threading: bool = True,
     progress_bar: bool = True,
     unpack: bool = False,
     progress_bar_desc: str | None = None,
 ) -> list[Any]:
-
     if max_workers == -1:
         max_workers = cpu_count()
 
     pool: Pool | ThreadPool = ThreadPool(max_workers) if use_threading else Pool(max_workers)
     results = (
         [pool.apply_async(func, (*i,), callback=callback) for i in items]
         if unpack
```

### Comparing `sec-certs-0.1.3/src/sec_certs/utils/sanitization.py` & `sec-certs-0.1.4/src/sec_certs/utils/sanitization.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         return None
     return record.replace(":443", "").replace(" ", "%20").replace("http://", "https://")
 
 
 def sanitize_date(record: pd.Timestamp | date | np.datetime64) -> date | None:
     if pd.isnull(record):
         return None
-    elif isinstance(record, pd.Timestamp):
+    if isinstance(record, pd.Timestamp):
         return record.date()
-    elif isinstance(record, (date, type(None))):
+    if isinstance(record, (date, type(None))):
         return record
     raise ValueError("Unsupported type given as input")
 
 
 def sanitize_string(record: str) -> str:
     # There is a sample with name 'ATMEL Secure Microcontroller AT90SC12872RCFT &#x2f; AT90SC12836RCFT rev. I &amp;&#x23;38&#x3b; J' that has to be unescaped twice
     string = html.unescape(html.unescape(record)).replace("\n", "")
```

### Comparing `sec-certs-0.1.3/src/sec_certs/utils/tables.py` & `sec-certs-0.1.4/src/sec_certs/utils/tables.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/src/sec_certs.egg-info/PKG-INFO` & `sec-certs-0.1.4/src/sec_certs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-certs
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for data scraping and analysis of security certificates from Common Criteria and FIPS 140-2/3 frameworks
 Author: Jan Jancar, Petr Svenda, Jiri Michalik, Stanislav Bobon
 Author-email: Adam Janovsky <adamjanovsky@mail.muni.cz>
 License: MIT
 Project-URL: Homepage, https://seccerts.org
 Project-URL: GitHub, https://github.com/crocs-muni/sec-certs/
 Project-URL: Documentation, https://seccerts.org/docs
@@ -79,7 +79,13 @@
 
 # Get certificates from 2015 and newer
 df_2015_and_newer = df.loc[df.year_from > 2014]
 
 # Plot distribution of years of certification
 df.year_from.value_counts().sort_index().plot.line()
 ```
+
+## Authors
+
+This work is being done at [CRoCS MUNI](https://crocs.fi.muni.cz/) by Adam Janovsky, Jan Jancar, Petr Svenda, Jiri Michalik, Lukasz Chmielewski and other contributors. This work was supported by the Internal grant agency of Masaryk University, CZ.02.2.69/0.0/0.0/19_073/0016943.
+
+![](docs/_static/logolink_OP_VVV_hor_barva_eng.jpg)
```

### Comparing `sec-certs-0.1.3/src/sec_certs.egg-info/SOURCES.txt` & `sec-certs-0.1.4/src/sec_certs.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.flake8
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 Dockerfile
 LICENSE
 README.md
@@ -20,16 +19,24 @@
 data/cert_id_eval/duplicate_ids.csv
 data/cert_id_eval/missing_ids.csv
 data/cert_id_eval/random.csv
 data/cert_id_eval/random_references.csv
 data/cert_id_eval/truth.csv
 data/cpe_eval/manual_cpe_labels.json
 data/cpe_eval/random.csv
+data/information_retrieval_split/metadata.csv
+data/information_retrieval_split/sampled_images.json
+data/information_retrieval_split/test.json
+data/information_retrieval_split/train.json
+data/information_retrieval_split/valid.json
 data/old_manual_cpe_labels/cc.json
 data/old_manual_cpe_labels/fips.json
+data/reference_annotations_split/test.json
+data/reference_annotations_split/train.json
+data/reference_annotations_split/valid.json
 data/sar_correlations/all_certs_sar_cve_corr.csv
 data/sar_correlations/readme.md
 data/sar_correlations/vuln_rich_certs_sar_cve_corr.csv
 data/validation_test_split/cc/test.json
 data/validation_test_split/cc/validation.json
 data/validation_test_split/fips/test.json
 data/validation_test_split/fips/validation.json
@@ -41,80 +48,88 @@
 docs/index.md
 docs/installation.md
 docs/license.md
 docs/make.bat
 docs/notebooks
 docs/quickstart.md
 docs/readme.md
+docs/user_guide.md
 docs/_static/logo.png
 docs/_static/logo.svg
 docs/_static/logo_badge.png
 docs/_static/logo_badge.svg
+docs/_static/logolink_OP_VVV_hor_barva_eng.jpg
 docs/api/dataset.md
 docs/api/model.md
 docs/api/sample.md
 notebooks/final_run.ipynb
 notebooks/latex_plotting.ipynb
 notebooks/ocr.ipynb
 notebooks/cc/cert_id_eval.ipynb
 notebooks/cc/cpe_eval.ipynb
 notebooks/cc/references.ipynb
 notebooks/cc/temporal_trends.ipynb
 notebooks/cc/vulnerabilities.ipynb
+notebooks/cc/reference_annotations/train_validation_test_split.ipynb
 notebooks/examples/cc.ipynb
+notebooks/examples/est_solution.ipynb
 notebooks/examples/fips.ipynb
 notebooks/examples/fips_iut.ipynb
 notebooks/examples/fips_mip.ipynb
 notebooks/examples/model.ipynb
+notebooks/examples/img/boxplot_validity.png
+notebooks/examples/img/cves_n_days_after_certification.png
 notebooks/fips/in_process.ipynb
 notebooks/fips/references.ipynb
 notebooks/fips/temporal_trends.ipynb
 notebooks/fips/vulnerabilities.ipynb
 requirements/compile.sh
 requirements/dev_requirements.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
 src/sec_certs/__init__.py
 src/sec_certs/__main__.py
 src/sec_certs/_version.py
 src/sec_certs/cert_rules.py
 src/sec_certs/cli.py
+src/sec_certs/configuration.py
 src/sec_certs/constants.py
 src/sec_certs/rules.yaml
 src/sec_certs.egg-info/PKG-INFO
 src/sec_certs.egg-info/SOURCES.txt
 src/sec_certs.egg-info/dependency_links.txt
 src/sec_certs.egg-info/entry_points.txt
 src/sec_certs.egg-info/requires.txt
 src/sec_certs.egg-info/top_level.txt
-src/sec_certs/config/__init__.py
-src/sec_certs/config/configuration.py
-src/sec_certs/config/settings-schema.json
-src/sec_certs/config/settings.yaml
 src/sec_certs/dataset/__init__.py
 src/sec_certs/dataset/cc.py
+src/sec_certs/dataset/cc_scheme.py
 src/sec_certs/dataset/cpe.py
 src/sec_certs/dataset/cve.py
 src/sec_certs/dataset/dataset.py
 src/sec_certs/dataset/fips.py
 src/sec_certs/dataset/fips_algorithm.py
 src/sec_certs/dataset/fips_iut.py
 src/sec_certs/dataset/fips_mip.py
 src/sec_certs/dataset/json_path_dataset.py
 src/sec_certs/dataset/protection_profile.py
 src/sec_certs/model/__init__.py
+src/sec_certs/model/cc_matching.py
 src/sec_certs/model/cpe_matching.py
 src/sec_certs/model/evaluation.py
+src/sec_certs/model/fips_matching.py
+src/sec_certs/model/matching.py
 src/sec_certs/model/reference_finder.py
 src/sec_certs/model/sar_transformer.py
 src/sec_certs/model/transitive_vulnerability_finder.py
 src/sec_certs/sample/__init__.py
 src/sec_certs/sample/cc.py
 src/sec_certs/sample/cc_certificate_id.py
 src/sec_certs/sample/cc_maintenance_update.py
+src/sec_certs/sample/cc_scheme.py
 src/sec_certs/sample/certificate.py
 src/sec_certs/sample/cpe.py
 src/sec_certs/sample/cve.py
 src/sec_certs/sample/fips.py
 src/sec_certs/sample/fips_algorithm.py
 src/sec_certs/sample/fips_iut.py
 src/sec_certs/sample/fips_mip.py
@@ -122,62 +137,78 @@
 src/sec_certs/sample/sar.py
 src/sec_certs/serialization/__init__.py
 src/sec_certs/serialization/json.py
 src/sec_certs/serialization/pandas.py
 src/sec_certs/utils/__init__.py
 src/sec_certs/utils/extract.py
 src/sec_certs/utils/helpers.py
+src/sec_certs/utils/nvd_dataset_builder.py
 src/sec_certs/utils/pandas.py
 src/sec_certs/utils/parallel_processing.py
 src/sec_certs/utils/pdf.py
 src/sec_certs/utils/sanitization.py
+src/sec_certs/utils/strings.py
 src/sec_certs/utils/tables.py
 src/sec_certs/utils/tqdm.py
 tests/__init__.py
 tests/conftest.py
 tests/test_common.py
+tests/test_config.py
 tests/test_cpe.py
 tests/test_cve.py
+tests/test_cve_matching.py
+tests/test_nvd_dataset_builder.py
+tests/cc/conftest.py
 tests/cc/test_cc_analysis.py
 tests/cc/test_cc_certificate.py
 tests/cc/test_cc_dataset.py
 tests/cc/test_cc_maintenance_updates.py
 tests/cc/test_cc_misc.py
 tests/cc/test_cc_schemes.py
 tests/data/__init__.py
-tests/data/settings_tests.yml
+tests/data/cc/__init__.py
 tests/data/cc/analysis/__init__.py
 tests/data/cc/analysis/cc_full_dataset.json
 tests/data/cc/analysis/reference_dataset.json
 tests/data/cc/analysis/transitive_vulnerability_dataset.json
 tests/data/cc/analysis/vulnerable_dataset.json
-tests/data/cc/analysis/auxillary_datasets/cpe_dataset.json
-tests/data/cc/analysis/auxillary_datasets/cve_dataset.json
 tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf
 tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt
 tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf
 tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt
+tests/data/cc/certificate/__init__.py
 tests/data/cc/certificate/fictional_cert.json
+tests/data/cc/dataset/__init__.py
 tests/data/cc/dataset/cc_products_active.csv
 tests/data/cc/dataset/cc_products_active.html
 tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt
 tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt
 tests/data/cc/dataset/toy_dataset.json
-tests/data/cc/dataset/auxillary_datasets/maintenances/maintenance_updates.json
+tests/data/cc/dataset/auxiliary_datasets/maintenances/maintenance_updates.json
+tests/data/common/__init__.py
+tests/data/common/cpe_dataset.json
+tests/data/common/cpe_match_feed.json
+tests/data/common/cve_dataset.json
+tests/data/common/settings_tests.yml
+tests/data/fips/certificate/__init__.py
 tests/data/fips/certificate/fictional_cert.json
+tests/data/fips/dataset/__init__.py
 tests/data/fips/dataset/alg_dataset.json
 tests/data/fips/dataset/fips_modules_active.html
 tests/data/fips/dataset/fips_modules_historical.html
 tests/data/fips/dataset/fips_modules_revoked.html
 tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt
 tests/data/fips/dataset/toy_dataset.json
+tests/data/fips/iut/__init__.py
 tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html
 tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html
+tests/data/fips/mip/__init__.py
 tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html
 tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html
 tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html
+tests/fips/conftest.py
 tests/fips/test_fips_algorithm_dataset.py
 tests/fips/test_fips_analysis.py
 tests/fips/test_fips_certificate.py
 tests/fips/test_fips_dataset.py
 tests/fips/test_fips_iut.py
 tests/fips/test_fips_mip.py
```

### Comparing `sec-certs-0.1.3/tests/cc/test_cc_analysis.py` & `sec-certs-0.1.4/tests/cc/test_cc_analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,128 +1,86 @@
 from __future__ import annotations
 
 import shutil
+from importlib import resources
 from pathlib import Path
+from typing import Generator
 
 import pytest
-
 import tests.data.cc.analysis
+import tests.data.common
+
 from sec_certs.cert_rules import SARS_IMPLIED_FROM_EAL
-from sec_certs.dataset import CCDataset
+from sec_certs.dataset.cc import CCDataset
 from sec_certs.dataset.cpe import CPEDataset
 from sec_certs.dataset.cve import CVEDataset
 from sec_certs.sample.cc import CCCertificate
-from sec_certs.sample.cpe import CPE
-from sec_certs.sample.cve import CVE
 from sec_certs.sample.protection_profile import ProtectionProfile
 from sec_certs.sample.sar import SAR
 
 
 @pytest.fixture(scope="module")
-def data_dir() -> Path:
-    return Path(tests.data.cc.analysis.__path__[0])
-
-
-@pytest.fixture(scope="module")
-def cpe_single_sign_on() -> CPE:
-    return CPE(
-        "cpe:2.3:a:ibm:security_access_manager_for_enterprise_single_sign-on:8.2.2:*:*:*:*:*:*:*",
-        "IBM Security Access Manager For Enterprise Single Sign-On 8.2.2",
-    )
-
-
-@pytest.fixture(scope="module")
-def cpes(cpe_single_sign_on: CPE) -> set[CPE]:
-    return {
-        cpe_single_sign_on,
-        CPE(
-            "cpe:2.3:a:ibm:security_key_lifecycle_manager:2.6.0.1:*:*:*:*:*:*:*",
-            "IBM Security Key Lifecycle Manager 2.6.0.1",
-        ),
-        CPE(
-            "cpe:2.3:a:semperplugins:all_in_one_seo_pack:1.3.6.4:*:*:*:*:wordpress:*:*",
-            "Semper Plugins All in One SEO Pack 1.3.6.4 for WordPress",
-        ),
-        CPE(
-            "cpe:2.3:a:tracker-software:pdf-xchange_lite_printer:6.0.320.0:*:*:*:*:*:*:*",
-            "Tracker Software PDF-XChange Lite Printer 6.0.320.0",
-        ),
-    }
-
-
-@pytest.fixture(scope="module")
-def cpe_dset(cpes: set[CPE]) -> CPEDataset:
-    return CPEDataset(False, {x.uri: x for x in cpes})
+def analysis_data_dir() -> Generator[Path, None, None]:
+    with resources.path(tests.data.cc.analysis, "") as path:
+        yield path
 
 
 @pytest.fixture(scope="module")
-def cves(cpe_single_sign_on) -> set[CVE]:
-    return {
-        CVE(
-            "CVE-2017-1732",
-            [cpe_single_sign_on],
-            CVE.Impact(5.3, "MEDIUM", 3.9, 1.4),
-            "2021-05-26T04:15Z",
-            {"CWE-200"},
-        ),
-        CVE(
-            "CVE-2019-4513",
-            [cpe_single_sign_on],
-            CVE.Impact(8.2, "HIGH", 3.9, 4.2),
-            "2000-05-26T04:15Z",
-            {"CVE-611"},
-        ),
-    }
-
-
-@pytest.fixture(scope="module")
-def cve_dset(cves: set[CVE]) -> CVEDataset:
-    cve_dset = CVEDataset({x.cve_id: x for x in cves})
-    cve_dset.build_lookup_dict(use_nist_mapping=False)
-    return cve_dset
-
-
-@pytest.fixture(scope="module")
-def cc_dset(data_dir: Path, cve_dset: CVEDataset, tmp_path_factory) -> CCDataset:
+def processed_cc_dset(
+    analysis_data_dir: Path, cve_dataset: CVEDataset, cpe_dataset: CPEDataset, tmp_path_factory
+) -> CCDataset:
     tmp_dir = tmp_path_factory.mktemp("cc_dset")
-    shutil.copytree(data_dir, tmp_dir, dirs_exist_ok=True)
+    shutil.copytree(analysis_data_dir, tmp_dir, dirs_exist_ok=True)
 
     cc_dset = CCDataset.from_json(tmp_dir / "vulnerable_dataset.json")
     cc_dset.process_protection_profiles()
     cc_dset.extract_data()
-    cc_dset.auxillary_datasets.cve_dset = cve_dset
+    cc_dset.auxiliary_datasets.cve_dset = cve_dataset
+    cc_dset.auxiliary_datasets.cpe_dset = cpe_dataset
     cc_dset._compute_heuristics()
+
     return cc_dset
 
 
 @pytest.fixture
-def reference_dataset(data_dir) -> CCDataset:
-    return CCDataset.from_json(data_dir / "reference_dataset.json")
+def reference_dataset(analysis_data_dir) -> CCDataset:
+    return CCDataset.from_json(analysis_data_dir / "reference_dataset.json")
 
 
 @pytest.fixture
-def transitive_vulnerability_dataset(data_dir) -> CCDataset:
-    return CCDataset.from_json(data_dir / "transitive_vulnerability_dataset.json")
+def transitive_vulnerability_dataset(analysis_data_dir) -> CCDataset:
+    return CCDataset.from_json(analysis_data_dir / "transitive_vulnerability_dataset.json")
 
 
 @pytest.fixture
-def random_certificate(cc_dset: CCDataset) -> CCCertificate:
-    return cc_dset["ebd276cca70fd723"]
+def random_certificate(processed_cc_dset: CCDataset) -> CCCertificate:
+    return processed_cc_dset["ebd276cca70fd723"]
+
 
+def test_match_cpe(random_certificate: CCCertificate):
+    assert {
+        "cpe:2.3:a:ibm:security_access_manager_for_enterprise_single_sign-on:8.2.2:*:*:*:*:*:*:*"
+    } == random_certificate.heuristics.cpe_matches
 
-def test_match_cpe(cpe_single_sign_on: CPE, random_certificate: CCCertificate):
-    assert {cpe_single_sign_on.uri} == random_certificate.heuristics.cpe_matches
+
+def test_find_related_cves(processed_cc_dset: CCDataset, random_certificate: CCCertificate):
+    random_certificate.heuristics.cpe_matches = {
+        "cpe:2.3:a:ibm:security_access_manager_for_enterprise_single_sign-on:8.2.2:*:*:*:*:*:*:*"
+    }
+    processed_cc_dset.compute_related_cves()
+    assert random_certificate.heuristics.related_cves == {"CVE-2017-1732", "CVE-2019-4513"}
 
 
-def test_find_related_cves(
-    cc_dset: CCDataset, cpe_single_sign_on: CPE, cves: set[CVE], random_certificate: CCCertificate
-):
-    random_certificate.heuristics.cpe_matches = {cpe_single_sign_on.uri}
-    cc_dset.compute_related_cves()
-    assert {x.cve_id for x in cves} == random_certificate.heuristics.related_cves
+def test_find_related_cves_criteria_configuration(processed_cc_dset: CCDataset, random_certificate: CCCertificate):
+    random_certificate.heuristics.cpe_matches = {
+        "cpe:2.3:a:ibm:websphere_application_server:7.0:*:*:*:*:*:*:*",
+        "cpe:2.3:o:ibm:zos:6.0.1:*:*:*:*:*:*:*",
+    }
+    processed_cc_dset.compute_related_cves()
+    assert random_certificate.heuristics.related_cves == {"CVE-2010-2325"}
 
 
 def test_version_extraction(random_certificate: CCCertificate):
     assert random_certificate.heuristics.extracted_versions == {"8.2"}
 
     new_cert = CCCertificate(
         "",
@@ -170,15 +128,15 @@
     assert "symmetric_crypto" in extracted_keywords
     assert extracted_keywords["symmetric_crypto"]["AES_competition"]["AES"]["AES"] == 2
 
     assert "cipher_mode" in extracted_keywords
     assert extracted_keywords["cipher_mode"]["CBC"]["CBC"] == 2
 
 
-def test_protection_profile_matching(cc_dset: CCDataset, random_certificate: CCCertificate):
+def test_protection_profile_matching(processed_cc_dset: CCDataset, random_certificate: CCCertificate):
     artificial_pp: ProtectionProfile = ProtectionProfile(
         "Korean National Protection Profile for Single Sign On V1.0",
         "EAL1+",
         pp_link="http://www.commoncriteriaportal.org/files/ppfiles/KECS-PP-0822-2017%20Korean%20National%20PP%20for%20Single%20Sign%20On%20V1.0(eng).pdf",
     )
 
     random_certificate.protection_profiles = {artificial_pp}
@@ -186,15 +144,15 @@
     expected_pp: ProtectionProfile = ProtectionProfile(
         "Korean National Protection Profile for Single Sign On V1.0",
         "EAL1+",
         pp_link="http://www.commoncriteriaportal.org/files/ppfiles/KECS-PP-0822-2017%20Korean%20National%20PP%20for%20Single%20Sign%20On%20V1.0(eng).pdf",
         pp_ids=frozenset(["KECS-PP-0822-2017 SSO V1.0"]),
     )
 
-    cc_dset.process_protection_profiles(to_download=False)
+    processed_cc_dset.process_protection_profiles(to_download=False)
     assert random_certificate.protection_profiles == {expected_pp}
 
 
 def test_single_record_references_heuristics(random_certificate: CCCertificate):
     # Single record in daset is not affecting nor affected by other records
     assert not random_certificate.heuristics.report_references.directly_referenced_by
     assert not random_certificate.heuristics.report_references.indirectly_referenced_by
```

### Comparing `sec-certs-0.1.3/tests/cc/test_cc_dataset.py` & `sec-certs-0.1.4/tests/cc/test_cc_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,19 @@
 import json
 import shutil
-from datetime import date
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import pytest
 
-import tests.data.cc.dataset
 from sec_certs import constants
-from sec_certs.dataset import CCDataset
+from sec_certs.dataset.cc import CCDataset
 from sec_certs.sample.cc import CCCertificate
 
 
-@pytest.fixture(scope="module")
-def data_dir() -> Path:
-    return Path(tests.data.cc.dataset.__path__[0])
-
-
-@pytest.fixture(scope="module")
-def crt() -> CCCertificate:
-    return CCCertificate(
-        "active",
-        "Access Control Devices and Systems",
-        "NetIQ Identity Manager 4.7",
-        "NetIQ Corporation",
-        "SE",
-        {"ALC_FLR.2", "EAL3+"},
-        date(2020, 6, 15),
-        date(2025, 6, 15),
-        "https://www.commoncriteriaportal.org/files/epfiles/Certification%20Report%20-%20NetIQ®%20Identity%20Manager%204.7.pdf",
-        "https://www.commoncriteriaportal.org/files/epfiles/ST%20-%20NetIQ%20Identity%20Manager%204.7.pdf",
-        "https://www.commoncriteriaportal.org/files/epfiles/Certifikat%20CCRA%20-%20NetIQ%20Identity%20Manager%204.7_signed.pdf",
-        "https://www.netiq.com/",
-        set(),
-        set(),
-        None,
-        None,
-        None,
-    )
-
-
-@pytest.fixture
-def toy_dataset(data_dir: Path) -> CCDataset:
-    return CCDataset.from_json(data_dir / "toy_dataset.json")
-
-
 def test_download_and_convert_pdfs(toy_dataset: CCDataset, data_dir: Path):
     template_report_pdf_hashes = {
         "309ac2fd7f2dcf17": "774c41fbba980191ca40ae610b2f61484c5997417b3325b6fd68b345173bde52",
         "8cf86948f02f047d": "533a5995ef8b736cc48cfda30e8aafec77d285511471e0e5a9e8007c8750203a",
         "8a5e6bcda602920c": "e277151e4b279085cd3041ce914ffb3942b43e5ace911c557ad6b8ed764a4ece",
     }
 
@@ -109,44 +74,49 @@
         template_data = json.load(handle)
 
     del data["timestamp"]
     del template_data["timestamp"]
     assert data == template_data
 
 
-def test_dataset_from_json(toy_dataset: CCDataset, data_dir: Path):
+def test_dataset_from_json(toy_dataset: CCDataset, data_dir: Path, tmp_path):
     assert toy_dataset == CCDataset.from_json(data_dir / "toy_dataset.json")
 
+    compressed_path = tmp_path / "dset.json.gz"
+    toy_dataset.to_json(compressed_path, compress=True)
+    decompressed_dataset = CCDataset.from_json(compressed_path, is_compressed=True)
+    assert toy_dataset == decompressed_dataset
+
 
 def test_build_empty_dataset():
     with TemporaryDirectory() as tmp_dir:
         dset = CCDataset({}, Path(tmp_dir), "sample_dataset", "sample dataset description")
         dset.get_certs_from_web(to_download=False, get_archived=False, get_active=False)
     assert len(dset) == 0
     assert dset.state.meta_sources_parsed
     assert not dset.state.artifacts_downloaded
     assert not dset.state.pdfs_converted
     assert not dset.state.certs_analyzed
 
 
-def test_build_dataset(data_dir: Path, crt: CCCertificate, toy_dataset: CCDataset):
+def test_build_dataset(data_dir: Path, cert_one: CCCertificate, toy_dataset: CCDataset):
     with TemporaryDirectory() as tmp_dir:
         dataset_path = Path(tmp_dir)
         (dataset_path / "web").mkdir()
         shutil.copyfile(data_dir / "cc_products_active.csv", dataset_path / "web" / "cc_products_active.csv")
         shutil.copyfile(data_dir / "cc_products_active.html", dataset_path / "web" / "cc_products_active.html")
 
         dset = CCDataset({}, dataset_path, "sample_dataset", "sample dataset description")
         dset.get_certs_from_web(
             keep_metadata=False, to_download=False, get_archived=False, get_active=True, update_json=False
         )
 
         assert len(list(dataset_path.iterdir())) == 0
         assert len(dset) == 3
-        assert crt in dset
+        assert cert_one in dset
         assert dset == toy_dataset
 
 
 def test_process_pp_dataset(toy_dataset: CCDataset):
     with TemporaryDirectory() as tmp_dir:
         toy_dataset.copy_dataset(tmp_dir)
         toy_dataset.process_protection_profiles()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sec-certs-0.1.3/tests/cc/test_cc_maintenance_updates.py` & `sec-certs-0.1.4/tests/cc/test_cc_maintenance_updates.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import json
+from importlib import resources
 from pathlib import Path
+from typing import Generator
 
 import pytest
-
 import tests.data.cc.dataset
-from sec_certs.dataset import CCDataset, CCDatasetMaintenanceUpdates
-from sec_certs.sample.cc_maintenance_update import CCMaintenanceUpdate
-
 
-@pytest.fixture(scope="module")
-def data_dir() -> Path:
-    return Path(tests.data.cc.dataset.__path__[0])
+from sec_certs.dataset import CCDatasetMaintenanceUpdates
+from sec_certs.sample.cc_maintenance_update import CCMaintenanceUpdate
 
 
 @pytest.fixture(scope="module")
-def cc_dset(data_dir: Path) -> CCDataset:
-    return CCDataset.from_json(data_dir / "toy_dataset.json")
+def data_dir() -> Generator[Path, None, None]:
+    with resources.path(tests.data.cc.dataset, "") as path:
+        yield path
 
 
 @pytest.fixture
 def mu_dset(data_dir: Path, tmp_path_factory) -> CCDatasetMaintenanceUpdates:
     tmp_dir = tmp_path_factory.mktemp("mu_dset")
-    dset = CCDatasetMaintenanceUpdates.from_json(data_dir / "auxillary_datasets/maintenances/maintenance_updates.json")
+    dset = CCDatasetMaintenanceUpdates.from_json(data_dir / "auxiliary_datasets/maintenances/maintenance_updates.json")
     dset.copy_dataset(tmp_dir)
     return dset
 
 
 def test_methods_not_meant_to_be_implemented():
     dset = CCDatasetMaintenanceUpdates()
     with pytest.raises(NotImplementedError):
         dset.analyze_certificates()
     with pytest.raises(NotImplementedError):
         dset._compute_heuristics()
     with pytest.raises(NotImplementedError):
-        dset.process_auxillary_datasets()
+        dset.process_auxiliary_datasets()
     with pytest.raises(NotImplementedError):
         dset.compute_related_cves()
     with pytest.raises(NotImplementedError):
         dset.get_certs_from_web()
 
 
 def test_download_artifacts(mu_dset: CCDatasetMaintenanceUpdates):
@@ -54,25 +52,25 @@
 
 def test_dataset_to_json(mu_dset: CCDatasetMaintenanceUpdates, data_dir: Path, tmp_path: Path):
     mu_dset.to_json(tmp_path / "dset.json")
 
     with (tmp_path / "dset.json").open("r") as handle:
         data = json.load(handle)
 
-    with (data_dir / "auxillary_datasets/maintenances/maintenance_updates.json").open("r") as handle:
+    with (data_dir / "auxiliary_datasets/maintenances/maintenance_updates.json").open("r") as handle:
         template_data = json.load(handle)
 
     del template_data["timestamp"]
     del data["timestamp"]
     assert data == template_data
 
 
 def test_dataset_from_json(mu_dset: CCDatasetMaintenanceUpdates, data_dir: Path):
     assert mu_dset == CCDatasetMaintenanceUpdates.from_json(
-        data_dir / "auxillary_datasets/maintenances/maintenance_updates.json"
+        data_dir / "auxiliary_datasets/maintenances/maintenance_updates.json"
     )
 
 
 def test_to_pandas(mu_dset: CCDatasetMaintenanceUpdates):
     df = mu_dset.to_pandas()
     assert df.shape == (len(mu_dset), len(CCMaintenanceUpdate.pandas_columns) - 1)
     assert df.index.name == "dgst"
```

### Comparing `sec-certs-0.1.3/tests/cc/test_cc_misc.py` & `sec-certs-0.1.4/tests/cc/test_cc_misc.py`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/auxillary_datasets/cpe_dataset.json` & `sec-certs-0.1.4/tests/data/common/cpe_dataset.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.45%*

 * *Differences: {"'cpes'": "{'cpe:2.3:a:ibm:security_access_manager_for_enterprise_single_sign-on:8.2.2:*:*:*:*:*:*:*': "*

 * *           "{'cpe_id': '249582E3-A298-4A7E-8483-5164C92E4464', delete: ['start_version', "*

 * *           "'end_version']}, 'cpe:2.3:a:ibm:security_key_lifecycle_manager:2.6.0.1:*:*:*:*:*:*:*': "*

 * *           "{'cpe_id': 'AD5D2211-6F47-44E8-8FDD-625D23ED54A0', delete: ['start_version', "*

 * *           "'end_version']}, "*

 * *           "'cpe:2.3:a:semperplugins:all_in_one_seo_pack:1.3.6.4:*:*:*:*:wordpress:*:*': "*

 * *  […]*

```diff
@@ -1,34 +1,36 @@
 {
     "_type": "sec_certs.dataset.cpe.CPEDataset",
     "cpes": {
         "cpe:2.3:a:ibm:security_access_manager_for_enterprise_single_sign-on:8.2.2:*:*:*:*:*:*:*": {
             "_type": "sec_certs.sample.cpe.CPE",
-            "end_version": null,
-            "start_version": null,
+            "cpe_id": "249582E3-A298-4A7E-8483-5164C92E4464",
             "title": "IBM Security Access Manager For Enterprise Single Sign-On 8.2.2",
             "uri": "cpe:2.3:a:ibm:security_access_manager_for_enterprise_single_sign-on:8.2.2:*:*:*:*:*:*:*"
         },
         "cpe:2.3:a:ibm:security_key_lifecycle_manager:2.6.0.1:*:*:*:*:*:*:*": {
             "_type": "sec_certs.sample.cpe.CPE",
-            "end_version": null,
-            "start_version": null,
+            "cpe_id": "AD5D2211-6F47-44E8-8FDD-625D23ED54A0",
             "title": "IBM Security Key Lifecycle Manager 2.6.0.1",
             "uri": "cpe:2.3:a:ibm:security_key_lifecycle_manager:2.6.0.1:*:*:*:*:*:*:*"
         },
         "cpe:2.3:a:semperplugins:all_in_one_seo_pack:1.3.6.4:*:*:*:*:wordpress:*:*": {
             "_type": "sec_certs.sample.cpe.CPE",
-            "end_version": null,
-            "start_version": null,
+            "cpe_id": "4D35FB4F-A452-4316-9BA7-B30636CEBD9E",
             "title": "Semper Plugins All in One SEO Pack 1.3.6.4 for WordPress",
             "uri": "cpe:2.3:a:semperplugins:all_in_one_seo_pack:1.3.6.4:*:*:*:*:wordpress:*:*"
         },
         "cpe:2.3:a:tracker-software:pdf-xchange_lite_printer:6.0.320.0:*:*:*:*:*:*:*": {
             "_type": "sec_certs.sample.cpe.CPE",
-            "end_version": null,
-            "start_version": null,
+            "cpe_id": "80415FAC-AA97-46F5-AD08-4E025676B4E3",
             "title": "Tracker Software PDF-XChange Lite Printer 6.0.320.0",
             "uri": "cpe:2.3:a:tracker-software:pdf-xchange_lite_printer:6.0.320.0:*:*:*:*:*:*:*"
+        },
+        "cpe:2.3:o:redhat:enterprise_linux:7.1:*:*:*:*:*:*:*": {
+            "_type": "sec_certs.sample.cpe.CPE",
+            "cpe_id": "24F46DB3-4EF1-4669-BCA0-C3EC498D3B4A",
+            "title": "Red Hat Enterprise Linux 7.1",
+            "uri": "cpe:2.3:o:redhat:enterprise_linux:7.1:*:*:*:*:*:*:*"
         }
     },
-    "was_enhanced_with_vuln_cpes": true
+    "last_update_timestamp": "2023-04-14 13:15:45.830000"
 }
```

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/cc_full_dataset.json` & `sec-certs-0.1.4/tests/data/cc/analysis/cc_full_dataset.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428572%*

 * *Differences: {"'state'": "{'auxiliary_datasets_processed': True, delete: ['auxillary_datasets_processed']}"}*

```diff
@@ -716,14 +716,14 @@
     "description": "sample dataset description",
     "n_certs": 1,
     "name": "cc_full_dataset",
     "sha256_digest": "not implemented",
     "state": {
         "_type": "sec_certs.dataset.dataset.Dataset.DatasetInternalState",
         "artifacts_downloaded": true,
-        "auxillary_datasets_processed": true,
+        "auxiliary_datasets_processed": true,
         "certs_analyzed": false,
         "meta_sources_parsed": true,
         "pdfs_converted": true
     },
     "timestamp": "2022-11-04 16:28:04.282938"
 }
```

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf` & `sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/pdf/ebd276cca70fd723.pdf`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt` & `sec-certs-0.1.4/tests/data/cc/analysis/certs/reports/txt/ebd276cca70fd723.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf` & `sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/pdf/ebd276cca70fd723.pdf`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt` & `sec-certs-0.1.4/tests/data/cc/analysis/certs/targets/txt/ebd276cca70fd723.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/reference_dataset.json` & `sec-certs-0.1.4/tests/data/cc/analysis/reference_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/transitive_vulnerability_dataset.json` & `sec-certs-0.1.4/tests/data/cc/analysis/transitive_vulnerability_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/analysis/vulnerable_dataset.json` & `sec-certs-0.1.4/tests/data/fips/certificate/fictional_cert.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.0782967032967033%*

 * *Differences: {"'_type'": "'sec_certs.sample.fips.FIPSCertificate'",*

 * * "'cert_id'": '3518',*

 * * "'dgst'": "'184097a88a9b4ad9'",*

 * * "'heuristics'": "OrderedDict([('_type', 'sec_certs.sample.fips.FIPSCertificate.Heuristics'), "*

 * *                 "('algorithms', OrderedDict([('_type', 'Set'), ('elements', [])])), "*

 * *                 "('extracted_versions', OrderedDict([('_type', 'Set'), ('elements', [])])), "*

 * *                 "('cpe_matches', None), ('verified_cpe_matches', None), ('related_cves', None), "*

 * *                 "('polic […]*

```diff
@@ -1,73 +1,84 @@
 {
-    "_type": "sec_certs.dataset.cc.CCDataset",
-    "certs": [
-        {
-            "_type": "sec_certs.sample.cc.CCCertificate",
-            "category": "Access Control Devices and Systems",
-            "cert_link": null,
-            "dgst": "ebd276cca70fd723",
-            "heuristics": {
-                "_type": "sec_certs.sample.cc.CCCertificate.Heuristics",
-                "cert_id": null,
-                "cert_lab": null,
-                "cpe_matches": null,
-                "extracted_versions": [
-                    "8.2"
-                ],
-                "related_cves": null,
-                "verified_cpe_matches": null
-            },
-            "maintenance_updates": [],
-            "manufacturer": "IBM Corporation",
-            "manufacturer_web": "http://www.ibm.com",
-            "name": "IBM Security Access Manager for Enterprise Single Sign-On Version 8.2",
-            "not_valid_after": null,
-            "not_valid_before": "2014-12-05",
-            "pdf_data": {
-                "_type": "sec_certs.sample.cc.CCCertificate.PdfData",
-                "report_filename": null,
-                "report_frontpage": null,
-                "report_keywords": null,
-                "report_metadata": null,
-                "st_filename": null,
-                "st_frontpage": null,
-                "st_keywords": null,
-                "st_metadata": null
-            },
-            "protection_profiles": [],
-            "report_link": "http://www.commoncriteriaportal.org/files/epfiles/0683a_pdf.pdf",
-            "scheme": "DE",
-            "security_level": {
-                "_type": "Set",
-                "elements": [
-                    "ALC_FLR.1",
-                    "EAL3+"
-                ]
-            },
-            "st_link": "http://www.commoncriteriaportal.org/files/epfiles/0683b_pdf.pdf",
-            "state": {
-                "_type": "sec_certs.sample.cc.CCCertificate.InternalState",
-                "report_convert_ok": true,
-                "report_download_ok": true,
-                "report_extract_ok": true,
-                "st_convert_ok": true,
-                "st_download_ok": true,
-                "st_extract_ok": true
-            },
-            "status": "active"
-        }
-    ],
-    "description": "sample dataset description",
-    "n_certs": 1,
-    "name": "cc_full_dataset",
-    "sha256_digest": "not implemented",
+    "_type": "sec_certs.sample.fips.FIPSCertificate",
+    "cert_id": 3518,
+    "dgst": "184097a88a9b4ad9",
+    "heuristics": {
+        "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
+        "algorithms": {
+            "_type": "Set",
+            "elements": []
+        },
+        "cpe_matches": null,
+        "direct_transitive_cves": null,
+        "extracted_versions": {
+            "_type": "Set",
+            "elements": []
+        },
+        "indirect_transitive_cves": null,
+        "module_processed_references": {
+            "_type": "sec_certs.sample.certificate.References",
+            "directly_referenced_by": null,
+            "directly_referencing": null,
+            "indirectly_referenced_by": null,
+            "indirectly_referencing": null
+        },
+        "module_prunned_references": {
+            "_type": "Set",
+            "elements": []
+        },
+        "policy_processed_references": {
+            "_type": "sec_certs.sample.certificate.References",
+            "directly_referenced_by": null,
+            "directly_referencing": null,
+            "indirectly_referenced_by": null,
+            "indirectly_referencing": null
+        },
+        "policy_prunned_references": {
+            "_type": "Set",
+            "elements": []
+        },
+        "related_cves": null,
+        "verified_cpe_matches": null
+    },
+    "pdf_data": {
+        "_type": "sec_certs.sample.fips.FIPSCertificate.PdfData",
+        "keywords": {},
+        "policy_metadata": {}
+    },
     "state": {
-        "_type": "sec_certs.dataset.dataset.Dataset.DatasetInternalState",
-        "artifacts_downloaded": false,
-        "auxillary_datasets_processed": true,
-        "certs_analyzed": false,
-        "meta_sources_parsed": true,
-        "pdfs_converted": false
+        "_type": "sec_certs.sample.fips.FIPSCertificate.InternalState",
+        "module_download_ok": true,
+        "module_extract_ok": false,
+        "policy_convert_garbage": false,
+        "policy_convert_ok": true,
+        "policy_download_ok": true,
+        "policy_extract_ok": false,
+        "policy_pdf_hash": "36b63890182f0aed29b305a0b4acc0d70b657262516f4be69138c70c2abdb1f1",
+        "policy_txt_hash": "cc1f8d0f7bb759894e81cbbfd1cfe02cdc443879fd47d3306f2a1b419fbf2872"
     },
-    "timestamp": "2021-04-16 15:05:18.386794"
+    "web_data": {
+        "_type": "sec_certs.sample.fips.FIPSCertificate.WebData",
+        "caveat": null,
+        "certificate_pdf_url": null,
+        "date_sunset": null,
+        "description": null,
+        "embodiment": null,
+        "exceptions": null,
+        "fw_versions": null,
+        "historical_reason": null,
+        "hw_versions": null,
+        "level": null,
+        "mentioned_certs": null,
+        "module_name": null,
+        "module_type": null,
+        "revoked_link": null,
+        "revoked_reason": null,
+        "standard": null,
+        "status": null,
+        "sw_versions": null,
+        "tested_conf": null,
+        "validation_history": null,
+        "vendor": null,
+        "vendor_url": null
+    }
 }
```

### Comparing `sec-certs-0.1.3/tests/data/cc/certificate/fictional_cert.json` & `sec-certs-0.1.4/tests/data/cc/certificate/fictional_cert.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979757085020242%*

 * *Differences: {"'heuristics'": "{'scheme_data': None}"}*

```diff
@@ -16,14 +16,15 @@
         "report_references": {
             "_type": "sec_certs.sample.certificate.References",
             "directly_referenced_by": null,
             "directly_referencing": null,
             "indirectly_referenced_by": null,
             "indirectly_referencing": null
         },
+        "scheme_data": null,
         "st_references": {
             "_type": "sec_certs.sample.certificate.References",
             "directly_referenced_by": null,
             "directly_referencing": null,
             "indirectly_referenced_by": null,
             "indirectly_referencing": null
         },
```

### Comparing `sec-certs-0.1.3/tests/data/cc/dataset/auxillary_datasets/maintenances/maintenance_updates.json` & `sec-certs-0.1.4/tests/data/cc/dataset/auxiliary_datasets/maintenances/maintenance_updates.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9819024725274725%*

 * *Differences: {"'certs'": "{0: {'heuristics': {'scheme_data': None}}}",*

 * * "'state'": "{'auxiliary_datasets_processed': False, delete: ['auxillary_datasets_processed']}"}*

```diff
@@ -17,14 +17,15 @@
                 "report_references": {
                     "_type": "sec_certs.sample.certificate.References",
                     "directly_referenced_by": null,
                     "directly_referencing": null,
                     "indirectly_referenced_by": null,
                     "indirectly_referencing": null
                 },
+                "scheme_data": null,
                 "st_references": {
                     "_type": "sec_certs.sample.certificate.References",
                     "directly_referenced_by": null,
                     "directly_referencing": null,
                     "indirectly_referenced_by": null,
                     "indirectly_referencing": null
                 },
@@ -66,14 +67,14 @@
     "description": "dataset_description",
     "n_certs": 1,
     "name": "maintenance_updates",
     "sha256_digest": "not implemented",
     "state": {
         "_type": "sec_certs.dataset.dataset.Dataset.DatasetInternalState",
         "artifacts_downloaded": true,
-        "auxillary_datasets_processed": false,
+        "auxiliary_datasets_processed": false,
         "certs_analyzed": false,
         "meta_sources_parsed": true,
         "pdfs_converted": false
     },
     "timestamp": "2022-11-10 13:44:35.171285"
 }
```

### Comparing `sec-certs-0.1.3/tests/data/cc/dataset/cc_products_active.csv` & `sec-certs-0.1.4/tests/data/cc/dataset/cc_products_active.csv`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/dataset/cc_products_active.html` & `sec-certs-0.1.4/tests/data/cc/dataset/cc_products_active.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt` & `sec-certs-0.1.4/tests/data/cc/dataset/report_309ac2fd7f2dcf17.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt` & `sec-certs-0.1.4/tests/data/cc/dataset/target_309ac2fd7f2dcf17.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/cc/dataset/toy_dataset.json` & `sec-certs-0.1.4/tests/data/cc/dataset/toy_dataset.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9820163389242337%*

 * *Differences: {"'certs'": "{0: {'heuristics': {'scheme_data': None}}, 1: {'heuristics': {'scheme_data': None}}, "*

 * *            "2: {'heuristics': {'scheme_data': None}}}",*

 * * "'state'": "{'auxiliary_datasets_processed': False, delete: ['auxillary_datasets_processed']}"}*

```diff
@@ -19,14 +19,15 @@
                 "report_references": {
                     "_type": "sec_certs.sample.certificate.References",
                     "directly_referenced_by": null,
                     "directly_referencing": null,
                     "indirectly_referenced_by": null,
                     "indirectly_referencing": null
                 },
+                "scheme_data": null,
                 "st_references": {
                     "_type": "sec_certs.sample.certificate.References",
                     "directly_referenced_by": null,
                     "directly_referencing": null,
                     "indirectly_referenced_by": null,
                     "indirectly_referencing": null
                 },
@@ -101,14 +102,15 @@
                 "report_references": {
                     "_type": "sec_certs.sample.certificate.References",
                     "directly_referenced_by": null,
                     "directly_referencing": null,
                     "indirectly_referenced_by": null,
                     "indirectly_referencing": null
                 },
+                "scheme_data": null,
                 "st_references": {
                     "_type": "sec_certs.sample.certificate.References",
                     "directly_referenced_by": null,
                     "directly_referencing": null,
                     "indirectly_referenced_by": null,
                     "indirectly_referencing": null
                 },
@@ -188,14 +190,15 @@
                 "report_references": {
                     "_type": "sec_certs.sample.certificate.References",
                     "directly_referenced_by": null,
                     "directly_referencing": null,
                     "indirectly_referenced_by": null,
                     "indirectly_referencing": null
                 },
+                "scheme_data": null,
                 "st_references": {
                     "_type": "sec_certs.sample.certificate.References",
                     "directly_referenced_by": null,
                     "directly_referencing": null,
                     "indirectly_referenced_by": null,
                     "indirectly_referencing": null
                 },
@@ -269,14 +272,14 @@
     "description": "toy dataset description",
     "n_certs": 3,
     "name": "toy dataset",
     "sha256_digest": "not implemented",
     "state": {
         "_type": "sec_certs.dataset.dataset.Dataset.DatasetInternalState",
         "artifacts_downloaded": false,
-        "auxillary_datasets_processed": false,
+        "auxiliary_datasets_processed": false,
         "certs_analyzed": false,
         "meta_sources_parsed": true,
         "pdfs_converted": false
     },
     "timestamp": "2020-11-16 17:04:14.770153"
 }
```

### Comparing `sec-certs-0.1.3/tests/data/fips/dataset/alg_dataset.json` & `sec-certs-0.1.4/tests/data/fips/dataset/alg_dataset.json`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/dataset/fips_modules_active.html` & `sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_active.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/dataset/fips_modules_historical.html` & `sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_historical.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/dataset/fips_modules_revoked.html` & `sec-certs-0.1.4/tests/data/fips/dataset/fips_modules_revoked.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt` & `sec-certs-0.1.4/tests/data/fips/dataset/template_policy_184097a88a9b4ad9.txt`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/dataset/toy_dataset.json` & `sec-certs-0.1.4/tests/data/fips/dataset/toy_dataset.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9776785714285715%*

 * *Differences: {"'certs'": "{0: {'cert_id': 2590}, 1: {'cert_id': 2997}, 2: {'cert_id': 3495}, 3: {'cert_id': "*

 * *            "2721}, 4: {'cert_id': 3090}, 5: {'cert_id': 2860}, 6: {'cert_id': 3176}, 7: "*

 * *            "{'cert_id': 3850}, 8: {'cert_id': 2665}, 9: {'cert_id': 3093}, 10: {'cert_id': 3711}, "*

 * *            "11: {'cert_id': 3493}, 12: {'cert_id': 3141}, 13: {'cert_id': 2630}, 14: {'cert_id': "*

 * *            "3095}, 15: {'cert_id': 3197}, 16: {'cert_id': 3651}, 17: {'cert_id': 2711}, 18: "*

 * *            "{'cert_id': 351 […]*

```diff
@@ -1,13 +1,13 @@
 {
     "_type": "sec_certs.dataset.fips.FIPSDataset",
     "certs": [
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2590",
+            "cert_id": 2590,
             "dgst": "69d9200c309f5f97",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -83,15 +83,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2997",
+            "cert_id": 2997,
             "dgst": "3b05cf67849835e3",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -167,15 +167,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3495",
+            "cert_id": 3495,
             "dgst": "618102f275d5649a",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -251,15 +251,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2721",
+            "cert_id": 2721,
             "dgst": "5b00a7bb92c1cb19",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -335,15 +335,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3090",
+            "cert_id": 3090,
             "dgst": "e1ff7d9997726782",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -419,15 +419,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2860",
+            "cert_id": 2860,
             "dgst": "ed16d272044ed81f",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -503,15 +503,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3176",
+            "cert_id": 3176,
             "dgst": "73e7f3f802b0e919",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -587,15 +587,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3850",
+            "cert_id": 3850,
             "dgst": "756a6524cdb2d4ea",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -671,15 +671,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2665",
+            "cert_id": 2665,
             "dgst": "0e8b7a7f79b3098b",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -755,15 +755,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3093",
+            "cert_id": 3093,
             "dgst": "f7df34ce0a0ad316",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -839,15 +839,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3711",
+            "cert_id": 3711,
             "dgst": "0df59fd6c41cadd2",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -923,15 +923,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3493",
+            "cert_id": 3493,
             "dgst": "24a05f4d1305d667",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1007,15 +1007,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3141",
+            "cert_id": 3141,
             "dgst": "51c94a510b50e68f",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1091,15 +1091,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2630",
+            "cert_id": 2630,
             "dgst": "75ca28395bfc9ad1",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1175,15 +1175,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3095",
+            "cert_id": 3095,
             "dgst": "cd0666cdd7ce0244",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1259,15 +1259,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3197",
+            "cert_id": 3197,
             "dgst": "ceab64951a30f684",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1343,15 +1343,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3651",
+            "cert_id": 3651,
             "dgst": "0ab77c56eece2d24",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1427,15 +1427,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2711",
+            "cert_id": 2711,
             "dgst": "9ca7b8be590113b8",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1511,15 +1511,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3518",
+            "cert_id": 3518,
             "dgst": "184097a88a9b4ad9",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1595,15 +1595,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2779",
+            "cert_id": 2779,
             "dgst": "c333a75353784177",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1679,15 +1679,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "2441",
+            "cert_id": 2441,
             "dgst": "ad1e075215267a28",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1763,15 +1763,15 @@
                 "validation_history": null,
                 "vendor": null,
                 "vendor_url": null
             }
         },
         {
             "_type": "sec_certs.sample.fips.FIPSCertificate",
-            "cert_id": "3488",
+            "cert_id": 3488,
             "dgst": "2aec3694418f35d8",
             "heuristics": {
                 "_type": "sec_certs.sample.fips.FIPSCertificate.Heuristics",
                 "algorithms": {
                     "_type": "Set",
                     "elements": []
                 },
@@ -1853,14 +1853,14 @@
     "description": "30/11/2022 16:38:51",
     "n_certs": 22,
     "name": "FIPSDataset dataset",
     "sha256_digest": "not implemented",
     "state": {
         "_type": "sec_certs.dataset.dataset.Dataset.DatasetInternalState",
         "artifacts_downloaded": true,
-        "auxillary_datasets_processed": false,
+        "auxiliary_datasets_processed": false,
         "certs_analyzed": false,
         "meta_sources_parsed": true,
         "pdfs_converted": true
     },
     "timestamp": "2022-11-30 16:38:51.953055"
 }
```

### Comparing `sec-certs-0.1.3/tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html` & `sec-certs-0.1.4/tests/data/fips/iut/fips_iut_2020-10-25T06+01:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html` & `sec-certs-0.1.4/tests/data/fips/iut/fips_iut_2021-12-10T06+01:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html` & `sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2020-10-24T06+02:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html` & `sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2021-02-19T06+01:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html` & `sec-certs-0.1.4/tests/data/fips/mip/fips_mip_2021-12-19T06+01:00.html`

 * *Files identical despite different names*

### Comparing `sec-certs-0.1.3/tests/fips/test_fips_algorithm_dataset.py` & `sec-certs-0.1.4/tests/fips/test_fips_algorithm_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-from pathlib import Path
+from importlib import resources
 from typing import Any
 
 import pytest
-
 import tests.data.fips.dataset
+
 from sec_certs.dataset.fips_algorithm import FIPSAlgorithmDataset
 from sec_certs.sample.fips_algorithm import FIPSAlgorithm
 from sec_certs.serialization.json import SerializationError
 
 
 @pytest.mark.xfail(reason="May fail due to errors with NIST server.")
 @pytest.mark.slow
@@ -19,21 +19,17 @@
     assert "TDES2840" in dset
     assert "SHS1619" in dset
     assert "RNG447" in dset
     assert len(dset) > 30000
 
 
 @pytest.fixture(scope="module")
-def alg_dset_path() -> Path:
-    return Path(tests.data.fips.dataset.__path__[0]) / "alg_dataset.json"
-
-
-@pytest.fixture(scope="module")
-def alg_dset(alg_dset_path: Path) -> FIPSAlgorithmDataset:
-    return FIPSAlgorithmDataset.from_json(alg_dset_path)
+def alg_dset() -> FIPSAlgorithmDataset:
+    with resources.path(tests.data.fips.dataset, "alg_dataset.json") as alg_dset_path:
+        return FIPSAlgorithmDataset.from_json(alg_dset_path)
 
 
 @pytest.fixture(scope="module")
 def alg_dict() -> dict[str, Any]:
     return {
         "alg_number": "2902",
         "algorithm_type": "AES",
```

### Comparing `sec-certs-0.1.3/tests/fips/test_fips_certificate.py` & `sec-certs-0.1.4/tests/fips/test_fips_certificate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+from __future__ import annotations
+
 import json
 import shutil
+from importlib import resources
 from pathlib import Path
+from typing import Generator
 
 import pytest
-
 import tests.data.fips.certificate
 import tests.data.fips.dataset
+
 from sec_certs.dataset.fips import FIPSDataset
 from sec_certs.sample.fips import FIPSCertificate
 
 
 @pytest.fixture(scope="module")
-def data_dir() -> Path:
-    return Path(tests.data.fips.certificate.__path__[0])
+def data_dir() -> Generator[Path, None, None]:
+    with resources.path(tests.data.fips.certificate, "") as path:
+        yield path
 
 
 @pytest.fixture
 def certificate(tmp_path_factory) -> FIPSCertificate:
     tmp_dir = tmp_path_factory.mktemp("dset")
-    dset_json_path = Path(tests.data.fips.dataset.__path__[0]) / "toy_dataset.json"
-    data_dir_path = dset_json_path.parent
-    shutil.copytree(data_dir_path, tmp_dir, dirs_exist_ok=True)
+
+    with resources.path(tests.data.fips.dataset, "") as dataset_path:
+        shutil.copytree(dataset_path, tmp_dir, dirs_exist_ok=True)
+
     fips_dset = FIPSDataset.from_json(tmp_dir / "toy_dataset.json")
 
     crt = fips_dset["184097a88a9b4ad9"]
     fips_dset.certs = {crt.dgst: crt}
     fips_dset.download_all_artifacts()
     fips_dset.convert_all_pdfs()
```

### Comparing `sec-certs-0.1.3/tests/fips/test_fips_dataset.py` & `sec-certs-0.1.4/tests/fips/test_fips_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+from __future__ import annotations
+
 import json
 import shutil
+from importlib import resources
 from pathlib import Path
 from tempfile import TemporaryDirectory
+from typing import Generator
 
 import pytest
-
-import sec_certs.constants as constants
 import tests.data.fips.dataset
+
+from sec_certs import constants
 from sec_certs.dataset.fips import FIPSDataset
 from sec_certs.sample.fips import FIPSCertificate
 
 
 @pytest.fixture(scope="module")
-def data_dir() -> Path:
-    return Path(tests.data.fips.dataset.__path__[0])
-
-
-@pytest.fixture
-def toy_dataset(data_dir: Path) -> FIPSDataset:
-    return FIPSDataset.from_json(data_dir / "toy_dataset.json")
+def data_dir() -> Generator[Path, None, None]:
+    with resources.path(tests.data.fips.dataset, "") as path:
+        yield path
 
 
 def test_dataset_to_json(toy_dataset: FIPSDataset, data_dir: Path, tmp_path: Path):
     toy_dataset.to_json(tmp_path / "dset.json")
 
     with (tmp_path / "dset.json").open("r") as handle:
         data = json.load(handle)
@@ -31,17 +31,22 @@
         template_data = json.load(handle)
 
     del data["timestamp"]
     del template_data["timestamp"]
     assert data == template_data
 
 
-def test_dataset_from_json(toy_dataset: FIPSDataset, data_dir: Path):
+def test_dataset_from_json(toy_dataset: FIPSDataset, data_dir: Path, tmp_path: Path):
     assert toy_dataset == FIPSDataset.from_json(data_dir / "toy_dataset.json")
 
+    compressed_path = tmp_path / "dset.json.gz"
+    toy_dataset.to_json(compressed_path, compress=True)
+    decompressed_dataset = FIPSDataset.from_json(compressed_path, is_compressed=True)
+    assert toy_dataset == decompressed_dataset
+
 
 def test_build_empty_dataset():
     with TemporaryDirectory() as tmp_dir:
         dset = FIPSDataset(root_dir=tmp_dir)
     assert len(dset) == 0
     assert not dset.state.meta_sources_parsed
     assert not dset.state.artifacts_downloaded
@@ -66,14 +71,15 @@
         assert set(dset.certs.keys()) == set(toy_dataset.certs.keys())
 
 
 @pytest.mark.xfail(reason="May fail due to error on FIPS server.")
 def test_download_meta_html_files():
     with TemporaryDirectory() as tmp_dir:
         dset = FIPSDataset(root_dir=Path(tmp_dir))
+        dset.web_dir.mkdir()
         dset._download_html_resources()
 
         assert (dset.web_dir / "fips_modules_active.html").exists()
         assert (dset.web_dir / "fips_modules_active.html").stat().st_size > constants.MIN_FIPS_HTML_SIZE
         assert (dset.web_dir / "fips_modules_historical.html").exists()
         assert (dset.web_dir / "fips_modules_historical.html").stat().st_size > constants.MIN_FIPS_HTML_SIZE
         assert (dset.web_dir / "fips_modules_revoked.html").exists()
```

