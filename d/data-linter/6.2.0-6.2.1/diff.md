# Comparing `tmp/data_linter-6.2.0.tar.gz` & `tmp/data_linter-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_linter-6.2.0.tar", max compression
+gzip compressed data, was "data_linter-6.2.1.tar", max compression
```

## Comparing `data_linter-6.2.0.tar` & `data_linter-6.2.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    10520 2023-01-10 14:16:35.147454 data_linter-6.2.0/README.md
--rw-r--r--   0        0        0       22 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/__init__.py
--rw-r--r--   0        0        0      490 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/command_line.py
--rw-r--r--   0        0        0      137 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/constants.py
--rw-r--r--   0        0        0     1881 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/iam.py
--rw-r--r--   0        0        0     5474 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/log_explorer_utils.py
--rw-r--r--   0        0        0     3206 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/logging_functions.py
--rw-r--r--   0        0        0    25362 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/schemas/config-schema.json
--rw-r--r--   0        0        0     7623 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/utils.py
--rw-r--r--   0        0        0    26887 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/validation.py
--rw-r--r--   0        0        0      109 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/validators/__init__.py
--rw-r--r--   0        0        0     5745 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/validators/base.py
--rw-r--r--   0        0        0    16469 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/validators/pandas_validator.py
--rw-r--r--   0        0        0     2634 2023-01-10 14:16:35.147454 data_linter-6.2.0/data_linter/validators/parquet_validator.py
--rw-r--r--   0        0        0     1195 2023-01-10 14:16:35.151454 data_linter-6.2.0/pyproject.toml
--rw-r--r--   0        0        0    11893 1970-01-01 00:00:00.000000 data_linter-6.2.0/setup.py
--rw-r--r--   0        0        0    11559 1970-01-01 00:00:00.000000 data_linter-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10520 2023-05-10 09:37:19.258138 data_linter-6.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/__init__.py
+-rw-r--r--   0        0        0      490 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/command_line.py
+-rw-r--r--   0        0        0      137 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/constants.py
+-rw-r--r--   0        0        0     1881 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/iam.py
+-rw-r--r--   0        0        0     5474 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/log_explorer_utils.py
+-rw-r--r--   0        0        0     3206 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/logging_functions.py
+-rw-r--r--   0        0        0    25362 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/schemas/config-schema.json
+-rw-r--r--   0        0        0     7623 2023-05-10 09:37:19.258138 data_linter-6.2.1/data_linter/utils.py
+-rw-r--r--   0        0        0    26887 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validation.py
+-rw-r--r--   0        0        0      109 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validators/__init__.py
+-rw-r--r--   0        0        0     5745 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validators/base.py
+-rw-r--r--   0        0        0    16469 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validators/pandas_validator.py
+-rw-r--r--   0        0        0     3316 2023-05-10 09:37:19.262138 data_linter-6.2.1/data_linter/validators/parquet_validator.py
+-rw-r--r--   0        0        0     1195 2023-05-10 09:37:19.262138 data_linter-6.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11559 1970-01-01 00:00:00.000000 data_linter-6.2.1/PKG-INFO
```

### Comparing `data_linter-6.2.0/README.md` & `data_linter-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/iam.py` & `data_linter-6.2.1/data_linter/iam.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/log_explorer_utils.py` & `data_linter-6.2.1/data_linter/log_explorer_utils.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/logging_functions.py` & `data_linter-6.2.1/data_linter/logging_functions.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/schemas/config-schema.json` & `data_linter-6.2.1/data_linter/schemas/config-schema.json`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/utils.py` & `data_linter-6.2.1/data_linter/utils.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/validation.py` & `data_linter-6.2.1/data_linter/validation.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/validators/base.py` & `data_linter-6.2.1/data_linter/validators/base.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/validators/pandas_validator.py` & `data_linter-6.2.1/data_linter/validators/pandas_validator.py`

 * *Files identical despite different names*

### Comparing `data_linter-6.2.0/data_linter/validators/parquet_validator.py` & `data_linter-6.2.1/data_linter/validators/parquet_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,57 @@
 import logging
+import os
+from typing import Union
 
-
-from data_linter.validators.base import (
-    BaseTableValidator,
-)
+import pyarrow.parquet as pq
+from dataengineeringutils3.s3 import s3_path_to_bucket_key
 from mojap_metadata import Metadata
 from mojap_metadata.converters.arrow_converter import ArrowConverter
-from typing import Union
-import pyarrow.parquet as pq
+from pyarrow import Schema
+from pyarrow.fs import S3FileSystem
 
+from data_linter.validators.base import BaseTableValidator
 
 log = logging.getLogger("root")
 default_date_format = "%Y-%m-%d"
 default_datetime_format = "%Y-%m-%d %H:%M:%S"
+aws_default_region = os.getenv(
+    "AWS_DEFAULT_REGION", os.getenv("AWS_REGION", "eu-west-1")
+)
 
 
 class ParquetValidator(BaseTableValidator):
     """
     Validator for checking that a parquet file's schema matches a given Metadata.
     For validating the data itself, use the Pandas validator.
     """
+
     def __init__(
         self,
         filepath: str,
         table_params: dict,
         metadata: Union[dict, str, Metadata],
-        **kwargs
+        **kwargs,
     ):
         super().__init__(filepath, table_params, metadata)
 
+    @staticmethod
+    def _read_schema(filepath: str) -> Schema:
+        if filepath.startswith("s3://"):
+            s3fs = S3FileSystem(region=aws_default_region)
+            b, k = s3_path_to_bucket_key(filepath)
+            pa_pth = os.path.join(b, k)
+            with s3fs.open_input_file(pa_pth) as file:
+                schema = pq.read_schema(file).remove_metadata()
+        else:
+            schema = pq.read_schema(filepath).remove_metadata()
+        return schema
+
     def read_data_and_validate(self):
-        table_arrow_schema = pq.read_schema(self.filepath).remove_metadata()
+        table_arrow_schema = self._read_schema(self.filepath)
         ac = ArrowConverter()
         metadata_arrow_schema = ac.generate_from_meta(self.metadata).remove_metadata()
         metas_match = table_arrow_schema.equals(metadata_arrow_schema)
 
         cols_in_meta_not_in_file = list(
             set([c.name for c in metadata_arrow_schema])
             - set([c.name for c in table_arrow_schema])
```

### Comparing `data_linter-6.2.0/pyproject.toml` & `data_linter-6.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data_linter"
-version = "6.2.0"
+version = "6.2.1"
 description = "data linter"
 authors = ["Thomas Hirsch <thomas.hirsch@digital.justice.gov.uk>",
            "George Kelly <george.kelly@digital.justice.gov.uk>",
            "Tapan Perkins <tapan.perkins@digital.justice.gov.uk>",
            "Karik Isichei <karik.isichei@digital.justice.gov.uk>",
            "Stephen Bias <stephen.bias@digital.justice.gov.uk>"]
```

### Comparing `data_linter-6.2.0/setup.py` & `data_linter-6.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,283 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: data-linter
+Version: 6.2.1
+Summary: data linter
+Home-page: https://github.com/moj-analytical-services/data_linter
+Author: Thomas Hirsch
+Author-email: thomas.hirsch@digital.justice.gov.uk
+Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: frictionless
+Provides-Extra: ge
+Requires-Dist: PyYAML (>=5.4.1)
+Requires-Dist: arrow-pd-parser (>=1.3.0,<2)
+Requires-Dist: awswrangler (>=2.3.0,<3.0.0)
+Requires-Dist: boto3 (>=1.14.7,<2.0.0)
+Requires-Dist: dataengineeringutils3 (>=1.0.1,<2.0.0)
+Requires-Dist: iam_builder (>=4.1.0,<5.0.0)
+Requires-Dist: jsonschema (>=4.10.0,<5.0.0)
+Requires-Dist: mojap-metadata[arrow] (>=1.10.0,<2.0.0)
+Requires-Dist: pandas (>=1.2,<2.0)
+Requires-Dist: toml (>=0.10,<0.11)
+Project-URL: Repository, https://github.com/moj-analytical-services/data_linter
+Description-Content-Type: text/markdown
 
-packages = \
-['data_linter', 'data_linter.validators']
+# Data Linter
 
-package_data = \
-{'': ['*'], 'data_linter': ['schemas/*']}
+A python package to to allow automatic validation of data as part of a Data Engineering pipeline. It is designed to read in and validate tabular data against a given schema for the data. The schemas provided adhere to [our metadata schemas standards](https://github.com/moj-analytical-services/mojap-metadata/) for data. This package can also be used to manage movement of data from a landing area (s3 or locally) to a new location based on the result of the validation.
 
-install_requires = \
-['PyYAML>=5.4.1',
- 'arrow-pd-parser>=1.3.0,<2',
- 'awswrangler>=2.3.0,<3.0.0',
- 'boto3>=1.14.7,<2.0.0',
- 'dataengineeringutils3>=1.0.1,<2.0.0',
- 'iam_builder>=4.1.0,<5.0.0',
- 'jsonschema>=4.10.0,<5.0.0',
- 'mojap-metadata[arrow]>=1.10.0,<2.0.0',
- 'pandas>=1.2,<2.0',
- 'toml>=0.10,<0.11']
-
-entry_points = \
-{'console_scripts': ['data_linter = data_linter.command_line:main']}
-
-setup_kwargs = {
-    'name': 'data-linter',
-    'version': '6.2.0',
-    'description': 'data linter',
-    'long_description': '# Data Linter\n\nA python package to to allow automatic validation of data as part of a Data Engineering pipeline. It is designed to read in and validate tabular data against a given schema for the data. The schemas provided adhere to [our metadata schemas standards](https://github.com/moj-analytical-services/mojap-metadata/) for data. This package can also be used to manage movement of data from a landing area (s3 or locally) to a new location based on the result of the validation.\n\nThis package uses own lightweight pandas dataframe operations to run simple validation tests on the columns based on the datatype and additional tags in the metadata. Utilises [mojap-arrow-pd-parser](https://github.com/moj-analytical-services/mojap-arrow-pd-parser) for reading data.\n\n## Installation\n\n```bash\npip install data_linter\n```\n\n## Usage\n\nThis package takes a `yaml` based config file written by the user (see example below), and validates data in the specified s3 folder path against specified metadata. If the data conforms to the metadata, it is moved to the specified s3 folder path for the next step in the pipeline (note can also provide local paths). Any failed checks are passed to a separate location for testing. The package also generates logs to allow you to explore issues in more detail.\n\n### Simple Use\n\nTo run the validation, at most simple you can use the following:\n\n**In Python:**\n\n```python\nfrom data_linter.validation import run_validation\n\nconfig_path = "config.yaml"\n\nrun_validation(config_path)\n```\n\n**Via command line:**\n\n```bash\ndata_linter --config_path config.yaml\n```\n\n### Example config file\n\n```yaml\nland-base-path: s3://testing-bucket/land/  # Where to get the data from\nfail-base-path: s3://testing-bucket/fail/  # Where to write the data if failed\npass-base-path: s3://testing-bucket/pass/  # Where to write the data if passed\nlog-base-path: s3://testing-bucket/logs/  # Where to write logs\ncompress-data: true  # Compress data when moving elsewhere (only applicable from CSV/JSON)\nremove-tables-on-pass: true  # Delete the tables in land if validation passes\nall-must-pass: true  # Only move data if all tables have passed\nfail-unknown-files:\n    exceptions:\n        - additional_file.txt\n        - another_additional_file.txt\n\nvalidator-engine-params:\n    log_verbosity: 2 # how many samples of incorrect data to include in logs, 0 means all. Pandas validator only. \n\n# Tables to validate\ntables:\n    table1:\n        required: true  # Does the table have to exist\n        pattern: null  # Assumes file is called table1 (same as key)\n        metadata: meta_data/table1.json # local path to metadata\n        log_verbosity: 5 # overrides the validator-engine-params log verbosity for this table only\n        allow-missing-cols: False # allows there to be data in the metadata but not actual data\n\n    table2:\n        required: true\n        pattern: ^table2\n        metadata: meta_data/table2.json\n        row-limit: 10000 # for big tables - only take the first x rows\n        allow-unexpected-data: True # allows there to be columns present in the data but not the metadata\n```\n**unexpected data and missing columns**\nTo allow flexibilty in what is validated in the data, the parameters `allow-unexpected-data` and `allow-missing-cols` has been added. These can be described neatly in one diagram:\n\n![](images/data_misalignment.png)\n\nYou can also run the validator as part of a python script, where you might want to dynamically generate your config:\n\n```python\nfrom data_linter.validation import run_validation\n\nbase_config = {\n    "land-base-path": "s3://my-bucket/land/",\n    "fail-base-path": "s3://my-bucket/fail/",\n    "pass-base-path": "s3://my-bucket/pass/",\n    "log-base-path": "s3://my-bucket/log/",\n    "compress-data": False,\n    "remove-tables-on-pass": False,\n    "all-must-pass": False,\n    "tables": {}\n}\n\ndef get_table_config(table_name):\n    d = {\n        "required": False,\n        "expect-header": True,\n        "metadata": f"metadata/{table_name}.json",\n        "pattern": r"^{}\\.jsonl$".format(table_name),\n        "headers-ignore-case": True,\n    }\n    return d\n\nfor table in ["table1", "table2"]:\n    base_config["tables"][table_name] = get_table_config(table_name)\n\nrun_validation(base_config) # Then watch that log go...\n```\n\n### Validating a single file\n\n> Without all the bells and whistles\n\nIf you do not need `data_linter` to match files to a specified config, log the process and then move data around based on the outcome of the validation you can just use the validators themselves:\n\n```python\n# Example using simple pandas validatior (without added data_linter features)\nimport json\nfrom data_linter.validators import PandasValidator\n\nfilepath = "tests/data/end_to_end1/land/table1.csv"\ntable_params = {\n    "expect-header": True\n}\nwith open("tests/data/end_to_end1/meta_data/table1.json") as f:\n    metadata = json.load(f)\n\npv = PandasValidator(filepath, table_params, metadata)\npv.read_data_and_validate()\n\npv.valid  # True (data in table1.csv is valid against metadata)\npv.response.get_result()  # Returns dict of all tests ran against data\n\n# The response object of the PandasValidator in itself, and has it\'s own functions\npv.response.get_names_of_column_failures()  #\xa0[], i.e. no cols failed\n```\n\n### Parallel Running\n\nData Linter can also work in parallel to trigger multiple validations at once (only supports use of S3 atm). An example below:\n\nIn this scenario we use the parallisation process to init the process split the job into 4 validators and then run the closedown.\n\n- **The init stage** splits the config into 4 chunks, based on the file size of the data sitting in the specified land path. It split configs are written to a temporary path in S3 for each validator to pick up and run in parallel.\n- **The validator stage** can be ran in parallel (for simplicity they are run sequentially in the example below). Each validator will take the config in the temp folder path and process the files given in that subsetting config.\n- **The closedown stage** will take all the logs all validator runs, conbine them then move the data based on the validators results. It will then finally clean up the temp folder.\n\n```python\n# Simple example running DL with multiple validators (in this case 4)\n# [init] -> [validator]x4 -> [closedown]\nimport yaml\nfrom data_linter import validation\nfrom dataengineeringutils3.s3 import get_filepaths_from_s3_folder\n\n\nsimple_yaml_config = """\nland-base-path: s3://land/\nfail-base-path: s3://fail/\npass-base-path: s3://pass/\nlog-base-path: s3://log/\n\ncompress-data: false\nremove-tables-on-pass: true\nall-must-pass: true\n\n# Tables to validate\ntables:\n  table1:\n    required: true\n    metadata: tests/data/end_to_end1/meta_data/table1.json\n    expect-header: true\n\n  table2:\n    required: true\n    pattern: ^table2\n    metadata: tests/data/end_to_end1/meta_data/table2.json\n"""\n\ntest_folder = "tests/data/end_to_end1/land/"\nconfig = yaml.safe_load(simple_yaml_config)\n\n# Init stage\nvalidation.para_run_init(4, config)\n\n# Validation stage (although ran sequentially this can be ran in parallel)\nfor i in range(4):\n    validation.para_run_validation(i, config)\n\n# Closedown stage\nvalidation.para_collect_all_status(config)\nvalidation.para_collect_all_logs(config)\n```\n\n> There are more parallelisation examples, which can be found in the [test_simple_examples.py test module](tests/test_simple_examples.py)\n\n## Validators\n\n### Pandas\n\nThis is the default validator used by data_linter as of the version 5 release.\n\n#### Dealing with timestamps and dates\n\nTimestamps are always a pain to deal with especially when using different file types. The Pandas Validator has tried to keep true to the file types based on the tests it runs.\n\nIf the file type stores date/timestamp information as a string (i.e. CSV and JSONL) then the pandas Validator will read in the timestamp / date columns as strings. It will then apply validation tests against those columns checking if the string representation of the dates in the data is a valid date. For timestamp and date types these tests assume ISO standard string representation `%Y-%m-%d %H:%M:%S` and `%Y-%m-%d`. If your timestamp/date types are comming in as strings that do not conform to the ISO standard format then you can provide you column in the metadata with a `datetime_format` property that specifies the exected format e.g.\n\n```json\n...\n"columns": [\n    {\n        "name": "date_in_uk",\n        "type": "date64",\n        "datetime_format": "%d/%m/%Y"\n    },\n...\n```\n\nOften you might recieve data that is exported from a system that might encode your timestamp as a date but is written to a format that encodes the data as a timestamp. In this scenario you would expect your dates (in a str timestamp format) to always have a time component of `00:00:00`. You can also use data_linter to validate this by specifing the datetime_format of your column as the expected timestamp in format but still specify that the data type is a date e.g.\n\n```json\n...\n"columns": [\n    {\n        "name": "date_in_uk",\n        "type": "date64",\n        "datetime_format": "%d/%m/%Y 00:00:00"\n    },\n...\n```\n\nIn the above data_linter will attempt to fist parse the column with the specified `datetime_format` and then as the column type is date it will check that it it truely a date (and not have a time component).\n\nIf the file_format is `parquet` then timestamps are encoded in the filetype and there are just read in as is. Currently data_linter doesn\'t support minimum and maximum tests for timestamps/dates and also does not currently have tests for time types. \n\n## Process Diagram\n\nHow logic works\n\n![](images/data_linter_process.png)\n\n## How to update\n\nWe have tests that run on the current state of the `poetry.lock` file (i.e. the current dependencies). We also run tests based on the most up to date dependencies allowed in `pyproject.toml`. This allows us to see if there will be any issues when updating dependences. These can be run locally in the `tests` folder.\n\nWhen updating this package, make sure to change the version number in `pyproject.toml` and describe the change in CHANGELOG.md.\n\nIf you have changed any dependencies in `pyproject.toml`, run `poetry update` to update `poetry.lock`.\n\nOnce you have created a release in GitHub, to publish the latest version to PyPI, run:\n\n```bash\npoetry build\npoetry publish -u <username>\n```\n\nHere, you should substitute <username> for your PyPI username. In order to publish to PyPI, you must be an owner of the project.\n',
-    'author': 'Thomas Hirsch',
-    'author_email': 'thomas.hirsch@digital.justice.gov.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/moj-analytical-services/data_linter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
+This package uses own lightweight pandas dataframe operations to run simple validation tests on the columns based on the datatype and additional tags in the metadata. Utilises [mojap-arrow-pd-parser](https://github.com/moj-analytical-services/mojap-arrow-pd-parser) for reading data.
+
+## Installation
+
+```bash
+pip install data_linter
+```
+
+## Usage
+
+This package takes a `yaml` based config file written by the user (see example below), and validates data in the specified s3 folder path against specified metadata. If the data conforms to the metadata, it is moved to the specified s3 folder path for the next step in the pipeline (note can also provide local paths). Any failed checks are passed to a separate location for testing. The package also generates logs to allow you to explore issues in more detail.
+
+### Simple Use
+
+To run the validation, at most simple you can use the following:
+
+**In Python:**
+
+```python
+from data_linter.validation import run_validation
+
+config_path = "config.yaml"
+
+run_validation(config_path)
+```
+
+**Via command line:**
+
+```bash
+data_linter --config_path config.yaml
+```
+
+### Example config file
+
+```yaml
+land-base-path: s3://testing-bucket/land/  # Where to get the data from
+fail-base-path: s3://testing-bucket/fail/  # Where to write the data if failed
+pass-base-path: s3://testing-bucket/pass/  # Where to write the data if passed
+log-base-path: s3://testing-bucket/logs/  # Where to write logs
+compress-data: true  # Compress data when moving elsewhere (only applicable from CSV/JSON)
+remove-tables-on-pass: true  # Delete the tables in land if validation passes
+all-must-pass: true  # Only move data if all tables have passed
+fail-unknown-files:
+    exceptions:
+        - additional_file.txt
+        - another_additional_file.txt
+
+validator-engine-params:
+    log_verbosity: 2 # how many samples of incorrect data to include in logs, 0 means all. Pandas validator only. 
+
+# Tables to validate
+tables:
+    table1:
+        required: true  # Does the table have to exist
+        pattern: null  # Assumes file is called table1 (same as key)
+        metadata: meta_data/table1.json # local path to metadata
+        log_verbosity: 5 # overrides the validator-engine-params log verbosity for this table only
+        allow-missing-cols: False # allows there to be data in the metadata but not actual data
+
+    table2:
+        required: true
+        pattern: ^table2
+        metadata: meta_data/table2.json
+        row-limit: 10000 # for big tables - only take the first x rows
+        allow-unexpected-data: True # allows there to be columns present in the data but not the metadata
+```
+**unexpected data and missing columns**
+To allow flexibilty in what is validated in the data, the parameters `allow-unexpected-data` and `allow-missing-cols` has been added. These can be described neatly in one diagram:
+
+![](images/data_misalignment.png)
+
+You can also run the validator as part of a python script, where you might want to dynamically generate your config:
+
+```python
+from data_linter.validation import run_validation
+
+base_config = {
+    "land-base-path": "s3://my-bucket/land/",
+    "fail-base-path": "s3://my-bucket/fail/",
+    "pass-base-path": "s3://my-bucket/pass/",
+    "log-base-path": "s3://my-bucket/log/",
+    "compress-data": False,
+    "remove-tables-on-pass": False,
+    "all-must-pass": False,
+    "tables": {}
 }
 
+def get_table_config(table_name):
+    d = {
+        "required": False,
+        "expect-header": True,
+        "metadata": f"metadata/{table_name}.json",
+        "pattern": r"^{}\.jsonl$".format(table_name),
+        "headers-ignore-case": True,
+    }
+    return d
+
+for table in ["table1", "table2"]:
+    base_config["tables"][table_name] = get_table_config(table_name)
+
+run_validation(base_config) # Then watch that log go...
+```
+
+### Validating a single file
+
+> Without all the bells and whistles
+
+If you do not need `data_linter` to match files to a specified config, log the process and then move data around based on the outcome of the validation you can just use the validators themselves:
+
+```python
+# Example using simple pandas validatior (without added data_linter features)
+import json
+from data_linter.validators import PandasValidator
+
+filepath = "tests/data/end_to_end1/land/table1.csv"
+table_params = {
+    "expect-header": True
+}
+with open("tests/data/end_to_end1/meta_data/table1.json") as f:
+    metadata = json.load(f)
+
+pv = PandasValidator(filepath, table_params, metadata)
+pv.read_data_and_validate()
+
+pv.valid  # True (data in table1.csv is valid against metadata)
+pv.response.get_result()  # Returns dict of all tests ran against data
+
+# The response object of the PandasValidator in itself, and has it's own functions
+pv.response.get_names_of_column_failures()  # [], i.e. no cols failed
+```
+
+### Parallel Running
+
+Data Linter can also work in parallel to trigger multiple validations at once (only supports use of S3 atm). An example below:
+
+In this scenario we use the parallisation process to init the process split the job into 4 validators and then run the closedown.
+
+- **The init stage** splits the config into 4 chunks, based on the file size of the data sitting in the specified land path. It split configs are written to a temporary path in S3 for each validator to pick up and run in parallel.
+- **The validator stage** can be ran in parallel (for simplicity they are run sequentially in the example below). Each validator will take the config in the temp folder path and process the files given in that subsetting config.
+- **The closedown stage** will take all the logs all validator runs, conbine them then move the data based on the validators results. It will then finally clean up the temp folder.
+
+```python
+# Simple example running DL with multiple validators (in this case 4)
+# [init] -> [validator]x4 -> [closedown]
+import yaml
+from data_linter import validation
+from dataengineeringutils3.s3 import get_filepaths_from_s3_folder
+
+
+simple_yaml_config = """
+land-base-path: s3://land/
+fail-base-path: s3://fail/
+pass-base-path: s3://pass/
+log-base-path: s3://log/
+
+compress-data: false
+remove-tables-on-pass: true
+all-must-pass: true
+
+# Tables to validate
+tables:
+  table1:
+    required: true
+    metadata: tests/data/end_to_end1/meta_data/table1.json
+    expect-header: true
+
+  table2:
+    required: true
+    pattern: ^table2
+    metadata: tests/data/end_to_end1/meta_data/table2.json
+"""
+
+test_folder = "tests/data/end_to_end1/land/"
+config = yaml.safe_load(simple_yaml_config)
+
+# Init stage
+validation.para_run_init(4, config)
+
+# Validation stage (although ran sequentially this can be ran in parallel)
+for i in range(4):
+    validation.para_run_validation(i, config)
+
+# Closedown stage
+validation.para_collect_all_status(config)
+validation.para_collect_all_logs(config)
+```
+
+> There are more parallelisation examples, which can be found in the [test_simple_examples.py test module](tests/test_simple_examples.py)
+
+## Validators
+
+### Pandas
+
+This is the default validator used by data_linter as of the version 5 release.
+
+#### Dealing with timestamps and dates
+
+Timestamps are always a pain to deal with especially when using different file types. The Pandas Validator has tried to keep true to the file types based on the tests it runs.
+
+If the file type stores date/timestamp information as a string (i.e. CSV and JSONL) then the pandas Validator will read in the timestamp / date columns as strings. It will then apply validation tests against those columns checking if the string representation of the dates in the data is a valid date. For timestamp and date types these tests assume ISO standard string representation `%Y-%m-%d %H:%M:%S` and `%Y-%m-%d`. If your timestamp/date types are comming in as strings that do not conform to the ISO standard format then you can provide you column in the metadata with a `datetime_format` property that specifies the exected format e.g.
+
+```json
+...
+"columns": [
+    {
+        "name": "date_in_uk",
+        "type": "date64",
+        "datetime_format": "%d/%m/%Y"
+    },
+...
+```
+
+Often you might recieve data that is exported from a system that might encode your timestamp as a date but is written to a format that encodes the data as a timestamp. In this scenario you would expect your dates (in a str timestamp format) to always have a time component of `00:00:00`. You can also use data_linter to validate this by specifing the datetime_format of your column as the expected timestamp in format but still specify that the data type is a date e.g.
+
+```json
+...
+"columns": [
+    {
+        "name": "date_in_uk",
+        "type": "date64",
+        "datetime_format": "%d/%m/%Y 00:00:00"
+    },
+...
+```
+
+In the above data_linter will attempt to fist parse the column with the specified `datetime_format` and then as the column type is date it will check that it it truely a date (and not have a time component).
+
+If the file_format is `parquet` then timestamps are encoded in the filetype and there are just read in as is. Currently data_linter doesn't support minimum and maximum tests for timestamps/dates and also does not currently have tests for time types. 
+
+## Process Diagram
+
+How logic works
+
+![](images/data_linter_process.png)
+
+## How to update
+
+We have tests that run on the current state of the `poetry.lock` file (i.e. the current dependencies). We also run tests based on the most up to date dependencies allowed in `pyproject.toml`. This allows us to see if there will be any issues when updating dependences. These can be run locally in the `tests` folder.
+
+When updating this package, make sure to change the version number in `pyproject.toml` and describe the change in CHANGELOG.md.
+
+If you have changed any dependencies in `pyproject.toml`, run `poetry update` to update `poetry.lock`.
+
+Once you have created a release in GitHub, to publish the latest version to PyPI, run:
+
+```bash
+poetry build
+poetry publish -u <username>
+```
+
+Here, you should substitute <username> for your PyPI username. In order to publish to PyPI, you must be an owner of the project.
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

