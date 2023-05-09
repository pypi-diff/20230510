# Comparing `tmp/img2table-0.1.2.tar.gz` & `tmp/img2table-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-0.1.2.tar", last modified: Fri May  5 20:47:46 2023, max compression
+gzip compressed data, was "dist/img2table-0.1.3.tar", last modified: Tue May  9 22:41:48 2023, max compression
```

## Comparing `img2table-0.1.2.tar` & `img2table-0.1.3.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 20:45:49.000000 img2table-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 20:45:49.000000 img2table-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-05 20:45:49.000000 img2table-0.1.2/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 20:45:49.000000 img2table-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-05 20:45:49.000000 img2table-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19679 2023-05-05 20:47:46.000000 img2table-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15791 2023-05-05 20:45:49.000000 img2table-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 20:45:49.000000 img2table-0.1.2/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/data/borderless_aws.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/data/borderless_ocr.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-05 20:45:49.000000 img2table-0.1.2/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 20:45:49.000000 img2table-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 20:45:49.000000 img2table-0.1.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-05 20:45:49.000000 img2table-0.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-05 20:45:49.000000 img2table-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-05 20:47:46.000000 img2table-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 20:45:49.000000 img2table-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-05 20:45:49.000000 img2table-0.1.2/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19679 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 20:47:46.000000 img2table-0.1.2/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/image/test_data/dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/image/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:47:46.000000 img2table-0.1.2/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-05 20:45:49.000000 img2table-0.1.2/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 22:39:27.000000 img2table-0.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-09 22:39:27.000000 img2table-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 22:39:27.000000 img2table-0.1.3/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-09 22:39:27.000000 img2table-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-09 22:39:27.000000 img2table-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-09 22:41:48.000000 img2table-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-05-09 22:39:27.000000 img2table-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-09 22:39:27.000000 img2table-0.1.3/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46047 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/borderless_aws.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/borderless_ocr.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 22:39:27.000000 img2table-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 22:39:27.000000 img2table-0.1.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-09 22:39:27.000000 img2table-0.1.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-09 22:39:27.000000 img2table-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 22:41:48.000000 img2table-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 22:39:27.000000 img2table-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-0.1.2/LICENSE.txt` & `img2table-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/Makefile` & `img2table-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/PKG-INFO` & `img2table-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.1.2
+Version: 0.1.3
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -70,15 +70,14 @@
         <li>OpenEXR Image files - *.exr</li>
         <li>Radiance HDR - <em>.hdr, </em>.pic</li>
         <li>Raster and Vector geospatial data supported by GDAL<br>
         <cite><a href="https://docs.opencv.org/4.x/d4/da8/group__imgcodecs.html#ga288b8b3da0892bd651fce07b3bbd3a56">OpenCV: Image file reading and writing</a></cite></li>
         </ul>
         </blockquote>
         </details>
-        <br>
         Multi-page images are not supported.
         
         ---
         
         ### PDF <a name="pdf-formats"></a>
         
         Both native and scanned PDF files are supported.
@@ -128,15 +127,15 @@
         PDF pages are converted to images with a 200 DPI for table identification.
         
         ---
         
         ### OCR <a name="ocr"></a>
         
         `img2table` provides an interface for several OCR services and tools in order to parse table content.<br>
-        If possible (i.e for searchable PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
+        If possible (i.e for native PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
         
         <details>
         <summary>Tesseract<a name="tesseract"></a></summary>
         <br>
         
         ```python
         from img2table.ocr import TesseractOCR
@@ -281,23 +280,23 @@
         ocr = TesseractOCR(n_threads=1, lang="eng")
         
         # Instantiation of document, either an image or a PDF
         doc = Image(src)
         
         # Table extraction
         extracted_tables = doc.extract_tables(ocr=ocr,
-                                              implicit_rows=True,
+                                              implicit_rows=False,
                                               borderless_tables=False,
                                               min_confidence=50)
         ```
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
-        >    <dt>implicit_rows : bool, optional, default <code>True</code></dt>
+        >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
         >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
         >    <dt>min_confidence : int, optional, default <code>50</code></dt>
         >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
         ></dl>
         
@@ -310,15 +309,15 @@
         > <h4>Attributes</h4>
         ><dl>
         >    <dt>bbox : <code><a href="/src/img2table/tables/objects/extraction.py#L12" target="_self">BBox</a></code></dt>
         >    <dd style="font-style: italic;">Table bounding box</dd>
         >    <dt>title : str</dt>
         >    <dd style="font-style: italic;">Extracted title of the table</dd>
         >    <dt>content : <code>OrderedDict</code></dt>
-        >    <dd style="font-style: italic;">Dict with with row indexes as keys and list of <code><a href="/src/img2table/tables/objects/extraction.py#L20" target="_self">TableCell</a></code> objects as values</dd>
+        >    <dd style="font-style: italic;">Dict with row indexes as keys and list of <code><a href="/src/img2table/tables/objects/extraction.py#L20" target="_self">TableCell</a></code> objects as values</dd>
         >    <dt>df : <code>pd.DataFrame</code></dt>
         >    <dd style="font-style: italic;">Pandas DataFrame representation of the table</dd>
         ></dl>
         
         <h5 style="color:grey">Images</h5>
         
         `extract_tables` method from the `Image` class returns a list of `ExtractedTable` objects. 
@@ -350,28 +349,28 @@
         
         # Instantiation of OCR
         ocr = TesseractOCR(n_threads=1, lang="eng")
         
         # Instantiation of document, either an image or a PDF
         doc = Image(src)
         
-        # Extraction of tables and creation of an xlsx file containing tables
+        # Extraction of tables and creation of a xlsx file containing tables
         doc.to_xlsx(dest=dest,
                     ocr=ocr,
-                    implicit_rows=True,
+                    implicit_rows=False,
                     borderless_tables=False,
                     min_confidence=50)
         ```
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>dest : str, <code>pathlib.Path</code> or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">Destination for xlsx file</dd>
         >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
-        >    <dt>implicit_rows : bool, optional, default <code>True</code></dt>
+        >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
         >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
         >    <dt>min_confidence : int, optional, default <code>50</code></dt>
         >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
         ></dl>
         > <h4>Returns</h4>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.1.2 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.1.3 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -38,16 +38,15 @@
          * PFM files - *.pfm
          * Sun rasters - .sr,.ras
          * TIFF files - .tiff,.tif
          * OpenEXR Image files - *.exr
          * Radiance HDR - .hdr,.pic
          * Raster and Vector geospatial data supported by GDAL
            OpenCV:_Image_file_reading_and_writing
-
-Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
+ Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
 files are supported. ## Usage  ### Documents  #### Images  Images are
 instantiated as follows : ```python from img2table.document import Image image
 = Image(src, detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 
@@ -59,16 +58,16 @@
 img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
-If possible (i.e for searchable PDF), PDF text will be extracted directly from
-the file and the OCR service/tool will not be called.  Tesseract
+If possible (i.e for native PDF), PDF text will be extracted directly from the
+file and the OCR service/tool will not be called.  Tesseract
 ```python from img2table.ocr import TesseractOCR ocr = TesseractOCR
 (n_threads=1, lang="eng", psm=11, tessdata_dir="...") ``` >
 *** Parameters ***
 >
 >
 *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires
 prior installation. Check [documentation](https://tesseract-ocr.github.io/
@@ -114,15 +113,15 @@
 >
 
  --- ### Table extraction  Multiple tables can be extracted at once from a PDF
 page/ an image using the `extract_tables` method of a document. ```python from
 img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) # Table
-extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=True,
+extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=False,
 borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 *Borderless table extraction released in version 0.0.14* #### Method return The
 [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
 used to model extracted tables from documents. >
@@ -140,16 +139,16 @@
 (...), ...] } ``` ### Excel export  Tables extracted from a document can be
 exported to a xlsx file. The resulting file is composed of one worksheet per
 extracted table.
 Method arguments are mostly common with the `extract_tables` method. ```python
 from img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) #
-Extraction of tables and creation of an xlsx file containing tables doc.to_xlsx
-(dest=dest, ocr=ocr, implicit_rows=True, borderless_tables=False,
+Extraction of tables and creation of a xlsx file containing tables doc.to_xlsx
+(dest=dest, ocr=ocr, implicit_rows=False, borderless_tables=False,
 min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 >
 *** Returns ***
 > If a io.BytesIO buffer is passed as dest arg, it is returned containing xlsx
```

### Comparing `img2table-0.1.2/README.md` & `img2table-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 <li>OpenEXR Image files - *.exr</li>
 <li>Radiance HDR - <em>.hdr, </em>.pic</li>
 <li>Raster and Vector geospatial data supported by GDAL<br>
 <cite><a href="https://docs.opencv.org/4.x/d4/da8/group__imgcodecs.html#ga288b8b3da0892bd651fce07b3bbd3a56">OpenCV: Image file reading and writing</a></cite></li>
 </ul>
 </blockquote>
 </details>
-<br>
 Multi-page images are not supported.
 
 ---
 
 ### PDF <a name="pdf-formats"></a>
 
 Both native and scanned PDF files are supported.
@@ -121,15 +120,15 @@
 PDF pages are converted to images with a 200 DPI for table identification.
 
 ---
 
 ### OCR <a name="ocr"></a>
 
 `img2table` provides an interface for several OCR services and tools in order to parse table content.<br>
-If possible (i.e for searchable PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
+If possible (i.e for native PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
 
 <details>
 <summary>Tesseract<a name="tesseract"></a></summary>
 <br>
 
 ```python
 from img2table.ocr import TesseractOCR
@@ -274,23 +273,23 @@
 ocr = TesseractOCR(n_threads=1, lang="eng")
 
 # Instantiation of document, either an image or a PDF
 doc = Image(src)
 
 # Table extraction
 extracted_tables = doc.extract_tables(ocr=ocr,
-                                      implicit_rows=True,
+                                      implicit_rows=False,
                                       borderless_tables=False,
                                       min_confidence=50)
 ```
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
->    <dt>implicit_rows : bool, optional, default <code>True</code></dt>
+>    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
 >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
 >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
 >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
 >    <dt>min_confidence : int, optional, default <code>50</code></dt>
 >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
 ></dl>
 
@@ -303,15 +302,15 @@
 > <h4>Attributes</h4>
 ><dl>
 >    <dt>bbox : <code><a href="/src/img2table/tables/objects/extraction.py#L12" target="_self">BBox</a></code></dt>
 >    <dd style="font-style: italic;">Table bounding box</dd>
 >    <dt>title : str</dt>
 >    <dd style="font-style: italic;">Extracted title of the table</dd>
 >    <dt>content : <code>OrderedDict</code></dt>
->    <dd style="font-style: italic;">Dict with with row indexes as keys and list of <code><a href="/src/img2table/tables/objects/extraction.py#L20" target="_self">TableCell</a></code> objects as values</dd>
+>    <dd style="font-style: italic;">Dict with row indexes as keys and list of <code><a href="/src/img2table/tables/objects/extraction.py#L20" target="_self">TableCell</a></code> objects as values</dd>
 >    <dt>df : <code>pd.DataFrame</code></dt>
 >    <dd style="font-style: italic;">Pandas DataFrame representation of the table</dd>
 ></dl>
 
 <h5 style="color:grey">Images</h5>
 
 `extract_tables` method from the `Image` class returns a list of `ExtractedTable` objects. 
@@ -343,28 +342,28 @@
 
 # Instantiation of OCR
 ocr = TesseractOCR(n_threads=1, lang="eng")
 
 # Instantiation of document, either an image or a PDF
 doc = Image(src)
 
-# Extraction of tables and creation of an xlsx file containing tables
+# Extraction of tables and creation of a xlsx file containing tables
 doc.to_xlsx(dest=dest,
             ocr=ocr,
-            implicit_rows=True,
+            implicit_rows=False,
             borderless_tables=False,
             min_confidence=50)
 ```
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>dest : str, <code>pathlib.Path</code> or <code>io.BytesIO</code>, required</dt>
 >    <dd style="font-style: italic;">Destination for xlsx file</dd>
 >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
->    <dt>implicit_rows : bool, optional, default <code>True</code></dt>
+>    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
 >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
 >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
 >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
 >    <dt>min_confidence : int, optional, default <code>50</code></dt>
 >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
 ></dl>
 > <h4>Returns</h4>
```

#### html2text {}

```diff
@@ -34,16 +34,15 @@
          * PFM files - *.pfm
          * Sun rasters - .sr,.ras
          * TIFF files - .tiff,.tif
          * OpenEXR Image files - *.exr
          * Radiance HDR - .hdr,.pic
          * Raster and Vector geospatial data supported by GDAL
            OpenCV:_Image_file_reading_and_writing
-
-Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
+ Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
 files are supported. ## Usage  ### Documents  #### Images  Images are
 instantiated as follows : ```python from img2table.document import Image image
 = Image(src, detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 
@@ -55,16 +54,16 @@
 img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
-If possible (i.e for searchable PDF), PDF text will be extracted directly from
-the file and the OCR service/tool will not be called.  Tesseract
+If possible (i.e for native PDF), PDF text will be extracted directly from the
+file and the OCR service/tool will not be called.  Tesseract
 ```python from img2table.ocr import TesseractOCR ocr = TesseractOCR
 (n_threads=1, lang="eng", psm=11, tessdata_dir="...") ``` >
 *** Parameters ***
 >
 >
 *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires
 prior installation. Check [documentation](https://tesseract-ocr.github.io/
@@ -110,15 +109,15 @@
 >
 
  --- ### Table extraction  Multiple tables can be extracted at once from a PDF
 page/ an image using the `extract_tables` method of a document. ```python from
 img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) # Table
-extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=True,
+extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=False,
 borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 *Borderless table extraction released in version 0.0.14* #### Method return The
 [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
 used to model extracted tables from documents. >
@@ -136,16 +135,16 @@
 (...), ...] } ``` ### Excel export  Tables extracted from a document can be
 exported to a xlsx file. The resulting file is composed of one worksheet per
 extracted table.
 Method arguments are mostly common with the `extract_tables` method. ```python
 from img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) #
-Extraction of tables and creation of an xlsx file containing tables doc.to_xlsx
-(dest=dest, ocr=ocr, implicit_rows=True, borderless_tables=False,
+Extraction of tables and creation of a xlsx file containing tables doc.to_xlsx
+(dest=dest, ocr=ocr, implicit_rows=False, borderless_tables=False,
 min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 >
 *** Returns ***
 > If a io.BytesIO buffer is passed as dest arg, it is returned containing xlsx
```

### Comparing `img2table-0.1.2/examples/Basic_usage.ipynb` & `img2table-0.1.3/examples/Basic_usage.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999755658436214%*

 * *Differences: {"'cells'": "{13: {'source': {insert: [(4, '                                      "*

 * *            "implicit_rows=False,\\n')], delete: [4]}}, 16: {'source': {insert: [(5, '            "*

 * *            "implicit_rows=False,\\n')], delete: [5]}}}"}*

```diff
@@ -339,15 +339,15 @@
                 }
             ],
             "source": [
                 "pdf = PDF(src=\"data/tables.pdf\")\n",
                 "\n",
                 "# Extract tables\n",
                 "extracted_tables = pdf.extract_tables(ocr=tesseract_ocr,\n",
-                "                                      implicit_rows=True,\n",
+                "                                      implicit_rows=False,\n",
                 "                                      borderless_tables=False,\n",
                 "                                      min_confidence=50)\n",
                 "\n",
                 "extracted_tables"
             ]
         },
         {
@@ -663,15 +663,15 @@
             ],
             "source": [
                 "pdf = PDF(src=\"data/tables.pdf\")\n",
                 "\n",
                 "# Export to file\n",
                 "pdf.to_xlsx('data/tables.xlsx',\n",
                 "            ocr=tesseract_ocr,\n",
-                "            implicit_rows=True,\n",
+                "            implicit_rows=False,\n",
                 "            borderless_tables=False,\n",
                 "            min_confidence=50)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
```

### Comparing `img2table-0.1.2/examples/Implicit_rows.ipynb` & `img2table-0.1.3/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/examples/borderless.ipynb` & `img2table-0.1.3/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/examples/data/borderless_aws.jpg` & `img2table-0.1.3/examples/data/borderless_aws.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/examples/data/borderless_ocr.jpg` & `img2table-0.1.3/examples/data/borderless_ocr.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/examples/data/implicit.png` & `img2table-0.1.3/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/examples/data/tables.pdf` & `img2table-0.1.3/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/examples/data/tables.png` & `img2table-0.1.3/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/examples/data/tables.xlsx` & `img2table-0.1.3/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/setup.cfg` & `img2table-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/__init__.py` & `img2table-0.1.3/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/document/base/__init__.py` & `img2table-0.1.3/src/img2table/document/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             with io.open(self.src, 'rb') as f:
                 return f.read()
 
     @property
     def images(self) -> Iterator[np.ndarray]:
         raise NotImplementedError
 
-    def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = True, borderless_tables: bool = False,
+    def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = False, borderless_tables: bool = False,
                        min_confidence: int = 50) -> Dict[int, List[ExtractedTable]]:
         """
         Extract tables from document
         :param ocr: OCRInstance object used to extract table content
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :param borderless_tables: boolean indicating if borderless tables should be detected
         :param min_confidence: minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)
@@ -79,15 +79,15 @@
             tables = {self.pages[k]: v for k, v in tables.items()}
 
         # Reset ocr_df attribute
         self.ocr_df = None
 
         return tables
 
-    def to_xlsx(self, dest: Union[str, Path, io.BytesIO], ocr: "OCRInstance" = None, implicit_rows: bool = True,
+    def to_xlsx(self, dest: Union[str, Path, io.BytesIO], ocr: "OCRInstance" = None, implicit_rows: bool = False,
                 borderless_tables: bool = False, min_confidence: int = 50) -> Optional[io.BytesIO]:
         """
         Create xlsx file containing all extracted tables from document
         :param dest: destination for xlsx file
         :param ocr: OCRInstance object used to extract table content
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :param borderless_tables: boolean indicating if borderless tables should be detected
```

### Comparing `img2table-0.1.2/src/img2table/document/base/rotation.py` & `img2table-0.1.3/src/img2table/document/base/rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/document/image.py` & `img2table-0.1.3/src/img2table/document/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         super(Image, self).__post_init__()
 
     @cached_property
     def images(self) -> List[np.ndarray]:
         img = cv2.imdecode(np.frombuffer(self.bytes, np.uint8), cv2.IMREAD_GRAYSCALE)
         return [fix_rotation_image(img=img) if self.detect_rotation else img]
 
-    def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = True, borderless_tables: bool = False,
+    def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = False, borderless_tables: bool = False,
                        min_confidence: int = 50) -> List[ExtractedTable]:
         """
         Extract tables from document
         :param ocr: OCRInstance object used to extract table content
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :param borderless_tables: boolean indicating if borderless tables should be detected
         :param min_confidence: minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)
```

### Comparing `img2table-0.1.2/src/img2table/document/pdf.py` & `img2table-0.1.3/src/img2table/document/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             page = doc.load_page(page_id=page_number)
             pix = page.get_pixmap(matrix=mat)
             img = np.frombuffer(buffer=pix.samples, dtype=np.uint8).reshape((pix.height, pix.width, 3))
             images.append(cv2.cvtColor(img, cv2.COLOR_BGR2GRAY))
 
         return images
 
-    def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = True, borderless_tables: bool = False,
+    def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = False, borderless_tables: bool = False,
                        min_confidence: int = 50) -> Dict[int, List[ExtractedTable]]:
         """
         Extract tables from document
         :param ocr: OCRInstance object used to extract table content
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :param borderless_tables: boolean indicating if borderless tables should be detected
         :param min_confidence: minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)
```

### Comparing `img2table-0.1.2/src/img2table/ocr/aws_textract.py` & `img2table-0.1.3/src/img2table/ocr/aws_textract.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,10 +93,10 @@
         Convert list of OCR elements by page to OCRDataframe object
         :param content: list of OCR elements by page
         :return: OCRDataframe object corresponding to content
         """
         list_dfs = list()
         for page_elements in content:
             if page_elements:
-                list_dfs.append(pl.LazyFrame(data=page_elements))
+                list_dfs.append(pl.LazyFrame(data=page_elements, schema=self.pl_schema))
 
         return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.1.2/src/img2table/ocr/azure.py` & `img2table-0.1.3/src/img2table/ocr/azure.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,10 +103,10 @@
                             "y1": min(bbox[1::2]),
                             "y2": max(bbox[1::2])
                         }
 
                         word_elements.append(d_word)
 
             if word_elements:
-                list_dfs.append(pl.LazyFrame(data=word_elements))
+                list_dfs.append(pl.LazyFrame(data=word_elements, schema=self.pl_schema))
 
         return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.1.2/src/img2table/ocr/data.py` & `img2table-0.1.3/src/img2table/ocr/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -151,12 +151,12 @@
             table.items[rec.get('row')].items[rec.get('col')].content = rec.get('text') or None
 
         return table
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             try:
-                assert self.df.collect(streaming=True).sort(by='id').frame_equal(other.df.collect(streaming=True).sort(by='id'))
+                assert self.df.collect(streaming=True).sort(by=['id']).frame_equal(other.df.collect(streaming=True).sort(by=['id']))
                 return True
             except AssertionError:
                 return False
         return False
```

### Comparing `img2table-0.1.2/src/img2table/ocr/google_vision.py` & `img2table-0.1.3/src/img2table/ocr/google_vision.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,10 +242,10 @@
         Convert list of OCR elements by page to OCRDataframe object
         :param content: list of OCR elements by page
         :return: OCRDataframe object corresponding to content
         """
         list_dfs = list()
         for page_elements in content:
             if page_elements:
-                list_dfs.append(pl.LazyFrame(data=page_elements))
+                list_dfs.append(pl.LazyFrame(data=page_elements, schema=self.pl_schema))
 
         return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.1.2/src/img2table/ocr/paddle.py` & `img2table-0.1.3/src/img2table/ocr/paddle.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,8 +87,8 @@
                     "y1": round(min([edge[1] for edge in bbox])),
                     "x2": round(max([edge[0] for edge in bbox])),
                     "y2": round(max([edge[1] for edge in bbox]))
                 }
 
                 list_elements.append(dict_word)
 
-        return OCRDataframe(df=pl.LazyFrame(list_elements)) if list_elements else None
+        return OCRDataframe(df=pl.LazyFrame(list_elements, schema=self.pl_schema)) if list_elements else None
```

### Comparing `img2table-0.1.2/src/img2table/ocr/pdf.py` & `img2table-0.1.3/src/img2table/ocr/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,10 +67,10 @@
         if min(map(len, content)) == 0:
             return None
 
         # Create OCRDataframe
         list_dfs = list()
         for page_elements in content:
             if page_elements:
-                list_dfs.append(pl.LazyFrame(data=page_elements))
+                list_dfs.append(pl.LazyFrame(data=page_elements, schema=self.pl_schema))
 
         return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.1.2/src/img2table/ocr/tesseract.py` & `img2table-0.1.3/src/img2table/ocr/tesseract.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,10 +133,10 @@
                 d_el["x1"], d_el["y1"], d_el["x2"], d_el["y2"] = tuple(
                     int(element) for element in re.sub(r"^bbox\s", "", bbox).split())
 
                 list_elements.append(d_el)
 
             # Create dataframe
             if list_elements:
-                list_dfs.append(pl.LazyFrame(data=list_elements))
+                list_dfs.append(pl.LazyFrame(data=list_elements, schema=self.pl_schema))
 
         return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.1.2/src/img2table/tables/image.py` & `img2table-0.1.3/src/img2table/tables/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 # Get content
                 borderless_tbs = [table.get_content(ocr_df=self.ocr_df, min_confidence=self.min_confidence)
                                   for table in borderless_tbs]
 
             # Add to tables
             self.tables += [tb for tb in borderless_tbs if min(tb.nb_rows, tb.nb_columns) >= 2]
 
-    def extract_tables(self, implicit_rows: bool = True, borderless_tables: bool = False) -> List[ExtractedTable]:
+    def extract_tables(self, implicit_rows: bool = False, borderless_tables: bool = False) -> List[ExtractedTable]:
         """
         Identify and extract tables from image
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :param borderless_tables: boolean indicating if borderless tables should be detected
         :return: list of identified tables
         """
         # Extract bordered tables
```

### Comparing `img2table-0.1.2/src/img2table/tables/metrics.py` & `img2table-0.1.3/src/img2table/tables/metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/objects/__init__.py` & `img2table-0.1.3/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/objects/extraction.py` & `img2table-0.1.3/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/objects/line.py` & `img2table-0.1.3/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/objects/row.py` & `img2table-0.1.3/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/objects/table.py` & `img2table-0.1.3/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/borderless_tables/column_delimiters.py` & `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/borderless_tables/lines.py` & `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/common.py` & `img2table-0.1.3/src/img2table/tables/processing/common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/prepare_image.py` & `img2table-0.1.3/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table/tables/processing/text/titles.py` & `img2table-0.1.3/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/src/img2table.egg-info/PKG-INFO` & `img2table-0.1.3/src/img2table.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.1.2
+Version: 0.1.3
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -70,15 +70,14 @@
         <li>OpenEXR Image files - *.exr</li>
         <li>Radiance HDR - <em>.hdr, </em>.pic</li>
         <li>Raster and Vector geospatial data supported by GDAL<br>
         <cite><a href="https://docs.opencv.org/4.x/d4/da8/group__imgcodecs.html#ga288b8b3da0892bd651fce07b3bbd3a56">OpenCV: Image file reading and writing</a></cite></li>
         </ul>
         </blockquote>
         </details>
-        <br>
         Multi-page images are not supported.
         
         ---
         
         ### PDF <a name="pdf-formats"></a>
         
         Both native and scanned PDF files are supported.
@@ -128,15 +127,15 @@
         PDF pages are converted to images with a 200 DPI for table identification.
         
         ---
         
         ### OCR <a name="ocr"></a>
         
         `img2table` provides an interface for several OCR services and tools in order to parse table content.<br>
-        If possible (i.e for searchable PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
+        If possible (i.e for native PDF), PDF text will be extracted directly from the file and the OCR service/tool will not be called.
         
         <details>
         <summary>Tesseract<a name="tesseract"></a></summary>
         <br>
         
         ```python
         from img2table.ocr import TesseractOCR
@@ -281,23 +280,23 @@
         ocr = TesseractOCR(n_threads=1, lang="eng")
         
         # Instantiation of document, either an image or a PDF
         doc = Image(src)
         
         # Table extraction
         extracted_tables = doc.extract_tables(ocr=ocr,
-                                              implicit_rows=True,
+                                              implicit_rows=False,
                                               borderless_tables=False,
                                               min_confidence=50)
         ```
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
-        >    <dt>implicit_rows : bool, optional, default <code>True</code></dt>
+        >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
         >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
         >    <dt>min_confidence : int, optional, default <code>50</code></dt>
         >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
         ></dl>
         
@@ -310,15 +309,15 @@
         > <h4>Attributes</h4>
         ><dl>
         >    <dt>bbox : <code><a href="/src/img2table/tables/objects/extraction.py#L12" target="_self">BBox</a></code></dt>
         >    <dd style="font-style: italic;">Table bounding box</dd>
         >    <dt>title : str</dt>
         >    <dd style="font-style: italic;">Extracted title of the table</dd>
         >    <dt>content : <code>OrderedDict</code></dt>
-        >    <dd style="font-style: italic;">Dict with with row indexes as keys and list of <code><a href="/src/img2table/tables/objects/extraction.py#L20" target="_self">TableCell</a></code> objects as values</dd>
+        >    <dd style="font-style: italic;">Dict with row indexes as keys and list of <code><a href="/src/img2table/tables/objects/extraction.py#L20" target="_self">TableCell</a></code> objects as values</dd>
         >    <dt>df : <code>pd.DataFrame</code></dt>
         >    <dd style="font-style: italic;">Pandas DataFrame representation of the table</dd>
         ></dl>
         
         <h5 style="color:grey">Images</h5>
         
         `extract_tables` method from the `Image` class returns a list of `ExtractedTable` objects. 
@@ -350,28 +349,28 @@
         
         # Instantiation of OCR
         ocr = TesseractOCR(n_threads=1, lang="eng")
         
         # Instantiation of document, either an image or a PDF
         doc = Image(src)
         
-        # Extraction of tables and creation of an xlsx file containing tables
+        # Extraction of tables and creation of a xlsx file containing tables
         doc.to_xlsx(dest=dest,
                     ocr=ocr,
-                    implicit_rows=True,
+                    implicit_rows=False,
                     borderless_tables=False,
                     min_confidence=50)
         ```
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>dest : str, <code>pathlib.Path</code> or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">Destination for xlsx file</dd>
         >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
-        >    <dt>implicit_rows : bool, optional, default <code>True</code></dt>
+        >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
         >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
         >    <dt>min_confidence : int, optional, default <code>50</code></dt>
         >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
         ></dl>
         > <h4>Returns</h4>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.1.2 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.1.3 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -38,16 +38,15 @@
          * PFM files - *.pfm
          * Sun rasters - .sr,.ras
          * TIFF files - .tiff,.tif
          * OpenEXR Image files - *.exr
          * Radiance HDR - .hdr,.pic
          * Raster and Vector geospatial data supported by GDAL
            OpenCV:_Image_file_reading_and_writing
-
-Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
+ Multi-page images are not supported. --- ### PDF  Both native and scanned PDF
 files are supported. ## Usage  ### Documents  #### Images  Images are
 instantiated as follows : ```python from img2table.document import Image image
 = Image(src, detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 
@@ -59,16 +58,16 @@
 img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
-If possible (i.e for searchable PDF), PDF text will be extracted directly from
-the file and the OCR service/tool will not be called.  Tesseract
+If possible (i.e for native PDF), PDF text will be extracted directly from the
+file and the OCR service/tool will not be called.  Tesseract
 ```python from img2table.ocr import TesseractOCR ocr = TesseractOCR
 (n_threads=1, lang="eng", psm=11, tessdata_dir="...") ``` >
 *** Parameters ***
 >
 >
 *Usage of [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract) requires
 prior installation. Check [documentation](https://tesseract-ocr.github.io/
@@ -114,15 +113,15 @@
 >
 
  --- ### Table extraction  Multiple tables can be extracted at once from a PDF
 page/ an image using the `extract_tables` method of a document. ```python from
 img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) # Table
-extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=True,
+extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=False,
 borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 *Borderless table extraction released in version 0.0.14* #### Method return The
 [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
 used to model extracted tables from documents. >
@@ -140,16 +139,16 @@
 (...), ...] } ``` ### Excel export  Tables extracted from a document can be
 exported to a xlsx file. The resulting file is composed of one worksheet per
 extracted table.
 Method arguments are mostly common with the `extract_tables` method. ```python
 from img2table.ocr import TesseractOCR from img2table.document import Image #
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) #
-Extraction of tables and creation of an xlsx file containing tables doc.to_xlsx
-(dest=dest, ocr=ocr, implicit_rows=True, borderless_tables=False,
+Extraction of tables and creation of a xlsx file containing tables doc.to_xlsx
+(dest=dest, ocr=ocr, implicit_rows=False, borderless_tables=False,
 min_confidence=50) ``` >
 *** Parameters ***
 >
 >
 >
 *** Returns ***
 > If a io.BytesIO buffer is passed as dest arg, it is returned containing xlsx
```

### Comparing `img2table-0.1.2/src/img2table.egg-info/SOURCES.txt` & `img2table-0.1.3/src/img2table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/_mock_data/azure.pkl` & `img2table-0.1.3/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/_mock_data/tesseract_hocr.html` & `img2table-0.1.3/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/_mock_data/textract.json` & `img2table-0.1.3/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/_mock_data/vision.json` & `img2table-0.1.3/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/_mock_data/vision.pkl` & `img2table-0.1.3/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/conftest.py` & `img2table-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/base/test_data/test.png` & `img2table-0.1.3/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/base/test_rotation.py` & `img2table-0.1.3/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/image/test_data/blank.png` & `img2table-0.1.3/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/image/test_data/dark.png` & `img2table-0.1.3/tests/document/image/test_data/dark.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/image/test_data/expected.xlsx` & `img2table-0.1.3/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/image/test_data/test.png` & `img2table-0.1.3/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/image/test_image.py` & `img2table-0.1.3/tests/document/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/pdf/test_data/test.pdf` & `img2table-0.1.3/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/document/pdf/test_pdf.py` & `img2table-0.1.3/tests/document/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-0.1.3/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/aws_textract/test_data/content.json` & `img2table-0.1.3/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-0.1.3/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-page;class;id;parent;value;confidence;x1;x2;y1;y2
-0;ocrx_word;88a72bbd-1228-4524-9acd-1c78d457965b;c1a786cc-b3bd-4a74-b286-8307156e136f;Title;100;383;423;39;55
-0;ocrx_word;ecc305af-e32c-4f01-8fd6-d769844add3f;bef0489e-378c-4af6-9804-fd420b65190c;Test;100;965;1000;40;55
-0;ocrx_word;c32bb03e-a29a-4695-aa6b-59bb88bbd25a;bef0489e-378c-4af6-9804-fd420b65190c;1;100;1006;1016;40;55
-0;ocrx_word;ea0e1f37-41e5-4a3e-83ef-edd2e0165e5f;f68dddd3-e0c8-411d-820d-fcfd853d28fe;Test;100;1061;1096;40;55
-0;ocrx_word;04e791eb-62ae-4d68-8ee5-2d672e0c3804;f68dddd3-e0c8-411d-820d-fcfd853d28fe;2;100;1101;1112;40;55
-0;ocrx_word;786208ae-2e98-44e5-a212-730fb60964b0;0712e1d7-2c31-4b62-82f6-441087e63779;Line;100;40;76;91;106
-0;ocrx_word;a809159b-3f1f-4d29-b68d-8ed34e61c31e;0712e1d7-2c31-4b62-82f6-441087e63779;1 -;69;82;105;91;107
-0;ocrx_word;a237beef-d207-4b3d-ad5c-37f1da97e6d0;0712e1d7-2c31-4b62-82f6-441087e63779;-;94;96;104;98;102
-0;ocrx_word;7fd41b4d-dc88-4593-bfdb-84887df80a67;0712e1d7-2c31-4b62-82f6-441087e63779;Col;100;109;138;90;106
-0;ocrx_word;f11bb2bb-b067-4cdd-9913-d8e094016ca3;0712e1d7-2c31-4b62-82f6-441087e63779;1;100;143;153;91;106
-0;ocrx_word;4bf52fb3-9996-41aa-95a0-872178c5e5c8;2ab46d87-2708-4cf3-b69e-9f2763af69a1;Line;100;280;316;91;106
-0;ocrx_word;e2a5eca7-be40-411b-8f5c-8e97c6eae001;2ab46d87-2708-4cf3-b69e-9f2763af69a1;1;100;322;332;91;106
-0;ocrx_word;32a19f1a-a490-4688-b8d5-b5d31c6f1881;2ab46d87-2708-4cf3-b69e-9f2763af69a1;Col;99;349;377;90;106
-0;ocrx_word;0ec66650-6ad5-4240-9983-c829de6dfa55;2ab46d87-2708-4cf3-b69e-9f2763af69a1;2;100;383;393;91;106
-0;ocrx_word;2b0e83f0-e0e2-49e2-92c1-7708973e3312;14c6de15-1642-41f6-a23c-357eaea5718c;Line;100;499;535;91;106
-0;ocrx_word;80743548-4e4e-4ce9-a9bf-306fb94dd079;14c6de15-1642-41f6-a23c-357eaea5718c;1;100;541;551;91;106
-0;ocrx_word;9f1f1f24-ecdb-4163-b986-3d211946a406;14c6de15-1642-41f6-a23c-357eaea5718c;-;97;556;563;97;102
-0;ocrx_word;e574f419-ef0d-4af9-b22e-29e337510b2a;14c6de15-1642-41f6-a23c-357eaea5718c;Col;99;568;596;90;106
-0;ocrx_word;b89c8819-5962-4f71-9b7d-a8cb633f0ea9;14c6de15-1642-41f6-a23c-357eaea5718c;3;100;602;612;91;106
-0;ocrx_word;931dac4a-8623-4ed4-b69d-d560e46b0965;3a1cb207-ccd9-498b-b31d-f71cae319ee1;Test;100;965;1001;91;106
-0;ocrx_word;eddd1221-175d-4acb-9d72-97d1940e9d80;3a1cb207-ccd9-498b-b31d-f71cae319ee1;3;100;1006;1016;91;106
-0;ocrx_word;5df5a361-60d4-4451-9501-8b932e6147b0;65f17b42-1979-445a-8274-db2234589249;Test;100;1061;1097;91;106
-0;ocrx_word;881eaaef-100b-4c2e-a0ad-9f99339e4d39;65f17b42-1979-445a-8274-db2234589249;4;100;1101;1113;91;106
-0;ocrx_word;57a883af-3e0b-4859-95ce-94fa6353fc80;bab0aefa-5ccf-42ea-8700-4390d26c1074;Line;100;40;77;142;157
-0;ocrx_word;f9467369-4c9c-4f2e-b205-d9a5f692ee9a;bab0aefa-5ccf-42ea-8700-4390d26c1074;2;100;81;92;142;157
-0;ocrx_word;e6036250-f943-4b8a-93d3-9dd7a28032bc;bab0aefa-5ccf-42ea-8700-4390d26c1074;-;96;97;104;149;153
-0;ocrx_word;56175999-eb57-4350-86b5-128bc6d167c7;bab0aefa-5ccf-42ea-8700-4390d26c1074;Col;100;109;137;141;157
-0;ocrx_word;7a4757f1-b91b-411c-8630-1bf10db1ac44;bab0aefa-5ccf-42ea-8700-4390d26c1074;1;100;143;153;142;157
-0;ocrx_word;59aa3ef7-d1bc-41ec-a119-ab36f35c9bc1;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;Line;100;499;535;142;157
-0;ocrx_word;ba7809d1-759a-4e0d-8795-ab9523a3724b;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;2;100;541;551;142;157
-0;ocrx_word;e11912eb-f984-434d-bf56-9f1b44c96338;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;-;98;556;563;149;153
-0;ocrx_word;57ec3919-7226-41fd-a53f-0c95722270bd;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;Col;99;568;596;141;157
-0;ocrx_word;3e277cae-536e-4bf0-a2f2-0caa03fd6258;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;3;100;602;612;142;157
-0;ocrx_word;793c3b43-171a-4f7e-9aaf-0c7845df2a8b;af397266-7263-46bc-968f-9153c323df2a;Line;100;40;76;193;208
-0;ocrx_word;c33c469a-67ba-4370-b9c6-ddff5b6f8be2;af397266-7263-46bc-968f-9153c323df2a;3;100;81;92;193;208
-0;ocrx_word;87f8f8ab-0b0c-46c3-8a67-13323e64df29;af397266-7263-46bc-968f-9153c323df2a;-;88;98;104;200;204
-0;ocrx_word;885eb402-735d-4fdd-96ae-dd781683599f;af397266-7263-46bc-968f-9153c323df2a;Col;99;109;138;192;208
-0;ocrx_word;20dc36c5-47cf-4e46-83d9-850e26ff06b8;af397266-7263-46bc-968f-9153c323df2a;1;100;143;153;193;208
-0;ocrx_word;0dfca725-ab3c-4af7-acb4-c37e2cce2909;2c1bd6de-63d2-4897-aeb4-4c4bea19dbc1;Merged;100;329;398;192;212
-0;ocrx_word;8c0de59a-d728-47da-ba92-03ec626e0318;2c1bd6de-63d2-4897-aeb4-4c4bea19dbc1;Cells;100;403;444;192;208
-0;ocrx_word;eb37a917-6e14-4d60-9a09-a81c6d6d6a47;bc442440-4344-47bb-94af-89e4ea61cd92;Line;100;498;535;193;208
-0;ocrx_word;0de0e673-f70a-4c0a-a9c5-4ace20caf7d2;bc442440-4344-47bb-94af-89e4ea61cd92;3;100;540;551;193;208
-0;ocrx_word;e12b2057-89f1-4d63-ad20-4ca33ebe98c8;bc442440-4344-47bb-94af-89e4ea61cd92;-;99;556;563;200;204
-0;ocrx_word;5f53c113-6ab9-4130-8832-d3f859b422a4;bc442440-4344-47bb-94af-89e4ea61cd92;Col;99;568;596;192;208
-0;ocrx_word;35d19815-0b10-408e-bf59-f951e490de9e;bc442440-4344-47bb-94af-89e4ea61cd92;3;100;602;612;193;208
-0;ocrx_word;36e8bef9-bd56-4f2f-bc4c-1779b9944ce7;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;Line;100;40;76;244;259
-0;ocrx_word;64227af2-a5ca-45cc-9d26-622fa707d719;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;4;100;81;93;244;259
-0;ocrx_word;e20fc9fc-2664-4fe2-9c10-7acaf3b83323;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;-;96;97;105;251;255
-0;ocrx_word;8d94d17a-4cf6-4930-a6fe-d2b8273bd3ef;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;Col;100;109;138;243;259
-0;ocrx_word;a6e92264-d305-468c-b064-0ec56cdf8df2;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;1;100;143;153;244;259
-0;ocrx_word;8b5be284-8122-4ab1-ba7d-7c0e9a0a993c;b49d9668-1b90-429f-8374-14eeddd24199;Line;100;499;535;244;259
-0;ocrx_word;af7ee184-66cc-44d4-84bc-e6508f965ba3;b49d9668-1b90-429f-8374-14eeddd24199;4;100;540;552;244;259
-0;ocrx_word;3808dfa3-ca18-4611-84d9-0f824ac01fb0;b49d9668-1b90-429f-8374-14eeddd24199;-;99;556;564;251;255
-0;ocrx_word;b5ecf045-377d-48d4-b97c-22485482ddb2;b49d9668-1b90-429f-8374-14eeddd24199;Col;100;568;596;243;259
-0;ocrx_word;9007bf10-d36d-4319-b0e8-e12fec61f58a;b49d9668-1b90-429f-8374-14eeddd24199;3;100;602;612;244;259
-0;ocrx_word;3ae4c7ba-905a-48eb-9cb0-a763cbf2dfe3;e8adc959-6816-4899-8bc2-e07d14d8fe80;Line;100;40;76;295;310
-0;ocrx_word;52000a95-0f07-4758-8545-7eaf62b18da8;e8adc959-6816-4899-8bc2-e07d14d8fe80;5;100;82;93;295;310
-0;ocrx_word;d79988f1-5392-43ac-af4c-a749b56828ba;e8adc959-6816-4899-8bc2-e07d14d8fe80;Col;99;109;138;294;310
-0;ocrx_word;50f1f132-9b63-469b-a381-d814bb8764ca;e8adc959-6816-4899-8bc2-e07d14d8fe80;1;100;143;153;295;310
-0;ocrx_word;098b03f3-d9a6-4369-b30a-4121e5361786;d1c0bb6d-7a03-487f-96ed-e7d854126c98;Line;100;280;316;295;310
-0;ocrx_word;85dd10f1-69b8-4451-bec8-e841cf1149f0;d1c0bb6d-7a03-487f-96ed-e7d854126c98;5;100;321;332;295;310
-0;ocrx_word;4f123c5e-2e85-4f27-9cf2-afea76e3ab4d;d1c0bb6d-7a03-487f-96ed-e7d854126c98;Col;100;349;378;294;310
-0;ocrx_word;9f5790f5-f63b-4e21-8ce3-551e3110b190;d1c0bb6d-7a03-487f-96ed-e7d854126c98;2;100;383;393;295;310
-0;ocrx_word;bf452562-8d5f-4326-8ad7-d185595138e9;8de5540e-3e09-40e7-a5d9-de152b433062;Line;100;499;535;295;310
-0;ocrx_word;e62d7690-c0c9-4456-86e5-b78eee33d297;8de5540e-3e09-40e7-a5d9-de152b433062;5;100;541;551;295;310
-0;ocrx_word;58cadea1-fbf2-4dfe-96c6-42ee1f34b321;8de5540e-3e09-40e7-a5d9-de152b433062;-;94;556;563;302;306
-0;ocrx_word;48dfcf15-838c-4282-a208-fc5d4486bd4e;8de5540e-3e09-40e7-a5d9-de152b433062;Col;100;568;596;294;310
-0;ocrx_word;96a626fa-f215-4070-913b-7acb59ef4b4a;8de5540e-3e09-40e7-a5d9-de152b433062;3;100;602;612;295;310
+page;class;id;parent;value;confidence;x1;y1;x2;y2
+0;ocrx_word;88a72bbd-1228-4524-9acd-1c78d457965b;c1a786cc-b3bd-4a74-b286-8307156e136f;Title;100;383;39;423;55
+0;ocrx_word;ecc305af-e32c-4f01-8fd6-d769844add3f;bef0489e-378c-4af6-9804-fd420b65190c;Test;100;965;40;1000;55
+0;ocrx_word;c32bb03e-a29a-4695-aa6b-59bb88bbd25a;bef0489e-378c-4af6-9804-fd420b65190c;1;100;1006;40;1016;55
+0;ocrx_word;ea0e1f37-41e5-4a3e-83ef-edd2e0165e5f;f68dddd3-e0c8-411d-820d-fcfd853d28fe;Test;100;1061;40;1096;55
+0;ocrx_word;04e791eb-62ae-4d68-8ee5-2d672e0c3804;f68dddd3-e0c8-411d-820d-fcfd853d28fe;2;100;1101;40;1112;55
+0;ocrx_word;786208ae-2e98-44e5-a212-730fb60964b0;0712e1d7-2c31-4b62-82f6-441087e63779;Line;100;40;91;76;106
+0;ocrx_word;a809159b-3f1f-4d29-b68d-8ed34e61c31e;0712e1d7-2c31-4b62-82f6-441087e63779;1 -;69;82;91;105;107
+0;ocrx_word;a237beef-d207-4b3d-ad5c-37f1da97e6d0;0712e1d7-2c31-4b62-82f6-441087e63779;-;94;96;98;104;102
+0;ocrx_word;7fd41b4d-dc88-4593-bfdb-84887df80a67;0712e1d7-2c31-4b62-82f6-441087e63779;Col;100;109;90;138;106
+0;ocrx_word;f11bb2bb-b067-4cdd-9913-d8e094016ca3;0712e1d7-2c31-4b62-82f6-441087e63779;1;100;143;91;153;106
+0;ocrx_word;4bf52fb3-9996-41aa-95a0-872178c5e5c8;2ab46d87-2708-4cf3-b69e-9f2763af69a1;Line;100;280;91;316;106
+0;ocrx_word;e2a5eca7-be40-411b-8f5c-8e97c6eae001;2ab46d87-2708-4cf3-b69e-9f2763af69a1;1;100;322;91;332;106
+0;ocrx_word;32a19f1a-a490-4688-b8d5-b5d31c6f1881;2ab46d87-2708-4cf3-b69e-9f2763af69a1;Col;99;349;90;377;106
+0;ocrx_word;0ec66650-6ad5-4240-9983-c829de6dfa55;2ab46d87-2708-4cf3-b69e-9f2763af69a1;2;100;383;91;393;106
+0;ocrx_word;2b0e83f0-e0e2-49e2-92c1-7708973e3312;14c6de15-1642-41f6-a23c-357eaea5718c;Line;100;499;91;535;106
+0;ocrx_word;80743548-4e4e-4ce9-a9bf-306fb94dd079;14c6de15-1642-41f6-a23c-357eaea5718c;1;100;541;91;551;106
+0;ocrx_word;9f1f1f24-ecdb-4163-b986-3d211946a406;14c6de15-1642-41f6-a23c-357eaea5718c;-;97;556;97;563;102
+0;ocrx_word;e574f419-ef0d-4af9-b22e-29e337510b2a;14c6de15-1642-41f6-a23c-357eaea5718c;Col;99;568;90;596;106
+0;ocrx_word;b89c8819-5962-4f71-9b7d-a8cb633f0ea9;14c6de15-1642-41f6-a23c-357eaea5718c;3;100;602;91;612;106
+0;ocrx_word;931dac4a-8623-4ed4-b69d-d560e46b0965;3a1cb207-ccd9-498b-b31d-f71cae319ee1;Test;100;965;91;1001;106
+0;ocrx_word;eddd1221-175d-4acb-9d72-97d1940e9d80;3a1cb207-ccd9-498b-b31d-f71cae319ee1;3;100;1006;91;1016;106
+0;ocrx_word;5df5a361-60d4-4451-9501-8b932e6147b0;65f17b42-1979-445a-8274-db2234589249;Test;100;1061;91;1097;106
+0;ocrx_word;881eaaef-100b-4c2e-a0ad-9f99339e4d39;65f17b42-1979-445a-8274-db2234589249;4;100;1101;91;1113;106
+0;ocrx_word;57a883af-3e0b-4859-95ce-94fa6353fc80;bab0aefa-5ccf-42ea-8700-4390d26c1074;Line;100;40;142;77;157
+0;ocrx_word;f9467369-4c9c-4f2e-b205-d9a5f692ee9a;bab0aefa-5ccf-42ea-8700-4390d26c1074;2;100;81;142;92;157
+0;ocrx_word;e6036250-f943-4b8a-93d3-9dd7a28032bc;bab0aefa-5ccf-42ea-8700-4390d26c1074;-;96;97;149;104;153
+0;ocrx_word;56175999-eb57-4350-86b5-128bc6d167c7;bab0aefa-5ccf-42ea-8700-4390d26c1074;Col;100;109;141;137;157
+0;ocrx_word;7a4757f1-b91b-411c-8630-1bf10db1ac44;bab0aefa-5ccf-42ea-8700-4390d26c1074;1;100;143;142;153;157
+0;ocrx_word;59aa3ef7-d1bc-41ec-a119-ab36f35c9bc1;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;Line;100;499;142;535;157
+0;ocrx_word;ba7809d1-759a-4e0d-8795-ab9523a3724b;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;2;100;541;142;551;157
+0;ocrx_word;e11912eb-f984-434d-bf56-9f1b44c96338;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;-;98;556;149;563;153
+0;ocrx_word;57ec3919-7226-41fd-a53f-0c95722270bd;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;Col;99;568;141;596;157
+0;ocrx_word;3e277cae-536e-4bf0-a2f2-0caa03fd6258;fc5f5124-de4d-4b5c-bd8a-e6da8a9fec65;3;100;602;142;612;157
+0;ocrx_word;793c3b43-171a-4f7e-9aaf-0c7845df2a8b;af397266-7263-46bc-968f-9153c323df2a;Line;100;40;193;76;208
+0;ocrx_word;c33c469a-67ba-4370-b9c6-ddff5b6f8be2;af397266-7263-46bc-968f-9153c323df2a;3;100;81;193;92;208
+0;ocrx_word;87f8f8ab-0b0c-46c3-8a67-13323e64df29;af397266-7263-46bc-968f-9153c323df2a;-;88;98;200;104;204
+0;ocrx_word;885eb402-735d-4fdd-96ae-dd781683599f;af397266-7263-46bc-968f-9153c323df2a;Col;99;109;192;138;208
+0;ocrx_word;20dc36c5-47cf-4e46-83d9-850e26ff06b8;af397266-7263-46bc-968f-9153c323df2a;1;100;143;193;153;208
+0;ocrx_word;0dfca725-ab3c-4af7-acb4-c37e2cce2909;2c1bd6de-63d2-4897-aeb4-4c4bea19dbc1;Merged;100;329;192;398;212
+0;ocrx_word;8c0de59a-d728-47da-ba92-03ec626e0318;2c1bd6de-63d2-4897-aeb4-4c4bea19dbc1;Cells;100;403;192;444;208
+0;ocrx_word;eb37a917-6e14-4d60-9a09-a81c6d6d6a47;bc442440-4344-47bb-94af-89e4ea61cd92;Line;100;498;193;535;208
+0;ocrx_word;0de0e673-f70a-4c0a-a9c5-4ace20caf7d2;bc442440-4344-47bb-94af-89e4ea61cd92;3;100;540;193;551;208
+0;ocrx_word;e12b2057-89f1-4d63-ad20-4ca33ebe98c8;bc442440-4344-47bb-94af-89e4ea61cd92;-;99;556;200;563;204
+0;ocrx_word;5f53c113-6ab9-4130-8832-d3f859b422a4;bc442440-4344-47bb-94af-89e4ea61cd92;Col;99;568;192;596;208
+0;ocrx_word;35d19815-0b10-408e-bf59-f951e490de9e;bc442440-4344-47bb-94af-89e4ea61cd92;3;100;602;193;612;208
+0;ocrx_word;36e8bef9-bd56-4f2f-bc4c-1779b9944ce7;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;Line;100;40;244;76;259
+0;ocrx_word;64227af2-a5ca-45cc-9d26-622fa707d719;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;4;100;81;244;93;259
+0;ocrx_word;e20fc9fc-2664-4fe2-9c10-7acaf3b83323;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;-;96;97;251;105;255
+0;ocrx_word;8d94d17a-4cf6-4930-a6fe-d2b8273bd3ef;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;Col;100;109;243;138;259
+0;ocrx_word;a6e92264-d305-468c-b064-0ec56cdf8df2;23307bb6-e4b2-4c72-85d9-d8578adbb7e7;1;100;143;244;153;259
+0;ocrx_word;8b5be284-8122-4ab1-ba7d-7c0e9a0a993c;b49d9668-1b90-429f-8374-14eeddd24199;Line;100;499;244;535;259
+0;ocrx_word;af7ee184-66cc-44d4-84bc-e6508f965ba3;b49d9668-1b90-429f-8374-14eeddd24199;4;100;540;244;552;259
+0;ocrx_word;3808dfa3-ca18-4611-84d9-0f824ac01fb0;b49d9668-1b90-429f-8374-14eeddd24199;-;99;556;251;564;255
+0;ocrx_word;b5ecf045-377d-48d4-b97c-22485482ddb2;b49d9668-1b90-429f-8374-14eeddd24199;Col;100;568;243;596;259
+0;ocrx_word;9007bf10-d36d-4319-b0e8-e12fec61f58a;b49d9668-1b90-429f-8374-14eeddd24199;3;100;602;244;612;259
+0;ocrx_word;3ae4c7ba-905a-48eb-9cb0-a763cbf2dfe3;e8adc959-6816-4899-8bc2-e07d14d8fe80;Line;100;40;295;76;310
+0;ocrx_word;52000a95-0f07-4758-8545-7eaf62b18da8;e8adc959-6816-4899-8bc2-e07d14d8fe80;5;100;82;295;93;310
+0;ocrx_word;d79988f1-5392-43ac-af4c-a749b56828ba;e8adc959-6816-4899-8bc2-e07d14d8fe80;Col;99;109;294;138;310
+0;ocrx_word;50f1f132-9b63-469b-a381-d814bb8764ca;e8adc959-6816-4899-8bc2-e07d14d8fe80;1;100;143;295;153;310
+0;ocrx_word;098b03f3-d9a6-4369-b30a-4121e5361786;d1c0bb6d-7a03-487f-96ed-e7d854126c98;Line;100;280;295;316;310
+0;ocrx_word;85dd10f1-69b8-4451-bec8-e841cf1149f0;d1c0bb6d-7a03-487f-96ed-e7d854126c98;5;100;321;295;332;310
+0;ocrx_word;4f123c5e-2e85-4f27-9cf2-afea76e3ab4d;d1c0bb6d-7a03-487f-96ed-e7d854126c98;Col;100;349;294;378;310
+0;ocrx_word;9f5790f5-f63b-4e21-8ce3-551e3110b190;d1c0bb6d-7a03-487f-96ed-e7d854126c98;2;100;383;295;393;310
+0;ocrx_word;bf452562-8d5f-4326-8ad7-d185595138e9;8de5540e-3e09-40e7-a5d9-de152b433062;Line;100;499;295;535;310
+0;ocrx_word;e62d7690-c0c9-4456-86e5-b78eee33d297;8de5540e-3e09-40e7-a5d9-de152b433062;5;100;541;295;551;310
+0;ocrx_word;58cadea1-fbf2-4dfe-96c6-42ee1f34b321;8de5540e-3e09-40e7-a5d9-de152b433062;-;94;556;302;563;306
+0;ocrx_word;48dfcf15-838c-4282-a208-fc5d4486bd4e;8de5540e-3e09-40e7-a5d9-de152b433062;Col;100;568;294;596;310
+0;ocrx_word;96a626fa-f215-4070-913b-7acb59ef4b4a;8de5540e-3e09-40e7-a5d9-de152b433062;3;100;602;295;612;310
```

### Comparing `img2table-0.1.2/tests/ocr/aws_textract/test_data/test.png` & `img2table-0.1.3/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/azure/test_azure.py` & `img2table-0.1.3/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-0.1.3/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-page;class;id;parent;value;confidence;x1;x2;y1;y2
-0;ocrx_word;word_1_1;word_1_1;Title;100;383;422;38;56
-0;ocrx_word;word_1_2;word_1_2;Test;99;965;1001;39;57
-0;ocrx_word;word_1_3;word_1_2;1;100;1004;1015;39;57
-0;ocrx_word;word_1_4;word_1_3;Test;99;1061;1096;38;57
-0;ocrx_word;word_1_5;word_1_3;2;100;1100;1111;38;57
-0;ocrx_word;word_1_6;word_1_4;Line;98;38;75;89;108
-0;ocrx_word;word_1_7;word_1_4;1;100;80;91;89;108
-0;ocrx_word;word_1_8;word_1_4;-;99;94;104;89;109
-0;ocrx_word;word_1_9;word_1_4;Col;100;107;137;89;109
-0;ocrx_word;word_1_10;word_1_4;1;99;141;153;88;109
-0;ocrx_word;word_1_11;word_1_5;Line;98;278;315;89;109
-0;ocrx_word;word_1_12;word_1_5;1;100;319;331;89;109
-0;ocrx_word;word_1_13;word_1_5;-;100;335;343;89;109
-0;ocrx_word;word_1_14;word_1_5;Col;100;347;377;88;109
-0;ocrx_word;word_1_15;word_1_5;2;100;381;393;88;109
-0;ocrx_word;word_1_16;word_1_6;Line;99;499;533;89;108
-0;ocrx_word;word_1_17;word_1_6;1;99;538;549;89;108
-0;ocrx_word;word_1_18;word_1_6;-;100;553;562;89;108
-0;ocrx_word;word_1_19;word_1_6;Col;100;566;596;89;108
-0;ocrx_word;word_1_20;word_1_6;3;100;599;611;88;108
-0;ocrx_word;word_1_21;word_1_7;Test;99;964;1000;89;108
-0;ocrx_word;word_1_22;word_1_7;3;100;1003;1014;89;108
-0;ocrx_word;word_1_23;word_1_8;Test;99;1060;1096;89;108
-0;ocrx_word;word_1_24;word_1_8;4;100;1099;1111;89;109
-0;ocrx_word;word_1_25;word_1_9;Line;99;39;74;140;159
-0;ocrx_word;word_1_26;word_1_9;2;99;79;91;141;159
-0;ocrx_word;word_1_27;word_1_9;-;100;94;103;141;159
-0;ocrx_word;word_1_28;word_1_9;Col;100;107;138;141;160
-0;ocrx_word;word_1_29;word_1_9;1;100;142;152;140;160
-0;ocrx_word;word_1_30;word_1_10;Line;99;497;533;140;159
-0;ocrx_word;word_1_31;word_1_10;2;99;537;550;141;159
-0;ocrx_word;word_1_32;word_1_10;-;100;554;563;141;159
-0;ocrx_word;word_1_33;word_1_10;Col;100;566;596;140;159
-0;ocrx_word;word_1_34;word_1_10;3;100;599;610;140;159
-0;ocrx_word;word_1_35;word_1_11;Line;98;38;74;191;210
-0;ocrx_word;word_1_36;word_1_11;3;100;80;91;191;210
-0;ocrx_word;word_1_37;word_1_11;-;100;94;103;191;210
-0;ocrx_word;word_1_38;word_1_11;Col;100;107;139;191;211
-0;ocrx_word;word_1_39;word_1_11;1;100;142;153;190;211
-0;ocrx_word;word_1_40;word_1_12;Merged;99;327;396;191;213
-0;ocrx_word;word_1_41;word_1_12;Cells;100;400;444;190;213
-0;ocrx_word;word_1_42;word_1_13;Line;99;498;533;191;210
-0;ocrx_word;word_1_43;word_1_13;3;100;537;548;191;210
-0;ocrx_word;word_1_44;word_1_13;-;100;553;562;191;210
-0;ocrx_word;word_1_45;word_1_13;Col;100;566;595;191;210
-0;ocrx_word;word_1_46;word_1_13;3;100;598;610;191;210
-0;ocrx_word;word_1_47;word_1_14;Line;98;38;75;242;261
-0;ocrx_word;word_1_48;word_1_14;4;100;79;91;242;262
-0;ocrx_word;word_1_49;word_1_14;-;99;94;104;242;262
-0;ocrx_word;word_1_50;word_1_14;Col;100;107;138;242;262
-0;ocrx_word;word_1_51;word_1_14;1;100;142;153;242;262
-0;ocrx_word;word_1_52;word_1_15;Line;99;497;533;242;262
-0;ocrx_word;word_1_53;word_1_15;4;100;538;549;242;261
-0;ocrx_word;word_1_54;word_1_15;-;100;554;562;242;261
-0;ocrx_word;word_1_55;word_1_15;Col;100;566;596;242;261
-0;ocrx_word;word_1_56;word_1_15;3;100;600;611;242;261
-0;ocrx_word;word_1_57;word_1_16;Line;99;38;74;293;313
-0;ocrx_word;word_1_58;word_1_16;5;98;78;91;293;313
-0;ocrx_word;word_1_59;word_1_16;-;100;95;103;293;313
-0;ocrx_word;word_1_60;word_1_16;Col;100;106;138;293;313
-0;ocrx_word;word_1_61;word_1_16;1;100;141;153;293;313
-0;ocrx_word;word_1_62;word_1_17;Line;98;278;314;293;313
-0;ocrx_word;word_1_63;word_1_17;5;100;319;330;293;313
-0;ocrx_word;word_1_64;word_1_17;-;100;335;343;293;313
-0;ocrx_word;word_1_65;word_1_17;Col;100;347;376;292;313
-0;ocrx_word;word_1_66;word_1_17;2;100;380;392;292;314
-0;ocrx_word;word_1_67;word_1_18;Line;98;497;533;293;313
-0;ocrx_word;word_1_68;word_1_18;5;98;537;550;293;313
-0;ocrx_word;word_1_69;word_1_18;-;100;554;562;293;313
-0;ocrx_word;word_1_70;word_1_18;Col;100;566;596;293;313
-0;ocrx_word;word_1_71;word_1_18;3;100;599;611;293;313
+page;class;id;parent;value;confidence;x1;y1;x2;y2
+0;ocrx_word;word_1_1;word_1_1;Title;100;383;38;422;56
+0;ocrx_word;word_1_2;word_1_2;Test;99;965;39;1001;57
+0;ocrx_word;word_1_3;word_1_2;1;100;1004;39;1015;57
+0;ocrx_word;word_1_4;word_1_3;Test;99;1061;38;1096;57
+0;ocrx_word;word_1_5;word_1_3;2;100;1100;38;1111;57
+0;ocrx_word;word_1_6;word_1_4;Line;98;38;89;75;108
+0;ocrx_word;word_1_7;word_1_4;1;100;80;89;91;108
+0;ocrx_word;word_1_8;word_1_4;-;99;94;89;104;109
+0;ocrx_word;word_1_9;word_1_4;Col;100;107;89;137;109
+0;ocrx_word;word_1_10;word_1_4;1;99;141;88;153;109
+0;ocrx_word;word_1_11;word_1_5;Line;98;278;89;315;109
+0;ocrx_word;word_1_12;word_1_5;1;100;319;89;331;109
+0;ocrx_word;word_1_13;word_1_5;-;100;335;89;343;109
+0;ocrx_word;word_1_14;word_1_5;Col;100;347;88;377;109
+0;ocrx_word;word_1_15;word_1_5;2;100;381;88;393;109
+0;ocrx_word;word_1_16;word_1_6;Line;99;499;89;533;108
+0;ocrx_word;word_1_17;word_1_6;1;99;538;89;549;108
+0;ocrx_word;word_1_18;word_1_6;-;100;553;89;562;108
+0;ocrx_word;word_1_19;word_1_6;Col;100;566;89;596;108
+0;ocrx_word;word_1_20;word_1_6;3;100;599;88;611;108
+0;ocrx_word;word_1_21;word_1_7;Test;99;964;89;1000;108
+0;ocrx_word;word_1_22;word_1_7;3;100;1003;89;1014;108
+0;ocrx_word;word_1_23;word_1_8;Test;99;1060;89;1096;108
+0;ocrx_word;word_1_24;word_1_8;4;100;1099;89;1111;109
+0;ocrx_word;word_1_25;word_1_9;Line;99;39;140;74;159
+0;ocrx_word;word_1_26;word_1_9;2;99;79;141;91;159
+0;ocrx_word;word_1_27;word_1_9;-;100;94;141;103;159
+0;ocrx_word;word_1_28;word_1_9;Col;100;107;141;138;160
+0;ocrx_word;word_1_29;word_1_9;1;100;142;140;152;160
+0;ocrx_word;word_1_30;word_1_10;Line;99;497;140;533;159
+0;ocrx_word;word_1_31;word_1_10;2;99;537;141;550;159
+0;ocrx_word;word_1_32;word_1_10;-;100;554;141;563;159
+0;ocrx_word;word_1_33;word_1_10;Col;100;566;140;596;159
+0;ocrx_word;word_1_34;word_1_10;3;100;599;140;610;159
+0;ocrx_word;word_1_35;word_1_11;Line;98;38;191;74;210
+0;ocrx_word;word_1_36;word_1_11;3;100;80;191;91;210
+0;ocrx_word;word_1_37;word_1_11;-;100;94;191;103;210
+0;ocrx_word;word_1_38;word_1_11;Col;100;107;191;139;211
+0;ocrx_word;word_1_39;word_1_11;1;100;142;190;153;211
+0;ocrx_word;word_1_40;word_1_12;Merged;99;327;191;396;213
+0;ocrx_word;word_1_41;word_1_12;Cells;100;400;190;444;213
+0;ocrx_word;word_1_42;word_1_13;Line;99;498;191;533;210
+0;ocrx_word;word_1_43;word_1_13;3;100;537;191;548;210
+0;ocrx_word;word_1_44;word_1_13;-;100;553;191;562;210
+0;ocrx_word;word_1_45;word_1_13;Col;100;566;191;595;210
+0;ocrx_word;word_1_46;word_1_13;3;100;598;191;610;210
+0;ocrx_word;word_1_47;word_1_14;Line;98;38;242;75;261
+0;ocrx_word;word_1_48;word_1_14;4;100;79;242;91;262
+0;ocrx_word;word_1_49;word_1_14;-;99;94;242;104;262
+0;ocrx_word;word_1_50;word_1_14;Col;100;107;242;138;262
+0;ocrx_word;word_1_51;word_1_14;1;100;142;242;153;262
+0;ocrx_word;word_1_52;word_1_15;Line;99;497;242;533;262
+0;ocrx_word;word_1_53;word_1_15;4;100;538;242;549;261
+0;ocrx_word;word_1_54;word_1_15;-;100;554;242;562;261
+0;ocrx_word;word_1_55;word_1_15;Col;100;566;242;596;261
+0;ocrx_word;word_1_56;word_1_15;3;100;600;242;611;261
+0;ocrx_word;word_1_57;word_1_16;Line;99;38;293;74;313
+0;ocrx_word;word_1_58;word_1_16;5;98;78;293;91;313
+0;ocrx_word;word_1_59;word_1_16;-;100;95;293;103;313
+0;ocrx_word;word_1_60;word_1_16;Col;100;106;293;138;313
+0;ocrx_word;word_1_61;word_1_16;1;100;141;293;153;313
+0;ocrx_word;word_1_62;word_1_17;Line;98;278;293;314;313
+0;ocrx_word;word_1_63;word_1_17;5;100;319;293;330;313
+0;ocrx_word;word_1_64;word_1_17;-;100;335;293;343;313
+0;ocrx_word;word_1_65;word_1_17;Col;100;347;292;376;313
+0;ocrx_word;word_1_66;word_1_17;2;100;380;292;392;314
+0;ocrx_word;word_1_67;word_1_18;Line;98;497;293;533;313
+0;ocrx_word;word_1_68;word_1_18;5;98;537;293;550;313
+0;ocrx_word;word_1_69;word_1_18;-;100;554;293;562;313
+0;ocrx_word;word_1_70;word_1_18;Col;100;566;293;596;313
+0;ocrx_word;word_1_71;word_1_18;3;100;599;293;611;313
```

### Comparing `img2table-0.1.2/tests/ocr/azure/test_data/test.png` & `img2table-0.1.3/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/data/test_data/expected_table.json` & `img2table-0.1.3/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/data/test_data/ocr_df.csv` & `img2table-0.1.3/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/data/test_ocr_data.py` & `img2table-0.1.3/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-0.1.3/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-0.1.3/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-page;class;id;parent;value;confidence;x1;x2;y1;y2
-0;ocrx_word;word_0_0_0_0;line_0_0_0;Line;99;41;74;90;105
+page;class;id;parent;value;confidence;x1;y1;x2;y2
+0;ocrx_word;word_0_0_0_0;line_0_0_0;Line;99;41;90;74;105
 0;ocrx_word;word_0_0_0_1;line_0_0_0;1;98;83;90;90;104
-0;ocrx_word;word_0_0_0_2;line_0_0_0;-;76;97;103;90;104
-0;ocrx_word;word_0_0_0_3;line_0_0_0;Col;98;110;136;90;104
-0;ocrx_word;word_0_0_0_4;line_0_0_0;1;98;142;151;90;104
-0;ocrx_word;word_1_0_0_0;line_1_0_0;Line;99;40;75;142;157
-0;ocrx_word;word_1_0_0_1;line_1_0_0;2;98;83;91;142;157
-0;ocrx_word;word_1_0_0_2;line_1_0_0;-;85;97;104;142;157
-0;ocrx_word;word_1_0_0_3;line_1_0_0;Col;97;110;137;142;157
-0;ocrx_word;word_1_0_0_4;line_1_0_0;1;99;144;152;142;157
-0;ocrx_word;word_2_0_0_0;line_2_0_0;Line;99;41;75;193;207
-0;ocrx_word;word_2_0_0_1;line_2_0_0;3;97;82;91;193;207
-0;ocrx_word;word_2_0_0_2;line_2_0_0;-;79;97;105;193;207
-0;ocrx_word;word_2_0_0_3;line_2_0_0;Col;98;110;137;193;207
-0;ocrx_word;word_2_0_0_4;line_2_0_0;1;99;144;152;193;207
-0;ocrx_word;word_3_0_0_0;line_3_0_0;Line;99;41;75;243;258
-0;ocrx_word;word_3_0_0_1;line_3_0_0;4;98;82;91;243;258
-0;ocrx_word;word_3_0_0_2;line_3_0_0;Col;99;110;137;243;258
-0;ocrx_word;word_3_0_0_3;line_3_0_0;1;98;143;152;243;258
-0;ocrx_word;word_4_0_0_0;line_4_0_0;Line;99;40;75;295;309
-0;ocrx_word;word_4_0_0_1;line_4_0_0;5;98;82;90;295;309
-0;ocrx_word;word_4_0_0_2;line_4_0_0;-;78;97;104;295;309
-0;ocrx_word;word_4_0_0_3;line_4_0_0;Col;97;109;136;295;309
-0;ocrx_word;word_4_0_0_4;line_4_0_0;1;98;142;152;295;309
-0;ocrx_word;word_5_0_0_0;line_5_0_0;Title;99;383;423;39;55
-0;ocrx_word;word_6_0_0_0;line_6_0_0;Line;99;281;316;91;105
-0;ocrx_word;word_6_0_0_1;line_6_0_0;1;98;323;330;91;105
-0;ocrx_word;word_6_0_0_2;line_6_0_0;-;76;337;344;91;105
-0;ocrx_word;word_6_0_0_3;line_6_0_0;Col;91;350;378;91;105
-0;ocrx_word;word_6_0_0_4;line_6_0_0;2;98;383;392;91;105
-0;ocrx_word;word_7_0_0_0;line_7_0_0;Merged;99;329;395;191;211
-0;ocrx_word;word_7_0_0_1;line_7_0_0;Cells;97;402;442;191;209
-0;ocrx_word;word_8_0_0_0;line_8_0_0;Line;98;280;316;295;309
-0;ocrx_word;word_8_0_0_1;line_8_0_0;5;97;323;332;295;309
-0;ocrx_word;word_8_0_0_2;line_8_0_0;-;79;338;345;295;309
-0;ocrx_word;word_8_0_0_3;line_8_0_0;Col;89;349;378;295;309
-0;ocrx_word;word_8_0_0_4;line_8_0_0;2;98;383;392;295;309
-0;ocrx_word;word_9_0_0_0;line_9_0_0;Line;99;499;534;91;105
-0;ocrx_word;word_9_0_0_1;line_9_0_0;1;98;542;549;91;105
-0;ocrx_word;word_9_0_0_2;line_9_0_0;-;75;556;563;91;105
-0;ocrx_word;word_9_0_0_3;line_9_0_0;Col;94;569;596;91;105
-0;ocrx_word;word_9_0_0_4;line_9_0_0;3;98;601;613;91;105
-0;ocrx_word;word_10_0_0_0;line_10_0_0;Line;99;499;534;142;156
-0;ocrx_word;word_10_0_0_1;line_10_0_0;2;98;541;550;142;156
-0;ocrx_word;word_10_0_0_2;line_10_0_0;-;79;556;563;142;156
-0;ocrx_word;word_10_0_0_3;line_10_0_0;Col;90;569;596;142;156
-0;ocrx_word;word_10_0_0_4;line_10_0_0;3;98;603;612;142;156
-0;ocrx_word;word_11_0_0_0;line_11_0_0;Line;99;500;534;193;207
-0;ocrx_word;word_11_0_0_1;line_11_0_0;3;98;541;550;193;207
-0;ocrx_word;word_11_0_0_2;line_11_0_0;-;79;556;564;193;207
-0;ocrx_word;word_11_0_0_3;line_11_0_0;Col;92;569;597;193;207
-0;ocrx_word;word_11_0_0_4;line_11_0_0;3;98;602;612;193;207
-0;ocrx_word;word_12_0_0_0;line_12_0_0;Line;99;499;534;243;258
-0;ocrx_word;word_12_0_0_1;line_12_0_0;4;97;541;550;243;258
-0;ocrx_word;word_12_0_0_2;line_12_0_0;-;70;556;562;243;258
-0;ocrx_word;word_12_0_0_3;line_12_0_0;Col;98;569;595;243;258
-0;ocrx_word;word_12_0_0_4;line_12_0_0;3;98;600;611;244;259
-0;ocrx_word;word_12_1_0_0;line_12_1_0;Line;99;500;534;294;309
-0;ocrx_word;word_12_1_0_1;line_12_1_0;5;97;542;551;294;309
-0;ocrx_word;word_12_1_0_2;line_12_1_0;-;72;556;563;294;309
-0;ocrx_word;word_12_1_0_3;line_12_1_0;Col;97;569;597;294;309
-0;ocrx_word;word_12_1_0_4;line_12_1_0;3;98;601;613;294;309
-0;ocrx_word;word_13_0_0_0;line_13_0_0;Test;98;965;1001;41;54
-0;ocrx_word;word_13_0_0_1;line_13_0_0;1;98;1006;1015;41;54
-0;ocrx_word;word_14_0_0_0;line_14_0_0;Test;99;965;1001;91;106
-0;ocrx_word;word_14_0_0_1;line_14_0_0;3;99;1006;1016;91;106
-0;ocrx_word;word_15_0_0_0;line_15_0_0;Test;98;1061;1095;40;54
-0;ocrx_word;word_15_0_0_1;line_15_0_0;2;98;1101;1110;40;53
-0;ocrx_word;word_16_0_0_0;line_16_0_0;Test;95;1061;1096;91;104
-0;ocrx_word;word_16_0_0_1;line_16_0_0;4;98;1102;1112;91;104
+0;ocrx_word;word_0_0_0_2;line_0_0_0;-;76;97;90;103;104
+0;ocrx_word;word_0_0_0_3;line_0_0_0;Col;98;110;90;136;104
+0;ocrx_word;word_0_0_0_4;line_0_0_0;1;98;142;90;151;104
+0;ocrx_word;word_1_0_0_0;line_1_0_0;Line;99;40;142;75;157
+0;ocrx_word;word_1_0_0_1;line_1_0_0;2;98;83;142;91;157
+0;ocrx_word;word_1_0_0_2;line_1_0_0;-;85;97;142;104;157
+0;ocrx_word;word_1_0_0_3;line_1_0_0;Col;97;110;142;137;157
+0;ocrx_word;word_1_0_0_4;line_1_0_0;1;99;144;142;152;157
+0;ocrx_word;word_2_0_0_0;line_2_0_0;Line;99;41;193;75;207
+0;ocrx_word;word_2_0_0_1;line_2_0_0;3;97;82;193;91;207
+0;ocrx_word;word_2_0_0_2;line_2_0_0;-;79;97;193;105;207
+0;ocrx_word;word_2_0_0_3;line_2_0_0;Col;98;110;193;137;207
+0;ocrx_word;word_2_0_0_4;line_2_0_0;1;99;144;193;152;207
+0;ocrx_word;word_3_0_0_0;line_3_0_0;Line;99;41;243;75;258
+0;ocrx_word;word_3_0_0_1;line_3_0_0;4;98;82;243;91;258
+0;ocrx_word;word_3_0_0_2;line_3_0_0;Col;99;110;243;137;258
+0;ocrx_word;word_3_0_0_3;line_3_0_0;1;98;143;243;152;258
+0;ocrx_word;word_4_0_0_0;line_4_0_0;Line;99;40;295;75;309
+0;ocrx_word;word_4_0_0_1;line_4_0_0;5;98;82;295;90;309
+0;ocrx_word;word_4_0_0_2;line_4_0_0;-;78;97;295;104;309
+0;ocrx_word;word_4_0_0_3;line_4_0_0;Col;97;109;295;136;309
+0;ocrx_word;word_4_0_0_4;line_4_0_0;1;98;142;295;152;309
+0;ocrx_word;word_5_0_0_0;line_5_0_0;Title;99;383;39;423;55
+0;ocrx_word;word_6_0_0_0;line_6_0_0;Line;99;281;91;316;105
+0;ocrx_word;word_6_0_0_1;line_6_0_0;1;98;323;91;330;105
+0;ocrx_word;word_6_0_0_2;line_6_0_0;-;76;337;91;344;105
+0;ocrx_word;word_6_0_0_3;line_6_0_0;Col;91;350;91;378;105
+0;ocrx_word;word_6_0_0_4;line_6_0_0;2;98;383;91;392;105
+0;ocrx_word;word_7_0_0_0;line_7_0_0;Merged;99;329;191;395;211
+0;ocrx_word;word_7_0_0_1;line_7_0_0;Cells;97;402;191;442;209
+0;ocrx_word;word_8_0_0_0;line_8_0_0;Line;98;280;295;316;309
+0;ocrx_word;word_8_0_0_1;line_8_0_0;5;97;323;295;332;309
+0;ocrx_word;word_8_0_0_2;line_8_0_0;-;79;338;295;345;309
+0;ocrx_word;word_8_0_0_3;line_8_0_0;Col;89;349;295;378;309
+0;ocrx_word;word_8_0_0_4;line_8_0_0;2;98;383;295;392;309
+0;ocrx_word;word_9_0_0_0;line_9_0_0;Line;99;499;91;534;105
+0;ocrx_word;word_9_0_0_1;line_9_0_0;1;98;542;91;549;105
+0;ocrx_word;word_9_0_0_2;line_9_0_0;-;75;556;91;563;105
+0;ocrx_word;word_9_0_0_3;line_9_0_0;Col;94;569;91;596;105
+0;ocrx_word;word_9_0_0_4;line_9_0_0;3;98;601;91;613;105
+0;ocrx_word;word_10_0_0_0;line_10_0_0;Line;99;499;142;534;156
+0;ocrx_word;word_10_0_0_1;line_10_0_0;2;98;541;142;550;156
+0;ocrx_word;word_10_0_0_2;line_10_0_0;-;79;556;142;563;156
+0;ocrx_word;word_10_0_0_3;line_10_0_0;Col;90;569;142;596;156
+0;ocrx_word;word_10_0_0_4;line_10_0_0;3;98;603;142;612;156
+0;ocrx_word;word_11_0_0_0;line_11_0_0;Line;99;500;193;534;207
+0;ocrx_word;word_11_0_0_1;line_11_0_0;3;98;541;193;550;207
+0;ocrx_word;word_11_0_0_2;line_11_0_0;-;79;556;193;564;207
+0;ocrx_word;word_11_0_0_3;line_11_0_0;Col;92;569;193;597;207
+0;ocrx_word;word_11_0_0_4;line_11_0_0;3;98;602;193;612;207
+0;ocrx_word;word_12_0_0_0;line_12_0_0;Line;99;499;243;534;258
+0;ocrx_word;word_12_0_0_1;line_12_0_0;4;97;541;243;550;258
+0;ocrx_word;word_12_0_0_2;line_12_0_0;-;70;556;243;562;258
+0;ocrx_word;word_12_0_0_3;line_12_0_0;Col;98;569;243;595;258
+0;ocrx_word;word_12_0_0_4;line_12_0_0;3;98;600;244;611;259
+0;ocrx_word;word_12_1_0_0;line_12_1_0;Line;99;500;294;534;309
+0;ocrx_word;word_12_1_0_1;line_12_1_0;5;97;542;294;551;309
+0;ocrx_word;word_12_1_0_2;line_12_1_0;-;72;556;294;563;309
+0;ocrx_word;word_12_1_0_3;line_12_1_0;Col;97;569;294;597;309
+0;ocrx_word;word_12_1_0_4;line_12_1_0;3;98;601;294;613;309
+0;ocrx_word;word_13_0_0_0;line_13_0_0;Test;98;965;41;1001;54
+0;ocrx_word;word_13_0_0_1;line_13_0_0;1;98;1006;41;1015;54
+0;ocrx_word;word_14_0_0_0;line_14_0_0;Test;99;965;91;1001;106
+0;ocrx_word;word_14_0_0_1;line_14_0_0;3;99;1006;91;1016;106
+0;ocrx_word;word_15_0_0_0;line_15_0_0;Test;98;1061;40;1095;54
+0;ocrx_word;word_15_0_0_1;line_15_0_0;2;98;1101;40;1110;53
+0;ocrx_word;word_16_0_0_0;line_16_0_0;Test;95;1061;91;1096;104
+0;ocrx_word;word_16_0_0_1;line_16_0_0;4;98;1102;91;1112;104
```

### Comparing `img2table-0.1.2/tests/ocr/google_vision/test_data/test.png` & `img2table-0.1.3/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/google_vision/test_google_vision.py` & `img2table-0.1.3/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/paddle/test_data/hocr.json` & `img2table-0.1.3/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-0.1.3/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/paddle/test_data/test.png` & `img2table-0.1.3/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/paddle/test_paddle.py` & `img2table-0.1.3/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/pdf/test_data/content.json` & `img2table-0.1.3/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-0.1.3/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/pdf/test_data/test.pdf` & `img2table-0.1.3/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-0.1.3/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-0.1.3/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/tesseract/test_data/test.png` & `img2table-0.1.3/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/ocr/tesseract/test_tesseract.py` & `img2table-0.1.3/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/image/test_data/blank.png` & `img2table-0.1.3/tests/tables/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/image/test_data/ocr.csv` & `img2table-0.1.3/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/image/test_data/test.png` & `img2table-0.1.3/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/image/test_image.py` & `img2table-0.1.3/tests/tables/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/image/test_metrics.py` & `img2table-0.1.3/tests/tables/image/test_metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/objects/test_data/expected_tables.json` & `img2table-0.1.3/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/objects/test_data/ocr.csv` & `img2table-0.1.3/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/objects/test_data/tables.json` & `img2table-0.1.3/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/objects/test_extraction.py` & `img2table-0.1.3/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/objects/test_line.py` & `img2table-0.1.3/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/objects/test_row.py` & `img2table-0.1.3/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/objects/test_table.py` & `img2table-0.1.3/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_data/contours.json` & `img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py` & `img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json` & `img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png` & `img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-0.1.3/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json` & `img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/lines/test_lines.py` & `img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json` & `img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/test_data/test.png` & `img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/common/test_common.py` & `img2table-0.1.3/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/common/test_data/test.jpg` & `img2table-0.1.3/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-0.1.3/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/text/test_data/ocr.csv` & `img2table-0.1.3/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/text/test_data/table.json` & `img2table-0.1.3/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/text/test_data/test.jpg` & `img2table-0.1.3/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.2/tests/tables/processing/text/test_titles.py` & `img2table-0.1.3/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

