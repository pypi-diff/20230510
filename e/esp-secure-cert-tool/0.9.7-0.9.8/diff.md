# Comparing `tmp/esp-secure-cert-tool-0.9.7.tar.gz` & `tmp/esp-secure-cert-tool-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-secure-cert-tool-0.9.7.tar", last modified: Tue Mar 28 05:46:07 2023, max compression
+gzip compressed data, was "dist/esp-secure-cert-tool-0.9.8.tar", last modified: Wed May 10 15:42:53 2023, max compression
```

## Comparing `esp-secure-cert-tool-0.9.7.tar` & `esp-secure-cert-tool-0.9.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/configure_esp_secure_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert/configure_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert/custflash_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert/esp_secure_cert_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert/nvs_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert/tlv_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/esp_secure_cert_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 05:46:07.000000 esp-secure-cert-tool-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-03-28 05:45:53.000000 esp-secure-cert-tool-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/configure_esp_secure_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/configure_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/custflash_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/esp_secure_cert_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/nvs_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert/tlv_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:42:53.000000 esp-secure-cert-tool-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-10 15:42:41.000000 esp-secure-cert-tool-0.9.8/setup.py
```

### Comparing `esp-secure-cert-tool-0.9.7/LICENSE` & `esp-secure-cert-tool-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.7/PKG-INFO` & `esp-secure-cert-tool-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-secure-cert-tool
-Version: 0.9.7
+Version: 0.9.8
 Summary: A python utility which helps to configure and provisionthe ESP platform with PKI credentials into the esp_secure_cert partition
 Home-page: https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/README.md
 Project-URL: Source, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/configure_esp_secure_cert.py
```

### Comparing `esp-secure-cert-tool-0.9.7/README.md` & `esp-secure-cert-tool-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.7/configure_esp_secure_cert.py` & `esp-secure-cert-tool-0.9.8/configure_esp_secure_cert.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.7/esp_secure_cert/configure_ds.py` & `esp-secure-cert-tool-0.9.8/esp_secure_cert/configure_ds.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.7/esp_secure_cert/custflash_format.py` & `esp-secure-cert-tool-0.9.8/esp_secure_cert/custflash_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.7/esp_secure_cert/esp_secure_cert_helper.py` & `esp-secure-cert-tool-0.9.8/esp_secure_cert/esp_secure_cert_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,25 @@
             key = key_file.read()
     except FileNotFoundError:
         raise FileNotFoundError(f"Key file not found: {key_file_path}")
 
     try:
         # Attempt to load the key as a PEM-encoded private key
         private_key = serialization.load_pem_private_key(key, password=password, backend=default_backend())
-        result["encoding"] = serialization.Encoding.PEM
+        result["encoding"] = serialization.Encoding.PEM.value
         result["bytes"] = private_key.private_bytes(encoding=serialization.Encoding.PEM,
                                                     format=serialization.PrivateFormat.TraditionalOpenSSL,
                                                     encryption_algorithm=serialization.NoEncryption())
         return result
     except ValueError:
         pass
 
     try:
         private_key = serialization.load_der_private_key(key, password=password, backend=default_backend())
-        result["encoding"] = serialization.Encoding.DER
+        result["encoding"] = serialization.Encoding.DER.value
         result["bytes"] = private_key.private_bytes(encoding=serialization.Encoding.DER,
                                                     format=serialization.PrivateFormat.TraditionalOpenSSL,
                                                     encryption_algorithm=serialization.NoEncryption())
         return result
     except ValueError:
         raise ValueError("Unsupported key encoding format, Please provide PEM or DER encoded key")
 
@@ -73,21 +73,21 @@
         with open(cert_file_path, "rb") as cert_file:
             cert_data = cert_file.read()
     except FileNotFoundError:
         raise FileNotFoundError(f"Cert file not found: {cert_file_path}")
 
     try:
         cert = load_pem_x509_certificate(cert_data, backend=default_backend())
-        result["encoding"] = serialization.Encoding.PEM
+        result["encoding"] = serialization.Encoding.PEM.value
         result["bytes"] = cert.public_bytes(encoding=serialization.Encoding.PEM)
         return result
     except ValueError:
         pass
 
     try:
         cert = load_der_x509_certificate(cert_data, backend=default_backend())
-        result["encoding"] = serialization.Encoding.DER
+        result["encoding"] = serialization.Encoding.DER.value
         result["bytes"] = cert.public_bytes(encoding=serialization.Encoding.DER)
         return result
     except ValueError:
         raise ValueError("Unsupported certificate encoding format, Please provide PEM or DER encoded certificate")
```

### Comparing `esp-secure-cert-tool-0.9.7/esp_secure_cert/nvs_format.py` & `esp-secure-cert-tool-0.9.8/esp_secure_cert/nvs_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.7/esp_secure_cert/tlv_format.py` & `esp-secure-cert-tool-0.9.8/esp_secure_cert/tlv_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-0.9.7/esp_secure_cert_tool.egg-info/PKG-INFO` & `esp-secure-cert-tool-0.9.8/esp_secure_cert_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-secure-cert-tool
-Version: 0.9.7
+Version: 0.9.8
 Summary: A python utility which helps to configure and provisionthe ESP platform with PKI credentials into the esp_secure_cert partition
 Home-page: https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/README.md
 Project-URL: Source, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/configure_esp_secure_cert.py
```

### Comparing `esp-secure-cert-tool-0.9.7/setup.py` & `esp-secure-cert-tool-0.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     print(
         "Package setuptools is missing from your Python installation. "
         "Please see the installation section in the esp-secure-cert-tool "
         "documentation for instructions on how to install it."
     )
     exit(1)
 
-VERSION = "0.9.7"
+VERSION = "0.9.8"
 
 long_description = """
 ====================
 esp-secure-cert-tool
 ====================
 The python utility helps to configure and provision the device with
 PKI credentials to generate the esp_secure_cert partition.
```

