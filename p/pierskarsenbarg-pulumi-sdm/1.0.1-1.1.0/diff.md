# Comparing `tmp/pierskarsenbarg_pulumi_sdm-1.0.1.tar.gz` & `tmp/pierskarsenbarg_pulumi_sdm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.0.1.tar", last modified: Wed Apr 12 13:12:11 2023, max compression
+gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.1.0.tar", last modified: Wed May 10 09:14:09 2023, max compression
```

## Comparing `pierskarsenbarg_pulumi_sdm-1.0.1.tar` & `pierskarsenbarg_pulumi_sdm-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   769508 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/account_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/node.py
--rw-r--r--   0 runner    (1001) docker     (123)  1110292 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)   145518 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/secret_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 13:12:11.000000 pierskarsenbarg_pulumi_sdm-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   786688 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/account_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1132822 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146818 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/secret_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-10 09:14:09.000000 pierskarsenbarg_pulumi_sdm-1.1.0/setup.py
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pierskarsenbarg_pulumi_sdm
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
@@ -65,8 +65,9 @@
         
         <!-- ## Reference
         
         For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/). -->
         
 Keywords: pulumi sdm category/cloud
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/README.md` & `pierskarsenbarg_pulumi_sdm-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/__init__.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/_inputs.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     'ResourceSqlServerArgs',
     'ResourceSshArgs',
     'ResourceSshCertArgs',
     'ResourceSshCustomerKeyArgs',
     'ResourceSybaseArgs',
     'ResourceSybaseIqArgs',
     'ResourceTeradataArgs',
+    'ResourceTrinoArgs',
     'SecretStoreAwsArgs',
     'SecretStoreAzureStoreArgs',
     'SecretStoreCyberarkConjurArgs',
     'SecretStoreCyberarkPamArgs',
     'SecretStoreCyberarkPamExperimentalArgs',
     'SecretStoreDelineaStoreArgs',
     'SecretStoreGcpStoreArgs',
@@ -867,14 +868,15 @@
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
@@ -1017,14 +1019,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -3291,14 +3296,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -3430,14 +3436,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -3491,16 +3500,16 @@
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
 class ResourceAthenaArgs:
     def __init__(__self__, *,
+                 athena_output: pulumi.Input[str],
                  name: pulumi.Input[str],
-                 output: pulumi.Input[str],
                  access_key: Optional[pulumi.Input[str]] = None,
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  role_external_id: Optional[pulumi.Input[str]] = None,
@@ -3520,16 +3529,16 @@
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
+        pulumi.set(__self__, "athena_output", athena_output)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "output", output)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if port_override is not None:
@@ -3562,35 +3571,35 @@
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
         if subdomain is not None:
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
+    @pulumi.getter(name="athenaOutput")
+    def athena_output(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "athena_output")
+
+    @athena_output.setter
+    def athena_output(self, value: pulumi.Input[str]):
+        pulumi.set(self, "athena_output", value)
+
+    @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def output(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "output")
-
-    @output.setter
-    def output(self, value: pulumi.Input[str]):
-        pulumi.set(self, "output", value)
-
-    @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "access_key")
 
     @access_key.setter
     def access_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_key", value)
@@ -3793,14 +3802,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -3940,14 +3950,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -4014,14 +4027,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -4172,14 +4186,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -4229,42 +4246,47 @@
 class ResourceAwsArgs:
     def __init__(__self__, *,
                  healthcheck_region: pulumi.Input[str],
                  name: pulumi.Input[str],
                  access_key: Optional[pulumi.Input[str]] = None,
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  role_external_id: Optional[pulumi.Input[str]] = None,
                  secret_access_key: Optional[pulumi.Input[str]] = None,
                  secret_store_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_access_key_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_region", healthcheck_region)
         pulumi.set(__self__, "name", name)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if role_arn is not None:
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_access_key_key is not None:
@@ -4281,14 +4303,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="healthcheckRegion")
     def healthcheck_region(self) -> pulumi.Input[str]:
         return pulumi.get(self, "healthcheck_region")
@@ -4339,14 +4363,23 @@
         return pulumi.get(self, "egress_filter")
 
     @egress_filter.setter
     def egress_filter(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "egress_filter", value)
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "role_arn")
 
     @role_arn.setter
     def role_arn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_arn", value)
@@ -4451,14 +4484,26 @@
 
     @secret_store_secret_access_key_path.setter
     def secret_store_secret_access_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_secret_access_key_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -5018,54 +5063,61 @@
 class ResourceAzureArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  app_id: Optional[pulumi.Input[str]] = None,
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_app_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_app_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_tenant_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_tenant_id_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] secret_store_tenant_id_key: * azure_mysql:
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_app_id_key is not None:
             pulumi.set(__self__, "secret_store_app_id_key", secret_store_app_id_key)
         if secret_store_app_id_path is not None:
             pulumi.set(__self__, "secret_store_app_id_path", secret_store_app_id_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_tenant_id_key is not None:
             pulumi.set(__self__, "secret_store_tenant_id_key", secret_store_tenant_id_key)
         if secret_store_tenant_id_path is not None:
             pulumi.set(__self__, "secret_store_tenant_id_path", secret_store_tenant_id_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter
@@ -5118,14 +5170,23 @@
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
     @pulumi.getter(name="secretStoreAppIdKey")
     def secret_store_app_id_key(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "secret_store_app_id_key")
 
     @secret_store_app_id_key.setter
     def secret_store_app_id_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_app_id_key", value)
@@ -5188,14 +5249,26 @@
 
     @secret_store_tenant_id_path.setter
     def secret_store_tenant_id_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_tenant_id_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -5216,54 +5289,61 @@
 class ResourceAzureCertificateArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  app_id: Optional[pulumi.Input[str]] = None,
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  client_certificate: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_app_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_app_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_tenant_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_tenant_id_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] secret_store_tenant_id_key: * azure_mysql:
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if client_certificate is not None:
             pulumi.set(__self__, "client_certificate", client_certificate)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_app_id_key is not None:
             pulumi.set(__self__, "secret_store_app_id_key", secret_store_app_id_key)
         if secret_store_app_id_path is not None:
             pulumi.set(__self__, "secret_store_app_id_path", secret_store_app_id_path)
         if secret_store_client_certificate_key is not None:
             pulumi.set(__self__, "secret_store_client_certificate_key", secret_store_client_certificate_key)
         if secret_store_client_certificate_path is not None:
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_tenant_id_key is not None:
             pulumi.set(__self__, "secret_store_tenant_id_key", secret_store_tenant_id_key)
         if secret_store_tenant_id_path is not None:
             pulumi.set(__self__, "secret_store_tenant_id_path", secret_store_tenant_id_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter
@@ -5316,14 +5396,23 @@
         return pulumi.get(self, "egress_filter")
 
     @egress_filter.setter
     def egress_filter(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "egress_filter", value)
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
     @pulumi.getter(name="secretStoreAppIdKey")
     def secret_store_app_id_key(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "secret_store_app_id_key")
 
     @secret_store_app_id_key.setter
     def secret_store_app_id_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_app_id_key", value)
@@ -5386,14 +5475,26 @@
 
     @secret_store_tenant_id_path.setter
     def secret_store_tenant_id_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_tenant_id_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -5430,14 +5531,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -5577,14 +5679,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -5651,14 +5756,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -5809,14 +5915,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -6066,14 +6175,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -6205,14 +6315,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -6288,14 +6401,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -6446,14 +6560,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -6519,14 +6636,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -6666,14 +6784,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -6740,14 +6861,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -6898,14 +7020,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -6971,14 +7096,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
@@ -7109,14 +7235,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -7191,14 +7320,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -7338,14 +7468,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -7411,14 +7544,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -7558,14 +7692,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -7632,14 +7769,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
@@ -7789,14 +7927,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -7861,14 +8002,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -7998,14 +8140,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -8351,14 +8496,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8490,14 +8636,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -8572,14 +8721,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8711,14 +8861,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -8777,39 +8930,46 @@
 class ResourceGcpArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  scopes: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  keyfile: Optional[pulumi.Input[str]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_keyfile_key: Optional[pulumi.Input[str]] = None,
                  secret_store_keyfile_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "scopes", scopes)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if keyfile is not None:
             pulumi.set(__self__, "keyfile", keyfile)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_keyfile_key is not None:
             pulumi.set(__self__, "secret_store_keyfile_key", secret_store_keyfile_key)
         if secret_store_keyfile_path is not None:
             pulumi.set(__self__, "secret_store_keyfile_path", secret_store_keyfile_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
@@ -8860,14 +9020,23 @@
         return pulumi.get(self, "keyfile")
 
     @keyfile.setter
     def keyfile(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keyfile", value)
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[pulumi.Input[str]]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
@@ -8891,14 +9060,26 @@
 
     @secret_store_keyfile_path.setter
     def secret_store_keyfile_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_keyfile_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -9353,14 +9534,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -9511,14 +9693,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -9786,14 +9971,15 @@
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[str] url: * kubernetes:
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "subdomain", subdomain)
         pulumi.set(__self__, "url", url)
         if bind_interface is not None:
@@ -9957,14 +10143,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -10466,14 +10655,15 @@
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
@@ -10616,14 +10806,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -11357,14 +11550,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -11504,14 +11698,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -11714,14 +11911,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -11861,14 +12059,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -11935,14 +12136,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -12084,14 +12286,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -12168,14 +12373,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -12328,14 +12534,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -12413,14 +12622,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
@@ -12583,14 +12793,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -12668,14 +12881,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
@@ -12838,14 +13052,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -12920,14 +13137,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -13058,14 +13276,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -13150,14 +13371,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -13398,14 +13620,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -13491,14 +13716,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -13750,14 +13976,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -13832,14 +14061,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -13979,14 +14209,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -14482,14 +14715,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
@@ -14630,14 +14864,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -14713,14 +14950,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -14871,14 +15109,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -15152,14 +15393,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -15291,14 +15533,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -15510,14 +15755,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -15658,14 +15904,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -15731,14 +15980,15 @@
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -15870,14 +16120,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -15953,14 +16206,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -16111,14 +16365,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -16184,14 +16441,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -16331,14 +16589,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -16404,14 +16665,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -16551,14 +16813,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -16786,14 +17051,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -16955,14 +17221,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -17028,14 +17297,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
@@ -17175,14 +17445,17 @@
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -17249,14 +17522,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
@@ -17407,14 +17681,17 @@
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -17481,14 +17758,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
@@ -17639,14 +17917,17 @@
     @secret_store_private_key_path.setter
     def secret_store_private_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_private_key_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -17711,14 +17992,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -17848,14 +18130,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -17920,14 +18205,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -18057,14 +18343,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -18129,14 +18418,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] secret_store_username_key: * trino:
         :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -18266,14 +18556,17 @@
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @secret_store_username_key.setter
     def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_key", value)
 
     @property
@@ -18287,14 +18580,210 @@
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[pulumi.Input[str]]:
         """
         Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
+class ResourceTrinoArgs:
+    def __init__(__self__, *,
+                 database: pulumi.Input[str],
+                 hostname: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 bind_interface: Optional[pulumi.Input[str]] = None,
+                 egress_filter: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 port: Optional[pulumi.Input[int]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
+                 secret_store_id: Optional[pulumi.Input[str]] = None,
+                 secret_store_password_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_password_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] bind_interface: Bind interface
+        :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "database", database)
+        pulumi.set(__self__, "hostname", hostname)
+        pulumi.set(__self__, "name", name)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if secret_store_password_key is not None:
+            pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
+        if secret_store_password_path is not None:
+            pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def database(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "database")
+
+    @database.setter
+    def database(self, value: pulumi.Input[str]):
+        pulumi.set(self, "database", value)
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "hostname")
+
+    @hostname.setter
+    def hostname(self, value: pulumi.Input[str]):
+        pulumi.set(self, "hostname", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[pulumi.Input[str]]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @bind_interface.setter
+    def bind_interface(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "bind_interface", value)
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @egress_filter.setter
+    def egress_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "egress_filter", value)
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port", value)
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @secret_store_id.setter
+    def secret_store_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_id", value)
+
+    @property
+    @pulumi.getter(name="secretStorePasswordKey")
+    def secret_store_password_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_password_key")
+
+    @secret_store_password_key.setter
+    def secret_store_password_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_password_key", value)
+
+    @property
+    @pulumi.getter(name="secretStorePasswordPath")
+    def secret_store_password_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_password_path")
+
+    @secret_store_password_path.setter
+    def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_password_path", value)
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @subdomain.setter
     def subdomain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subdomain", value)
 
     @property
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/_utilities.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/_utilities.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/account.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/account.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/account_attachment.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/config/vars.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/config/vars.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_account.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_account.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_node.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_resource.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_resource.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_role.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_role.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/node.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/outputs.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     'ResourceSqlServer',
     'ResourceSsh',
     'ResourceSshCert',
     'ResourceSshCustomerKey',
     'ResourceSybase',
     'ResourceSybaseIq',
     'ResourceTeradata',
+    'ResourceTrino',
     'SecretStoreAws',
     'SecretStoreAzureStore',
     'SecretStoreCyberarkConjur',
     'SecretStoreCyberarkPam',
     'SecretStoreCyberarkPamExperimental',
     'SecretStoreDelineaStore',
     'SecretStoreGcpStore',
@@ -185,14 +186,15 @@
     'GetResourceResourceSqlServerResult',
     'GetResourceResourceSshResult',
     'GetResourceResourceSshCertResult',
     'GetResourceResourceSshCustomerKeyResult',
     'GetResourceResourceSybaseResult',
     'GetResourceResourceSybaseIqResult',
     'GetResourceResourceTeradataResult',
+    'GetResourceResourceTrinoResult',
     'GetRoleRoleResult',
     'GetSecretStoreSecretStoreResult',
     'GetSecretStoreSecretStoreAwResult',
     'GetSecretStoreSecretStoreAzureStoreResult',
     'GetSecretStoreSecretStoreCyberarkConjurResult',
     'GetSecretStoreSecretStoreCyberarkPamResult',
     'GetSecretStoreSecretStoreCyberarkPamExperimentalResult',
@@ -914,14 +916,15 @@
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
@@ -1020,14 +1023,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -3019,14 +3025,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -3118,14 +3125,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -3157,15 +3167,17 @@
 
 
 @pulumi.output_type
 class ResourceAthena(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "accessKey":
+        if key == "athenaOutput":
+            suggest = "athena_output"
+        elif key == "accessKey":
             suggest = "access_key"
         elif key == "bindInterface":
             suggest = "bind_interface"
         elif key == "egressFilter":
             suggest = "egress_filter"
         elif key == "portOverride":
             suggest = "port_override"
@@ -3202,16 +3214,16 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ResourceAthena.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
+                 athena_output: str,
                  name: str,
-                 output: str,
                  access_key: Optional[str] = None,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  port_override: Optional[int] = None,
                  region: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
@@ -3231,16 +3243,16 @@
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
+        pulumi.set(__self__, "athena_output", athena_output)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "output", output)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if port_override is not None:
@@ -3273,27 +3285,27 @@
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
         if subdomain is not None:
             pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
+    @pulumi.getter(name="athenaOutput")
+    def athena_output(self) -> str:
+        return pulumi.get(self, "athena_output")
+
+    @property
     @pulumi.getter
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def output(self) -> str:
-        return pulumi.get(self, "output")
-
-    @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
@@ -3451,14 +3463,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -3554,14 +3567,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -3641,14 +3657,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -3751,14 +3768,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -3793,14 +3813,16 @@
             suggest = "healthcheck_region"
         elif key == "accessKey":
             suggest = "access_key"
         elif key == "bindInterface":
             suggest = "bind_interface"
         elif key == "egressFilter":
             suggest = "egress_filter"
+        elif key == "portOverride":
+            suggest = "port_override"
         elif key == "roleArn":
             suggest = "role_arn"
         elif key == "roleExternalId":
             suggest = "role_external_id"
         elif key == "secretAccessKey":
             suggest = "secret_access_key"
         elif key == "secretStoreAccessKeyKey":
@@ -3835,42 +3857,47 @@
 
     def __init__(__self__, *,
                  healthcheck_region: str,
                  name: str,
                  access_key: Optional[str] = None,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_access_key_key: Optional[str] = None,
                  secret_store_access_key_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_role_arn_key: Optional[str] = None,
                  secret_store_role_arn_path: Optional[str] = None,
                  secret_store_role_external_id_key: Optional[str] = None,
                  secret_store_role_external_id_path: Optional[str] = None,
                  secret_store_secret_access_key_key: Optional[str] = None,
                  secret_store_secret_access_key_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_region", healthcheck_region)
         pulumi.set(__self__, "name", name)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if role_arn is not None:
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_access_key_key is not None:
@@ -3887,14 +3914,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="healthcheckRegion")
     def healthcheck_region(self) -> str:
         return pulumi.get(self, "healthcheck_region")
@@ -3925,14 +3954,19 @@
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
@@ -3989,14 +4023,22 @@
     @property
     @pulumi.getter(name="secretStoreSecretAccessKeyPath")
     def secret_store_secret_access_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_secret_access_key_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -4487,14 +4529,16 @@
         suggest = None
         if key == "appId":
             suggest = "app_id"
         elif key == "bindInterface":
             suggest = "bind_interface"
         elif key == "egressFilter":
             suggest = "egress_filter"
+        elif key == "portOverride":
+            suggest = "port_override"
         elif key == "secretStoreAppIdKey":
             suggest = "secret_store_app_id_key"
         elif key == "secretStoreAppIdPath":
             suggest = "secret_store_app_id_path"
         elif key == "secretStoreId":
             suggest = "secret_store_id"
         elif key == "secretStorePasswordKey":
@@ -4521,54 +4565,61 @@
 
     def __init__(__self__, *,
                  name: str,
                  app_id: Optional[str] = None,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  password: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  secret_store_app_id_key: Optional[str] = None,
                  secret_store_app_id_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_tenant_id_key: Optional[str] = None,
                  secret_store_tenant_id_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str secret_store_tenant_id_key: * azure_mysql:
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_app_id_key is not None:
             pulumi.set(__self__, "secret_store_app_id_key", secret_store_app_id_key)
         if secret_store_app_id_path is not None:
             pulumi.set(__self__, "secret_store_app_id_path", secret_store_app_id_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_tenant_id_key is not None:
             pulumi.set(__self__, "secret_store_tenant_id_key", secret_store_tenant_id_key)
         if secret_store_tenant_id_path is not None:
             pulumi.set(__self__, "secret_store_tenant_id_path", secret_store_tenant_id_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter
@@ -4601,14 +4652,19 @@
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         return pulumi.get(self, "password")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="secretStoreAppIdKey")
     def secret_store_app_id_key(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_app_id_key")
 
     @property
     @pulumi.getter(name="secretStoreAppIdPath")
     def secret_store_app_id_path(self) -> Optional[str]:
@@ -4643,14 +4699,22 @@
     @property
     @pulumi.getter(name="secretStoreTenantIdPath")
     def secret_store_tenant_id_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_tenant_id_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -4668,14 +4732,16 @@
             suggest = "app_id"
         elif key == "bindInterface":
             suggest = "bind_interface"
         elif key == "clientCertificate":
             suggest = "client_certificate"
         elif key == "egressFilter":
             suggest = "egress_filter"
+        elif key == "portOverride":
+            suggest = "port_override"
         elif key == "secretStoreAppIdKey":
             suggest = "secret_store_app_id_key"
         elif key == "secretStoreAppIdPath":
             suggest = "secret_store_app_id_path"
         elif key == "secretStoreClientCertificateKey":
             suggest = "secret_store_client_certificate_key"
         elif key == "secretStoreClientCertificatePath":
@@ -4702,54 +4768,61 @@
 
     def __init__(__self__, *,
                  name: str,
                  app_id: Optional[str] = None,
                  bind_interface: Optional[str] = None,
                  client_certificate: Optional[str] = None,
                  egress_filter: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  secret_store_app_id_key: Optional[str] = None,
                  secret_store_app_id_path: Optional[str] = None,
                  secret_store_client_certificate_key: Optional[str] = None,
                  secret_store_client_certificate_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_tenant_id_key: Optional[str] = None,
                  secret_store_tenant_id_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str secret_store_tenant_id_key: * azure_mysql:
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if client_certificate is not None:
             pulumi.set(__self__, "client_certificate", client_certificate)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_app_id_key is not None:
             pulumi.set(__self__, "secret_store_app_id_key", secret_store_app_id_key)
         if secret_store_app_id_path is not None:
             pulumi.set(__self__, "secret_store_app_id_path", secret_store_app_id_path)
         if secret_store_client_certificate_key is not None:
             pulumi.set(__self__, "secret_store_client_certificate_key", secret_store_client_certificate_key)
         if secret_store_client_certificate_path is not None:
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_tenant_id_key is not None:
             pulumi.set(__self__, "secret_store_tenant_id_key", secret_store_tenant_id_key)
         if secret_store_tenant_id_path is not None:
             pulumi.set(__self__, "secret_store_tenant_id_path", secret_store_tenant_id_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter
@@ -4782,14 +4855,19 @@
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
         return pulumi.get(self, "egress_filter")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="secretStoreAppIdKey")
     def secret_store_app_id_key(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_app_id_key")
 
     @property
     @pulumi.getter(name="secretStoreAppIdPath")
     def secret_store_app_id_path(self) -> Optional[str]:
@@ -4824,14 +4902,22 @@
     @property
     @pulumi.getter(name="secretStoreTenantIdPath")
     def secret_store_tenant_id_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_tenant_id_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -4891,14 +4977,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -4994,14 +5081,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -5081,14 +5171,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -5191,14 +5282,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -5438,14 +5532,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5537,14 +5632,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -5629,14 +5727,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -5739,14 +5838,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -5823,14 +5925,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -5926,14 +6029,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -6013,14 +6119,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -6123,14 +6230,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -6209,14 +6319,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
@@ -6307,14 +6418,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -6396,14 +6510,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -6499,14 +6614,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -6585,14 +6703,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -6688,14 +6807,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -6779,14 +6901,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
@@ -6888,14 +7011,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -6971,14 +7097,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -7068,14 +7195,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -7397,14 +7527,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -7496,14 +7627,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -7587,14 +7721,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -7686,14 +7821,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -7729,14 +7867,16 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bindInterface":
             suggest = "bind_interface"
         elif key == "egressFilter":
             suggest = "egress_filter"
+        elif key == "portOverride":
+            suggest = "port_override"
         elif key == "secretStoreId":
             suggest = "secret_store_id"
         elif key == "secretStoreKeyfileKey":
             suggest = "secret_store_keyfile_key"
         elif key == "secretStoreKeyfilePath":
             suggest = "secret_store_keyfile_path"
 
@@ -7753,39 +7893,46 @@
 
     def __init__(__self__, *,
                  name: str,
                  scopes: str,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  keyfile: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_keyfile_key: Optional[str] = None,
                  secret_store_keyfile_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "scopes", scopes)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if keyfile is not None:
             pulumi.set(__self__, "keyfile", keyfile)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_keyfile_key is not None:
             pulumi.set(__self__, "secret_store_keyfile_key", secret_store_keyfile_key)
         if secret_store_keyfile_path is not None:
             pulumi.set(__self__, "secret_store_keyfile_path", secret_store_keyfile_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
@@ -7816,14 +7963,19 @@
 
     @property
     @pulumi.getter
     def keyfile(self) -> Optional[str]:
         return pulumi.get(self, "keyfile")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
@@ -7835,14 +7987,22 @@
     @property
     @pulumi.getter(name="secretStoreKeyfilePath")
     def secret_store_keyfile_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_keyfile_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -8280,14 +8440,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -8390,14 +8551,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -8661,14 +8825,15 @@
         """
         :param str name: Unique human-readable name of the Resource.
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param str url: * kubernetes:
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "subdomain", subdomain)
         pulumi.set(__self__, "url", url)
         if bind_interface is not None:
@@ -8780,14 +8945,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -9254,14 +9422,15 @@
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
@@ -9360,14 +9529,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -10029,14 +10201,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -10132,14 +10305,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -10340,14 +10516,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -10443,14 +10620,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -10532,14 +10712,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -10637,14 +10818,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -10734,14 +10918,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -10846,14 +11031,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -10946,14 +11134,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
@@ -11064,14 +11253,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -11164,14 +11356,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
@@ -11282,14 +11475,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -11375,14 +11571,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -11473,14 +11670,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -11592,14 +11792,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -11760,14 +11961,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -11882,14 +12086,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -12057,14 +12262,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -12146,14 +12354,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -12249,14 +12458,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -12711,14 +12923,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
@@ -12815,14 +13028,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -12907,14 +13123,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -13017,14 +13234,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -13280,14 +13500,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -13379,14 +13600,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -13594,14 +13818,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -13698,14 +13923,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -13784,14 +14012,15 @@
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -13883,14 +14112,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -13975,14 +14207,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -14085,14 +14318,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -14169,14 +14405,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -14272,14 +14509,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -14356,14 +14596,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -14459,14 +14700,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -14694,14 +14938,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
@@ -14811,14 +15056,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -14899,14 +15147,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
@@ -15002,14 +15251,17 @@
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -15093,14 +15345,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
@@ -15203,14 +15456,17 @@
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -15294,14 +15550,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
@@ -15404,14 +15661,17 @@
     @pulumi.getter(name="secretStorePrivateKeyPath")
     def secret_store_private_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_private_key_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -15487,14 +15747,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -15584,14 +15845,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -15667,14 +15931,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -15764,14 +16029,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -15847,14 +16115,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str secret_store_username_key: * trino:
         :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -15944,14 +16213,17 @@
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreUsernameKey")
     def secret_store_username_key(self) -> Optional[str]:
+        """
+        * trino:
+        """
         return pulumi.get(self, "secret_store_username_key")
 
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
@@ -15974,14 +16246,181 @@
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
+class ResourceTrino(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "bindInterface":
+            suggest = "bind_interface"
+        elif key == "egressFilter":
+            suggest = "egress_filter"
+        elif key == "portOverride":
+            suggest = "port_override"
+        elif key == "secretStoreId":
+            suggest = "secret_store_id"
+        elif key == "secretStorePasswordKey":
+            suggest = "secret_store_password_key"
+        elif key == "secretStorePasswordPath":
+            suggest = "secret_store_password_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ResourceTrino. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ResourceTrino.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ResourceTrino.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 database: str,
+                 hostname: str,
+                 name: str,
+                 bind_interface: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 password: Optional[str] = None,
+                 port: Optional[int] = None,
+                 port_override: Optional[int] = None,
+                 secret_store_id: Optional[str] = None,
+                 secret_store_password_key: Optional[str] = None,
+                 secret_store_password_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 username: Optional[str] = None):
+        """
+        :param str name: Unique human-readable name of the Resource.
+        :param str bind_interface: Bind interface
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "database", database)
+        pulumi.set(__self__, "hostname", hostname)
+        pulumi.set(__self__, "name", name)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if secret_store_password_key is not None:
+            pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
+        if secret_store_password_path is not None:
+            pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def database(self) -> str:
+        return pulumi.get(self, "database")
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> str:
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[str]:
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter(name="secretStorePasswordKey")
+    def secret_store_password_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_password_key")
+
+    @property
+    @pulumi.getter(name="secretStorePasswordPath")
+    def secret_store_password_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_password_path")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
 class SecretStoreAws(dict):
     def __init__(__self__, *,
                  name: str,
                  region: str,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the SecretStore.
@@ -17181,15 +17620,16 @@
                  snowsights: Sequence['outputs.GetResourceResourceSnowsightResult'],
                  sql_servers: Sequence['outputs.GetResourceResourceSqlServerResult'],
                  ssh_certs: Sequence['outputs.GetResourceResourceSshCertResult'],
                  ssh_customer_keys: Sequence['outputs.GetResourceResourceSshCustomerKeyResult'],
                  sshes: Sequence['outputs.GetResourceResourceSshResult'],
                  sybase_iqs: Sequence['outputs.GetResourceResourceSybaseIqResult'],
                  sybases: Sequence['outputs.GetResourceResourceSybaseResult'],
-                 teradatas: Sequence['outputs.GetResourceResourceTeradataResult']):
+                 teradatas: Sequence['outputs.GetResourceResourceTeradataResult'],
+                 trinos: Sequence['outputs.GetResourceResourceTrinoResult']):
         pulumi.set(__self__, "aks", aks)
         pulumi.set(__self__, "aks_basic_auths", aks_basic_auths)
         pulumi.set(__self__, "aks_service_account_user_impersonations", aks_service_account_user_impersonations)
         pulumi.set(__self__, "aks_service_accounts", aks_service_accounts)
         pulumi.set(__self__, "aks_user_impersonations", aks_user_impersonations)
         pulumi.set(__self__, "amazon_eks", amazon_eks)
         pulumi.set(__self__, "amazon_eks_instance_profile_user_impersonations", amazon_eks_instance_profile_user_impersonations)
@@ -17259,14 +17699,15 @@
         pulumi.set(__self__, "sql_servers", sql_servers)
         pulumi.set(__self__, "ssh_certs", ssh_certs)
         pulumi.set(__self__, "ssh_customer_keys", ssh_customer_keys)
         pulumi.set(__self__, "sshes", sshes)
         pulumi.set(__self__, "sybase_iqs", sybase_iqs)
         pulumi.set(__self__, "sybases", sybases)
         pulumi.set(__self__, "teradatas", teradatas)
+        pulumi.set(__self__, "trinos", trinos)
 
     @property
     @pulumi.getter
     def aks(self) -> Sequence['outputs.GetResourceResourceAkResult']:
         return pulumi.get(self, "aks")
 
     @property
@@ -17645,14 +18086,19 @@
         return pulumi.get(self, "sybases")
 
     @property
     @pulumi.getter
     def teradatas(self) -> Sequence['outputs.GetResourceResourceTeradataResult']:
         return pulumi.get(self, "teradatas")
 
+    @property
+    @pulumi.getter
+    def trinos(self) -> Sequence['outputs.GetResourceResourceTrinoResult']:
+        return pulumi.get(self, "trinos")
+
 
 @pulumi.output_type
 class GetResourceResourceAkResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
                  certificate_authority: Optional[str] = None,
                  client_certificate: Optional[str] = None,
@@ -19813,47 +20259,54 @@
     def __init__(__self__, *,
                  access_key: Optional[str] = None,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  healthcheck_region: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_region is not None:
             pulumi.set(__self__, "healthcheck_region", healthcheck_region)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if role_arn is not None:
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
@@ -19892,14 +20345,19 @@
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="roleExternalId")
     def role_external_id(self) -> Optional[str]:
@@ -19916,14 +20374,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -20250,23 +20716,26 @@
     def __init__(__self__, *,
                  app_id: Optional[str] = None,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str tenant_id: * azure_mysql:
         """
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -20274,16 +20743,20 @@
             pulumi.set(__self__, "egress_filter", egress_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter(name="appId")
@@ -20324,23 +20797,36 @@
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         return pulumi.get(self, "password")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -20357,23 +20843,26 @@
     def __init__(__self__, *,
                  app_id: Optional[str] = None,
                  bind_interface: Optional[str] = None,
                  client_certificate: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str tenant_id: * azure_mysql:
         """
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -20381,16 +20870,20 @@
             pulumi.set(__self__, "client_certificate", client_certificate)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
 
     @property
     @pulumi.getter(name="appId")
@@ -20431,23 +20924,36 @@
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -22572,39 +23078,46 @@
 class GetResourceResourceGcpResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  id: Optional[str] = None,
                  keyfile: Optional[str] = None,
                  name: Optional[str] = None,
+                 port_override: Optional[int] = None,
                  scopes: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if keyfile is not None:
             pulumi.set(__self__, "keyfile", keyfile)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
         if scopes is not None:
             pulumi.set(__self__, "scopes", scopes)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -22638,28 +23151,41 @@
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
     @pulumi.getter
     def scopes(self) -> Optional[str]:
         return pulumi.get(self, "scopes")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -28636,14 +29162,153 @@
 
     @property
     @pulumi.getter(name="egressFilter")
     def egress_filter(self) -> Optional[str]:
         """
         A filter applied to the routing logic to pin datasource to nodes.
         """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> Optional[str]:
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[str]:
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
+class GetResourceResourceTrinoResult(dict):
+    def __init__(__self__, *,
+                 bind_interface: Optional[str] = None,
+                 database: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 hostname: Optional[str] = None,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None,
+                 password: Optional[str] = None,
+                 port: Optional[int] = None,
+                 port_override: Optional[int] = None,
+                 secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 username: Optional[str] = None):
+        """
+        :param str bind_interface: Bind interface
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str id: Unique identifier of the Resource.
+        :param str name: Unique human-readable name of the Resource.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if database is not None:
+            pulumi.set(__self__, "database", database)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if hostname is not None:
+            pulumi.set(__self__, "hostname", hostname)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter
+    def database(self) -> Optional[str]:
+        return pulumi.get(self, "database")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
         return pulumi.get(self, "egress_filter")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
         return pulumi.get(self, "hostname")
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/provider.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/provider.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/remote_identity.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/resource.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,26 +88,27 @@
                  snowsight: Optional[pulumi.Input['ResourceSnowsightArgs']] = None,
                  sql_server: Optional[pulumi.Input['ResourceSqlServerArgs']] = None,
                  ssh: Optional[pulumi.Input['ResourceSshArgs']] = None,
                  ssh_cert: Optional[pulumi.Input['ResourceSshCertArgs']] = None,
                  ssh_customer_key: Optional[pulumi.Input['ResourceSshCustomerKeyArgs']] = None,
                  sybase: Optional[pulumi.Input['ResourceSybaseArgs']] = None,
                  sybase_iq: Optional[pulumi.Input['ResourceSybaseIqArgs']] = None,
-                 teradata: Optional[pulumi.Input['ResourceTeradataArgs']] = None):
+                 teradata: Optional[pulumi.Input['ResourceTeradataArgs']] = None,
+                 trino: Optional[pulumi.Input['ResourceTrinoArgs']] = None):
         """
         The set of arguments for constructing a Resource resource.
         :param pulumi.Input['ResourceAwsConsoleArgs'] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs'] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
-        :param pulumi.Input['ResourceAzureMysqlArgs'] azure_mysql: AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoHostArgs'] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoReplicaSetArgs'] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoShardedClusterArgs'] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMtlsMysqlArgs'] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceSnowsightArgs'] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        :param pulumi.Input['ResourceTrinoArgs'] trino: Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         if aks is not None:
             pulumi.set(__self__, "aks", aks)
         if aks_basic_auth is not None:
             pulumi.set(__self__, "aks_basic_auth", aks_basic_auth)
         if aks_service_account is not None:
             pulumi.set(__self__, "aks_service_account", aks_service_account)
@@ -255,14 +256,16 @@
             pulumi.set(__self__, "ssh_customer_key", ssh_customer_key)
         if sybase is not None:
             pulumi.set(__self__, "sybase", sybase)
         if sybase_iq is not None:
             pulumi.set(__self__, "sybase_iq", sybase_iq)
         if teradata is not None:
             pulumi.set(__self__, "teradata", teradata)
+        if trino is not None:
+            pulumi.set(__self__, "trino", trino)
 
     @property
     @pulumi.getter
     def aks(self) -> Optional[pulumi.Input['ResourceAksArgs']]:
         return pulumi.get(self, "aks")
 
     @aks.setter
@@ -437,17 +440,14 @@
     @azure_certificate.setter
     def azure_certificate(self, value: Optional[pulumi.Input['ResourceAzureCertificateArgs']]):
         pulumi.set(self, "azure_certificate", value)
 
     @property
     @pulumi.getter(name="azureMysql")
     def azure_mysql(self) -> Optional[pulumi.Input['ResourceAzureMysqlArgs']]:
-        """
-        AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "azure_mysql")
 
     @azure_mysql.setter
     def azure_mysql(self, value: Optional[pulumi.Input['ResourceAzureMysqlArgs']]):
         pulumi.set(self, "azure_mysql", value)
 
     @property
@@ -974,14 +974,26 @@
     def teradata(self) -> Optional[pulumi.Input['ResourceTeradataArgs']]:
         return pulumi.get(self, "teradata")
 
     @teradata.setter
     def teradata(self, value: Optional[pulumi.Input['ResourceTeradataArgs']]):
         pulumi.set(self, "teradata", value)
 
+    @property
+    @pulumi.getter
+    def trino(self) -> Optional[pulumi.Input['ResourceTrinoArgs']]:
+        """
+        Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        """
+        return pulumi.get(self, "trino")
+
+    @trino.setter
+    def trino(self, value: Optional[pulumi.Input['ResourceTrinoArgs']]):
+        pulumi.set(self, "trino", value)
+
 
 @pulumi.input_type
 class _ResourceState:
     def __init__(__self__, *,
                  aks: Optional[pulumi.Input['ResourceAksArgs']] = None,
                  aks_basic_auth: Optional[pulumi.Input['ResourceAksBasicAuthArgs']] = None,
                  aks_service_account: Optional[pulumi.Input['ResourceAksServiceAccountArgs']] = None,
@@ -1054,26 +1066,27 @@
                  snowsight: Optional[pulumi.Input['ResourceSnowsightArgs']] = None,
                  sql_server: Optional[pulumi.Input['ResourceSqlServerArgs']] = None,
                  ssh: Optional[pulumi.Input['ResourceSshArgs']] = None,
                  ssh_cert: Optional[pulumi.Input['ResourceSshCertArgs']] = None,
                  ssh_customer_key: Optional[pulumi.Input['ResourceSshCustomerKeyArgs']] = None,
                  sybase: Optional[pulumi.Input['ResourceSybaseArgs']] = None,
                  sybase_iq: Optional[pulumi.Input['ResourceSybaseIqArgs']] = None,
-                 teradata: Optional[pulumi.Input['ResourceTeradataArgs']] = None):
+                 teradata: Optional[pulumi.Input['ResourceTeradataArgs']] = None,
+                 trino: Optional[pulumi.Input['ResourceTrinoArgs']] = None):
         """
         Input properties used for looking up and filtering Resource resources.
         :param pulumi.Input['ResourceAwsConsoleArgs'] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs'] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
-        :param pulumi.Input['ResourceAzureMysqlArgs'] azure_mysql: AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoHostArgs'] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoReplicaSetArgs'] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoShardedClusterArgs'] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMtlsMysqlArgs'] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceSnowsightArgs'] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        :param pulumi.Input['ResourceTrinoArgs'] trino: Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         if aks is not None:
             pulumi.set(__self__, "aks", aks)
         if aks_basic_auth is not None:
             pulumi.set(__self__, "aks_basic_auth", aks_basic_auth)
         if aks_service_account is not None:
             pulumi.set(__self__, "aks_service_account", aks_service_account)
@@ -1221,14 +1234,16 @@
             pulumi.set(__self__, "ssh_customer_key", ssh_customer_key)
         if sybase is not None:
             pulumi.set(__self__, "sybase", sybase)
         if sybase_iq is not None:
             pulumi.set(__self__, "sybase_iq", sybase_iq)
         if teradata is not None:
             pulumi.set(__self__, "teradata", teradata)
+        if trino is not None:
+            pulumi.set(__self__, "trino", trino)
 
     @property
     @pulumi.getter
     def aks(self) -> Optional[pulumi.Input['ResourceAksArgs']]:
         return pulumi.get(self, "aks")
 
     @aks.setter
@@ -1403,17 +1418,14 @@
     @azure_certificate.setter
     def azure_certificate(self, value: Optional[pulumi.Input['ResourceAzureCertificateArgs']]):
         pulumi.set(self, "azure_certificate", value)
 
     @property
     @pulumi.getter(name="azureMysql")
     def azure_mysql(self) -> Optional[pulumi.Input['ResourceAzureMysqlArgs']]:
-        """
-        AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "azure_mysql")
 
     @azure_mysql.setter
     def azure_mysql(self, value: Optional[pulumi.Input['ResourceAzureMysqlArgs']]):
         pulumi.set(self, "azure_mysql", value)
 
     @property
@@ -1940,14 +1952,26 @@
     def teradata(self) -> Optional[pulumi.Input['ResourceTeradataArgs']]:
         return pulumi.get(self, "teradata")
 
     @teradata.setter
     def teradata(self, value: Optional[pulumi.Input['ResourceTeradataArgs']]):
         pulumi.set(self, "teradata", value)
 
+    @property
+    @pulumi.getter
+    def trino(self) -> Optional[pulumi.Input['ResourceTrinoArgs']]:
+        """
+        Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        """
+        return pulumi.get(self, "trino")
+
+    @trino.setter
+    def trino(self, value: Optional[pulumi.Input['ResourceTrinoArgs']]):
+        pulumi.set(self, "trino", value)
+
 
 class Resource(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aks: Optional[pulumi.Input[pulumi.InputType['ResourceAksArgs']]] = None,
@@ -2023,14 +2047,15 @@
                  sql_server: Optional[pulumi.Input[pulumi.InputType['ResourceSqlServerArgs']]] = None,
                  ssh: Optional[pulumi.Input[pulumi.InputType['ResourceSshArgs']]] = None,
                  ssh_cert: Optional[pulumi.Input[pulumi.InputType['ResourceSshCertArgs']]] = None,
                  ssh_customer_key: Optional[pulumi.Input[pulumi.InputType['ResourceSshCustomerKeyArgs']]] = None,
                  sybase: Optional[pulumi.Input[pulumi.InputType['ResourceSybaseArgs']]] = None,
                  sybase_iq: Optional[pulumi.Input[pulumi.InputType['ResourceSybaseIqArgs']]] = None,
                  teradata: Optional[pulumi.Input[pulumi.InputType['ResourceTeradataArgs']]] = None,
+                 trino: Optional[pulumi.Input[pulumi.InputType['ResourceTrinoArgs']]] = None,
                  __props__=None):
         """
         ## Import
 
         Resource can be imported using the id, e.g.,
 
         ```sh
@@ -2038,20 +2063,20 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
-        :param pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']] azure_mysql: AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoHostArgs']] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoReplicaSetArgs']] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoShardedClusterArgs']] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMtlsMysqlArgs']] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        :param pulumi.Input[pulumi.InputType['ResourceTrinoArgs']] trino: Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ResourceArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -2152,14 +2177,15 @@
                  sql_server: Optional[pulumi.Input[pulumi.InputType['ResourceSqlServerArgs']]] = None,
                  ssh: Optional[pulumi.Input[pulumi.InputType['ResourceSshArgs']]] = None,
                  ssh_cert: Optional[pulumi.Input[pulumi.InputType['ResourceSshCertArgs']]] = None,
                  ssh_customer_key: Optional[pulumi.Input[pulumi.InputType['ResourceSshCustomerKeyArgs']]] = None,
                  sybase: Optional[pulumi.Input[pulumi.InputType['ResourceSybaseArgs']]] = None,
                  sybase_iq: Optional[pulumi.Input[pulumi.InputType['ResourceSybaseIqArgs']]] = None,
                  teradata: Optional[pulumi.Input[pulumi.InputType['ResourceTeradataArgs']]] = None,
+                 trino: Optional[pulumi.Input[pulumi.InputType['ResourceTrinoArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -2238,14 +2264,15 @@
             __props__.__dict__["sql_server"] = sql_server
             __props__.__dict__["ssh"] = ssh
             __props__.__dict__["ssh_cert"] = ssh_cert
             __props__.__dict__["ssh_customer_key"] = ssh_customer_key
             __props__.__dict__["sybase"] = sybase
             __props__.__dict__["sybase_iq"] = sybase_iq
             __props__.__dict__["teradata"] = teradata
+            __props__.__dict__["trino"] = trino
         super(Resource, __self__).__init__(
             'sdm:index/resource:Resource',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -2324,31 +2351,32 @@
             snowsight: Optional[pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']]] = None,
             sql_server: Optional[pulumi.Input[pulumi.InputType['ResourceSqlServerArgs']]] = None,
             ssh: Optional[pulumi.Input[pulumi.InputType['ResourceSshArgs']]] = None,
             ssh_cert: Optional[pulumi.Input[pulumi.InputType['ResourceSshCertArgs']]] = None,
             ssh_customer_key: Optional[pulumi.Input[pulumi.InputType['ResourceSshCustomerKeyArgs']]] = None,
             sybase: Optional[pulumi.Input[pulumi.InputType['ResourceSybaseArgs']]] = None,
             sybase_iq: Optional[pulumi.Input[pulumi.InputType['ResourceSybaseIqArgs']]] = None,
-            teradata: Optional[pulumi.Input[pulumi.InputType['ResourceTeradataArgs']]] = None) -> 'Resource':
+            teradata: Optional[pulumi.Input[pulumi.InputType['ResourceTeradataArgs']]] = None,
+            trino: Optional[pulumi.Input[pulumi.InputType['ResourceTrinoArgs']]] = None) -> 'Resource':
         """
         Get an existing Resource resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
-        :param pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']] azure_mysql: AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoHostArgs']] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoReplicaSetArgs']] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoShardedClusterArgs']] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMtlsMysqlArgs']] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        :param pulumi.Input[pulumi.InputType['ResourceTrinoArgs']] trino: Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ResourceState.__new__(_ResourceState)
 
         __props__.__dict__["aks"] = aks
         __props__.__dict__["aks_basic_auth"] = aks_basic_auth
@@ -2423,14 +2451,15 @@
         __props__.__dict__["sql_server"] = sql_server
         __props__.__dict__["ssh"] = ssh
         __props__.__dict__["ssh_cert"] = ssh_cert
         __props__.__dict__["ssh_customer_key"] = ssh_customer_key
         __props__.__dict__["sybase"] = sybase
         __props__.__dict__["sybase_iq"] = sybase_iq
         __props__.__dict__["teradata"] = teradata
+        __props__.__dict__["trino"] = trino
         return Resource(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def aks(self) -> pulumi.Output[Optional['outputs.ResourceAks']]:
         return pulumi.get(self, "aks")
 
@@ -2530,17 +2559,14 @@
     @pulumi.getter(name="azureCertificate")
     def azure_certificate(self) -> pulumi.Output[Optional['outputs.ResourceAzureCertificate']]:
         return pulumi.get(self, "azure_certificate")
 
     @property
     @pulumi.getter(name="azureMysql")
     def azure_mysql(self) -> pulumi.Output[Optional['outputs.ResourceAzureMysql']]:
-        """
-        AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "azure_mysql")
 
     @property
     @pulumi.getter(name="azurePostgres")
     def azure_postgres(self) -> pulumi.Output[Optional['outputs.ResourceAzurePostgres']]:
         return pulumi.get(self, "azure_postgres")
 
@@ -2835,7 +2861,15 @@
         return pulumi.get(self, "sybase_iq")
 
     @property
     @pulumi.getter
     def teradata(self) -> pulumi.Output[Optional['outputs.ResourceTeradata']]:
         return pulumi.get(self, "teradata")
 
+    @property
+    @pulumi.getter
+    def trino(self) -> pulumi.Output[Optional['outputs.ResourceTrino']]:
+        """
+        Trino is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        """
+        return pulumi.get(self, "trino")
+
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/role.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/role.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm/secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm/secret_store.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pierskarsenbarg-pulumi-sdm
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
@@ -65,8 +65,9 @@
         
         <!-- ## Reference
         
         For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/). -->
         
 Keywords: pulumi sdm category/cloud
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt` & `pierskarsenbarg_pulumi_sdm-1.1.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.0.1/setup.py` & `pierskarsenbarg_pulumi_sdm-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.1"
-PLUGIN_VERSION = "1.0.1"
+VERSION = "1.1.0"
+PLUGIN_VERSION = "1.1.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'sdm', PLUGIN_VERSION, '--server', 'github://api.github.com/pierskarsenbarg/pulumi-sdm'])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "sdm Pulumi Package - Development Version"
 
 
 setup(name='pierskarsenbarg_pulumi_sdm',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing StrongDM cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

