# Comparing `tmp/ecsmgmt_cli-0.4.5.tar.gz` & `tmp/ecsmgmt_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecsmgmt_cli-0.4.5.tar", max compression
+gzip compressed data, was "ecsmgmt_cli-0.5.0.tar", max compression
```

## Comparing `ecsmgmt_cli-0.4.5.tar` & `ecsmgmt_cli-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0    16725 2022-12-27 14:49:23.886876 ecsmgmt_cli-0.4.5/LICENSE
--rw-r--r--   0        0        0      641 2022-12-27 18:59:11.069238 ecsmgmt_cli-0.4.5/README.md
--rw-r--r--   0        0        0     1435 2022-12-27 19:06:37.707168 ecsmgmt_cli-0.4.5/ecsmgmt/__init__.py
--rw-r--r--   0        0        0        0 2022-12-27 14:49:23.890876 ecsmgmt_cli-0.4.5/ecsmgmt/_util/__init__.py
--rw-r--r--   0        0        0     1474 2023-01-06 04:26:27.388254 ecsmgmt_cli-0.4.5/ecsmgmt/_util/config.py
--rw-r--r--   0        0        0       85 2022-12-27 14:49:23.890876 ecsmgmt_cli-0.4.5/ecsmgmt/_util/const.py
--rw-r--r--   0        0        0     2704 2022-12-27 19:06:37.707168 ecsmgmt_cli-0.4.5/ecsmgmt/_util/core.py
--rw-r--r--   0        0        0      128 2022-12-27 14:49:23.890876 ecsmgmt_cli-0.4.5/ecsmgmt/_util/echo.py
--rw-r--r--   0        0        0      447 2022-12-27 14:49:23.890876 ecsmgmt_cli-0.4.5/ecsmgmt/_util/exceptions.py
--rw-r--r--   0        0        0      705 2022-12-27 19:06:37.707168 ecsmgmt_cli-0.4.5/ecsmgmt/_util/format.py
--rw-r--r--   0        0        0     1210 2022-12-27 19:06:37.707168 ecsmgmt_cli-0.4.5/ecsmgmt/_util/types.py
--rw-r--r--   0        0        0      246 2022-12-27 14:49:23.890876 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/__init__.py
--rw-r--r--   0        0        0      247 2022-12-27 14:49:23.890876 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/acl/__init__.py
--rw-r--r--   0        0        0      495 2022-12-27 19:06:37.707168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/acl/get.py
--rw-r--r--   0        0        0     2127 2022-12-27 19:06:37.707168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/acl/set.py
--rw-r--r--   0        0        0      761 2022-12-27 19:06:37.707168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/chown.py
--rw-r--r--   0        0        0     1016 2022-12-27 19:06:37.707168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/create.py
--rw-r--r--   0        0        0      673 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/delete.py
--rw-r--r--   0        0        0      495 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/get.py
--rw-r--r--   0        0        0      574 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/list.py
--rw-r--r--   0        0        0      259 2022-12-27 14:49:23.890876 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/retention/__init__.py
--rw-r--r--   0        0        0      513 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/retention/get.py
--rw-r--r--   0        0        0      790 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/bucket/retention/set.py
--rw-r--r--   0        0        0      307 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/get_acl_permissions.py
--rw-r--r--   0        0        0      254 2022-12-27 14:49:23.890876 ecsmgmt_cli-0.4.5/ecsmgmt/secret_key/__init__.py
--rw-r--r--   0        0        0     1436 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/secret_key/create.py
--rw-r--r--   0        0        0     2434 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/secret_key/delete.py
--rw-r--r--   0        0        0     1220 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/secret_key/list.py
--rw-r--r--   0        0        0      249 2022-12-27 14:49:23.894876 ecsmgmt_cli-0.4.5/ecsmgmt/user/__init__.py
--rw-r--r--   0        0        0      969 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/user/create.py
--rw-r--r--   0        0        0      645 2022-12-27 19:06:37.711168 ecsmgmt_cli-0.4.5/ecsmgmt/user/delete.py
--rw-r--r--   0        0        0      476 2022-12-27 19:06:37.715169 ecsmgmt_cli-0.4.5/ecsmgmt/user/get.py
--rw-r--r--   0        0        0      538 2022-12-27 19:06:37.715169 ecsmgmt_cli-0.4.5/ecsmgmt/user/list.py
--rw-r--r--   0        0        0     1942 2023-01-06 04:26:27.388254 ecsmgmt_cli-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 ecsmgmt_cli-0.4.5/setup.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 ecsmgmt_cli-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0      641 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.5.0/README.md
+-rw-r--r--   0        0        0     1611 2023-05-10 01:03:02.448024 ecsmgmt_cli-0.5.0/ecsmgmt/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/__init__.py
+-rw-r--r--   0        0        0     1111 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/callbacks.py
+-rw-r--r--   0        0        0       85 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/const.py
+-rw-r--r--   0        0        0     2704 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/core.py
+-rw-r--r--   0        0        0      128 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/echo.py
+-rw-r--r--   0        0        0      447 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/exceptions.py
+-rw-r--r--   0        0        0      705 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/format.py
+-rw-r--r--   0        0        0     1210 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/_util/types.py
+-rw-r--r--   0        0        0      246 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/__init__.py
+-rw-r--r--   0        0        0      247 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/acl/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/acl/get.py
+-rw-r--r--   0        0        0     2071 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/acl/set.py
+-rw-r--r--   0        0        0      705 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/chown.py
+-rw-r--r--   0        0        0      960 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/create.py
+-rw-r--r--   0        0        0      617 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/delete.py
+-rw-r--r--   0        0        0      439 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/get.py
+-rw-r--r--   0        0        0      518 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/list.py
+-rw-r--r--   0        0        0      259 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/retention/__init__.py
+-rw-r--r--   0        0        0      457 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/retention/get.py
+-rw-r--r--   0        0        0      734 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/bucket/retention/set.py
+-rw-r--r--   0        0        0      307 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/get_acl_permissions.py
+-rw-r--r--   0        0        0      254 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/__init__.py
+-rw-r--r--   0        0        0     1350 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/create.py
+-rw-r--r--   0        0        0     2348 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/delete.py
+-rw-r--r--   0        0        0     1164 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/list.py
+-rw-r--r--   0        0        0      249 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/create.py
+-rw-r--r--   0        0        0      589 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/delete.py
+-rw-r--r--   0        0        0      420 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/get.py
+-rw-r--r--   0        0        0      482 2023-05-10 01:03:02.452024 ecsmgmt_cli-0.5.0/ecsmgmt/user/list.py
+-rw-r--r--   0        0        0     1942 2023-05-10 01:06:15.288843 ecsmgmt_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 ecsmgmt_cli-0.5.0/PKG-INFO
```

### Comparing `ecsmgmt_cli-0.4.5/LICENSE` & `ecsmgmt_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.4.5/README.md` & `ecsmgmt_cli-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/__init__.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import os.path
 import pathlib
 
 import click
 from ecsclient.client import Client
 
-from ._util.config import load_config
+from ._util.callbacks import config_callback, namespace_callback
 from ._util.const import CONTEXT_SETTINGS
 from ._util.core import DynamicMultiCommandFactory
 
 DynamicMultiCommand = DynamicMultiCommandFactory().create(__file__, __package__)
 
 
 @click.command(cls=DynamicMultiCommand, context_settings=CONTEXT_SETTINGS)
 @click.option(
     '-c', '--config', 'config_path',
     type=click.Path(dir_okay=False, path_type=pathlib.Path),
     default=os.path.join(click.get_app_dir('ecsmgmt-cli'), 'config.yml'),
     help='Configuration file in YAML format',
-    callback=load_config,
+    callback=config_callback,
     is_eager=True,
     expose_value=False,
     show_default=True,
 )
 @click.option(
+    '-n', '--namespace',
+    type=click.STRING,
+    callback=namespace_callback,
+    expose_value=False,
+    show_default=True,
+)
+@click.option(
     '-u', '--username',
     type=click.STRING,
     prompt=True,
     show_default=True,
 )
 @click.option(
     '-p', '--password',
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/_util/core.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/_util/core.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/_util/format.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/_util/format.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/_util/types.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/_util/types.py`

 * *Files identical despite different names*

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/bucket/acl/set.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/acl/set.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from ..._util.echo import success
 from ..._util.exceptions import EcsmgmtClickException
 from ..._util.format import IndentedListDumper
 
 
 @click.command()
 @click.argument('bucket-name', type=click.STRING)
-@click.option('-n', '--namespace', type=click.STRING, show_default=True)
 @click.pass_obj
-def cli(obj: dict, bucket_name: str, namespace: str):
+def cli(obj: dict, bucket_name: str):
     """Set bucket acl
 
     **This command is only for advanced users!**
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     acl_get = client.bucket.get_acl(bucket_name=bucket_name, namespace=namespace)
     acl_before = acl_get['acl']
     # removing to supported values
     acl_before.pop('default_group_dir_perms')
     acl_before.pop('default_group_file_perms')
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/bucket/chown.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/chown.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from .._util.echo import success
 from .._util.exceptions import EcsmgmtClickException
 
 
 @click.command()
 @click.argument('bucket-name', type=click.STRING)
 @click.argument('user-id', type=click.STRING)
-@click.option('-n', '--namespace', type=click.STRING, show_default=True)
 @click.pass_obj
-def cli(obj: dict, bucket_name: str, user_id: str, namespace: str):
+def cli(obj: dict, bucket_name: str, user_id: str):
     """Change owner of bucket
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     try:
         client.bucket.set_owner(bucket_name=bucket_name, new_owner=user_id, namespace=namespace)
         success(f'changed owner of bucket "{bucket_name}" to "{user_id}"')
     except ECSClientException as e:
         raise EcsmgmtClickException(e.message)
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/bucket/create.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/create.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from .._util.echo import success
 from .._util.exceptions import EcsmgmtClickException
 
 
 @click.command()
 @click.argument('bucket-name', type=click.STRING)
-@click.option('-n', '--namespace', type=click.STRING, show_default=True)
 @click.pass_obj
-def cli(obj: dict, bucket_name: str, namespace: str):
+def cli(obj: dict, bucket_name: str):
     """Create bucket
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     if len(bucket_name) > 255:
         raise EcsmgmtClickException('Bucket name too long. Maximum allowed length is 255 chars.')
     if not all(x.isalnum() or x == '.' or x == '-' or x == '_' for x in bucket_name):
         raise EcsmgmtClickException('Bucket name contains invalid characters. Only alphanumeric, ".", "-" or "_" is allowed.')
 
     try:
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/bucket/delete.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/delete.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 from .._util.echo import success
 from .._util.exceptions import EcsmgmtClickException
 
 
 @click.command()
 @click.argument('bucket-name', type=click.STRING)
-@click.option('-n', '--namespace', type=click.STRING, show_default=True)
 @click.pass_obj
-def cli(obj: dict, bucket_name: str, namespace: str):
+def cli(obj: dict, bucket_name: str):
     """Delete bucket
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     try:
         client.bucket.delete(bucket_name=bucket_name, namespace=namespace)
         success(f'deleted bucket "{bucket_name}" in namespace "{namespace}"')
     except ECSClientException as e:
         raise EcsmgmtClickException(e.message)
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/bucket/list.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import click
 
 from .._util.format import pretty_table
 
 
 @click.command()
-@click.option('-n', '--namespace', type=click.STRING, show_default=True)
 @click.pass_obj
-def cli(obj: dict, namespace: str):
+def cli(obj: dict):
     """List all buckets in namespace
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     bucket_request = client.bucket.list(namespace=namespace)
     bucket_list = [(bucket['namespace'], bucket['name'], bucket['owner']) for bucket in bucket_request['object_bucket']]
     headers = ['Namespace', 'Bucket Name', 'Owner']
     table = pretty_table(bucket_list, headers)
     click.echo(table)
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/bucket/retention/set.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/bucket/retention/set.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from ..._util.echo import success
 from ..._util.exceptions import EcsmgmtClickException
 
 
 @click.command()
 @click.argument('bucket-name', type=click.STRING)
 @click.argument('period', type=types.TIME)
-@click.option('-n', '--namespace', type=click.STRING, show_default=True)
 @click.pass_obj
-def cli(obj: dict, bucket_name: str, period: int, namespace: str):
+def cli(obj: dict, bucket_name: str, period: int):
     """Set bucket retention
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     try:
         client.bucket.set_retention(bucket_name=bucket_name, namespace=namespace, period=period)
         success(f'Set retention for bucket "{bucket_name}" to {period} seconds')
     except ECSClientException as e:
         raise EcsmgmtClickException(e.message)
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/secret_key/create.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/create.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from .._util.echo import success
 from .._util.exceptions import EcsmgmtClickException
 from .._util.format import pretty_table
 
 
 @click.command()
 @click.argument('user-id')
-@click.option('-n', '--namespace', type=click.STRING, show_default=True, help='Namespace of the user')
 @click.option('-e', '--expiry-time', type=click.INT, help='Expiry time in minutes for the previous secret key.')
 @click.option('-k', '--secret-key', type=click.STRING, help='Provide secret key instead of generating one.')
 @click.pass_obj
-def cli(obj: dict, user_id: str, namespace: str, expiry_time: int, secret_key: str):
+def cli(obj: dict, user_id: str, expiry_time: int, secret_key: str):
     """Create new secret key
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     try:
         res = client.secret_key.create(user_id=user_id, namespace=namespace, expiry_time=expiry_time,
                                        secret_key=secret_key)
         data = [
             ('Secret Key:', res['secret_key']),
         ]
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/secret_key/delete.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from .._util.echo import success
 from .._util.exceptions import EcsmgmtClickException
 
 
 @click.command()
 @click.argument('user-id')
-@click.option('-n', '--namespace', type=click.STRING, show_default=True, help='Namespace of the user')
 @click.option('-k', '--secret-key', type=click.STRING, help='Secret key which should get deleted')
 @click.pass_obj
-def cli(obj: dict, user_id: str, namespace: str, secret_key: str):
+def cli(obj: dict, user_id: str, secret_key: str):
     """Deletes secret key
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     res = client.secret_key.get(user_id=user_id, namespace=namespace)
     existing_secret_keys = []
     for i in [1, 2]:
         if res[f'secret_key_{i}_exist']:
             existing_secret_keys.append(res[f'secret_key_{i}'])
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/secret_key/list.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/secret_key/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from .._util.echo import success
 from .._util.format import pretty_table
 
 
 @click.command()
 @click.argument('user-id')
-@click.option('-n', '--namespace', type=click.STRING, show_default=True)
 @click.pass_obj
-def cli(obj: dict, user_id: str, namespace: str):
+def cli(obj: dict, user_id: str):
     """Get a users secret key
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     res = client.secret_key.get(user_id=user_id, namespace=namespace)
     data = []
     for i in [1, 2]:
         if res[f'secret_key_{i}_exist']:
             if res[f'key_expiry_timestamp_{i}'] != '':
                 timestamp = datetime.datetime.fromisoformat(res[f'key_expiry_timestamp_{i}'] + '+00:00')
```

### Comparing `ecsmgmt_cli-0.4.5/ecsmgmt/user/create.py` & `ecsmgmt_cli-0.5.0/ecsmgmt/user/create.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 from .._util.echo import success
 from .._util.exceptions import EcsmgmtClickException
 
 
 @click.command()
 @click.argument('user-id', type=click.STRING)
-@click.option('-n', '--namespace', type=click.STRING, show_default=True)
 @click.option(
     '-t', '--tag', 'tags',
     multiple=True,
     type=click.STRING,
     help='User tags seperated by ",", option can be provided multiple times'
 )
 @click.pass_obj
-def cli(obj: dict, user_id: str, namespace: str, tags: list[str]):
+def cli(obj: dict, user_id: str, tags: list[str]):
     """Create new object user
     """
     client = obj['client']
+    namespace = obj['namespace']
 
     sane_tags = []
     for tag in tags:
         splited = tag.split(',')
         sane_tags.extend(splited)
 
     try:
```

### Comparing `ecsmgmt_cli-0.4.5/pyproject.toml` & `ecsmgmt_cli-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecsmgmt-cli"
-version = "0.4.5"
+version = "0.5.0"
 description = "Small CLI tool for interacting with the ECS Management API"
 authors = ["Dominik Rimpf <dev@drimpf.de>"]
 license = "MPL-2.0"
 
 readme = "README.md"
 repository = "https://gitlab.com/domrim/ecsmgmt-cli"
 homepage = "https://gitlab.com/domrim/ecsmgmt-cli"
@@ -24,15 +24,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-ecsclient = "^1.1.12"
 click = "^8.1.3"
 PyYAML = "^6.0"
 tabulate = "^0.9.0"
-inquirer = "^3.1.1"
+inquirer = "^3.1.3"
 
 [tool.poetry.group.lint.dependencies]
 bandit = {extras = ["toml"], version = "^1.7.4"}
 flake8 = "^6.0.0"
 flake8-annotations = "^2.9.1"
 flake8-pep585 = "^0.1.6"
 flake8-pyproject = "^1.2.2" # until flake8 gets its shit together...
```

### Comparing `ecsmgmt_cli-0.4.5/PKG-INFO` & `ecsmgmt_cli-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecsmgmt-cli
-Version: 0.4.5
+Version: 0.5.0
 Summary: Small CLI tool for interacting with the ECS Management API
 Home-page: https://gitlab.com/domrim/ecsmgmt-cli
 License: MPL-2.0
 Author: Dominik Rimpf
 Author-email: dev@drimpf.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: inquirer (>=3.1.1,<4.0.0)
+Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: python-ecsclient (>=1.1.12,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://gitlab.com/domrim/ecsmgmt-cli
 Description-Content-Type: text/markdown
 
 # ecsmgmt-cli
```

