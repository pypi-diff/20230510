# Comparing `tmp/NikeCA-0.2.1.tar.gz` & `tmp/NikeCA-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.2.1.tar", last modified: Wed May 10 17:50:52 2023, max compression
+gzip compressed data, was "NikeCA-0.2.2.tar", last modified: Wed May 10 18:28:18 2023, max compression
```

## Comparing `NikeCA-0.2.1.tar` & `NikeCA-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.900535 NikeCA-0.2.1/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.1/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 17:50:52.900140 NikeCA-0.2.1/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.1/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 17:50:52.900655 NikeCA-0.2.1/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2502 2023-05-10 17:50:03.000000 NikeCA-0.2.1/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.892196 NikeCA-0.2.1/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.893756 NikeCA-0.2.1/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4020 2023-05-07 22:07:42.000000 NikeCA-0.2.1/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.894836 NikeCA-0.2.1/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.2.1/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.896470 NikeCA-0.2.1/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6140 2023-05-08 17:16:29.000000 NikeCA-0.2.1/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.899442 NikeCA-0.2.1/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.2.1/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23793 2023-05-08 17:16:29.000000 NikeCA-0.2.1/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.2.1/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.2.1/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.2.1/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.871101 NikeCA-0.2.2/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.2/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 18:28:18.870650 NikeCA-0.2.2/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.2/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 18:28:18.871221 NikeCA-0.2.2/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2502 2023-05-10 18:27:12.000000 NikeCA-0.2.2/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.861583 NikeCA-0.2.2/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.863152 NikeCA-0.2.2/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4020 2023-05-07 22:07:42.000000 NikeCA-0.2.2/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.864641 NikeCA-0.2.2/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.2.2/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.866826 NikeCA-0.2.2/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6140 2023-05-08 17:16:29.000000 NikeCA-0.2.2/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.870016 NikeCA-0.2.2/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.2.2/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19181 2023-05-10 18:07:25.000000 NikeCA-0.2.2/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.2.2/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.2.2/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.2.2/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/__init__.py
```

### Comparing `NikeCA-0.2.1/LICENSE` & `NikeCA-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/PKG-INFO` & `NikeCA-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.1
+Version: 0.2.2
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.1/README.md` & `NikeCA-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/setup.py` & `NikeCA-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.2.1',
+	version='0.2.2',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"_BuildSearchQuery",
 		"_GitHub",
 		"_SearchFiles",
 		"_SnowflakeData",
```

### Comparing `NikeCA-0.2.1/src/Dashboards/Dashboards.py` & `NikeCA-0.2.2/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.2.2/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.2.2/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.2.2/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.2.2/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.1
+Version: 0.2.2
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.1/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.2.2/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.2.2/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/NikeQA.py` & `NikeCA-0.2.2/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/NikeSF.py` & `NikeCA-0.2.2/src/NikeSF.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import pandas as pd
 
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
-from Dashboards.Dashboards import Dashboards
-from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
-from Dashboards.Telemetry.Telemetry import Telemetry
-from Dashboards.Telemetry.ProductUsage import ProductUsage
 
 
-class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery):#, InclusionExclusion):
+class Snowflake(SnowflakeData, SnowflakeDependencies, BuildSearchQuery):
 
-    Dashboards = Dashboards()
-    Telemetry = Telemetry()
-    ProductUsage = ProductUsage()
 
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
@@ -238,14 +231,29 @@
     def polars(self):
         return self.__polars
 
     @polars.setter
     def polars(self, value):
         self.__polars = value
 
+    @property
+    def Dashboards(self):
+        from Dashboards.Dashboards import Dashboards
+        return Dashboards(username=self.username, role=self.role, database=self.database, warehouse=self.warehouse)
+
+    @property
+    def Telemetry(self):
+        from Dashboards.Telemetry.Telemetry import Telemetry
+        return Telemetry(username=self.username, role=self.role, database=self.database, warehouse=self.warehouse)
+
+    @property
+    def InclusionExclusion(self):
+        from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
+        return InclusionExclusion(username=self.username, role=self.role, database=self.database, warehouse=self.warehouse)
+
     def build_search_query(self
                            , inp_db: str = None
                            , schema: str = None
                            , table: str = None
                            , column_name=None
                            , like_flag: bool = False
                            , col_and_or: str = 'AND'
@@ -327,15 +335,15 @@
             :param role:
             :param table:
             :param schema:
         """
 
         # Set default values for the parameters if they are not provided
         if username is None:
-            username = self.__username
+            username = str(self.__username)
         if warehouse is None:
             warehouse = self.__warehouse
         if database is None:
             database = self.__database
         if role is None:
             role = self.__role
         if schema is None:
@@ -515,123 +523,7 @@
         if save_path is None:
             save_path = self.__save_path
 
         return SnowflakeData.snowflake_dependencies(self, tables=tables, username=username,
                                                     warehouse=warehouse, role=role, database=database,
                                                     schema=schema, save_path=save_path)
 
-    def imp_summary_dashboard(self
-                              , username: str | None = None
-                              , warehouse: str | None = None
-                              , database: str | None = None
-                              , role: str | None = None
-                              , date_min: str = '1900-01-01'
-                              , date_max: str = '9999-12-31'
-                              , column_filters=None
-                              , polars: bool = False
-                              ):
-
-        if username is None:
-            username = self.__username
-        if warehouse is None:
-            warehouse = self.__warehouse
-        if database is None:
-            database = self.__database
-        if role is None:
-            role = self.__role
-        if date_min is None:
-            date_min = self.__date_min
-        if date_max is None:
-            date_max = self.__date_max
-        if column_filters is None:
-            column_filters = self.__column_filters
-        if polars is False:
-            polars = self.__polars
-
-        return Dashboards.imp_summary_dashboard(self, username=username, warehouse=warehouse, database=database
-                                                , role=role, date_min=date_min, date_max=date_max,
-                                                column_filters=column_filters, polars=polars)
-
-    def pos_data_quality_review(self
-                                , username: str = None
-                                , warehouse: str = None
-                                , database: str = None
-                                , role: str = None
-                                , columns=None
-                                , filters=None
-                                , order_by=None
-                                , polars: bool = False
-                                , start_date: str | None = None
-                                , end_date: str | None = None
-                                ):
-
-        if username is None:
-            username = self.__username
-        if warehouse is None:
-            warehouse = self.__warehouse
-        if database is None:
-            database = self.__database
-        if role is None:
-            role = self.__role
-        if polars is False:
-            polars = self.__polars
-
-        return InclusionExclusion.pos_data_quality_review(self, username=username, warehouse=warehouse,
-                                                          database=database, role=role, columns=columns,
-                                                          filters=filters, order_by=order_by, polars=polars,
-                                                          start_date=start_date, end_date=end_date)
-
-    def summary(self
-                , username: str = None
-                , warehouse: str = None
-                , database: str = None
-                , role: str = None
-                , columns=None
-                , filters=None
-                , order_by=None
-                , polars: bool = True
-                , start_date: str | None = None
-                , end_date: str | None = None
-                ):
-
-        if username is None:
-            username = self.__username
-        if warehouse is None:
-            warehouse = self.__warehouse
-        if database is None:
-            database = self.__database
-        if role is None:
-            role = self.__role
-        if polars is False:
-            polars = self.__polars
-
-        return InclusionExclusion.summary(self, username=username, warehouse=warehouse, database=database, role=role,
-                                          columns=columns, filters=filters, order_by=order_by, polars=polars,
-                                          start_date=start_date, end_date=end_date)
-
-    def home_summary(self
-                     , username: str = None
-                     , warehouse: str = None
-                     , database: str = None
-                     , role: str = None
-                     , columns=None
-                     , filters=None
-                     , order_by=None
-                     , polars: bool = True
-                     , start_date: str | None = None
-                     , end_date: str | None = None
-                     ):
-
-        if username is None:
-            username = self.__username
-        if warehouse is None:
-            warehouse = self.__warehouse
-        if database is None:
-            database = self.__database
-        if role is None:
-            role = self.__role
-        if polars is False:
-            polars = self.__polars
-
-        return InclusionExclusion.home_summary(self, username=username, warehouse=warehouse, database=database,
-                                               role=role, columns=columns, filters=filters, order_by=order_by,
-                                               polars=polars, start_date=start_date, end_date=end_date)
```

### Comparing `NikeCA-0.2.1/src/_BuildSearchQuery.py` & `NikeCA-0.2.2/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/_GitHub.py` & `NikeCA-0.2.2/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/_QA.py` & `NikeCA-0.2.2/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/_SearchFiles.py` & `NikeCA-0.2.2/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/_SnowflakeData.py` & `NikeCA-0.2.2/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/_SnowflakeDependencies.py` & `NikeCA-0.2.2/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.1/src/_SnowflakePull.py` & `NikeCA-0.2.2/src/_SnowflakePull.py`

 * *Files identical despite different names*

