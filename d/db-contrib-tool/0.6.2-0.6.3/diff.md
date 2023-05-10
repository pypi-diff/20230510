# Comparing `tmp/db_contrib_tool-0.6.2.tar.gz` & `tmp/db_contrib_tool-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_contrib_tool-0.6.2.tar", max compression
+gzip compressed data, was "db_contrib_tool-0.6.3.tar", max compression
```

## Comparing `db_contrib_tool-0.6.2.tar` & `db_contrib_tool-0.6.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     5222 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/README.md
--rw-r--r--   0        0        0     2139 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       13 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/__init__.py
--rw-r--r--   0        0        0      883 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/cli.py
--rw-r--r--   0        0        0        0 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/__init__.py
--rw-r--r--   0        0        0     7147 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/download_client.py
--rw-r--r--   0        0        0     1329 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/file_service.py
--rw-r--r--   0        0        0     2636 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/git_client.py
--rw-r--r--   0        0        0      305 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/io_client.py
--rw-r--r--   0        0        0      984 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/platform_details.py
--rw-r--r--   0        0        0     2524 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/resmoke_proxy.py
--rw-r--r--   0        0        0     6667 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/config/setup_repro_env_config.yml
--rw-r--r--   0        0        0     5999 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/config.py
--rw-r--r--   0        0        0     8844 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/__init__.py
--rw-r--r--   0        0        0     4639 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/cli.py
--rw-r--r--   0        0        0      110 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
--rw-r--r--   0        0        0      418 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
--rw-r--r--   0        0        0       52 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
--rw-r--r--   0        0        0        0 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/services/__init__.py
--rw-r--r--   0        0        0     9131 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/services/evergreen_service.py
--rw-r--r--   0        0        0     2404 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/services/git_service.py
--rw-r--r--   0        0        0     2027 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/services/platform_service.py
--rw-r--r--   0        0        0    13919 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/README.md
--rw-r--r--   0        0        0       13 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/__init__.py
--rw-r--r--   0        0        0    17392 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
--rw-r--r--   0        0        0     8912 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/cli.py
--rw-r--r--   0        0        0     8290 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/download_service.py
--rw-r--r--   0        0        0     4513 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
--rw-r--r--   0        0        0     5586 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/release_models.py
--rw-r--r--   0        0        0     3155 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/request_models.py
--rw-r--r--   0        0        0    11018 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
--rw-r--r--   0        0        0      614 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/README.md
--rw-r--r--   0        0        0        0 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/__init__.py
--rw-r--r--   0        0        0     4190 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/cli.py
--rw-r--r--   0        0        0     4798 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
--rw-r--r--   0        0        0    24229 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/mongosymb.py
--rw-r--r--   0        0        0     2269 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/usage_analytics.py
--rw-r--r--   0        0        0      235 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/__init__.py
--rw-r--r--   0        0        0     1855 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/build_system_options.py
--rw-r--r--   0        0        0     2160 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/evergreen_conn.py
--rw-r--r--   0        0        0     1085 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/filesystem.py
--rw-r--r--   0        0        0    10608 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/oauth.py
--rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.2/setup.py
--rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/README.md
+-rw-r--r--   0        0        0     2139 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/__init__.py
+-rw-r--r--   0        0        0      883 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/cli.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/clients/__init__.py
+-rw-r--r--   0        0        0     7147 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/clients/download_client.py
+-rw-r--r--   0        0        0     1329 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/clients/file_service.py
+-rw-r--r--   0        0        0     2636 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/clients/git_client.py
+-rw-r--r--   0        0        0      305 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/clients/io_client.py
+-rw-r--r--   0        0        0      984 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/clients/platform_details.py
+-rw-r--r--   0        0        0     2524 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/clients/resmoke_proxy.py
+-rw-r--r--   0        0        0     9291 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/config/setup_repro_env_config.yml
+-rw-r--r--   0        0        0     5999 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/config.py
+-rw-r--r--   0        0        0     8844 2023-05-10 07:35:06.365389 db_contrib_tool-0.6.3/src/db_contrib_tool/evg_aware_bisect/__init__.py
+-rw-r--r--   0        0        0     4639 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/evg_aware_bisect/cli.py
+-rw-r--r--   0        0        0      110 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
+-rw-r--r--   0        0        0      418 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
+-rw-r--r--   0        0        0       52 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
+-rw-r--r--   0        0        0        0 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/services/__init__.py
+-rw-r--r--   0        0        0     9131 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/services/evergreen_service.py
+-rw-r--r--   0        0        0     2404 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/services/git_service.py
+-rw-r--r--   0        0        0     2029 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/services/platform_service.py
+-rw-r--r--   0        0        0    13919 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/README.md
+-rw-r--r--   0        0        0       13 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/__init__.py
+-rw-r--r--   0        0        0    17392 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
+-rw-r--r--   0        0        0     8912 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/cli.py
+-rw-r--r--   0        0        0     8290 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/download_service.py
+-rw-r--r--   0        0        0     4513 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
+-rw-r--r--   0        0        0     5586 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/release_models.py
+-rw-r--r--   0        0        0     3155 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/request_models.py
+-rw-r--r--   0        0        0    11018 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
+-rw-r--r--   0        0        0      614 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/__init__.py
+-rw-r--r--   0        0        0     4190 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/cli.py
+-rw-r--r--   0        0        0     4798 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
+-rw-r--r--   0        0        0    24229 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/mongosymb.py
+-rw-r--r--   0        0        0     2269 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/usage_analytics.py
+-rw-r--r--   0        0        0      235 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/utils/build_system_options.py
+-rw-r--r--   0        0        0     2160 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/utils/evergreen_conn.py
+-rw-r--r--   0        0        0     1085 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/utils/filesystem.py
+-rw-r--r--   0        0        0    10608 2023-05-10 07:35:06.369390 db_contrib_tool-0.6.3/src/db_contrib_tool/utils/oauth.py
+-rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.3/setup.py
+-rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.3/PKG-INFO
```

### Comparing `db_contrib_tool-0.6.2/README.md` & `db_contrib_tool-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/pyproject.toml` & `db_contrib_tool-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "db-contrib-tool"
-version = "0.6.2"
+version = "0.6.3"
 description = "The `db-contrib-tool` - MongoDB's tool for contributors."
 authors = ["DAG team <dev-prod-dag@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/10gen/db-contrib-tool"
 include = [
     "src/db_contrib_tool/bisect/*.sh",
     "src/db_contrib_tool/config/*.yml",
```

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/cli.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/download_client.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/clients/download_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/file_service.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/clients/file_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/git_client.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/platform_details.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/clients/platform_details.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/resmoke_proxy.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/clients/resmoke_proxy.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/config/setup_repro_env_config.yml` & `db_contrib_tool-0.6.3/src/db_contrib_tool/config/setup_repro_env_config.yml`

 * *Files 18% similar despite different names*

```diff
@@ -20,24 +20,30 @@
       - compile
     symbols:
       - compile
     push:
       - push
 
 evergreen_buildvariants:
+####################
+### Ubuntu 16.04 ###
+####################
   - name: ubuntu1604
     edition: targeted
     platform: ubuntu1604
     architecture: x86_64
 
   - name: enterprise-ubuntu1604-64
     edition: enterprise
     platform: ubuntu1604
     architecture: x86_64
 
+####################
+### Ubuntu 18.04 ###
+####################
   - name: ubuntu1804
     edition: targeted
     platform: ubuntu1804
     architecture: x86_64
 
   - name: enterprise-ubuntu1804-64
     edition: enterprise
@@ -65,14 +71,17 @@
     architecture: s390x
 
   - name: enterprise-ubuntu1804-s390x
     edition: enterprise
     platform: ubuntu1804
     architecture: s390x
 
+####################
+### Ubuntu 20.04 ###
+####################
   - name: ubuntu2004
     edition: targeted
     platform: ubuntu2004
     architecture: x86_64
 
   - name: enterprise-ubuntu2004-64
     edition: enterprise
@@ -85,109 +94,206 @@
     architecture: aarch64
 
   - name: enterprise-ubuntu2004-arm64
     edition: enterprise
     platform: ubuntu2004
     architecture: aarch64
 
+####################
+### Ubuntu 22.04 ###
+####################
+  - name: ubuntu2204
+    edition: targeted
+    platform: ubuntu2204
+    architecture: x86_64
+
+  - name: enterprise-ubuntu2204-64
+    edition: enterprise
+    platform: ubuntu2204
+    architecture: x86_64
+
+  - name: ubuntu2204-arm64
+    edition: targeted
+    platform: ubuntu2204
+    architecture: aarch64
+
+  - name: enterprise-ubuntu2204-arm64
+    edition: enterprise
+    platform: ubuntu2204
+    architecture: aarch64
+
+##############
+### Amazon ###
+##############
   - name: amazon
     edition: targeted
     platform: amazon
     architecture: x86_64
 
   - name: enterprise-linux-64-amazon-ami
     edition: enterprise
     platform: amzn64
     architecture: x86_64
 
+################
+### Amazon 2 ###
+################
   - name: amazon2
     edition: targeted
     platform: amazon2
     architecture: x86_64
 
   - name: enterprise-amazon2
     edition: enterprise
     platform: amazon2
     architecture: x86_64
 
+  - name: amazon2-arm64
+    edition: targeted
+    platform: amazon2
+    architecture: aarch64
+
   - name: enterprise-amazon2-arm64
     edition: enterprise
     platform: amazon2
     architecture: aarch64
 
+###################
+### Amazon 2022 ###
+###################
+  - name: amazon2022
+    edition: targeted
+    platform: amazon2022
+    architecture: x86_64
+
+  - name: enterprise-amazon2022
+    edition: enterprise
+    platform: amazon2022
+    architecture: x86_64
+
+  - name: amazon2022-arm64
+    edition: targeted
+    platform: amazon2022
+    architecture: aarch64
+
+  - name: enterprise-amazon2022-arm64
+    edition: enterprise
+    platform: amazon2022
+    architecture: aarch64
+
+##############
+### RHEL 6 ###
+##############
   - name: rhel62
     edition: targeted
     platform: rhel62
     architecture: x86_64
 
   - name: enterprise-rhel-62-64-bit
     edition: enterprise
     platform: rhel62
     architecture: x86_64
 
+  - name: rhel-67-s390x
+    edition: targeted
+    platform: rhel67
+    architecture: s390x
+
+  - name: enterprise-rhel-67-s390x
+    edition: enterprise
+    platform: rhel67
+    architecture: s390x
+
+##############
+### RHEL 7 ###
+##############
   - name: rhel70
     edition: targeted
     platform: rhel70
     architecture: x86_64
 
   - name: enterprise-rhel-70-64-bit
     edition: enterprise
     platform: rhel70
     architecture: x86_64
 
+  - name: enterprise-rhel-71-ppc64le
+    edition: enterprise
+    platform: rhel71
+    architecture: ppc64le
+
+  - name: rhel-72-s390x
+    edition: targeted
+    platform: rhel72
+    architecture: s390x
+
+  - name: enterprise-rhel-72-s390x
+    edition: enterprise
+    platform: rhel72
+    architecture: s390x
+
+##############
+### RHEL 8 ###
+##############
   - name: rhel80
     edition: targeted
     platform: rhel80
     architecture: x86_64
 
   - name: enterprise-rhel-80-64-bit
     edition: enterprise
     platform: rhel80
     architecture: x86_64
 
+  - name: enterprise-rhel-81-ppc64le
+    edition: enterprise
+    platform: rhel81
+    architecture: ppc64le
+
   - name: rhel-82-arm64
     edition: targeted
     platform: rhel82
-    architecture: arm64
+    architecture: aarch64
 
   - name: enterprise-rhel-82-arm64
     edition: enterprise
     platform: rhel82
-    architecture: arm64
-
-  - name: enterprise-rhel-71-ppc64le
-    edition: enterprise
-    platform: rhel71
-    architecture: ppc64le
+    architecture: aarch64
 
-  - name: enterprise-rhel-81-ppc64le
+  - name: enterprise-rhel-83-s390x
     edition: enterprise
-    platform: rhel81
-    architecture: ppc64le
+    platform: rhel83
+    architecture: s390x
 
-  - name: rhel-67-s390x
+##############
+### RHEL 9 ###
+##############
+  - name: rhel90
     edition: targeted
-    platform: rhel67
-    architecture: s390x
+    platform: rhel90
+    architecture: x86_64
 
-  - name: enterprise-rhel-67-s390x
+  - name: enterprise-rhel-90-64-bit
     edition: enterprise
-    platform: rhel67
-    architecture: s390x
+    platform: rhel90
+    architecture: x86_64
 
-  - name: rhel-72-s390x
+  - name: rhel90-arm64
     edition: targeted
-    platform: rhel72
-    architecture: s390x
+    platform: rhel90
+    architecture: aarch64
 
-  - name: enterprise-rhel-72-s390x
+  - name: enterprise-rhel90-arm64
     edition: enterprise
-    platform: rhel72
-    architecture: s390x
+    platform: rhel90
+    architecture: aarch64
 
+####################
+### SUSE/SLES 12 ###
+####################
   - name: suse12
     edition: targeted
     platform: suse12
     architecture: x86_64
 
   - name: enterprise-suse12-64
     edition: enterprise
@@ -200,44 +306,56 @@
     architecture: s390x
 
   - name: enterprise-suse12-s390x
     edition: enterprise
     platform: suse12
     architecture: s390x
 
+####################
+### SUSE/SLES 15 ###
+####################
   - name: suse15
     edition: targeted
     platform: suse15
     architecture: x86_64
 
   - name: enterprise-suse15-64
     edition: enterprise
     platform: suse15
     architecture: x86_64
 
+################
+### Debian 9 ###
+################
   - name: debian92
     edition: targeted
     platform: debian92
     architecture: x86_64
 
   - name: enterprise-debian92-64
     edition: enterprise
     platform: debian92
     architecture: x86_64
 
+#################
+### Debian 10 ###
+#################
   - name: debian10
     edition: targeted
     platform: debian10
     architecture: x86_64
 
   - name: enterprise-debian10-64
     edition: enterprise
     platform: debian10
     architecture: x86_64
 
+#################
+### Debian 11 ###
+#################
   - name: debian11
     edition: targeted
     platform: debian11
     architecture: x86_64
 
   - name: enterprise-debian11-64
     edition: enterprise
@@ -253,14 +371,17 @@
 
   - name: enterprise-debian10-64
     edition: enterprise
     platform: debian11
     architecture: x86_64
     versions: ["4.2", "4.4", "5.3"]
 
+###############
+### Windows ###
+###############
   - name: windows
     edition: base
     platform: windows
     architecture: x86_64
 
   - name: windows-64-2k8-ssl
     edition: base
@@ -281,34 +402,50 @@
 
   - name: enterprise-windows-64-2k8
     edition: enterprise
     platform: windows
     architecture: x86_64
     versions: ["4.0", "4.2"]
 
+#############
+### MacOS ###
+#############
   - name: macos
     edition: base
-    platform: osx
+    platform: macos
     architecture: x86_64
 
   - name: osx-1010
     edition: base
     platform: osx-ssl
     architecture: x86_64
     versions: ["4.0"]
 
   - name: enterprise-macos
     edition: enterprise
-    platform: osx
+    platform: macos
     architecture: x86_64
 
   - name: enterprise-osx-1010
     edition: enterprise
     platform: osx
     architecture: x86_64
     versions: ["4.0"]
 
+  - name: macos-arm64
+    edition: base
+    platform: macos
+    architecture: arm64
+
+  - name: enterprise-macos-arm64
+    edition: enterprise
+    platform: macos
+    architecture: arm64
+
+############
+### Misc ###
+############
   - name: linux-64
     edition: base
     platform: linux_x86_64
     architecture: x86_64
     versions: ["4.0"]
```

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/config.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/config.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/__init__.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/evg_aware_bisect/__init__.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/cli.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/evg_aware_bisect/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/services/evergreen_service.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/services/evergreen_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/services/git_service.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/services/git_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/services/platform_service.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/services/platform_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         :param version: Mongo version that should be targeted.
         :return: Platform to target.
         """
         system_name = self.platform_details_client.get_platform_system()
         platform_name = None
 
         if system_name == "Darwin":
-            platform_name = "osx"
+            platform_name = "macos"
 
         elif system_name == "Windows":
             platform_name = "windows"
             if edition == "base" and version == "4.2":
                 platform_name += "_x86_64-2012plus"
 
         elif system_name == "Linux":
```

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/README.md` & `db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/cli.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/download_service.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/download_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/release_discovery_service.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/release_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/release_models.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/release_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/request_models.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/request_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/setup_repro_env.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/setup_repro_env/setup_repro_env.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/README.md` & `db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/cli.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/mongosymb.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/symbolizer/mongosymb.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/usage_analytics.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/usage_analytics.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/utils/build_system_options.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/utils/build_system_options.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/utils/evergreen_conn.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/utils/evergreen_conn.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/utils/filesystem.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/src/db_contrib_tool/utils/oauth.py` & `db_contrib_tool-0.6.3/src/db_contrib_tool/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.2/setup.py` & `db_contrib_tool-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'tenacity>=8.0.1,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['db-contrib-tool = db_contrib_tool.cli:cli']}
 
 setup_kwargs = {
     'name': 'db-contrib-tool',
-    'version': '0.6.2',
+    'version': '0.6.3',
     'description': "The `db-contrib-tool` - MongoDB's tool for contributors.",
     'long_description': '# db-contrib-tool\n\nThe `db-contrib-tool` - MongoDB\'s tools for contributors.\n\n## Table of contents\n\n- [db-contrib-tool](#db-contrib-tool)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor\'s Guide (local development)](#contributors-guide-local-development)\n    - [Install project dependencies](#install-project-dependencies)\n    - [Run command line tool (local development)](#run-command-line-tool-local-development)\n    - [Run linters](#run-linters)\n    - [Run tests](#run-tests)\n    - [Pre-commit](#pre-commit)\n    - [Testing changes in mongo](#testing-changes-in-mongo)\n    - [Test pipx package](#test-pipx-package)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThe command line tool with various subcommands:\n- `bisect` - performs an evergreen-aware git-bisect to find the \'last passing version\' and \'first failing version\' of mongo\n- `setup-repro-env`\n  - [README.md](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/setup_repro_env/README.md)\n  - downloads and installs:\n    - particular MongoDB versions\n    - debug symbols\n    - artifacts (including resmoke, python scripts etc)\n    - python venv for resmoke, python scripts etc\n- `symbolize`\n  - [README.md](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/symbolizer/README.md)\n  - Symbolizes stacktraces from recent `mongod` and `mongos` binaries compiled in Evergreen, including patch builds, mainline builds, and release/production builds.\n  - Requires authenticating to an internal MongoDB symbol mapping service.\n\n## Dependencies\n\n- Python 3.9 or later (python3 from the [MongoDB Toolchain](https://github.com/10gen/toolchain-builder/blob/master/INSTALL.md) is highly recommended)\n\n## Installation\n\nMake sure [dependencies](#dependencies) are installed.\nUse [pipx](https://pypa.github.io/pipx/) to install db-contrib-tool that will be available globally on your machine:\n```bash\n$ python3 -m pip install pipx\n$ python3 -m pipx ensurepath\n```\n\nInstalling db-contrib-tool:\n```bash\n$ python3 -m pipx install db-contrib-tool\n```\n\nUpgrading db-contrib-tool:\n```bash\n$ python3 -m pipx upgrade db-contrib-tool\n```\n\n## Usage\n\nPrint out help message:\n```bash\n$ db-contrib-tool -h\n```\nMore information on the usage of `setup-repro-env` can be found [here](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/setup_repro_env/README.md).\n\n## Contributor\'s Guide (local development)\n\n### Install project dependencies\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management.\n```bash\n$ poetry install\n```\n\n### Run command line tool (local development)\n\n```bash\n$ ENV=DEV poetry run db-contrib-tool -h\n```\n\n### Run linters\n\n```bash\n$ poetry run isort src tests\n$ poetry run black src tests\n```\n\n### Run tests\n\n```bash\n$ poetry run pytest\n```\n\n### Pre-commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time.<br>\nTo enable pre-commit on your local repository run:\n```bash\n$ poetry run pre-commit install\n```\n\nTo run pre-commit manually:\n```bash\n$ poetry run pre-commit run\n```\n\n### Testing changes in mongo\n\nThis tool is used to help run tests in the mongodb/mongo repository. On occasion, it may be\ndesirable to run a mongodb-mongo-* patch build with in-flight changes to this repository. The\nfollowing steps can be take to accomplish that.\n\n- Create a branch with the changes you wish to test.\n- Push the branch to the origin repository: `git push -u origin <branch_name>`.\n- In the "mongo" repository, edit the [evergreen/prelude_db_contrib_tool.sh](https://github.com/10gen/mongo/blob/b1a3a357af735a53981737d91fd49e5e3ae67b95/evergreen/prelude_db_contrib_tool.sh#L10)\n  to install from the git repository instead of from pypi:\n\n  ```bash\n  pipx install "git+ssh://git@github.com/<user_name>/db-contrib-tool.git@<branch_name>" || exit 1\n  ```\n\n- Create a patch build.\n\nThe patch build should now pull down the changes from your branch instead of using the published\ndb-contrib-tool.\n\n**Note**: Since the db-contrib-tool is pulled from your branch, if you need to make additional\nchanges to the tool, you can just push to the branch and then restart the desired tasks. There is\nno need to create an additional patch build unless you also need to make updates to the mongo\nrepository.\n\n### Test pipx package\n\nPipx installation recommendations can be found in [installation](#installation) section.<br>\nThe tool can be installed via pipx from your local repo:\n```bash\n$ python3 -m pipx install /path/to/db-contrib-tool\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a Github Pull Request for code review.\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to pypi is automatically triggered on merges to main.\n',
     'author': 'DAG team',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/10gen/db-contrib-tool',
```

### Comparing `db_contrib_tool-0.6.2/PKG-INFO` & `db_contrib_tool-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-contrib-tool
-Version: 0.6.2
+Version: 0.6.3
 Summary: The `db-contrib-tool` - MongoDB's tool for contributors.
 Home-page: https://github.com/10gen/db-contrib-tool
 Author: DAG team
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

