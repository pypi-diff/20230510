# Comparing `tmp/polymatica_api-0.1.0.tar.gz` & `tmp/polymatica_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.1.0.tar", last modified: Sat May  6 17:32:07 2023, max compression
+gzip compressed data, was "polymatica_api-0.2.0.tar", last modified: Wed May 10 18:58:42 2023, max compression
```

## Comparing `polymatica_api-0.1.0.tar` & `polymatica_api-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-06 17:32:07.320909 polymatica_api-0.1.0/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.1.0/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-06 17:32:07.320717 polymatica_api-0.1.0/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      948 2023-05-06 17:31:41.000000 polymatica_api-0.1.0/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-06 17:32:07.319233 polymatica_api-0.1.0/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     2474 2023-05-06 17:26:38.000000 polymatica_api-0.1.0/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.1.0/polymatica_api/data.py
--rw-r--r--   0 leggnom    (501) staff       (20)     5825 2023-05-06 15:46:48.000000 polymatica_api-0.1.0/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)     2370 2023-05-06 15:20:02.000000 polymatica_api-0.1.0/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-06 17:32:07.320453 polymatica_api-0.1.0/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/requires.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-06 17:32:07.320973 polymatica_api-0.1.0/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-06 14:49:31.000000 polymatica_api-0.1.0/setup.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 18:58:42.312589 polymatica_api-0.2.0/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.2.0/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-10 18:58:42.312380 polymatica_api-0.2.0/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      948 2023-05-06 17:31:41.000000 polymatica_api-0.2.0/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 18:58:42.310971 polymatica_api-0.2.0/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     2870 2023-05-10 18:57:42.000000 polymatica_api-0.2.0/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.2.0/polymatica_api/data.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     5825 2023-05-06 15:46:48.000000 polymatica_api-0.2.0/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     2674 2023-05-10 18:55:53.000000 polymatica_api-0.2.0/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 18:58:42.312100 polymatica_api-0.2.0/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/requires.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-10 18:58:42.312656 polymatica_api-0.2.0/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-10 18:58:35.000000 polymatica_api-0.2.0/setup.py
```

### Comparing `polymatica_api-0.1.0/LICENSE` & `polymatica_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.1.0/PKG-INFO` & `polymatica_api-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica_api
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
```

### Comparing `polymatica_api-0.1.0/README.md` & `polymatica_api-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.1.0/polymatica_api/__init__.py` & `polymatica_api-0.2.0/polymatica_api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from .types import Dataset, Data
+from .types import Dataset, Data, CreateColumn
 from .data_option import DataOption
 
 import typing
 import requests
 import urllib.parse
 
 
 HOST_ROUTE = dict(
     dataset='/proxy/manager/api/v1/dataset',
     data_dataset='/proxy/manager/api/v1/data/dataset',
     write_line='/api/v1/data-line/{id}',
     write_lines='/api/v1/data-line/{id}/rows',
     delete_line='/api/v1/data-line/{id}/{uid}',
-    update_line='/api/v1/data-line/{id}/{uid}'
+    update_line='/api/v1/data-line/{id}/{uid}',
+    dataset_create='/api/v1/dataset-local'
 )
 
 
 class PolymaticaAPI:
     _host: str
     _session: requests.Session
 
@@ -62,11 +63,20 @@
 
         result = dict()
         for key in data:
             result[key] = Data.parse_obj(data[key])
 
         return result
 
+    def create_dataset(self, name: str, columns: typing.List[CreateColumn], descriotion: str=''):
+        data = self._session.post(self.route('dataset_create'), json=dict(
+            name=name,
+            descriotion=descriotion,
+            columns=list(map(lambda item: item.dict(), columns))
+        ))
+
+        return data.json()
+
     def route(self, name: str) -> str:
         if name not in HOST_ROUTE:
             raise Exception(f'Route "{name}" not found')
         return urllib.parse.urljoin(self._host, HOST_ROUTE[name])
```

### Comparing `polymatica_api-0.1.0/polymatica_api/data_option.py` & `polymatica_api-0.2.0/polymatica_api/data_option.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.1.0/polymatica_api/types.py` & `polymatica_api-0.2.0/polymatica_api/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 
 
 class _BaseEnum(Enum):
     def __str__(self):
         return self.value
 
 
+class ColumnBaseType(int, _BaseEnum):
+    String = 0
+    Number = 1
+    Date = 2
+    Boolean = 3
+
+
+
 class SortDirection(_BaseEnum):
     Asc = 'ASC'
     Desc = 'DESC'
 
 
 class DataOptionBlockAggFn(_BaseEnum):
     Any = '-'
@@ -55,14 +63,27 @@
     EndsLikeCaseIgnore = 'END_LIKE_I'
     EndsLikeNot = 'NEND_LIKE'
     EndsLikeNotCaseIgnore = 'NEND_LIKE_I'
     DateRange = 'DATE_RANGE'
     DateRangeNot = 'NDATE_RANGE'
 
 
+
+class CreateColumn(BaseModel):
+    name: str
+    path: str
+    source_path: Optional[str]
+    field_type: Optional[str]
+    base_type: ColumnBaseType
+
+    class Config:
+        use_enum_values = True
+
+
+
 class Column(BaseModel):
     id: int
     name: str
     field_type: str
     base_type: int
     path: str
     source_path: str
```

### Comparing `polymatica_api-0.1.0/polymatica_api.egg-info/PKG-INFO` & `polymatica_api-0.2.0/polymatica_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica-api
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
```

### Comparing `polymatica_api-0.1.0/setup.py` & `polymatica_api-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     "pydantic==1.10.7",
     "requests==2.29.0"
 ]
 
 setuptools.setup(
     name="polymatica_api",
-    version="0.1.0",
+    version="0.2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.7',
```

