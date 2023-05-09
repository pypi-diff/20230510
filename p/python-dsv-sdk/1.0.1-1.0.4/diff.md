# Comparing `tmp/python-dsv-sdk-1.0.1.tar.gz` & `tmp/python-dsv-sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dsv-sdk-1.0.1.tar", last modified: Wed Oct  6 16:15:23 2021, max compression
+gzip compressed data, was "python-dsv-sdk-1.0.4.tar", last modified: Tue May  9 22:56:21 2023, max compression
```

## Comparing `python-dsv-sdk-1.0.1.tar` & `python-dsv-sdk-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,51 @@
--rw-r--r--   0        0        0      590 2021-10-06 16:15:14.846469 python-dsv-sdk-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      759 2021-10-06 16:15:14.846469 python-dsv-sdk-1.0.1/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0     1832 2021-10-06 16:15:14.846469 python-dsv-sdk-1.0.1/.gitignore
--rw-r--r--   0        0        0    11338 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/LICENSE
--rw-r--r--   0        0        0     3472 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/README.md
--rw-r--r--   0        0        0      643 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/conftest.py
--rw-r--r--   0        0        0      810 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/example.py
--rw-r--r--   0        0        0      668 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       63 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/requirements.txt
--rw-r--r--   0        0        0     1201 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/tests/test_vault.py
--rw-r--r--   0        0        0       72 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/thycotic/__init__.py
--rw-r--r--   0        0        0        0 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/thycotic/secrets/__init__.py
--rw-r--r--   0        0        0     9063 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/thycotic/secrets/vault.py
--rw-r--r--   0        0        0      567 2021-10-06 16:15:14.850470 python-dsv-sdk-1.0.1/tox.ini
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 python-dsv-sdk-1.0.1/setup.py
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 python-dsv-sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      305 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.changes/header.tpl.md
+-rw-r--r--   0        0        0        0 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.changes/unreleased/.gitkeep
+-rw-r--r--   0        0        0       95 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.changes/v1.0.1.md
+-rw-r--r--   0        0        0      485 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.changes/v1.0.2.md
+-rw-r--r--   0        0        0      203 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.changes/v1.0.3.md
+-rw-r--r--   0        0        0      158 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.changes/v1.0.4.md
+-rw-r--r--   0        0        0     1500 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.changie.yaml
+-rwxr-xr-x   0        0        0     1043 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.devcontainer/Dockerfile
+-rwxr-xr-x   0        0        0     3436 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     1220 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.devcontainer/files/.zshrc
+-rwxr-xr-x   0        0        0      288 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.devcontainer/files/first-run-notice.txt
+-rwxr-xr-x   0        0        0      266 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.devcontainer/init
+-rwxr-xr-x   0        0        0      309 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.devcontainer/init.bat
+-rw-r--r--   0        0        0      251 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      331 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      582 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      489 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/ISSUE_TEMPLATE/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      742 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      269 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/auto-assign.yml
+-rw-r--r--   0        0        0      240 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/workflows/assign.yml
+-rw-r--r--   0        0        0      344 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/workflows/conventional-pr.yml
+-rw-r--r--   0        0        0      593 2023-05-09 22:56:15.778254 python-dsv-sdk-1.0.4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1058 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      824 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1832 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.gitignore
+-rw-r--r--   0        0        0     4395 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.golangci.yml
+-rw-r--r--   0        0        0     2131 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.markdownlint.yaml
+-rw-r--r--   0        0        0       69 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.trunk/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.trunk/config/.flake8
+-rw-r--r--   0        0        0       78 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.trunk/config/.hadolint.yaml
+-rw-r--r--   0        0        0       25 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.trunk/config/.isort.cfg
+-rw-r--r--   0        0        0      217 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.trunk/config/.markdownlint.yaml
+-rw-r--r--   0        0        0      835 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.trunk/trunk.yaml
+-rw-r--r--   0        0        0      541 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.whitesource
+-rw-r--r--   0        0        0      502 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/.yamllint.yaml
+-rw-r--r--   0        0        0     1250 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1052 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4092 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/README.md
+-rw-r--r--   0        0        0      742 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/aqua.yaml
+-rw-r--r--   0        0        0      527 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/codecov.yml
+-rw-r--r--   0        0        0      642 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/conftest.py
+-rw-r--r--   0        0        0       72 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/delinea/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/delinea/secrets/__init__.py
+-rw-r--r--   0        0        0     9060 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/delinea/secrets/vault.py
+-rw-r--r--   0        0        0      831 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/example.py
+-rw-r--r--   0        0        0      551 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/renovate.json
+-rw-r--r--   0        0        0       46 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/requirements.txt
+-rw-r--r--   0        0        0     1200 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/tests/test_vault.py
+-rw-r--r--   0        0        0      562 2023-05-09 22:56:15.782254 python-dsv-sdk-1.0.4/tox.ini
+-rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 python-dsv-sdk-1.0.4/PKG-INFO
```

### Comparing `python-dsv-sdk-1.0.1/.github/workflows/publish.yml` & `python-dsv-sdk-1.0.4/.github/workflows/release.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-name: Release
+name: release
 
 on:
   push:
     tags:
-      - 'v*'
+      - "v*"
+  workflow_dispatch:
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
-
-    - name: Set up Python
-      uses: actions/setup-python@v2
-      with:
-        python-version: '3.x'
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python -m pip install flit
-        
-    - name: Build package
-      run: flit build
-
-    - name: Publish package
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}
+      - id: dsv
+        uses: DelineaXPM/dsv-github-action@v2.0.2
+        with:
+          domain: ${{ secrets.DSV_SERVER }}
+          clientId: ${{ secrets.DSV_CLIENT_ID }}
+          clientSecret: ${{ secrets.DSV_CLIENT_SECRET }}
+          retrieve: |
+            [
+             {"secretPath": "ci:publish:pypi", "secretKey": "PYPI_API_TOKEN", "outputVariable": "PYPI_API_TOKEN"}
+            ]
+      - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.x"
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install flit
+
+      - name: Build package
+        run: flit build
+
+      - name: Publish package
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          user: __token__
+          password: "${{ env.PYPI_API_TOKEN }}" # ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `python-dsv-sdk-1.0.1/.github/workflows/run_tests.yml` & `python-dsv-sdk-1.0.4/.github/workflows/test.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-name: Run Tests
+name: test
 
 on: [pull_request]
 
 jobs:
-  
   build:
     runs-on: ubuntu-latest
     environment: testing
     strategy:
       matrix:
-        python: [3.6, 3.7, 3.8, 3.9, "3.10"]
+        python: [3.7, 3.8, 3.9, "3.10"]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
 
       - name: Install Tox
         run: |
           python -m pip install --upgrade pip
           pip install tox
-          
+
       - name: Run Tox
         # Run tox using the version of Python in `PATH`
         run: tox -e py
         env:
           DSV_CLIENT_ID: ${{ secrets.DSV_CLIENT_ID }}
           DSV_CLIENT_SECRET: ${{ secrets.DSV_CLIENT_SECRET }}
           DSV_BASE_URL: ${{ secrets.DSV_BASE_URL }}
+      - uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: false
```

### Comparing `python-dsv-sdk-1.0.1/.gitignore` & `python-dsv-sdk-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python-dsv-sdk-1.0.1/conftest.py` & `python-dsv-sdk-1.0.4/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pytest
 from dotenv import load_dotenv
-from thycotic.secrets.vault import PasswordGrantAuthorizer, SecretsVault
+from delinea.secrets.vault import PasswordGrantAuthorizer, SecretsVault
 
 
 load_dotenv()
 
 
 @pytest.fixture
 def env_vars():
```

### Comparing `python-dsv-sdk-1.0.1/example.py` & `python-dsv-sdk-1.0.4/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from thycotic.secrets.vault import (
+from delinea.secrets.vault import (
     PasswordGrantAuthorizer,
     SecretsVault,
     SecretsVaultAccessError,
     SecretsVaultError,
     VaultSecret,
 )
 
@@ -17,18 +17,20 @@
 def main():
 
     try:
         authorizer = PasswordGrantAuthorizer(BASE_URL, CLIENT_ID, CLIENT_SECRET)
         vault = SecretsVault(BASE_URL, authorizer)
         secret = VaultSecret(**vault.get_secret("/test/sdk/simple"))
 
-        print(f"""
+        print(
+            f"""
         username: {secret.data['username']}
         password: {secret.data['password']}
-        """)
+        """
+        )
 
     except SecretsVaultAccessError as e:
         print(e.message)
     except SecretsVaultError as e:
         print(e.response.text)
```

### Comparing `python-dsv-sdk-1.0.1/pyproject.toml` & `python-dsv-sdk-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
-module = "thycotic"
-author = "Adam Migus"
-author-email = "adam@migus.org"
-classifiers = [ 
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
+module = "delinea"
+author = "Delinea"
+classifiers = [
+  "License :: OSI Approved :: Apache Software License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
 ]
 description-file = "README.md"
-requires = [
-    "dataclasses",
-    "requests >= 2.22.0"
-]
-requires-python=">=3.6"
+requires = ["requests >= 2.22.0"]
+requires-python = ">=3.7"
 dist-name = "python-dsv-sdk"
```

### Comparing `python-dsv-sdk-1.0.1/tests/test_vault.py` & `python-dsv-sdk-1.0.4/tests/test_vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from thycotic.secrets.vault import (
+from delinea.secrets.vault import (
     AccessTokenAuthorizer,
     SecretsVault,
     SecretsVaultAccessError,
     VaultSecret,
 )
```

### Comparing `python-dsv-sdk-1.0.1/thycotic/secrets/vault.py` & `python-dsv-sdk-1.0.4/delinea/secrets/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" The Thycotic DevOps Secrets Vault (DSV) SDK API facilitates access to DSV
+""" The Delinea DevOps Secrets Vault (DSV) SDK API facilitates access to DSV
 using bearer token authentication.
 
 Example::
     authorizer = PasswordGrantAuthorizer("https://mytenant.secretsvaultcloud.com/", "my_client_id", "my_client_secret")
     vault = SecretsVault("https://mytenant.secretsvaultcloud.com/", authorizer)
     # to get the secret as a ``dict``
     secret = vault.get_secret("/path/to/secret")
@@ -180,15 +180,15 @@
         self._refresh_access_grant()
         return self.access_grant["accessToken"]
 
 
 class SecretsVault:
     """A class that uses bearer token authentication to access the DSV API.
 
-    It Uses :attr:`base_url`, :attr:`authorizer` to make calls to the DSV REST 
+    It Uses :attr:`base_url`, :attr:`authorizer` to make calls to the DSV REST
     API
     """
 
     SECRET_PATH_URI = "secrets"
 
     @staticmethod
     def process(response):
@@ -216,15 +216,15 @@
         base_url,
         authorizer: Authorizer,
         api_path_uri="/v1",
     ):
         """
         :param base_url: The DSV URL i.e. mytenant.secretsvaultcloud.com
         :type base_url: str
-        :param authorizer: The Authorizer class used to authenticate to the DSV 
+        :param authorizer: The Authorizer class used to authenticate to the DSV
             REST API
         :type authorizer: Authorizer class
         """
 
         self.base_url = base_url.rstrip("/")
         self.authorizer = authorizer
         self.api_url = base_url.rstrip("/") + "/" + api_path_uri.strip("/")
```

### Comparing `python-dsv-sdk-1.0.1/tox.ini` & `python-dsv-sdk-1.0.4/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 # Docs for tox config -> https://tox.readthedocs.io/en/latest/config.html
 
 [tox]
-envlist = 3.6, 3.7, 3.8, 3.9, 3.10
+envlist = 3.7, 3.8, 3.9, 3.10
 isolated_build = True
 skipsdist = True
 
 [testenv]
 deps =
     pytest
     requests
```

### Comparing `python-dsv-sdk-1.0.1/PKG-INFO` & `python-dsv-sdk-1.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: python-dsv-sdk
-Version: 1.0.1
-Summary: The Thycotic DevOps Secret Vault Python SDK
-Author: Adam Migus
-Author-email: adam@migus.org
-Requires-Python: >=3.6
+Version: 1.0.4
+Summary: The Delinea DevOps Secret Vault Python SDK
+Author: Delinea
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: dataclasses
 Requires-Dist: requests >= 2.22.0
 
-# The Thycotic DevOps Secrets Vault Python SDK
+# The Delinea DevOps Secrets Vault Python SDK
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ![PyPI Version](https://img.shields.io/pypi/v/python-dsv-sdk)
-![License](https://img.shields.io/github/license/thycotic/python-dsv-sdk)
+![License](https://img.shields.io/github/license/DelineaXPM/python-dsv-sdk)
 ![Python Versions](https://img.shields.io/pypi/pyversions/python-dsv-sdk)
 
-The [Thycotic](https://thycotic.com/)
-[DevOps Secrets Vault](https://thycotic.com/products/devops-secrets-vault-password-management/)
+The [Delinea](https://delinea.com/)
+[DevOps Secrets Vault](https://delinea.com/products/devops-secrets-management-vault)
 (DSV) Python SDK contains classes that interact with the DSV REST API.
 
 ## Install
 
 ```shell
 python -m pip install python-dsv-sdk
 ```
@@ -42,75 +41,79 @@
 ### Authorizers
 
 #### Password Authorization
 
 If using a traditional `client_id` and a `client_secret` to authenticate in to your DevOps Secrets Vault, you can pass the `PasswordGrantAuthorizer` into the `SecretsVault` class at instantiation. The `PasswordGrantAuthorizer` requires a `base_url`, `username`, and `password`. It _optionally_ takes a `token_path_uri`, but defaults to `/v1/token`.
 
 ```python
-from thycotic.secrets.vault import PasswordGrantAuthorizer
+from delinea.secrets.vault import PasswordGrantAuthorizer
 
 authorizer = PasswordGrantAuthorizer("https://mytenant.secretsvaultcloud.com/", "my_client_id", "my_client_secret")
 ```
 
 #### Access Token Authorization
 
 If you already have a valid `access_token`, you can pass directly via the `AccessTokenAuthorizer`.
 
 ```python
-from thycotic.secrets.vault import AccessTokenAuthorizer
+from delinea.secrets.vault import AccessTokenAuthorizer
 
 authorizer = AccessTokenAuthorizer("YgJ1slfZs8ng9bKsRsB-tic0Kh8I...")
 ```
 
 ### Secrets Vault
 
 Instantiate `SecretsVault` by passing your `base_url` and `Authorizer` as arguments:
 
 ```python
-from thycotic.secrets.vault import SecretsVault
+from delinea.secrets.vault import SecretsVault
 
 vault = SecretsVault("https://mytenant.secretsvaultcloud.com/", authorizer)
 ```
 
 Secrets can be fetched using the `get_secret` method, which takes the `secret_path` of the secret and returns a `json` object. Alternatively, you can use pass the json to `VaultSecret` which returns a `dataclass` object representation of the secret:
 
 ```python
-from thycotic.secrets.vault import VaultSecret
+from delinea.secrets.vault import VaultSecret
 
 secret = VaultSecret(**vault.get_secret("/test/secret"))
 
 print(f"username: {secret.data['username']}\npassword: {secret.data['password']}")
 ```
 
+## Using Self-Signed Certificates
+
+When using a self-signed certificate for SSL, the `REQUESTS_CA_BUNDLE` environment variable should be set to the path of the certificate (in `.pem` format). This will negate the need to ignore SSL certificate verification, which makes your application vunerable. Please reference the [`requests` documentation](https://docs.python-requests.org/en/master/user/advanced/#ssl-cert-verification) for further details on the `REQUESTS_CA_BUNDLE` environment variable, should you require it.
+
 ## Create a Build Environment (optional)
 
-The SDK requires [Python 3.6](https://www.python.org/downloads/) or higher.
+The SDK requires [Python 3.7](https://www.python.org/downloads/) or higher.
 
-First, ensure Python 3.6 is in `$PATH` then run:
+Assuming that you have a supported version of Python installed, you can clone
+this repository and set up your environment with:
 
 ```shell
 # Clone the repo
-git clone https://github.com/thycotic/python-dsv-sdk
+git clone https://github.com/DelineaXPM/python-dsv-sdk
 cd python-dsv-sdk
 
 # Create a virtual environment
 python -m venv venv
 . venv/bin/activate
 
 # Install dependencies
 python -m pip install --upgrade pip
 pip install -r requirements.txt
-
 ```
 
 Valid credentials are required to run the unit tests. The credentials should be stored in environment variables or in a `.env` file:
 
 ```shell
-export DSV_CLIENT_ID="e7f6be68-0acb-4020-9c55-c7b161620199"
-export DSV_CLIENT_SECRET="0lYBbBbaXtkMd3WYydhfhuy0rHNFet_jq7QA4ZfEjxU"
+export DSV_CLIENT_ID=""
+export DSV_CLIENT_SECRET=""
 export DSV_BASE_URL="https://my.secretsvaultcloud.com/"
 ```
 
 The tests assume that the client associated with the specified `CLIENT_ID` can read the secret with the path `/test/sdk/simple`.
 
 > Note: The secret path can be changed manually in `test_server.py` to a secret path that the client can access.
```

