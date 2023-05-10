# Comparing `tmp/cnert-0.4.0.tar.gz` & `tmp/cnert-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnert-0.4.0.tar", max compression
+gzip compressed data, was "cnert-0.5.0.tar", max compression
```

## Comparing `cnert-0.4.0.tar` & `cnert-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.4.0/LICENSE
--rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.4.0/LICENSE.apache2
--rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.4.0/LICENSE.mit
--rw-r--r--   0        0        0     7873 2023-05-09 15:49:26.045857 cnert-0.4.0/README.md
--rw-r--r--   0        0        0     3150 2023-05-09 15:49:26.049096 cnert-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    22638 2023-05-10 12:29:07.445474 cnert-0.4.0/src/cnert/__init__.py
--rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.4.0/src/cnert/py.typed
--rw-r--r--   0        0        0     9637 1970-01-01 00:00:00.000000 cnert-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.5.0/LICENSE
+-rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.5.0/LICENSE.apache2
+-rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.5.0/LICENSE.mit
+-rw-r--r--   0        0        0     8577 2023-05-10 13:45:50.023695 cnert-0.5.0/README.md
+-rw-r--r--   0        0        0     3150 2023-05-10 14:05:49.946732 cnert-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    22623 2023-05-10 14:05:49.980463 cnert-0.5.0/src/cnert/__init__.py
+-rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.5.0/src/cnert/py.typed
+-rw-r--r--   0        0        0    10341 1970-01-01 00:00:00.000000 cnert-0.5.0/PKG-INFO
```

### Comparing `cnert-0.4.0/LICENSE.apache2` & `cnert-0.5.0/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `cnert-0.4.0/LICENSE.mit` & `cnert-0.5.0/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `cnert-0.4.0/README.md` & `cnert-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,37 @@
 TLS certificate and there for can make tailor made certificates for testing
 those apps.
 
 If you don't need that and you just need any "old" certificate, you probably
 better of with [trustme], trust me, or better: trust them.
 
 
+# Cnert - TLS Certificates for testing
+
+Cnert is simple Python API for creating TLS Certificates and stuff for testing
+purposes (on top of [cryptography]).
+
+[cnert.CA][] makes it easy to create CAs, intermediate CAs. These CA objects
+can then issue directly [certificates][cnert._Cert].
+
+Cnert can make CSRs. CA objects also use these to issue certificates.
+
+Subject and Issuer Name Attributes, Subject Alternative Names, not_before_date
+and not_after_data can all be set.
+
+Cnert has different methods to introspect these.
+
+Cnert is made specially made for testing application that *do something* with
+TLS certificate and there for can make tailor made certificates for testing
+those apps.
+
+If you don't need that and you just need any "old" certificate, you probably
+better of with [trustme], trust me, or better: trust them.
+
+
 ## Usage
 
 ### Create a root CA
 
     >>> import cnert
     >>> ca = cnert.CA()
 
@@ -91,15 +114,15 @@
 
     >>> ca.cert.path_length
     9
 
     >>> ca.cert.public_key.key_size
     2048
 
-    >>> ca.cert.public_key_pem
+    >>> ca.cert.pem
     b'-----BEGIN CERTIFICATE-----\nMIIC9zCCAd+gAwIBAgIUGyCBgdyVPVGlYIJj25+x1AMQPHswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODQyNThaFw0yMzA4MDcw\nODQyNThaMBIxEDAOBgNVBAoMB1Jvb3QgQ0EwggEiMA0GCSqGSIb3DQEBAQUAA4IB\nDwAwggEKAoIBAQDK13Q6dZdK17SPmplwTq4Phh7TatM4HQqONEq6+xE2VnJ9eeCh\nQYM5w5dnxIUeV10j3ODPJz5L+6IirV/e6voCWkS6Vgzh/lAVTbUVGANR26NpMnjm\n/qU0NUYuSQo5QFJuwFEx9CZ1xGTac9gspBo1jO7E9m01pRAXlr1HqTZT7mY4LNWb\nDyjKmMa/tfK0+itiKce48hZDxqy3YLnWYyIAZ+rTrf9RW5hpLb6g/KeAf3w5q55Q\nL2dCsC6flZ6NFVRm7okpawwN2tf5c451fMm3B+GtVJJMP+6lmk6MC3h++pcwOimg\nUwB8tYEPoZHuMjd1hacZcbfGFzCGAbme+BZbAgMBAAGjRTBDMB0GA1UdDgQWBBSA\nIsRH6giY94MEfhzafTd5WC2HMzASBgNVHRMBAf8ECDAGAQH/AgEJMA4GA1UdDwEB\n/wQEAwIBpjANBgkqhkiG9w0BAQsFAAOCAQEACLdxWMlmr3drMvA7GaQArzlbe/ny\nx8mThDhZP6gx+yTJ6LXk8CFc7S23JXFZVquwcV5yFa0DavaodBI3RNWknx/Yu5Lm\nM7cOByu2IuJhcEu4o+ZntLZLb7heFMXMIf01lVkYpyYyvS/NvVdu9km8f6ZvxV9r\nDyTDDMjeh+hg5l2Wwc4P6UGoMlmOruUiunsb8hiDLhD+brYBHKHqJY9pCrzJQd0v\nWEkAOsBwaTv/POO0F4VDZSfA5CqjYOkppupw9nXXfJkk9PvKuDI1G2XO7pcW1PWh\nDdGK6Wz0AXMWWbbX8LToDrFA9q7YOxGNOVPhbHZ++bDJvLNmjrtruy3UTQ==\n-----END CERTIFICATE-----\n'
 
 
 
 ###  Inspect the Intermediate CA
 
     >>> intermediate.cert.subject_attrs
@@ -123,15 +146,15 @@
 
     >>> cert.subject_attrs.COMMON_NAME
     'example.com'
 
     >>> cert.public_key
     <cryptography.hazmat.backends.openssl.rsa._RSAPublicKey object at 0x10361c150>
 
-    >>> cert.public_key_pem
+    >>> cert.pem
     b'-----BEGIN CERTIFICATE-----\nMIIDITCCAgmgAwIBAgIUAx6AA8z3BqH/ICCmqOJXGI7PHCswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODU5NTlaFw0yMzA4MDcw\nODU5NTlaMBYxFDASBgNVBAMMC2V4YW1wbGUuY29tMIIBIjANBgkqhkiG9w0BAQEF\nAAOCAQ8AMIIBCgKCAQEAnWAlLvbR0hE8seqI8uBj8ESicJ/nF8I3KF9CFlTexQ73\nKdyqTRCoPZ6uuK0quX+qX5KeeNlWSnJRxSDc0WmLwYxWFVg6hmBDPLK1Ijntc1Uj\n4HENkolgPUBxgf9VBSmojqd1XL0o8PwGFIoyZ6Z/YTc3MqML4QZaB0m+TYlVgoJP\nQgFT9d9nQadvyswIx7nOMkT0Rd3sGl8nWaNgDaBLB6mkylGrtaiyo2M2LWKvNz69\nDWbjlccj65B04cBLwRcA2Zmx80leajX1zNWt0+dhJFo6rnLtmvIgqdLhCrNTmDMK\nrlyVsOrwJfXNreIPDEgYztZlrUdTnynmF4bW6W5KcwIDAQABo2swaTAdBgNVHQ4E\nFgQURd1r0d7XJBtT651AbuR2hg7TQBIwDAYDVR0TAQH/BAIwADAOBgNVHQ8BAf8E\nBAMCBaAwKgYDVR0lAQH/BCAwHgYIKwYBBQUHAwIGCCsGAQUFBwMBBggrBgEFBQcD\nAzANBgkqhkiG9w0BAQsFAAOCAQEANcFmZZkt4Z6jc069IOonGfcpUdnZieSEVyBE\nCQC+QWaHYqcD0ryYV8n1/UzNVcSkptQ5YrbgXNikV6+cuklFq4OjHlUDGOxchrkc\nSFGYAf+j7wAAx+OZWH5IwvMSTWGhfi7FWNFrzbO3JUE1q3OOnsIUmcDpd/8zucyE\njPf6F0MVujwMJq8VAH8UtUpVm1SApEBz9vgx0n7Z0l5fgRw7PMwwDkaoyplSC0VA\n7F7AUX3K0oJ7Gyw+9onfS090GMo6mlTfhtXNpPArleUUOTrp+TKVhwtz8GRRzxEW\nBE1OaNZaipKILZPbgDa5u67pRdU/OhuMFDsBh1GlPopcax+rCQ==\n-----END CERTIFICATE-----\n'
 
     >>> cert.SHA1
     '21B99CE5588417932ACB65C54398115C75240B04'
 
 
 
@@ -165,12 +188,9 @@
 
     >>> csr.subject_attrs.COMMON_NAME
     'example.com'
 
 [cryptography]: https://cryptography.io/en/latest/
 [trustme]: https://github.com/python-trio/trustme
 
-
-[cryptography]: https://cryptography.io/en/latest/
-[trustme]: https://github.com/python-trio/trustme
 [cnert.CA]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnertca
-[cnert._Cert]]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
+[cnert._Cert]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
```

### Comparing `cnert-0.4.0/pyproject.toml` & `cnert-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cnert"
-version = "0.4.0"
+version = "0.5.0"
 description = "Cnert is trying to be a simple API for creating TLS Certificates testing purposes."
 authors = ["Maarten <ikmaarten@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maartenq/cnert"
 repository = "https://github.com/maartenq/cnert"
 documentation = "https://cnert.readthedocs.io/en/latest/"
```

### Comparing `cnert-0.4.0/src/cnert/__init__.py` & `cnert-0.5.0/src/cnert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cnert/__init__.py
 
 """
 Cnert makes TLS private keys, CSRs, private CAs and certificates.
 """
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __title__ = "Cnert"
 __description__ = (
     "Cnert makes TLS private keys, CSRs, private CAs and certificates."
 )
 __uri__ = "https://github.com/maartenq/cnert"
 __author__ = "Maarten"
 __email__ = "ikmaarten@gmail.com"
@@ -412,17 +412,15 @@
             self.is_ca,
             None if not self.is_ca else self.path_length,
             self.public_key,
         )
         self.certificate = cert_builder.sign(
             self.parent.private_key if self.parent else self.private_key,
         )
-        self.public_key_pem = self.certificate.public_bytes(
-            serialization.Encoding.PEM
-        )
+        self.pem = self.certificate.public_bytes(serialization.Encoding.PEM)
 
     @property
     def private_key_pem_PKCS1(self) -> bytes:
         """
         Examples:
             >>> cert = CA().issue_cert()
             >>> cert.private_key_pem_PKCS1
@@ -437,19 +435,19 @@
         return self.private_key.private_bytes(
             serialization.Encoding.PEM,
             format=serialization.PrivateFormat.TraditionalOpenSSL,
             encryption_algorithm=serialization.NoEncryption(),
         )
 
     @property
-    def private_key_pem(self) -> bytes:
+    def private_key_pem_PKCS8(self) -> bytes:
         """
         Examples:
             >>> cert = CA().issue_cert()
-            >>> cert.private_key_pem
+            >>> cert.private_key_pem_PKCS8
             b'-----BEGIN PRIVATE KEY-----
             ...
             \n-----END PRIVATE KEY-----\n'
 
 
         Returns:
             PEM encoded serialized key in PKCS8 format.
@@ -586,15 +584,15 @@
         return self.private_key.private_bytes(
             serialization.Encoding.PEM,
             format=serialization.PrivateFormat.TraditionalOpenSSL,
             encryption_algorithm=serialization.NoEncryption(),
         )
 
     @property
-    def private_key_pem(self) -> bytes:
+    def private_key_pem_PKCS8(self) -> bytes:
         return self.private_key.private_bytes(
             serialization.Encoding.PEM,
             format=serialization.PrivateFormat.PKCS8,
             encryption_algorithm=serialization.NoEncryption(),
         )
 
     @property
```

### Comparing `cnert-0.4.0/PKG-INFO` & `cnert-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnert
-Version: 0.4.0
+Version: 0.5.0
 Summary: Cnert is trying to be a simple API for creating TLS Certificates testing purposes.
 Home-page: https://github.com/maartenq/cnert
 License: MIT
 Keywords: certificate,X.509,TLS,cryptography,testing
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -66,14 +66,37 @@
 TLS certificate and there for can make tailor made certificates for testing
 those apps.
 
 If you don't need that and you just need any "old" certificate, you probably
 better of with [trustme], trust me, or better: trust them.
 
 
+# Cnert - TLS Certificates for testing
+
+Cnert is simple Python API for creating TLS Certificates and stuff for testing
+purposes (on top of [cryptography]).
+
+[cnert.CA][] makes it easy to create CAs, intermediate CAs. These CA objects
+can then issue directly [certificates][cnert._Cert].
+
+Cnert can make CSRs. CA objects also use these to issue certificates.
+
+Subject and Issuer Name Attributes, Subject Alternative Names, not_before_date
+and not_after_data can all be set.
+
+Cnert has different methods to introspect these.
+
+Cnert is made specially made for testing application that *do something* with
+TLS certificate and there for can make tailor made certificates for testing
+those apps.
+
+If you don't need that and you just need any "old" certificate, you probably
+better of with [trustme], trust me, or better: trust them.
+
+
 ## Usage
 
 ### Create a root CA
 
     >>> import cnert
     >>> ca = cnert.CA()
 
@@ -130,15 +153,15 @@
 
     >>> ca.cert.path_length
     9
 
     >>> ca.cert.public_key.key_size
     2048
 
-    >>> ca.cert.public_key_pem
+    >>> ca.cert.pem
     b'-----BEGIN CERTIFICATE-----\nMIIC9zCCAd+gAwIBAgIUGyCBgdyVPVGlYIJj25+x1AMQPHswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODQyNThaFw0yMzA4MDcw\nODQyNThaMBIxEDAOBgNVBAoMB1Jvb3QgQ0EwggEiMA0GCSqGSIb3DQEBAQUAA4IB\nDwAwggEKAoIBAQDK13Q6dZdK17SPmplwTq4Phh7TatM4HQqONEq6+xE2VnJ9eeCh\nQYM5w5dnxIUeV10j3ODPJz5L+6IirV/e6voCWkS6Vgzh/lAVTbUVGANR26NpMnjm\n/qU0NUYuSQo5QFJuwFEx9CZ1xGTac9gspBo1jO7E9m01pRAXlr1HqTZT7mY4LNWb\nDyjKmMa/tfK0+itiKce48hZDxqy3YLnWYyIAZ+rTrf9RW5hpLb6g/KeAf3w5q55Q\nL2dCsC6flZ6NFVRm7okpawwN2tf5c451fMm3B+GtVJJMP+6lmk6MC3h++pcwOimg\nUwB8tYEPoZHuMjd1hacZcbfGFzCGAbme+BZbAgMBAAGjRTBDMB0GA1UdDgQWBBSA\nIsRH6giY94MEfhzafTd5WC2HMzASBgNVHRMBAf8ECDAGAQH/AgEJMA4GA1UdDwEB\n/wQEAwIBpjANBgkqhkiG9w0BAQsFAAOCAQEACLdxWMlmr3drMvA7GaQArzlbe/ny\nx8mThDhZP6gx+yTJ6LXk8CFc7S23JXFZVquwcV5yFa0DavaodBI3RNWknx/Yu5Lm\nM7cOByu2IuJhcEu4o+ZntLZLb7heFMXMIf01lVkYpyYyvS/NvVdu9km8f6ZvxV9r\nDyTDDMjeh+hg5l2Wwc4P6UGoMlmOruUiunsb8hiDLhD+brYBHKHqJY9pCrzJQd0v\nWEkAOsBwaTv/POO0F4VDZSfA5CqjYOkppupw9nXXfJkk9PvKuDI1G2XO7pcW1PWh\nDdGK6Wz0AXMWWbbX8LToDrFA9q7YOxGNOVPhbHZ++bDJvLNmjrtruy3UTQ==\n-----END CERTIFICATE-----\n'
 
 
 
 ###  Inspect the Intermediate CA
 
     >>> intermediate.cert.subject_attrs
@@ -162,15 +185,15 @@
 
     >>> cert.subject_attrs.COMMON_NAME
     'example.com'
 
     >>> cert.public_key
     <cryptography.hazmat.backends.openssl.rsa._RSAPublicKey object at 0x10361c150>
 
-    >>> cert.public_key_pem
+    >>> cert.pem
     b'-----BEGIN CERTIFICATE-----\nMIIDITCCAgmgAwIBAgIUAx6AA8z3BqH/ICCmqOJXGI7PHCswDQYJKoZIhvcNAQEL\nBQAwEjEQMA4GA1UECgwHUm9vdCBDQTAeFw0yMzA1MDgwODU5NTlaFw0yMzA4MDcw\nODU5NTlaMBYxFDASBgNVBAMMC2V4YW1wbGUuY29tMIIBIjANBgkqhkiG9w0BAQEF\nAAOCAQ8AMIIBCgKCAQEAnWAlLvbR0hE8seqI8uBj8ESicJ/nF8I3KF9CFlTexQ73\nKdyqTRCoPZ6uuK0quX+qX5KeeNlWSnJRxSDc0WmLwYxWFVg6hmBDPLK1Ijntc1Uj\n4HENkolgPUBxgf9VBSmojqd1XL0o8PwGFIoyZ6Z/YTc3MqML4QZaB0m+TYlVgoJP\nQgFT9d9nQadvyswIx7nOMkT0Rd3sGl8nWaNgDaBLB6mkylGrtaiyo2M2LWKvNz69\nDWbjlccj65B04cBLwRcA2Zmx80leajX1zNWt0+dhJFo6rnLtmvIgqdLhCrNTmDMK\nrlyVsOrwJfXNreIPDEgYztZlrUdTnynmF4bW6W5KcwIDAQABo2swaTAdBgNVHQ4E\nFgQURd1r0d7XJBtT651AbuR2hg7TQBIwDAYDVR0TAQH/BAIwADAOBgNVHQ8BAf8E\nBAMCBaAwKgYDVR0lAQH/BCAwHgYIKwYBBQUHAwIGCCsGAQUFBwMBBggrBgEFBQcD\nAzANBgkqhkiG9w0BAQsFAAOCAQEANcFmZZkt4Z6jc069IOonGfcpUdnZieSEVyBE\nCQC+QWaHYqcD0ryYV8n1/UzNVcSkptQ5YrbgXNikV6+cuklFq4OjHlUDGOxchrkc\nSFGYAf+j7wAAx+OZWH5IwvMSTWGhfi7FWNFrzbO3JUE1q3OOnsIUmcDpd/8zucyE\njPf6F0MVujwMJq8VAH8UtUpVm1SApEBz9vgx0n7Z0l5fgRw7PMwwDkaoyplSC0VA\n7F7AUX3K0oJ7Gyw+9onfS090GMo6mlTfhtXNpPArleUUOTrp+TKVhwtz8GRRzxEW\nBE1OaNZaipKILZPbgDa5u67pRdU/OhuMFDsBh1GlPopcax+rCQ==\n-----END CERTIFICATE-----\n'
 
     >>> cert.SHA1
     '21B99CE5588417932ACB65C54398115C75240B04'
 
 
 
@@ -204,13 +227,10 @@
 
     >>> csr.subject_attrs.COMMON_NAME
     'example.com'
 
 [cryptography]: https://cryptography.io/en/latest/
 [trustme]: https://github.com/python-trio/trustme
 
-
-[cryptography]: https://cryptography.io/en/latest/
-[trustme]: https://github.com/python-trio/trustme
 [cnert.CA]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnertca
-[cnert._Cert]]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
+[cnert._Cert]: https://cnert.readthedocs.io/en/latest/cnert/#class-cnert_cert
```

