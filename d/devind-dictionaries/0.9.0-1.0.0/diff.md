# Comparing `tmp/devind_dictionaries-0.9.0.tar.gz` & `tmp/devind_dictionaries-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devind_dictionaries-0.9.0.tar", max compression
+gzip compressed data, was "devind_dictionaries-1.0.0.tar", max compression
```

## Comparing `devind_dictionaries-0.9.0.tar` & `devind_dictionaries-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
--rw-r--r--   0        0        0        0 2023-04-06 17:05:16.106498 devind_dictionaries-0.9.0/LICENSE
--rw-r--r--   0        0        0      139 2023-04-06 17:05:16.994505 devind_dictionaries-0.9.0/devind_dictionaries/__init__.py
--rw-r--r--   0        0        0      186 2023-04-06 17:05:16.106498 devind_dictionaries-0.9.0/devind_dictionaries/apps.py
--rw-r--r--   0        0        0     1123 2023-04-06 17:05:16.106498 devind_dictionaries-0.9.0/devind_dictionaries/management/commands/load_budget_classification.py
--rw-r--r--   0        0        0   462738 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/management/seed/001.devind_dictionaries/001.BudgetClassification.json
--rw-r--r--   0        0        0      102 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/managers/__init__.py
--rw-r--r--   0        0        0      475 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/managers/budget_classification_manager.py
--rw-r--r--   0        0        0     6546 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/migrations/0001_initial.py
--rw-r--r--   0        0        0      898 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/migrations/0002_auto_20220407_2148.py
--rw-r--r--   0        0        0     2764 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/migrations/0003_auto_20220420_2056.py
--rw-r--r--   0        0        0      914 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/migrations/0004_auto_20220421_2151.py
--rw-r--r--   0        0        0      575 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/migrations/0005_delete_parent_constraint.py
--rw-r--r--   0        0        0        0 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/migrations/__init__.py
--rw-r--r--   0        0        0      197 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/models/__init__.py
--rw-r--r--   0        0        0      910 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/models/budget_classification.py
--rw-r--r--   0        0        0     1270 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/models/department.py
--rw-r--r--   0        0        0     1302 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/models/districts.py
--rw-r--r--   0        0        0     2336 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/models/organizations.py
--rw-r--r--   0        0        0      326 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/permissions.py
--rw-r--r--   0        0        0     3040 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/schema/__init__.py
--rw-r--r--   0        0        0      764 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/schema/mutations.py
--rw-r--r--   0        0        0     5999 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/schema/types.py
--rw-r--r--   0        0        0     2834 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/services.py
--rw-r--r--   0        0        0     1530 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/settings.py
--rw-r--r--   0        0        0       90 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/tasks/__init__.py
--rw-r--r--   0        0        0      841 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/tasks/update_organizations.py
--rw-r--r--   0        0        0      217 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/tests/__init__.py
--rw-r--r--   0        0        0   185519 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/tests/data/organizations.xml
--rw-r--r--   0        0        0     4339 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/tests/test_budget_classification.py
--rw-r--r--   0        0        0     2145 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/tests/test_queries.py
--rw-r--r--   0        0        0     2405 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/tests/test_services.py
--rw-r--r--   0        0        0      378 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/devind_dictionaries/tests/test_settings.py
--rw-r--r--   0        0        0     1568 2023-04-06 17:05:16.994505 devind_dictionaries-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      819 2023-04-06 17:05:16.110499 devind_dictionaries-0.9.0/readme.md
--rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 devind_dictionaries-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-07 12:18:00.957581 devind_dictionaries-1.0.0/LICENSE
+-rw-r--r--   0        0        0      139 2022-07-07 12:18:02.549727 devind_dictionaries-1.0.0/devind_dictionaries/__init__.py
+-rw-r--r--   0        0        0      186 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/apps.py
+-rw-r--r--   0        0        0   251834 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/fixtures/budget_classification.json
+-rw-r--r--   0        0        0     6546 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/migrations/0001_initial.py
+-rw-r--r--   0        0        0      898 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/migrations/0002_auto_20220407_2148.py
+-rw-r--r--   0        0        0     2764 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/migrations/0003_auto_20220420_2056.py
+-rw-r--r--   0        0        0      914 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/migrations/0004_auto_20220421_2151.py
+-rw-r--r--   0        0        0      457 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/migrations/0005_alter_budgetclassification_updated_at.py
+-rw-r--r--   0        0        0        0 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/migrations/__init__.py
+-rw-r--r--   0        0        0      197 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/models/__init__.py
+-rw-r--r--   0        0        0      824 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/models/budget_classification.py
+-rw-r--r--   0        0        0     1270 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/models/department.py
+-rw-r--r--   0        0        0     1302 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/models/districts.py
+-rw-r--r--   0        0        0     2260 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/models/organizations.py
+-rw-r--r--   0        0        0     1937 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/schema/__init__.py
+-rw-r--r--   0        0        0      972 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/schema/filters.py
+-rw-r--r--   0        0        0     2736 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/schema/types.py
+-rw-r--r--   0        0        0      204 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/services/__init__.py
+-rw-r--r--   0        0        0      670 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/services/budget_classification_services.py
+-rw-r--r--   0        0        0     2836 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/services/organization_services.py
+-rw-r--r--   0        0        0     1530 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/settings.py
+-rw-r--r--   0        0        0       90 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/tasks/__init__.py
+-rw-r--r--   0        0        0      841 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/tasks/update_organizations.py
+-rw-r--r--   0        0        0      217 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/tests/__init__.py
+-rw-r--r--   0        0        0   185519 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/tests/data/organizations.xml
+-rw-r--r--   0        0        0     4518 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/tests/test_budget_classification.py
+-rw-r--r--   0        0        0     1980 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/tests/test_queries.py
+-rw-r--r--   0        0        0     2406 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/tests/test_services.py
+-rw-r--r--   0        0        0      378 2022-07-07 12:18:01.197603 devind_dictionaries-1.0.0/devind_dictionaries/tests/test_settings.py
+-rw-r--r--   0        0        0     1182 2022-07-07 12:18:02.549727 devind_dictionaries-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1195 2022-07-07 12:18:12.848775 devind_dictionaries-1.0.0/setup.py
+-rw-r--r--   0        0        0      836 2022-07-07 12:18:12.849109 devind_dictionaries-1.0.0/PKG-INFO
```

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/migrations/0001_initial.py` & `devind_dictionaries-1.0.0/devind_dictionaries/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/migrations/0002_auto_20220407_2148.py` & `devind_dictionaries-1.0.0/devind_dictionaries/migrations/0002_auto_20220407_2148.py`

 * *Files identical despite different names*

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/migrations/0003_auto_20220420_2056.py` & `devind_dictionaries-1.0.0/devind_dictionaries/migrations/0003_auto_20220420_2056.py`

 * *Files identical despite different names*

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/migrations/0004_auto_20220421_2151.py` & `devind_dictionaries-1.0.0/devind_dictionaries/migrations/0004_auto_20220421_2151.py`

 * *Files identical despite different names*

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/models/budget_classification.py` & `devind_dictionaries-1.0.0/devind_dictionaries/models/budget_classification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """Contains information's about budget classification codes."""
 
 from django.db import models
 
-from ..managers import BudgetClassificationManager
-
 
 class BudgetClassification(models.Model):
     """Budget classification codes."""
 
     code = models.CharField(max_length=40, unique=True, help_text='Code')
     name = models.CharField(max_length=1024, help_text='Name')
 
     active = models.BooleanField(default=True, help_text='Active')
     start = models.DateTimeField(auto_now_add=True, help_text='Date of start activity')
     end = models.DateTimeField(null=True, help_text='Date of end activity')
 
     created_at = models.DateTimeField(auto_now_add=True, help_text='Created date')
-    updated_at = models.DateTimeField(auto_now=True, help_text='Updated date')
-
-    objects = BudgetClassificationManager()
+    updated_at = models.DateTimeField(auto_now=True, null=True, help_text='Updated date')
 
     class Meta:
         """Metaclass of budget classification codes."""
 
         ordering = ('code',)
```

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/models/department.py` & `devind_dictionaries-1.0.0/devind_dictionaries/models/department.py`

 * *Files identical despite different names*

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/models/districts.py` & `devind_dictionaries-1.0.0/devind_dictionaries/models/districts.py`

 * *Files identical despite different names*

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/models/organizations.py` & `devind_dictionaries-1.0.0/devind_dictionaries/models/organizations.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,22 +26,15 @@
     address = models.TextField(null=True, help_text='Address')
 
     attributes = models.JSONField(help_text='Additional fields')
 
     created_at = models.DateTimeField(auto_now_add=True, help_text='Created date')
     updated_at = models.DateTimeField(auto_now=True, help_text='Updated date')
 
-    parent = models.ForeignKey(
-        'self',
-        null=True,
-        default=None,
-        on_delete=models.SET_NULL,
-        db_constraint=False,
-        help_text='Parent',
-    )
+    parent = models.ForeignKey('self', null=True, default=None, on_delete=models.SET_NULL, help_text='Parent')
     region = models.ForeignKey(Region, null=True, default=None, on_delete=models.SET_NULL, help_text='Region')
 
     user = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         null=True,
         on_delete=models.SET_NULL,
         related_name='organization',
```

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/services.py` & `devind_dictionaries-1.0.0/devind_dictionaries/services/organization_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from typing import Dict, Tuple, Type, Union
 
 import requests
 from devind_helpers.utils import convert_str_to_int
 from django.db import transaction
 from django.db.models import QuerySet
 
-from .models import District, Organization, Region
-from .settings import dictionaries_settings as settings
+from ..models import District, Organization, Region
+from ..settings import dictionaries_settings as settings
 
 
 def parse_organizations(content: str) -> Tuple[Dict, Dict, Dict]:
     """Parse xml file to three structures: District, Regions, Organizations."""
     districts: Dict[int, Dict] = {}
     regions: Dict[int, Dict] = {}
     organizations: Dict[int, Dict] = defaultdict(dict)
```

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/settings.py` & `devind_dictionaries-1.0.0/devind_dictionaries/settings.py`

 * *Files identical despite different names*

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/tasks/update_organizations.py` & `devind_dictionaries-1.0.0/devind_dictionaries/tasks/update_organizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
         content: str = get_content(dictionaries_settings.ORGANIZATIONS_LINK)
     except Exception as ex:
         return str(ex)
     districts, regions, organizations = parse_organizations(content)
     update_entity(District, districts)
     update_entity(Region, regions)
     update_entity(Organization, organizations)
-    return f'Districts: {len(districts)}, Regions: {len(regions)}, Organizations: {len(organizations)}'
+    return f'Districts: {len(districts)}, Regions: {len(regions)}, Organizatinos: {len(organizations)}'
```

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/tests/data/organizations.xml` & `devind_dictionaries-1.0.0/devind_dictionaries/tests/data/organizations.xml`

 * *Files identical despite different names*

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/tests/test_budget_classification.py` & `devind_dictionaries-1.0.0/devind_dictionaries/tests/test_budget_classification.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from datetime import datetime, timedelta
 
 from devind_dictionaries.models import BudgetClassification
 from django.core.management import call_command
 from django.test import TestCase
 from django.utils.timezone import make_aware
-from example.schema import schema
-from graphene.test import Client
+from strawberry_django_plus.test.client import Response, TestClient
 
 
 COUNT_BUDGET_CLASSIFICATION_CODE = 378
 COUNT_CHANGE_CODES = 10
 
 ACTIVE_BUDGET_CLASSIFICATIONS = """
     query {
@@ -36,74 +35,78 @@
 
 
 class TestBudgetClassification(TestCase):
     """Testing budget classification."""
 
     def setUp(self) -> None:
         """Setuping test settings."""
-        call_command('load_budget_classification')
-        self.client = Client(schema)
+        call_command('loaddata', 'budget_classification')
+        self.client = TestClient('/graphql/')
 
     def test_invoke_command(self) -> None:
         """Testing invoke command python manage.py load_budget_classification."""
         self.assertEqual(BudgetClassification.objects.count(), COUNT_BUDGET_CLASSIFICATION_CODE)
 
     def test_budget_classifications(self) -> None:
         """Test budget classification relay query."""
         query = """
-        query {
-          budgetClassifications {
-            totalCount
-            pageInfo {
-              hasNextPage
-              hasPreviousPage
-              startCursor
-              endCursor
-              __typename
-            }
-            edges {
-              node {
-                id
+          query {
+            budgetClassifications {
+              totalCount
+              pageInfo {
+                hasNextPage
+                hasPreviousPage
+                startCursor
+                endCursor
                 __typename
               }
+              edges {
+                node {
+                  id
+                  __typename
+                }
+              }
             }
           }
-        }
         """
-        find_budget_classification = self.client.execute(query)
-        self.assertIsNone(find_budget_classification.get('errors'))
-        budget_classification = find_budget_classification['data']['budgetClassifications']
+        response: Response = self.client.query(query)
+        self.assertIsNone(response.errors)
+        budget_classification: dict[str, str | dict] | None = response.data.get('budgetClassifications')
+        self.assertIsNotNone(budget_classification)
         self.assertEqual(budget_classification['totalCount'], COUNT_BUDGET_CLASSIFICATION_CODE)
 
     def test_active_budget_classifications(self) -> None:
         """Testing active budget classifications."""
-        find_budget_classification = self.client.execute(ACTIVE_BUDGET_CLASSIFICATIONS)
-        self.assertIsNone(find_budget_classification.get('errors'))
-        budget_classification = find_budget_classification['data']['activeBudgetClassifications']
-        self.assertEqual(budget_classification['totalCount'], COUNT_BUDGET_CLASSIFICATION_CODE)
+        response: Response = self.client.query(ACTIVE_BUDGET_CLASSIFICATIONS)
+        self.assertIsNone(response.errors)
+        budget_classifications: dict[str, str | dict] | None = response.data.get('activeBudgetClassifications')
+        self.assertIsNotNone(budget_classifications)
+        self.assertEqual(budget_classifications['totalCount'], COUNT_BUDGET_CLASSIFICATION_CODE)
 
     def test_active_budget_classification(self) -> None:
         """Testing active flag in budget classification."""
         budget_classifications_ids: list[int] = BudgetClassification.objects \
             .values_list('id', flat=True)[:COUNT_CHANGE_CODES]
         self.assertEqual(len(budget_classifications_ids), COUNT_CHANGE_CODES)
         BudgetClassification.objects.filter(pk__in=budget_classifications_ids).update(active=False)
-        find_budget_classification = self.client.execute(ACTIVE_BUDGET_CLASSIFICATIONS)
-        self.assertIsNone(find_budget_classification.get('errors'))
-        budget_classification = find_budget_classification['data']['activeBudgetClassifications']
-        self.assertEqual(budget_classification['totalCount'], COUNT_BUDGET_CLASSIFICATION_CODE - COUNT_CHANGE_CODES)
+        response: Response = self.client.query(ACTIVE_BUDGET_CLASSIFICATIONS)
+        self.assertIsNone(response.errors)
+        budget_classifications: dict[str, str | dict] | None = response.data.get('activeBudgetClassifications')
+        self.assertIsNotNone(budget_classifications)
+        self.assertEqual(budget_classifications['totalCount'], COUNT_BUDGET_CLASSIFICATION_CODE - COUNT_CHANGE_CODES)
 
     def test_end_budget_classification_back(self) -> None:
         """Testing end date in budget classification."""
         end = datetime.now() - timedelta(days=2)
         budget_classifications_ids: list[int] = BudgetClassification.objects \
             .values_list('id', flat=True)[:COUNT_CHANGE_CODES]
         self.assertEqual(len(budget_classifications_ids), COUNT_CHANGE_CODES)
         BudgetClassification.objects.filter(pk__in=budget_classifications_ids).update(end=make_aware(end))
-        find_budget_classification = self.client.execute(ACTIVE_BUDGET_CLASSIFICATIONS)
-        self.assertIsNone(find_budget_classification.get('errors'))
-        budget_classification = find_budget_classification['data']['activeBudgetClassifications']
+        response: Response = self.client.query(ACTIVE_BUDGET_CLASSIFICATIONS)
+        self.assertIsNone(response.errors)
+        budget_classification: dict[str, str | dict] | None = response.data.get('activeBudgetClassifications')
+        self.assertIsNotNone(budget_classification)
         self.assertEqual(budget_classification['totalCount'], COUNT_BUDGET_CLASSIFICATION_CODE - COUNT_CHANGE_CODES)
 
     def tearDown(self) -> None:
         """Delete all budget classification code."""
         BudgetClassification.objects.all().delete()
```

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/tests/test_queries.py` & `devind_dictionaries-1.0.0/devind_dictionaries/tests/test_queries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """Test queries."""
 
-from typing import Any
-
 from django.test import TestCase
-from example.schema import schema
-from graphene.test import Client
+from strawberry_django_plus.test.client import Response, TestClient
 
 from .test_services import get_test_organizations
 from ..models import District, Organization, Region
 from ..services import parse_organizations, update_entity
 
 
 class TestQueries(TestCase):
@@ -18,52 +15,49 @@
         """Set up data for testing."""
         content = get_test_organizations()
         districts, regions, organizations = parse_organizations(content)
         update_entity(District, districts)
         update_entity(Region, regions)
         update_entity(Organization, organizations)
 
-        self.client: Client = Client(schema)
+        self.client = TestClient('/graphql/')
 
     def test_district(self) -> None:
         """Testing district query."""
-        def query(district_id: int) -> Any:
-            """Helpers for execute query."""
-            return self.client.execute(
-                """
-                query ($districtId: Int!) {
-                  district (districtId: $districtId) {
-                    id
-                    name
-                    __typename
-                  }
-                }
-                """,
-                variables={'districtId': district_id}
-            )
-        find_district = query(1)
-        self.assertIsNone(find_district.get('errors'))
-        district = find_district['data']['district']
+        query: str = """
+          query ($pk: ID!) {
+            district (pk: $pk) {
+              id
+              name
+              __typename
+            }
+          }
+        """
+        response: Response = self.client.query(query, {'pk': 1})
+        self.assertIsNone(response.errors)
+        district: dict[str, str] | None = response.data.get('district')
+        self.assertIsNotNone(district)
         self.assertEqual(district['__typename'], 'DistrictType')
 
     def test_districts(self) -> None:
         """Testing districts query."""
-        districts_result = self.client.execute(
+        response: Response = self.client.query(
             """
             query {
               districts {
                 id
                 name
                 __typename
               }
             }
             """
         )
-        self.assertIsNone(districts_result.get('errors'))
-        districts = districts_result['data']['districts']
+        self.assertIsNone(response.errors)
+        districts: list[dict[str, str]] | None = response.data.get('districts')
+        self.assertIsNotNone(districts)
         self.assertEqual(len(districts), District.objects.count())
 
     def tearDown(self) -> None:
         """Free seeder data."""
         Organization.objects.all().delete()
         Region.objects.all().delete()
         District.objects.all().delete()
```

### Comparing `devind_dictionaries-0.9.0/devind_dictionaries/tests/test_services.py` & `devind_dictionaries-1.0.0/devind_dictionaries/tests/test_services.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ..settings import dictionaries_settings
 
 
 @lru_cache
 def get_test_organizations() -> str:
     """Get testing organizations."""
     data_file: str = join(settings.BASE_DIR, 'devind_dictionaries', 'tests', 'data', 'organizations.xml')
-    with open(data_file, encoding='utf8') as file:
+    with open(data_file, encoding='utf-8') as file:
         content: str = file.read()
     return content
 
 
 @dataclass
 class MockRequestResponse:
     """Mock response instead of request.get."""
```

### Comparing `devind_dictionaries-0.9.0/pyproject.toml` & `devind_dictionaries-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 [tool.poetry]
 name = "devind_dictionaries"
-version = "0.9.0"
-description = "Common dictionaries for devind applications."
-authors = ["Luferov Victor <lyferov@yandex.ru>"]
+version = "1.0.0"
+description = "Common dictionaries for devind applications"
+authors = ["Victor <lyferov@yandex.ru>"]
 license = "MIT"
-readme = "readme.md"
-homepage = "https://github.com/devind-team/devind-django-dictionaries"
-repository = "https://github.com/devind-team/devind-django-dictionaries"
-keywords = ["django", "graphene", "dictionaries"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Framework :: Django"
-]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-Django = ">=3.2.12,<5.0.0"
-graphene-django = "^2.15.0"
-requests = "^2.27.1"
-beautifulsoup4 = "^4.10.0"
-celery = "^5.2.5"
-devind-helpers = "^0"
-graphene-django-filter = "^0.6.4"
+Django = "^4.0.5"
+requests = "^2.28.0"
+beautifulsoup4 = "^4.11.1"
+celery = "^5.2.7"
+devind-helpers = "^1.0.0"
+python-dotenv = "^0.20.0"
+strawberry-graphql-django = "^0.3.1"
+strawberry-graphql = "^0.116.4"
+strawberry-django-plus = "^1.17.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 flake8-import-order = "^0.18.1"
 flake8-docstrings = "^1.6.0"
 flake8-builtins = "^1.5.3"
 flake8-quotes = "^3.3.1"
 flake8-comprehensions = "^3.8.0"
 flake8-eradicate = "^1.2.0"
 flake8-simplify = "^0.19.2"
 flake8-spellcheck = "^0.28.0"
 pep8-naming = "^0.13.0"
 flake8-use-fstring = "^1.3"
 flake8-annotations = "^2.7.0"
-django-seed = "^0.3.1"
 coveralls = "^3.3.1"
-python-dotenv = "^0.20.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = [
     "devind_dictionaries/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
-build_command = "pip install poetry && poetry build"
+build_command = "pip install poetry && poetry build"
```

