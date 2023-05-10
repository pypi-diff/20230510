# Comparing `tmp/primap2-0.9.6.tar.gz` & `tmp/primap2-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primap2-0.9.6.tar", last modified: Fri Apr 28 09:39:42 2023, max compression
+gzip compressed data, was "primap2-0.9.7.tar", last modified: Wed May 10 09:55:47 2023, max compression
```

## Comparing `primap2-0.9.6.tar` & `primap2-0.9.7.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.022160 primap2-0.9.6/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/.github/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-03-31 17:51:36.000000 primap2-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-03-31 17:51:36.000000 primap2-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      364 2023-03-31 17:51:36.000000 primap2-0.9.6/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/.github/workflows/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      955 2023-04-24 13:56:22.000000 primap2-0.9.6/.github/workflows/ci.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1340 2023-04-28 09:36:40.000000 primap2-0.9.6/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1197 2023-04-28 09:36:40.000000 primap2-0.9.6/.pre-commit-config.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      406 2023-04-28 09:36:40.000000 primap2-0.9.6/.readthedocs.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      173 2023-04-28 09:36:40.000000 primap2-0.9.6/AUTHORS.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5612 2023-04-28 09:37:40.000000 primap2-0.9.6/CHANGELOG.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1608 2023-03-31 17:51:36.000000 primap2-0.9.6/CONTRIBUTING.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11357 2023-03-31 17:51:36.000000 primap2-0.9.6/LICENSE
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2860 2023-03-31 17:51:36.000000 primap2-0.9.6/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8851 2023-04-28 09:39:42.022160 primap2-0.9.6/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2284 2023-04-28 09:39:18.000000 primap2-0.9.6/README.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      167 2023-03-31 17:51:36.000000 primap2-0.9.6/TODO.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-03-31 17:51:36.000000 primap2-0.9.6/codecov.yml
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/docs/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      620 2023-04-04 07:09:04.000000 primap2-0.9.6/docs/Makefile
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/docs/_static/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       28 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/_static/custom.css
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1796 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/api.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/changelog.rst
--rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5210 2023-04-24 13:56:22.000000 primap2-0.9.6/docs/conf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      356 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/credits.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8297 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_format_details.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14060 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_format_examples.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3891 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading.rst
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/docs/data_reading_writing_examples/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      105 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    33106 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/FAOstat.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    44497 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/PRIMAP-hist.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_long.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_sec_cat.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1201 2023-04-28 07:59:57.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      332 2023-04-28 07:59:57.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5669 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_data_long.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5774 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/data_reading_writing_examples/test_data_wide.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1538 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/datalad.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    19051 2023-04-28 09:36:09.000000 primap2-0.9.6/docs/development.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      436 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/index.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1106 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/installation.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4579 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/interchange_format_details.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11376 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/interchange_format_examples.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/make.bat
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    15032 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/minimal_ds.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   543680 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/opulent_ds.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      292 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/pm2io.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-03-31 17:51:36.000000 primap2-0.9.6/docs/readme.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      111 2023-04-04 07:21:47.000000 primap2-0.9.6/docs/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    28635 2023-04-04 07:21:47.000000 primap2-0.9.6/docs/usage.ipynb
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/licenses/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.6/licenses/pint_xarray_license
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.6/licenses/xarray_license
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       64 2023-03-31 17:51:36.000000 primap2-0.9.6/mypy.ini
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2261 2023-04-04 07:21:47.000000 primap2-0.9.6/primap-stubs.patch
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/primap2/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-28 09:37:24.000000 primap2-0.9.6/primap2/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      327 2023-04-25 14:13:52.000000 primap2-0.9.6/primap2/_accessor_base.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21858 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_aggregate.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9076 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_alias_selection.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18227 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_data_format.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    12288 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_downscale.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9246 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_merge.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2720 2023-04-25 13:24:13.000000 primap2-0.9.6/primap2/_metadata.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5656 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_overview.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23888 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_setters.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      423 2023-04-25 13:05:58.000000 primap2-0.9.6/primap2/_types.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11482 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/_units.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1508 2023-04-25 13:14:07.000000 primap2-0.9.6/primap2/accessors.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/primap2/pm2io/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6332 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/pm2io/_GHG_inventory_reading.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      728 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/pm2io/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13487 2023-04-25 15:48:53.000000 primap2-0.9.6/primap2/pm2io/_conversion.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    61245 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/pm2io/_data_reading.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13953 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/pm2io/_interchange_format.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.022160 primap2-0.9.6/primap2/tests/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       79 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1640 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/conftest.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.022160 primap2-0.9.6/primap2/tests/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2999 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21056 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      701 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/long.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       84 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/long_no_time.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       87 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      113 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_category_name.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      109 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_category_name_fill_cat_code.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      231 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_category_name_long.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_sec_cat.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      434 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_csv_data_sec_cat_strings.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14880 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_from_interchange_format_output.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      198 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_no_sec_cats.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      224 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_no_sec_cats_cat_name.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      446 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_output.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      492 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_output_entity_def.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_read_wide_csv_file_output_unit_def.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    90672 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6126 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/examples.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11711 2023-04-04 07:21:47.000000 primap2-0.9.6/primap2/tests/test_aggregate.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2988 2023-04-28 08:57:53.000000 primap2-0.9.6/primap2/tests/test_alias_selection.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5501 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_conversion.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11752 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_data_format.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    37510 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/tests/test_data_reading.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6827 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_downscale.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1737 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_interchange_format.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3597 2023-04-04 07:21:47.000000 primap2-0.9.6/primap2/tests/test_merge.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1384 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_metadata.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6107 2023-04-28 08:58:51.000000 primap2-0.9.6/primap2/tests/test_overview.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17597 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/tests/test_setters.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2621 2023-03-31 17:51:36.000000 primap2-0.9.6/primap2/tests/test_units.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1911 2023-04-28 09:36:40.000000 primap2-0.9.6/primap2/tests/utils.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.018160 primap2-0.9.6/primap2.egg-info/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8851 2023-04-28 09:39:41.000000 primap2-0.9.6/primap2.egg-info/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3607 2023-04-28 09:39:42.000000 primap2-0.9.6/primap2.egg-info/SOURCES.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-04-28 09:39:41.000000 primap2-0.9.6/primap2.egg-info/dependency_links.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      415 2023-04-28 09:39:41.000000 primap2-0.9.6/primap2.egg-info/requires.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        8 2023-04-28 09:39:41.000000 primap2-0.9.6/primap2.egg-info/top_level.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      322 2023-04-28 09:36:40.000000 primap2-0.9.6/pyproject.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-03-31 17:51:36.000000 primap2-0.9.6/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-03-31 17:51:36.000000 primap2-0.9.6/requirements_dev.txt
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-28 09:39:42.022160 primap2-0.9.6/rosetta/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4711 2023-03-31 17:51:36.000000 primap2-0.9.6/rosetta/combine_rows-set.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1695 2023-04-28 09:39:42.022160 primap2-0.9.6/setup.cfg
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-03-31 17:51:36.000000 primap2-0.9.6/setup.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1315 2023-04-28 09:37:24.000000 primap2-0.9.6/tbump.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-24 13:56:22.000000 primap2-0.9.6/tox.ini
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      706 2023-03-31 17:51:36.000000 primap2-0.9.6/update_changelog.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1147 2023-03-31 17:51:36.000000 primap2-0.9.6/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/.github/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-03-31 17:51:36.000000 primap2-0.9.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-03-31 17:51:36.000000 primap2-0.9.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      364 2023-03-31 17:51:36.000000 primap2-0.9.7/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      955 2023-04-24 13:56:22.000000 primap2-0.9.7/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1340 2023-04-28 09:36:40.000000 primap2-0.9.7/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1197 2023-05-10 09:45:31.000000 primap2-0.9.7/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      406 2023-04-28 09:36:40.000000 primap2-0.9.7/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      173 2023-04-28 09:36:40.000000 primap2-0.9.7/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5678 2023-05-10 09:46:07.000000 primap2-0.9.7/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1608 2023-03-31 17:51:36.000000 primap2-0.9.7/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11357 2023-03-31 17:51:36.000000 primap2-0.9.7/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2880 2023-05-10 09:55:38.000000 primap2-0.9.7/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8917 2023-05-10 09:55:47.829400 primap2-0.9.7/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2284 2023-05-10 09:49:45.000000 primap2-0.9.7/README.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      167 2023-03-31 17:51:36.000000 primap2-0.9.7/TODO.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-03-31 17:51:36.000000 primap2-0.9.7/codecov.yml
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      620 2023-04-04 07:09:04.000000 primap2-0.9.7/docs/Makefile
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.825400 primap2-0.9.7/docs/_static/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       28 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/_static/custom.css
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1796 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5210 2023-04-24 13:56:22.000000 primap2-0.9.7/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      356 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8297 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_format_details.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14060 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_format_examples.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3891 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/docs/data_reading_writing_examples/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      105 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    33106 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/FAOstat.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    44497 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/PRIMAP-hist.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_sec_cat.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1201 2023-04-28 07:59:57.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      332 2023-04-28 07:59:57.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5669 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_data_long.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5774 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/data_reading_writing_examples/test_data_wide.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1538 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/datalad.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    19051 2023-04-28 09:36:09.000000 primap2-0.9.7/docs/development.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      436 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1106 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4579 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/interchange_format_details.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11376 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/interchange_format_examples.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    15032 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/minimal_ds.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   543680 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/opulent_ds.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      292 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/pm2io.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-03-31 17:51:36.000000 primap2-0.9.7/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      111 2023-04-04 07:21:47.000000 primap2-0.9.7/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    28635 2023-04-04 07:21:47.000000 primap2-0.9.7/docs/usage.ipynb
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/licenses/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.7/licenses/pint_xarray_license
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      565 2023-03-31 17:51:36.000000 primap2-0.9.7/licenses/xarray_license
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       64 2023-03-31 17:51:36.000000 primap2-0.9.7/mypy.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2261 2023-04-04 07:21:47.000000 primap2-0.9.7/primap-stubs.patch
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-05-10 09:45:47.000000 primap2-0.9.7/primap2/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      327 2023-04-25 14:13:52.000000 primap2-0.9.7/primap2/_accessor_base.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21858 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_aggregate.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9076 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_alias_selection.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18227 2023-05-10 09:15:27.000000 primap2-0.9.7/primap2/_data_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    12288 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_downscale.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9246 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_merge.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2720 2023-04-25 13:24:13.000000 primap2-0.9.7/primap2/_metadata.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5656 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_overview.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23888 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_setters.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      423 2023-04-25 13:05:58.000000 primap2-0.9.7/primap2/_types.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11482 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/_units.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1508 2023-04-25 13:14:07.000000 primap2-0.9.7/primap2/accessors.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2/pm2io/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6332 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/pm2io/_GHG_inventory_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      728 2023-05-10 09:15:27.000000 primap2-0.9.7/primap2/pm2io/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13487 2023-04-25 15:48:53.000000 primap2-0.9.7/primap2/pm2io/_conversion.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    61245 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/pm2io/_data_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    13953 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/pm2io/_interchange_format.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       79 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1640 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/conftest.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2/tests/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2999 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21056 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      701 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      199 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       84 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/long_no_time.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       87 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      113 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_category_name.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      109 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_category_name_fill_cat_code.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      231 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_category_name_long.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      432 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_sec_cat.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      434 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_csv_data_sec_cat_strings.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14880 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_from_interchange_format_output.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      198 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_no_sec_cats.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      224 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_no_sec_cats_cat_name.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      446 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_output.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      492 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_output_entity_def.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_read_wide_csv_file_output_unit_def.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    90672 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6126 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/examples.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11731 2023-05-10 09:45:31.000000 primap2-0.9.7/primap2/tests/test_aggregate.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2988 2023-04-28 08:57:53.000000 primap2-0.9.7/primap2/tests/test_alias_selection.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5501 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_conversion.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11752 2023-05-10 09:15:27.000000 primap2-0.9.7/primap2/tests/test_data_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    37510 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/tests/test_data_reading.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6827 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_downscale.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1737 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_interchange_format.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3597 2023-04-04 07:21:47.000000 primap2-0.9.7/primap2/tests/test_merge.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1384 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_metadata.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     6107 2023-04-28 08:58:51.000000 primap2-0.9.7/primap2/tests/test_overview.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17597 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/tests/test_setters.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2621 2023-03-31 17:51:36.000000 primap2-0.9.7/primap2/tests/test_units.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1911 2023-04-28 09:36:40.000000 primap2-0.9.7/primap2/tests/utils.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/primap2.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8917 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3607 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      415 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        8 2023-05-10 09:55:47.000000 primap2-0.9.7/primap2.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      322 2023-04-28 09:36:40.000000 primap2-0.9.7/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-03-31 17:51:36.000000 primap2-0.9.7/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-03-31 17:51:36.000000 primap2-0.9.7/requirements_dev.txt
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-10 09:55:47.829400 primap2-0.9.7/rosetta/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4711 2023-03-31 17:51:36.000000 primap2-0.9.7/rosetta/combine_rows-set.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1696 2023-05-10 09:55:47.829400 primap2-0.9.7/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-03-31 17:51:36.000000 primap2-0.9.7/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1315 2023-05-10 09:45:47.000000 primap2-0.9.7/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-24 13:56:22.000000 primap2-0.9.7/tox.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      706 2023-03-31 17:51:36.000000 primap2-0.9.7/update_changelog.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1147 2023-03-31 17:51:36.000000 primap2-0.9.7/update_citation_info.py
```

### Comparing `primap2-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md` & `primap2-0.9.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md` & `primap2-0.9.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/.github/workflows/ci.yml` & `primap2-0.9.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/.gitignore` & `primap2-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/.pre-commit-config.yaml` & `primap2-0.9.7/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - id: check-ast
       - id: fix-byte-order-marker
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: detect-private-key
       - id: mixed-line-ending
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 'v0.0.263'
+    rev: 'v0.0.265'
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
```

### Comparing `primap2-0.9.6/CHANGELOG.rst` & `primap2-0.9.7/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =========
 Changelog
 =========
 
+0.9.7
+-----
+* Fix the test suite to work with Pint release 0.21.
+
 0.9.6
 -----
 * Add dependency on openscm_units > 0.5.1 for compatibility with latest pandas.
 * stop building pdf output documentation, it doesn't support SVG and isn't used much.
 * Drop support for Python version 3.8 to prepare for it being dropped
   in Numpy on April 14.
```

### Comparing `primap2-0.9.6/CONTRIBUTING.rst` & `primap2-0.9.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/LICENSE` & `primap2-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/Makefile` & `primap2-0.9.7/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
 
 servedocs: docs ## compile the docs watching for changes
 	watchmedo shell-command -p '*.rst' -c '$(MAKE) -C docs html' -R -D .
 
 release: venv dist ## package and upload a release
-	venv/bin/twine upload dist/*
+	venv/bin/twine upload --repository primap dist/*
 
 dist: clean venv ## builds source and wheel package
 	venv/bin/python -m build
 	ls -l dist
 
 install: clean ## install the package to the active Python's site-packages
 	python setup.py install
```

### Comparing `primap2-0.9.6/PKG-INFO` & `primap2-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primap2
-Version: 0.9.6
+Version: 0.9.7
 Summary: The next generation of the PRIMAP climate policy analysis suite.
 Home-page: https://github.com/pik-primap/primap2
 Author: Mika Pflüger
 Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://primap2.readthedocs.io/
 Classifier: Development Status :: 3 - Alpha
@@ -79,22 +79,26 @@
 Apache License, Version 2.0 as well. The full text of the xarray copyright statement is
 included in the licenses directory.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger and Johannes Gütschow. (2023-04-28).
-pik-primap/primap2: PRIMAP2 Version 0.9.6.
-Zenodo. https://doi.org/10.5281/zenodo.7875234
+Mika Pflüger and Johannes Gütschow. (2023-05-10).
+pik-primap/primap2: PRIMAP2 Version 0.9.7.
+Zenodo. https://doi.org/10.5281/zenodo.7919586
 
 =========
 Changelog
 =========
 
+0.9.7
+-----
+* Fix the test suite to work with Pint release 0.21.
+
 0.9.6
 -----
 * Add dependency on openscm_units > 0.5.1 for compatibility with latest pandas.
 * stop building pdf output documentation, it doesn't support SVG and isn't used much.
 * Drop support for Python version 3.8 to prepare for it being dropped
   in Numpy on April 14.
```

### Comparing `primap2-0.9.6/README.rst` & `primap2-0.9.7/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 Apache License, Version 2.0 as well. The full text of the xarray copyright statement is
 included in the licenses directory.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger and Johannes Gütschow. (2023-04-28).
-pik-primap/primap2: PRIMAP2 Version 0.9.6.
-Zenodo. https://doi.org/10.5281/zenodo.7875234
+Mika Pflüger and Johannes Gütschow. (2023-05-10).
+pik-primap/primap2: PRIMAP2 Version 0.9.7.
+Zenodo. https://doi.org/10.5281/zenodo.7919586
```

### Comparing `primap2-0.9.6/docs/Makefile` & `primap2-0.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/api.rst` & `primap2-0.9.7/docs/api.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/conf.py` & `primap2-0.9.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/data_format_details.rst` & `primap2-0.9.7/docs/data_format_details.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/data_format_examples.ipynb` & `primap2-0.9.7/docs/data_format_examples.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/data_reading.rst` & `primap2-0.9.7/docs/data_reading.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/data_reading_writing_examples/FAOstat.ipynb` & `primap2-0.9.7/docs/data_reading_writing_examples/FAOstat.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/data_reading_writing_examples/PRIMAP-hist.ipynb` & `primap2-0.9.7/docs/data_reading_writing_examples/PRIMAP-hist.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv` & `primap2-0.9.7/docs/data_reading_writing_examples/test_csv_data_sec_cat_if.csv`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/data_reading_writing_examples/test_data_long.ipynb` & `primap2-0.9.7/docs/data_reading_writing_examples/test_data_long.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/data_reading_writing_examples/test_data_wide.ipynb` & `primap2-0.9.7/docs/data_reading_writing_examples/test_data_wide.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/datalad.rst` & `primap2-0.9.7/docs/datalad.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/development.rst` & `primap2-0.9.7/docs/development.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/installation.rst` & `primap2-0.9.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/interchange_format_details.rst` & `primap2-0.9.7/docs/interchange_format_details.rst`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/interchange_format_examples.ipynb` & `primap2-0.9.7/docs/interchange_format_examples.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/make.bat` & `primap2-0.9.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/minimal_ds.nc` & `primap2-0.9.7/docs/minimal_ds.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/opulent_ds.nc` & `primap2-0.9.7/docs/opulent_ds.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/docs/usage.ipynb` & `primap2-0.9.7/docs/usage.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/licenses/pint_xarray_license` & `primap2-0.9.7/licenses/pint_xarray_license`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/licenses/xarray_license` & `primap2-0.9.7/licenses/xarray_license`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap-stubs.patch` & `primap2-0.9.7/primap-stubs.patch`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_aggregate.py` & `primap2-0.9.7/primap2/_aggregate.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_alias_selection.py` & `primap2-0.9.7/primap2/_alias_selection.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_data_format.py` & `primap2-0.9.7/primap2/_data_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_downscale.py` & `primap2-0.9.7/primap2/_downscale.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_merge.py` & `primap2-0.9.7/primap2/_merge.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_metadata.py` & `primap2-0.9.7/primap2/_metadata.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_overview.py` & `primap2-0.9.7/primap2/_overview.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_setters.py` & `primap2-0.9.7/primap2/_setters.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/_units.py` & `primap2-0.9.7/primap2/_units.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/accessors.py` & `primap2-0.9.7/primap2/accessors.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/pm2io/_GHG_inventory_reading.py` & `primap2-0.9.7/primap2/pm2io/_GHG_inventory_reading.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/pm2io/__init__.py` & `primap2-0.9.7/primap2/pm2io/__init__.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/pm2io/_conversion.py` & `primap2-0.9.7/primap2/pm2io/_conversion.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/pm2io/_data_reading.py` & `primap2-0.9.7/primap2/pm2io/_data_reading.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/pm2io/_interchange_format.py` & `primap2-0.9.7/primap2/pm2io/_interchange_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/conftest.py` & `primap2-0.9.7/primap2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv` & `primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.csv`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc` & `primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml` & `primap2-0.9.7/primap2/tests/data/Guetschow-et-al-2021-PRIMAP-crf96_2021-v1.yaml`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/data/test_from_interchange_format_output.nc` & `primap2-0.9.7/primap2/tests/data/test_from_interchange_format_output.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc` & `primap2-0.9.7/primap2/tests/data/test_sum_skip_allna_inhomogeneous_result.nc`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/examples.py` & `primap2-0.9.7/primap2/tests/examples.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_aggregate.py` & `primap2-0.9.7/primap2/tests/test_aggregate.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 
         shared_ds = opulent_ds[["CO2", "SF6 (SARGWP100)"]]
         xr.testing.assert_allclose(
             shared_ds.pr.sum(reduce_to_dim=["area"]),
             shared_ds.sum(set(shared_ds.dims) - {"area (ISO3)"}, keep_attrs=True)
             .to_array("entity")
             .sum("entity", keep_attrs=True),
+            atol=0,
         )
 
 
 def test_any(opulent_ds_or_da):
     xr.testing.assert_identical(
         opulent_ds_or_da.pr.any(dim="area"), opulent_ds_or_da.any(dim="area (ISO3)")
     )
```

### Comparing `primap2-0.9.6/primap2/tests/test_alias_selection.py` & `primap2-0.9.7/primap2/tests/test_alias_selection.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_conversion.py` & `primap2-0.9.7/primap2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_data_format.py` & `primap2-0.9.7/primap2/tests/test_data_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_data_reading.py` & `primap2-0.9.7/primap2/tests/test_data_reading.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_downscale.py` & `primap2-0.9.7/primap2/tests/test_downscale.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_interchange_format.py` & `primap2-0.9.7/primap2/tests/test_interchange_format.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_merge.py` & `primap2-0.9.7/primap2/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_metadata.py` & `primap2-0.9.7/primap2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_overview.py` & `primap2-0.9.7/primap2/tests/test_overview.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_setters.py` & `primap2-0.9.7/primap2/tests/test_setters.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/test_units.py` & `primap2-0.9.7/primap2/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2/tests/utils.py` & `primap2-0.9.7/primap2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/primap2.egg-info/PKG-INFO` & `primap2-0.9.7/primap2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primap2
-Version: 0.9.6
+Version: 0.9.7
 Summary: The next generation of the PRIMAP climate policy analysis suite.
 Home-page: https://github.com/pik-primap/primap2
 Author: Mika Pflüger
 Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://primap2.readthedocs.io/
 Classifier: Development Status :: 3 - Alpha
@@ -79,22 +79,26 @@
 Apache License, Version 2.0 as well. The full text of the xarray copyright statement is
 included in the licenses directory.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger and Johannes Gütschow. (2023-04-28).
-pik-primap/primap2: PRIMAP2 Version 0.9.6.
-Zenodo. https://doi.org/10.5281/zenodo.7875234
+Mika Pflüger and Johannes Gütschow. (2023-05-10).
+pik-primap/primap2: PRIMAP2 Version 0.9.7.
+Zenodo. https://doi.org/10.5281/zenodo.7919586
 
 =========
 Changelog
 =========
 
+0.9.7
+-----
+* Fix the test suite to work with Pint release 0.21.
+
 0.9.6
 -----
 * Add dependency on openscm_units > 0.5.1 for compatibility with latest pandas.
 * stop building pdf output documentation, it doesn't support SVG and isn't used much.
 * Drop support for Python version 3.8 to prepare for it being dropped
   in Numpy on April 14.
```

### Comparing `primap2-0.9.6/primap2.egg-info/SOURCES.txt` & `primap2-0.9.7/primap2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/rosetta/combine_rows-set.ipynb` & `primap2-0.9.7/rosetta/combine_rows-set.ipynb`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/setup.cfg` & `primap2-0.9.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = primap2
-version = 0.9.6
+version = 0.9.7
 author = Mika Pflüger
 author_email = mika.pflueger@climate-resource.com
 description = The next generation of the PRIMAP climate policy analysis suite.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/primap2
 project_urls = 
@@ -16,15 +16,15 @@
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 license = Apache Software License 2.0
-license_file = LICENSE
+license_files = LICENSE
 
 [options]
 packages = 
 	primap2
 	primap2.pm2io
 	primap2.tests
 	primap2.tests.data
```

### Comparing `primap2-0.9.6/tbump.toml` & `primap2-0.9.7/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/primap2/"
 
 [version]
-current = "0.9.6"
+current = "0.9.7"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `primap2-0.9.6/update_changelog.py` & `primap2-0.9.7/update_changelog.py`

 * *Files identical despite different names*

### Comparing `primap2-0.9.6/update_citation_info.py` & `primap2-0.9.7/update_citation_info.py`

 * *Files identical despite different names*

