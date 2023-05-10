# Comparing `tmp/sensorbucket-0.2.0.tar.gz` & `tmp/sensorbucket-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensorbucket-0.2.0.tar", last modified: Mon Oct 24 10:21:09 2022, max compression
+gzip compressed data, was "sensorbucket-1.0.0.tar", last modified: Wed May 10 09:41:21 2023, max compression
```

## Comparing `sensorbucket-0.2.0.tar` & `sensorbucket-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,58 @@
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2022-10-24 10:21:09.532352 sensorbucket-0.2.0/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    13827 2022-10-21 14:13:45.000000 sensorbucket-0.2.0/LICENSE
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2633 2022-10-24 10:21:09.532352 sensorbucket-0.2.0/PKG-INFO
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2314 2022-10-21 14:13:45.000000 sensorbucket-0.2.0/README.md
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2022-10-24 10:21:09.532352 sensorbucket-0.2.0/sensorbucket/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      181 2022-09-22 12:35:14.000000 sensorbucket-0.2.0/sensorbucket/__init__.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       99 2022-09-22 12:35:14.000000 sensorbucket-0.2.0/sensorbucket/errors.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3411 2022-10-21 14:13:45.000000 sensorbucket-0.2.0/sensorbucket/facade.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     5189 2022-10-21 14:14:10.000000 sensorbucket-0.2.0/sensorbucket/models.py
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2022-10-24 10:21:09.532352 sensorbucket-0.2.0/sensorbucket.egg-info/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2633 2022-10-24 10:21:09.000000 sensorbucket-0.2.0/sensorbucket.egg-info/PKG-INFO
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      299 2022-10-24 10:21:09.000000 sensorbucket-0.2.0/sensorbucket.egg-info/SOURCES.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)        1 2022-10-24 10:21:09.000000 sensorbucket-0.2.0/sensorbucket.egg-info/dependency_links.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       26 2022-10-24 10:21:09.000000 sensorbucket-0.2.0/sensorbucket.egg-info/requires.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       13 2022-10-24 10:21:09.000000 sensorbucket-0.2.0/sensorbucket.egg-info/top_level.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       38 2022-10-24 10:21:09.532352 sensorbucket-0.2.0/setup.cfg
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      592 2022-10-21 14:13:45.000000 sensorbucket-0.2.0/setup.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      816 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/PKG-INFO
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     7280 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/README.md
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.023907 sensorbucket-1.0.0/openapi_client/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     4124 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/__init__.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.023907 sensorbucket-1.0.0/openapi_client/api/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      276 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/__init__.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    73878 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/devices_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    25492 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/measurements_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    41586 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/pipelines_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     8949 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/uplink_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    30485 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api_client.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      844 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    15684 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/configuration.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     5599 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/exceptions.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/openapi_client/models/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3352 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/__init__.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2761 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_device201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3030 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_device_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2470 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_device_sensor201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2785 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2532 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_pipeline_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2970 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/create_sensor_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2943 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/datastream.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2470 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/delete_device_sensor200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3682 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/device.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2446 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/disable_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2737 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/get_device200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2761 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/get_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3499 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_datastreams200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2921 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_datastreams200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3499 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_device_sensors200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2921 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_device_sensors200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3451 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_devices200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2873 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_devices200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3475 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_pipelines200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2897 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_pipelines200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     6406 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/measurement.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2992 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/paginated_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2500 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/paginated_response_links.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2836 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/pipeline.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3519 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/query_measurements200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2941 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/query_measurements200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3067 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/sensor.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2422 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/update_device200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2965 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/update_device_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2785 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/update_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2807 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/update_pipeline_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    13245 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/rest.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      713 2023-05-10 09:39:16.000000 sensorbucket-1.0.0/pyproject.toml
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/sensorbucket.egg-info/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      816 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/PKG-INFO
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2153 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/SOURCES.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)        1 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/dependency_links.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       58 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/requires.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       15 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/top_level.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       69 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/setup.cfg
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2134 2023-05-10 09:41:14.000000 sensorbucket-1.0.0/setup.py
```

### Comparing `sensorbucket-0.2.0/sensorbucket/facade.py` & `sensorbucket-1.0.0/openapi_client/models/sensor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,85 @@
-import requests as r
-from urllib.parse import urlparse,parse_qs
-from datetime import datetime, timedelta
-from typing import List, Union
-
-from .models import Measurement, Location, Device
-
-
-class Facade:
-    """Facade is a class which simplifies your interaction with the SensorBucket API."""
-    def __init__(self, url: str, apiKey: str):
-        """This class acts as a Facade for the SensorBucket API
-
-        Parameters
-        ----------
-        url : str
-            The base url for the SensorBucket API
-        apiKey : str
-            API Key used to authenticate with Sensorbucket
-        """
-        self.url = url
-        self.apiKey = apiKey
-
-    def get_locations(self) -> List[Location]:
-        """Fetches all the available locations for the authenticated user
-
-        Returns
-        -------
-        List[Location]
-            The locations
-        """
-        res = r.get(f"{self.url}/api/v1/locations", headers={
-            "authorization": f"bearer {self.apiKey}"
-        })
-        res.raise_for_status()
-        return Location.schema().load(res.json()["data"], many=True)
-
-    def get_devices(self) -> List[Device]:
-        """Fetches all devices for the authenticated user
+# coding: utf-8
 
-        Returns
-        _______
-        List[Device]
-            The list of devices
-        """
-        res = r.get(f"{self.url}/api/v1/devices", headers={
-            "authorization": f"bearer {self.apiKey}"
-        })
-        res.raise_for_status()
-        return Device.schema().load(res.json()["data"], many=True)
+"""
+    Sensorbucket API
 
-    def get_measurements(self,start: Union[datetime, str], end: Union[datetime, str], measurement_type: str = None, location_id: int = None, sensor_code: str = None, limit: int = 100) -> List[Measurement]:
-        """Fetches a list of measurements from a given location in a given time window
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
 
-        Parameters
-        ----------
-        start : Union[datetime, str]
-            The start time of the time window
-        end : Union[datetime, str]
-            The end time of the time windows
-        measurement_type : str
-            ID or name of the measurement type
-        location_id : Optional[int]
-            The location id of the measurements
-        sensor_code : Optional[str]
-            The sensor which performed the measurements
-
-        Returns
-        -------
-        List[Measurement]
-            A list of measurements
-
-        Raises
-        ------
-        """
-
-        # Start and End parameters can be datetime objects, but the API expects
-        # ISO8601 strings, so convert them
-        if type(start) == datetime:
-            start = start.isoformat()
-        if type(end) == datetime:
-            end = end.isoformat()
-
-        # Perform request to API
-        query = {
-            "location_id": location_id,
-            "measurement_type": measurement_type,
-            "start": start,
-            "end": end,
-            "limit": limit
-        }
-
-        while True:
-            res = r.get(f"{self.url}/api/v1/measurements", params=query, headers={
-                "authorization": f"bearer {self.apiKey}"
-            })
-            res.raise_for_status()
-            data = res.json()
-            yield Measurement.schema().load(data["data"], many=True)
-            if data['next'] == "":
-                break
-            else:
-                qs = parse_qs(urlparse(data['next']).query)
-                query["cursor"] = qs.get('cursor')[0]
-        
+    The version of the OpenAPI document: 1.0
+    Contact: info@pollex.nl
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""
+
+
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import Any, Dict, Optional, Union
+from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
+
+class Sensor(BaseModel):
+    """
+    Sensor
+    """
+    id: Optional[Union[StrictFloat, StrictInt]] = None
+    code: Optional[StrictStr] = None
+    description: Optional[StrictStr] = None
+    external_id: Optional[StrictStr] = None
+    brand: Optional[StrictStr] = None
+    archive_time: Optional[Union[StrictFloat, StrictInt]] = None
+    properties: Optional[Dict[str, Any]] = None
+    created_at: Optional[StrictStr] = None
+    __properties = ["id", "code", "description", "external_id", "brand", "archive_time", "properties", "created_at"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Sensor:
+        """Create an instance of Sensor from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> Sensor:
+        """Create an instance of Sensor from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return Sensor.parse_obj(obj)
+
+        _obj = Sensor.parse_obj({
+            "id": obj.get("id"),
+            "code": obj.get("code"),
+            "description": obj.get("description"),
+            "external_id": obj.get("external_id"),
+            "brand": obj.get("brand"),
+            "archive_time": obj.get("archive_time"),
+            "properties": obj.get("properties"),
+            "created_at": obj.get("created_at")
+        })
+        return _obj
```

