# Comparing `tmp/spotON_sdk-0.0.3.4.tar.gz` & `tmp/spotON_sdk-0.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.3.4.tar", last modified: Tue May  9 22:02:11 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.3.5.tar", last modified: Tue May  9 22:15:45 2023, max compression
```

## Comparing `spotON_sdk-0.0.3.4.tar` & `spotON_sdk-0.0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.4/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.4/LICENSE
--rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.4/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-09 22:01:53.903935 spotON_sdk-0.0.3.4/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.4/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.4/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2142 2023-05-09 22:01:08.230855 spotON_sdk-0.0.3.4/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.3.4/spotON_sdk/logic/BestHour.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.4/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.4/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.4/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0       94 2023-05-09 21:55:38.975092 spotON_sdk-0.0.3.4/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.5/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.5/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-09 22:15:41.320706 spotON_sdk-0.0.3.5/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.5/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.5/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2215 2023-05-09 22:15:15.648490 spotON_sdk-0.0.3.5/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.3.5/spotON_sdk/logic/BestHour.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.5/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.5/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.5/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0       94 2023-05-09 21:55:38.975092 spotON_sdk-0.0.3.5/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.5/PKG-INFO
```

### Comparing `spotON_sdk-0.0.3.4/.gitignore` & `spotON_sdk-0.0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.4/LICENSE` & `spotON_sdk-0.0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.4/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.3.5/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.4/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.3.5/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.4/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.3.5/spotON_sdk/constants/markets.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,16 @@
             my_string = ', '.join(city_List)
             self.cities = my_string
         except:
             self.cities = ""
 
 
         self.name = f"{self.country.emoji} {self.country.country_name} {self.area_code} {self.cities}"
+        self.name = f"{self.country.emoji} {self.country.country_name}"
+
         #self.get_Market_by_area_code(self.area.name)
 
 dataclass
 class Markets():
     austria = Market(Area.AT,Austria)
     germany = Market(Area.DE_LU,Germany,alias="DE_LU")
     #luxembourg = Market(Area.DE_LU,Luxembourg)
```

### Comparing `spotON_sdk-0.0.3.4/spotON_sdk/logic/BestHour.py` & `spotON_sdk-0.0.3.5/spotON_sdk/logic/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.4/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.3.5/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.4/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.3.5/spotON_sdk/logic/Entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.4/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.3.5/spotON_sdk/logic/dataframe_modifier.py`

 * *Files identical despite different names*

