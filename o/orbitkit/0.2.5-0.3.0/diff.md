# Comparing `tmp/orbitkit-0.2.5.tar.gz` & `tmp/orbitkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.2.5.tar", last modified: Fri May  6 07:48:04 2022, max compression
+gzip compressed data, was "dist/orbitkit-0.3.0.tar", last modified: Wed May 10 06:36:25 2023, max compression
```

## Comparing `orbitkit-0.2.5.tar` & `orbitkit-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2022-05-06 07:48:04.000000 orbitkit-0.2.5/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.2.5/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.2.5/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3828 2022-05-06 07:48:04.000000 orbitkit-0.2.5/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     2207 2021-10-31 14:45:20.000000 orbitkit-0.2.5/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2022-05-06 07:47:12.000000 orbitkit-0.2.5/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      376 2022-01-24 07:50:23.000000 orbitkit-0.2.5/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit/file_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        1 2021-07-15 08:55:40.000000 orbitkit-0.2.5/orbitkit/file_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     2111 2021-10-31 14:31:58.000000 orbitkit-0.2.5/orbitkit/file_extractor/dispatcher.py
--rw-r--r--   0 crown      (501) staff       (20)      244 2021-10-31 03:25:18.000000 orbitkit-0.2.5/orbitkit/file_extractor/exception.py
--rw-r--r--   0 crown      (501) staff       (20)     1912 2021-10-31 14:48:38.000000 orbitkit-0.2.5/orbitkit/file_extractor/extractor.py
--rw-r--r--   0 crown      (501) staff       (20)      224 2021-10-31 14:31:58.000000 orbitkit-0.2.5/orbitkit/file_extractor/extractor_audio.py
--rw-r--r--   0 crown      (501) staff       (20)     1211 2021-10-31 14:31:58.000000 orbitkit-0.2.5/orbitkit/file_extractor/extractor_html.py
--rw-r--r--   0 crown      (501) staff       (20)     2034 2021-10-31 14:31:58.000000 orbitkit-0.2.5/orbitkit/file_extractor/extractor_json.py
--rw-r--r--   0 crown      (501) staff       (20)     1016 2021-10-31 14:31:58.000000 orbitkit-0.2.5/orbitkit/file_extractor/extractor_office.py
--rw-r--r--   0 crown      (501) staff       (20)     2983 2022-05-06 07:35:45.000000 orbitkit-0.2.5/orbitkit/file_extractor/extractor_pdf.py
--rw-r--r--   0 crown      (501) staff       (20)      868 2021-10-31 14:31:58.000000 orbitkit-0.2.5/orbitkit/file_extractor/extractor_txt.py
--rw-r--r--   0 crown      (501) staff       (20)      277 2021-07-27 10:13:23.000000 orbitkit-0.2.5/orbitkit/file_extractor/util.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.2.5/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     1533 2021-12-26 11:07:53.000000 orbitkit-0.2.5/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.2.5/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     5064 2022-01-05 07:16:58.000000 orbitkit-0.2.5/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)       80 2020-10-29 07:41:20.000000 orbitkit-0.2.5/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      814 2021-10-12 06:35:20.000000 orbitkit-0.2.5/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)     1466 2021-07-15 09:45:02.000000 orbitkit-0.2.5/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      173 2021-07-15 09:45:02.000000 orbitkit-0.2.5/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    19087 2021-12-26 13:51:52.000000 orbitkit-0.2.5/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3828 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)      949 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       31 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2022-05-06 07:48:04.000000 orbitkit-0.2.5/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2022-05-06 07:48:04.000000 orbitkit-0.2.5/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1450 2022-01-24 07:52:12.000000 orbitkit-0.2.5/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-10 06:36:25.000000 orbitkit-0.3.0/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.3.0/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.3.0/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3828 2023-05-10 06:36:25.000000 orbitkit-0.3.0/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     2207 2021-10-31 14:45:20.000000 orbitkit-0.3.0/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2023-05-10 05:36:50.000000 orbitkit-0.3.0/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      376 2022-01-24 07:50:23.000000 orbitkit-0.3.0/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit/file_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        1 2021-07-15 08:55:40.000000 orbitkit-0.3.0/orbitkit/file_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     2111 2021-10-31 14:31:58.000000 orbitkit-0.3.0/orbitkit/file_extractor/dispatcher.py
+-rw-r--r--   0 crown      (501) staff       (20)      244 2021-10-31 03:25:18.000000 orbitkit-0.3.0/orbitkit/file_extractor/exception.py
+-rw-r--r--   0 crown      (501) staff       (20)     1912 2021-10-31 14:48:38.000000 orbitkit-0.3.0/orbitkit/file_extractor/extractor.py
+-rw-r--r--   0 crown      (501) staff       (20)      224 2021-10-31 14:31:58.000000 orbitkit-0.3.0/orbitkit/file_extractor/extractor_audio.py
+-rw-r--r--   0 crown      (501) staff       (20)     1211 2021-10-31 14:31:58.000000 orbitkit-0.3.0/orbitkit/file_extractor/extractor_html.py
+-rw-r--r--   0 crown      (501) staff       (20)     2034 2021-10-31 14:31:58.000000 orbitkit-0.3.0/orbitkit/file_extractor/extractor_json.py
+-rw-r--r--   0 crown      (501) staff       (20)     1016 2021-10-31 14:31:58.000000 orbitkit-0.3.0/orbitkit/file_extractor/extractor_office.py
+-rw-r--r--   0 crown      (501) staff       (20)     2983 2022-05-06 07:35:45.000000 orbitkit-0.3.0/orbitkit/file_extractor/extractor_pdf.py
+-rw-r--r--   0 crown      (501) staff       (20)      868 2021-10-31 14:31:58.000000 orbitkit-0.3.0/orbitkit/file_extractor/extractor_txt.py
+-rw-r--r--   0 crown      (501) staff       (20)      277 2021-07-27 10:13:23.000000 orbitkit-0.3.0/orbitkit/file_extractor/util.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.3.0/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     1533 2021-12-26 11:07:53.000000 orbitkit-0.3.0/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.3.0/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     5064 2022-01-05 07:16:58.000000 orbitkit-0.3.0/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.3.0/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.3.0/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     4888 2023-05-10 06:34:32.000000 orbitkit-0.3.0/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    11739 2023-05-10 06:34:32.000000 orbitkit-0.3.0/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      104 2023-05-10 05:26:36.000000 orbitkit-0.3.0/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      790 2023-05-10 05:20:41.000000 orbitkit-0.3.0/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      520 2023-05-10 05:26:36.000000 orbitkit-0.3.0/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     1442 2023-05-10 05:20:41.000000 orbitkit-0.3.0/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      148 2023-05-10 05:19:04.000000 orbitkit-0.3.0/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    19087 2021-12-26 13:51:52.000000 orbitkit-0.3.0/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3828 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1159 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       89 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2023-05-10 06:36:25.000000 orbitkit-0.3.0/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2023-05-10 06:36:25.000000 orbitkit-0.3.0/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1547 2023-05-10 05:35:02.000000 orbitkit-0.3.0/setup.py
```

### Comparing `orbitkit-0.2.5/LICENSE` & `orbitkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/PKG-INFO` & `orbitkit-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.2.5
+Version: 0.3.0
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.2.5/README.md` & `orbitkit-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/file_extractor/dispatcher.py` & `orbitkit-0.3.0/orbitkit/file_extractor/dispatcher.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/file_extractor/extractor.py` & `orbitkit-0.3.0/orbitkit/file_extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/file_extractor/extractor_html.py` & `orbitkit-0.3.0/orbitkit/file_extractor/extractor_html.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/file_extractor/extractor_json.py` & `orbitkit-0.3.0/orbitkit/file_extractor/extractor_json.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/file_extractor/extractor_office.py` & `orbitkit-0.3.0/orbitkit/file_extractor/extractor_office.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/file_extractor/extractor_pdf.py` & `orbitkit-0.3.0/orbitkit/file_extractor/extractor_pdf.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/file_extractor/extractor_txt.py` & `orbitkit-0.3.0/orbitkit/file_extractor/extractor_txt.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/id_srv/id_gen.py` & `orbitkit-0.3.0/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/lark_send/lark.py` & `orbitkit-0.3.0/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit/util/common.py` & `orbitkit-0.3.0/orbitkit/util/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import re
 import uuid
 
 
 def gen_ot_uuid_random():
     """
     :return:
```

### Comparing `orbitkit-0.2.5/orbitkit/util/util_date.py` & `orbitkit-0.3.0/orbitkit/util/util_date.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import datetime
 
 
 def get_date_range_list_v1(start_date, end_date):
     """
     This method will return a list in which all date range are included with the very start and ending.
     :param start_date: '2019-06-03'
```

### Comparing `orbitkit-0.2.5/orbitkit/util/util_type_mapping.py` & `orbitkit-0.3.0/orbitkit/util/util_type_mapping.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.2.5/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.3.0/orbitkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.2.5
+Version: 0.3.0
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.2.5/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.3.0/orbitkit.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,12 +21,17 @@
 orbitkit/file_extractor/extractor_pdf.py
 orbitkit/file_extractor/extractor_txt.py
 orbitkit/file_extractor/util.py
 orbitkit/id_srv/__init__.py
 orbitkit/id_srv/id_gen.py
 orbitkit/lark_send/__init__.py
 orbitkit/lark_send/lark.py
+orbitkit/pdf_extractor/__init__.py
+orbitkit/pdf_extractor/pdf_block_extractor_base.py
+orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+orbitkit/pdf_extractor/pdf_block_extractor_v2.py
 orbitkit/util/__init__.py
 orbitkit/util/common.py
+orbitkit/util/util_aws.py
 orbitkit/util/util_date.py
 orbitkit/util/util_str.py
 orbitkit/util/util_type_mapping.py
```

### Comparing `orbitkit-0.2.5/setup.py` & `orbitkit-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,9 +35,12 @@
         'Topic :: Software Development :: Libraries'
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         "boto3 >= 1.16.0",
         "requests >= 2.12.1",
+        "pdfplumber >= 0.9.0",
+        "pycryptodome >= 3.11.0",
+        "prettytable >= 3.0.0",
     ]
 )
```

