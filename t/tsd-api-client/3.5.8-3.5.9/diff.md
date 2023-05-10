# Comparing `tmp/tsd_api_client-3.5.8.tar.gz` & `tmp/tsd_api_client-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsd_api_client-3.5.8.tar", max compression
+gzip compressed data, was "tsd_api_client-3.5.9.tar", max compression
```

## Comparing `tsd_api_client-3.5.8.tar` & `tsd_api_client-3.5.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1454 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/LICENSE
--rw-r--r--   0        0        0      704 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/README.md
--rw-r--r--   0        0        0      853 2023-04-17 07:13:54.457957 tsd_api_client-3.5.8/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/__init__.py
--rw-r--r--   0        0        0       61 2023-04-17 07:13:54.457957 tsd_api_client-3.5.8/tsdapiclient/_version.py
--rw-r--r--   0        0        0      679 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/administrator.py
--rw-r--r--   0        0        0     5273 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/authapi.py
--rw-r--r--   0        0        0      590 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/client_config.py
--rw-r--r--   0        0        0     4182 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/configurer.py
--rw-r--r--   0        0        0     1430 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/crypto.py
--rw-r--r--   0        0        0      127 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/exc.py
--rw-r--r--   0        0        0    36522 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/fileapi.py
--rw-r--r--   0        0        0     6070 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/guide.py
--rw-r--r--   0        0        0     4642 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/session.py
--rw-r--r--   0        0        0    26350 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/sync.py
--rw-r--r--   0        0        0    25828 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/tacl.py
--rw-r--r--   0        0        0     9546 2023-04-17 07:13:39.397892 tsd_api_client-3.5.8/tsdapiclient/tools.py
--rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 tsd_api_client-3.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1454 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/LICENSE
+-rw-r--r--   0        0        0      704 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/README.md
+-rw-r--r--   0        0        0      853 2023-05-10 15:41:32.125521 tsd_api_client-3.5.9/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-10 15:41:32.129521 tsd_api_client-3.5.9/tsdapiclient/_version.py
+-rw-r--r--   0        0        0      679 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/administrator.py
+-rw-r--r--   0        0        0     5273 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/authapi.py
+-rw-r--r--   0        0        0      590 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/client_config.py
+-rw-r--r--   0        0        0     4182 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/configurer.py
+-rw-r--r--   0        0        0     1430 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/crypto.py
+-rw-r--r--   0        0        0      127 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/exc.py
+-rw-r--r--   0        0        0    36522 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/fileapi.py
+-rw-r--r--   0        0        0     6070 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/guide.py
+-rw-r--r--   0        0        0     4642 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/session.py
+-rw-r--r--   0        0        0    26350 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/sync.py
+-rw-r--r--   0        0        0    26601 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/tacl.py
+-rw-r--r--   0        0        0     9926 2023-05-10 15:41:18.409550 tsd_api_client-3.5.9/tsdapiclient/tools.py
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 tsd_api_client-3.5.9/PKG-INFO
```

### Comparing `tsd_api_client-3.5.8/LICENSE` & `tsd_api_client-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/README.md` & `tsd_api_client-3.5.9/README.md`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/pyproject.toml` & `tsd_api_client-3.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsd-api-client"
-version = "3.5.8" # managed by poetry-dynamic-versioning
+version = "3.5.9" # managed by poetry-dynamic-versioning
 description = "A client for the TSD REST API"
 authors = [
     "Leon du Toit <l.c.d.toit@usit.uio.no>",
 ]
 maintainers = [
     "Eirik Haatveit <haatveit@uio.no>",
     "Milen Kouylekov <milen@uio.no>",
```

### Comparing `tsd_api_client-3.5.8/tsdapiclient/administrator.py` & `tsd_api_client-3.5.9/tsdapiclient/administrator.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/authapi.py` & `tsd_api_client-3.5.9/tsdapiclient/authapi.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/client_config.py` & `tsd_api_client-3.5.9/tsdapiclient/client_config.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/configurer.py` & `tsd_api_client-3.5.9/tsdapiclient/configurer.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/crypto.py` & `tsd_api_client-3.5.9/tsdapiclient/crypto.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/fileapi.py` & `tsd_api_client-3.5.9/tsdapiclient/fileapi.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/guide.py` & `tsd_api_client-3.5.9/tsdapiclient/guide.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/session.py` & `tsd_api_client-3.5.9/tsdapiclient/session.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/sync.py` & `tsd_api_client-3.5.9/tsdapiclient/sync.py`

 * *Files identical despite different names*

### Comparing `tsd_api_client-3.5.8/tsdapiclient/tacl.py` & `tsd_api_client-3.5.9/tsdapiclient/tacl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 import getpass
 import os
 import platform
 import sys
 
+from dataclasses import dataclass
 from textwrap import dedent
 from typing import Optional
 
 import click
 import requests
 
 from tsdapiclient import __version__
@@ -54,16 +55,18 @@
     SerialDirectoryDownloadSynchroniser,
     UploadCache,
     DownloadCache,
     UploadDeleteCache,
     DownloadDeleteCache,
 )
 from tsdapiclient.tools import (
+    EDUCLOUD_CONTACT_URL,
     HELP_URL,
     check_if_key_has_expired,
+    get_external_ip_address,
     has_api_connectivity,
     user_agent,
     debug_step,
     as_bytes,
     get_claims,
 )
 
@@ -112,26 +115,31 @@
     'downloads': downloads,
     'debugging': debugging,
     'automation': automation,
     'sync': sync,
     'encryption': encryption,
 }
 
+ENV_HTTPS_PROXY = "https_proxy"
+
+
+@dataclass(frozen=True)
+class SoftwareInfo:
+    version: str = __version__
+    os: str = platform.system()
+    cpu_arch: str = platform.uname().machine
+    python_version: str = platform.python_version()
+
+
 def print_version_info() -> None:
-    version_text = """\
-        tacl v{version}
-        - OS/Arch: {os}/{arch}
-        - Python: {pyver}\
-    """.format(
-        version=__version__,
-        os=platform.system(),
-        arch=platform.uname().machine,
-        pyver=platform.python_version()
-    )
-    print(dedent(version_text))
+    print(dedent(f"""\
+        tacl v{SoftwareInfo.version}
+        - OS/Arch: {SoftwareInfo.os}/{SoftwareInfo.cpu_arch}
+        - Python: {SoftwareInfo.python_version}\
+    """))
 
 
 def get_api_envs(ctx: str, args: list, incomplete: str) -> list:
     return [k for k, v in API_ENVS.items() if incomplete in k]
 
 
 def get_guide_options(ctx: str, args: list, incomplete: str) -> list:
@@ -201,22 +209,32 @@
         pass
     return api_key
 
 
 def check_api_connection(env: str) -> None:
     if env == "dev":
         return
-    if os.getenv("HTTPS_PROXY"):
+    if ENV_HTTPS_PROXY.casefold() in [s.casefold() for s in os.environ]:
         debug_step('skipping connection test as a proxy is set')
         return
     if not has_api_connectivity(hostname=API_ENVS[env]):
+        org = "Educloud Research" if env.startswith("ec") else "TSD"
+        contact_url = EDUCLOUD_CONTACT_URL if env.startswith("ec") else HELP_URL
         sys.exit(
             dedent(f'''\
-                The API environment hosted at {ENV[env]} is not accessible from your current network connection.
-                Please contact TSD for help: {HELP_URL}'''
+                The selected API environment appears to be inaccessible from your current network connection.
+
+                Technical details:
+                - {__package__} version {SoftwareInfo.version}
+                - Python {SoftwareInfo.python_version} on {SoftwareInfo.os}/{SoftwareInfo.cpu_arch}
+                - API environment: {env} ({ENV[env]})
+                - External IPv4 address: {get_external_ip_address()}
+
+                Please copy the above information and contact {org} for help:
+                {contact_url}'''
             )
         )
 
 
 def construct_correct_upload_path(path: str) -> str:
     if path.startswith('../'):
         return os.path.abspath(path)
```

### Comparing `tsd_api_client-3.5.8/tsdapiclient/tools.py` & `tsd_api_client-3.5.9/tsdapiclient/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,25 +23,29 @@
     RequestException,
     Timeout,
 )
 from tsdapiclient.client_config import API_VERSION
 from tsdapiclient.exc import AuthzError, AuthnError
 
 HELP_URL = 'https://www.uio.no/english/services/it/research/sensitive-data/contact/index.html'
+EDUCLOUD_CONTACT_URL = "https://www.uio.no/english/services/it/research/platforms/edu-research/help/contact-us.html"
 
 HOSTS = {
     'test': 'test.api.tsd.usit.no',
     'prod': 'api.tsd.usit.no',
     'ec-prod': 'api.fp.educloud.no',
     'ec-test': 'test.api.fp.educloud.no',
     'alt': 'alt.api.tsd.usit.no',
     'int': 'internal.api.tsd.usit.no',
     'dev': 'localhost:3003',
 }
 
+IP_LOOKUP_API_URL = "https://api.ipify.org"
+
+
 def auth_api_url(env: str, pnum: str, auth_method: str) -> str:
     endpoints = {
         'default': {
             'basic': f'{pnum}/auth/basic/token',
             'tsd': f'{pnum}/auth/tsd/token',
             'iam': f'{pnum}/auth/iam/token',
             'refresh': f'{pnum}/auth/refresh/token',
@@ -229,14 +233,22 @@
         connectivity = True
         sock.close()
     except:
         pass
     return connectivity
 
 
+def get_external_ip_address(timeout: float = 5) -> str:
+    try:
+        ip_address_request = requests.get(IP_LOOKUP_API_URL, timeout=timeout)
+    except:
+        return "UNKNOWN"
+    return ip_address_request.text
+
+
 def as_bytes(amount: str) -> int:
     """
     Change a string like '1kb' to 1000, or '12mb' to 12000000.
 
     """
     if amount.endswith('kb'):
         num_bytes = int(amount.replace('kb', ''))*1000
```

### Comparing `tsd_api_client-3.5.8/PKG-INFO` & `tsd_api_client-3.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsd-api-client
-Version: 3.5.8
+Version: 3.5.9
 Summary: A client for the TSD REST API
 Home-page: https://github.com/unioslo/tsd-api-client
 License: BSD-3-Clause
 Author: Leon du Toit
 Author-email: l.c.d.toit@usit.uio.no
 Maintainer: Eirik Haatveit
 Maintainer-email: haatveit@uio.no
```

