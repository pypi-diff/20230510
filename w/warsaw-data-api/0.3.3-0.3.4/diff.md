# Comparing `tmp/warsaw_data_api-0.3.3.tar.gz` & `tmp/warsaw_data_api-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warsaw_data_api-0.3.3.tar", max compression
+gzip compressed data, was "warsaw_data_api-0.3.4.tar", max compression
```

## Comparing `warsaw_data_api-0.3.3.tar` & `warsaw_data_api-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1098 2023-05-10 19:07:42.200389 warsaw_data_api-0.3.3/LICENSE.md
--rw-r--r--   0        0        0     1692 2023-05-10 19:07:42.932399 warsaw_data_api-0.3.3/README.md
--rw-r--r--   0        0        0      689 2023-05-10 19:07:42.940399 warsaw_data_api-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      234 2023-05-10 19:07:42.932399 warsaw_data_api-0.3.3/warsaw_data_api/__init__.py
--rw-r--r--   0        0        0      688 2023-05-10 19:07:42.200389 warsaw_data_api-0.3.3/warsaw_data_api/exceptions.py
--rw-r--r--   0        0        0      297 2023-05-10 19:07:42.200389 warsaw_data_api-0.3.3/warsaw_data_api/session.py
--rw-r--r--   0        0        0     4692 2023-05-10 19:07:42.200389 warsaw_data_api-0.3.3/warsaw_data_api/ztm/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-10 19:07:42.200389 warsaw_data_api-0.3.3/warsaw_data_api/ztm/models.py
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 warsaw_data_api-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-10 21:28:19.104042 warsaw_data_api-0.3.4/LICENSE.md
+-rw-r--r--   0        0        0     1535 2023-05-10 21:28:19.792040 warsaw_data_api-0.3.4/README.md
+-rw-r--r--   0        0        0     1136 2023-05-10 21:28:19.800041 warsaw_data_api-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-05-10 21:28:19.788040 warsaw_data_api-0.3.4/warsaw_data_api/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-10 21:28:19.104042 warsaw_data_api-0.3.4/warsaw_data_api/exceptions.py
+-rw-r--r--   0        0        0      294 2023-05-10 21:28:19.104042 warsaw_data_api-0.3.4/warsaw_data_api/session.py
+-rw-r--r--   0        0        0     4942 2023-05-10 21:28:19.104042 warsaw_data_api-0.3.4/warsaw_data_api/ztm/__init__.py
+-rw-r--r--   0        0        0     2423 2023-05-10 21:28:19.104042 warsaw_data_api-0.3.4/warsaw_data_api/ztm/models.py
+-rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 warsaw_data_api-0.3.4/PKG-INFO
```

### Comparing `warsaw_data_api-0.3.3/LICENSE.md` & `warsaw_data_api-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `warsaw_data_api-0.3.3/README.md` & `warsaw_data_api-0.3.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -68,22 +68,7 @@
 
 ### Passing API Key
 
 We can pass API Key in two different ways:
 
 1. Pass API Key to factory function (`ztm()` in this case) as a parameter `ztm = warsaw_data_api.ztm(apikey='your_api_key')`
 2. Create environment variable called `WARSAW_DATA_API_KEY`
-
-## Running tests:
-
-1. Go to root directory
-2. Install packages:
-
-```bash
-pip install -r requirements.txt
-```
-
-3. Run tests:
-
-```bash
-python -m unittest
-```
```

### Comparing `warsaw_data_api-0.3.3/warsaw_data_api/exceptions.py` & `warsaw_data_api-0.3.4/warsaw_data_api/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # All exceptions in this class should subclass from WarsawDataApiException
 class WarsawDataApiException(Exception):
     """Base class for all warsaw-data-api errors."""
 
 
 class LongitudeOutsideBoundaryException(WarsawDataApiException):
     def __init__(
-        self, longitude, message="Longitude is not in (-180, 180) range"
+        self, longitude: float, message: str = "Longitude is not in (-180, 180) range"
     ):
         self.longitude = longitude
         self.message = message
         super().__init__(self.message)
 
 
 class LatitudeOutsideBoundaryException(WarsawDataApiException):
-    def __init__(self, latitude, message="Latitude is not in (-90, 90) range"):
+    def __init__(self, latitude: float, message: str = "Latitude is not in (-90, 90) range"):
         self.latitude = latitude
         self.message = message
         super().__init__(self.message)
```

### Comparing `warsaw_data_api-0.3.3/warsaw_data_api/ztm/__init__.py` & `warsaw_data_api-0.3.4/warsaw_data_api/ztm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from .models import ZtmSchedule, ZtmRide, ZtmVehicle, Location
 from datetime import datetime
-from typing import List, Dict, Union
+from typing import Any, List, Dict, Optional, Union
 import requests
 
 from warsaw_data_api.session import Session
+from .models import ZtmSchedule, ZtmRide, ZtmVehicle, Location
 
 
 class ZtmSession(Session):
     location_endpoint: str
     schedule_endpoint: str
 
-    def __init__(self, apikey: str = None) -> None:
+    def __init__(self, apikey: Optional[str] = None) -> None:
         super().__init__(apikey=apikey)
         self.location_endpoint = (
             "https://api.um.warszawa.pl/api/action/busestrams_get/"
         )
         self.schedule_endpoint = (
             "https://api.um.warszawa.pl/api/action/dbtimetable_get"
         )
 
     def __parse_vehicle_location_data(
-        self, record, vehicle_type: int
+        self, record: Dict[str, str], vehicle_type: int
     ) -> ZtmVehicle:
         return ZtmVehicle(
             location=Location(
                 longitude=float(record["Lon"]), latitude=float(record["Lat"])
             ),
             line=record["Lines"],
             vehicle_number=record["VehicleNumber"],
             time=datetime.strptime(record["Time"], "%Y-%m-%d %H:%M:%S"),
             brigade=int(record["Brigade"]),
             type=vehicle_type,
         )
 
     def __parse_multiple_vehicle_location_data(
-        self, records, vehicle_type: int
+        self, records: List[Dict[str, str]], vehicle_type: int
     ) -> List[ZtmVehicle]:
         vehicles = []
         for record in records:
             vehicles.append(
                 self.__parse_vehicle_location_data(
                     record=record, vehicle_type=vehicle_type
                 )
             )
 
         return vehicles
 
-    def __get_data_from_ztm(self, url, query_params):
+    def __get_data_from_ztm(self, url: str, query_params: Dict[str, Union[str, int, None]]) -> Any:
         r = requests.get(url=url, params=query_params)
         if r.status_code == requests.codes.ok:
             response = r.json()
         else:
             raise Exception(
                 f"Error fetching data from {url}, status: {r.status_code}"
             )
 
         if response.get("error"):
             raise Exception(response["error"])
 
-        return response["result"]
+        return [*response["result"]]  # TODO
 
     def __get_vehicle_location(
-        self, vehicle_type: int, line: str = None
+        self, vehicle_type: int, line: Optional[str] = None
     ) -> List[ZtmVehicle]:
         query_params: Dict[str, Union[str, int, None]] = {
             "resource_id": "f2e5503e927d-4ad3-9500-4ab9e55deb59",
             "type": vehicle_type,
             "apikey": self.apikey,
             "line": line,
         }
@@ -74,52 +74,52 @@
         )
         vehicles = self.__parse_multiple_vehicle_location_data(
             response, vehicle_type
         )
 
         return vehicles
 
-    def get_buses_location(self, line: str = None) -> List[ZtmVehicle]:
+    def get_buses_location(self, line: Optional[str] = None) -> List[ZtmVehicle]:
         return self.__get_vehicle_location(line=line, vehicle_type=1)
 
-    def get_trams_location(self, line: str = None) -> List[ZtmVehicle]:
+    def get_trams_location(self, line: Optional[str] = None) -> List[ZtmVehicle]:
         return self.__get_vehicle_location(line=line, vehicle_type=2)
 
-    def __parse_schedule_data(self, schedule) -> ZtmRide:
+    def __parse_schedule_data(self, schedule: Dict[str, str]) -> ZtmRide:
         return ZtmRide(
             int(schedule["brygada"]),
             schedule["kierunek"],
             schedule["trasa"],
             schedule["czas"],
         )
 
-    def __parse_multiple_schedule_data(self, schedules) -> List[ZtmRide]:
+    def __parse_multiple_schedule_data(self, schedules: List[Dict[str, List[Dict[str, str]]]]) -> List[ZtmRide]:
         rides = []
         for record in schedules:
             clean_record = convert_list_to_dict(record["values"])
             rides.append(self.__parse_schedule_data(clean_record))
 
         return rides
 
     def get_bus_stop_schedule_by_id(
-        self, bus_stop_id: int, bus_stop_nr: str, line: str
+        self, bus_stop_id: str, bus_stop_nr: str, line: str
     ) -> ZtmSchedule:
         query_params: Dict[str, Union[str, int, None]] = {
             "id": "e923fa0e-d96c-43f9-ae6e-60518c9f3238",
             "apikey": self.apikey,
             "busstopId": bus_stop_id,
             "busstopNr": bus_stop_nr,
             "line": line,
         }
         response = self.__get_data_from_ztm(
             self.schedule_endpoint, query_params
         )
         rides = self.__parse_multiple_schedule_data(response)
 
-        ztm_schedule = ZtmSchedule(line, bus_stop_id, bus_stop_nr, rides)
+        ztm_schedule = ZtmSchedule(line, int(bus_stop_id), bus_stop_nr, rides)
 
         return ztm_schedule
 
     def get_bus_stop_schedule_by_name(
         self, bus_stop_name: str, bus_stop_nr: str, line: str
     ) -> ZtmSchedule:
         query_params: Dict[str, Union[str, int, None]] = {
@@ -133,13 +133,13 @@
         clean_response = convert_list_to_dict(response[0]["values"])
         return self.get_bus_stop_schedule_by_id(
             clean_response["zespol"], bus_stop_nr, line
         )
 
 
 # utils
-def convert_list_to_dict(input_list):
+def convert_list_to_dict(input_list: List[Dict[str, str]]) -> Dict[str, str]:
     output_dict = {}
     for x in input_list:
         output_dict[x["key"]] = x["value"]
 
     return output_dict
```

### Comparing `warsaw_data_api-0.3.3/warsaw_data_api/ztm/models.py` & `warsaw_data_api-0.3.4/warsaw_data_api/ztm/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,21 +44,23 @@
         self.location = location
         self.lines = line
         self.vehicle_number = vehicle_number
         self.time = time
         self.brigade = brigade
         self.type = type
 
-    def __str__(self):
+    def __str__(self) -> str:
         return (
             f"ZtmVehicle(line={self.lines}, type={self.type}, "
-            "lat={self.location.latitude}, lon={self.location.longitude})"
+            f"lat={self.location.latitude}, lon={self.location.longitude})"
         )
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, ZtmVehicle):
+            raise NotImplementedError
         return self.__dict__ == other.__dict__
 
 
 @dataclass
 class ZtmRide:
     brigade: int
     direction: str
@@ -88,9 +90,11 @@
         rides: List[ZtmRide],
     ) -> None:
         self.line = line
         self.bus_stop_id = bus_stop_id
         self.bus_stop_nr = bus_stop_nr
         self.rides = rides
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, ZtmSchedule):
+            raise NotImplementedError
         return self.__dict__ == other.__dict__
```

### Comparing `warsaw_data_api-0.3.3/PKG-INFO` & `warsaw_data_api-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warsaw-data-api
-Version: 0.3.3
+Version: 0.3.4
 Summary: Warsaw data python api
 Home-page: https://github.com/radekwielonski/warsaw-data-api
 License: MIT
 Author: Radoslaw Wielonski
 Author-email: radek.wielonski@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -88,22 +88,7 @@
 ### Passing API Key
 
 We can pass API Key in two different ways:
 
 1. Pass API Key to factory function (`ztm()` in this case) as a parameter `ztm = warsaw_data_api.ztm(apikey='your_api_key')`
 2. Create environment variable called `WARSAW_DATA_API_KEY`
 
-## Running tests:
-
-1. Go to root directory
-2. Install packages:
-
-```bash
-pip install -r requirements.txt
-```
-
-3. Run tests:
-
-```bash
-python -m unittest
-```
-
```

