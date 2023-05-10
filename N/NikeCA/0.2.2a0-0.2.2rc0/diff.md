# Comparing `tmp/NikeCA-0.2.2a0.tar.gz` & `tmp/NikeCA-0.2.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.2.2a0.tar", last modified: Wed May 10 19:02:33 2023, max compression
+gzip compressed data, was "NikeCA-0.2.2rc0.tar", last modified: Wed May 10 19:56:07 2023, max compression
```

## Comparing `NikeCA-0.2.2a0.tar` & `NikeCA-0.2.2rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.371349 NikeCA-0.2.2a0/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.2a0/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-10 19:02:33.370838 NikeCA-0.2.2a0/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.2a0/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 19:02:33.371483 NikeCA-0.2.2a0/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-10 19:02:23.000000 NikeCA-0.2.2a0/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.363345 NikeCA-0.2.2a0/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.364772 NikeCA-0.2.2a0/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4020 2023-05-07 22:07:42.000000 NikeCA-0.2.2a0/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.365745 NikeCA-0.2.2a0/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.2.2a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.367304 NikeCA-0.2.2a0/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6140 2023-05-08 17:16:29.000000 NikeCA-0.2.2a0/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.370246 NikeCA-0.2.2a0/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.2.2a0/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19181 2023-05-10 18:07:25.000000 NikeCA-0.2.2a0/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.2.2a0/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.2.2a0/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.2.2a0/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.070460 NikeCA-0.2.2rc0/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.2rc0/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18014 2023-05-10 19:56:07.070051 NikeCA-0.2.2rc0/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.2rc0/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 19:56:07.070587 NikeCA-0.2.2rc0/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2487 2023-05-10 19:55:46.000000 NikeCA-0.2.2rc0/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.061057 NikeCA-0.2.2rc0/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.062524 NikeCA-0.2.2rc0/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.2rc0/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.064377 NikeCA-0.2.2rc0/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.2rc0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       27 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.066670 NikeCA-0.2.2rc0/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.2rc0/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.2rc0/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       39 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       44 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.069408 NikeCA-0.2.2rc0/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18014 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-05-10 19:50:52.000000 NikeCA-0.2.2rc0/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19225 2023-05-10 19:50:52.000000 NikeCA-0.2.2rc0/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14091 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       45 2023-05-10 19:46:50.000000 NikeCA-0.2.2rc0/src/__init__.py
```

### Comparing `NikeCA-0.2.2a0/LICENSE` & `NikeCA-0.2.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/PKG-INFO` & `NikeCA-0.2.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.2a0
+Version: 0.2.2rc0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.2a0/README.md` & `NikeCA-0.2.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/setup.py` & `NikeCA-0.2.2rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.2.2a',
+	version='0.2.2c',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"_BuildSearchQuery",
 		"_GitHub",
 		"_SearchFiles",
 		"_SnowflakeData",
 		"_SnowflakeDependencies",
 		"_SnowflakePull",
 		"_QA",
-		"Dashboards",
 		"Dashboards/__init__",
 		"Dashboards/Dashboards",
 		"Dashboards/InclusionExclusion/InclusionExclusion",
 		"Dashboards/InclusionExclusion/__init__",
 		"Dashboards/Telemetry/ProductUsage",
 		"Dashboards/Telemetry/Telemetry",
 		"Dashboards/Telemetry/__init__",
```

### Comparing `NikeCA-0.2.2a0/src/Dashboards/Dashboards.py` & `NikeCA-0.2.2rc0/src/Dashboards/Dashboards.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 
 
-from .Telemetry.Telemetry import Telemetry
-from .InclusionExclusion.InclusionExclusion import InclusionExclusion
+from NikeSF import Snowflake
 
 
-class Dashboards(Telemetry, InclusionExclusion):
+class Dashboards(Snowflake):
 
-    Telemetry = Telemetry()
-    Telemetry.ProductUsage = Telemetry.ProductUsage()
-    InclusionExclusion = InclusionExclusion()
+    def __init__(self, username, role, warehouse, database):
+        super().__init__(username, role, warehouse, database)
+
+        self.username = username
+        self.role = role
+        self.warehouse = warehouse
+        self.database = database
+
+    @property
+    def Telemetry(self):
+        from .Telemetry.Telemetry import Telemetry
+        return Telemetry(username=self.username, role=self.role, warehouse=self.warehouse, database=self.database)
 
     def imp_summary_dashboard(self
                               , username: str
                               , warehouse: str
                               , database: str
                               , role: str
                               , date_min: str = '1900-01-01'
```

### Comparing `NikeCA-0.2.2a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.2.2rc0/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 
 
-class InclusionExclusion:
+from Dashboards.Dashboards import Dashboards
+from NikeCA import Snowflake
+
+
+class InclusionExclusion(Dashboards, Snowflake):
+
+    def __init__(self, username, warehouse, role, database):
+        super().__init__(username=username, warehouse=warehouse, role=role, database=database)
+
+        self.username = username
+        self.warehouse = warehouse
+        self.role = role
+        self.database = database
 
     def pos_data_quality_review(self
-                                , username: str
-                                , warehouse: str
-                                , database: str
-                                , role: str
+                                , username: str | None = None
+                                , warehouse: str | None = None
+                                , database: str | None = None
+                                , role: str | None = None
                                 , columns: list | None = None
                                 , filters: list | None = None
                                 , order_by: list | None = None
                                 , polars: bool = False
                                 , start_date: str | None = None
                                 , end_date: str | None = None):
 
-        from NikeCA import Snowflake
+        if username is None:
+            username = self.username
+        if warehouse is None:
+            warehouse = self.warehouse
+        if database is None:
+            database = self.database
+        if role is None:
+            role = self.role
+
         import polars as pl
         import datetime
         import configparser
 
         config = configparser.ConfigParser()
         config.read('pip.ini')
 
@@ -70,36 +90,58 @@
             ;
         """
 
         df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
                                     role=role).snowflake_pull(query=query, polars=polars))
 
         if start_date is None and end_date is None:
-            return df.filter(pl.col(a) == pl.col(a).max())
+            if polars:
+                return df.filter(pl.col(a) == pl.col(a).max())
+            else:
+                return df.filter(pl.col(a) == pl.col(a).max()).to_pandas()
         elif end_date is None:
-            return df.filter((pl.col(a) >= datetime.datetime.strptime(start_date, '%Y-%m-%d')))
+            if polars:
+                return df.filter((pl.col(a) >= datetime.datetime.strptime(start_date, '%Y-%m-%d')))
+            else:
+                return df.filter((pl.col(a) >= datetime.datetime.strptime(start_date, '%Y-%m-%d'))).to_pandas()
         elif start_date is None:
-            return df.filter((pl.col(a) <= datetime.datetime.strptime(end_date, '%Y-%m-%d')))
+            if polars:
+                return df.filter((pl.col(a) <= datetime.datetime.strptime(end_date, '%Y-%m-%d')))
+            else:
+                return df.filter((pl.col(a) <= datetime.datetime.strptime(end_date, '%Y-%m-%d'))).to_pandas()
         else:
             df = df.filter((pl.col(a) >= datetime.datetime.strptime(start_date, '%Y-%m-%d')))
-            return df.filter((pl.col(a) <= datetime.datetime.strptime(end_date, '%Y-%m-%d')))
+            if polars:
+                return df.filter((pl.col(a) <= datetime.datetime.strptime(end_date, '%Y-%m-%d')))
+            else:
+                return df.filter((pl.col(a) <= datetime.datetime.strptime(end_date, '%Y-%m-%d'))).to_pandas()
 
     def summary(self
-                , username: str
-                , warehouse: str
-                , database: str
-                , role: str
+                , username: str | None = None
+                , warehouse: str | None = None
+                , database: str | None = None
+                , role: str | None = None
                 , columns=None
                 , filters=None
                 , order_by=None
                 , polars: bool = True
                 , start_date: str | None = None
                 , end_date: str | None = None
                 ):
 
+        if username is None:
+            username = self.username
+        if warehouse is None:
+            warehouse = self.warehouse
+        if database is None:
+            database = self.database
+        if role is None:
+            role = self.role
+
+
         import polars as pl
         import pandas as pd
         import configparser
 
         config = configparser.ConfigParser()
         config.read('pip.ini')
 
@@ -122,26 +164,35 @@
         df_pd['PERCENT_EXCLUDED'] = f"{str(round(df_pd['EXCLUDED']/df_pd['RETAILERS'] * 100, 0))}%"
 
         if polars:
             return pl.DataFrame(df_pd)
         return df_pd
 
     def home_summary(self
-                     , username: str
-                     , warehouse: str
-                     , database: str
-                     , role: str
+                     , username: str | None = None
+                     , warehouse: str | None = None
+                     , database: str | None = None
+                     , role: str | None = None
                      , columns=None
                      , filters=None
                      , order_by=None
                      , polars: bool = True
                      , start_date: str | None = None
                      , end_date: str | None = None
                      ):
 
+        if username is None:
+            username = self.username
+        if warehouse is None:
+            warehouse = self.warehouse
+        if database is None:
+            database = self.database
+        if role is None:
+            role = self.role
+
         import datetime
 
         import polars as pl
         import configparser
 
         config = configparser.ConfigParser()
         config.read('pip.ini')
```

### Comparing `NikeCA-0.2.2a0/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.2.2rc0/src/Dashboards/Telemetry/Telemetry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,107 @@
 
-class ProductUsage:
 
-    def get_base_query(self
+from Dashboards.Dashboards import Dashboards
+from NikeCA import Snowflake
+
+
+class Telemetry(Dashboards, Snowflake):
+
+    def __init__(self, username, warehouse, role, database):
+        super().__init__(username=username, warehouse=warehouse, role=role, database=database)
+
+        self.username = username
+        self.warehouse = warehouse
+        self.role = role
+        self.database = database
+
+    @property
+    def ProductUsage(self):
+        from Dashboards.Telemetry.ProductUsage import ProductUsage
+        return ProductUsage(username=self.username, role=self.role, warehouse=self.warehouse, database=self.database)
+
+    def product_viewed(self
+                                 , username: str = None
+                                 , warehouse: str = None
+                                 , database: str = None
+                                 , role: str = None
+                                 , filters: list | None = None
+                                 , order_by: list | None = None
+                                 , polars: bool = False
+                                 , start_date: str = '1900-01-01'
+                                 , end_date: str = '9999-12-31'
+                                 ):
+
+        import polars as pl
+        import configparser
+
+        if username is None:
+            username = self.username
+        if warehouse is None:
+            warehouse = self.warehouse
+        if database is None:
+            database = self.database
+        if role is None:
+            role = self.role
+
+        config = configparser.ConfigParser()
+        config.read('pip.ini')
+
+        b = config['telemetry_product_usage'].get('col_b')
+
+        # Ensure filters is a list
+        if not (isinstance(filters, list) or filters is None):
+            raise TypeError("filters must be a list")
+
+        # Ensure order_by is a list
+        if not (isinstance(order_by, list) or order_by is None):
+            raise TypeError("order_by must be a list")
+
+        if order_by is None:
+            order_by = config['telemetry_product_usage'].get('order_by')
+        else:
+            order_by = ', '.join(order_by)
+
+        print('testt')
+        query = f"""
+                /*
+                The query calculates the daily usage of different data products on different platforms, groups the data by platform and product, and sorts the result in descending order based on the total usage
+                */
+                SELECT 
+                    {b}
+                    , PRODUCT_NAME
+                    , SUM(DAILY_USAGE) AS TOTAL_USAGE
+                FROM (
+
+                {self.telemetry_get_base_query(start_date=start_date, end_date=end_date)}
+
+                )
+
+                GROUP BY 
+                    {b}
+                    , PRODUCT_NAME
+
+                HAVING 
+                    TOTAL_USAGE > 0
+
+                ORDER BY
+                    {order_by}
+
+                ;
+            """
+
+        df = pl.DataFrame(Snowflake(username=username, database=database, warehouse=warehouse,
+                                    role=role).snowflake_pull(query=query, polars=polars))
+
+        print(query)
+
+        return df
+
+
+    def telemetry_get_base_query(self
                        , filters: list | None = None
                        , start_date: str = '1900-01-01'
                        , end_date: str = '9999-12-31'
                        ):
 
         import configparser
 
@@ -37,144 +133,84 @@
         if len(filters) > 0:
             filters_str = 'AND '.join(filters)
             filters_str = f"WHERE {date_column} BETWEEN '{start_date}' AND '{end_date}' AND {filters_str}"
         else:
             filters_str = f"WHERE {date_column} BETWEEN '{start_date}' AND '{end_date}'"
 
         base_query = f"""
-            SELECT
-                DISTINCT 
-                {a}
-                , {b}
-                , CASE 
-                    WHEN {b} = '{filter_a}' THEN {c}
-                    WHEN {b} = '{filter_b}' THEN {d}
-                    WHEN {b} = '{filter_c}' THEN {e}
-                    else null 
-                END AS PRODUCT_NAME
-                , COUNT(DISTINCT {f})
-                , (SUM({g})/NULLIF(COUNT(DISTINCT {f}),0 )) AS DAILY_USAGE
-            FROM 
-                {table}
-            
-            {filters_str}
-            
-            GROUP BY
-                {a}
-                , {b}
-                , PRODUCT_NAME
-    """
-        return base_query
-
-    def product_viewed(self
-                       , username: str
-                       , warehouse: str
-                       , database: str
-                       , role: str
-                       , filters: list | None = None
-                       , order_by: list | None = None
-                       , polars: bool = False
-                       , start_date: str = '1900-01-01'
-                       , end_date: str = '9999-12-31'
-                       ):
-
-        from NikeCA import Snowflake
-        import polars as pl
-        import configparser
-
-        config = configparser.ConfigParser()
-        config.read('pip.ini')
-
-        b = config['telemetry_product_usage'].get('col_b')
-
-        # Ensure filters is a list
-        if not (isinstance(filters, list) or filters is None):
-            raise TypeError("filters must be a list")
-
-        # Ensure order_by is a list
-        if not (isinstance(order_by, list) or order_by is None):
-            raise TypeError("order_by must be a list")
-
-        if order_by is None:
-            order_by = config['telemetry_product_usage'].get('order_by')
-        else:
-            order_by = ', '.join(order_by)
-
-        query = f"""
-            /*
-            The query calculates the daily usage of different data products on different platforms, groups the data by platform and product, and sorts the result in descending order based on the total usage
-            */
-            SELECT 
-                {b}
-                , PRODUCT_NAME
-                , SUM(DAILY_USAGE) AS TOTAL_USAGE
-            FROM (
-
-            {self.get_base_query(start_date=start_date, end_date=end_date)}
-            
-            )
-            
-            GROUP BY 
-                {b}
-                , PRODUCT_NAME
-                
-            HAVING 
-                TOTAL_USAGE > 0
-                
-            ORDER BY
-                {order_by}
-                
-            ;
+                SELECT
+                    DISTINCT 
+                    {a}
+                    , {b}
+                    , CASE 
+                        WHEN {b} = '{filter_a}' THEN {c}
+                        WHEN {b} = '{filter_b}' THEN {d}
+                        WHEN {b} = '{filter_c}' THEN {e}
+                        else null 
+                    END AS PRODUCT_NAME
+                    , COUNT(DISTINCT {f})
+                    , (SUM({g})/NULLIF(COUNT(DISTINCT {f}),0 )) AS DAILY_USAGE
+                FROM 
+                    {table}
+
+                {filters_str}
+
+                GROUP BY
+                    {a}
+                    , {b}
+                    , PRODUCT_NAME
         """
-
-        df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
-                                    role=role).snowflake_pull(query=query, polars=polars))
-
-        print(query)
-
-        return df
+        return base_query
 
     def summary(self
-                , username: str
-                , warehouse: str
-                , database: str
-                , role: str
+                , username: str | None = None
+                , warehouse: str | None = None
+                , database: str | None = None
+                , role: str | None = None
                 , filters: list | None = None
                 , order_by: list | None = None
                 , polars: bool = False
                 , start_date: str = '1900-01-01'
                 , end_date: str = '9999-12-31'
                 ):
         import configparser
 
         config = configparser.ConfigParser()
         config.read('pip.ini')
         b = config['telemetry_product_usage'].get('col_b')
 
+        if username is None:
+            username = self.username
+        if warehouse is None:
+            warehouse = self.warehouse
+        if database is None:
+            database = self.database
+        if role is None:
+            role = self.role
+
         if order_by is None:
             order_by = config['telemetry_product_usage'].get('order_by')
         else:
             order_by = ', '.join(order_by)
 
         query = f"""
-    SELECT 
-        DISTINCT
-        {b}
-        , SUM(DAILY_USAGE) OVER (PARTITION BY {b}) AS TOTAL_USAGE
-    FROM (
-        {self.get_base_query(start_date=start_date, end_date=end_date, filters=filters)}   
-    )
-    ORDER BY
-        {order_by}
-"""
+        SELECT 
+            DISTINCT
+            {b}
+            , SUM(DAILY_USAGE) OVER (PARTITION BY {b}) AS TOTAL_USAGE
+        FROM (
+            {self.telemetry_get_base_query(start_date=start_date, end_date=end_date, filters=filters)}   
+        )
+        ORDER BY
+            {order_by}
+    """
 
-        from NikeCA import Snowflake
+        # from NikeCA import Snowflake
         import polars as pl
 
         df = pl.DataFrame(Snowflake(username=username, warehouse=warehouse, database=database,
                                     role=role).snowflake_pull(query=query, polars=polars))
 
         print(query)
 
         return df
 
-
```

### Comparing `NikeCA-0.2.2a0/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.2.2rc0/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.2a0
+Version: 0.2.2rc0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.2a0/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.2.2rc0/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.2.2rc0/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/src/NikeQA.py` & `NikeCA-0.2.2rc0/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/src/NikeSF.py` & `NikeCA-0.2.2rc0/src/NikeSF.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,17 @@
         return Telemetry(username=self.username, role=self.role, database=self.database, warehouse=self.warehouse)
 
     @property
     def InclusionExclusion(self):
         from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
         return InclusionExclusion(username=self.username, role=self.role, database=self.database, warehouse=self.warehouse)
 
+
+    def test(self):
+        print('teste')
     def build_search_query(self
                            , inp_db: str = None
                            , schema: str = None
                            , table: str = None
                            , column_name=None
                            , like_flag: bool = False
                            , col_and_or: str = 'AND'
```

### Comparing `NikeCA-0.2.2a0/src/_BuildSearchQuery.py` & `NikeCA-0.2.2rc0/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/src/_GitHub.py` & `NikeCA-0.2.2rc0/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/src/_QA.py` & `NikeCA-0.2.2rc0/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/src/_SearchFiles.py` & `NikeCA-0.2.2rc0/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/src/_SnowflakeData.py` & `NikeCA-0.2.2rc0/src/_SnowflakeData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import _BuildSearchQuery
 import _SnowflakePull
 import _SnowflakeDependencies
-from Dashboards import Dashboards
+# from Dashboards import Dashboards
 
 
-class SnowflakeData(Dashboards.Dashboards
-                    , _SnowflakePull.SnowflakePull
+class SnowflakeData(
+                    _SnowflakePull.SnowflakePull
                     , _SnowflakeDependencies.SnowflakeDependencies
                     , _BuildSearchQuery.BuildSearchQuery):
 
     def snowflake_pull(self, query: str | dict | None, un, wh, db, role, schema=None, table=None,
                        sample_table: bool = False, sample_val: bool = False, table_sample: dict = None,
                        dtypes_conv=None, separate_dataframes: bool = True, polars: bool = True): # -> pandas.DataFrame:
```

### Comparing `NikeCA-0.2.2a0/src/_SnowflakeDependencies.py` & `NikeCA-0.2.2rc0/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2a0/src/_SnowflakePull.py` & `NikeCA-0.2.2rc0/src/_SnowflakePull.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,22 +158,22 @@
             finally:
                 cnn.close()
                 print('process complete')
         else:
             # connection settings
             from snowflake.connector.converter_null import SnowflakeNoConverterToPython
             conn = snowflake.connector.connect(
-                user=un,
+                user=str(un),
                 account='nike',
 
                 # opens separate browser window to confirm authentication
                 authenticator='externalbrowser',
-                warehouse=wh,
-                database=db,
-                role=role,
+                warehouse=str(wh),
+                database=str(db),
+                role=str(role),
                 converter_class=SnowflakeNoConverterToPython
             )
 
             # connect to snowflake using conn variables
             cur = conn.cursor()
 
             try:
```

