# Comparing `tmp/spotON_sdk-0.0.3.3.tar.gz` & `tmp/spotON_sdk-0.0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.3.3.tar", last modified: Tue May  9 15:29:24 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.3.4.tar", last modified: Tue May  9 22:02:11 2023, max compression
```

## Comparing `spotON_sdk-0.0.3.3.tar` & `spotON_sdk-0.0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.3/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.3/LICENSE
--rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.3/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-09 15:29:20.830201 spotON_sdk-0.0.3.3/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.3/spotON_sdk/constants/bidding_zones.py
--rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.3/spotON_sdk/constants/countries.py
--rw-r--r--   0        0        0     2068 2023-05-09 14:25:18.706494 spotON_sdk-0.0.3.3/spotON_sdk/constants/markets.py
--rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.3.3/spotON_sdk/logic/BestHour.py
--rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.3/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.3/spotON_sdk/logic/Entsoe_query.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.3/spotON_sdk/logic/dataframe_modifier.py
--rw-r--r--   0        0        0      201 2023-05-08 20:50:42.181852 spotON_sdk-0.0.3.3/tests/test.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.3.4/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.3.4/LICENSE
+-rw-r--r--   0        0        0      317 2023-05-09 09:46:50.739083 spotON_sdk-0.0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-09 22:01:53.903935 spotON_sdk-0.0.3.4/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.3.4/spotON_sdk/constants/bidding_zones.py
+-rw-r--r--   0        0        0     4567 2023-05-09 10:06:06.205353 spotON_sdk-0.0.3.4/spotON_sdk/constants/countries.py
+-rw-r--r--   0        0        0     2142 2023-05-09 22:01:08.230855 spotON_sdk-0.0.3.4/spotON_sdk/constants/markets.py
+-rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.3.4/spotON_sdk/logic/BestHour.py
+-rw-r--r--   0        0        0     2846 2023-05-08 10:29:44.045628 spotON_sdk-0.0.3.4/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0     3480 2023-05-09 10:03:04.606749 spotON_sdk-0.0.3.4/spotON_sdk/logic/Entsoe_query.py
+-rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.3.4/spotON_sdk/logic/dataframe_modifier.py
+-rw-r--r--   0        0        0       94 2023-05-09 21:55:38.975092 spotON_sdk-0.0.3.4/tests/test.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.3.4/PKG-INFO
```

### Comparing `spotON_sdk-0.0.3.3/.gitignore` & `spotON_sdk-0.0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.3/LICENSE` & `spotON_sdk-0.0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.3/spotON_sdk/constants/bidding_zones.py` & `spotON_sdk-0.0.3.4/spotON_sdk/constants/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.3/spotON_sdk/constants/countries.py` & `spotON_sdk-0.0.3.4/spotON_sdk/constants/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.3/spotON_sdk/constants/markets.py` & `spotON_sdk-0.0.3.4/spotON_sdk/constants/markets.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .countries import *
 from .bidding_zones import bidding_zones
 
 @dataclass
 class Market():
     area:Area
     country :Country
+    alias : List[str] | None = None
     area_code :str = field(init=False)
     country_code : str = field(init=False)
     region_code : str | None = field(init=False,default=None)
     cities : str = field(init=False)
 
     def __post_init__(self):
         self.area_code = self.area.name
@@ -37,22 +38,22 @@
 
         self.name = f"{self.country.emoji} {self.country.country_name} {self.area_code} {self.cities}"
         #self.get_Market_by_area_code(self.area.name)
 
 dataclass
 class Markets():
     austria = Market(Area.AT,Austria)
-    germany = Market(Area.DE_LU,Germany)
-    luxembourg = Market(Area.DE_LU,Luxembourg)
+    germany = Market(Area.DE_LU,Germany,alias="DE_LU")
+    #luxembourg = Market(Area.DE_LU,Luxembourg)
     sweden1 = Market(Area.SE_1,Sweden)
     #sweden2 = Market(Area.SE_2,Sweden)
     #sweden3 = Market(Area.SE_3,Sweden)
     #sweden4 = Market(Area.SE_4,Sweden)
     markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
-
+    merged_Markets = []
     @staticmethod
     def get_Market_by_area_code(area_code: str) -> Optional[Market]:
         for country in Markets.markets_List:
             if country.country_code == area_code:
                 return country
 
         return None
```

### Comparing `spotON_sdk-0.0.3.3/spotON_sdk/logic/BestHour.py` & `spotON_sdk-0.0.3.4/spotON_sdk/logic/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.3/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.3.4/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.3/spotON_sdk/logic/Entsoe_query.py` & `spotON_sdk-0.0.3.4/spotON_sdk/logic/Entsoe_query.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.3.3/spotON_sdk/logic/dataframe_modifier.py` & `spotON_sdk-0.0.3.4/spotON_sdk/logic/dataframe_modifier.py`

 * *Files identical despite different names*

