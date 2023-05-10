# Comparing `tmp/iam_ape-1.1.0.tar.gz` & `tmp/iam_ape-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_ape-1.1.0.tar", max compression
+gzip compressed data, was "iam_ape-1.1.1.tar", max compression
```

## Comparing `iam_ape-1.1.0.tar` & `iam_ape-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-03-21 14:09:32.879473 iam_ape-1.1.0/LICENSE
--rw-r--r--   0        0        0     3031 2023-04-27 15:10:48.767861 iam_ape-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-21 14:09:32.880346 iam_ape-1.1.0/iam_ape/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 14:09:32.880510 iam_ape-1.1.0/iam_ape/aws_iam_actions/__init__.py
--rw-r--r--   0        0        0   259037 2023-04-27 15:10:48.769019 iam_ape-1.1.0/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
--rw-r--r--   0        0        0     2773 2023-03-23 15:18:42.493898 iam_ape-1.1.0/iam_ape/aws_iam_actions/scrape_iam_actions.py
--rw-r--r--   0        0        0     1655 2023-03-21 14:09:32.881248 iam_ape-1.1.0/iam_ape/consts.py
--rw-r--r--   0        0        0    31885 2023-04-27 15:10:48.769584 iam_ape-1.1.0/iam_ape/evaluator.py
--rw-r--r--   0        0        0    14524 2023-04-27 15:10:48.769991 iam_ape-1.1.0/iam_ape/expand_policy.py
--rw-r--r--   0        0        0     3724 2023-04-27 15:10:48.770267 iam_ape-1.1.0/iam_ape/helper_classes.py
--rw-r--r--   0        0        0     7900 2023-04-27 15:10:48.770543 iam_ape-1.1.0/iam_ape/helper_functions.py
--rw-r--r--   0        0        0     1224 2023-04-27 15:10:48.770874 iam_ape-1.1.0/iam_ape/helper_types.py
--rw-r--r--   0        0        0     9584 2023-04-27 15:10:48.771237 iam_ape-1.1.0/iam_ape/main.py
--rw-r--r--   0        0        0        0 2023-03-23 15:18:42.495823 iam_ape-1.1.0/iam_ape/py.typed
--rw-r--r--   0        0        0     1257 2023-04-27 15:10:48.772004 iam_ape-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 iam_ape-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 15:26:26.770889 iam_ape-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3031 2023-04-27 15:26:26.771008 iam_ape-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771631 iam_ape-1.1.1/iam_ape/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771725 iam_ape-1.1.1/iam_ape/aws_iam_actions/__init__.py
+-rw-r--r--   0        0        0   260932 2023-05-10 17:36:52.355616 iam_ape-1.1.1/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
+-rw-r--r--   0        0        0     2773 2023-04-27 15:26:26.772225 iam_ape-1.1.1/iam_ape/aws_iam_actions/scrape_iam_actions.py
+-rw-r--r--   0        0        0     1748 2023-05-10 17:34:00.350992 iam_ape-1.1.1/iam_ape/consts.py
+-rw-r--r--   0        0        0    31885 2023-04-27 15:26:26.772497 iam_ape-1.1.1/iam_ape/evaluator.py
+-rw-r--r--   0        0        0    15478 2023-05-10 17:34:00.351179 iam_ape-1.1.1/iam_ape/expand_policy.py
+-rw-r--r--   0        0        0     3422 2023-05-10 17:34:00.351308 iam_ape-1.1.1/iam_ape/helper_classes.py
+-rw-r--r--   0        0        0     7858 2023-05-10 17:34:00.351446 iam_ape-1.1.1/iam_ape/helper_functions.py
+-rw-r--r--   0        0        0     1224 2023-04-27 15:26:26.773011 iam_ape-1.1.1/iam_ape/helper_types.py
+-rw-r--r--   0        0        0     9999 2023-05-10 17:34:00.351593 iam_ape-1.1.1/iam_ape/main.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.773181 iam_ape-1.1.1/iam_ape/py.typed
+-rw-r--r--   0        0        0     1257 2023-05-10 17:37:12.129154 iam_ape-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 iam_ape-1.1.1/PKG-INFO
```

### Comparing `iam_ape-1.1.0/LICENSE` & `iam_ape-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.0/README.md` & `iam_ape-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.0/iam_ape/aws_iam_actions/scrape_iam_actions.py` & `iam_ape-1.1.1/iam_ape/aws_iam_actions/scrape_iam_actions.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.0/iam_ape/consts.py` & `iam_ape-1.1.1/iam_ape/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
+import re
 from dataclasses import dataclass
 from typing import Literal
 
+RESOURCE_ARN_RE = re.compile("arn:(aws|aws-gov|aws-china):(?P<service>[^:]+):.*")
+
 
 @dataclass(frozen=True)
 class PolicyElement:
     WILDCARD: Literal["*"] = "*"
     EFFECT: Literal["Effect"] = "Effect"
     ALLOW: Literal["Allow"] = "Allow"
     DENY: Literal["Deny"] = "Deny"
```

### Comparing `iam_ape-1.1.0/iam_ape/evaluator.py` & `iam_ape-1.1.1/iam_ape/evaluator.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.0/iam_ape/expand_policy.py` & `iam_ape-1.1.1/iam_ape/expand_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tarfile
 from collections import defaultdict
 from fnmatch import fnmatch
 from typing import Any, Dict, FrozenSet, List, Literal, Optional, Set, Tuple
 
 from requests.structures import CaseInsensitiveDict
 
-from iam_ape.consts import PolicyElement, actions_json_location
+from iam_ape.consts import RESOURCE_ARN_RE, PolicyElement, actions_json_location
 from iam_ape.helper_classes import (
     Action,
     HashableDict,
     HashableList,
     PermissionsContainer,
     PolicyWithSource,
 )
@@ -20,20 +20,37 @@
 
 logger = logging.getLogger("policy expander")
 
 
 def _append_action(
     res: Dict[str, Set[Action]],
     action: str,
+    service: str,
     resources: Optional[List[str]],
     not_resources: Optional[List[str]],
     condition: Optional[Dict[str, Any]],
     source: str,
 ) -> None:
+    def relevant_resource(resource: str, service: str) -> bool:
+        if resource.lower() in (
+            "*",
+            "arn:*",
+            "arn:aws:*",
+            "arn:aws-gov:*",
+            "arn:aws-china:*",
+        ):
+            return True
+        if match := RESOURCE_ARN_RE.match(resource):
+            res_service = match.group("service")
+            return res_service.lower() == service.lower()
+        return False
+
     for resource in resources or []:
+        if not relevant_resource(resource, service):
+            continue
         if condition:
             for key, val in condition.items():
                 res[action].add(
                     Action(
                         action=action,
                         resource=resource,
                         not_resource=None,
@@ -48,14 +65,16 @@
                     resource=resource,
                     not_resource=None,
                     condition=None,
                     source=source,
                 )
             )
     for not_resource in not_resources or []:
+        if not relevant_resource(not_resource, service):
+            continue
         if condition:
             for key, val in condition.items():
                 res[action].add(
                     Action(
                         action=action,
                         resource=None,
                         not_resource=not_resource,
@@ -139,50 +158,53 @@
         return PermissionsContainer(
             allowed_permissions=all_actions[PolicyElement.ALLOW],
             denied_permissions=all_actions[PolicyElement.DENY],
         )
 
     def expand_action(self, iam_action: Action) -> Dict[str, Set[Action]]:
         res: Dict[str, Set[Action]] = defaultdict(set)
-
-        if iam_action.action == PolicyElement.WILDCARD:  # {"Action": ["*"]}
-            for service, action_dicts in self.all_iam_actions.items():
-                for action in action_dicts.keys():
-                    _append_action(
-                        res=res,
-                        action=f"{service}:{action}",
-                        resources=as_list(iam_action.resource),
-                        not_resources=as_list(iam_action.not_resource),
-                        condition=iam_action.condition,
-                        source=iam_action.source,
-                    )
-        elif PolicyElement.WILDCARD in iam_action.action:  # {"Action": ["iam:*"]}
-            service, wildcard_action = iam_action.action.split(":", maxsplit=1)
-            for action in self.all_iam_actions[service].keys():
-                if fnmatch(action.lower(), wildcard_action.lower()):
-                    _append_action(
-                        res=res,
-                        action=f"{service}:{action}",
-                        resources=as_list(iam_action.resource),
-                        not_resources=as_list(iam_action.not_resource),
-                        condition=iam_action.condition,
-                        source=iam_action.source,
-                    )
-        else:  # {"Action": ["sts:GetCallerIdentity"]}
-            try:
+        try:
+            if iam_action.action == PolicyElement.WILDCARD:  # {"Action": ["*"]}
+                for service, action_dicts in self.all_iam_actions.items():
+                    for action in action_dicts.keys():
+                        _append_action(
+                            res=res,
+                            service=service,
+                            action=f"{service}:{action}",
+                            resources=as_list(iam_action.resource),
+                            not_resources=as_list(iam_action.not_resource),
+                            condition=iam_action.condition,
+                            source=iam_action.source,
+                        )
+            elif PolicyElement.WILDCARD in iam_action.action:  # {"Action": ["iam:*"]}
+                service, wildcard_action = iam_action.action.split(":", maxsplit=1)
+                for action in self.all_iam_actions[service].keys():
+                    if fnmatch(action.lower(), wildcard_action.lower()):
+                        _append_action(
+                            res=res,
+                            service=service,
+                            action=f"{service}:{action}",
+                            resources=as_list(iam_action.resource),
+                            not_resources=as_list(iam_action.not_resource),
+                            condition=iam_action.condition,
+                            source=iam_action.source,
+                        )
+            else:  # {"Action": ["sts:GetCallerIdentity"]}
+                service, action = iam_action.action.split(":", maxsplit=1)
                 _append_action(
                     res=res,
+                    service=service,
                     action=self.normalize_action(iam_action.action),
                     resources=as_list(iam_action.resource),
                     not_resources=as_list(iam_action.not_resource),
                     condition=iam_action.condition,
                     source=iam_action.source,
                 )
-            except KeyError:  # not a valid action
-                logger.debug(f"Got an invalid action: {iam_action.action}")
+        except KeyError:  # not a valid action
+            logger.debug(f"Got an invalid action: {iam_action.action}")
 
         return res
 
     def expand_not_action(
         self, statement: AwsPolicyStatementType, sid: str
     ) -> Dict[str, Set[Action]]:
         res: Dict[str, Set[Action]] = defaultdict(set)
@@ -203,14 +225,15 @@
                             for not_action in notactions
                         ]
                     ):
                         continue
                     _append_action(
                         res=res,
                         action=curr_action,
+                        service=iam_service,
                         resources=statement.get(PolicyElement.RESOURCE),
                         not_resources=statement.get(PolicyElement.NOTRESOURCE),
                         condition=statement.get(PolicyElement.CONDITION),
                         source=sid,
                     )
 
         return res
```

### Comparing `iam_ape-1.1.0/iam_ape/helper_classes.py` & `iam_ape-1.1.1/iam_ape/helper_classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,43 +8,35 @@
     AwsPolicyType,
     IneffectiveActionDict,
     PermissionsContainerDict,
 )
 
 
 class HashableList(List[Any]):
-    def flatten(self, list_obj: List[Any]) -> List[Any]:
-        all_items = []
-        for item in list_obj:
-            if hasattr(item, "__hash__"):
-                all_items.append(item)
-            elif isinstance(item, list):
-                all_items.extend(self.flatten(item))
-            else:
-                raise TypeError(f"Unhashable type: {type(item)}")
-        return all_items
-
     def __hash__(self) -> int:  # type: ignore[override]
-        return hash(tuple(sorted(self.flatten(self))))
+        return hash(tuple(self))
 
 
 class HashableDict(Dict[Any, Any]):
     def __hash__(self) -> int:  # type: ignore[override]
-        return hash(tuple(sorted(self.items())))
+        return hash(tuple(self.items()))
 
     @classmethod
     def recursively(cls, dict_obj: Optional[Dict[Any, Any]]):
         if dict_obj is None:
             return dict_obj
         for key, value in dict_obj.items():
             if isinstance(value, dict):
-                dict_obj[key] = HashableDict.recursively(value)
+                dict_obj[key] = cls.recursively(value)
             elif isinstance(value, list):
                 dict_obj[key] = HashableList(value)
-        return HashableDict(dict_obj)
+            else:
+                assert hasattr(value, "__hash__"), f"Unhashable type: {type(value)}"
+                dict_obj[key] = value
+        return cls(dict_obj)
 
 
 @dataclass(unsafe_hash=True)
 class Action:
     action: str
     resource: Optional[str]
     not_resource: Optional[str]
```

### Comparing `iam_ape-1.1.0/iam_ape/helper_functions.py` & `iam_ape-1.1.1/iam_ape/helper_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from copy import deepcopy
 from typing import Any, Dict, List, Literal, Optional, Set, TypeVar
 
 from iam_ape.consts import CONDITIONS_NEGATIONS
 from iam_ape.helper_classes import HashableDict, HashableList
 from iam_ape.helper_types import AwsPolicyType
 
 logger = logging.getLogger(__name__)
@@ -120,15 +119,15 @@
                         new_action_list.append(action)
                 statement[action_key] = new_action_list
 
     return policy
 
 
 def negate_condition(condition: Dict[str, Any]) -> Dict[str, Any]:
-    res_condition = deepcopy(condition)
+    res_condition = condition.copy()
     condition_prefix = None
     condition_key, condition_value = list(res_condition.items())[0]
 
     if negated := CONDITIONS_NEGATIONS.get(condition_key):
         return {negated: condition_value}
 
     if condition_key.count(":") == 1:
@@ -143,21 +142,24 @@
 
     if condition_key.lower().endswith("ifexists"):
         condition_key = condition_key[:-8]
         if negated := CONDITIONS_NEGATIONS.get(condition_key):
             return {f"{negated}IfExists": condition_value}
 
     if condition_key.lower() in ("bool", "null"):
-        for _condition, _values in condition_value.items():
-            if all(v.lower() == "false" for v in _values):
-                condition_value[_condition] = HashableList(["true"])
-            elif all(v.lower() == "true" for v in _values):
-                condition_value[_condition] = HashableList(["false"])
-            else:
-                condition_value[_condition] = HashableList(["true", "false"])
+        condition_value = {
+            _condition: (
+                HashableList(["true"])
+                if all(v.lower() == "false" for v in _values)
+                else HashableList(["false"])
+                if all(v.lower() == "true" for v in _values)
+                else HashableList(["true", "false"])
+            )
+            for _condition, _values in condition_value.items()
+        }
 
     if condition_key == "BinaryEquals":  # there is no bloody negation
         logger.info(f"BinaryEquals used in a deny condition: {condition}")
 
     if condition_prefix:
         return {f"{condition_prefix}:{condition_key}": condition_value}
```

### Comparing `iam_ape-1.1.0/iam_ape/helper_types.py` & `iam_ape-1.1.1/iam_ape/helper_types.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.0/iam_ape/main.py` & `iam_ape-1.1.1/iam_ape/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,17 +94,28 @@
     return AuthorizationDetails(auth_report)
 
 
 def load_auth_details_from_aws(profile: Optional[str] = None) -> AuthorizationDetails:
     logger.info("Attempting to fetch authorization details report from AWS...")
     auth_report: Dict[str, Any] = {}
     profile = profile or os.environ.get("AWS_PROFILE")
-    if not profile:
-        raise ValueError("No AWS profile found")
-    boto3.setup_default_session(profile_name=profile)
+    if profile:
+        logger.info(f"AWS Auth: Using profile: {profile}")
+        boto3.setup_default_session(profile_name=profile)
+    elif (
+        not profile
+        and os.environ.get("AWS_ACCESS_KEY_ID")
+        and os.environ.get("AWS_SECRET_ACCESS_KEY")
+    ):
+        logger.info("AWS Auth: Using environment variables")
+    else:
+        raise ValueError(
+            "AWS Auth: No authentication method found. "
+            "Please set AWS_PROFILE (or use --profile) or AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY"
+        )
     iam_client = boto3.client("iam")
     paginator = iam_client.get_paginator("get_account_authorization_details")
     for page in paginator.paginate():
         auth_report = deep_update(auth_report, page)
     a = AuthorizationDetails(auth_report)
     return a
```

### Comparing `iam_ape-1.1.0/pyproject.toml` & `iam_ape-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-ape"
-version = "1.1.0"
+version = "1.1.1"
 description = "IAM AWS Permissions Evaluator"
 authors = ["Tohar Braun, Orca Security <tohar@orca.security>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 repository = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 keywords = ["aws", "iam"]
```

### Comparing `iam_ape-1.1.0/PKG-INFO` & `iam_ape-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-ape
-Version: 1.1.0
+Version: 1.1.1
 Summary: IAM AWS Permissions Evaluator
 Home-page: https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/
 License: GPL-3.0-or-later
 Keywords: aws,iam
 Author: Tohar Braun, Orca Security
 Author-email: tohar@orca.security
 Requires-Python: >=3.8,<4.0
```

