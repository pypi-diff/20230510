# Comparing `tmp/fpds-1.0.3.tar.gz` & `tmp/fpds-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpds-1.0.3.tar", last modified: Wed Apr 26 22:19:23 2023, max compression
+gzip compressed data, was "fpds-1.2.0.tar", last modified: Wed May 10 18:17:56 2023, max compression
```

## Comparing `fpds-1.0.3.tar` & `fpds-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.297100 fpds-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 22:18:26.000000 fpds-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 22:18:26.000000 fpds-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-04-26 22:19:23.297100 fpds-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-26 22:18:26.000000 fpds-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 22:19:23.297100 fpds-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:18:26.000000 fpds-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.285099 fpds-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.289100 fpds-1.0.3/src/fpds/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/cli/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/constants/fields.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/core/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-26 22:18:26.000000 fpds-1.0.3/src/fpds/utilities/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.293099 fpds-1.0.3/src/fpds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 22:19:23.000000 fpds-1.0.3/src/fpds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:19:23.297100 fpds-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-26 22:18:26.000000 fpds-1.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-26 22:18:26.000000 fpds-1.0.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-26 22:18:26.000000 fpds-1.0.3/tests/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.635260 fpds-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 18:16:59.000000 fpds-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 18:16:59.000000 fpds-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-10 18:17:56.635260 fpds-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-10 18:16:59.000000 fpds-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-10 18:17:56.635260 fpds-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:16:59.000000 fpds-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.631260 fpds-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.631260 fpds-1.2.0/src/fpds/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.635260 fpds-1.2.0/src/fpds/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/cli/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.635260 fpds-1.2.0/src/fpds/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/constants/fields.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.635260 fpds-1.2.0/src/fpds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/core/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/core/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/core/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.635260 fpds-1.2.0/src/fpds/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-10 18:16:59.000000 fpds-1.2.0/src/fpds/utilities/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.631260 fpds-1.2.0/src/fpds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-10 18:17:56.000000 fpds-1.2.0/src/fpds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-10 18:17:56.000000 fpds-1.2.0/src/fpds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:17:56.000000 fpds-1.2.0/src/fpds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:17:56.000000 fpds-1.2.0/src/fpds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-10 18:17:56.000000 fpds-1.2.0/src/fpds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 18:17:56.000000 fpds-1.2.0/src/fpds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:17:56.635260 fpds-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-10 18:16:59.000000 fpds-1.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-10 18:16:59.000000 fpds-1.2.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-10 18:16:59.000000 fpds-1.2.0/tests/test_xml.py
```

### Comparing `fpds-1.0.3/LICENSE` & `fpds-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fpds-1.0.3/PKG-INFO` & `fpds-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpds
-Version: 1.0.3
+Version: 1.2.0
 Summary: A parser for the Federal Procurement Data System (FPDS) Atom feed
 Author: Derek Herincx
 Author-email: derek663@gmail.com
 Keywords: fpds python atom cli
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
@@ -75,14 +75,17 @@
 request = fpdsRequest(
     LAST_MOD_DATE="[2022/01/01, 2022/05/01]",
     AGENCY_CODE="7504"
 )
 
 # Records saved as a python list
 records = request()
+
+# or equivalently, explicity call the `parse_content` method
+records = request.parse_content()
 ```
 
 For linting and formatting, we use `flake8` and `black`.
 
 ```
 $ make lint
 $ make formatters
@@ -95,28 +98,50 @@
 ```
 
 ### Testing
 ```
 $ make test
 ```
 
-
-## Additional Notes
-To ensure no data is lost during export, `fpds` will save tag attributes as
-individual data elements. For example, parsing the `contractActionType` tag
-and extracting the text value would only return `E` and omit data contained
-in the `description` and `part80orPart13` attributes.
-
-```
- <ns1:contractActionType description="BPA" part8OrPart13="PART8">E</ns1:contractActionType>
-```
-
-When parsing such elements, `fpds` will represent the tag above in the
-following manner:
-
-```
-    {
-        "contractActionType": "E",
-        "contractActionType__description": "BPA"
-        "contractActionType__part8OrPart13": "PART8"
-    }
+## What's New
+As of v1.2.0, tag names include their full XML tag hierarchy due to duplicate
+tag names being overwritten in v1.1.X. For example, the `content` XML below has the
+following duplicate tag names: `agencyID`, `PIID`, and `modNumber`.
+Based on the original hierarchy, it's clear that one set of tags represents
+the actual award info and the second, the award's referenced IDV.
+
+```
+<content xmlns:ns1="https://www.fpds.gov/FPDS" type="application/xml">
+    <ns1:awardID>
+        <ns1:awardContractID>
+            <ns1:agencyID name="ENVIRONMENTAL PROTECTION AGENCY">6800</ns1:agencyID>
+            <ns1:PIID>0002</ns1:PIID>
+            <ns1:modNumber>P00018</ns1:modNumber>
+            <ns1:transactionNumber>0</ns1:transactionNumber>
+        </ns1:awardContractID>
+        <ns1:referencedIDVID>
+            <ns1:agencyID name="ENVIRONMENTAL PROTECTION AGENCY">6800</ns1:agencyID>
+            <ns1:PIID>EPS31703</ns1:PIID>
+            <ns1:modNumber>0</ns1:modNumber>
+        </ns1:referencedIDVID>
+    </ns1:awardID>
+</content>
+```
+
+In lieu of this, the final JSON structure would represent this snippet of data
+the following (note that additional attributes like `name` in `agencyID` are
+still captured and represented by their proper hierarchy; the name of the
+attribute is appended to the end of the tag name):
+
+```
+{
+    "awardID__awardContractID__agenycID": "6800"
+    "awardID__awardContractID__agenycID__name": "ENVIRONMENTAL PROTECTION AGENCY"
+    "awardID__awardContractID__PIID": "0002"
+    "awardID__awardContractID__modNumber": "P00018"
+    "awardID__awardContractID__transactionNUmber: "0"
+    "referencedIDVID__awardContractID__agenycID": "6800"
+    "referencedIDVID__awardContractID__agenycID__name": "ENVIRONMENTAL PROTECTION AGENCY"
+    "referencedIDVID__awardContractID__PIID": "EPS31703"
+    "referencedIDVID__awardContractID__modNumber": "0"
+}
 ```
```

### Comparing `fpds-1.0.3/setup.cfg` & `fpds-1.2.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = fpds
 author = Derek Herincx
 author_email = derek663@gmail.com
-version = 1.0.3
+version = 1.2.0
 description = A parser for the Federal Procurement Data System (FPDS) Atom feed
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = fpds python atom cli
 classifiers = 
 	Intended Audience :: Developers
 	Natural Language :: English
@@ -14,17 +14,17 @@
 
 [options]
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	click==8.1.3
-	requests==2.28.1
-	tqdm==4.64.1
+	click>=8.1.3
+	requests>=2.29.0
+	tqdm>=4.65.0
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 fpds.constants = 
 	*.json
```

### Comparing `fpds-1.0.3/src/fpds/cli/parse.py` & `fpds-1.2.0/src/fpds/cli/parse.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.3/src/fpds/config.py` & `fpds-1.2.0/src/fpds/config.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.3/src/fpds/constants/fields.json` & `fpds-1.2.0/src/fpds/constants/fields.json`

 * *Files identical despite different names*

### Comparing `fpds-1.0.3/src/fpds/utilities/params.py` & `fpds-1.2.0/src/fpds/utilities/params.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.3/src/fpds.egg-info/PKG-INFO` & `fpds-1.2.0/src/fpds.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpds
-Version: 1.0.3
+Version: 1.2.0
 Summary: A parser for the Federal Procurement Data System (FPDS) Atom feed
 Author: Derek Herincx
 Author-email: derek663@gmail.com
 Keywords: fpds python atom cli
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
@@ -75,14 +75,17 @@
 request = fpdsRequest(
     LAST_MOD_DATE="[2022/01/01, 2022/05/01]",
     AGENCY_CODE="7504"
 )
 
 # Records saved as a python list
 records = request()
+
+# or equivalently, explicity call the `parse_content` method
+records = request.parse_content()
 ```
 
 For linting and formatting, we use `flake8` and `black`.
 
 ```
 $ make lint
 $ make formatters
@@ -95,28 +98,50 @@
 ```
 
 ### Testing
 ```
 $ make test
 ```
 
-
-## Additional Notes
-To ensure no data is lost during export, `fpds` will save tag attributes as
-individual data elements. For example, parsing the `contractActionType` tag
-and extracting the text value would only return `E` and omit data contained
-in the `description` and `part80orPart13` attributes.
-
-```
- <ns1:contractActionType description="BPA" part8OrPart13="PART8">E</ns1:contractActionType>
-```
-
-When parsing such elements, `fpds` will represent the tag above in the
-following manner:
-
-```
-    {
-        "contractActionType": "E",
-        "contractActionType__description": "BPA"
-        "contractActionType__part8OrPart13": "PART8"
-    }
+## What's New
+As of v1.2.0, tag names include their full XML tag hierarchy due to duplicate
+tag names being overwritten in v1.1.X. For example, the `content` XML below has the
+following duplicate tag names: `agencyID`, `PIID`, and `modNumber`.
+Based on the original hierarchy, it's clear that one set of tags represents
+the actual award info and the second, the award's referenced IDV.
+
+```
+<content xmlns:ns1="https://www.fpds.gov/FPDS" type="application/xml">
+    <ns1:awardID>
+        <ns1:awardContractID>
+            <ns1:agencyID name="ENVIRONMENTAL PROTECTION AGENCY">6800</ns1:agencyID>
+            <ns1:PIID>0002</ns1:PIID>
+            <ns1:modNumber>P00018</ns1:modNumber>
+            <ns1:transactionNumber>0</ns1:transactionNumber>
+        </ns1:awardContractID>
+        <ns1:referencedIDVID>
+            <ns1:agencyID name="ENVIRONMENTAL PROTECTION AGENCY">6800</ns1:agencyID>
+            <ns1:PIID>EPS31703</ns1:PIID>
+            <ns1:modNumber>0</ns1:modNumber>
+        </ns1:referencedIDVID>
+    </ns1:awardID>
+</content>
+```
+
+In lieu of this, the final JSON structure would represent this snippet of data
+the following (note that additional attributes like `name` in `agencyID` are
+still captured and represented by their proper hierarchy; the name of the
+attribute is appended to the end of the tag name):
+
+```
+{
+    "awardID__awardContractID__agenycID": "6800"
+    "awardID__awardContractID__agenycID__name": "ENVIRONMENTAL PROTECTION AGENCY"
+    "awardID__awardContractID__PIID": "0002"
+    "awardID__awardContractID__modNumber": "P00018"
+    "awardID__awardContractID__transactionNUmber: "0"
+    "referencedIDVID__awardContractID__agenycID": "6800"
+    "referencedIDVID__awardContractID__agenycID__name": "ENVIRONMENTAL PROTECTION AGENCY"
+    "referencedIDVID__awardContractID__PIID": "EPS31703"
+    "referencedIDVID__awardContractID__modNumber": "0"
+}
 ```
```

### Comparing `fpds-1.0.3/src/fpds.egg-info/SOURCES.txt` & `fpds-1.2.0/src/fpds.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,13 +12,15 @@
 src/fpds.egg-info/requires.txt
 src/fpds.egg-info/top_level.txt
 src/fpds/cli/__init__.py
 src/fpds/cli/parse.py
 src/fpds/constants/__init__.py
 src/fpds/constants/fields.json
 src/fpds/core/__init__.py
+src/fpds/core/mixins.py
 src/fpds/core/parser.py
+src/fpds/core/xml.py
 src/fpds/utilities/__init__.py
 src/fpds/utilities/params.py
 tests/test_cli.py
 tests/test_parser.py
 tests/test_xml.py
```

### Comparing `fpds-1.0.3/tests/test_cli.py` & `fpds-1.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.3/tests/test_parser.py` & `fpds-1.2.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `fpds-1.0.3/tests/test_xml.py` & `fpds-1.2.0/tests/test_xml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from unittest import TestCase
-from xml.etree.ElementTree import Element
+from xml.etree.ElementTree import Element, ElementTree
 
 from fpds import fpdsXML
+from fpds.core.xml import fpdsElement
 from tests import FULL_RESPONSE_DATA_BYTES, TRUNCATED_RESPONSE_DATA_BYTES
 
 FPDS_REQUEST_PARAMS_DICT = {
     "LAST_MOD_DATE": "[2022/01/01, 2022/05/01]",
     "AGENCY_CODE": "7504",
 }
 TEST_NAMESPACE_DICT = {
@@ -21,15 +22,15 @@
 
     def test_invalid_content_type(self):
         with pytest.raises(TypeError):
             fpdsXML(content="a-string-not-bytes-or-tree")
 
     def test_convert_to_lxml_tree(self):
         content = self._class.convert_to_lxml_tree()
-        self.assertIsInstance(content, Element)
+        self.assertIsInstance(content, ElementTree)
 
     def test_response_size(self):
         self.assertEqual(self._class.response_size, 10)
 
     def test_namespace_dict(self):
         namespace_dict = self._class.namespace_dict
         self.assertEqual(namespace_dict, TEST_NAMESPACE_DICT)
@@ -53,7 +54,18 @@
 
     def test_get_atom_feed_entries(self):
         entries = self._class.get_atom_feed_entries()
         # all entries should be of the same type
         entry_types = set([type(entry) for entry in entries])
         self.assertEqual(len(entries), 10)
         self.assertEqual(len(entry_types), 1)
+
+
+class TestFpdsElement(TestCase):
+    def setUp(self):
+        xml = fpdsXML(content=FULL_RESPONSE_DATA_BYTES)
+        element = xml.get_atom_feed_entries()[0]
+        self._class = fpdsElement(content=element)
+
+    def test_str_magic_method(self):
+        object_as_string = "<fpdsElement {http://www.w3.org/2005/Atom}entry>"
+        self.assertEqual(self._class.__str__(), object_as_string)
```

