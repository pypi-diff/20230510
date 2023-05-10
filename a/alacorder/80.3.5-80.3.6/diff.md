# Comparing `tmp/alacorder-80.3.5.tar.gz` & `tmp/alacorder-80.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.3.5.tar", max compression
+gzip compressed data, was "alacorder-80.3.6.tar", max compression
```

## Comparing `alacorder-80.3.5.tar` & `alacorder-80.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.5/LICENSE
--rw-r--r--   0        0        0     6538 2023-05-09 14:42:24.077836 alacorder-80.3.5/README.md
--rw-r--r--   0        0        0      697 2023-05-09 15:03:25.559939 alacorder-80.3.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-09 14:49:08.351375 alacorder-80.3.5/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.5/src/alacorder/__init__.py
--rw-r--r--   0        0        0   210716 2023-05-09 14:48:41.791672 alacorder-80.3.5/src/alacorder/__main__.py
--rw-r--r--   0        0        0   210716 2023-05-09 14:48:34.344123 alacorder-80.3.5/src/alacorder/alac.py
--rw-r--r--   0        0        0     7467 1970-01-01 00:00:00.000000 alacorder-80.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.6/LICENSE
+-rw-r--r--   0        0        0     6538 2023-05-09 14:42:24.077836 alacorder-80.3.6/README.md
+-rw-r--r--   0        0        0      697 2023-05-10 17:48:38.930662 alacorder-80.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-09 14:49:08.351375 alacorder-80.3.6/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.6/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   210898 2023-05-10 17:48:13.766329 alacorder-80.3.6/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   210898 2023-05-10 17:47:57.031458 alacorder-80.3.6/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7467 1970-01-01 00:00:00.000000 alacorder-80.3.6/PKG-INFO
```

### Comparing `alacorder-80.3.5/LICENSE` & `alacorder-80.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.5/README.md` & `alacorder-80.3.6/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.5/pyproject.toml` & `alacorder-80.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.3.5"
+version = "80.3.6"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.3.5/src/alacorder/.DS_Store` & `alacorder-80.3.6/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.5/src/alacorder/__main__.py` & `alacorder-80.3.6/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.5"
+version = "80.3.6"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
+from datetime import datetime
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
 
 #   #   #   #                LOGS                #   #   #   #
@@ -3126,14 +3127,20 @@
             goodquery = True
 
     # add other temp columns as empty
     for col in tempcols:
         if col not in query.columns:
             query = query.with_columns([pl.lit("").alias(col)])
 
+    query = query.with_columns(
+        [
+            pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
+        ]
+    )
+
     if goodquery:
         print(f"{query.shape[0]} queries found in input query file.")
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
@@ -3221,27 +3228,27 @@
             filed_before=r["TEMP_FILED_BEFORE"],
             filed_after=r["TEMP_FILED_AFTER"],
             window=window,
         )
 
         if len(results) > 0:
             print(
-                f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']}) ({len(results)} records returned)"
+                f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']} ({len(results)} records returned)"
             )
             if window:
                 window.write_event_value("PROGRESS-TEXT", 0)
                 window.write_event_value("PROGRESS-TEXT-TOTAL", 100)
-                for i, url in enumerate(results):
-                    window.write_event_value("PROGRESS-TEXT", i + 1)
+                for x, url in enumerate(results):
+                    window.write_event_value("PROGRESS-TEXT", x + 1)
                     downloadPDF(driver, url)
             else:
-                for i, url in enumerate(tqdm(results)):
+                for x, url in enumerate(tqdm(results)):
                     downloadPDF(driver, url)
             query[i, "CASES_FOUND"] = len(results)
-            query[i, "RETRIEVED"] = time.time()
+            query[i, "RETRIEVED"] = datetime.now().strftime("%H:%M:%S %d-%m-%Y")
             query[i, "QUERY_COMPLETE"] = "Y"
             if not no_update:
                 qwrite = query.drop(
                     "TEMP_NAME",
                     "TEMP_PARTY_TYPE",
                     "TEMP_SSN",
                     "TEMP_DOB",
```

### Comparing `alacorder-80.3.5/src/alacorder/alac.py` & `alacorder-80.3.6/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.5"
+version = "80.3.6"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
+from datetime import datetime
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
 
 #   #   #   #                LOGS                #   #   #   #
@@ -3126,14 +3127,20 @@
             goodquery = True
 
     # add other temp columns as empty
     for col in tempcols:
         if col not in query.columns:
             query = query.with_columns([pl.lit("").alias(col)])
 
+    query = query.with_columns(
+        [
+            pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
+        ]
+    )
+
     if goodquery:
         print(f"{query.shape[0]} queries found in input query file.")
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
@@ -3221,27 +3228,27 @@
             filed_before=r["TEMP_FILED_BEFORE"],
             filed_after=r["TEMP_FILED_AFTER"],
             window=window,
         )
 
         if len(results) > 0:
             print(
-                f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']}) ({len(results)} records returned)"
+                f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']} ({len(results)} records returned)"
             )
             if window:
                 window.write_event_value("PROGRESS-TEXT", 0)
                 window.write_event_value("PROGRESS-TEXT-TOTAL", 100)
-                for i, url in enumerate(results):
-                    window.write_event_value("PROGRESS-TEXT", i + 1)
+                for x, url in enumerate(results):
+                    window.write_event_value("PROGRESS-TEXT", x + 1)
                     downloadPDF(driver, url)
             else:
-                for i, url in enumerate(tqdm(results)):
+                for x, url in enumerate(tqdm(results)):
                     downloadPDF(driver, url)
             query[i, "CASES_FOUND"] = len(results)
-            query[i, "RETRIEVED"] = time.time()
+            query[i, "RETRIEVED"] = datetime.now().strftime("%H:%M:%S %d-%m-%Y")
             query[i, "QUERY_COMPLETE"] = "Y"
             if not no_update:
                 qwrite = query.drop(
                     "TEMP_NAME",
                     "TEMP_PARTY_TYPE",
                     "TEMP_SSN",
                     "TEMP_DOB",
```

### Comparing `alacorder-80.3.5/PKG-INFO` & `alacorder-80.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.3.5
+Version: 80.3.6
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

