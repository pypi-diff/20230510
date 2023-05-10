# Comparing `tmp/cnert-0.3.0.tar.gz` & `tmp/cnert-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnert-0.3.0.tar", max compression
+gzip compressed data, was "cnert-0.4.0.tar", max compression
```

## Comparing `cnert-0.3.0.tar` & `cnert-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.3.0/LICENSE
--rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.3.0/LICENSE.apache2
--rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.3.0/LICENSE.mit
--rw-r--r--   0        0        0     7708 2023-05-08 16:56:02.305888 cnert-0.3.0/README.md
--rw-r--r--   0        0        0     3150 2023-05-08 17:02:19.302109 cnert-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    20537 2023-05-08 17:02:19.302246 cnert-0.3.0/src/cnert/__init__.py
--rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.3.0/src/cnert/py.typed
--rw-r--r--   0        0        0     9472 1970-01-01 00:00:00.000000 cnert-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.4.0/LICENSE.apache2
+-rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.4.0/LICENSE.mit
+-rw-r--r--   0        0        0     7873 2023-05-09 15:49:26.045857 cnert-0.4.0/README.md
+-rw-r--r--   0        0        0     3150 2023-05-09 15:49:26.049096 cnert-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    22638 2023-05-10 12:29:07.445474 cnert-0.4.0/src/cnert/__init__.py
+-rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.4.0/src/cnert/py.typed
+-rw-r--r--   0        0        0     9637 1970-01-01 00:00:00.000000 cnert-0.4.0/PKG-INFO
```

### Comparing `cnert-0.3.0/LICENSE.apache2` & `cnert-0.4.0/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `cnert-0.3.0/LICENSE.mit` & `cnert-0.4.0/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `cnert-0.3.0/README.md` & `cnert-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 [![PyPI version](https://badge.fury.io/py/cnert.svg)](https://badge.fury.io/py/cnert)
 [![Documentation Status](https://readthedocs.org/projects/cnert/badge/?version=latest)](https://cnert.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/maartenq/cnert/main.svg)](https://results.pre-commit.ci/latest/github/maartenq/cnert/main)
 [![workflow ci](https://github.com/maartenq/cnert/actions/workflows/main.yml/badge.svg)](https://github.com/maartenq/cnert/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/maartenq/cnert/branch/main/graph/badge.svg?token=XXXXXXXXXX)](https://codecov.io/gh/maartenq/cnert)
 [![License](https://img.shields.io/badge/license-MIT%2FApache--2.0-blue.svg)](LICENSE)
 
+
 # Cnert - TLS Certificates for testing
 
 Cnert is simple Python API for creating TLS Certificates and stuff for testing
 purposes (on top of [cryptography]).
 
-[cnert.CA][cnert_CA] makes it easy to create CAs, intermediate CAs. These CA
-objects can then issue directly [certificates][cnert_Cert].
+[cnert.CA][] makes it easy to create CAs, intermediate CAs. These CA objects
+can then issue directly [certificates][cnert._Cert].
 
 Cnert can make CSRs. CA objects also use these to issue certificates.
 
 Subject and Issuer Name Attributes, Subject Alternative Names, not_before_date
 and not_after_data can all be set.
 
 Cnert has different methods to introspect these.
@@ -125,14 +126,17 @@
 
     >>> cert.public_key
     <cryptography.hazmat.backends.openssl.rsa._RSAPublicKey object at 0x10361c150>
 
     >>> cert.public_key_pem
     b'-----BEGIN CERTIFICATE-----\nMIIDITCCAgmgAwIBAgIUAx6AA8z3BqH/ICCmqOJXGI7PHCswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODU5NTlaFw0yMzA4MDcw\nODU5NTlaMBYxFDASBgNVBAMMC2V4YW1wbGUuY29tMIIBIjANBgkqhkiG9w0BAQEF\nAAOCAQ8AMIIBCgKCAQEAnWAlLvbR0hE8seqI8uBj8ESicJ/nF8I3KF9CFlTexQ73\nKdyqTRCoPZ6uuK0quX+qX5KeeNlWSnJRxSDc0WmLwYxWFVg6hmBDPLK1Ijntc1Uj\n4HENkolgPUBxgf9VBSmojqd1XL0o8PwGFIoyZ6Z/YTc3MqML4QZaB0m+TYlVgoJP\nQgFT9d9nQadvyswIx7nOMkT0Rd3sGl8nWaNgDaBLB6mkylGrtaiyo2M2LWKvNz69\nDWbjlccj65B04cBLwRcA2Zmx80leajX1zNWt0+dhJFo6rnLtmvIgqdLhCrNTmDMK\nrlyVsOrwJfXNreIPDEgYztZlrUdTnynmF4bW6W5KcwIDAQABo2swaTAdBgNVHQ4E\nFgQURd1r0d7XJBtT651AbuR2hg7TQBIwDAYDVR0TAQH/BAIwADAOBgNVHQ8BAf8E\nBAMCBaAwKgYDVR0lAQH/BCAwHgYIKwYBBQUHAwIGCCsGAQUFBwMBBggrBgEFBQcD\nAzANBgkqhkiG9w0BAQsFAAOCAQEANcFmZZkt4Z6jc069IOonGfcpUdnZieSEVyBE\nCQC+QWaHYqcD0ryYV8n1/UzNVcSkptQ5YrbgXNikV6+cuklFq4OjHlUDGOxchrkc\nSFGYAf+j7wAAx+OZWH5IwvMSTWGhfi7FWNFrzbO3JUE1q3OOnsIUmcDpd/8zucyE\njPf6F0MVujwMJq8VAH8UtUpVm1SApEBz9vgx0n7Z0l5fgRw7PMwwDkaoyplSC0VA\n7F7AUX3K0oJ7Gyw+9onfS090GMo6mlTfhtXNpPArleUUOTrp+TKVhwtz8GRRzxEW\nBE1OaNZaipKILZPbgDa5u67pRdU/OhuMFDsBh1GlPopcax+rCQ==\n-----END CERTIFICATE-----\n'
 
+    >>> cert.SHA1
+    '21B99CE5588417932ACB65C54398115C75240B04'
+
 
 
 ###  Issue a cert from a CA with alt names
 
     >>> cert = ca.issue_cert("www.example.com", "host1.example.com", "example.com")
 
     >>> cert.subject_attrs
@@ -160,9 +164,13 @@
     HatP/+RbrQ==\n-----END CERTIFICATE REQUEST-----\n'
 
     >>> csr.subject_attrs.COMMON_NAME
     'example.com'
 
 [cryptography]: https://cryptography.io/en/latest/
 [trustme]: https://github.com/python-trio/trustme
-[cnert_CA]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnertca
-[cnert_Cert]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
+
+
+[cryptography]: https://cryptography.io/en/latest/
+[trustme]: https://github.com/python-trio/trustme
+[cnert.CA]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnertca
+[cnert._Cert]]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
```

### Comparing `cnert-0.3.0/pyproject.toml` & `cnert-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cnert"
-version = "0.3.0"
+version = "0.4.0"
 description = "Cnert is trying to be a simple API for creating TLS Certificates testing purposes."
 authors = ["Maarten <ikmaarten@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maartenq/cnert"
 repository = "https://github.com/maartenq/cnert"
 documentation = "https://cnert.readthedocs.io/en/latest/"
```

### Comparing `cnert-0.3.0/src/cnert/__init__.py` & `cnert-0.4.0/src/cnert/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cnert/__init__.py
 
 """
 Cnert makes TLS private keys, CSRs, private CAs and certificates.
 """
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __title__ = "Cnert"
 __description__ = (
     "Cnert makes TLS private keys, CSRs, private CAs and certificates."
 )
 __uri__ = "https://github.com/maartenq/cnert"
 __author__ = "Maarten"
 __email__ = "ikmaarten@gmail.com"
@@ -418,32 +418,109 @@
         )
         self.public_key_pem = self.certificate.public_bytes(
             serialization.Encoding.PEM
         )
 
     @property
     def private_key_pem_PKCS1(self) -> bytes:
+        """
+        Examples:
+            >>> cert = CA().issue_cert()
+            >>> cert.private_key_pem_PKCS1
+            b'-----begin rsa private key-----
+            ...
+            \n-----end rsa private key-----\n'
+
+
+        Returns:
+            PEM encoded serialized key in TraditionalOpenSSL format.
+        """
         return self.private_key.private_bytes(
             serialization.Encoding.PEM,
             format=serialization.PrivateFormat.TraditionalOpenSSL,
             encryption_algorithm=serialization.NoEncryption(),
         )
 
     @property
     def private_key_pem(self) -> bytes:
+        """
+        Examples:
+            >>> cert = CA().issue_cert()
+            >>> cert.private_key_pem
+            b'-----BEGIN PRIVATE KEY-----
+            ...
+            \n-----END PRIVATE KEY-----\n'
+
+
+        Returns:
+            PEM encoded serialized key in PKCS8 format.
+        """
         return self.private_key.private_bytes(
             serialization.Encoding.PEM,
             format=serialization.PrivateFormat.PKCS8,
             encryption_algorithm=serialization.NoEncryption(),
         )
 
     @property
     def public_key(self) -> rsa.RSAPublicKey:
+        """
+        Examples:
+            >>> cert = cnert.CA().issue_cert()
+            >>> cert.private_key
+            <cryptography.hazmat.backends.openssl.rsa._RSAPrivateKey object
+            at 0x1014e4e10>
+
+        Returns:
+            An RSA private key.
+        """
         return self.private_key.public_key()
 
+    @property
+    def MD5(self) -> str:
+        """
+        Examples:
+            >>> cert = cnert.CA().issue_cert()
+            >>> cert.MD5
+            'A03D37486DD47BE3E9C7EC1624073856'
+
+        Returns:
+            MD5 Fingerprint string in upper case.
+        """
+        return bytes.hex(
+            self.certificate.fingerprint(hashes.MD5()),  # noqa: S303
+        ).upper()
+
+    @property
+    def SHA1(self) -> str:
+        """
+        Examples:
+            >>> cert = cnert.CA().issue_cert()
+            >>> cert.SHA1
+            '9E0A06CFB37B352FDA5B2226E6D631CF07D5D185'
+
+        Returns:
+            SHA1 Fingerprint string in upper case.
+        """
+        return bytes.hex(
+            self.certificate.fingerprint(hashes.SHA1()),  # noqa: S303
+        ).upper()
+
+    @property
+    def SHA256(self) -> str:
+        """
+        Examples:
+            >>> cert = cnert.CA().issue_cert()
+            >>> cert.SHA256
+            '68307A6CBE2804038DF85FB53AEE96AB47EA81439AB2E059DDDEA9F901097D84'
+
+        Returns:
+            SHA256 Fingerprint string in upper case.
+        """
+        return bytes.hex(self.certificate.fingerprint(hashes.SHA256())).upper()
+
     def __str__(self) -> str:
         return f"Certificate {self.subject_attrs}"
 
 
 class CSR:
     """
     A CSR object.
@@ -646,18 +723,19 @@
 
         Examples:
             >>> ca = CA()
             >>> ca.issue_cert()
             <cnert.Cert at 0x107f87f50>
 
         Parameters:
-            sans: Subject Alternative Names as positional arguments
-            subject_attrs: Subject Name Attributes
-            not_valid_before: Certificate not valid before date
-            not_valid_after: Certificate not valid after date
+            sans: Subject Alternative Names as positional arguments.
+            subject_attrs: Subject Name Attributes.
+            not_valid_before: Certificate not valid before date.
+            not_valid_after: Certificate not valid after date.
+            csr: A CSR object.
 
         Returns:
             A _Cert object.
 
         """
         if csr is None:
             private_key = None
```

### Comparing `cnert-0.3.0/PKG-INFO` & `cnert-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnert
-Version: 0.3.0
+Version: 0.4.0
 Summary: Cnert is trying to be a simple API for creating TLS Certificates testing purposes.
 Home-page: https://github.com/maartenq/cnert
 License: MIT
 Keywords: certificate,X.509,TLS,cryptography,testing
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -42,21 +42,22 @@
 [![PyPI version](https://badge.fury.io/py/cnert.svg)](https://badge.fury.io/py/cnert)
 [![Documentation Status](https://readthedocs.org/projects/cnert/badge/?version=latest)](https://cnert.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/maartenq/cnert/main.svg)](https://results.pre-commit.ci/latest/github/maartenq/cnert/main)
 [![workflow ci](https://github.com/maartenq/cnert/actions/workflows/main.yml/badge.svg)](https://github.com/maartenq/cnert/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/maartenq/cnert/branch/main/graph/badge.svg?token=XXXXXXXXXX)](https://codecov.io/gh/maartenq/cnert)
 [![License](https://img.shields.io/badge/license-MIT%2FApache--2.0-blue.svg)](LICENSE)
 
+
 # Cnert - TLS Certificates for testing
 
 Cnert is simple Python API for creating TLS Certificates and stuff for testing
 purposes (on top of [cryptography]).
 
-[cnert.CA][cnert_CA] makes it easy to create CAs, intermediate CAs. These CA
-objects can then issue directly [certificates][cnert_Cert].
+[cnert.CA][] makes it easy to create CAs, intermediate CAs. These CA objects
+can then issue directly [certificates][cnert._Cert].
 
 Cnert can make CSRs. CA objects also use these to issue certificates.
 
 Subject and Issuer Name Attributes, Subject Alternative Names, not_before_date
 and not_after_data can all be set.
 
 Cnert has different methods to introspect these.
@@ -164,14 +165,17 @@
 
     >>> cert.public_key
     <cryptography.hazmat.backends.openssl.rsa._RSAPublicKey object at 0x10361c150>
 
     >>> cert.public_key_pem
     b'-----BEGIN CERTIFICATE-----\nMIIDITCCAgmgAwIBAgIUAx6AA8z3BqH/ICCmqOJXGI7PHCswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODU5NTlaFw0yMzA4MDcw\nODU5NTlaMBYxFDASBgNVBAMMC2V4YW1wbGUuY29tMIIBIjANBgkqhkiG9w0BAQEF\nAAOCAQ8AMIIBCgKCAQEAnWAlLvbR0hE8seqI8uBj8ESicJ/nF8I3KF9CFlTexQ73\nKdyqTRCoPZ6uuK0quX+qX5KeeNlWSnJRxSDc0WmLwYxWFVg6hmBDPLK1Ijntc1Uj\n4HENkolgPUBxgf9VBSmojqd1XL0o8PwGFIoyZ6Z/YTc3MqML4QZaB0m+TYlVgoJP\nQgFT9d9nQadvyswIx7nOMkT0Rd3sGl8nWaNgDaBLB6mkylGrtaiyo2M2LWKvNz69\nDWbjlccj65B04cBLwRcA2Zmx80leajX1zNWt0+dhJFo6rnLtmvIgqdLhCrNTmDMK\nrlyVsOrwJfXNreIPDEgYztZlrUdTnynmF4bW6W5KcwIDAQABo2swaTAdBgNVHQ4E\nFgQURd1r0d7XJBtT651AbuR2hg7TQBIwDAYDVR0TAQH/BAIwADAOBgNVHQ8BAf8E\nBAMCBaAwKgYDVR0lAQH/BCAwHgYIKwYBBQUHAwIGCCsGAQUFBwMBBggrBgEFBQcD\nAzANBgkqhkiG9w0BAQsFAAOCAQEANcFmZZkt4Z6jc069IOonGfcpUdnZieSEVyBE\nCQC+QWaHYqcD0ryYV8n1/UzNVcSkptQ5YrbgXNikV6+cuklFq4OjHlUDGOxchrkc\nSFGYAf+j7wAAx+OZWH5IwvMSTWGhfi7FWNFrzbO3JUE1q3OOnsIUmcDpd/8zucyE\njPf6F0MVujwMJq8VAH8UtUpVm1SApEBz9vgx0n7Z0l5fgRw7PMwwDkaoyplSC0VA\n7F7AUX3K0oJ7Gyw+9onfS090GMo6mlTfhtXNpPArleUUOTrp+TKVhwtz8GRRzxEW\nBE1OaNZaipKILZPbgDa5u67pRdU/OhuMFDsBh1GlPopcax+rCQ==\n-----END CERTIFICATE-----\n'
 
+    >>> cert.SHA1
+    '21B99CE5588417932ACB65C54398115C75240B04'
+
 
 
 ###  Issue a cert from a CA with alt names
 
     >>> cert = ca.issue_cert("www.example.com", "host1.example.com", "example.com")
 
     >>> cert.subject_attrs
@@ -199,10 +203,14 @@
     HatP/+RbrQ==\n-----END CERTIFICATE REQUEST-----\n'
 
     >>> csr.subject_attrs.COMMON_NAME
     'example.com'
 
 [cryptography]: https://cryptography.io/en/latest/
 [trustme]: https://github.com/python-trio/trustme
-[cnert_CA]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnertca
-[cnert_Cert]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
+
+
+[cryptography]: https://cryptography.io/en/latest/
+[trustme]: https://github.com/python-trio/trustme
+[cnert.CA]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnertca
+[cnert._Cert]]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
```

