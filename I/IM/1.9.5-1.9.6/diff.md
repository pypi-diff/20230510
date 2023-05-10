# Comparing `tmp/IM-1.9.5.tar.gz` & `tmp/IM-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/IM-1.9.5.tar", last modified: Thu Nov  5 08:07:43 2020, max compression
+gzip compressed data, was "dist/IM-1.9.6.tar", last modified: Thu Dec 17 12:29:41 2020, max compression
```

## Comparing `IM-1.9.5.tar` & `IM-1.9.6.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/scripts/
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3640 2020-11-05 08:07:41.000000 IM-1.9.5/scripts/im
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      264 2020-11-05 08:07:41.000000 IM-1.9.5/scripts/im.service
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    13086 2020-11-05 08:07:41.000000 IM-1.9.5/im_service.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      202 2020-11-05 08:07:41.000000 IM-1.9.5/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       38 2020-11-05 08:07:43.000000 IM-1.9.5/setup.cfg
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15266 2020-11-05 08:07:41.000000 IM-1.9.5/README.md
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    35147 2020-11-05 08:07:41.000000 IM-1.9.5/LICENSE
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/IM/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11348 2020-11-05 08:07:41.000000 IM-1.9.5/IM/InfrastructureList.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4438 2020-11-05 08:07:41.000000 IM-1.9.5/IM/CloudInfo.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5524 2020-11-05 08:07:41.000000 IM-1.9.5/IM/xmlobject.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2982 2020-11-05 08:07:41.000000 IM-1.9.5/IM/UnixHTTPAdapter.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/IM/connectors/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    23217 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/CloudConnector.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22033 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/Kubernetes.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26899 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/LibCloud.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    37187 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/FogBow.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2616 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/DeployedNode.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25655 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/vSphere.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      934 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3148 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/Dummy.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    38983 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/AzureClassic.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40609 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/Azure.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    75169 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/OpenStack.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    47736 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/OpenNebula.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    20781 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/CloudStack.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    73019 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/EC2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31752 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/Docker.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    38735 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/GCE.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    68022 2020-11-05 08:07:41.000000 IM-1.9.5/IM/connectors/OCCI.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5471 2020-11-05 08:07:41.000000 IM-1.9.5/IM/config.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21525 2020-11-05 08:07:41.000000 IM-1.9.5/IM/CtxtAgentBase.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1366 2020-11-05 08:07:41.000000 IM-1.9.5/IM/LoggerMixin.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6571 2020-11-05 08:07:41.000000 IM-1.9.5/IM/AppDB.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    71387 2020-11-05 08:07:41.000000 IM-1.9.5/IM/ConfManager.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4116 2020-11-05 08:07:41.000000 IM-1.9.5/IM/SSHRetry.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15292 2020-11-05 08:07:41.000000 IM-1.9.5/IM/ServiceRequests.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    46924 2020-11-05 08:07:41.000000 IM-1.9.5/IM/REST.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    65292 2020-11-05 08:07:41.000000 IM-1.9.5/IM/InfrastructureManager.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1803 2020-11-05 08:07:41.000000 IM-1.9.5/IM/xmlrpcssl.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4810 2020-11-05 08:07:41.000000 IM-1.9.5/IM/recipe.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4810 2020-11-05 08:07:41.000000 IM-1.9.5/IM/timedcall.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8127 2020-11-05 08:07:41.000000 IM-1.9.5/IM/auth.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27152 2020-11-05 08:07:41.000000 IM-1.9.5/IM/InfrastructureInfo.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2067 2020-11-05 08:07:41.000000 IM-1.9.5/IM/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2008 2020-11-05 08:07:41.000000 IM-1.9.5/IM/retry.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    47484 2020-11-05 08:07:41.000000 IM-1.9.5/IM/VirtualMachine.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/IM/tosca/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      734 2020-11-05 08:07:41.000000 IM-1.9.5/IM/tosca/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    68870 2020-11-05 08:07:41.000000 IM-1.9.5/IM/tosca/Tosca.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10100 2020-11-05 08:07:41.000000 IM-1.9.5/IM/db.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11162 2020-11-05 08:07:41.000000 IM-1.9.5/IM/request.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22896 2020-11-05 08:07:41.000000 IM-1.9.5/IM/SSH.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/IM/ansible_utils/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2704 2020-11-05 08:07:41.000000 IM-1.9.5/IM/ansible_utils/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19932 2020-11-05 08:07:41.000000 IM-1.9.5/IM/ansible_utils/ansible_executor_v2.py
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    11487 2020-11-05 08:07:41.000000 IM-1.9.5/IM/ansible_utils/ansible_launcher.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6960 2020-11-05 08:07:41.000000 IM-1.9.5/IM/VMRC.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/IM/openid/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2965 2020-11-05 08:07:41.000000 IM-1.9.5/IM/openid/OpenIDClient.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:41.000000 IM-1.9.5/IM/openid/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2278 2020-11-05 08:07:41.000000 IM-1.9.5/IM/openid/JWT.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/IM/tts/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4259 2020-11-05 08:07:41.000000 IM-1.9.5/IM/tts/tts.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:41.000000 IM-1.9.5/IM/tts/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1393 2020-11-05 08:07:41.000000 IM-1.9.5/IM/tts/onetts.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/contextualization/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9844 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/conf-ansible.yml
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2809 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/basic.yml
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10175 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/ctxt_agent.py
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3087 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/ansible_install.sh
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      734 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/__init__.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/contextualization/AnsibleRecipes/
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/tasks/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1318 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/tasks/disk_format_mount.yml
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1278 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/tasks/main.yml
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      236 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/epel-es.repo
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      813 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/vpn-hosts.conf
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      187 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/epel.repo
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2687 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/ssh_known_hosts.conf
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1015 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/etc-vpn-hosts.conf
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      809 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/hosts.conf
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    27338 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/ctxt_agent_dist.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6144 2020-11-05 08:07:41.000000 IM-1.9.5/contextualization/recipes_ansible.db
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/etc/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6342 2020-11-05 08:07:41.000000 IM-1.9.5/etc/im.cfg
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      714 2020-11-05 08:07:41.000000 IM-1.9.5/etc/logging.conf
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    18659 2020-11-05 08:07:43.000000 IM-1.9.5/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1018 2020-11-05 08:07:41.000000 IM-1.9.5/NOTICE
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-11-05 08:07:43.000000 IM-1.9.5/IM.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2020-11-05 08:07:43.000000 IM-1.9.5/IM.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2103 2020-11-05 08:07:43.000000 IM-1.9.5/IM.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      170 2020-11-05 08:07:43.000000 IM-1.9.5/IM.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    18659 2020-11-05 08:07:43.000000 IM-1.9.5/IM.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        3 2020-11-05 08:07:43.000000 IM-1.9.5/IM.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2983 2020-11-05 08:07:41.000000 IM-1.9.5/setup.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27919 2020-11-05 08:07:41.000000 IM-1.9.5/changelog
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/scripts/
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3640 2020-12-17 12:29:36.000000 IM-1.9.6/scripts/im
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      264 2020-12-17 12:29:36.000000 IM-1.9.6/scripts/im.service
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    13086 2020-12-17 12:29:36.000000 IM-1.9.6/im_service.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      202 2020-12-17 12:29:36.000000 IM-1.9.6/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       38 2020-12-17 12:29:41.000000 IM-1.9.6/setup.cfg
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15266 2020-12-17 12:29:36.000000 IM-1.9.6/README.md
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    35147 2020-12-17 12:29:36.000000 IM-1.9.6/LICENSE
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/IM/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11348 2020-12-17 12:29:36.000000 IM-1.9.6/IM/InfrastructureList.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4438 2020-12-17 12:29:36.000000 IM-1.9.6/IM/CloudInfo.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5524 2020-12-17 12:29:36.000000 IM-1.9.6/IM/xmlobject.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2982 2020-12-17 12:29:36.000000 IM-1.9.6/IM/UnixHTTPAdapter.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/IM/connectors/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    23217 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/CloudConnector.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26301 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/Kubernetes.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    26482 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/LibCloud.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    37187 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/FogBow.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2616 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/DeployedNode.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25655 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/vSphere.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      944 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     3148 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/Dummy.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    38983 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/AzureClassic.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40609 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/Azure.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    76276 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/OpenStack.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    48189 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/OpenNebula.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    20781 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/CloudStack.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    73019 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/EC2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31752 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/Docker.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    17520 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/Linode.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    38735 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/GCE.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    68022 2020-12-17 12:29:36.000000 IM-1.9.6/IM/connectors/OCCI.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5471 2020-12-17 12:29:36.000000 IM-1.9.6/IM/config.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    21525 2020-12-17 12:29:36.000000 IM-1.9.6/IM/CtxtAgentBase.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1366 2020-12-17 12:29:36.000000 IM-1.9.6/IM/LoggerMixin.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6571 2020-12-17 12:29:36.000000 IM-1.9.6/IM/AppDB.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    71620 2020-12-17 12:29:36.000000 IM-1.9.6/IM/ConfManager.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4116 2020-12-17 12:29:36.000000 IM-1.9.6/IM/SSHRetry.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    15292 2020-12-17 12:29:36.000000 IM-1.9.6/IM/ServiceRequests.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    46924 2020-12-17 12:29:36.000000 IM-1.9.6/IM/REST.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    65292 2020-12-17 12:29:36.000000 IM-1.9.6/IM/InfrastructureManager.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1803 2020-12-17 12:29:36.000000 IM-1.9.6/IM/xmlrpcssl.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4810 2020-12-17 12:29:36.000000 IM-1.9.6/IM/recipe.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4810 2020-12-17 12:29:36.000000 IM-1.9.6/IM/timedcall.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8127 2020-12-17 12:29:36.000000 IM-1.9.6/IM/auth.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    27156 2020-12-17 12:29:36.000000 IM-1.9.6/IM/InfrastructureInfo.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2067 2020-12-17 12:29:36.000000 IM-1.9.6/IM/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2008 2020-12-17 12:29:36.000000 IM-1.9.6/IM/retry.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    47729 2020-12-17 12:29:36.000000 IM-1.9.6/IM/VirtualMachine.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/IM/tosca/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      734 2020-12-17 12:29:36.000000 IM-1.9.6/IM/tosca/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    68870 2020-12-17 12:29:36.000000 IM-1.9.6/IM/tosca/Tosca.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10100 2020-12-17 12:29:36.000000 IM-1.9.6/IM/db.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11162 2020-12-17 12:29:36.000000 IM-1.9.6/IM/request.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    22896 2020-12-17 12:29:36.000000 IM-1.9.6/IM/SSH.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/IM/ansible_utils/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2704 2020-12-17 12:29:36.000000 IM-1.9.6/IM/ansible_utils/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19932 2020-12-17 12:29:36.000000 IM-1.9.6/IM/ansible_utils/ansible_executor_v2.py
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    11487 2020-12-17 12:29:36.000000 IM-1.9.6/IM/ansible_utils/ansible_launcher.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6960 2020-12-17 12:29:36.000000 IM-1.9.6/IM/VMRC.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/IM/openid/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2965 2020-12-17 12:29:36.000000 IM-1.9.6/IM/openid/OpenIDClient.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:36.000000 IM-1.9.6/IM/openid/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2278 2020-12-17 12:29:36.000000 IM-1.9.6/IM/openid/JWT.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/IM/tts/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4259 2020-12-17 12:29:36.000000 IM-1.9.6/IM/tts/tts.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:36.000000 IM-1.9.6/IM/tts/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1393 2020-12-17 12:29:36.000000 IM-1.9.6/IM/tts/onetts.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/contextualization/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11083 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/conf-ansible.yml
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2809 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/basic.yml
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    10175 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/ctxt_agent.py
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3087 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/ansible_install.sh
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      734 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/__init__.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/contextualization/AnsibleRecipes/
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/tasks/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1318 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/tasks/disk_format_mount.yml
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1278 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/tasks/main.yml
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      236 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/epel-es.repo
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      813 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/vpn-hosts.conf
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      187 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/epel.repo
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2687 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/ssh_known_hosts.conf
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1015 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/etc-vpn-hosts.conf
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      809 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/hosts.conf
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)    27338 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/ctxt_agent_dist.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6144 2020-12-17 12:29:36.000000 IM-1.9.6/contextualization/recipes_ansible.db
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/etc/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     6342 2020-12-17 12:29:36.000000 IM-1.9.6/etc/im.cfg
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      714 2020-12-17 12:29:36.000000 IM-1.9.6/etc/logging.conf
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    18659 2020-12-17 12:29:41.000000 IM-1.9.6/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1018 2020-12-17 12:29:36.000000 IM-1.9.6/NOTICE
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2020-12-17 12:29:41.000000 IM-1.9.6/IM.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2020-12-17 12:29:40.000000 IM-1.9.6/IM.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2127 2020-12-17 12:29:41.000000 IM-1.9.6/IM.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      170 2020-12-17 12:29:40.000000 IM-1.9.6/IM.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    18659 2020-12-17 12:29:40.000000 IM-1.9.6/IM.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        3 2020-12-17 12:29:40.000000 IM-1.9.6/IM.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2983 2020-12-17 12:29:36.000000 IM-1.9.6/setup.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    28211 2020-12-17 12:29:36.000000 IM-1.9.6/changelog
```

### Comparing `IM-1.9.5/scripts/im` & `IM-1.9.6/scripts/im`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/im_service.py` & `IM-1.9.6/im_service.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/README.md` & `IM-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/LICENSE` & `IM-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/InfrastructureList.py` & `IM-1.9.6/IM/InfrastructureList.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/CloudInfo.py` & `IM-1.9.6/IM/CloudInfo.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/xmlobject.py` & `IM-1.9.6/IM/xmlobject.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/UnixHTTPAdapter.py` & `IM-1.9.6/IM/UnixHTTPAdapter.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/CloudConnector.py` & `IM-1.9.6/IM/connectors/CloudConnector.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/Kubernetes.py` & `IM-1.9.6/IM/connectors/vSphere.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,532 +10,626 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import base64
-import json
-import requests
+import time
+from netaddr import IPNetwork, IPAddress
+
+try:
+    from pyVim.connect import SmartConnect
+    from pyVmomi import vim, vmodl
+except Exception as ex:
+    print("WARN: VMWare pyVmomi library not correctly installed. vSphereCloudConnector will not work!.")
+    print(ex)
+
 try:
     from urlparse import urlparse
 except ImportError:
     from urllib.parse import urlparse
 from IM.VirtualMachine import VirtualMachine
-from .CloudConnector import CloudConnector
-from radl.radl import Feature
 from IM.config import Config
+from .CloudConnector import CloudConnector
 
 
-class KubernetesCloudConnector(CloudConnector):
-    """
-    Cloud Launcher to Kubernetes platform
+class vSphereCloudConnector(CloudConnector):
     """
+    Cloud Launcher to VMWare vSphere using pyvmomi lib
+    https://github.com/vmware/pyvmomi
 
-    type = "Kubernetes"
+    This connector is still EXPERIMENTAL!!
+    """
 
-    _port_base_num = 35000
-    """ Base number to assign SSH port on Kubernetes node."""
-    _port_counter = 0
-    """ Counter to assign SSH port on Kubernetes node."""
-    _root_password = "Aspecial+0ne"
-    """ Default password to set to the root in the container"""
-    _apiVersions = ["v1", "v1beta3"]
-    """ Supported API versions"""
+    type = "vSphere"
+    """str with the name of the provider."""
 
     VM_STATE_MAP = {
-        'Pending': VirtualMachine.PENDING,
-        'Running': VirtualMachine.RUNNING,
-        'Succeeded': VirtualMachine.OFF,
-        'Failed': VirtualMachine.FAILED
+        'poweredOn': VirtualMachine.RUNNING,
+        'poweredOff': VirtualMachine.OFF,
+        'suspended': VirtualMachine.STOPPED
     }
-    """Dictionary with a map with the Kubernetes POD states to the IM states."""
-
-    def create_request(self, method, url, auth_data, headers=None, body=None):
-        auth_header = self.get_auth_header(auth_data)
-        if auth_header:
-            if headers is None:
-                headers = {}
-            headers.update(auth_header)
+    """Dictionary with a map with the vSphere VM states to the IM states."""
 
-        url = "%s://%s:%d%s%s" % (self.cloud.protocol, self.cloud.server, self.cloud.port, self.cloud.path, url)
-        resp = requests.request(method, url, verify=self.verify_ssl, headers=headers, data=body)
+    def __init__(self, cloud_info, inf):
+        self.connection = None
+        CloudConnector.__init__(self, cloud_info, inf)
 
-        return resp
-
-    def get_auth_header(self, auth_data):
-        """
-        Generate the auth header needed to contact with the Kubernetes API server.
+    @staticmethod
+    def wait_for_tasks(service_instance, tasks):
         """
-        url = urlparse(self.cloud.server)
-        auths = auth_data.getAuthInfo(self.type, url[1])
-        if not auths:
-            self.log_error(
-                "No correct auth data has been specified to Kubernetes.")
-            return None
-        else:
-            auth = auths[0]
+        Written by Michael Rice <michael@michaelrice.org>
+        Github: https://github.com/michaelrice
+        Website: https://michaelrice.github.io/
+        Blog: http://www.errr-online.com/
+        This code has been released under the terms of the Apache 2 licenses
+        http://www.apache.org/licenses/LICENSE-2.0.html
+        Helper module for task operations.
 
-        auth_header = None
+        Given the service instance si and tasks, it returns after all the
+        tasks are complete
+        """
+        property_collector = service_instance.content.propertyCollector
+        task_list = [str(task) for task in tasks]
+        # Create filter
+        property_spec = vmodl.query.PropertyCollector.PropertySpec(type=vim.Task,
+                                                                   pathSet=[],
+                                                                   all=True)
+        obj_specs = [vmodl.query.PropertyCollector.ObjectSpec(obj=task) for task in tasks]
+
+        filter_spec = vmodl.query.PropertyCollector.FilterSpec()
+        filter_spec.objectSet = obj_specs
+        filter_spec.propSet = [property_spec]
+        pcfilter = property_collector.CreateFilter(filter_spec, True)
+        try:
+            version, state = None, None
+            # Loop looking for updates till the state moves to a completed state.
+            while len(task_list):
+                update = property_collector.WaitForUpdates(version)
+                for filter_set in update.filterSet:
+                    for obj_set in filter_set.objectSet:
+                        task = obj_set.obj
+                        for change in obj_set.changeSet:
+                            if change.name == 'info':
+                                state = change.val.state
+                            elif change.name == 'info.state':
+                                state = change.val
+                            else:
+                                continue
+
+                            if not str(task) in task_list:
+                                continue
+
+                            if state == vim.TaskInfo.State.success:
+                                # Remove task from taskList
+                                task_list.remove(str(task))
+                            elif state == vim.TaskInfo.State.error:
+                                raise task.info.error
+                # Move to next version
+                version = update.version
+        finally:
+            if pcfilter:
+                pcfilter.Destroy()
 
-        if 'username' in auth and 'password' in auth:
-            passwd = auth['password']
-            user = auth['username']
-            auth_header = {'Authorization': 'Basic ' +
-                           (base64.encodestring((user + ':' + passwd).encode('utf-8'))).strip().decode('utf-8')}
-        elif 'token' in auth:
-            token = auth['token']
-            auth_header = {'Authorization': 'Bearer ' + token}
+    def get_connection(self, auth_data):
+        """
+        Get the vSphere connection object from the auth data
 
-        return auth_header
+        Arguments:
+            - auth(Authentication): parsed authentication tokens.
 
-    def get_api_version(self, auth_data):
-        """
-        Return the API version to use to connect with kubernetes API server
+        Returns: a :py:class:`vim.connect.SmartConnect` or None in case of error
         """
-        version = self._apiVersions[0]
-
-        try:
-            resp = self.create_request('GET', "/api/", auth_data)
+        if self.connection:
+            return self.connection
+        else:
+            auth = auth_data.getAuthInfo(self.type)
 
-            if resp.status_code == 200:
-                output = json.loads(resp.text)
-                for v in self._apiVersions:
-                    if v in output["versions"]:
-                        return v
+            if auth and 'username' in auth[0] and 'password' in auth[0]:
 
-        except Exception:
-            self.log_exception(
-                "Error connecting with Kubernetes API server")
+                connection = SmartConnect(host=self.cloud.server,
+                                          user=auth[0]['username'],
+                                          pwd=auth[0]['password'],
+                                          port=self.cloud.port)
 
-        self.log_warn("Error getting a compatible API version. Setting the default one.")
-        self.log_debug("Using %s API version." % version)
-        return version
+                self.connection = connection
+                return connection
+            else:
+                self.log_error("No correct auth data has been specified to vSpere: username, password")
+                self.log_debug(auth)
+                raise Exception("No correct auth data has been specified to vSpere: username, password")
 
     def concrete_system(self, radl_system, str_url, auth_data):
         url = urlparse(str_url)
         protocol = url[0]
-        if protocol == 'docker' and url[1]:
+        src_host = url[1].split(':')[0]
+
+        if protocol == "vsp" and self.cloud.server == src_host:
+            # Check the space in image and compare with disks.free_size
+            if radl_system.getValue('disks.free_size'):
+                disk_free = int(radl_system.getFeature('disks.free_size').getValue('M'))
+                # The VMRC specified the value in MB
+                disk_size = int(radl_system.getValue("disk.0.size"))
+
+                if disk_size < disk_free:
+                    # if the image do not have enough space, discard it
+                    return None
+
             res_system = radl_system.clone()
 
-            res_system.addFeature(Feature("virtual_system_type", "=", "docker"), conflict="other", missing="other")
             res_system.getFeature("cpu.count").operator = "="
             res_system.getFeature("memory.size").operator = "="
 
-            res_system.setValue('disk.0.os.credentials.username', 'root')
-            res_system.setValue('disk.0.os.credentials.password', self._root_password)
-
             return res_system
         else:
             return None
 
-    def _delete_volume_claim(self, namespace, vc_name, auth_data):
-        try:
-            apiVersion = self.get_api_version(auth_data)
+    @staticmethod
+    def gen_nic(num, network):
+        """
+        Get a nic for the specified network
+        """
+        nic = vim.vm.device.VirtualDeviceSpec()
+        nic.operation = vim.vm.device.VirtualDeviceSpec.Operation.add  # or edit if a device exists
+        nic.device = vim.vm.device.VirtualVmxnet3()
+        nic.device.wakeOnLanEnabled = True
+        nic.device.addressType = 'assigned'
+        nic.device.key = 4000  # 4000 seems to be the value to use for a vmxnet3 device
+        nic.device.deviceInfo = vim.Description()
+        nic.device.deviceInfo.label = "Network Adapter %d" % num
+        nic.device.deviceInfo.summary = "Net summary"
+        nic.device.backing = vim.vm.device.VirtualEthernetCard.NetworkBackingInfo()
+        nic.device.backing.network = network
+        nic.device.backing.deviceName = "Device%d" % num
+        nic.device.backing.useAutoDetect = False
+        nic.device.connectable = vim.vm.device.VirtualDevice.ConnectInfo()
+        nic.device.connectable.startConnected = True
+        nic.device.connectable.allowGuestControl = True
 
-            uri = "/api/" + apiVersion + "/namespaces/" + namespace + "/persistentvolumeclaims/" + vc_name
-            resp = self.create_request('DELETE', uri, auth_data)
+        return nic
 
-            if resp.status_code == 404:
-                self.log_warn("Trying to remove a non existing PersistentVolumeClaim: " + vc_name)
-                return True
-            elif resp.status_code != 200:
-                self.log_error("Error deleting the PersistentVolumeClaim: " + resp.txt)
-                return False
-            else:
-                return True
-        except Exception:
-            self.log_exception("Error connecting with Kubernetes API server")
-            return False
+    def create_vm(self, radl, vm_name, connection, vm_folder, resource_pool,
+                  datastore, template_name, cpu, memory, nets, vm):
+        """
+        Create a VM from a template
 
-    def _delete_volume_claims(self, pod_data, auth_data):
-        if 'volumes' in pod_data['spec']:
-            for volume in pod_data['spec']['volumes']:
-                if 'persistentVolumeClaim' in volume and 'claimName' in volume['persistentVolumeClaim']:
-                    vc_name = volume['persistentVolumeClaim']['claimName']
-                    success = self._delete_volume_claim(pod_data["metadata"]["namespace"], vc_name, auth_data)
-                    if not success:
-                        self.log_error("Error deleting PersistentVolumeClaim:" + vc_name)
+        Arguments:
+            - vm_name(str): Name of the VM (must be unique).
+            - connection(:py:class:`vim.connect.SmartConnect` ): Connection object.
+            - vm_folder(:py:class:`vim.Folder` ): Folder this VM will be a child.
+            - resource_pool(:py:class:`vim.ResourcePool`): Resource pool to locate this VM.
+            - datastore(:py:class:`vim.Datastore`): Datastore to store this VM.
+            - template_name(str): Name of the template used to clone this VM.
+            - cpu(int): Number of CPUs of the VM.
+            - memory(int): Amount of RAM memory of the VM (in MB).
+            - auth(Authentication): parsed authentication tokens.
 
-    def _create_volume_claim(self, claim_data, auth_data):
-        try:
-            apiVersion = self.get_api_version(auth_data)
+        Returns: a :py:class:`vim.connect.SmartConnect` or None in case of error
+        """
+        system = radl.systems[0]
+        # set relospec
+        relospec = vim.vm.RelocateSpec()
+        relospec.datastore = datastore
+        relospec.pool = resource_pool
+
+        config = vim.vm.ConfigSpec(name=vm_name,
+                                   memoryMB=memory,
+                                   numCPUs=cpu)
 
-            headers = {'Content-Type': 'application/json'}
-            uri = ("/api/" + apiVersion + "/namespaces/" +
-                   claim_data['metadata']['namespace'] +
-                   "/persistentvolumeclaims")
-            body = json.dumps(claim_data)
-            resp = self.create_request('POST', uri, auth_data, headers, body)
-
-            output = str(resp.text)
-            if resp.status_code != 201:
-                self.log_error("Error deleting the POD: " + output)
-                return False
+        devices = []
+        adaptermaps = []
+
+        i = 0
+        while system.getValue("net_interface." + str(i) + ".connection"):
+            net_name = system.getValue("net_interface." + str(i) + ".connection")
+            fixed_ip = system.getValue("net_interface." + str(i) + ".ip")
+
+            # get the one network info
+            subnet_address = None
+            subnet_mask = None
+            gateway = None
+            net_obj = None
+            if nets[net_name]:
+                net_obj = nets[net_name][0]
+                subnet_address = nets[net_name][2].subnetAddress
+                subnet_mask = nets[net_name][2].netmask
+                gateway = nets[net_name][2].gateway
+                radl.get_network_by_id(net_name).setValue('provider_id', str(net_name))
             else:
-                return True
-        except Exception:
-            self.log_exception(
-                "Error connecting with Kubernetes API server")
-            return False
+                self.log_error("No vSphere network found for network: " + net_name)
+                raise Exception("No vSphere network found for network: " + net_name)
 
-    def _create_volumes(self, apiVersion, namespace, system, pod_name, auth_data, persistent=False):
-        res = []
-        cont = 1
-        while (system.getValue("disk." + str(cont) + ".size") and
-                system.getValue("disk." + str(cont) + ".mount_path") and
-                system.getValue("disk." + str(cont) + ".device")):
-            disk_mount_path = system.getValue("disk." + str(cont) + ".mount_path")
-            # Use the device as volume host path to bind
-            disk_device = system.getValue("disk." + str(cont) + ".device")
-            disk_size = system.getFeature("disk." + str(cont) + ".size").getValue('B')
-            if not disk_mount_path.startswith('/'):
-                disk_mount_path = '/' + disk_mount_path
-            if not disk_device.startswith('/'):
-                disk_device = '/' + disk_device
-            self.log_info("Binding a volume in %s to %s" % (disk_device, disk_mount_path))
-            name = "%s-%d" % (pod_name, cont)
-
-            if persistent:
-                claim_data = {'apiVersion': apiVersion, 'kind': 'PersistentVolumeClaim'}
-                claim_data['metadata'] = {'name': name, 'namespace': namespace}
-                claim_data['spec'] = {'accessModes': ['ReadWriteOnce'], 'resources': {
-                    'requests': {'storage': disk_size}}}
-
-                success = self._create_volume_claim(claim_data, auth_data)
-                if success:
-                    res.append((name, disk_device, disk_size, disk_mount_path, persistent))
-                else:
-                    self.log_error("Error creating PersistentVolumeClaim:" + name)
+            nic = self.gen_nic(i, net_obj)
+            devices.append(nic)
+
+            # guest NIC settings, i.e. "adapter map"
+            guest_map = vim.vm.customization.AdapterMapping()
+            guest_map.adapter = vim.vm.customization.IPSettings()
+
+            if fixed_ip:
+                if not subnet_mask:
+                    subnet_mask = system.getValue("net_interface." + str(i) + ".subnet")
+                if not subnet_mask:
+                    raise Exception("net_interface." + str(i) + ".subnet must be defined for this network.")
+
+                if not gateway:
+                    gateway = system.getValue("net_interface." + str(i) + ".gateway")
+                if not gateway:
+                    raise Exception("net_interface." + str(i) + ".gateway must be defined for this network.")
+
+                if not IPAddress(fixed_ip) in IPNetwork(subnet_address + "/" + subnet_mask):
+                    raise Exception("IP %s not in the subnet: %s/%s" % (fixed_ip, subnet_address, subnet_mask))
+
+                guest_map.adapter.ip = vim.vm.customization.FixedIp()
+                guest_map.adapter.ip.ipAddress = fixed_ip
+                guest_map.adapter.subnetMask = subnet_mask
+                guest_map.adapter.gateway = gateway
             else:
-                res.append((name, disk_device, disk_size, disk_mount_path, persistent))
+                guest_map.adapter.ip = vim.vm.customization.DhcpIpGenerator()
 
-            cont += 1
+            adaptermaps.append(guest_map)
+            i += 1
 
-        return res
+        config.deviceChange = devices
 
-    def _generate_pod_data(self, apiVersion, namespace, name, outports, system, ssh_port, volumes):
-        cpu = str(system.getValue('cpu.count'))
-        memory = "%s" % system.getFeature('memory.size').getValue('B')
-        # The URI has this format: docker://image_name
-        image_name = system.getValue("disk.0.image.url")[9:]
-
-        ports = [{'containerPort': 22, 'protocol': 'TCP', 'hostPort': ssh_port}]
-        if outports:
-            for outport in outports:
-                if outport.is_range():
-                    self.log_warn("Port range not allowed in Kubernetes connector. Ignoring.")
-                elif outport.get_local_port() != 22:
-                    ports.append({'containerPort': outport.get_local_port(), 'protocol': outport.get_protocol().upper(
-                    ), 'hostPort': outport.get_remote_port()})
-
-        pod_data = {'apiVersion': apiVersion, 'kind': 'Pod'}
-        pod_data['metadata'] = {
-            'name': name,
-            'namespace': namespace,
-            'labels': {'name': name}
-        }
-        command = "yum install -y openssh-server python"
-        command += " ; "
-        command += "apt-get update && apt-get install -y openssh-server python"
-        command += " ; "
-        command += "mkdir /var/run/sshd"
-        command += " ; "
-        command += "sed -i '/PermitRootLogin/c\PermitRootLogin yes' /etc/ssh/sshd_config"
-        command += " ; "
-        command += "ssh-keygen -t rsa -f /etc/ssh/ssh_host_rsa_key -N ''"
-        command += " ; "
-        command += "echo 'root:" + self._root_password + "' | chpasswd"
-        command += " ; "
-        command += "sed 's@session\s*required\s*pam_loginuid.so@session optional pam_loginuid.so@g' -i /etc/pam.d/sshd"
-        command += " ; "
-        command += " /usr/sbin/sshd -D"
-        containers = [{
-            'name': name,
-            'image': image_name,
-            'command': ["/bin/bash", "-c", command],
-            'imagePullPolicy': 'IfNotPresent',
-            'ports': ports,
-            'resources': {'limits': {'cpu': cpu, 'memory': memory}}
-        }]
-
-        if system.getValue("docker.privileged") == 'yes':
-            containers[0]['securityContext'] = {'privileged': True}
-
-        if volumes:
-            containers[0]['volumeMounts'] = []
-            for (v_name, _, _, v_mount_path, _) in volumes:
-                containers[0]['volumeMounts'].append(
-                    {'name': v_name, 'mountPath': v_mount_path})
-
-        pod_data['spec'] = {'containers': containers, 'restartPolicy': 'Never'}
-
-        if volumes:
-            pod_data['spec']['volumes'] = []
-            for (v_name, v_device, _, _, persistent) in volumes:
-                if persistent:
-                    pod_data['spec']['volumes'].append(
-                        {'name': v_name, 'persistentVolumeClaim': {'claimName': v_name}})
-                else:
-                    if v_device:
-                        # Use the device as volume host path to bind
-                        pod_data['spec']['volumes'].append(
-                            {'name': v_name, 'hostPath:': {'path': v_device}})
-                    else:
-                        pod_data['spec']['volumes'].append(
-                            {'name': v_name, 'emptyDir:': {}})
+        # Hostname settings
+        ident = vim.vm.customization.LinuxPrep()
+        (nodename, nodedom) = vm.getRequestedName(default_hostname=Config.DEFAULT_VM_NAME,
+                                                  default_domain=Config.DEFAULT_DOMAIN)
+        ident.domain = nodedom
+        ident.hostName = vim.vm.customization.FixedName()
+        ident.hostName.name = nodename
+
+        # DNS settings
+        globalip = vim.vm.customization.GlobalIPSettings()
+        dns_servers = system.getValue("net_interface.0.dns_servers")
+        if dns_servers:
+            globalip.dnsServerList = dns_servers.split(",")
+        globalip.dnsSuffixList = [nodedom]
+
+        customspec = vim.vm.customization.Specification()
+        customspec.nicSettingMap = adaptermaps
+        customspec.globalIPSettings = globalip
+        customspec.identity = ident
+
+        clonespec = vim.vm.CloneSpec()
+        clonespec.location = relospec
+        clonespec.powerOn = True
+        clonespec.config = config
+        clonespec.customization = customspec
+
+        template = self.get_vm_by_name(connection.RetrieveContent(), template_name)
+
+        task = template.Clone(folder=vm_folder, name=vm_name, spec=clonespec)
+        return task
 
-        return pod_data
+    # The path must be: vsp://template_name
+    @staticmethod
+    def get_template_name(path):
+        """
+        Get the region and the image name from an URL of a VMI
+
+        Arguments:
+           - path(str): URL of a VMI (some like this: vsp://template_name)
+        Returns: a str with the template name
+        """
+        uri = urlparse(path)
+        return uri[2][1:]
+
+    @staticmethod
+    def get_datastores(content):
+        """
+        Returns all datastores
+        """
+        obj = {}
+        container = content.viewManager.CreateContainerView(content.rootFolder, [vim.Datastore], True)
+        for c in container.view:
+            obj[c.name] = c
+        return obj
+
+    @staticmethod
+    def map_radl_vsphere_networks(radl_nets, vsphere_nets):
+        """
+        Generate a mapping between the RADL networks and the ONE networks
+
+        Arguments:
+           - radl_nets(list of :py:class:`radl.network` objects): RADL networks.
+           - vsphere_nets(a list of :py:class:`vim.Network` objects): vSpehere networks
+
+         Returns: a dict with key the RADL network id and value a tuple (one_net_name, one_net_id, is_public)
+        """
+        # TODO: get the ip and subnet of an interface to select the network
+        res = {}
+
+        used_nets = []
+        last_net = None
+        for radl_net in radl_nets:
+            # First check if the user has specified a provider ID
+            net_provider_id = radl_net.getValue('provider_id')
+            if net_provider_id:
+                for net_name, net_values in vsphere_nets.items():
+                    is_public = net_values[1]
+                    # If the name is the same and have the same "publicity" value
+                    if net_name == net_provider_id and radl_net.isPublic() == is_public:
+                        res[radl_net.id] = net_values
+                        used_nets.append(net_name)
+                        break
+            else:
+                for net_name, net_values in vsphere_nets.items():
+                    is_public = net_values[1]
+                    if net_name not in used_nets and radl_net.isPublic() == is_public:
+                        res[radl_net.id] = net_values
+                        used_nets.append(net_name)
+                        last_net = net_values
+                        break
+                if radl_net.id not in res:
+                    res[radl_net.id] = last_net
+
+        # In case of there are no private network, use public ones for non mapped networks
+        used_nets = []
+        for radl_net in radl_nets:
+            if not res[radl_net.id]:
+                for net_name, net_values in vsphere_nets.items():
+                    is_public = net_values[1]
+                    if net_name not in used_nets and is_public:
+                        res[radl_net.id] = net_values
+                        used_nets.append(net_name)
+                        last_net = net_values
+                        break
+                if radl_net.id not in res:
+                    res[radl_net.id] = last_net
+
+        return res
 
     def launch(self, inf, radl, requested_radl, num_vm, auth_data):
         system = radl.systems[0]
 
-        public_net = None
-        for net in radl.networks:
-            if net.isPublic():
-                public_net = net
-
-        outports = None
-        if public_net:
-            outports = public_net.getOutPorts()
+        cpu = system.getValue('cpu.count')
+        memory = system.getFeature('memory.size').getValue('M')
 
-        apiVersion = self.get_api_version(auth_data)
+        connection = self.get_connection(auth_data)
 
-        res = []
-        # First create the namespace for the infrastructure
-        namespace = inf.id
-        headers = {'Content-Type': 'application/json'}
-        uri = "/api/" + apiVersion + "/namespaces"
-        with inf._lock:
-            resp = self.create_request('GET', uri + "/" + namespace, auth_data, headers)
-            if resp.status_code != 200:
-                namespace_data = {'apiVersion': apiVersion, 'kind': 'Namespace',
-                                  'metadata': {'name': namespace}}
-                body = json.dumps(namespace_data)
-                resp = self.create_request('POST', uri, auth_data, headers, body)
-
-                if resp.status_code != 201:
-                    for _ in range(num_vm):
-                        res.append((False, "Error creating the Namespace: " + resp.text))
-                        return res
+        content = connection.RetrieveContent()
+        datacenter = content.rootFolder.childEntity[0]
+        vm_folder = datacenter.vmFolder
+        hosts = datacenter.hostFolder.childEntity
+        resource_pool = hosts[0].resourcePool
+
+        template = self.get_template_name(system.getValue("disk.0.image.url"))
+
+        datastores = self.get_datastores(content)
+        networks = self.get_networks(content, datacenter)
 
+        nets = self.map_radl_vsphere_networks(radl.networks, networks)
+
+        tasks = []
+        res = []
         i = 0
         while i < num_vm:
-            try:
-                i += 1
+            self.log_debug("Creating node")
 
-                vm = VirtualMachine(inf, None, self.cloud, radl, requested_radl, self)
-                vm.destroy = True
-                inf.add_vm(vm)
-                (nodename, _) = vm.getRequestedName(default_hostname=Config.DEFAULT_VM_NAME,
-                                                    default_domain=Config.DEFAULT_DOMAIN)
-                pod_name = nodename
-
-                # Do not use the Persistent volumes yet
-                volumes = self._create_volumes(apiVersion, namespace, system, pod_name, auth_data)
-
-                ssh_port = (KubernetesCloudConnector._port_base_num + KubernetesCloudConnector._port_counter) % 65535
-                KubernetesCloudConnector._port_counter += 1
-                pod_data = self._generate_pod_data(apiVersion, namespace, pod_name, outports,
-                                                   system, ssh_port, volumes)
-                body = json.dumps(pod_data)
-
-                uri = "/api/" + apiVersion + "/namespaces/" + namespace + "/pods"
-                resp = self.create_request('POST', uri, auth_data, headers, body)
-
-                if resp.status_code != 201:
-                    res.append((False, "Error creating the Container: " + resp.text))
-                    try:
-                        self._delete_volume_claims(pod_data, auth_data)
-                    except Exception:
-                        self.log_exception("Error deleting volumes.")
-                else:
-                    output = json.loads(resp.text)
-                    vm.id = output["metadata"]["name"]
-                    # Set SSH port in the RADL info of the VM
-                    vm.setSSHPort(ssh_port)
-                    # Set the default user and password to access the container
-                    vm.info.systems[0].setValue(
-                        'disk.0.os.credentials.username', 'root')
-                    vm.info.systems[0].setValue(
-                        'disk.0.os.credentials.password', self._root_password)
-                    vm.info.systems[0].setValue('instance_id', str(vm.id))
-                    vm.info.systems[0].setValue('instance_name', str(vm.id))
+            vm_name = self.gen_instance_name(system)
+            vm = VirtualMachine(inf, vm_name, self.cloud, radl, requested_radl, self)
+            task = self.create_vm(radl, vm_name, connection, vm_folder, resource_pool,
+                                  list(datastores.values())[0], template, cpu, memory, nets, vm)
+            tasks.append(task)
 
-                    vm.destroy = False
-                    res.append((True, vm))
+            i += 1
 
+        for task in tasks:
+            try:
+                self.wait_for_tasks(connection, [task])
+                self.log_debug("Node successfully created.")
+                res.append((True, vm))
             except Exception as ex:
-                self.log_exception("Error connecting with Kubernetes API server")
-                res.append((False, "ERROR: " + str(ex)))
+                self.log_exception("Error waiting VM creation task.")
+                res.append((False, "Error creating the node: " + str(ex)))
 
         return res
 
-    def _get_pod(self, vm, auth_data):
-        try:
-            namespace = vm.inf.id
-            pod_name = vm.id
+    @staticmethod
+    def get_networks(content, datacenter):
+        """
+        Returns all metworks
+        """
+        nets = {}
+        poolmgr = vim.IpPoolManager()
+        ippools = poolmgr.QueryIpPools(datacenter)
+        container = content.viewManager.CreateContainerView(content.rootFolder, [vim.Network], True)
+        for c in container.view:
+            is_public = None
+            for ippool in ippools:
+                if c.summary.ipPoolName == ippool.name:
+                    is_public = not any([IPAddress(ippool.ipv4Config.subnetAddress) in IPNetwork(
+                        mask) for mask in Config.PRIVATE_NET_MASKS])
+                    break
 
-            apiVersion = self.get_api_version(auth_data)
+            nets[c.name] = (c, is_public, ippool.ipv4Config)
 
-            uri = "/api/" + apiVersion + "/namespaces/" + namespace + "/pods/" + pod_name
-            resp = self.create_request('GET', uri, auth_data)
+        return nets
 
-            if resp.status_code == 200:
-                return (True, resp.status_code, resp.text)
-            else:
-                return (False, resp.status_code, resp.text)
+    @staticmethod
+    def get_vm_by_name(content, name):
+        """
+        Find a virtual machine by it's name and return it
+        """
+        vm = None
+        container = content.viewManager.CreateContainerView(content.rootFolder, [vim.VirtualMachine], True)
+        for c in container.view:
+            # c.summary.config.template
+            if c.name == name:
+                vm = c
+                break
+        return vm
+
+    def finalize(self, vm, last, auth_data):
+        connection = self.get_connection(auth_data)
+        node = self.get_vm_by_name(connection.RetrieveContent(), vm.id)
 
-        except Exception as ex:
-            self.log_exception(
-                "Error connecting with Kubernetes API server")
-            return (False, None, "Error connecting with Kubernetes API server: " + str(ex))
+        if node:
+            if format(node.runtime.powerState) == "poweredOn":
+                task = node.PowerOff()
+                try:
+                    self.wait_for_tasks(connection, [task])
+                except Exception:
+                    self.log_exception("Error powering off VM " + str(vm.id))
 
-    def updateVMInfo(self, vm, auth_data):
-        success, status, output = self._get_pod(vm, auth_data)
-        if success:
-            output = json.loads(output)
-            vm.state = self.VM_STATE_MAP.get(
-                output["status"]["phase"], VirtualMachine.UNKNOWN)
-
-            # Update the network info
-            self.setIPs(vm, output)
-            return (True, vm)
+            task = node.Destroy()
+            try:
+                self.wait_for_tasks(connection, [task])
+            except Exception as ex:
+                self.log_exception("Error destroying the VM " + str(vm.id))
+                return (False, "Error destroying the VM: " + str(ex))
+
+            self.log_debug("VM " + str(vm.id) + " successfully destroyed")
         else:
-            self.log_error("Error getting info about the POD: code: %s, msg: %s" % (status, output))
-            return (False, "Error getting info about the POD: code: %s, msg: %s" % (status, output))
+            self.log_warn("VM " + str(vm.id) + " not found.")
+        return (True, "")
 
     @staticmethod
-    def setIPs(vm, pod_info):
+    def setIps(vm, node):
         """
-        Adapt the RADL information of the VM to the real IPs assigned by the cloud provider
-
-        Arguments:
-           - vm(:py:class:`IM.VirtualMachine`): VM information.
-           - pod_info(dict): JSON information about the POD
+        Set the IPs of the VM from the info obtained from vSphere
         """
-
         public_ips = []
         private_ips = []
-        if 'hostIP' in pod_info["status"]:
-            public_ips = [str(pod_info["status"]["hostIP"])]
-        if 'podIP' in pod_info["status"]:
-            private_ips = [str(pod_info["status"]["podIP"])]
+
+        if node.guest:
+            for nic in node.guest.net:
+                if nic.ipAddress:
+                    ip = nic.ipAddress
+                    is_private = any([IPAddress(ip) in IPNetwork(mask) for mask in Config.PRIVATE_NET_MASKS])
+                    if is_private:
+                        private_ips.append(ip)
+                    else:
+                        public_ips.append(ip)
 
         vm.setIps(public_ips, private_ips)
 
-    def finalize(self, vm, last, auth_data):
-        if vm.id:
-            success, status, output = self._get_pod(vm, auth_data)
-            if success:
-                if status == 404:
-                    self.log_warn("Trying to remove a non existing POD id: %s" % vm.id)
-                    return (True, vm.id)
-                else:
-                    pod_data = json.loads(output)
-                    self._delete_volume_claims(pod_data, auth_data)
+    def updateVMInfo(self, vm, auth_data):
+        connection = self.get_connection(auth_data)
+        node = self.get_vm_by_name(connection.RetrieveContent(), vm.id)
 
-            success = self._delete_pod(vm, auth_data)
+        if node:
+            state = node.summary.runtime.powerState
+            vm.state = self.VM_STATE_MAP.get(state, VirtualMachine.UNKNOWN)
+            self.setIps(vm, node)
+            self.attach_volumes(connection, node, vm)
         else:
-            self.log_warn("No VM ID. Ignoring")
-            success = True
+            self.log_warn("VM " + str(vm.id) + " does not exist.")
+            vm.state = VirtualMachine.OFF
 
-        if last:
-            self._delete_namespace(vm, auth_data)
+        return (True, vm)
 
-        return success
-
-    def _delete_namespace(self, vm, auth_data):
-        apiVersion = self.get_api_version(auth_data)
-        headers = {'Content-Type': 'application/json'}
-        uri = "/api/" + apiVersion + "/namespaces/" + vm.inf.id
-        resp = self.create_request('DELETE', uri, auth_data, headers)
-        if resp.status_code != 200:
-            self.log_error("Error deleting Namespace")
-            return False
-        return True
-
-    def _delete_pod(self, vm, auth_data):
-        try:
-            namespace = vm.inf.id
-            pod_name = vm.id
-
-            apiVersion = self.get_api_version(auth_data)
-            uri = "/api/" + apiVersion + "/namespaces/" + namespace + "/pods/" + pod_name
-            resp = self.create_request('DELETE', uri, auth_data)
-
-            if resp.status_code == 404:
-                self.log_warn("Trying to remove a non existing POD id: " + pod_name)
-                return (True, pod_name)
-            elif resp.status_code != 200:
-                return (False, "Error deleting the POD: " + resp.text)
-            else:
-                return (True, pod_name)
-        except Exception:
-            self.log_exception("Error connecting with Kubernetes API server")
-            return (False, "Error connecting with Kubernetes API server")
+    def start(self, vm, auth_data):
+        return self.vm_action(vm, 'start', auth_data)
 
     def stop(self, vm, auth_data):
-        return (False, "Not supported")
-
-    def start(self, vm, auth_data):
-        return (False, "Not supported")
+        return self.vm_action(vm, 'stop', auth_data)
 
     def reboot(self, vm, auth_data):
-        return (False, "Not supported")
+        return self.vm_action(vm, 'reboot', auth_data)
 
-    def alterVM(self, vm, radl, auth_data):
-        # This function is correctly implemented
-        # But kubernetes does not permit cpu to be updated yet
-        system = radl.systems[0]
+    def vm_action(self, vm, action, auth_data):
+        connection = self.get_connection(auth_data)
+        node = self.get_vm_by_name(connection.RetrieveContent(), vm.id)
+
+        if node:
+            if action == 'stop':
+                if format(node.runtime.powerState) != "poweredOn":
+                    return (False, "Error stopping the VM. The VM is not running.")
+                task = node.Suspend()
+            elif action == 'start':
+                if format(node.runtime.powerState) != "suspended":
+                    return (False, "Error starting the VM. The VM is not suspended.")
+                task = node.PowerOn()
+            elif action == 'reboot':
+                task = node.Reset()
 
-        apiVersion = self.get_api_version(auth_data)
+            try:
+                self.wait_for_tasks(connection, [task])
+            except Exception as ex:
+                self.log_exception("Error in VM action " + str(vm.id))
+                return (False, "Error in VM action: " + str(ex))
 
-        try:
-            pod_data = []
+            self.log_debug("VM " + str(vm.id) + " successfully " + action)
+        else:
+            self.log_warn("VM " + str(vm.id) + " not found.")
+        return (True, "")
 
-            cpu = vm.info.systems[0].getValue('cpu.count')
-            memory = vm.info.systems[0].getFeature('memory.size').getValue('B')
+    def add_disk(self, vm, si, disk_size, disk_type="thin"):
+        """
+        Written by Dann Bohn
+        Github: https://github.com/whereismyjetpack
+        Email: dannbohn@gmail.com
+        Script to add a Hard disk to an existing VM
+
+        Known issues:
+        This will not add more than 15 disks to a VM
+        To do that the VM needs an additional scsi controller
+        and I have not yet worked through that
 
-            new_cpu = system.getValue('cpu.count')
-            new_memory = system.getFeature('memory.size').getValue('B')
+        Arguments:
+            - vm(:py:class:`vim.VirtualMachine` ): VM to add the disk.
+            - si(:py:class:`vim.connect.SmartConnect` ): Connection object.
+            - disk_size(str): disk size, in GB, to add to the VM
+            - disk_type(str): thick or thin (default value thin).
 
-            changed = False
-            if new_cpu and new_cpu != cpu:
-                pod_data.append(
-                    {"op": "replace", "path": "/spec/containers/0/resources/limits/cpu", "value": new_cpu})
-                changed = True
-            if new_memory and new_memory != memory:
-                pod_data.append(
-                    {"op": "replace", "path": "/spec/containers/0/resources/limits/memory", "value": new_memory})
-                changed = True
-
-            if not changed:
-                self.log_info("Nothing changes in the kubernetes pod: " + str(vm.id))
-                return (True, vm)
-
-            # Create the container
-            namespace = vm.inf.id
-            pod_name = vm.id
-
-            headers = {'Content-Type': 'application/json-patch+json'}
-            uri = "/api/" + apiVersion + "/namespaces/" + namespace + "/pods/" + pod_name
-            body = json.dumps(pod_data)
-            resp = self.create_request('PATCH', uri, auth_data, headers, body)
+        Returns: True if the disk is added successfully and False otherwise.
+        """
+        spec = vim.vm.ConfigSpec()
+        # get all disks on a VM, set unit_number to the next available
+        for dev in vm.config.hardware.device:
+            if hasattr(dev.backing, 'fileName'):
+                unit_number = int(dev.unitNumber) + 1
+                # unit_number 7 reserved for scsi controller
+                if unit_number == 7:
+                    unit_number += 1
+                if unit_number >= 16:
+                    self.log_error("Error adding disks to a VM. We don't support this many disks")
+                    return False
+            if isinstance(dev, vim.vm.device.VirtualSCSIController):
+                controller = dev
+        # add disk here
+        dev_changes = []
+        new_disk_kb = int(disk_size) * 1024 * 1024
+        disk_spec = vim.vm.device.VirtualDeviceSpec()
+        disk_spec.fileOperation = "create"
+        disk_spec.operation = vim.vm.device.VirtualDeviceSpec.Operation.add
+        disk_spec.device = vim.vm.device.VirtualDisk()
+        disk_spec.device.backing = vim.vm.device.VirtualDisk.FlatVer2BackingInfo()
+        if disk_type == 'thin':
+            disk_spec.device.backing.thinProvisioned = True
+        disk_spec.device.backing.diskMode = 'persistent'
+        disk_spec.device.unitNumber = unit_number
+        disk_spec.device.capacityInKB = new_disk_kb
+        disk_spec.device.controllerKey = controller.key
+        dev_changes.append(disk_spec)
+        spec.deviceChange = dev_changes
+        vm.ReconfigVM(spec=spec)
+        self.log_debug("%sGB disk added to %s" % (disk_size, vm.config.name))
+        return True
 
-            if resp.status_code != 201:
-                return (False, "Error updating the Pod: " + resp.text)
-            else:
-                if new_cpu:
-                    vm.info.systems[0].setValue('cpu.count', new_cpu)
-                if new_memory:
-                    vm.info.systems[0].addFeature(
-                        Feature("memory.size", "=", new_memory, 'B'), conflict="other", missing="other")
-                return (True, self.updateVMInfo(vm, auth_data))
-
-        except Exception as ex:
-            self.log_exception(
-                "Error connecting with Kubernetes API server")
-            return (False, "ERROR: " + str(ex))
+    def attach_volumes(self, conn, node, vm):
+        """
+        Attach a the required volumes (in the RADL) to the launched instance
 
-        return (False, "Not supported")
+        Arguments:
+           - conn(:py:class:`vim.connect.SmartConnect` ): Connection object.
+           - node(:py:class:`vim.VirtualMachine` ): VM to add the disk.
+           - vm(:py:class:`IM.VirtualMachine`): VM information.
+        """
+        try:
+            if node.summary.runtime.powerState == "poweredOn" and "volumes" not in vm.__dict__.keys():
+                # Flag to set that this VM has created (or is creating) the
+                # volumes
+                vm.volumes = True
+                cont = 1
+                while vm.info.systems[0].getValue("disk." + str(cont) + ".size"):
+                    disk_size = vm.info.systems[0].getFeature("disk." + str(cont) + ".size").getValue('G')
+                    # disk_device = vm.info.systems[0].getValue("disk." + str(cont) + ".device")
+                    self.log_info("Creating a %d GB volume for the disk %d" % (int(disk_size), cont))
+                    self.add_disk(node, conn, disk_size)
+                    cont += 1
+        except Exception:
+            self.log_exception("Error creating or attaching the volume to the instance")
```

### Comparing `IM-1.9.5/IM/connectors/LibCloud.py` & `IM-1.9.6/IM/connectors/LibCloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 
     VM_STATE_MAP = {
         NodeState.RUNNING: VirtualMachine.RUNNING,
         NodeState.REBOOTING: VirtualMachine.RUNNING,
         NodeState.PENDING: VirtualMachine.PENDING,
         NodeState.TERMINATED: VirtualMachine.OFF,
         NodeState.STOPPED: VirtualMachine.STOPPED,
-        NodeState.ERROR: VirtualMachine.FAILED
+        NodeState.ERROR: VirtualMachine.FAILED,
+        NodeState.UNKNOWN: VirtualMachine.UNKNOWN
     }
     """State map"""
 
     def __init__(self, cloud_info, inf):
         self.driver = None
         CloudConnector.__init__(self, cloud_info, inf)
 
@@ -450,40 +451,30 @@
         except Exception as ex:
             self.log_exception("Error removing Elastic/Floating IPs to VM ID: " + str(vm.id))
             return False, "Error removing Elastic/Floating IPs: %s" % ex.args[0]
 
     def start(self, vm, auth_data):
         node = self.get_node_with_id(vm.id, auth_data)
         if node:
-            func = getattr(node.driver, "ex_start_node",
-                           getattr(node.driver, "ex_resume_node", None))
-            if func:
-                success = func(node)
-                if success:
-                    return (True, "")
-                else:
-                    return (False, "Error in start operations")
+            success = node.start()
+            if success:
+                return (True, "")
             else:
-                return (False, "Not supported")
+                return (False, "Error in stop operation")
         else:
             return (False, "VM not found with id: " + vm.id)
 
     def stop(self, vm, auth_data):
         node = self.get_node_with_id(vm.id, auth_data)
         if node:
-            func = getattr(node.driver, "ex_stop_node",
-                           getattr(node.driver, "ex_suspend_node", None))
-            if func:
-                success = func(node)
-                if success:
-                    return (True, "")
-                else:
-                    return (False, "Error in stop operation")
+            success = node.stop_node()
+            if success:
+                return (True, "")
             else:
-                return (False, "Not supported")
+                return (False, "Error in stop operation")
         else:
             return (False, "VM not found with id: " + vm.id)
 
     @staticmethod
     def wait_volume(volume, state='available', timeout=60):
         """
         Wait a volume (with the state extra parameter) to be in certain state.
```

### Comparing `IM-1.9.5/IM/connectors/FogBow.py` & `IM-1.9.6/IM/connectors/FogBow.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/DeployedNode.py` & `IM-1.9.6/IM/connectors/DeployedNode.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/__init__.py` & `IM-1.9.6/IM/connectors/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
-__all__ = ['CloudConnector', 'EC2', 'OCCI', 'OpenNebula', 'OpenStack', 'AzureClassic',
-           'Docker', 'GCE', 'FogBow', 'Azure', 'DeployedNode', 'Kubernetes', 'Dummy', 'vSphere', 'CloudStack']
+__all__ = ['CloudConnector', 'EC2', 'OCCI', 'OpenNebula', 'OpenStack', 'AzureClassic', 'Docker',
+           'GCE', 'FogBow', 'Azure', 'DeployedNode', 'Kubernetes', 'Dummy', 'vSphere', 'CloudStack', 'Linode']
```

### Comparing `IM-1.9.5/IM/connectors/Dummy.py` & `IM-1.9.6/IM/connectors/Dummy.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/AzureClassic.py` & `IM-1.9.6/IM/connectors/AzureClassic.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/Azure.py` & `IM-1.9.6/IM/connectors/Azure.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/OpenStack.py` & `IM-1.9.6/IM/connectors/OpenStack.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,33 +184,47 @@
                     driver.image_connection.service_region = None
                     driver.network_connection.service_region = None
                     driver.volumev2_connection.service_region = None
 
             self.driver = driver
             return driver
 
+    def guess_instance_type_gpu(self, size):
+        """Try to guess if this NodeSize has GPU support"""
+        try:
+            extra_specs = size.driver.ex_get_size_extra_specs(size.id)
+            for k, v in extra_specs.items():
+                if k.lower().find("gpu") and v.lower() not in ['false', 'no', '0']:
+                    return True
+        except Exception:
+            self.log_exception("Error trying to get flavor extra_specs.")
+        return False
+
     def get_instance_type(self, sizes, radl):
         """
         Get the name of the instance type to launch to LibCloud
 
         Arguments:
            - size(list of :py:class: `libcloud.compute.base.NodeSize`): List of sizes on a provider
            - radl(str): RADL document with the requirements of the VM to get the instance type
         Returns: a :py:class:`libcloud.compute.base.NodeSize` with the instance type to launch
         """
         instance_type_name = radl.getValue('instance_type')
 
         (cpu, cpu_op, memory, memory_op, disk_free, disk_free_op) = self.get_instance_selectors(radl, disk_unit="G")
+        gpu = radl.getValue('gpu.count')
 
         # get the node size with the lowest price, vcpus, memory and disk
         sizes.sort(key=lambda x: (x.price, x.vcpus, x.ram, x.disk))
         for size in sizes:
             comparison = cpu_op(size.vcpus, cpu)
             comparison = comparison and memory_op(size.ram, memory)
             comparison = comparison and disk_free_op(size.disk, disk_free)
+            if gpu and not self.guess_instance_type_gpu(size):
+                continue
 
             if comparison:
                 if not instance_type_name or size.name == instance_type_name:
                     return size
 
         self.log_error("No compatible size found")
         return None
@@ -360,14 +374,20 @@
             self.log_warn("Error getting volume info: %s" % get_ex_error(ex))
 
     def updateVMInfo(self, vm, auth_data):
         node = self.get_node_with_id(vm.id, auth_data)
         if node:
             vm.state = self.VM_STATE_MAP.get(node.state, VirtualMachine.UNKNOWN)
 
+            if vm.state == VirtualMachine.FAILED:
+                if 'fault' in node.extra and node.extra['fault']:
+                    error_msg = str(node.extra['fault']['message'])
+                    if error_msg not in self.error_messages:
+                        self.error_messages += error_msg
+
             try:
                 flavorId = node.extra['flavorId']
                 instance_type = node.driver.ex_get_size(flavorId)
                 self.update_system_info_from_instance(vm.info.systems[0], instance_type)
             except Exception as ex:
                 self.log_warn("Error updating VM info from flavor ID: %s" % get_ex_error(ex))
 
@@ -1528,15 +1548,18 @@
                             # wait the node to be in correct state to confirm
                             while node.extra['vm_state'] != 'resized' and cont < 30:
                                 time.sleep(2)
                                 cont += 2
                                 self.log_debug("Confirming resize of the node: %s" % node.id)
                                 node = self.get_node_with_id(vm.id, auth_data)
 
-                            success = node.driver.ex_confirm_resize(node)
+                            if node.extra['vm_state'] == 'resized':
+                                success = node.driver.ex_confirm_resize(node)
+                            else:
+                                return (False, "Error resizing VM: Resize cannot be confirmed.")
                     except Exception as ex:
                         self.log_exception("Error resizing VM.")
                         return (False, "Error resizing VM: " + str(ex))
                 else:
                     self.log_debug("Same instance_type of the current node. No need to resize.")
                     return (True, "")
```

### Comparing `IM-1.9.5/IM/connectors/OpenNebula.py` & `IM-1.9.6/IM/connectors/OpenNebula.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,18 @@
     values = ['CPU', 'MEMORY', 'NAME', 'RANK', 'REQUIREMENTS', 'VMID', 'VCPU']
     tuples = {'GRAPHICS': GRAPHICS, 'OS': OS}
     tuples_lists = {'DISK': DISK, 'NIC': NIC}
     numeric = ['CPU', 'MEMORY', 'VCPU']
     noneval = 0
 
 
+class USER_TEMPLATE(XMLObject):
+    values = ['ERROR']
+
+
 class HISTORY(XMLObject):
     values = ['SEQ', 'HOSTNAME', 'HID', 'STIME', 'ETIME', 'PSTIME',
               'PETIME', 'RSTIME', 'RETIME', 'ESTIME', 'EETIME', 'REASON']
 
 
 class VM(XMLObject):
     STATE_INIT = 0
@@ -80,15 +84,15 @@
     STATE_STOPPED = 4
     STATE_SUSPENDED = 5
     STATE_DONE = 6
     STATE_FAILED = 7
     STATE_POWEROFF = 8
     values = ['ID', 'UID', 'NAME', 'LAST_POLL', 'STATE', 'LCM_STATE',
               'DEPLOY_ID', 'MEMORY', 'CPU', 'NET_TX', 'NET_RX', 'STIME', 'ETIME']
-    tuples = {'TEMPLATE': TEMPLATE}
+    tuples = {'TEMPLATE': TEMPLATE, 'USER_TEMPLATE': USER_TEMPLATE}
     numeric = ['ID', 'UID', 'STATE', 'LCM_STATE', 'STIME', 'ETIME']
 
 
 class LEASE(XMLObject):
     values = ['IP', 'MAC', 'USED']
 
 
@@ -325,14 +329,21 @@
                 res_state = VirtualMachine.FAILED
             elif res_vm.STATE == 6 or res_vm.STATE == 8 or res_vm.STATE == 9:
                 res_state = VirtualMachine.OFF
             else:
                 res_state = VirtualMachine.UNKNOWN
             vm.state = res_state
 
+            if vm.state == VirtualMachine.FAILED:
+                # in case of error try to get the error message
+                if res_vm.USER_TEMPLATE and res_vm.USER_TEMPLATE.ERROR:
+                    error_msg = res_vm.USER_TEMPLATE.ERROR
+                    if error_msg not in self.error_messages:
+                        self.error_messages += error_msg
+
             # Update network data
             self.setIPsFromTemplate(vm, res_vm.TEMPLATE)
 
             # Update disks data
             self.setDisksFromTemplate(vm, res_vm.TEMPLATE)
 
             vm.info.systems[0].addFeature(Feature(
```

### Comparing `IM-1.9.5/IM/connectors/CloudStack.py` & `IM-1.9.6/IM/connectors/CloudStack.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -220,16 +220,16 @@
         if system.getValue('availability_zone'):
             args['location'] = system.getValue('availability_zone')
 
         keypair = None
         public_key = system.getValue("disk.0.os.credentials.public_key")
 
         if public_key and public_key.find('-----BEGIN CERTIFICATE-----') == -1:
-            public_key = None
             keypair = driver.get_key_pair(public_key)
+            public_key = None
             if keypair:
                 system.setUserKeyCredentials(system.getCredentials().username, None, keypair.private_key)
             else:
                 args["ex_keyname"] = keypair.name
         else:
             public_key, private_key = self.keygen()
             system.setUserKeyCredentials(system.getCredentials().username, None, private_key)
```

### Comparing `IM-1.9.5/IM/connectors/EC2.py` & `IM-1.9.6/IM/connectors/EC2.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/Docker.py` & `IM-1.9.6/IM/connectors/Docker.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/GCE.py` & `IM-1.9.6/IM/connectors/GCE.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/connectors/OCCI.py` & `IM-1.9.6/IM/connectors/OCCI.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/config.py` & `IM-1.9.6/IM/config.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/CtxtAgentBase.py` & `IM-1.9.6/IM/CtxtAgentBase.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/LoggerMixin.py` & `IM-1.9.6/IM/LoggerMixin.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/AppDB.py` & `IM-1.9.6/IM/AppDB.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/ConfManager.py` & `IM-1.9.6/IM/ConfManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -668,15 +668,19 @@
                     res += '      mount_path: "' + disk_mount_path + '"\n'
                     res += '      fstype: "' + disk_fstype + '"\n'
                     res += "    with_dict: '{{ ansible_devices }}'\n"
                     res += "    when: ansible_os_family != 'Windows' and ("
                     # Devices hdb, sdb, xvdb, etc
                     res += "item.key.endswith('d%s') or " % disk_device[-1]
                     # Devices nvme0n1 (NVMe type in EC2)
-                    res += "item.key.startswith('nvme%sn1')" % (ord(disk_device[-1]) - 97)
+                    res += "item.key.startswith('nvme%sn1') or " % (ord(disk_device[-1]) - 97)
+                    # Full name device
+                    res += "item.key == '%s' or " % disk_device
+                    # Use also link names (Linode case)
+                    res += "'%s' in item.value.links.ids" % disk_device
                     res += ")\n"
 
             cont += 1
 
         return res
 
     def generate_main_playbook(self, vm, group, tmp_dir):
@@ -1183,15 +1187,15 @@
                 change_creds = False
                 if self.cmp_credentials(new_creds, creds) != 0:
                     (_, new_passwd, new_public_key, new_private_key) = new_creds
                     # only change to the new password if there are a previous
                     # passwd value
                     if passwd and new_passwd:
                         self.log_info("Changing password to master VM")
-                        (out, err, code) = ssh.execute('echo "' + passwd + '" | sudo -S bash -c \'echo "' +
+                        (out, err, code) = ssh.execute('echo "' + passwd + '" | sudo -S sh -c \'echo "' +
                                                        user + ':' + new_passwd +
                                                        '" | /usr/sbin/chpasswd && echo "OK"\' 2> /dev/null')
 
                         if code == 0:
                             change_creds = True
                             ssh.password = new_passwd
                         else:
```

### Comparing `IM-1.9.5/IM/SSHRetry.py` & `IM-1.9.6/IM/SSHRetry.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/ServiceRequests.py` & `IM-1.9.6/IM/ServiceRequests.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/REST.py` & `IM-1.9.6/IM/REST.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/InfrastructureManager.py` & `IM-1.9.6/IM/InfrastructureManager.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/xmlrpcssl.py` & `IM-1.9.6/IM/xmlrpcssl.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/recipe.py` & `IM-1.9.6/IM/recipe.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/timedcall.py` & `IM-1.9.6/IM/timedcall.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/auth.py` & `IM-1.9.6/IM/auth.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/InfrastructureInfo.py` & `IM-1.9.6/IM/InfrastructureInfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,15 +583,15 @@
         if not ctxt:
             InfrastructureInfo.logger.info("Inf ID: " + str(self.id) + ": Contextualization disabled by the RADL. " +
                                            "Only wait for VM IPs.")
 
             ctxt_task.append((-2, 0, self, ['check_vm_ips']))
             ctxt_task.append((-1, 0, self, ['wait_all_vm_ips']))
 
-            self.cont_out = "Contextualization disabled by the RADL."
+            self.cont_out = "Contextualization disabled by the RADL.\n\n"
             for vm in self.get_vm_list():
                 vm.configured = True
         else:
             self.cont_out = ""
             self.configured = None
             # get the default ctxts in case of the RADL has not specified them
             ctxts = [contextualize_item(group, group, 1) for group in self.get_vm_list_by_system_name(
```

### Comparing `IM-1.9.5/IM/__init__.py` & `IM-1.9.6/IM/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 __all__ = ['auth', 'CloudInfo', 'config', 'ConfManager', 'db',
            'InfrastructureInfo', 'InfrastructureManager', 'recipe', 'request', 'REST', 'retry',
            'ServiceRequests', 'SSH', 'SSHRetry', 'timedcall', 'UnixHTTPAdapter',
            'VirtualMachine', 'VMRC', 'xmlobject']
-__version__ = '1.9.5'
+__version__ = '1.9.6'
 __author__ = 'Miguel Caballer'
 
 
 def get_ex_error(ex):
     """
     Return a secure string with the error of the exception in Py2 and Py3
     """
```

### Comparing `IM-1.9.5/IM/retry.py` & `IM-1.9.6/IM/retry.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/VirtualMachine.py` & `IM-1.9.6/IM/VirtualMachine.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import time
 import threading
 import shutil
 import string
 import json
 import tempfile
 import logging
+import sys
 from netaddr import IPNetwork, IPAddress
 
 from radl.radl import network, RADL
 from radl.radl_parse import parse_radl
 from IM.LoggerMixin import LoggerMixin
 from IM.SSH import SSH
 from IM.SSHRetry import SSHRetry
@@ -931,15 +932,22 @@
         tmp_dir = tempfile.mkdtemp()
 
         # Download the contextualization agent log
         try:
             # Get the messages of the contextualization process
             self.log_debug("Get File: " + remote_dir + '/ctxt_agent.log')
             ssh.sftp_get(remote_dir + '/ctxt_agent.log', tmp_dir + '/ctxt_agent.log')
-            with open(tmp_dir + '/ctxt_agent.log') as f:
+
+            # patch for support python2 and avoid UnicodeDecodeError in python3
+            if sys.version_info[0] < 3:
+                open_args = {}
+            else:
+                open_args = {'encoding': 'utf-8'}
+
+            with open(tmp_dir + '/ctxt_agent.log', **open_args) as f:
                 # Read removing problematic chars
                 conf_out = str("".join(list(filter(lambda x: x in string.printable,
                                                    f.read()))).encode("ascii", "replace").decode("utf-8"))
             try:
                 if delete:
                     ssh.sftp_remove(remote_dir + '/ctxt_agent.log')
             except Exception:
```

### Comparing `IM-1.9.5/IM/tosca/__init__.py` & `IM-1.9.6/IM/tosca/__init__.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/tosca/Tosca.py` & `IM-1.9.6/IM/tosca/Tosca.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/db.py` & `IM-1.9.6/IM/db.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/request.py` & `IM-1.9.6/IM/request.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/SSH.py` & `IM-1.9.6/IM/SSH.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/ansible_utils/__init__.py` & `IM-1.9.6/IM/ansible_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/ansible_utils/ansible_executor_v2.py` & `IM-1.9.6/IM/ansible_utils/ansible_executor_v2.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/ansible_utils/ansible_launcher.py` & `IM-1.9.6/IM/ansible_utils/ansible_launcher.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/VMRC.py` & `IM-1.9.6/IM/VMRC.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/openid/OpenIDClient.py` & `IM-1.9.6/IM/openid/OpenIDClient.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/openid/JWT.py` & `IM-1.9.6/IM/openid/JWT.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/tts/tts.py` & `IM-1.9.6/IM/tts/tts.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM/tts/onetts.py` & `IM-1.9.6/IM/tts/onetts.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/conf-ansible.yml` & `IM-1.9.6/contextualization/conf-ansible.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 - hosts: "{{IM_HOST}}"
   become: yes
   become_method: sudo
   gather_facts: false
   vars:
     # Ansible specific Version or "latest"
-    ANSIBLE_VERSION: 2.6.20
+    ANSIBLE_VERSION: 2.9.15
   tasks:
     - name: Set Ansible version from env if defined
       set_fact: ANSIBLE_VERSION={{ lookup('env','ANSIBLE_VERSION') }}
       when: lookup('env','ANSIBLE_VERSION') != ""
 
   ################### Some OSs does not have python by default #########################
     - name: Check Python is installed
@@ -96,14 +96,43 @@
       yum: name=gcc,libffi-devel,openssl-devel,python-devel update_cache=yes
       when: ansible_os_family == "RedHat" and ansible_distribution_major_version|int <= 6 
 
     - name: Zypper install requirements Suse
       zypper: name=python-pip,python-setuptools,gcc,python-devel,wget,libffi-devel,openssl-devel,python-cryptography,make state=present
       when: ansible_os_family == "Suse"
 
+    - name: Apk install requirements Alpine
+      package: name=py-setuptools,sshpass,openssh-client,unzip,gcc,libffi-dev,openssl-dev,musl-dev,make,wget,python2-dev
+      when: ansible_os_family == "Alpine"
+
+    - name: Apk install pip in Alpine 3.11-
+      package: name=py-pip
+      when: ansible_os_family == "Alpine" and ansible_distribution_version is version('3.12', '<')
+
+    - name: Apk install pip in Alpine 3.12+
+      shell: wget https://bootstrap.pypa.io/get-pip.py && python2 get-pip.py warn=false creates=/usr/local/bin/pip2 chdir=/tmp
+      when: ansible_os_family == "Alpine" and ansible_distribution_version is version('3.12', '>=')
+
+    - name: Move original ps in Alpine
+      command: mv /bin/ps /sbin/ps creates=/sbin/ps
+      when: ansible_os_family == "Alpine"
+
+    - name: Install ps with -p support in Alpine
+      get_url:
+        url: https://gist.githubusercontent.com/micafer/f74de4dc21a636df30d51202cbeee475/raw/388945406b9e9d225a0c7e95b97fc2515f1a17ef/ps_opt_p_enabled_for_alpine.sh
+        dest: /bin/ps
+        mode: 0755
+        owner: root
+        group: root
+      when: ansible_os_family == "Alpine"
+
+    - name: Pip install cffi Alpine
+      pip: name=wheel
+      when: ansible_os_family == "Alpine"
+
     - name: Install pip and setuptools Py3
       package: name=python3-setuptools,python3-pip
       when: ansible_python.version.major > 2
       ignore_errors: yes
 
   ######################################### Use pip to enable to set the version #############################################
```

### Comparing `IM-1.9.5/contextualization/basic.yml` & `IM-1.9.6/contextualization/basic.yml`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/ctxt_agent.py` & `IM-1.9.6/contextualization/ctxt_agent.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/ansible_install.sh` & `IM-1.9.6/contextualization/ansible_install.sh`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/__init__.py` & `IM-1.9.6/contextualization/__init__.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/AnsibleRecipes/utils/tasks/disk_format_mount.yml` & `IM-1.9.6/contextualization/AnsibleRecipes/utils/tasks/disk_format_mount.yml`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/AnsibleRecipes/utils/tasks/main.yml` & `IM-1.9.6/contextualization/AnsibleRecipes/utils/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/vpn-hosts.conf` & `IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/vpn-hosts.conf`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/ssh_known_hosts.conf` & `IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/ssh_known_hosts.conf`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/etc-vpn-hosts.conf` & `IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/etc-vpn-hosts.conf`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/AnsibleRecipes/utils/templates/hosts.conf` & `IM-1.9.6/contextualization/AnsibleRecipes/utils/templates/hosts.conf`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/ctxt_agent_dist.py` & `IM-1.9.6/contextualization/ctxt_agent_dist.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/contextualization/recipes_ansible.db` & `IM-1.9.6/contextualization/recipes_ansible.db`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/etc/im.cfg` & `IM-1.9.6/etc/im.cfg`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/etc/logging.conf` & `IM-1.9.6/etc/logging.conf`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/PKG-INFO` & `IM-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IM
-Version: 1.9.5
+Version: 1.9.6
 Summary: IM is a tool to manage virtual infrastructures on Cloud deployments
 Home-page: http://www.grycap.upv.es/im
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: micafer1@upv.es
 License: GPL version 3, http://www.gnu.org/licenses/gpl-3.0.txt
 Description: # IM - Infrastructure Manager
```

### Comparing `IM-1.9.5/NOTICE` & `IM-1.9.6/NOTICE`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/IM.egg-info/SOURCES.txt` & `IM-1.9.6/IM.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 IM/connectors/Docker.py
 IM/connectors/Dummy.py
 IM/connectors/EC2.py
 IM/connectors/FogBow.py
 IM/connectors/GCE.py
 IM/connectors/Kubernetes.py
 IM/connectors/LibCloud.py
+IM/connectors/Linode.py
 IM/connectors/OCCI.py
 IM/connectors/OpenNebula.py
 IM/connectors/OpenStack.py
 IM/connectors/__init__.py
 IM/connectors/vSphere.py
 IM/openid/JWT.py
 IM/openid/OpenIDClient.py
```

### Comparing `IM-1.9.5/IM.egg-info/PKG-INFO` & `IM-1.9.6/IM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IM
-Version: 1.9.5
+Version: 1.9.6
 Summary: IM is a tool to manage virtual infrastructures on Cloud deployments
 Home-page: http://www.grycap.upv.es/im
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: micafer1@upv.es
 License: GPL version 3, http://www.gnu.org/licenses/gpl-3.0.txt
 Description: # IM - Infrastructure Manager
```

### Comparing `IM-1.9.5/setup.py` & `IM-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `IM-1.9.5/changelog` & `IM-1.9.6/changelog`

 * *Files 0% similar despite different names*

```diff
@@ -600,7 +600,14 @@
     * Return the dns_name of a VM with the special string #N# correctly replaced.
     * TOSCA not correctly managed in case of Relationships with interfaces defined in custom types.
     * Fix error returning incorrect error msg in VM creation in OpenStack conn in case of error deleting SG.
     * Fix error returning TOSCA function values.
     * Enable CORS.
     * Fix incorrect contextualizarion in case of using vault password.
     * Fix IP public not attached in case of disabled contextualization.
+
+IM 1.9.6:
+    * Return OpenStack and OpenNebula error in case of failed VM.
+    * Enable to request GPUs in OpenStack conn.
+    * Add Linode support.
+    * Fix error when reading contextualization log in case of "strange" chars.
+    * Update ansible version to avoid errors in Ubuntu 20.04.
```

