# Comparing `tmp/iam_actions-1.2.20230509.tar.gz` & `tmp/iam_actions-1.2.20230510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230509.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230510.tar", max compression
```

## Comparing `iam_actions-1.2.20230509.tar` & `iam_actions-1.2.20230510.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/README.md
--rw-r--r--   0        0        0      228 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/__init__.py
--rw-r--r--   0        0        0  4248083 2023-05-09 02:28:42.381904 iam_actions-1.2.20230509/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-09 02:27:11.260299 iam_actions-1.2.20230509/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-09 02:27:11.260299 iam_actions-1.2.20230509/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-09 02:27:11.260299 iam_actions-1.2.20230509/iam_actions/generate/services.py
--rw-r--r--   0        0        0   546214 2023-05-09 02:28:42.381904 iam_actions-1.2.20230509/iam_actions/policies.json
--rw-r--r--   0        0        0   193734 2023-05-09 02:28:42.381904 iam_actions-1.2.20230509/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   529800 2023-05-09 02:28:42.381904 iam_actions-1.2.20230509/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-09 02:28:43.121917 iam_actions-1.2.20230509/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230509/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230509/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/README.md
+-rw-r--r--   0        0        0      228 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4248257 2023-05-10 02:27:05.651587 iam_actions-1.2.20230510/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-10 02:24:55.508541 iam_actions-1.2.20230510/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   546378 2023-05-10 02:27:05.651587 iam_actions-1.2.20230510/iam_actions/policies.json
+-rw-r--r--   0        0        0   193758 2023-05-10 02:27:05.651587 iam_actions-1.2.20230510/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   530028 2023-05-10 02:27:05.651587 iam_actions-1.2.20230510/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-10 02:27:06.695580 iam_actions-1.2.20230510/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230510/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230510/PKG-INFO
```

### Comparing `iam_actions-1.2.20230509/LICENSE` & `iam_actions-1.2.20230510/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230509/README.md` & `iam_actions-1.2.20230510/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230509/iam_actions/actions.json` & `iam_actions-1.2.20230510/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970883032164367%*

 * *Differences: {"'connect'": "{delete: ['UpdatedescribeContent']}",*

 * * "'inspector2'": "{'SearchVulnerabilities': {'access_level': 'Read', 'description': 'Grants "*

 * *                 'permission to list Amazon Inspector coverage details for a specific '*

 * *                 "vulnerability'}}",*

 * * "'simspaceweaver'": "{'CreateSnapshot': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                     "'CreateSnapshot'), ('condition_keys', []), ('description', 'Not Documented "*

 * *                     "by AWS'), ('orphan […]*

```diff
@@ -32006,27 +32006,14 @@
             ],
             "description": "Grants permission to update security profiles for a user in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "security-profile",
                 "user"
             ]
-        },
-        "UpdatedescribeContent": {
-            "access_level": "Write",
-            "action": "UpdatedescribeContent",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "connect:InstanceId"
-            ],
-            "description": "Grants permission to update contact flow module content in an Amazon Connect instance",
-            "orphan": false,
-            "resources": [
-                "contact-flow-module"
-            ]
         }
     },
     "connect-campaigns": {
         "CreateCampaign": {
             "access_level": "Write",
             "action": "CreateCampaign",
             "condition_keys": [
@@ -73606,18 +73593,18 @@
             "action": "ListUsageTotals",
             "condition_keys": [],
             "description": "Grants permission to retrieve aggregated usage data for an account",
             "orphan": false,
             "resources": []
         },
         "SearchVulnerabilities": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "SearchVulnerabilities",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list Amazon Inspector coverage details for a specific vulnerability",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
@@ -133039,14 +133026,22 @@
             "orphan": false,
             "resources": [
                 "signing-profile"
             ]
         }
     },
     "simspaceweaver": {
+        "CreateSnapshot": {
+            "access_level": "Undocumented",
+            "action": "CreateSnapshot",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteApp": {
             "access_level": "Write",
             "action": "DeleteApp",
             "condition_keys": [],
             "description": "Grants permission to delete an app",
             "orphan": false,
             "resources": [
@@ -140964,18 +140959,18 @@
             "description": "Grants permission to update a Slack channel configuration for your account",
             "orphan": false,
             "resources": []
         }
     },
     "supportplans": {
         "CreateSupportPlanSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSupportPlanSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create support plan schedules for this AWS account",
             "orphan": false,
             "resources": []
         },
         "GetSupportPlan": {
             "access_level": "Read",
             "action": "GetSupportPlan",
             "condition_keys": [],
@@ -144560,14 +144555,24 @@
             "description": "Grants permission to update the security profile snapshot release configuration",
             "orphan": false,
             "resources": [
                 "SecurityProfile"
             ]
         }
     },
+    "verified-access": {
+        "AllowVerifiedAccess": {
+            "access_level": "Undocumented",
+            "action": "AllowVerifiedAccess",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "voiceid": {
         "AssociateFraudster": {
             "access_level": "Write",
             "action": "AssociateFraudster",
             "condition_keys": [],
             "description": "Grants permission to associate a fraudster with a watchlist",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230509/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230510/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230509/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230510/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230509/iam_actions/generate/generate.py` & `iam_actions-1.2.20230510/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230509/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230510/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230509/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230510/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230509/iam_actions/generate/services.py` & `iam_actions-1.2.20230510/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230509/iam_actions/policies.json` & `iam_actions-1.2.20230510/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997333499556739%*

 * *Differences: {"'serviceMap'": "{'AWS SimSpace Weaver': {'Actions': {insert: [(0, 'CreateSnapshot')]}}, 'AWS "*

 * *                 "Verified Access': OrderedDict([('StringPrefix', 'verified-access'), ('Actions', "*

 * *                 "['AllowVerifiedAccess']), ('HasResource', False)])}"}*

```diff
@@ -8124,14 +8124,15 @@
                 "signer:ProfileVersion"
             ]
         },
         "AWS SimSpace Weaver": {
             "ARNFormat": "arn:aws:simspaceweaver:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:simspaceweaver:.+:.+:.+",
             "Actions": [
+                "CreateSnapshot",
                 "DeleteApp",
                 "DeleteSimulation",
                 "DescribeApp",
                 "DescribeSimulation",
                 "ListApps",
                 "ListSimulations",
                 "ListTagsForResource",
@@ -9012,14 +9013,21 @@
             "StringPrefix": "notifications-contacts",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "AWS Verified Access": {
+            "Actions": [
+                "AllowVerifiedAccess"
+            ],
+            "HasResource": false,
+            "StringPrefix": "verified-access"
+        },
         "AWS WAF": {
             "ARNFormat": "arn:aws:waf::${Account}:${ResourceId}/${Id}",
             "ARNRegex": "^arn:aws:waf::[0-9]+:.+/.+",
             "Actions": [
                 "CreateByteMatchSet",
                 "CreateGeoMatchSet",
                 "CreateIPSet",
```

### Comparing `iam_actions-1.2.20230509/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230510/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972144846796658%*

 * *Differences: {"'verified-access'": 'OrderedDict()'}*

```diff
@@ -6279,14 +6279,15 @@
             "condition_keys": "aws:RequestTag/${TagKey}"
         },
         "SecurityProfile": {
             "arn_pattern": "arn:*:vendor-insights:::security-profile:*",
             "condition_keys": "aws:RequestTag/${TagKey}"
         }
     },
+    "verified-access": {},
     "voiceid": {
         "domain": {
             "arn_pattern": "arn:*:voiceid:*:*:domain/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "vpc-lattice": {
```

### Comparing `iam_actions-1.2.20230509/iam_actions/services.json` & `iam_actions-1.2.20230510/iam_actions/services.json`

 * *Files identical despite different names*

#### Pretty-printed

 * *Similarity: 0.9972072307335191%*

 * *Differences: {"'simspaceweaver'": "{'Actions': {insert: [(0, 'CreateSnapshot')]}}",*

 * * "'verified-access'": "OrderedDict([('Actions', ['AllowVerifiedAccess']), ('ServiceNames', ['AWS "*

 * *                      "Verified Access']), ('ARNFormats', []), ('ARNRegexes', []), "*

 * *                      "('ConditionKeys', []), ('HasResource', False)])"}*

```diff
@@ -18484,14 +18484,15 @@
         "ARNFormats": [
             "arn:aws:simspaceweaver:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:simspaceweaver:.+:.+:.+"
         ],
         "Actions": [
+            "CreateSnapshot",
             "DeleteApp",
             "DeleteSimulation",
             "DescribeApp",
             "DescribeSimulation",
             "ListApps",
             "ListSimulations",
             "ListTagsForResource",
@@ -20338,14 +20339,26 @@
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Marketplace Vendor Insights"
         ]
     },
+    "verified-access": {
+        "ARNFormats": [],
+        "ARNRegexes": [],
+        "Actions": [
+            "AllowVerifiedAccess"
+        ],
+        "ConditionKeys": [],
+        "HasResource": false,
+        "ServiceNames": [
+            "AWS Verified Access"
+        ]
+    },
     "voiceid": {
         "ARNFormats": [
             "arn:aws:voiceid:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:voiceid:.+"
         ],
```

### Comparing `iam_actions-1.2.20230509/pyproject.toml` & `iam_actions-1.2.20230510/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230509"
+version = "1.2.20230510"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230509/setup.py` & `iam_actions-1.2.20230510/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230509',
+    'version': '1.2.20230510',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230509/PKG-INFO` & `iam_actions-1.2.20230510/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230509
+Version: 1.2.20230510
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

