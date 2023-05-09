# Comparing `tmp/gandai-0.1.tar.gz` & `tmp/gandai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-0.1.tar", last modified: Fri Apr  7 12:54:30 2023, max compression
+gzip compressed data, was "gandai-0.1.1.tar", last modified: Tue May  9 22:04:07 2023, max compression
```

## Comparing `gandai-0.1.tar` & `gandai-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,44 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-04-07 12:54:30.253601 gandai-0.1/
--rw-r--r--   0 parker     (501) staff       (20)       25 2023-03-30 16:03:27.000000 gandai-0.1/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      213 2023-04-07 12:54:30.253474 gandai-0.1/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-04-07 12:54:30.250910 gandai-0.1/gandai/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-02 13:58:25.000000 gandai-0.1/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-04-07 12:54:30.251861 gandai-0.1/gandai/adapters/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-03 12:29:00.000000 gandai-0.1/gandai/adapters/__init__.py
--rw-r--r--   0 parker     (501) staff       (20)     1222 2023-04-06 10:55:20.000000 gandai-0.1/gandai/adapters/dealcloud.py
--rw-r--r--   0 parker     (501) staff       (20)     1824 2023-03-18 19:53:14.000000 gandai-0.1/gandai/adapters/filters.py
--rw-r--r--   0 parker     (501) staff       (20)     9798 2023-04-06 16:56:22.000000 gandai-0.1/gandai/adapters/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1578 2023-04-06 14:54:25.000000 gandai-0.1/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)      140 2023-03-30 16:03:27.000000 gandai-0.1/gandai/example.env
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-04-07 12:54:30.252075 gandai-0.1/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-05 18:51:06.000000 gandai-0.1/gandai/migrations/__init__.py
--rw-r--r--   0 parker     (501) staff       (20)     1764 2023-04-07 12:52:41.000000 gandai-0.1/gandai/migrations/dealcloud_to_gandai.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-04-07 12:54:30.253133 gandai-0.1/gandai/models/
--rw-r--r--   0 parker     (501) staff       (20)     1704 2023-03-30 16:03:27.000000 gandai-0.1/gandai/models/Auth.py
--rw-r--r--   0 parker     (501) staff       (20)       83 2023-03-02 13:58:25.000000 gandai-0.1/gandai/models/Bot.py
--rw-r--r--   0 parker     (501) staff       (20)      857 2023-04-06 15:01:55.000000 gandai-0.1/gandai/models/Comment.py
--rw-r--r--   0 parker     (501) staff       (20)      862 2023-03-17 12:15:55.000000 gandai-0.1/gandai/models/Company.py
--rw-r--r--   0 parker     (501) staff       (20)     2399 2023-04-06 15:42:10.000000 gandai-0.1/gandai/models/Event.py
--rw-r--r--   0 parker     (501) staff       (20)     4127 2023-04-06 14:41:06.000000 gandai-0.1/gandai/models/Search.py
--rw-r--r--   0 parker     (501) staff       (20)      406 2023-03-02 13:58:25.000000 gandai-0.1/gandai/models/Target.py
--rw-r--r--   0 parker     (501) staff       (20)      633 2023-03-03 12:29:00.000000 gandai-0.1/gandai/models/User.py
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-02 13:58:25.000000 gandai-0.1/gandai/models/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-04-07 12:54:30.253331 gandai-0.1/gandai/services/
--rw-r--r--   0 parker     (501) staff       (20)     4142 2023-04-06 15:49:39.000000 gandai-0.1/gandai/services/Query.py
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-02 13:58:25.000000 gandai-0.1/gandai/services/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-04-07 12:54:30.251347 gandai-0.1/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      213 2023-04-07 12:54:30.000000 gandai-0.1/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)      658 2023-04-07 12:54:30.000000 gandai-0.1/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-04-07 12:54:30.000000 gandai-0.1/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-04-07 12:54:30.000000 gandai-0.1/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      376 2023-04-07 12:52:02.000000 gandai-0.1/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-04-07 12:54:30.253636 gandai-0.1/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-0.1/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:04:07.225245 gandai-0.1.1/
+-rw-r--r--   0 parker     (501) staff       (20)       53 2023-05-09 22:04:03.000000 gandai-0.1.1/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-09 22:04:07.225112 gandai-0.1.1/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:04:07.221833 gandai-0.1.1/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-02 13:58:25.000000 gandai-0.1.1/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:04:07.223695 gandai-0.1.1/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      179 2023-04-07 16:05:45.000000 gandai-0.1.1/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-0.1.1/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-0.1.1/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4152 2023-04-12 13:11:27.000000 gandai-0.1.1/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-0.1.1/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3736 2023-05-09 18:28:28.000000 gandai-0.1.1/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5999 2023-05-09 18:36:56.000000 gandai-0.1.1/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    16739 2023-05-09 21:51:04.000000 gandai-0.1.1/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-0.1.1/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7725 2023-05-09 18:21:29.000000 gandai-0.1.1/gandai/__pycache__/sources.cpython-311.pyc
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:04:07.224119 gandai-0.1.1/gandai/adapters/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-03 12:29:00.000000 gandai-0.1.1/gandai/adapters/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:04:07.224593 gandai-0.1.1/gandai/adapters/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      188 2023-04-07 16:05:45.000000 gandai-0.1.1/gandai/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1875 2023-04-10 12:31:26.000000 gandai-0.1.1/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      924 2023-04-07 16:06:33.000000 gandai-0.1.1/gandai/adapters/__pycache__/filters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    14686 2023-04-14 19:20:28.000000 gandai-0.1.1/gandai/adapters/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1223 2023-05-05 19:45:58.000000 gandai-0.1.1/gandai/adapters/dealcloud.py
+-rw-r--r--   0 parker     (501) staff       (20)     1824 2023-03-18 19:53:14.000000 gandai-0.1.1/gandai/adapters/filters.py
+-rw-r--r--   0 parker     (501) staff       (20)    10094 2023-05-04 03:54:50.000000 gandai-0.1.1/gandai/adapters/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1704 2023-03-30 16:03:27.000000 gandai-0.1.1/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1578 2023-04-12 13:11:26.000000 gandai-0.1.1/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     3089 2023-05-09 18:28:27.000000 gandai-0.1.1/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:04:07.224925 gandai-0.1.1/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-0.1.1/gandai/migrations/__init__.py
+-rw-r--r--   0 parker     (501) staff       (20)     2536 2023-05-09 21:46:03.000000 gandai-0.1.1/gandai/migrations/create_db.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1764 2023-04-12 12:53:47.000000 gandai-0.1.1/gandai/migrations/dealcloud_to_gandai.py
+-rw-r--r--   0 parker     (501) staff       (20)     2560 2023-05-09 18:36:54.000000 gandai-0.1.1/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    17560 2023-05-09 21:51:02.000000 gandai-0.1.1/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     5348 2023-05-09 18:21:27.000000 gandai-0.1.1/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:04:07.222247 gandai-0.1.1/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-09 22:04:07.000000 gandai-0.1.1/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1120 2023-05-09 22:04:07.000000 gandai-0.1.1/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-09 22:04:07.000000 gandai-0.1.1/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-09 22:04:07.000000 gandai-0.1.1/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-09 21:49:41.000000 gandai-0.1.1/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-09 22:04:07.225275 gandai-0.1.1/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-0.1.1/setup.py
```

### Comparing `gandai-0.1/gandai/adapters/dealcloud.py` & `gandai-0.1.1/gandai/adapters/dealcloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def seed_search(engagement: pd.Series, force=False) -> None:
     data = json.loads(engagement.dropna().to_json())  # ugly
 
     DEFAULT_KEYWORDS = []
 
     DEFAULT_FILTER =  {
-        "employee_range": [25,2500],
+        "employees_range": [25,2500],
         "country": ["USA", "CAN", "MEX"],
         "state": [],
     }
 
     DEFAULT_SORT = {
         "sort_field": "employee_count", 
         "sort_order": "desc"
```

### Comparing `gandai-0.1/gandai/adapters/filters.py` & `gandai-0.1.1/gandai/adapters/filters.py`

 * *Files identical despite different names*

### Comparing `gandai-0.1/gandai/adapters/grata.py` & `gandai-0.1.1/gandai/adapters/grata.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import requests
 from pathlib import Path
 from dotenv import load_dotenv
 
 from gandai.datastore import Cloudstore
 from gandai.adapters import filters
 
-load_dotenv(f'{Path(__file__).parent.parent}/.env')
+# load_dotenv(f'{Path(__file__).parent.parent.parent}/.env') # well this doesn't feel good
 
 ds = Cloudstore()
 
 class GrataWrapper:
     def __init__(self) -> None:
         self.token = self._authenticate()
         self.headers = {"authorization": self.token}
@@ -80,15 +80,15 @@
             headers=self.headers,
             params=params,
         )
         data = response.json()
         for company in data["companies"]:
             if domain in company['domains']:
                 return company['id']
-        return company["id"]
+        
 
     def get_company_features_by_id(self, id: str) -> dict:
         """company from direct endpoint(s)"""
 
         def _get_company_by_id(id: str) -> dict:
             response = requests.get(
                 f"https://search.grata.com/api/company/{id}/", headers=self.headers
@@ -109,14 +109,16 @@
             return data
 
         def _get_hq_by_id(id: str) -> dict:
             def _get_hq(locations: list):
                 for location in locations:
                     if location["location_type"] == "HQ":
                         return location
+                    
+                return {} # todo handle no hq
 
             locations = _get_locations_by_id(id)
             return _get_hq(locations)
 
         def _get_employee_count(company) -> int:
             try:
                 return company["employees_estimate"]["grata"]["count"]
@@ -130,15 +132,17 @@
         def _get_state(company_hq) -> str:
             return company_hq.get("region_iso")
 
         def _get_country(company_hq) -> str:
             return company_hq.get("country_iso3")
 
         def _get_city_state(company_hq) -> str:
-            return f"{company_hq['city_name']}, {_get_state(company_hq)}"
+            return f"{company_hq.get('city_name')}, {_get_state(company_hq)}"
+            
+        
 
         company = _get_company_by_id(id)
         company_hq = _get_hq_by_id(id)
         # ^ async opportunity
 
         return {
             "id": company.get("id"),
@@ -218,18 +222,27 @@
             except:
                 return None
 
         def _get_country(headquarters: dict) -> str:
             return headquarters.get("country_iso")
 
         df["employee_count"] = df.apply(_get_employee_count, axis=1)
-        df["country"] = df["headquarters"].dropna().apply(_get_country)
-        df["state"] = df["headquarters"].dropna().apply(lambda x: x.get("region_iso"))
-        # df["web_hit_count"] = df["hits"].apply(lambda x: x["web"]["hit_count"]) # d
-        df["city_state"] = df["headquarters_pretty"]
+        
+        # null hq is a problem
+        if 'headquarters' in df.columns:
+            df["country"] = df["headquarters"].dropna().apply(_get_country)
+            df["state"] = df["headquarters"].dropna().apply(lambda x: x.get("region_iso"))
+        else:
+            df["country"] = None
+            df["state"] = None
+        if 'headquarters_pretty' in df.columns:
+            df["city_state"] = df["headquarters_pretty"]
+        else:
+            df["city_state"] = None
+
         df = df.dropna(subset=["employee_count", "domain"])
         df = df[
             [
                 "name",
                 "domain",
                 "description",
                 "employee_count",
```

### Comparing `gandai-0.1/gandai/datastore.py` & `gandai-0.1.1/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-0.1/gandai/migrations/dealcloud_to_gandai.py` & `gandai-0.1.1/gandai/migrations/dealcloud_to_gandai.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def run_dealcloud_engagement_to_gandai_search(limit=None):
     """
     Transfer DealCloud engagements to Gandai
     """
     df = Query.dealcloud_engagement_query(
-        "/Users/parker/Development/gandai-workspace/notebooks/2023-04-06/data/engagement.xlsx"
+        "/Users/parker/Development/gandai-workspace/notebooks/2023-04-10/data/engagement.xlsx"
     )
     df = df[df["modified_days_ago"] < 365].reset_index(drop=True)
     df = df[
         ~df["status"].isin(
             ["Lost Pre-Mandate", "Completed Engagement", "Dead Post-Mandate"]
         )
     ].reset_index(drop=True)
@@ -33,15 +33,15 @@
 
 
 def run_dealcloud_company_to_gandai_company():
     """
     Transfer DealCloud companies to Gandai
     """
     df = Query.dealcloud_company_query(
-        "/Users/parker/Development/gandai-workspace/notebooks/2023-04-06/data/company.xlsx"
+        "/Users/parker/Development/gandai-workspace/notebooks/2023-04-10/data/company.xlsx"
     )
     table_uri = f"gs://{ds.BUCKET_NAME}/sources/dealcloud/company_id_domain.feather"
     df.to_feather(table_uri)
 
 
 def main(engagement_limit=None):
     """
```

### Comparing `gandai-0.1/gandai/models/Auth.py` & `gandai-0.1.1/gandai/auth.py`

 * *Files identical despite different names*

