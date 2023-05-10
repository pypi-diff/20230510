# Comparing `tmp/cognite_transformations_cli-2.3.4.tar.gz` & `tmp/cognite_transformations_cli-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_transformations_cli-2.3.4.tar", max compression
+gzip compressed data, was "cognite_transformations_cli-2.3.5.tar", max compression
```

## Comparing `cognite_transformations_cli-2.3.4.tar` & `cognite_transformations_cli-2.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10172 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/LICENSE
--rw-r--r--   0        0        0     4288 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/README.md
--rw-r--r--   0        0        0       22 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/__init__.py
--rw-r--r--   0        0        0      270 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/__main__.py
--rw-r--r--   0        0        0     2933 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/clients.py
--rw-r--r--   0        0        0        0 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/__init__.py
--rw-r--r--   0        0        0     3615 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/base.py
--rw-r--r--   0        0        0     1491 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/delete.py
--rw-r--r--   0        0        0        0 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/__init__.py
--rw-r--r--   0        0        0     6459 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/deploy.py
--rw-r--r--   0        0        0     6754 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/load_yaml.py
--rw-r--r--   0        0        0     5351 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_config.py
--rw-r--r--   0        0        0     4342 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_types.py
--rw-r--r--   0        0        0     4705 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
--rw-r--r--   0        0        0    13811 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformations_api.py
--rw-r--r--   0        0        0     2166 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/jobs.py
--rw-r--r--   0        0        0     2438 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/list.py
--rw-r--r--   0        0        0     1242 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/query.py
--rw-r--r--   0        0        0     3639 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/run.py
--rw-r--r--   0        0        0     2787 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/show.py
--rw-r--r--   0        0        0     5792 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/utils.py
--rw-r--r--   0        0        0     1616 2023-05-10 07:21:58.057352 cognite_transformations_cli-2.3.4/pyproject.toml
--rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0    10172 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/LICENSE
+-rw-r--r--   0        0        0     4288 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/README.md
+-rw-r--r--   0        0        0       22 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/__main__.py
+-rw-r--r--   0        0        0     1489 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/clients.py
+-rw-r--r--   0        0        0        0 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/__init__.py
+-rw-r--r--   0        0        0     3615 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/base.py
+-rw-r--r--   0        0        0     1491 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/delete.py
+-rw-r--r--   0        0        0        0 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/__init__.py
+-rw-r--r--   0        0        0     6459 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/deploy.py
+-rw-r--r--   0        0        0     6754 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/load_yaml.py
+-rw-r--r--   0        0        0     5351 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_config.py
+-rw-r--r--   0        0        0     4342 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_types.py
+-rw-r--r--   0        0        0     4705 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
+-rw-r--r--   0        0        0    13069 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformations_api.py
+-rw-r--r--   0        0        0     2166 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/jobs.py
+-rw-r--r--   0        0        0     2438 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/list.py
+-rw-r--r--   0        0        0     1242 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/query.py
+-rw-r--r--   0        0        0     3639 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/run.py
+-rw-r--r--   0        0        0     2787 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/show.py
+-rw-r--r--   0        0        0     5792 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/utils.py
+-rw-r--r--   0        0        0     1616 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.5/PKG-INFO
```

### Comparing `cognite_transformations_cli-2.3.4/LICENSE` & `cognite_transformations_cli-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/README.md` & `cognite_transformations_cli-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/clients.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/clients.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,41 @@
 import logging
 import sys
 from typing import Dict
 
 from cognite.client import CogniteClient
 from cognite.client.config import ClientConfig
-from cognite.client.credentials import APIKey, OAuthClientCredentials
+from cognite.client.credentials import OAuthClientCredentials
 from cognite.client.exceptions import CogniteAPIError
 
 logger = logging.getLogger(name=None)
 
 
-def get_project_from_api_key(client: CogniteClient) -> str:
-    project = client.login.status().project
-    if not project:
-        sys.exit("Invalid authentication, please check the base_url or api_key.")
-    return project
-
-
 def get_client(obj: Dict, timeout: int = 60) -> CogniteClient:
-    api_key = obj.get("api_key")
     client_id = obj.get("client_id")
     client_secret = obj.get("client_secret")
     token_url = obj.get("token_url")
     scopes = obj.get("scopes")
     audience = obj.get("audience")
     cdf_project_name = obj.get("cdf_project_name")
     cluster = obj.get("cluster", "europe-west1-1")
     base_url = f"https://{cluster}.cognitedata.com"
-    if not api_key and not audience:
+    if not audience:
         scopes = scopes.strip().split(" ") if scopes else [f"https://{cluster}.cognitedata.com/.default"]
     try:
-        if api_key is not None and (
-            client_id is not None
-            or client_secret is not None
-            or token_url is not None
-            or scopes is not None
-            or audience is not None
-        ):
-            sys.exit("Please provide only API key configuration or only OAuth2 configuration.")
-        elif api_key is not None:
-            client_config = ClientConfig(
-                client_name="transformations_cli",
-                base_url=base_url,
-                project=cdf_project_name,
-                timeout=timeout,
-                credentials=APIKey(api_key),
-            )
-            client = CogniteClient(client_config)
-            prj = get_project_from_api_key(client)
-            if not cdf_project_name:
-                logger.warn("CDF project name is not provided, it will be detected using the API key.")
-                client.config.project = prj
-            elif prj.lower() != cdf_project_name.lower():
-                sys.exit(f"API key does not grant access to the project {cdf_project_name}.")
-            return client
-        else:
-            token_custom_args = {"audience": audience} if audience else {}
-            client_config = ClientConfig(
-                base_url=base_url,
-                client_name="transformations_cli",
-                project=cdf_project_name,
-                timeout=timeout,
-                credentials=OAuthClientCredentials(
-                    client_id=client_id,
-                    client_secret=client_secret,
-                    token_url=token_url,
-                    scopes=scopes,
-                    **token_custom_args,
-                ),
-            )
-            return CogniteClient(client_config)
+        token_custom_args = {"audience": audience} if audience else {}
+        client_config = ClientConfig(
+            base_url=base_url,
+            client_name="transformations_cli",
+            project=cdf_project_name,
+            timeout=timeout,
+            credentials=OAuthClientCredentials(
+                client_id=client_id,
+                client_secret=client_secret,
+                token_url=token_url,
+                scopes=scopes,
+                **token_custom_args,
+            ),
+        )
+        return CogniteClient(client_config)
     except CogniteAPIError as e:
         sys.exit(f"Cognite client cannot be initialised: {e}.")
```

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/base.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/delete.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/deploy.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/load_yaml.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/load_yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_config.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_config.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_types.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_types.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformations_api.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformations_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,16 +53,14 @@
         name=config.name,
         external_id=config.external_id,
         destination=to_destination(config.destination),
         conflict_mode=to_action(config.action),
         is_public=config.shared,
         ignore_null_fields=config.ignore_null_fields,
         query=to_query(conf_path, config.query),
-        source_api_key=to_read_api_key(config.authentication),
-        destination_api_key=to_write_api_key(config.authentication),
         source_oidc_credentials=to_read_oidc(config.authentication, cluster),
         destination_oidc_credentials=to_write_oidc(config.authentication, cluster),
         data_set_id=to_data_set_id(client, config.data_set_id, config.data_set_external_id),
         tags=config.tags,
     )
 
 
@@ -142,30 +140,14 @@
             with open(sql_path, "r") as f:
                 return f.read()
         return query
     except:
         sys.exit("Please provide a valid path for sql file.")
 
 
-def to_read_api_key(authentication: Union[AuthConfig, ReadWriteAuthentication]) -> Optional[str]:
-    if isinstance(authentication, AuthConfig):
-        return authentication.api_key
-    if isinstance(authentication, ReadWriteAuthentication):
-        return authentication.read.api_key
-    return None
-
-
-def to_write_api_key(authentication: Union[AuthConfig, ReadWriteAuthentication]) -> Optional[str]:
-    if isinstance(authentication, AuthConfig):
-        return authentication.api_key
-    if isinstance(authentication, ReadWriteAuthentication):
-        return authentication.write.api_key
-    return None
-
-
 def stringify_scopes(scopes: Optional[List[str]]) -> Optional[str]:
     if scopes:
         return " ".join(scopes)
     return None
 
 
 def get_default_scopes(scopes: Optional[str], cluster: str) -> str:
```

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/jobs.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/list.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/query.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/run.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/show.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/utils.py` & `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.4/pyproject.toml` & `cognite_transformations_cli-2.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-transformations-cli"
-version = "2.3.4"
+version = "2.3.5"
 description = "A CLI for the Transformations service in CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>", "Emel Varol <emel.varol@cognite.com>", "Einar Marstrander Omang <einar.omang@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/transformations-cli"
 
 packages = [
@@ -26,15 +26,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.2"
 types-retry = "^0.1.5"
 tabulate = "^0.8.9"
 types-tabulate = "^0.8.3"
 sqlparse = "^0.4.2"
-cognite-sdk = "5.7.*"
+cognite-sdk = "6.1.5"
 regex = "^2021.11.10"
 dacite = "^1.6.0"
 python-dotenv = "^0.21.0"
 pyparsing = "^3.0.9"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `cognite_transformations_cli-2.3.4/PKG-INFO` & `cognite_transformations_cli-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cognite-transformations-cli
-Version: 2.3.4
+Version: 2.3.5
 Summary: A CLI for the Transformations service in CDF
 Home-page: https://github.com/cognitedata/transformations-cli
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.0.2,<9.0.0)
-Requires-Dist: cognite-sdk (>=5.7.0,<5.8.0)
+Requires-Dist: cognite-sdk (==6.1.5)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: regex (>=2021.11.10,<2022.0.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: types-retry (>=0.1.5,<0.2.0)
```

