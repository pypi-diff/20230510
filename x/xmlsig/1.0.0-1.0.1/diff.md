# Comparing `tmp/xmlsig-1.0.0.tar.gz` & `tmp/xmlsig-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlsig-1.0.0.tar", last modified: Wed Feb  8 15:59:40 2023, max compression
+gzip compressed data, was "xmlsig-1.0.1.tar", last modified: Wed May 10 13:50:23 2023, max compression
```

## Comparing `xmlsig-1.0.0.tar` & `xmlsig-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 operador  (1000) operador  (1000)        0 2023-02-08 15:59:40.874985 xmlsig-1.0.0/
--rw-rw-r--   0 operador  (1000) operador  (1000)     7651 2023-02-08 15:53:56.000000 xmlsig-1.0.0/LICENSE
--rw-rw-r--   0 operador  (1000) operador  (1000)      299 2023-02-08 15:53:28.000000 xmlsig-1.0.0/MANIFEST.in
--rw-rw-r--   0 operador  (1000) operador  (1000)      847 2023-02-08 15:59:40.874985 xmlsig-1.0.0/PKG-INFO
--rw-rw-r--   0 operador  (1000) operador  (1000)     1432 2023-02-08 15:53:28.000000 xmlsig-1.0.0/README.rst
--rw-rw-r--   0 operador  (1000) operador  (1000)      582 2023-02-08 15:59:40.874985 xmlsig-1.0.0/setup.cfg
--rw-rw-r--   0 operador  (1000) operador  (1000)     1571 2023-02-08 15:55:09.000000 xmlsig-1.0.0/setup.py
-drwxrwxr-x   0 operador  (1000) operador  (1000)        0 2023-02-08 15:59:40.870985 xmlsig-1.0.0/src/
-drwxrwxr-x   0 operador  (1000) operador  (1000)        0 2023-02-08 15:59:40.870985 xmlsig-1.0.0/src/xmlsig/
--rw-rw-r--   0 operador  (1000) operador  (1000)      137 2023-02-08 15:53:28.000000 xmlsig-1.0.0/src/xmlsig/__init__.py
-drwxrwxr-x   0 operador  (1000) operador  (1000)        0 2023-02-08 15:59:40.874985 xmlsig-1.0.0/src/xmlsig/algorithms/
--rw-rw-r--   0 operador  (1000) operador  (1000)       62 2023-02-08 15:53:28.000000 xmlsig-1.0.0/src/xmlsig/algorithms/__init__.py
--rw-rw-r--   0 operador  (1000) operador  (1000)     1542 2023-02-08 15:54:52.000000 xmlsig-1.0.0/src/xmlsig/algorithms/base.py
--rw-rw-r--   0 operador  (1000) operador  (1000)      683 2023-02-08 15:54:52.000000 xmlsig-1.0.0/src/xmlsig/algorithms/hmac.py
--rw-rw-r--   0 operador  (1000) operador  (1000)     2099 2023-02-08 15:54:52.000000 xmlsig-1.0.0/src/xmlsig/algorithms/rsa.py
--rw-rw-r--   0 operador  (1000) operador  (1000)     4170 2023-02-08 15:54:52.000000 xmlsig-1.0.0/src/xmlsig/constants.py
-drwxrwxr-x   0 operador  (1000) operador  (1000)        0 2023-02-08 15:59:40.874985 xmlsig-1.0.0/src/xmlsig/data/
--rw-rw-r--   0 operador  (1000) operador  (1000)    10355 2023-02-08 15:53:28.000000 xmlsig-1.0.0/src/xmlsig/data/xmldsig-core-schema.xsd
--rw-rw-r--   0 operador  (1000) operador  (1000)      739 2023-02-08 15:54:52.000000 xmlsig-1.0.0/src/xmlsig/ns.py
--rw-rw-r--   0 operador  (1000) operador  (1000)    15063 2023-02-08 15:54:52.000000 xmlsig-1.0.0/src/xmlsig/signature_context.py
--rw-rw-r--   0 operador  (1000) operador  (1000)     3488 2023-02-08 15:54:52.000000 xmlsig-1.0.0/src/xmlsig/template.py
--rw-rw-r--   0 operador  (1000) operador  (1000)     3154 2023-02-08 15:54:52.000000 xmlsig-1.0.0/src/xmlsig/utils.py
-drwxrwxr-x   0 operador  (1000) operador  (1000)        0 2023-02-08 15:59:40.874985 xmlsig-1.0.0/src/xmlsig.egg-info/
--rw-rw-r--   0 operador  (1000) operador  (1000)      847 2023-02-08 15:59:40.000000 xmlsig-1.0.0/src/xmlsig.egg-info/PKG-INFO
--rw-rw-r--   0 operador  (1000) operador  (1000)      553 2023-02-08 15:59:40.000000 xmlsig-1.0.0/src/xmlsig.egg-info/SOURCES.txt
--rw-rw-r--   0 operador  (1000) operador  (1000)        1 2023-02-08 15:59:40.000000 xmlsig-1.0.0/src/xmlsig.egg-info/dependency_links.txt
--rw-rw-r--   0 operador  (1000) operador  (1000)        1 2023-02-08 15:59:40.000000 xmlsig-1.0.0/src/xmlsig.egg-info/not-zip-safe
--rw-rw-r--   0 operador  (1000) operador  (1000)      255 2023-02-08 15:59:40.000000 xmlsig-1.0.0/src/xmlsig.egg-info/requires.txt
--rw-rw-r--   0 operador  (1000) operador  (1000)        7 2023-02-08 15:59:40.000000 xmlsig-1.0.0/src/xmlsig.egg-info/top_level.txt
+drwxrwxr-x   0 etobella  (1000) etobella  (1000)        0 2023-05-10 13:50:23.536340 xmlsig-1.0.1/
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)     7651 2023-05-10 13:27:20.000000 xmlsig-1.0.1/LICENSE
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      299 2023-05-10 13:27:20.000000 xmlsig-1.0.1/MANIFEST.in
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      847 2023-05-10 13:50:23.536340 xmlsig-1.0.1/PKG-INFO
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)     1432 2023-05-10 13:27:20.000000 xmlsig-1.0.1/README.rst
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      582 2023-05-10 13:50:23.536340 xmlsig-1.0.1/setup.cfg
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)     1541 2023-05-10 13:45:06.000000 xmlsig-1.0.1/setup.py
+drwxrwxr-x   0 etobella  (1000) etobella  (1000)        0 2023-05-10 13:50:23.536340 xmlsig-1.0.1/src/
+drwxrwxr-x   0 etobella  (1000) etobella  (1000)        0 2023-05-10 13:50:23.536340 xmlsig-1.0.1/src/xmlsig/
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      137 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/__init__.py
+drwxrwxr-x   0 etobella  (1000) etobella  (1000)        0 2023-05-10 13:50:23.536340 xmlsig-1.0.1/src/xmlsig/algorithms/
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)       62 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/algorithms/__init__.py
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)     1542 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/algorithms/base.py
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      683 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/algorithms/hmac.py
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)     2099 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/algorithms/rsa.py
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)     4170 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/constants.py
+drwxrwxr-x   0 etobella  (1000) etobella  (1000)        0 2023-05-10 13:50:23.536340 xmlsig-1.0.1/src/xmlsig/data/
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)    10355 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/data/xmldsig-core-schema.xsd
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      739 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/ns.py
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)    15136 2023-05-10 13:35:01.000000 xmlsig-1.0.1/src/xmlsig/signature_context.py
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)     3488 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/template.py
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)     3154 2023-05-10 13:27:20.000000 xmlsig-1.0.1/src/xmlsig/utils.py
+drwxrwxr-x   0 etobella  (1000) etobella  (1000)        0 2023-05-10 13:50:23.536340 xmlsig-1.0.1/src/xmlsig.egg-info/
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      847 2023-05-10 13:50:23.000000 xmlsig-1.0.1/src/xmlsig.egg-info/PKG-INFO
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      553 2023-05-10 13:50:23.000000 xmlsig-1.0.1/src/xmlsig.egg-info/SOURCES.txt
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)        1 2023-05-10 13:50:23.000000 xmlsig-1.0.1/src/xmlsig.egg-info/dependency_links.txt
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)        1 2023-05-10 13:50:23.000000 xmlsig-1.0.1/src/xmlsig.egg-info/not-zip-safe
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)      239 2023-05-10 13:50:23.000000 xmlsig-1.0.1/src/xmlsig.egg-info/requires.txt
+-rw-rw-r--   0 etobella  (1000) etobella  (1000)        7 2023-05-10 13:50:23.000000 xmlsig-1.0.1/src/xmlsig.egg-info/top_level.txt
```

### Comparing `xmlsig-1.0.0/LICENSE` & `xmlsig-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/PKG-INFO` & `xmlsig-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlsig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python based XML signature
 Home-page: http://github.com/etobella/python-xmlsig
 Author: Enric Tobella Alomar
 Author-email: etobella@creublanca.es
 License: LGPL-3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `xmlsig-1.0.0/README.rst` & `xmlsig-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -53,13 +53,13 @@
 
 Signature is only valid using RSA and HMAC validation.
 ECDSA and DSA is still being implemented
 
 License
 =======
 
-This library is published under the AGPL-3 license.
+This library is published under the LGPL-3 license.
 
 Contributors
 ============
 
 * Enric Tobella <etobella@creublanca.es>
```

### Comparing `xmlsig-1.0.0/setup.cfg` & `xmlsig-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/setup.py` & `xmlsig-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from setuptools import find_packages, setup
 
 install_requires = [
     "lxml>=3.0.0",
     "cryptography",
-    "asn1crypto",
-    "cffi",
 ]
 
 tests_require = [
     "freezegun==0.3.8",
     "mock==2.0.0",
     "pretend==1.0.8",
     "pytest-cov==2.5.1",
@@ -21,15 +19,15 @@
     "flake8-debugger==1.4.0",
     "flake8-imports==0.1.1",
 ]
 
 
 setup(
     name="xmlsig",
-    version="1.0.0",
+    version="1.0.1",
     description="Python based XML signature",
     long_description="XML Signature created with cryptography and lxml",
     author="Enric Tobella Alomar",
     author_email="etobella@creublanca.es",
     url="http://github.com/etobella/python-xmlsig",
     install_requires=install_requires,
     tests_require=tests_require,
```

### Comparing `xmlsig-1.0.0/src/xmlsig/algorithms/base.py` & `xmlsig-1.0.1/src/xmlsig/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/src/xmlsig/algorithms/hmac.py` & `xmlsig-1.0.1/src/xmlsig/algorithms/hmac.py`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/src/xmlsig/algorithms/rsa.py` & `xmlsig-1.0.1/src/xmlsig/algorithms/rsa.py`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/src/xmlsig/constants.py` & `xmlsig-1.0.1/src/xmlsig/constants.py`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/src/xmlsig/data/xmldsig-core-schema.xsd` & `xmlsig-1.0.1/src/xmlsig/data/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/src/xmlsig/ns.py` & `xmlsig-1.0.1/src/xmlsig/ns.py`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/src/xmlsig/signature_context.py` & `xmlsig-1.0.1/src/xmlsig/signature_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # © 2017 Creu Blanca
 # License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl.html).
 
 import base64
 import hashlib
 from os import path
 
-import OpenSSL
 from cryptography.hazmat.primitives import serialization
 from cryptography.x509.oid import ExtensionOID
 from lxml import etree
 
 from . import constants
 from .utils import b64_print, create_node, get_rdns_name
 
+try:
+    import OpenSSL
+except ImportError:
+    OpenSSL = None
+
 
 class SignatureContext(object):
     """
     Signature context is used to sign and verify Signature nodes with keys
     """
 
     def __init__(self):
@@ -363,15 +367,15 @@
         """
         This function fills the context public_key, private_key and x509 from
         PKCS12 Object
         :param key: the PKCS12 Object
         :type key: Union[OpenSSL.crypto.PKCS12, tuple]
         :return: None
         """
-        if isinstance(key, OpenSSL.crypto.PKCS12):
+        if OpenSSL is not None and isinstance(key, OpenSSL.crypto.PKCS12):
             # This would happen if we are using pyOpenSSL
             self.x509 = key.get_certificate().to_cryptography()
             self.public_key = key.get_certificate().to_cryptography().public_key()
             self.private_key = key.get_privatekey().to_cryptography_key()
         elif isinstance(key, tuple):
             # This would happen if we are using cryptography
             self.x509 = key[1]
```

### Comparing `xmlsig-1.0.0/src/xmlsig/template.py` & `xmlsig-1.0.1/src/xmlsig/template.py`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/src/xmlsig/utils.py` & `xmlsig-1.0.1/src/xmlsig/utils.py`

 * *Files identical despite different names*

### Comparing `xmlsig-1.0.0/src/xmlsig.egg-info/PKG-INFO` & `xmlsig-1.0.1/src/xmlsig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlsig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python based XML signature
 Home-page: http://github.com/etobella/python-xmlsig
 Author: Enric Tobella Alomar
 Author-email: etobella@creublanca.es
 License: LGPL-3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `xmlsig-1.0.0/src/xmlsig.egg-info/SOURCES.txt` & `xmlsig-1.0.1/src/xmlsig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

