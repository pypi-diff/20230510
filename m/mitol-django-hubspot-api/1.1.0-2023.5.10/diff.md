# Comparing `tmp/mitol-django-hubspot-api-1.1.0.tar.gz` & `tmp/mitol-django-hubspot-api-2023.5.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-hubspot-api-1.1.0.tar", last modified: Tue Jan 17 16:19:41 2023, max compression
+gzip compressed data, was "mitol-django-hubspot-api-2023.5.10.tar", last modified: Wed May 10 17:42:21 2023, max compression
```

## Comparing `mitol-django-hubspot-api-1.1.0.tar` & `mitol-django-hubspot-api-2023.5.10.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:19:41.573572 mitol-django-hubspot-api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1973 2023-01-17 16:19:41.573572 mitol-django-hubspot-api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:19:41.573572 mitol-django-hubspot-api-1.1.0/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:19:41.573572 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    18860 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:19:41.573572 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:19:41.573572 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      555 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/settings/hubspot_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:19:41.573572 mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1973 2023-01-17 16:19:41.000000 mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-01-17 16:19:41.000000 mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:19:41.000000 mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:19:41.000000 mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-01-17 16:19:41.000000 mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:19:41.000000 mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:19:41.000000 mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:19:41.573572 mitol-django-hubspot-api-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2947 2023-01-17 16:19:40.000000 mitol-django-hubspot-api-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.328985 mitol-django-hubspot-api-2023.5.10/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22389 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/settings/hubspot_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:42:21.324985 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 17:42:21.000000 mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 17:42:21.328985 mitol-django-hubspot-api-2023.5.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-05-10 17:42:20.000000 mitol-django-hubspot-api-2023.5.10/setup.py
```

### Comparing `mitol-django-hubspot-api-1.1.0/PKG-INFO` & `mitol-django-hubspot-api-2023.5.10/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-hubspot-api
-Version: 1.1.0
+Version: 2023.5.10
 Summary: Django application for Hubspot API integration
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-hubspot-api
 ---
 
 This is the Open Learning Hubspot API integration app. It provides helper functions for Hubspot CRM API calls:
```

### Comparing `mitol-django-hubspot-api-1.1.0/backend_shim.py` & `mitol-django-hubspot-api-2023.5.10/backend_shim.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/README.md` & `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/api.py` & `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 https://developers.hubspot.com/docs/api/overview
 """
 import json
 import logging
 import re
 from enum import Enum
 from typing import Dict, Iterable, List
+from urllib.parse import quote
 
+import requests
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from hubspot import HubSpot
 from hubspot.crm.objects import (
     ApiException,
     PublicObjectSearchRequest,
     SimplePublicObject,
@@ -93,14 +95,30 @@
 
     Returns:
         dict: The search filter
     """
     return {"propertyName": name, "operator": operator, "value": value}
 
 
+def delete_secondary_email(email: str, hubspot_id: str):
+    """
+    The CRM API Python library does not provide a function to delete secondary emails, so need to make a raw request
+
+    Args:
+        email(str): The email address to delete
+        hubspot_id: The id of the hubspot contact
+    """
+    headers = {"Authorization": f"Bearer {settings.MITOL_HUBSPOT_API_PRIVATE_TOKEN}"}
+    response = requests.delete(
+        f"https://api.hubapi.com/contacts/v1/secondary-email/{hubspot_id}/email/{quote(email)}?",
+        headers=headers,
+    )
+    response.raise_for_status()
+
+
 def get_all_objects(
     object_type: str, limit: int = 100, **kwargs
 ) -> Iterable[SimplePublicObject]:
     """
     Yield objects instead of returning all at once like client.crm.objects.get_all does
 
     Args:
@@ -147,14 +165,110 @@
 
     Returns:
         str: The hubspot_api id
     """
     return "{}-{}".format(settings.MITOL_HUBSPOT_API_ID_PREFIX, object_id)
 
 
+def handle_secondary_email_error(content_type: str, hubspot_id: str, email: str) -> str:
+    """
+    Check if the Hubspot contact has multiple emails, and if so, remove secondary email
+
+     Args:
+        content_type(ContentType): The object content type
+        hubspot_type(str): The hubspot_api type (deals, contacts, etc)
+        hubspot_id(int): The hubspot id of the contact
+        email(str): The email of the user to add to Hubspot
+
+    Returns:
+        str: The primary email of the existing hubspot contact, if it exists
+
+    """
+    contact = find_contact(email)
+    other_hso = HubspotObject.objects.filter(
+        content_type=content_type, hubspot_id=hubspot_id
+    ).first()
+    if contact and other_hso:
+        if contact.properties["email"] == email:
+            # Delete the HubspotObject it will be synced again next time
+            other_hso.delete()
+            # Delete the secondary email for the other user
+            delete_secondary_email(other_hso.content_object.email, contact.id)
+        else:
+            # Delete the secondary email for this user
+            delete_secondary_email(email, contact.id)
+        return contact.properties["email"]
+    return None
+
+
+def handle_create_api_error(
+    error: ApiException,
+    content_type: str,
+    hubspot_type: str,
+    object_id: int = None,
+    body: SimplePublicObjectInput = None,
+    ignore_conflict=False,
+) -> SimplePublicObject:
+    """
+    Handle cases where an object already exists but hubspot_id is not in db
+
+     Args:
+        error(ApiException): The Hubspot API exception
+        content_type(ContentType): The object content type
+        hubspot_type(str): The hubspot_api type (deals, contacts, etc)
+        object_id(int): The database id of the object
+        body (SimplePublicObjectInput): The properties of the object to set in Hubspot
+        ignore_conflict(bool): If true, a conflict error on create will be retried as an update
+
+    Returns:
+        SimplePublicObject: The Hubspot object returned from the API - if an update is doable and succeeds
+
+    """
+    if error.status in (400, 409):
+        details = json.loads(error.body)
+        message = details.get("message", "")
+        hubspot_id_matches = [
+            match
+            for match in list(sum(re.findall(HUBSPOT_EXISTING_ID, message), ()))
+            if match
+        ]
+        retry_update = False
+        retry_create = False
+        if hubspot_id_matches:
+            hubspot_id = hubspot_id_matches[0]
+            if hubspot_type == HubspotObjectType.CONTACTS.value:
+                user_email = body.properties["email"]
+                secondary_email = handle_secondary_email_error(
+                    content_type, hubspot_id, user_email
+                )
+                if secondary_email == user_email:
+                    # Retry contact update w/this email
+                    retry_update = True
+                elif secondary_email:
+                    # Retry contact creation w/this email
+                    retry_create = True
+            elif object_id and not ignore_conflict:
+                retry_update = True
+            elif ignore_conflict:
+                return SimplePublicObject(id=hubspot_id)
+            if retry_update:
+                return HubspotApi().crm.objects.basic_api.update(
+                    simple_public_object_input=body,
+                    object_id=hubspot_id,
+                    object_type=hubspot_type,
+                )
+            elif retry_create:
+                return HubspotApi().crm.objects.basic_api.create(
+                    simple_public_object_input=body,
+                    object_type=hubspot_type,
+                )
+    # This was some other kind of error so raise it
+    raise error
+
+
 def upsert_object_request(
     content_type: ContentType,
     hubspot_type: str,
     object_id: int = None,
     body: SimplePublicObjectInput = None,
     ignore_conflict=False,
 ) -> SimplePublicObject:
@@ -180,39 +294,24 @@
             object_type=hubspot_type,
         )
     else:
         try:
             result = api.create(
                 simple_public_object_input=body, object_type=hubspot_type
             )
-        except ApiException as err:  # pylint:disable=broad-except
-            # Handle cases where an object already exists but hubspot_id is not in db (redo as a PATCH)
-            if err.status in (400, 409):
-                details = json.loads(err.body)
-                message = details.get("message", "")
-                hubspot_id_matches = [
-                    match
-                    for match in list(sum(re.findall(HUBSPOT_EXISTING_ID, message), ()))
-                    if match
-                ]
-                if hubspot_id_matches:
-                    hubspot_id = hubspot_id_matches[0]
-                    if object_id and not ignore_conflict:
-                        HubspotObject.objects.update_or_create(
-                            object_id=object_id,
-                            content_type=content_type,
-                            hubspot_id=hubspot_id,
-                        )
-                        return upsert_object_request(
-                            content_type, hubspot_type, object_id=object_id, body=body
-                        )
-                    elif ignore_conflict:
-                        return SimplePublicObject(id=hubspot_id)
-            raise
-    if object_id and not hubspot_id:
+        except ApiException as err:
+            result = handle_create_api_error(
+                err,
+                content_type,
+                hubspot_type,
+                object_id=object_id,
+                body=body,
+                ignore_conflict=ignore_conflict,
+            )
+    if object_id and result and not hubspot_id:
         HubspotObject.objects.update_or_create(
             object_id=object_id, content_type=content_type, hubspot_id=result.id
         )
     return result
 
 
 def associate_objects_request(
@@ -428,15 +527,17 @@
 
     Args:
         email(str): The email of the user to find
 
     Returns:
         SimplePublicObject: The Hubspot contact returned by the API
     """
-    return HubspotApi().crm.contacts.basic_api.get_by_id(email, id_property="email")
+    return HubspotApi().crm.contacts.basic_api.get_by_id(
+        email, id_property="email", properties=["email", "hs_additional_emails"]
+    )
 
 
 def find_objects(
     object_type: str,
     query: str = None,
     filters: List[Dict] = None,
     properties: List[Dict] = None,
```

### Comparing `mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/decorators.py` & `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/decorators.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/factories.py` & `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/factories.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/migrations/0001_initial.py` & `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/models.py` & `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/models.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-1.1.0/mitol/hubspot_api/settings/hubspot_api.py` & `mitol-django-hubspot-api-2023.5.10/mitol/hubspot_api/settings/hubspot_api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/PKG-INFO` & `mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-hubspot-api
-Version: 1.1.0
+Version: 2023.5.10
 Summary: Django application for Hubspot API integration
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-hubspot-api
 ---
 
 This is the Open Learning Hubspot API integration app. It provides helper functions for Hubspot CRM API calls:
```

### Comparing `mitol-django-hubspot-api-1.1.0/mitol_django_hubspot_api.egg-info/SOURCES.txt` & `mitol-django-hubspot-api-2023.5.10/mitol_django_hubspot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-hubspot-api-1.1.0/setup.py` & `mitol-django-hubspot-api-2023.5.10/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     ],
     'description': 'Django application for Hubspot API integration',
     'install_requires': (
         'django<4.0,>=2.2.12',
         'djangorestframework>=3.0.0',
         'factory-boy~=3.2',
         'hubspot-api-client==6.1.0',
-        'mitol-django-common~=2.7.0',
-        'pytest==6.1.2',
+        'mitol-django-common',
+        'pytest',
+        'requests>=2.20.0',
         'setuptools',
         'urllib3>=1.26.5',
     ),
     'license': 'BSD 3-Clause License',
     'long_description': """mitol-django-hubspot-api
 ---
 
@@ -96,11 +97,11 @@
     },
     'packages': (
         'mitol',
         'mitol.hubspot_api',
         'mitol.hubspot_api.migrations',
         'mitol.hubspot_api.settings',
     ),
-    'python_requires': '>=3.7',
-    'version': '1.1.0',
+    'python_requires': '>=3.8',
+    'version': '2023.5.10',
     'zip_safe': True,
 })
```

