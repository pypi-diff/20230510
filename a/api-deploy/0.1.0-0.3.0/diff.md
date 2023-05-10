# Comparing `tmp/api-deploy-0.1.0.tar.gz` & `tmp/api-deploy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-deploy-0.1.0.tar", last modified: Tue May  9 14:24:18 2023, max compression
+gzip compressed data, was "api-deploy-0.3.0.tar", last modified: Wed May 10 15:16:57 2023, max compression
```

## Comparing `api-deploy-0.1.0.tar` & `api-deploy-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-05-09 14:24:18.080102 api-deploy-0.1.0/
--rw-r--r--   0 fabian     (501) staff       (20)      740 2023-05-09 14:24:18.079978 api-deploy-0.1.0/PKG-INFO
--rw-r--r--   0 fabian     (501) staff       (20)       12 2022-12-17 05:34:22.000000 api-deploy-0.1.0/README.md
-drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-05-09 14:24:18.078820 api-deploy-0.1.0/api_deploy/
--rw-r--r--   0 fabian     (501) staff       (20)       18 2023-05-09 14:24:12.000000 api-deploy-0.1.0/api_deploy/__init__.py
--rw-r--r--   0 fabian     (501) staff       (20)     2694 2023-05-09 09:19:16.000000 api-deploy-0.1.0/api_deploy/cli.py
--rw-r--r--   0 fabian     (501) staff       (20)     2401 2023-05-09 12:45:13.000000 api-deploy-0.1.0/api_deploy/client.py
--rw-r--r--   0 fabian     (501) staff       (20)     1119 2023-05-09 12:12:46.000000 api-deploy-0.1.0/api_deploy/config.py
--rw-r--r--   0 fabian     (501) staff       (20)    12746 2023-05-09 10:31:27.000000 api-deploy-0.1.0/api_deploy/converters.py
--rw-r--r--   0 fabian     (501) staff       (20)     1075 2023-05-09 14:24:00.000000 api-deploy-0.1.0/api_deploy/schema.py
-drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-05-09 14:24:18.079816 api-deploy-0.1.0/api_deploy.egg-info/
--rw-r--r--   0 fabian     (501) staff       (20)      740 2023-05-09 14:24:18.000000 api-deploy-0.1.0/api_deploy.egg-info/PKG-INFO
--rw-r--r--   0 fabian     (501) staff       (20)      386 2023-05-09 14:24:18.000000 api-deploy-0.1.0/api_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 fabian     (501) staff       (20)        1 2023-05-09 14:24:18.000000 api-deploy-0.1.0/api_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 fabian     (501) staff       (20)       44 2023-05-09 14:24:18.000000 api-deploy-0.1.0/api_deploy.egg-info/entry_points.txt
--rw-r--r--   0 fabian     (501) staff       (20)        1 2022-12-17 05:34:25.000000 api-deploy-0.1.0/api_deploy.egg-info/not-zip-safe
--rw-r--r--   0 fabian     (501) staff       (20)       61 2023-05-09 14:24:18.000000 api-deploy-0.1.0/api_deploy.egg-info/requires.txt
--rw-r--r--   0 fabian     (501) staff       (20)       11 2023-05-09 14:24:18.000000 api-deploy-0.1.0/api_deploy.egg-info/top_level.txt
--rw-r--r--   0 fabian     (501) staff       (20)       38 2023-05-09 14:24:18.080137 api-deploy-0.1.0/setup.cfg
--rw-r--r--   0 fabian     (501) staff       (20)     1366 2023-05-09 12:32:53.000000 api-deploy-0.1.0/setup.py
+drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-05-10 15:16:57.872376 api-deploy-0.3.0/
+-rw-r--r--   0 fabian     (501) staff       (20)      740 2023-05-10 15:16:57.872247 api-deploy-0.3.0/PKG-INFO
+-rw-r--r--   0 fabian     (501) staff       (20)       12 2022-12-17 05:34:22.000000 api-deploy-0.3.0/README.md
+drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-05-10 15:16:57.870891 api-deploy-0.3.0/api_deploy/
+-rw-r--r--   0 fabian     (501) staff       (20)       18 2023-05-10 15:14:53.000000 api-deploy-0.3.0/api_deploy/__init__.py
+-rw-r--r--   0 fabian     (501) staff       (20)     2806 2023-05-09 14:47:12.000000 api-deploy-0.3.0/api_deploy/cli.py
+-rw-r--r--   0 fabian     (501) staff       (20)     2400 2023-05-09 14:47:12.000000 api-deploy-0.3.0/api_deploy/client.py
+-rw-r--r--   0 fabian     (501) staff       (20)     1143 2023-05-09 14:47:12.000000 api-deploy-0.3.0/api_deploy/config.py
+-rw-r--r--   0 fabian     (501) staff       (20)    13055 2023-05-10 15:14:53.000000 api-deploy-0.3.0/api_deploy/converters.py
+-rw-r--r--   0 fabian     (501) staff       (20)     1075 2023-05-09 14:47:12.000000 api-deploy-0.3.0/api_deploy/schema.py
+drwxr-xr-x   0 fabian     (501) staff       (20)        0 2023-05-10 15:16:57.872081 api-deploy-0.3.0/api_deploy.egg-info/
+-rw-r--r--   0 fabian     (501) staff       (20)      740 2023-05-10 15:16:57.000000 api-deploy-0.3.0/api_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 fabian     (501) staff       (20)      386 2023-05-10 15:16:57.000000 api-deploy-0.3.0/api_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabian     (501) staff       (20)        1 2023-05-10 15:16:57.000000 api-deploy-0.3.0/api_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabian     (501) staff       (20)       44 2023-05-10 15:16:57.000000 api-deploy-0.3.0/api_deploy.egg-info/entry_points.txt
+-rw-r--r--   0 fabian     (501) staff       (20)        1 2022-12-17 05:34:25.000000 api-deploy-0.3.0/api_deploy.egg-info/not-zip-safe
+-rw-r--r--   0 fabian     (501) staff       (20)       61 2023-05-10 15:16:57.000000 api-deploy-0.3.0/api_deploy.egg-info/requires.txt
+-rw-r--r--   0 fabian     (501) staff       (20)       11 2023-05-10 15:16:57.000000 api-deploy-0.3.0/api_deploy.egg-info/top_level.txt
+-rw-r--r--   0 fabian     (501) staff       (20)       38 2023-05-10 15:16:57.872413 api-deploy-0.3.0/setup.cfg
+-rw-r--r--   0 fabian     (501) staff       (20)     1366 2023-05-09 14:47:12.000000 api-deploy-0.3.0/setup.py
```

### Comparing `api-deploy-0.1.0/PKG-INFO` & `api-deploy-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: api-deploy
-Version: 0.1.0
+Version: 0.3.0
 Summary: Manage Amazon REST API Gateway deployments
 Home-page: https://github.com/fabfuel/api-deploy
 Author: Fabian Fuelling
 Author-email: pypi@fabfuel.de
 License: BSD-3-Clause
-Download-URL: https://github.com/fabfuel/api-deploy/archive/0.1.0.tar.gz
+Download-URL: https://github.com/fabfuel/api-deploy/archive/0.3.0.tar.gz
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
```

### Comparing `api-deploy-0.1.0/api_deploy/cli.py` & `api-deploy-0.3.0/api_deploy/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,25 @@
 @click.argument('source_file')
 @click.option('--region', required=False, help='AWS region (e.g. eu-central-1)')
 @click.option('--access-key-id', required=False, help='AWS access key id')
 @click.option('--secret-access-key', required=False, help='AWS secret access key')
 @click.option('--profile', required=False, help='AWS configuration profile name')
 @click.option('--account', required=False, help='Target AWS account id to deploy in')
 @click.option('--assume-role', required=False, help='AWS Role to assume in target account')
-def deploy(config_file, api_id, stage_name, source_file, region, access_key_id, secret_access_key, profile, account, assume_role):
+def deploy(config_file,
+           api_id,
+           stage_name,
+           source_file,
+           region,
+           access_key_id,
+           secret_access_key,
+           profile,
+           account,
+           assume_role,
+           ):
     client = _get_client(access_key_id, secret_access_key, region, profile, account, assume_role)
     config = Config.from_file(config_file)
 
     click.secho(f'Deploying API "{api_id}", stage "{stage_name}"\n')
     click.secho(f'Compiling OpenAPI file: "{source_file}"')
 
     source_schema = Schema.from_file(source_file)
```

### Comparing `api-deploy-0.1.0/api_deploy/client.py` & `api-deploy-0.3.0/api_deploy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,7 @@
         )
 
     def deploy_to_stage(self, api_id: str, stage_name: str):
         self.boto.create_deployment(
             restApiId=api_id,
             stageName=stage_name
         )
-
```

### Comparing `api-deploy-0.1.0/api_deploy/config.py` & `api-deploy-0.3.0/api_deploy/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from typing import TextIO, Dict
-import yaml
-
+from typing import Dict
 from api_deploy.schema import YamlDict
 
 
 class ConfigFile(YamlDict):
     ...
 
 
@@ -17,15 +15,16 @@
             },
             'gateway': {},
             'cors': {},
         }
         default_config['headers']['request'] = config_file.get('headers', {}).get('request', [])
         default_config['headers']['response'] = config_file.get('headers', {}).get('response', [])
 
-        default_config['gateway'].setdefault('integration_host', config_file.get('gateway', {}).get('integrationHost', ''))
+        default_config['gateway'].setdefault('integration_host',
+                                             config_file.get('gateway', {}).get('integrationHost', ''))
         default_config['gateway'].setdefault('connection_id', config_file.get('gateway', {}).get('connectionId', ''))
 
         default_config['cors'].setdefault('allow_origin', config_file.get('cors', {}).get('origin', '*'))
 
         super().__init__(default_config)
 
     @classmethod
```

### Comparing `api-deploy-0.1.0/api_deploy/converters.py` & `api-deploy-0.3.0/api_deploy/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,19 +185,26 @@
         parameters = {
             'integration.request.header.User-Agent': 'context.identity.userAgent',
             'integration.request.header.X-Forwarded-For': 'context.identity.sourceIp',
             'integration.request.header.X-Stage': 'context.stage',
         }
 
         for parameter in schema['paths'][path][method].get('parameters', []):
-            source = parameter.get('in')
-            if source == 'query':
-                source = 'querystring'
+            source_integration = parameter.get('in')
+            source_method = parameter.get('in')
+
+            if parameter.get('in') == 'query':
+                source_integration = 'querystring'
+                if parameter.get('schema', {}).get('type') == 'array':
+                    source_method = 'multivaluequerystring'
+                else:
+                    source_method = 'querystring'
+
             name = parameter.get('name')
-            parameters[f'integration.request.{source}.{name}'] = f'method.request.{source}.{name}'
+            parameters[f'integration.request.{source_integration}.{name}'] = f'method.request.{source_method}.{name}'
 
         return parameters
 
 
 class CorsProcessor(AbstractProcessor):
     def __init__(self, headers, allow_origin, **kwargs) -> None:
         super().__init__()
```

### Comparing `api-deploy-0.1.0/api_deploy/schema.py` & `api-deploy-0.3.0/api_deploy/schema.py`

 * *Files identical despite different names*

### Comparing `api-deploy-0.1.0/api_deploy.egg-info/PKG-INFO` & `api-deploy-0.3.0/api_deploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: api-deploy
-Version: 0.1.0
+Version: 0.3.0
 Summary: Manage Amazon REST API Gateway deployments
 Home-page: https://github.com/fabfuel/api-deploy
 Author: Fabian Fuelling
 Author-email: pypi@fabfuel.de
 License: BSD-3-Clause
-Download-URL: https://github.com/fabfuel/api-deploy/archive/0.1.0.tar.gz
+Download-URL: https://github.com/fabfuel/api-deploy/archive/0.3.0.tar.gz
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
```

### Comparing `api-deploy-0.1.0/setup.py` & `api-deploy-0.3.0/setup.py`

 * *Files identical despite different names*

