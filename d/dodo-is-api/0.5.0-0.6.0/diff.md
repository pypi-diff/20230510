# Comparing `tmp/dodo_is_api-0.5.0.tar.gz` & `tmp/dodo_is_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodo_is_api-0.5.0.tar", max compression
+gzip compressed data, was "dodo_is_api-0.6.0.tar", max compression
```

## Comparing `dodo_is_api-0.5.0.tar` & `dodo_is_api-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.5.0/LICENSE
--rw-r--r--   0        0        0     3628 2023-03-24 05:03:49.211961 dodo_is_api-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.5.0/dodo_is_api/__init__.py
--rw-r--r--   0        0        0       55 2023-05-09 10:02:09.923060 dodo_is_api-0.5.0/dodo_is_api/connection/__init__.py
--rw-r--r--   0        0        0     1932 2023-05-09 09:57:16.078330 dodo_is_api-0.5.0/dodo_is_api/connection/asynchronous.py
--rw-r--r--   0        0        0     1291 2023-05-09 10:07:07.658345 dodo_is_api-0.5.0/dodo_is_api/connection/base.py
--rw-r--r--   0        0        0     2131 2023-03-18 06:06:54.112897 dodo_is_api-0.5.0/dodo_is_api/connection/http_clients.py
--rw-r--r--   0        0        0     7300 2023-05-09 10:07:07.653484 dodo_is_api-0.5.0/dodo_is_api/connection/synchronous.py
--rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.5.0/dodo_is_api/exceptions.py
--rw-r--r--   0        0        0     7200 2023-04-15 05:46:29.175976 dodo_is_api-0.5.0/dodo_is_api/mappers.py
--rw-r--r--   0        0        0       45 2023-03-18 11:36:04.461463 dodo_is_api-0.5.0/dodo_is_api/models/__init__.py
--rw-r--r--   0        0        0     2798 2023-04-15 05:38:46.839507 dodo_is_api-0.5.0/dodo_is_api/models/dodo_is_api.py
--rw-r--r--   0        0        0     1685 2023-04-15 05:38:46.839663 dodo_is_api-0.5.0/dodo_is_api/models/raw.py
--rw-r--r--   0        0        0      539 2023-05-09 10:15:21.294850 dodo_is_api-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 dodo_is_api-0.5.0/setup.py
--rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 dodo_is_api-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3628 2023-03-24 05:03:49.211961 dodo_is_api-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.6.0/dodo_is_api/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.6.0/dodo_is_api/connection/__init__.py
+-rw-r--r--   0        0        0     4078 2023-05-10 05:30:00.804758 dodo_is_api-0.6.0/dodo_is_api/connection/asynchronous.py
+-rw-r--r--   0        0        0     1291 2023-05-10 05:26:32.091787 dodo_is_api-0.6.0/dodo_is_api/connection/base.py
+-rw-r--r--   0        0        0     2131 2023-03-18 06:06:54.112897 dodo_is_api-0.6.0/dodo_is_api/connection/http_clients.py
+-rw-r--r--   0        0        0     7300 2023-05-10 05:26:32.092054 dodo_is_api-0.6.0/dodo_is_api/connection/synchronous.py
+-rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.6.0/dodo_is_api/exceptions.py
+-rw-r--r--   0        0        0     7200 2023-05-10 05:26:32.092333 dodo_is_api-0.6.0/dodo_is_api/mappers.py
+-rw-r--r--   0        0        0       45 2023-03-18 11:36:04.461463 dodo_is_api-0.6.0/dodo_is_api/models/__init__.py
+-rw-r--r--   0        0        0     2798 2023-05-10 05:26:32.092595 dodo_is_api-0.6.0/dodo_is_api/models/dodo_is_api.py
+-rw-r--r--   0        0        0     1685 2023-05-10 05:26:32.092836 dodo_is_api-0.6.0/dodo_is_api/models/raw.py
+-rw-r--r--   0        0        0      539 2023-05-10 05:31:21.339757 dodo_is_api-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 dodo_is_api-0.6.0/setup.py
+-rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 dodo_is_api-0.6.0/PKG-INFO
```

### Comparing `dodo_is_api-0.5.0/LICENSE` & `dodo_is_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.5.0/README.md` & `dodo_is_api-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.5.0/dodo_is_api/connection/base.py` & `dodo_is_api-0.6.0/dodo_is_api/connection/base.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.5.0/dodo_is_api/connection/http_clients.py` & `dodo_is_api-0.6.0/dodo_is_api/connection/http_clients.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.5.0/dodo_is_api/connection/synchronous.py` & `dodo_is_api-0.6.0/dodo_is_api/connection/synchronous.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.5.0/dodo_is_api/mappers.py` & `dodo_is_api-0.6.0/dodo_is_api/mappers.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.5.0/dodo_is_api/models/dodo_is_api.py` & `dodo_is_api-0.6.0/dodo_is_api/models/dodo_is_api.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.5.0/dodo_is_api/models/raw.py` & `dodo_is_api-0.6.0/dodo_is_api/models/raw.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.5.0/pyproject.toml` & `dodo_is_api-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dodo-is-api"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Eldos <eldos.baktybekov@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dodo_is_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dodo_is_api-0.5.0/setup.py` & `dodo_is_api-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.3,<0.24.0']
 
 setup_kwargs = {
     'name': 'dodo-is-api',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': '',
     'long_description': '<div align="center">\n<a href="https://dodo-brands.stoplight.io">\n<img width="350px" src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">\n</a>\n</div>\n    \n<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n- Delivery:\n    - [Late delivery vouchers](#get-late-delivery-vouchers-)\n- Production:\n    - [Stop sales](#get-stop-sales-)\n\n---\n\n#### 🛵 Get late delivery vouchers:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_late_delivery_voucher_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # it will handle pagination for you\n    for late_delivery_vouchers in dodo_is_api_connection.iter_late_delivery_vouchers(\n            from_date=from_date,\n            to_date=to_date,\n            units=units\n    ):\n        # map to dataclass DTO if you need\n        late_delivery_voucher_dtos = [\n            map_late_delivery_voucher_dto(late_delivery_voucher)\n            for late_delivery_voucher in late_delivery_vouchers\n        ]\n        ...\n```\n\n---\n\n#### 📦 Get stop sales:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_stop_sale_by_ingredient_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # for products - dodo_is_api_connection.get_stop_sales_by_products\n    # for sales channels - dodo_is_api_connection.get_stop_sales_by_sales_channels\n    stop_sales = dodo_is_api_connection.get_stop_sales_by_ingredients(\n        from_date=from_date,\n        to_date=to_date,\n        units=units\n    )\n\n    # map to dataclass DTO if you need\n    # use suitable mapper\n    # in this case, ingredient stop sale mapper is used\n    late_delivery_voucher_dtos = [\n        map_stop_sale_by_ingredient_dto(stop_sale)\n        for stop_sale in stop_sales\n    ]\n    ...\n```\n',
     'author': 'Eldos',
     'author_email': 'eldos.baktybekov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['dodo_is_api', 'dodo_is_api.connection', 'dodo_is_api.models'] package_data =
 \ {'': ['*']} install_requires = \ ['httpx>=0.23.3,<0.24.0'] setup_kwargs =
-{ 'name': 'dodo-is-api', 'version': '0.5.0', 'description': '',
+{ 'name': 'dodo-is-api', 'version': '0.6.0', 'description': '',
 'long_description': '
   \n\n[https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]\n\n
 \n \n
                   ****** \nð Dodo IS API Wrapper\n ******
 \n\n
 \n\n[Test_badge]\n\n\n[https://codecov.io/gh/goretsky-integration/dodo-is-api-
   python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD]\n\n[python]\n
```

### Comparing `dodo_is_api-0.5.0/PKG-INFO` & `dodo_is_api-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodo-is-api
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Eldos
 Author-email: eldos.baktybekov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dodo-is-api Version: 0.5.0 Summary: Author: Eldos
+Metadata-Version: 2.1 Name: dodo-is-api Version: 0.6.0 Summary: Author: Eldos
 Author-email: eldos.baktybekov@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.3,<0.24.0) Description-
 Content-Type: text/markdown
       [https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]
                     ****** ð Dodo IS API Wrapper ******
  [Test_badge] [https://codecov.io/gh/goretsky-integration/dodo-is-api-python-
```

