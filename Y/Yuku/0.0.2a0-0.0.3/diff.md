# Comparing `tmp/Yuku-0.0.2a0.tar.gz` & `tmp/Yuku-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Yuku-0.0.2a0.tar", last modified: Wed Feb 15 23:24:15 2023, max compression
+gzip compressed data, was "Yuku-0.0.3.tar", last modified: Tue May  9 22:49:27 2023, max compression
```

## Comparing `Yuku-0.0.2a0.tar` & `Yuku-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:24:15.835852 Yuku-0.0.2a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-02-15 23:24:02.000000 Yuku-0.0.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-15 23:24:02.000000 Yuku-0.0.2a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-02-15 23:24:15.835852 Yuku-0.0.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-02-15 23:24:02.000000 Yuku-0.0.2a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:24:15.835852 Yuku-0.0.2a0/Yuku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-02-15 23:24:15.000000 Yuku-0.0.2a0/Yuku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-15 23:24:15.000000 Yuku-0.0.2a0/Yuku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 23:24:15.000000 Yuku-0.0.2a0/Yuku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-15 23:24:15.000000 Yuku-0.0.2a0/Yuku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-15 23:24:15.000000 Yuku-0.0.2a0/Yuku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:24:15.835852 Yuku-0.0.2a0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-02-15 23:24:02.000000 Yuku-0.0.2a0/bin/yuku_run
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 23:24:15.835852 Yuku-0.0.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-02-15 23:24:02.000000 Yuku-0.0.2a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:24:15.835852 Yuku-0.0.2a0/yuku/
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-02-15 23:24:02.000000 Yuku-0.0.2a0/yuku/Yuku.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 23:24:02.000000 Yuku-0.0.2a0/yuku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-15 23:24:02.000000 Yuku-0.0.2a0/yuku/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:27.717598 Yuku-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-09 22:49:14.000000 Yuku-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 22:49:14.000000 Yuku-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-09 22:49:27.717598 Yuku-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-09 22:49:14.000000 Yuku-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:27.713598 Yuku-0.0.3/Yuku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-09 22:49:27.000000 Yuku-0.0.3/Yuku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 22:49:27.000000 Yuku-0.0.3/Yuku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:49:27.000000 Yuku-0.0.3/Yuku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 22:49:27.000000 Yuku-0.0.3/Yuku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 22:49:27.000000 Yuku-0.0.3/Yuku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:27.713598 Yuku-0.0.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-09 22:49:14.000000 Yuku-0.0.3/bin/yuku_run
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:49:27.717598 Yuku-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-09 22:49:14.000000 Yuku-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:27.713598 Yuku-0.0.3/yuku/
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-05-09 22:49:14.000000 Yuku-0.0.3/yuku/Yuku.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:14.000000 Yuku-0.0.3/yuku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 22:49:14.000000 Yuku-0.0.3/yuku/_version.py
```

### Comparing `Yuku-0.0.2a0/LICENSE` & `Yuku-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Yuku-0.0.2a0/PKG-INFO` & `Yuku-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: Yuku
-Version: 0.0.2a0
-Summary: Scienti Open Data
-Home-page: https://github.com/colav/Yuku
-Author: Colav
-Author-email: colav@udea.edu.co
-License: BSD
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <center><img src="https://raw.githubusercontent.com/colav/colav.github.io/master/img/Logo.png"/></center>
 
 # Yuku
 Scienti Open Data / Yuku, god of rain in Yaqui mythology in northern Mexico.
 
 
 # Description
@@ -195,23 +184,29 @@
 
 By default the data is saved in the database **yuku** with the next collections:
 ```
 yuku> show collections
 cvlac_data
 cvlac_dataset_info
 cvlac_stage
+cvlac_stage_empty
+cvlac_stage_private
+cvlac_stage_raw
 gruplac_groups_data
 gruplac_groups_dataset_info
 gruplac_production_data
 gruplac_production_dataset_info
 ```
 
 * cvlav_data: is the dataset for cvlac, downloaded from socrata (www.datos.gov.co)
 * cvlac_dataset_info: information about the dataset, this explains the fields and provide metadata about the cvlac dataset.
 * cvlac_stage: this is the collection for the scrapped data from cvlac (minciencias web site).
+* cvlac_stage_empty: Empty pages, not possible to do any scrapping
+* cvlac_stage_private: private profiles but still some basic information
+* cvlac_stage_raw: raw html text
 * gruplac_groups_data: is the dataset for gruplac groups, downloaded from socrata (www.datos.gov.co)
 * gruplac_groups_dataset_info: information about the dataset, this explains the fields and provide metadata about the gruplac groups dataset.
 * gruplac_production_data: is the dataset for gruplac production, downloaded from socrata (www.datos.gov.co)
 * gruplac_production_dataset_info: information about the dataset, this explains the fields and provide metadata about the gruplac production dataset.
 
 # License
 BSD-3-Clause License
```

### Comparing `Yuku-0.0.2a0/README.md` & `Yuku-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: Yuku
+Version: 0.0.3
+Summary: Scienti Open Data
+Home-page: https://github.com/colav/Yuku
+Author: Colav
+Author-email: colav@udea.edu.co
+License: BSD
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <center><img src="https://raw.githubusercontent.com/colav/colav.github.io/master/img/Logo.png"/></center>
 
 # Yuku
 Scienti Open Data / Yuku, god of rain in Yaqui mythology in northern Mexico.
 
 
 # Description
@@ -184,23 +195,29 @@
 
 By default the data is saved in the database **yuku** with the next collections:
 ```
 yuku> show collections
 cvlac_data
 cvlac_dataset_info
 cvlac_stage
+cvlac_stage_empty
+cvlac_stage_private
+cvlac_stage_raw
 gruplac_groups_data
 gruplac_groups_dataset_info
 gruplac_production_data
 gruplac_production_dataset_info
 ```
 
 * cvlav_data: is the dataset for cvlac, downloaded from socrata (www.datos.gov.co)
 * cvlac_dataset_info: information about the dataset, this explains the fields and provide metadata about the cvlac dataset.
 * cvlac_stage: this is the collection for the scrapped data from cvlac (minciencias web site).
+* cvlac_stage_empty: Empty pages, not possible to do any scrapping
+* cvlac_stage_private: private profiles but still some basic information
+* cvlac_stage_raw: raw html text
 * gruplac_groups_data: is the dataset for gruplac groups, downloaded from socrata (www.datos.gov.co)
 * gruplac_groups_dataset_info: information about the dataset, this explains the fields and provide metadata about the gruplac groups dataset.
 * gruplac_production_data: is the dataset for gruplac production, downloaded from socrata (www.datos.gov.co)
 * gruplac_production_dataset_info: information about the dataset, this explains the fields and provide metadata about the gruplac production dataset.
 
 # License
 BSD-3-Clause License
```

### Comparing `Yuku-0.0.2a0/Yuku.egg-info/PKG-INFO` & `Yuku-0.0.3/Yuku.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Yuku
-Version: 0.0.2a0
+Version: 0.0.3
 Summary: Scienti Open Data
 Home-page: https://github.com/colav/Yuku
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -195,23 +195,29 @@
 
 By default the data is saved in the database **yuku** with the next collections:
 ```
 yuku> show collections
 cvlac_data
 cvlac_dataset_info
 cvlac_stage
+cvlac_stage_empty
+cvlac_stage_private
+cvlac_stage_raw
 gruplac_groups_data
 gruplac_groups_dataset_info
 gruplac_production_data
 gruplac_production_dataset_info
 ```
 
 * cvlav_data: is the dataset for cvlac, downloaded from socrata (www.datos.gov.co)
 * cvlac_dataset_info: information about the dataset, this explains the fields and provide metadata about the cvlac dataset.
 * cvlac_stage: this is the collection for the scrapped data from cvlac (minciencias web site).
+* cvlac_stage_empty: Empty pages, not possible to do any scrapping
+* cvlac_stage_private: private profiles but still some basic information
+* cvlac_stage_raw: raw html text
 * gruplac_groups_data: is the dataset for gruplac groups, downloaded from socrata (www.datos.gov.co)
 * gruplac_groups_dataset_info: information about the dataset, this explains the fields and provide metadata about the gruplac groups dataset.
 * gruplac_production_data: is the dataset for gruplac production, downloaded from socrata (www.datos.gov.co)
 * gruplac_production_dataset_info: information about the dataset, this explains the fields and provide metadata about the gruplac production dataset.
 
 # License
 BSD-3-Clause License
```

### Comparing `Yuku-0.0.2a0/bin/yuku_run` & `Yuku-0.0.3/bin/yuku_run`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 from yuku.Yuku import Yuku
-
+from pymongo import MongoClient
 import argparse
 import faulthandler
 faulthandler.enable()
 
 parser = argparse.ArgumentParser(description='Yuku Scienti')
 parser.add_argument('--mongo_dburi', type=str,
                     default='mongodb://localhost:27017/', help='uri for MongoDb database')
@@ -31,14 +31,17 @@
 parser.add_argument('--download_collection', type=str,
                     help='Collection name to --download')
 
 if __name__ == '__main__':
     args = parser.parse_args()
     yuku = Yuku(args.mongo_dbname, args.mongo_dburi,
                 args.socrata_endpoint)
+    
+    if args.drop_mongodb:
+        MongoClient(args.mongo_dburi).drop_database(args.mongo_dbname)
     if args.search is not None:
         yuku.search(args.search, args.search_limit)
 
     if args.download_cvlac is not None:
         yuku.download_cvlac(args.download_cvlac)
 
     if args.download_gruplac_production is not None:
```

### Comparing `Yuku-0.0.2a0/setup.py` & `Yuku-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
         # Dependent packages (distributions)
         install_requires=[
             'pymongo>=3.10.1',
             'pandas',
             'requests>=2.22.0',
             'sodapy',
-            'beautifulsoup4'
+            'beautifulsoup4',
+            'lxml'
         ],
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `Yuku-0.0.2a0/yuku/Yuku.py` & `Yuku-0.0.3/yuku/Yuku.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 import pandas as pd
 from pymongo import MongoClient
 from sodapy import Socrata
 from bs4 import BeautifulSoup
 import time
 import urllib3
+import sys
 
 
 class Yuku:
     def __init__(self, mongo_db: str = "yuku", mongodb_uri: str = "mongodb://localhost:27017/", socrata_endpoint: str = "www.datos.gov.co"):
         """
         Contructor for Yuku, we only support open datasets, credentials are not supported.
 
@@ -45,91 +46,113 @@
             print("WARNING: cvlac_data already in the database, it wont be downloaded again, drop the database if you want start over.")
         else:
             data = self.client.get_all(dataset_id)
             data = list(data)
             self.db["cvlac_data"].insert_many(data)
         cod_rh_data = self.db["cvlac_data"].distinct("id_persona_pr")
         cod_rh_stage = self.db["cvlac_stage"].distinct("id_persona_pr")
+        cod_rh_stage_priv = self.db["cvlac_stage_private"].distinct(
+            "id_persona_pr")
+        cod_rh_stage_empty = self.db["cvlac_stage_empty"].distinct(
+            "id_persona_pr")
+
         # computing the remaining ids for scrapping
-        cod_rh = set(cod_rh_data) - set(cod_rh_stage)
+        cod_rh = set(cod_rh_data) - set(cod_rh_stage) - \
+            set(cod_rh_stage_priv) - set(cod_rh_stage_empty)
         cod_rh = list(cod_rh)
         print(f"INFO: found {len(cod_rh_data)} records in data\n      found {len(cod_rh_stage)} in stage\n      found {len(cod_rh)} remain records to download.")
 
         counter = 0
         count = len(cod_rh)
         for cvlac in cod_rh:
             if counter % 10 == 0:
                 print(f"INFO: Downloaded {counter} of {count}")
             url = f'{scienti_url}{cvlac}'
 
-            dd = {'id_persona_pr': cvlac}
-
             try:
                 r = requests.get(url, verify=False)
             except Exception:
                 continue
 
             if not r.text:
                 continue
 
             soup = BeautifulSoup(r.text, 'lxml')  # Parse the HTML as a string
-            tables = soup.find_all('table')
 
-            # 1: Full names
-            if len(tables) > 2:
-                t = tables[1]
-            else:
-                dd['nombre'] = ''
-                continue
+            reg = {'id_persona_pr': cvlac, "url": url}
+            try:
+                # Datos Generales
+                a_tag = soup.find('a', {'name': 'datos_generales'})
+                table_tag = a_tag.find_next('table')
+
+                if table_tag is None:
+                    print(
+                        f"WARNING: found empty id {cvlac}  with url = {url} ")
+                    self.db["cvlac_stage_empty"].insert_one(reg)
+                    continue
 
-            tr = pd.read_html(t.decode())[0].to_dict(orient='records')
+                record = pd.read_html(table_tag.decode())[
+                    0].to_dict(orient='records')
+            except Exception as e:
+                print(f"Error processing id {cvlac}  with url = {url} ")
+                print(e, file=sys.stderr)
+                continue
 
-            for d in tr:
+            for d in record:
                 if d and isinstance(d.get(0), str) and isinstance(d.get(1), str):
-                    dd[d.get(0)] = d.get(1).replace('\xa0', ' ')
+                    reg[d.get(0)] = d.get(1).replace('\xa0', ' ')
                 else:
                     continue
-
-            # 2. Academic Social Networks  and authors Ids
-            t = tables[2]
-
-            # 2.a) Academic Social Networks (Google Scholar)
-            next = 2
             try:
-                ids = t.find_all('h3')[0].text
-            except Exception:
-                ids = ''
-            if ids == 'Redes sociales académicas':
-                next = 3
-                ll = t.find_all('a')
-                for x in ll:
-                    try:
-                        dd[x.text.split(' (')[0]] = x['href']
-                    except Exception:
-                        continue
-            # 2.b) authors Ids (ORCID, Scopus, ...)
-            try:
-                t = tables[next]
-            except Exception:
-                continue
+                # Redes
+                a_tag = soup.find('a', {'name': 'redes_identificadoes'})
+                if a_tag is None:
+                    print(
+                        f"WARNING: found private id {cvlac}  with url = {url} ")
+                    self.db["cvlac_stage_private"].insert_one(reg)
+                    self.db["cvlac_stage_raw"].insert_one(
+                        {"_id": cvlac, "html": r.text})
+                    time.sleep(0.3)
+                    counter += 1
+                    continue
 
-            try:
-                ids = t.find_all('h3')[0].text
-            except Exception:
-                ids = ''
-            if ids == 'Identificadores de autor':
-                ll = t.find_all('a')
-                for x in ll:
+                table_tag = a_tag.find_next('table')
+                record = table_tag.find_all('a')
+                for link in record:
+                    reg[link.text] = link['href']
+
+                # Identificadores
+                a_tag = soup.find('a', {'name': 'red_identificadores'})
+                table_tag = a_tag.find_next('table')
+                record = table_tag.find_all('a')
+                for link in record:
                     try:
-                        dd[re.search('\(([\w]+)\)', x.text).groups()[0]] = x['href']  # noqa
+                        reg[re.search('\(([\w]+)\)', link.text).groups()
+                            [0]] = link['href']
                     except Exception:
+                        reg[link.text] = link['href']
                         continue
-            self.db["cvlac_stage"].insert_one(dd)
-            time.sleep(0.3)
-            counter += 1
+
+                # Formación académica
+                a_tag = soup.find('a', {'name': 'formacion_acad'})
+                table_tag = a_tag.find_next('table')
+                record = table_tag.find_all('td')
+
+                for tag in record:
+                    b_title = tag.find_all('b')
+                    if len(b_title) > 0:
+                        reg[b_title[0].text] = tag.text.split('\r\n')
+                self.db["cvlac_stage"].insert_one(reg)
+                self.db["cvlac_stage_raw"].insert_one(
+                    {"_id": cvlac, "html": r.text})
+                time.sleep(0.3)
+                counter += 1
+            except Exception as e:
+                print(f"Error processing id {cvlac}  with url = {url} ")
+                print(e, file=sys.stderr)
         print(f"INFO: Downloaded {counter} of {count}")
 
     def download_gruplac_production(self, dataset_id: str):
         """
         Method to download gruplac production information.
         Unfortunately we dont have support for checkpoint in this method.
```

