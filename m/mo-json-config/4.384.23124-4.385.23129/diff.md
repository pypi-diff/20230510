# Comparing `tmp/mo_json_config-4.384.23124-py2.py3-none-any.whl.zip` & `tmp/mo_json_config-4.385.23129-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15685 bytes, number of entries: 8
+Zip file size: 15682 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat    11053 b- defN 23-Apr-29 14:14 mo_json_config/__init__.py
 -rw-rw-rw-  2.0 fat     2411 b- defN 23-Apr-29 14:14 mo_json_config/configuration.py
 -rw-rw-rw-  2.0 fat      763 b- defN 20-Jul-08 11:16 mo_json_config/convert.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-May-04 10:55 mo_json_config-4.384.23124.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    11524 b- defN 23-May-04 10:55 mo_json_config-4.384.23124.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-04 10:55 mo_json_config-4.384.23124.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-04 10:55 mo_json_config-4.384.23124.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      711 b- defN 23-May-04 10:55 mo_json_config-4.384.23124.dist-info/RECORD
-8 files, 43312 bytes uncompressed, 14435 bytes compressed:  66.7%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-May-09 23:37 mo_json_config-4.385.23129.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    11524 b- defN 23-May-09 23:37 mo_json_config-4.385.23129.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-09 23:37 mo_json_config-4.385.23129.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-09 23:37 mo_json_config-4.385.23129.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      711 b- defN 23-May-09 23:37 mo_json_config-4.385.23129.dist-info/RECORD
+8 files, 43312 bytes uncompressed, 14432 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: mo_json_config/configuration.py
 Comment: 
 
 Filename: mo_json_config/convert.py
 Comment: 
 
-Filename: mo_json_config-4.384.23124.dist-info/LICENSE.txt
+Filename: mo_json_config-4.385.23129.dist-info/LICENSE.txt
 Comment: 
 
-Filename: mo_json_config-4.384.23124.dist-info/METADATA
+Filename: mo_json_config-4.385.23129.dist-info/METADATA
 Comment: 
 
-Filename: mo_json_config-4.384.23124.dist-info/WHEEL
+Filename: mo_json_config-4.385.23129.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json_config-4.384.23124.dist-info/top_level.txt
+Filename: mo_json_config-4.385.23129.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json_config-4.384.23124.dist-info/RECORD
+Filename: mo_json_config-4.385.23129.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mo_json_config-4.384.23124.dist-info/LICENSE.txt` & `mo_json_config-4.385.23129.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `mo_json_config-4.384.23124.dist-info/METADATA` & `mo_json_config-4.385.23129.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json-config
-Version: 4.384.23124
+Version: 4.385.23129
 Summary: More JSON Configuration! JSON configuration files with `$ref` and template overlays
 Home-page: https://github.com/klahnakoski/mo-json-config
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: hjson
 Requires-Dist: mo-dots (==9.376.23121)
-Requires-Dist: mo-files (==6.384.23124)
+Requires-Dist: mo-files (==6.385.23129)
 Requires-Dist: mo-future (==7.340.23006)
-Requires-Dist: mo-json (==6.384.23124)
-Requires-Dist: mo-logs (==7.378.23124)
+Requires-Dist: mo-json (==6.385.23129)
+Requires-Dist: mo-logs (==7.385.23129)
 Requires-Dist: requests
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: keyring ; extra == 'tests'
 Requires-Dist: boto3 ; extra == 'tests'
 Requires-Dist: moto ; extra == 'tests'
 Requires-Dist: pyyaml ; extra == 'tests'
```

## Comparing `mo_json_config-4.384.23124.dist-info/RECORD` & `mo_json_config-4.385.23129.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 mo_json_config/__init__.py,sha256=29Z-UDXEtVDPApQB6EloAMzND_MtG9TZiW3zxHBY3bs,11053
 mo_json_config/configuration.py,sha256=SKpP26n1CzyiGyZpZ1FgzlZ_oL3m-aJVIcZpm_IxaSg,2411
 mo_json_config/convert.py,sha256=hAgOJpIs7bbnJCdQG4Ldg3rzQKikZwaS7VltSU_xhm0,763
-mo_json_config-4.384.23124.dist-info/LICENSE.txt,sha256=x290DRUhub7ZynoErVJsMQSTxiYhsTQdYjtDFzZTOzA,16725
-mo_json_config-4.384.23124.dist-info/METADATA,sha256=l6epT39C77o1LA57JwjV8rOcKwR6hvRG_QXMz7iwmbM,11524
-mo_json_config-4.384.23124.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_json_config-4.384.23124.dist-info/top_level.txt,sha256=x4UKOkmRDxEplnJZkDPS5qyG1HkuVXfCXNu-BrUn8Qg,15
-mo_json_config-4.384.23124.dist-info/RECORD,,
+mo_json_config-4.385.23129.dist-info/LICENSE.txt,sha256=x290DRUhub7ZynoErVJsMQSTxiYhsTQdYjtDFzZTOzA,16725
+mo_json_config-4.385.23129.dist-info/METADATA,sha256=6ldOvVkqmngYHfqq9d4nJC93mP7KoB_OJYD56mConIY,11524
+mo_json_config-4.385.23129.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_json_config-4.385.23129.dist-info/top_level.txt,sha256=x4UKOkmRDxEplnJZkDPS5qyG1HkuVXfCXNu-BrUn8Qg,15
+mo_json_config-4.385.23129.dist-info/RECORD,,
```

