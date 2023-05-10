# Comparing `tmp/qbandas-1.2.0.tar.gz` & `tmp/qbandas-1.2.1.tar.gz`

## Comparing `qbandas-1.2.0.tar` & `qbandas-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.2.0/requirements.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qbandas-1.2.0/requirements_dev.txt
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/__main__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/data/address-fields.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/data/config.ini
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/data/field_types.json
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/profiles/__init__.py
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/profiles/profiles.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/records/__init__.py
--rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/records/_pack.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/records/records.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/schemas/__init__.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 qbandas-1.2.0/qbandas/schemas/schemas.py
--rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 qbandas-1.2.0/scripts/build.bat
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 qbandas-1.2.0/scripts/doc-build.bat
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 qbandas-1.2.0/test/test_headers.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 qbandas-1.2.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.2.0/LICENSE
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 qbandas-1.2.0/README.md
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 qbandas-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 qbandas-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qbandas-1.2.1/requirements.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qbandas-1.2.1/requirements_dev.txt
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/__main__.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/_constants.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/_pack.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/profiles.py
+-rw-r--r--   0        0        0     8856 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/records.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/schemas.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/data/address-fields.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/data/config.ini
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 qbandas-1.2.1/qbandas/data/field_types.json
+-rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 qbandas-1.2.1/scripts/build.bat
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 qbandas-1.2.1/scripts/doc-build.bat
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 qbandas-1.2.1/test/data.csv
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 qbandas-1.2.1/test/test__pack.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 qbandas-1.2.1/test/test_profiles.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qbandas-1.2.1/test/test_records.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qbandas-1.2.1/test/test_schemas.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 qbandas-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 qbandas-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 qbandas-1.2.1/README.md
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 qbandas-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 qbandas-1.2.1/PKG-INFO
```

### Comparing `qbandas-1.2.0/qbandas/data/field_types.json` & `qbandas-1.2.1/qbandas/data/field_types.json`

 * *Files identical despite different names*

### Comparing `qbandas-1.2.0/qbandas/profiles/profiles.py` & `qbandas-1.2.1/qbandas/profiles.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,76 @@
+'''
+Manage qbandas profiles
+
+Profiles control the authorization of all qbandas requests. Each profile
+contains some set of QuickBase API headers that can be configured using 
+qbandas.set_profile().
+'''
+
 import json
 import os
 import os.path as op
 import re
 
-from .. import USER_PATH
+from ._constants import USER_PATH
+
+try: os.makedirs(op.join(USER_PATH, 'profiles'))
+except FileExistsError: pass
 
 
 def set_profile(profile: str, *, host: str = None, user: str = None, 
                 auth: str = None, temp_token: bool = False, 
                 auto_user: bool = True) -> None:
     '''
     Configure a profile
 
     If no profile exists with the name `profile`, a new profile will be created. Unspecified arguments will not override existing profile 
     information.
+    
+    More information about QuickBase API headers can be found 
+    [here](https://developer.quickbase.com/headers), and more 
+    information about QuickBase API tokens can be found 
+    [here](https://developer.quickbase.com/auth).
 
     Parameters
     ----------
-    name : str
-        The name of the profile to configure
+    profile : str
+        The name of the profile to configure. You will use this name to 
+        reference this profile in all future calls.
     host : str, optional
-        The QuickBase realm hostname, by default None
+        The QuickBase realm hostname. You only need the first part of 
+        the host. For example, you would just need 'demo' from 
+        'demo.quickbase.com', by default None
     user : str, optional
-        The name of the user agent, by default None
+        The name of the user agent. If not supplied, use `auto_user` to
+        fill this in for you, by default None
     auth : str, optional
-        The QuickBase API token, by default None
+        The QuickBase API token. Just the token, you don't need the TEMP
+        or USER specifier, by default None
     temp_token : bool, optional
         Specify if the API token is temporary, by default False
     auto_user : bool, optional
         Specify if this profile should automatically populate the user 
         argument with `profile`, by default True
         
-    Exmaples
-    --------
-    >>> import qbandas as qq
-    >>> qq.set_profile('example', host='sample', auth='12345')
-    >>> qq._get_headers('example')
-    {
-        'QB-Realm-Hostname': 'sample.quickbase.com'
-        'User-Agent': 'example'
-        'Authorization': 'QB-USER-TOKEN 12345'
-    }
-
     '''
 
     token_prefix = 'QB-TEMP-TOKEN ' if temp_token else 'QB-USER-TOKEN '
     generated = {
         'QB-Realm-Hostname': (host + '.quickbase.com') if host else None,
         'User-Agent': profile if auto_user and not user else user,
         'Authorization': (token_prefix + auth) if auth else None
     }
     
     # remove the Nones from both dictonaries
     current = {k: v for k, v in _get_headers(profile).items() if v}
     generated = {k: v for k, v in generated.items() if v}
     
     profile_path = _get_profile_path(profile)
-    mode = 'w' if op.exists(profile_path) else 'x'
-    with open(profile_path, mode) as f:
+    with open(profile_path, 'w') as f:
         json.dump(current | generated, f, indent = 4)
         
 def list_profiles() -> list[str]:
     '''
     List all the usable profiles
 
     Profiles in this list are not guaranteed to authorize your requests.
@@ -75,39 +84,32 @@
     files = os.listdir(op.join(USER_PATH, 'profiles'))    
     return [re.sub(r'\.json', '', x) for x in files]
     
 def is_valid_profile(profile: str, talk: bool = False) -> bool:
     '''
     Check if a profile is usable
 
-    If a profile is valid, you will be able to make requests to the 
-    QuickBase API; however, these requests are not guaranteed to be 
-    authorized. If a profile doesn't exist, it is automaically 
+    If a profile is usable, you will be able to make requests to the 
+    QuickBase API using it; however, these requests are not guaranteed 
+    to be authorized. If a profile doesn't exist, it is automaically 
     invalid. 
 
     Parameters
     ----------
     profile : str
         The name of the profile to check
     talk : bool, optional
         Whether to tell you what is wrong with the profile's headers, by 
         default False
     
     Returns
     -------
     bool
         the validity of the profile
-
-    Examples
-    --------
-    >>> import qbandas as qq
-    >>> qq.create_profile()
-    >>> qq.headers.valid()
-    False
-
+        
     '''
     
     headers = _get_headers(profile)
     
     def error(text):
         '''convenience function for returning an error'''
         import sys
@@ -149,14 +151,15 @@
     profile : str
         Check this profile for headers
 
     Returns
     -------
     dict[str, str] | None
         The API headers if the profile exists or None
+        
     '''
     
     profile_path = _get_profile_path(profile)
     
     if op.exists(profile_path):
         with open(profile_path) as f:
             return json.load(f)
@@ -171,14 +174,15 @@
     profile : str
         The name of the profile
 
     Returns
     -------
     str
         The path to the profile whether it exists or not
+        
     '''
     
     return op.join(USER_PATH, 'profiles', profile + '.json')
 
 def _del_profile(profile: str):
     '''
     Remove a profile from your saved list
```

### Comparing `qbandas-1.2.0/qbandas/records/_pack.py` & `qbandas-1.2.1/qbandas/_pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 '''
 Functions for converting data from Python's representation to 
-QuickBase's representation.
+QuickBase's representation
 '''
 
 import datetime as dt
 import re
 from typing import Any
 
 import pandas as pd
 
 
-def _pack_default(x: Any) -> dict|None:
+def _pack_default(x: Any) -> dict[str, Any] | None:
     '''
     Pack a value into the default QuickBase API format.
 
     Parameters
     ----------
     x : Any
         The value to pack
 
     Returns
     -------
-    dict | None : the packed value
+    dict[str, Any] | None 
+        the packed value
 
     Examples
     --------
-    >>> import qbandas
-    >>> qbandas.pack._pack_default('Object')
+    >>> import qbandas._pack as pack
+    >>> pack._pack_default('Object')
     {'value': 'Object'}
-    >>> qbandas.pack._pack_default(None) == None
+    >>> pack._pack_default(None) == None
     True
 
     '''
 
     if pd.isna(x):
         return None
     return {'value':x}
```

### Comparing `qbandas-1.2.0/qbandas/records/records.py` & `qbandas-1.2.1/qbandas/records.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,57 @@
+'''
+Functions that deal with sending records or information to a Quickbase 
+application.
+'''
+
 import asyncio
 import datetime as dt
-import json
-import os.path as op
 from functools import partial
 
 import pandas as pd
 import requests
 
-from .. import MAX_BATCH_RECORDS, QB_PATH, TIMEZONE_OFFSET
-from ..profiles import _get_headers, is_valid_profile
-from ..schemas import _read_schema
-from . import _pack
-
-with open(op.join(QB_PATH, 'data', 'field_types.json')) as f:
-    FIELD_TYPES = json.load(f)
-    
-# resolve the packing functions
-for _, cnfg in FIELD_TYPES.items():
-    if cnfg["packing-function"]:
-        cnfg["packing-function"] = getattr(_pack, cnfg["packing-function"])
+from ._constants import FIELD_TYPES, MAX_BATCH_RECORDS, TIMEZONE_OFFSET
+from .profiles import _get_headers, is_valid_profile
+from .schemas import _read_schema
 
 
 def upload_records(df: pd.DataFrame, table_name: str, profile: str,
                    drop: bool = False): 
     '''
     Send a table of records (rows) to a table on QuickBase.
 
     If no errors are thrown, the data was successfully uploaded to 
     QuickBase. If an error occurs when sending the data, it is possible 
     that only _some_ of your records will have been uploaded to 
     QuickBase. If that is an issue, please fix the data, and send it 
     all again.
+    
+    Using this method without specifying `-O` to the python interpreter 
+    will print debug info. It can be useful for seeing if the data is 
+    being uploaded correctly.  
 
     Parameters
     ----------
     df : pd.DataFrame
         The table of records
     table_name : str
         Identifies which table to send the data to. You should use 
-        `pull_schema()` to create a valid `table_name`.
+        `fetch_schema()` to create a `table_name`.
     profile : str
         The profile to authorize this request
     drop : bool, optional
-        Toggle dropping extra columns. If False, all columns must match, by deafult False
+        Toggle dropping extra columns. If False, all columns must match, 
+        by deafult False
     '''
 
+    # for developers looking to work on this function, it's a lot of 
+    # code, but it's all sequential. Each peice feeds right into the
+    # next. 
+    
     if __debug__: 
         from pprint import pp
         print(df.head())
     
     # headers
     if not is_valid_profile(profile, talk =  True):
         raise ValueError(f'profile {profile} cannot be used')
@@ -132,31 +135,41 @@
         jobs = []
         for i in range(0, len(records), MAX_BATCH_RECORDS):
             jobs.append(_upload_batch(i))
         await asyncio.gather(*jobs)
         
     asyncio.run(_upload_all())
 
-def fetch_records(table_name: str, profile: str, *, columns: list[str] = None, 
-                  where: str = None, order: list = None, 
-                  group_by: list = None, skip: int = 0, 
-                  limit: int = None) -> pd.DataFrame:
+def fetch_records(table_name: str, profile: str, *columns_, 
+                  columns: list[str] = None, where: str = None, 
+                  order: list = None, group_by: list = None,
+                  skip: int = 0, limit: int = None) -> pd.DataFrame:
     '''
     Fetch a table of records from a QuickBase app
+    
+    This method emulates the functionality of a SQL statement. 
 
-    Retrieves records from QuickBase
+    More information about fetching 
+    records through the QuickBase API can be found 
+    [here](https://developer.quickbase.com/operation/runQuery).
+    
+    Using this method without specifying `-O` to the python interpreter 
+    will print debug info. It can be useful for seeing if the data is 
+    being fetched correctly.  
 
     Parameters
     ----------
     table_name : str
-        The table to pull from
+        The table to pull records from
     profile : str
         The name of the profile to authorize this request
     columns : list[str], optional
         The columns to select, by default None
+    *columns_ : list[str], optional
+        More columns to select, by default list()
     where : str, optional
         Should be written like an SQL statement, by default None
     order : list, optional
         The order in which to sort the returned records. Each entry 
         in this list is a tuple with the first element being the 
         column name, and the second is the word 'asc' or 'desc'. 
         by default None
```

### Comparing `qbandas-1.2.0/LICENSE` & `qbandas-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbandas-1.2.0/README.md` & `qbandas-1.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # qBandas
 
-qBandas (QuickBase + Pandas) is a Python package designed to effeciently transfer tabular data between QuickBase applications and the popular Python data handling library Pandas. If you are new to Pandas, you can read more about it [here](https://pandas.pydata.org/).
+qBandas (QuickBase + Pandas) is a Python package designed to effeciently 
+transfer tabular data between QuickBase applications and the popular Python data
+handling package Pandas. If you are new to Pandas, you can read more about it 
+[here](https://pandas.pydata.org/).
 
 The advantages of this approach over a QuickBase pipeline are:
-* Access to databases through Python libraries like [pyodbc](https://github.com/mkleehammer/pyodbc) and [SASPy](https://sassoftware.github.io/saspy/).
-* Greater control over features like error logging, data processing, automated reporting, and scheduling.
+
+* Access to databases through Python packages.
+* Greater control over features like error logging, data processing, 
+  automated reporting, and scheduling.
 * Significantly less performance impact on your QuickBase application.
 * Access tabular data from local sources. 
 * Easily pull data from a QuickBase app into Python.
 
 The disadvantages of this approach compared to a pipeline are:
-* Requires some knowledge of Python and Pandas.
 
-[Read the docs](https://jhopwood-jjk.github.io/qbandas/index.html)
-
-## Setup
+* Requires some knowledge of Python and Pandas.
 
-To use this library, simply get it from pypi. First, update your pip, then install qBandas 
+Please [read the docs](https://jhopwood-jjk.github.io/qbandas/index.html) before
+using this package.
 
+## Installation
 
 ```bash
-python -m pip install -U pip qbandas
+python3 -m pip install -U pip qbandas
 ```
 
 You can now use it through import.
 
 ```python
 import qbandas
 ```
```

### Comparing `qbandas-1.2.0/pyproject.toml` & `qbandas-1.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "qbandas"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name = "Joshua Hopwood" },
 ]
 description = "Integrates the popular data handling library Pandas and the QuickBase API"
 dependencies = [
   "pandas==1.4.3",
   "requests==2.28.1"
```

### Comparing `qbandas-1.2.0/PKG-INFO` & `qbandas-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbandas
-Version: 1.2.0
+Version: 1.2.1
 Summary: Integrates the popular data handling library Pandas and the QuickBase API
 Project-URL: homepage, https://pypi.org/project/qbandas/
 Project-URL: repository, https://github.com/jhopwood-jjk/qBandas
 Project-URL: documentation, https://jhopwood-jjk.github.io/qbandas/index.html
 Author: Joshua Hopwood
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -13,35 +13,39 @@
 Requires-Python: >=3.7
 Requires-Dist: pandas==1.4.3
 Requires-Dist: requests==2.28.1
 Description-Content-Type: text/markdown
 
 # qBandas
 
-qBandas (QuickBase + Pandas) is a Python package designed to effeciently transfer tabular data between QuickBase applications and the popular Python data handling library Pandas. If you are new to Pandas, you can read more about it [here](https://pandas.pydata.org/).
+qBandas (QuickBase + Pandas) is a Python package designed to effeciently 
+transfer tabular data between QuickBase applications and the popular Python data
+handling package Pandas. If you are new to Pandas, you can read more about it 
+[here](https://pandas.pydata.org/).
 
 The advantages of this approach over a QuickBase pipeline are:
-* Access to databases through Python libraries like [pyodbc](https://github.com/mkleehammer/pyodbc) and [SASPy](https://sassoftware.github.io/saspy/).
-* Greater control over features like error logging, data processing, automated reporting, and scheduling.
+
+* Access to databases through Python packages.
+* Greater control over features like error logging, data processing, 
+  automated reporting, and scheduling.
 * Significantly less performance impact on your QuickBase application.
 * Access tabular data from local sources. 
 * Easily pull data from a QuickBase app into Python.
 
 The disadvantages of this approach compared to a pipeline are:
-* Requires some knowledge of Python and Pandas.
 
-[Read the docs](https://jhopwood-jjk.github.io/qbandas/index.html)
-
-## Setup
+* Requires some knowledge of Python and Pandas.
 
-To use this library, simply get it from pypi. First, update your pip, then install qBandas 
+Please [read the docs](https://jhopwood-jjk.github.io/qbandas/index.html) before
+using this package.
 
+## Installation
 
 ```bash
-python -m pip install -U pip qbandas
+python3 -m pip install -U pip qbandas
 ```
 
 You can now use it through import.
 
 ```python
 import qbandas
 ```
```

