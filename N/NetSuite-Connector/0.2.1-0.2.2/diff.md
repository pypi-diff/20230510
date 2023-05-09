# Comparing `tmp/NetSuite-Connector-0.2.1.tar.gz` & `tmp/NetSuite-Connector-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetSuite-Connector-0.2.1.tar", last modified: Wed Mar 22 20:46:25 2023, max compression
+gzip compressed data, was "NetSuite-Connector-0.2.2.tar", last modified: Tue May  9 22:45:01 2023, max compression
```

## Comparing `NetSuite-Connector-0.2.1.tar` & `NetSuite-Connector-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 20:46:25.641000 NetSuite-Connector-0.2.1/
--rw-rw-rw-   0        0        0     1090 2023-03-22 19:27:04.000000 NetSuite-Connector-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3928 2023-03-22 20:46:25.632000 NetSuite-Connector-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2111 2022-10-25 21:58:40.000000 NetSuite-Connector-0.2.1/README.md
--rw-rw-rw-   0        0        0      735 2023-03-22 20:45:46.000000 NetSuite-Connector-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-22 20:46:25.639000 NetSuite-Connector-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-22 20:46:25.402000 NetSuite-Connector-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-22 20:46:25.522000 NetSuite-Connector-0.2.1/src/NetSuite_Connector/
--rw-rw-rw-   0        0        0     4004 2023-03-22 20:45:12.000000 NetSuite-Connector-0.2.1/src/NetSuite_Connector/NetSuite.py
--rw-rw-rw-   0        0        0     4154 2023-03-22 20:27:37.000000 NetSuite-Connector-0.2.1/src/NetSuite_Connector/ODBC.py
--rw-rw-rw-   0        0        0        0 2022-10-25 21:58:40.000000 NetSuite-Connector-0.2.1/src/NetSuite_Connector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 20:46:25.599000 NetSuite-Connector-0.2.1/src/NetSuite_Connector.egg-info/
--rw-rw-rw-   0        0        0     3928 2023-03-22 20:46:25.000000 NetSuite-Connector-0.2.1/src/NetSuite_Connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-03-22 20:46:25.000000 NetSuite-Connector-0.2.1/src/NetSuite_Connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 20:46:25.000000 NetSuite-Connector-0.2.1/src/NetSuite_Connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-03-22 20:46:25.000000 NetSuite-Connector-0.2.1/src/NetSuite_Connector.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 20:46:25.618000 NetSuite-Connector-0.2.1/tests/
--rw-rw-rw-   0        0        0      345 2022-10-25 22:40:03.000000 NetSuite-Connector-0.2.1/tests/test_odbc.py
+drwxrwxrwx   0        0        0        0 2023-05-09 22:45:00.965000 NetSuite-Connector-0.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-03-22 19:27:04.000000 NetSuite-Connector-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4284 2023-05-09 22:45:00.911000 NetSuite-Connector-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2467 2023-03-22 21:11:08.000000 NetSuite-Connector-0.2.2/README.md
+-rw-rw-rw-   0        0        0      735 2023-05-09 22:42:04.000000 NetSuite-Connector-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 22:45:00.953000 NetSuite-Connector-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 22:44:58.483000 NetSuite-Connector-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 22:44:59.736000 NetSuite-Connector-0.2.2/src/NetSuite_Connector/
+-rw-rw-rw-   0        0        0     4004 2023-03-22 21:05:45.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector/NetSuite.py
+-rw-rw-rw-   0        0        0     4154 2023-03-22 20:27:37.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector/ODBC.py
+-rw-rw-rw-   0        0        0        0 2022-10-25 21:58:40.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 22:45:00.562000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/
+-rw-rw-rw-   0        0        0     4284 2023-05-09 22:44:57.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-05-09 22:44:58.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 22:44:57.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-09 22:44:57.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 22:45:00.771000 NetSuite-Connector-0.2.2/tests/
+-rw-rw-rw-   0        0        0      345 2022-10-25 22:40:03.000000 NetSuite-Connector-0.2.2/tests/test_odbc.py
```

### Comparing `NetSuite-Connector-0.2.1/LICENSE` & `NetSuite-Connector-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NetSuite-Connector-0.2.1/PKG-INFO` & `NetSuite-Connector-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetSuite-Connector
-Version: 0.2.1
+Version: 0.2.2
 Summary: NetSuite Connector
 Author-email: Marcos Lopez <merick16@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Marcos Lopez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,34 +54,34 @@
 )
 
 x = nt.get(
     url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
     headers={"Content-Type": "application/json"},
     params={}
 )
-print(x.__dict__)
-# Response <200>
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
 ```
-### RESTlet PUT - POST
+### RESTlet PUT - POST - DELETE
 ```python
 from NetSuite_Connector.NetSuite import NetSuite
 nt = NetSuite(
     account_id=123456,
     consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
     token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
 )
 body={"foo":"bar"}
 x = nt.post(
     url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
     headers={"Content-Type": "application/json"},
     params={},
     body=body
 )
-print(x.__dict__)
-# Response <200>
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
 ```
 # ODBC Queries
 
 Connector only supports ODBC Driver queries, JDBC is not supported
 ## Get Started
 
 Before you begin install [ODBC Driver](https://system.netsuite.com/app/help/helpcenter.nl?fid=book_N748613.html).
@@ -97,15 +97,14 @@
     account_id="*****",
     user_email="*****",
     role_id="*****",
     dsn="*****",
     password="*****"
 )
 q = nt.query("SELECT * FROM OA_tables")
-# <NetSuite_Connector.NetsuiteObject>
 print(q.status)
 # 200
 print(q.response)
 #[{"foo":"bar"}]
 print(q.data_received)
 # SELECT * FROM OA_tables
 print(q.columns)
```

### Comparing `NetSuite-Connector-0.2.1/README.md` & `NetSuite-Connector-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 )
 
 x = nt.get(
     url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
     headers={"Content-Type": "application/json"},
     params={}
 )
-print(x.__dict__)
-# Response <200>
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
 ```
-### RESTlet PUT - POST
+### RESTlet PUT - POST - DELETE
 ```python
 from NetSuite_Connector.NetSuite import NetSuite
 nt = NetSuite(
     account_id=123456,
     consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
     token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
 )
 body={"foo":"bar"}
 x = nt.post(
     url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
     headers={"Content-Type": "application/json"},
     params={},
     body=body
 )
-print(x.__dict__)
-# Response <200>
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
 ```
 # ODBC Queries
 
 Connector only supports ODBC Driver queries, JDBC is not supported
 ## Get Started
 
 Before you begin install [ODBC Driver](https://system.netsuite.com/app/help/helpcenter.nl?fid=book_N748613.html).
@@ -61,15 +61,14 @@
     account_id="*****",
     user_email="*****",
     role_id="*****",
     dsn="*****",
     password="*****"
 )
 q = nt.query("SELECT * FROM OA_tables")
-# <NetSuite_Connector.NetsuiteObject>
 print(q.status)
 # 200
 print(q.response)
 #[{"foo":"bar"}]
 print(q.data_received)
 # SELECT * FROM OA_tables
 print(q.columns)
```

### Comparing `NetSuite-Connector-0.2.1/pyproject.toml` & `NetSuite-Connector-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests==2.27.1","requests-oauthlib==1.3.1","pyodbc>=4.0.34","pandas>=1.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NetSuite-Connector"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Marcos Lopez", email="merick16@gmail.com" },
 ]
 description = "NetSuite Connector"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `NetSuite-Connector-0.2.1/src/NetSuite_Connector/NetSuite.py` & `NetSuite-Connector-0.2.2/src/NetSuite_Connector/NetSuite.py`

 * *Files identical despite different names*

### Comparing `NetSuite-Connector-0.2.1/src/NetSuite_Connector/ODBC.py` & `NetSuite-Connector-0.2.2/src/NetSuite_Connector/ODBC.py`

 * *Files identical despite different names*

### Comparing `NetSuite-Connector-0.2.1/src/NetSuite_Connector.egg-info/PKG-INFO` & `NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetSuite-Connector
-Version: 0.2.1
+Version: 0.2.2
 Summary: NetSuite Connector
 Author-email: Marcos Lopez <merick16@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Marcos Lopez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,34 +54,34 @@
 )
 
 x = nt.get(
     url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
     headers={"Content-Type": "application/json"},
     params={}
 )
-print(x.__dict__)
-# Response <200>
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
 ```
-### RESTlet PUT - POST
+### RESTlet PUT - POST - DELETE
 ```python
 from NetSuite_Connector.NetSuite import NetSuite
 nt = NetSuite(
     account_id=123456,
     consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
     token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
 )
 body={"foo":"bar"}
 x = nt.post(
     url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
     headers={"Content-Type": "application/json"},
     params={},
     body=body
 )
-print(x.__dict__)
-# Response <200>
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
 ```
 # ODBC Queries
 
 Connector only supports ODBC Driver queries, JDBC is not supported
 ## Get Started
 
 Before you begin install [ODBC Driver](https://system.netsuite.com/app/help/helpcenter.nl?fid=book_N748613.html).
@@ -97,15 +97,14 @@
     account_id="*****",
     user_email="*****",
     role_id="*****",
     dsn="*****",
     password="*****"
 )
 q = nt.query("SELECT * FROM OA_tables")
-# <NetSuite_Connector.NetsuiteObject>
 print(q.status)
 # 200
 print(q.response)
 #[{"foo":"bar"}]
 print(q.data_received)
 # SELECT * FROM OA_tables
 print(q.columns)
```

