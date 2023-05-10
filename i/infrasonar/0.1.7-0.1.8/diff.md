# Comparing `tmp/infrasonar-0.1.7.tar.gz` & `tmp/infrasonar-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrasonar-0.1.7.tar", last modified: Mon Feb 27 08:18:35 2023, max compression
+gzip compressed data, was "infrasonar-0.1.8.tar", last modified: Wed May 10 18:56:00 2023, max compression
```

## Comparing `infrasonar-0.1.7.tar` & `infrasonar-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-27 08:18:35.786073 infrasonar-0.1.7/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-27 08:18:35.782073 infrasonar-0.1.7/.github/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-27 08:18:35.786073 infrasonar-0.1.7/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 infrasonar-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 infrasonar-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-27 08:18:35.786073 infrasonar-0.1.7/.github/workflows/
--rw-rw-r--   0 joente    (1000) joente    (1000)      690 2023-02-23 15:19:16.000000 infrasonar-0.1.7/.github/workflows/ci.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)     1203 2019-07-16 19:49:06.000000 infrasonar-0.1.7/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2020-01-31 09:24:30.000000 infrasonar-0.1.7/LICENSE
--rw-rw-r--   0 joente    (1000) joente    (1000)     3089 2023-02-27 08:18:35.786073 infrasonar-0.1.7/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     2413 2023-02-27 08:16:16.000000 infrasonar-0.1.7/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-27 08:18:35.786073 infrasonar-0.1.7/bin/
--rwxrwxr-x   0 joente    (1000) joente    (1000)    39861 2023-02-27 08:15:45.000000 infrasonar-0.1.7/bin/infrasonar
--rw-rw-r--   0 joente    (1000) joente    (1000)      269 2022-12-29 15:38:21.000000 infrasonar-0.1.7/example.yaml
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-27 08:18:35.786073 infrasonar-0.1.7/infrasonar.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)     3089 2023-02-27 08:18:35.000000 infrasonar-0.1.7/infrasonar.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      355 2023-02-27 08:18:35.000000 infrasonar-0.1.7/infrasonar.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-02-27 08:18:35.000000 infrasonar-0.1.7/infrasonar.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       39 2023-02-27 08:18:35.000000 infrasonar-0.1.7/infrasonar.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-02-27 08:18:35.000000 infrasonar-0.1.7/infrasonar.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       39 2022-12-29 15:47:18.000000 infrasonar-0.1.7/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-02-27 08:18:35.786073 infrasonar-0.1.7/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1707 2023-02-27 08:15:27.000000 infrasonar-0.1.7/setup.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.714298 infrasonar-0.1.8/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 infrasonar-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 infrasonar-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      690 2023-02-23 15:19:16.000000 infrasonar-0.1.8/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1203 2019-07-16 19:49:06.000000 infrasonar-0.1.8/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2020-01-31 09:24:30.000000 infrasonar-0.1.8/LICENSE
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3089 2023-05-10 18:56:00.718298 infrasonar-0.1.8/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2413 2023-02-27 08:16:16.000000 infrasonar-0.1.8/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/bin/
+-rwxrwxr-x   0 joente    (1000) joente    (1000)    40006 2023-05-10 18:49:43.000000 infrasonar-0.1.8/bin/infrasonar
+-rw-rw-r--   0 joente    (1000) joente    (1000)      269 2022-12-29 15:38:21.000000 infrasonar-0.1.8/example.yaml
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/infrasonar.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3089 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      355 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       39 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       39 2022-12-29 15:47:18.000000 infrasonar-0.1.8/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-05-10 18:56:00.722298 infrasonar-0.1.8/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1707 2023-05-10 18:49:52.000000 infrasonar-0.1.8/setup.py
```

### Comparing `infrasonar-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md` & `infrasonar-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md` & `infrasonar-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.7/.github/workflows/ci.yml` & `infrasonar-0.1.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.7/.gitignore` & `infrasonar-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.7/LICENSE` & `infrasonar-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.7/PKG-INFO` & `infrasonar-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrasonar
-Version: 0.1.7
+Version: 0.1.8
 Summary: InfraSonar Toolkit
 Home-page: https://github.com/infrasonar/toolkit
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: GPLv3
 Keywords: infrasonar monitoring toolkit util
 Platform: UNKNOWN
```

### Comparing `infrasonar-0.1.7/README.md` & `infrasonar-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.7/bin/infrasonar` & `infrasonar-0.1.8/bin/infrasonar`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import yamlloader
 from aiohttp import ClientSession
 from collections import OrderedDict
 from dataclasses import dataclass
 from setproctitle import setproctitle
 from typing import Any, Optional, Dict, List, Tuple
 
-__version__ = '0.1.7'  # Update version in setup as well
+__version__ = '0.1.8'  # Update version in setup as well
 
 
 _labels_example = """
 Invalid "labels". Expecting something like:
 
 labels:
   dns: 1409
@@ -120,14 +120,19 @@
 def _json_headers(token: str):
     return {
         'Authorization': f'Bearer {token}',
         'Content-Type': 'application/json'
     }
 
 
+def _assetstr(name: str, asset_id: Optional[int]):
+    return \
+        f'asset "{name}" (assetId: {"new" if asset_id is None else asset_id})'
+
+
 _yaml_keys = {
     'container',
     'token',
     'labels',
     'configs',
     'assets'
 }
@@ -579,15 +584,15 @@
     for prop in ('name', 'kind', 'description', 'mode'):
         val = dest.get(prop)
         if val is not None and orig[prop] != val:
             changes = make_changes(changes)
             if not silent:
                 print(
                     f'Change {prop} to "{val}" '
-                    f'for asset "{name}" ({asset_id})')
+                    f'for {_assetstr(name, asset_id)}')
 
             if not dry_run:
                 await asyncio.sleep(0.5)
                 data = {prop: val}
                 url = _join(api, f'asset/{asset_id}/{prop}')
                 async with ClientSession(headers=jheaders) as session:
                     async with session.patch(url, json=data, ssl=vssl) as r:
@@ -604,15 +609,15 @@
             control = _collectors.get(key)
             if oc and config_eq(oc.get('config'), config, control):
                 continue
 
             changes = make_changes(changes)
             if not silent:
                 prefix = 'Update collector' if oc else 'Add collector'
-                print(f'{prefix} "{key}" on asset "{name}" ({asset_id})')
+                print(f'{prefix} "{key}" on {_assetstr(name, asset_id)}')
 
             if not dry_run:
                 await asyncio.sleep(0.5)
                 url = _join(api, f'asset/{asset_id}/collector/{key}')
                 if config is None:
                     async with ClientSession(headers=headers) as session:
                         async with session.post(url, ssl=vssl) as r:
@@ -632,15 +637,15 @@
             dkeys = {c['key'] for c in collectors}
             okeys = {c['key'] for c in orig['collectors']}
             rkeys = okeys - dkeys
             for key in rkeys:
                 changes = make_changes(changes)
                 if not silent:
                     prefix = 'Remove collector'
-                    print(f'{prefix} "{key}" from asset "{name}" ({asset_id})')
+                    print(f'{prefix} "{key}" from {_assetstr(name, asset_id)}')
                 if not dry_run:
                     await asyncio.sleep(0.5)
                     url = _join(api, f'asset/{asset_id}/collector/{key}')
                     async with ClientSession(headers=headers) as session:
                         async with session.delete(url, ssl=vssl) as r:
                             if r.status != 204:
                                 msg = await r.text()
@@ -651,15 +656,15 @@
     if labels is not None:
         for lid in labels:
             if lid in orig['labels']:
                 continue
 
             changes = make_changes(changes)
             if not silent:
-                print(f'Add label {lid} on asset "{name}" ({asset_id})')
+                print(f'Add label {lid} on {_assetstr(name, asset_id)}')
 
             if not dry_run:
                 await asyncio.sleep(0.5)
                 url = _join(api, f'asset/{asset_id}/label/{lid}')
                 async with ClientSession(headers=headers) as session:
                     async with session.post(url, ssl=vssl) as r:
                         if r.status != 204:
@@ -667,15 +672,15 @@
                             raise Exception(f'{msg} (error code: {r.status})')
 
         if not aa.add_only:
             rlabels = set(orig['labels']) - set(labels)
             for lid in rlabels:
                 changes = make_changes(changes)
                 if not silent:
-                    print(f'Remove label {lid} on asset "{name}" ({asset_id})')
+                    print(f'Remove label {lid} on {_assetstr(name, asset_id)}')
 
                 if not dry_run:
                     await asyncio.sleep(0.5)
                     url = _join(api, f'asset/{asset_id}/label/{lid}')
                     async with ClientSession(headers=headers) as session:
                         async with session.delete(url, ssl=vssl) as r:
                             if r.status != 204:
```

### Comparing `infrasonar-0.1.7/infrasonar.egg-info/PKG-INFO` & `infrasonar-0.1.8/infrasonar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrasonar
-Version: 0.1.7
+Version: 0.1.8
 Summary: InfraSonar Toolkit
 Home-page: https://github.com/infrasonar/toolkit
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: GPLv3
 Keywords: infrasonar monitoring toolkit util
 Platform: UNKNOWN
```

### Comparing `infrasonar-0.1.7/setup.py` & `infrasonar-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with open('README.md', 'r') as f:
         long_description = f.read()
 except IOError:
     long_description = ''
 
 setup(
     name='infrasonar',
-    version='0.1.7',  # Update version in infrasonar as well
+    version='0.1.8',  # Update version in infrasonar as well
     description='InfraSonar Toolkit',
     url='https://github.com/infrasonar/toolkit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jeroen van der Heijden',
     author_email='jeroen@cesbit.com',
     scripts=['bin/infrasonar'],
```

