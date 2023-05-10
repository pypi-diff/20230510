# Comparing `tmp/databend_py-0.3.9-py3-none-any.whl.zip` & `tmp/databend_py-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 16256 bytes, number of entries: 17
--rw-r--r--  2.0 unx      227 b- defN 23-Mar-23 13:43 databend_py/__init__.py
--rw-r--r--  2.0 unx     9557 b- defN 23-Mar-23 13:43 databend_py/client.py
--rw-r--r--  2.0 unx     6043 b- defN 23-Mar-23 13:14 databend_py/connection.py
+Zip file size: 16651 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      227 b- defN 23-May-10 01:50 databend_py/__init__.py
+-rw-r--r--  2.0 unx    10825 b- defN 23-May-08 09:31 databend_py/client.py
+-rw-r--r--  2.0 unx     6321 b- defN 23-May-08 09:31 databend_py/connection.py
 -rw-r--r--  2.0 unx      909 b- defN 22-Nov-07 03:45 databend_py/context.py
 -rw-r--r--  2.0 unx      931 b- defN 23-Jan-12 08:08 databend_py/datetypes.py
 -rw-r--r--  2.0 unx      184 b- defN 22-Nov-16 02:52 databend_py/defines.py
 -rw-r--r--  2.0 unx      581 b- defN 22-Nov-07 03:45 databend_py/errors.py
 -rw-r--r--  2.0 unx      206 b- defN 22-Nov-07 03:45 databend_py/log.py
 -rw-r--r--  2.0 unx     2128 b- defN 23-Feb-13 02:21 databend_py/result.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-07 03:45 databend_py/util/__init__.py
 -rw-r--r--  2.0 unx     1452 b- defN 22-Nov-07 03:45 databend_py/util/escape.py
 -rw-r--r--  2.0 unx     2254 b- defN 22-Nov-12 09:37 databend_py/util/helper.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-23 13:43 databend_py-0.3.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     3462 b- defN 23-Mar-23 13:43 databend_py-0.3.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-23 13:43 databend_py-0.3.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Mar-23 13:43 databend_py-0.3.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1359 b- defN 23-Mar-23 13:43 databend_py-0.3.9.dist-info/RECORD
-17 files, 40754 bytes uncompressed, 14030 bytes compressed:  65.6%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3537 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1360 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/RECORD
+17 files, 42376 bytes uncompressed, 14425 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: databend_py/util/escape.py
 Comment: 
 
 Filename: databend_py/util/helper.py
 Comment: 
 
-Filename: databend_py-0.3.9.dist-info/LICENSE
+Filename: databend_py-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: databend_py-0.3.9.dist-info/METADATA
+Filename: databend_py-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: databend_py-0.3.9.dist-info/WHEEL
+Filename: databend_py-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: databend_py-0.3.9.dist-info/top_level.txt
+Filename: databend_py-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: databend_py-0.3.9.dist-info/RECORD
+Filename: databend_py-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databend_py/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .client import Client
 from .connection import Connection
 from .datetypes import DatabendDataType
 
-VERSION = (0, 3, 9)
+VERSION = (0, 4, 0)
 __version__ = '.'.join(str(x) for x in VERSION)
 
 __all__ = ['Client', 'Connection', 'DatabendDataType']
```

## databend_py/client.py

```diff
@@ -43,25 +43,25 @@
         raw_data = json.loads(resp.content)
         helper = self.helper()
         helper.response = raw_data
         helper.check_error()
         return raw_data
 
     def receive_result(self, query, query_id=None, with_column_types=False):
-        raw_data = self.connection.query(query, None)
+        raw_data = self.connection.query(query)
         helper = self.helper()
         helper.response = raw_data
         helper.check_error()
         gen = self.data_generator(raw_data)
         result = self.query_result_cls(
             gen, raw_data, with_column_types=with_column_types)
         return result.get_result()
 
     def iter_receive_result(self, query, query_id=None, with_column_types=False):
-        raw_data = self.connection.query(query, None)
+        raw_data = self.connection.query(query)
         helper = self.helper()
         helper.response = raw_data
         helper.check_error()
         gen = self.data_generator(raw_data)
         result = self.query_result_cls(
             gen, raw_data, with_column_types=with_column_types)
         _, rows = result.get_result()
@@ -164,15 +164,15 @@
     @classmethod
     def from_url(cls, url):
         """
         Return a client configured from the given URL.
 
         For example::
 
-            http://[user:password]@localhost:8000/default
+            https://[user:password]@localhost:8000/default?secure=True
             http://[user:password]@localhost:8000/default
             databend://[user:password]@localhost:8000/default
 
         Any additional querystring arguments will be passed along to
         the Connection class's initializer.
         """
         parsed_url = urlparse(url)
@@ -191,18 +191,21 @@
 
             value = value[0]
 
             if name == 'client_name':
                 kwargs[name] = value
             elif name == 'secure':
                 kwargs[name] = asbool(value)
+            elif name == 'copy_purge':
+                kwargs[name] = asbool(value)
+                settings[name] = asbool(value)
             elif name in timeouts:
                 kwargs[name] = float(value)
             else:
-                settings[name] = value
+                settings[name] = value  # settings={'copy_purge':False}
         secure = kwargs.get("secure", False)
         kwargs['secure'] = secure
 
         host = parsed_url.hostname
 
         if parsed_url.port is not None:
             kwargs['port'] = parsed_url.port
@@ -242,10 +245,39 @@
         resp = requests.put(presigned_url, headers=headers, data=data)
         resp.raise_for_status()
         return stage_path
 
     def sync_csv_file_into_table(self, filename, data, table):
         start = time.time()
         stage_path = self.stage_csv_file(filename, data)
-        _, _ = self.execute("COPY INTO %s FROM %s FILE_FORMAT = (type = CSV)" % (table, stage_path))
+        copy_options = self.generate_copy_options()
+        print(copy_options)
+        _, _ = self.execute(
+            f"COPY INTO {table} FROM {stage_path} FILE_FORMAT = (type = CSV)\
+             PURGE = {copy_options['PURGE']} FORCE = {copy_options['FORCE']}\
+              SIZE_LIMIT={copy_options['SIZE_LIMIT']} ON_ERROR = {copy_options['ON_ERROR']}")
         print("sync %s duration:%ss" % (filename, int(time.time() - start)))
         os.remove(filename)
+
+    def generate_copy_options(self):
+        # copy options docs: https://databend.rs/doc/sql-commands/dml/dml-copy-into-table#copyoptions
+        copy_options = {}
+        if "copy_purge" in self.settings:
+            copy_options["PURGE"] = self.settings["copy_purge"]
+        else:
+            copy_options["PURGE"] = False
+
+        if "force" in self.settings:
+            copy_options["FORCE"] = self.settings["force"]
+        else:
+            copy_options["FORCE"] = False
+
+        if "size_limit" in self.settings:
+            copy_options["SIZE_LIMIT"] = self.settings["size_limit"]
+        else:
+            copy_options["SIZE_LIMIT"] = 0
+        if "on_error" in self.settings:
+            copy_options["ON_ERROR"] = self.settings["on_error"]
+
+        else:
+            copy_options["ON_ERROR"] = "abort"
+        return copy_options
```

## databend_py/connection.py

```diff
@@ -63,23 +63,24 @@
     # {
     #   'user': 'root',
     #   'host': '127.0.0.1',
     #   'port': 3307,
     #   'database': 'default'
     # }
     def __init__(self, host, port=None, user=defines.DEFAULT_USER, password=defines.DEFAULT_PASSWORD,
-                 database=defines.DEFAULT_DATABASE, secure=False, ):
+                 database=defines.DEFAULT_DATABASE, secure=False, copy_purge=False, session_settings=None):
         self.host = host
         self.port = port
         self.user = user
         self.password = password
         self.database = database
         self.secure = secure
+        self.copy_purge = copy_purge
         self.session_max_idle_time = defines.DEFAULT_SESSION_IDLE_TIME
-        self.session = {}
+        self.client_session = session_settings
         self.additional_headers = dict()
         self.query_option = None
         self.context = Context()
         self.schema = 'http'
         if self.secure:
             self.schema = 'https'
         e = environs.Env()
@@ -98,74 +99,75 @@
         else:
             return {**headers, **self.additional_headers}
 
     def get_description(self):
         return '{}:{}'.format(self.host, self.port)
 
     def disconnect(self):
-        self.session = {}
+        self.client_session = dict()
 
-    def query(self, statement, session):
+    def query(self, statement):
         url = self.format_url()
         log.logger.debug(f"http sql: {statement}")
         query_sql = {'sql': statement, "string_fields": True}
-        if session is not None:
-            query_sql['session'] = session
+        if self.client_session is not None and len(self.client_session) != 0:
+            query_sql['session'] = self.client_session
         else:
-            session = {"database": self.database}
-            query_sql['session'] = session
+            self.client_session = {"db": self.database}
+            query_sql['session'] = self.client_session
         log.logger.debug(f"http headers {self.make_headers()}")
         response = requests.post(url,
                                  data=json.dumps(query_sql),
                                  headers=self.make_headers(),
                                  auth=HTTPBasicAuth(self.user, self.password),
                                  verify=True)
-
         try:
-            return json.loads(response.content)
+            resp_dict = json.loads(response.content)
+            self.client_session = resp_dict["session"]
+            return resp_dict
         except Exception as err:
             log.logger.error(
                 f"http error on {url}, SQL: {statement} content: {response.content} error msg:{str(err)}"
             )
             raise
 
     def format_url(self):
         if self.schema == "https" and self.port is None:
             self.port = 443
         elif self.schema == "http" and self.port is None:
             self.port = 80
         return f"{self.schema}://{self.host}:{self.port}/v1/query/"
 
     def reset_session(self):
-        self.session = {}
+        self.client_session = dict()
 
     def next_page(self, next_uri):
         url = "{}://{}:{}{}".format(self.schema, self.host, self.port, next_uri)
         return requests.get(url=url, headers=self.make_headers())
 
     # return a list of response util empty next_uri
     def query_with_session(self, statement):
-        current_session = self.session
+        current_session = self.client_session
         response_list = list()
-        response = self.query(statement, current_session)
+        response = self.query(statement)
         log.logger.debug(f"response content: {response}")
         response_list.append(response)
         start_time = time.time()
         time_limit = 12
         session = response['session']
         if session:
-            self.session = session
+            self.client_session = session
         while response['next_uri'] is not None:
             resp = self.next_page(response['next_uri'])
             response = json.loads(resp.content)
             log.logger.debug(f"Sql in progress, fetch next_uri content: {response}")
             self.check_error(response)
             session = response['session']
             if session:
-                self.session = session
+                self.client_session = session
             response_list.append(response)
             if time.time() - start_time > time_limit:
                 log.logger.warning(
                     f"after waited for {time_limit} secs, query still not finished (next uri not none)!"
                 )
         return response_list
```

## Comparing `databend_py-0.3.9.dist-info/LICENSE` & `databend_py-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `databend_py-0.3.9.dist-info/METADATA` & `databend_py-0.4.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.3.9
+Version: 0.4.0
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Classifier: Development Status :: 4 - Beta
@@ -34,19 +34,19 @@
 Requires-Dist: environs
 Requires-Dist: requests
 
 # databend-py
 
 Databend Cloud Python Driver with native http interface support
 
-[![image](https://img.shields.io/pypi/v/databend-py.svg)](https://pypi.org/project/databend-driver)
+[![image](https://img.shields.io/pypi/v/databend-py.svg)](https://pypi.org/project/databend-py)
 
 [![image](https://coveralls.io/repos/github/databendcloud/databend-py/badge.svg?branch=master)](https://coveralls.io/github/databendcloud/databend-py?branch=master)
 
-[![image](https://img.shields.io/pypi/l/databend-driver.svg)](https://pypi.org/project/databend-py)
+[![image](https://img.shields.io/pypi/l/databend-py.svg)](https://pypi.org/project/databend-py)
 
 [![image](https://img.shields.io/pypi/pyversions/databend-py.svg)](https://pypi.org/project/databend-py)
 
 # Installation
 
 pip install databend-py
 
@@ -58,26 +58,27 @@
 > >>> from databend_py import Client
 > >>> client = Client(
 >     host='tenant--warehouse.ch.datafusecloud.com',
 >     database="default",
 >     user="user",
 >     port="443",
 >     password="password")
+>     settings={"copy_purge":True,"force":True}
 > >>> print(client.execute("SELECT 1"))
 > ```
 
 The [host]{.title-ref}, [user]{.title-ref}, [password]{.title-ref} info
 will be found in databend cloud warehouse connect page as flows:
 
 Pure Client example:
 
 > ``` python
-> >>> from databend_pyimport Client
+> >>> from databend_py import Client
 > >>>
-> >>> client = Client('http://root:rootlocalhost:8081/db')
+> >>> client = Client.from_url('http://root@localhost:8000/db?secure=False&copy_purge=True')
 > >>>
 > >>> client.execute('SHOW TABLES')
 > [('test',)]
 > >>> client.execute('DROP TABLE IF EXISTS test')
 > []
 > >>> client.execute('CREATE TABLE test (x Int32)')
 > []
```

## Comparing `databend_py-0.3.9.dist-info/RECORD` & `databend_py-0.4.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-databend_py/__init__.py,sha256=hDT5yQhn2ybawGnf5xmmUcuilDX6cHTA1OQvSLEZCDY,227
-databend_py/client.py,sha256=5OjHD5ngNzJWGBKPTuzQl9dxkGShBM9decMetv2dOOg,9557
-databend_py/connection.py,sha256=Xy1QBNNe0BRZu_IeLHkBwy8JIVTVPTb-XYw-ZqHblYk,6043
+databend_py/__init__.py,sha256=bR_AXJjyGNK71Ai0KSngKhxaRj8SRFSR9C2nXnEfM4M,227
+databend_py/client.py,sha256=xPD1186k53Pz8sJ5B0P5Bjp9SylzEXxXrRVuuXQqIlw,10825
+databend_py/connection.py,sha256=9s_aY-5Ki4o1LhbTlh38ujscDDeLG8ZORyPlBr-kNgg,6321
 databend_py/context.py,sha256=yPkJ_BN4LGODvKCOjNlDGqABwxAMQTQl7w1vIGRPBDg,909
 databend_py/datetypes.py,sha256=Yl5ZS_C5oPfyOcE2xTQNtxgPZnxnMKIc_lYSmEnFJdg,931
 databend_py/defines.py,sha256=eQOK22KSKfcBukcD4oHsmlgpXFms92ew0ORxWNnxxH0,184
 databend_py/errors.py,sha256=CJE2LDMAUqnrGT1AOd5pfLKCDgiaKKiWU7FMtN-xs88,581
 databend_py/log.py,sha256=dMuMaWptI_nexWDZMtZaAnoEOluIfYWNdoR9OSAhgKM,206
 databend_py/result.py,sha256=Ru1FwwMtbbT5E2Iesv9d6fGZeL8pFJ0lG0vA3bLN3m8,2128
 databend_py/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databend_py/util/escape.py,sha256=DE7PaShERoOw285fkg3pu7T_oMU4_2dMkHbjXEqPcn4,1452
 databend_py/util/helper.py,sha256=0r1d3CeNtMLdTPN_v8yW-GjjpjHVneIJJKKGdTioOoE,2254
-databend_py-0.3.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-databend_py-0.3.9.dist-info/METADATA,sha256=7x4pTarPeb8eC49WywO02aHmaxtUbY-yIqq0jjfiDAs,3462
-databend_py-0.3.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-databend_py-0.3.9.dist-info/top_level.txt,sha256=t0rUVwHfEpXcuMreSkL69rc5DWv6FmzB4AfEGcc4_7U,12
-databend_py-0.3.9.dist-info/RECORD,,
+databend_py-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+databend_py-0.4.0.dist-info/METADATA,sha256=e-qkck-eXtdTMBA9_nRcSYisbZRf4ASTH5Gzr8ne8as,3537
+databend_py-0.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+databend_py-0.4.0.dist-info/top_level.txt,sha256=t0rUVwHfEpXcuMreSkL69rc5DWv6FmzB4AfEGcc4_7U,12
+databend_py-0.4.0.dist-info/RECORD,,
```

