# Comparing `tmp/censys_cloud_connectors-3.1.1b1.tar.gz` & `tmp/censys_cloud_connectors-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censys_cloud_connectors-3.1.1b1.tar", max compression
+gzip compressed data, was "censys_cloud_connectors-3.1.2.tar", max compression
```

## Comparing `censys_cloud_connectors-3.1.1b1.tar` & `censys_cloud_connectors-3.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11342 2023-03-24 17:52:59.951152 censys_cloud_connectors-3.1.1b1/LICENSE
--rw-r--r--   0        0        0     2143 2023-03-24 17:52:59.952152 censys_cloud_connectors-3.1.1b1/README.md
--rw-r--r--   0        0        0     4776 2023-03-24 17:52:59.973154 censys_cloud_connectors-3.1.1b1/pyproject.toml
--rw-r--r--   0        0        0      920 2023-03-24 17:52:59.973154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/__init__.py
--rw-r--r--   0        0        0      439 2023-03-24 17:52:59.973154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/__init__.py
--rw-r--r--   0        0        0    28603 2023-03-24 17:52:59.973154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/connector.py
--rw-r--r--   0        0        0     2766 2023-03-24 17:52:59.973154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/enums.py
--rw-r--r--   0        0        0    18732 2023-03-24 17:52:59.973154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/provider_setup.py
--rwxr-xr-x   0        0        0     1240 2023-03-24 17:52:59.973154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/serverless.py
--rw-r--r--   0        0        0     8355 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/service.py
--rw-r--r--   0        0        0     4192 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/settings.py
--rw-r--r--   0        0        0      343 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/__init__.py
--rw-r--r--   0        0        0    10933 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/connector.py
--rw-r--r--   0        0        0      895 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/enums.py
--rw-r--r--   0        0        0     9199 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/provider_setup.py
--rw-r--r--   0        0        0     1665 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/settings.py
--rw-r--r--   0        0        0      713 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/__init__.py
--rw-r--r--   0        0        0      849 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/__init__.py
--rw-r--r--   0        0        0      888 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/args.py
--rw-r--r--   0        0        0     6405 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/base.py
--rw-r--r--   0        0        0       87 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/commands/__init__.py
--rw-r--r--   0        0        0     2948 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/commands/config.py
--rw-r--r--   0        0        0     3277 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/commands/scan.py
--rw-r--r--   0        0        0     9860 2023-03-24 17:52:59.974154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/provider_setup.py
--rw-r--r--   0        0        0     2609 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cloud_asset.py
--rw-r--r--   0        0        0     8372 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/connector.py
--rw-r--r--   0        0        0      659 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/context.py
--rw-r--r--   0        0        0     1598 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/enums.py
--rw-r--r--   0        0        0     6533 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/healthcheck.py
--rw-r--r--   0        0        0      957 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/ignore_list.py
--rw-r--r--   0        0        0      823 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/logger.py
--rw-r--r--   0        0        0      506 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/models.py
--rw-r--r--   0        0        0      296 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/plugins/__init__.py
--rw-r--r--   0        0        0      489 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/plugins/events.py
--rw-r--r--   0        0        0     1455 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/plugins/plugin.py
--rw-r--r--   0        0        0     5633 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/plugins/registry.py
--rw-r--r--   0        0        0     2858 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/seed.py
--rw-r--r--   0        0        0     8864 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/settings.py
--rw-r--r--   0        0        0      329 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/__init__.py
--rw-r--r--   0        0        0    12081 2023-03-24 17:52:59.975154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/connector.py
--rw-r--r--   0        0        0     5883 2023-03-24 17:52:59.976154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/enums.py
--rw-r--r--   0        0        0    27935 2023-03-24 17:52:59.976154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/provider_setup.py
--rw-r--r--   0        0        0     1688 2023-03-24 17:52:59.976154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/settings.py
--rw-r--r--   0        0        0       36 2023-03-24 17:52:59.976154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/plugins/__init__.py
--rw-r--r--   0        0        0    14559 2023-03-24 17:52:59.976154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/plugins/aws_tags.py
--rw-r--r--   0        0        0     1882 2023-03-24 17:52:59.976154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/plugins/example.py
--rw-r--r--   0        0        0        0 2023-03-24 17:52:59.976154 censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/py.typed
--rw-r--r--   0        0        0     4227 1970-01-01 00:00:00.000000 censys_cloud_connectors-3.1.1b1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-10 15:51:44.059371 censys_cloud_connectors-3.1.2/LICENSE
+-rw-r--r--   0        0        0     2143 2023-05-10 15:51:44.059371 censys_cloud_connectors-3.1.2/README.md
+-rw-r--r--   0        0        0     4562 2023-05-10 15:51:44.072372 censys_cloud_connectors-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0      920 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/__init__.py
+-rw-r--r--   0        0        0    28603 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/connector.py
+-rw-r--r--   0        0        0     2766 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/enums.py
+-rw-r--r--   0        0        0    18732 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/provider_setup.py
+-rwxr-xr-x   0        0        0     1240 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/serverless.py
+-rw-r--r--   0        0        0     8355 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/service.py
+-rw-r--r--   0        0        0     4192 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/settings.py
+-rw-r--r--   0        0        0      343 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/__init__.py
+-rw-r--r--   0        0        0    10933 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/connector.py
+-rw-r--r--   0        0        0      895 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/enums.py
+-rw-r--r--   0        0        0     9199 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/provider_setup.py
+-rw-r--r--   0        0        0     1665 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/settings.py
+-rw-r--r--   0        0        0      713 2023-05-10 15:51:44.073372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/__init__.py
+-rw-r--r--   0        0        0      849 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/__init__.py
+-rw-r--r--   0        0        0      888 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/args.py
+-rw-r--r--   0        0        0     6405 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/base.py
+-rw-r--r--   0        0        0       87 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2948 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/config.py
+-rw-r--r--   0        0        0     3277 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/scan.py
+-rw-r--r--   0        0        0     9860 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/provider_setup.py
+-rw-r--r--   0        0        0     2609 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cloud_asset.py
+-rw-r--r--   0        0        0     8372 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/connector.py
+-rw-r--r--   0        0        0      659 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/context.py
+-rw-r--r--   0        0        0     1598 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/enums.py
+-rw-r--r--   0        0        0     6533 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/healthcheck.py
+-rw-r--r--   0        0        0      957 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/ignore_list.py
+-rw-r--r--   0        0        0      857 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/logger.py
+-rw-r--r--   0        0        0      506 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/models.py
+-rw-r--r--   0        0        0      296 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/__init__.py
+-rw-r--r--   0        0        0      489 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/events.py
+-rw-r--r--   0        0        0     1455 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/plugin.py
+-rw-r--r--   0        0        0     5633 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/registry.py
+-rw-r--r--   0        0        0     2858 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/seed.py
+-rw-r--r--   0        0        0     8864 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/settings.py
+-rw-r--r--   0        0        0      329 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/__init__.py
+-rw-r--r--   0        0        0    12081 2023-05-10 15:51:44.074372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/connector.py
+-rw-r--r--   0        0        0     5883 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/enums.py
+-rw-r--r--   0        0        0    27935 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/provider_setup.py
+-rw-r--r--   0        0        0     1688 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/settings.py
+-rw-r--r--   0        0        0       36 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/__init__.py
+-rw-r--r--   0        0        0    14559 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/aws_tags.py
+-rw-r--r--   0        0        0     1882 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/example.py
+-rw-r--r--   0        0        0        0 2023-05-10 15:51:44.075372 censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/py.typed
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 censys_cloud_connectors-3.1.2/PKG-INFO
```

### Comparing `censys_cloud_connectors-3.1.1b1/LICENSE` & `censys_cloud_connectors-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/README.md` & `censys_cloud_connectors-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/pyproject.toml` & `censys_cloud_connectors-3.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 [tool.poetry]
 name = "censys-cloud-connectors"
-version = "3.1.1b1"
+version = "3.1.2"
 description = "The Censys Unified Cloud Connector is a standalone connector that gathers assets from various cloud providers and stores them in Censys ASM."
 authors = ["Censys, Inc. <support@censys.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "censys/cloud_connectors", from = "src" }]
 keywords = ["censys", "cloud", "connector", "attack surface management"]
 classifiers = [
     "Typing :: Typed",
     "Topic :: Internet",
     "Topic :: Security",
+    "Topic :: System :: Monitoring",
     "Topic :: System :: Networking",
     "Topic :: System :: Networking :: Monitoring",
     "Topic :: Utilities",
     "Environment :: Console",
     "Natural Language :: English",
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.urls]
 "Censys Homepage" = "https://censys.io/"
 "Discussions" = "https://github.com/censys/censys-cloud-connector/discussions"
 "Changelog" = "https://github.com/censys/censys-cloud-connector/releases"
 "Tracker" = "https://github.com/censys/censys-cloud-connector/issues"
 "Source" = "https://github.com/censys/censys-cloud-connector"
 
 [tool.poetry.scripts]
 censys-cc = "censys.cloud_connectors.common.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-backoff = "^2.1.2"
-censys = "^2.1.8"
+backoff = "^2.2.1"
+censys = "^2.2.2"
 inquirerpy = "^0.3.3"
 pydantic = {extras = ["dotenv", "email"], version = "^1.9.0"}
 PyYAML = "^6.0"
-requests = "^2.27.1"
-rich = "^12.4.4"
-
-[tool.poetry.group.dev]
-optional = true
+requests = "^2.30.0"
+rich = "^13.3.5"
 
 [tool.poetry.group.dev.dependencies]
 # Debug
 ipython = "^8.11.0"
 # Linting
 black = "^22.1.0"
 blacken-docs = "^1.12.1"
@@ -101,27 +100,18 @@
 sphinxcontrib-asciinema = "^0.3.6"
 
 [tool.poetry.group.aws.dependencies]
 boto3 = "^1.24.63"
 boto3-stubs = {extras = ["apigateway", "apigatewayv2", "ec2", "ecs", "elb", "elbv2", "rds", "route53", "route53domains", "s3", "sts"], version = "^1.24.63"}
 
 [tool.poetry.group.azure.dependencies]
-azure-cli = "^2.34.1"
-azure-common = "^1.1.28"
-azure-core = "^1.22.0"
-azure-identity = "^1.7.1"
-azure-mgmt-compute = ">=25.0.0,<25.1.0"
-azure-mgmt-containerinstance = "^9.1.0"
-azure-mgmt-core = "^1.3.0"
-azure-mgmt-dns = "^8.0.0"
-azure-mgmt-network = "^19.3.0"
-azure-mgmt-resource = "20.0.0"
-azure-mgmt-sql = "^3.0.1"
-azure-mgmt-storage = "^19.1.0"
-azure-storage-blob = "^12.9.0"
+azure-cli = "^2.48.1"
+azure-identity = "^1.12.0"
+azure-mgmt-network = "^23.0.1"
+azure-storage-blob = "^12.16.0"
 # Specified sys_platform to avoid issues with platform_system
 pywin32 = {version = "^303", markers = "sys_platform == 'win32'"}
 
 [tool.poetry.group.gcp.dependencies]
 google-auth = "^2.6.0"
 google-cloud-resource-manager = "^1.4.1"
 google-cloud-securitycenter = "^1.9.0"
```

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/__init__.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/connector.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/connector.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/enums.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/provider_setup.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/serverless.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/serverless.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/service.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/service.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/aws_connector/settings.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/aws_connector/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/connector.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/connector.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/enums.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/provider_setup.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/azure_connector/settings.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/azure_connector/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/__init__.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/__init__.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/args.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/args.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/base.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/base.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/commands/config.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/commands/scan.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/commands/scan.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cli/provider_setup.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cli/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/cloud_asset.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/cloud_asset.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/connector.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/connector.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/context.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/context.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/enums.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/healthcheck.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/healthcheck.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/ignore_list.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/ignore_list.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/logger.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,16 @@
             Options are [CRITICAL, ERROR, WARNING, INFO, DEBUG].
 
     Returns:
         logger: A logger configured with the provided logging settings.
     """
     logger = logging.getLogger(log_name)
     if not logger.hasHandlers():
-        formatter = logging.Formatter(fmt="%(levelname)s:%(name)s: %(message)s")
+        formatter = logging.Formatter(
+            fmt="%(asctime)s:%(levelname)s:%(name)s: %(message)s"
+        )
         handler = logging.StreamHandler()
         handler.setFormatter(formatter)
         logger.addHandler(handler)
     logger.setLevel(level)
 
     return logger
```

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/plugins/plugin.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/plugins/registry.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/seed.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/seed.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/common/settings.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/common/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/connector.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/connector.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/enums.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/provider_setup.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/gcp_connector/settings.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/gcp_connector/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/plugins/aws_tags.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/aws_tags.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/src/censys/cloud_connectors/plugins/example.py` & `censys_cloud_connectors-3.1.2/src/censys/cloud_connectors/plugins/example.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.1b1/PKG-INFO` & `censys_cloud_connectors-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: censys-cloud-connectors
-Version: 3.1.1b1
+Version: 3.1.2
 Summary: The Censys Unified Cloud Connector is a standalone connector that gathers assets from various cloud providers and stores them in Censys ASM.
 License: Apache-2.0
 Keywords: censys,cloud,connector,attack surface management
 Author: Censys, Inc.
 Author-email: support@censys.io
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
+Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: backoff (>=2.1.2,<3.0.0)
-Requires-Dist: censys (>=2.1.8,<3.0.0)
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: censys (>=2.2.2,<3.0.0)
 Requires-Dist: inquirerpy (>=0.3.3,<0.4.0)
 Requires-Dist: pydantic[dotenv,email] (>=1.9.0,<2.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: rich (>=12.4.4,<13.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
 Project-URL: Censys Homepage, https://censys.io/
 Project-URL: Changelog, https://github.com/censys/censys-cloud-connector/releases
 Project-URL: Discussions, https://github.com/censys/censys-cloud-connector/discussions
 Project-URL: Source, https://github.com/censys/censys-cloud-connector
 Project-URL: Tracker, https://github.com/censys/censys-cloud-connector/issues
 Description-Content-Type: text/markdown
```

