# Comparing `tmp/mse_lib_crypto-1.1.tar.gz` & `tmp/mse_lib_crypto-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_crypto-1.1.tar", last modified: Wed Feb  8 17:07:46 2023, max compression
+gzip compressed data, was "mse_lib_crypto-1.2.tar", last modified: Wed May 10 12:42:34 2023, max compression
```

## Comparing `mse_lib_crypto-1.1.tar` & `mse_lib_crypto-1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:07:46.724175 mse_lib_crypto-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-08 17:07:46.724175 mse_lib_crypto-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-08 17:07:46.724175 mse_lib_crypto-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:07:46.724175 mse_lib_crypto-1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:07:46.724175 mse_lib_crypto-1.1/src/mse_lib_crypto/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/src/mse_lib_crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/src/mse_lib_crypto/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/src/mse_lib_crypto/ed25519.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/src/mse_lib_crypto/error.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/src/mse_lib_crypto/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/src/mse_lib_crypto/seal_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/src/mse_lib_crypto/x25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/src/mse_lib_crypto/xsalsa20_poly1305.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:07:46.724175 mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-08 17:07:46.000000 mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-08 17:07:46.000000 mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 17:07:46.000000 mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 17:07:46.000000 mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-08 17:07:46.000000 mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-08 17:07:46.000000 mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:07:46.724175 mse_lib_crypto-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/tests/test_ed25519.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/tests/test_seal.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/tests/test_x25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-08 17:07:13.000000 mse_lib_crypto-1.1/tests/test_xsalsa20_poly1305.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:42:34.467814 mse_lib_crypto-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-10 12:42:34.467814 mse_lib_crypto-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 12:42:34.471814 mse_lib_crypto-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:42:34.467814 mse_lib_crypto-1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:42:34.467814 mse_lib_crypto-1.2/src/mse_lib_crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/src/mse_lib_crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/src/mse_lib_crypto/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/src/mse_lib_crypto/ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/src/mse_lib_crypto/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/src/mse_lib_crypto/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/src/mse_lib_crypto/seal_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/src/mse_lib_crypto/x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/src/mse_lib_crypto/xsalsa20_poly1305.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:42:34.467814 mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-10 12:42:34.000000 mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-10 12:42:34.000000 mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:42:34.000000 mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:42:34.000000 mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 12:42:34.000000 mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 12:42:34.000000 mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:42:34.467814 mse_lib_crypto-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/tests/test_ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/tests/test_seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/tests/test_x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-10 12:41:55.000000 mse_lib_crypto-1.2/tests/test_xsalsa20_poly1305.py
```

### Comparing `mse_lib_crypto-1.1/PKG-INFO` & `mse_lib_crypto-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_lib_crypto
-Version: 1.1
+Version: 1.2
 Summary: Cryptography Library for MicroService Encryption
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_crypto-1.1/setup.py` & `mse_lib_crypto-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     author_email="tech@cosmian.com",
     description="Cryptography Library for MicroService Encryption",
     packages=find_packages("src"),
     package_dir={"": "src"},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     zip_safe=False,
-    install_requires=["cryptography>=39.0.0,<40.0.0", "pynacl>=1.5.0,<2.0.0"],
+    install_requires=["cryptography>=40.0.2,<40.1.0", "pynacl>=1.5.0,<2.0.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     setup_requires=["wheel"],
     tests_require=["pytest>=7.2.0,<8.0.0"],
```

### Comparing `mse_lib_crypto-1.1/src/mse_lib_crypto/conversion.py` & `mse_lib_crypto-1.2/src/mse_lib_crypto/conversion.py`

 * *Files identical despite different names*

### Comparing `mse_lib_crypto-1.1/src/mse_lib_crypto/ed25519.py` & `mse_lib_crypto-1.2/src/mse_lib_crypto/ed25519.py`

 * *Files identical despite different names*

### Comparing `mse_lib_crypto-1.1/src/mse_lib_crypto/seal_box.py` & `mse_lib_crypto-1.2/src/mse_lib_crypto/seal_box.py`

 * *Files identical despite different names*

### Comparing `mse_lib_crypto-1.1/src/mse_lib_crypto/x25519.py` & `mse_lib_crypto-1.2/src/mse_lib_crypto/x25519.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     """
     private_key: PrivateKey = PrivateKey.generate()
     public_key: PublicKey = private_key.public_key
 
     return bytes(public_key), bytes(private_key)
 
 
+def x25519_pk_from_sk(private_key: bytes) -> bytes:
+    """X25519 public key from `private_key`."""
+    return bytes(PrivateKey(private_key).public_key)
+
+
 def x25519(private_key: bytes, public_key: bytes) -> bytes:
     """Scalar multiplication over Curve25519.
 
     Parameters
     ----------
     private_key: bytes
         Scalar to be used as private key.
```

### Comparing `mse_lib_crypto-1.1/src/mse_lib_crypto/xsalsa20_poly1305.py` & `mse_lib_crypto-1.2/src/mse_lib_crypto/xsalsa20_poly1305.py`

 * *Files identical despite different names*

### Comparing `mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/PKG-INFO` & `mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-lib-crypto
-Version: 1.1
+Version: 1.2
 Summary: Cryptography Library for MicroService Encryption
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_crypto-1.1/src/mse_lib_crypto.egg-info/SOURCES.txt` & `mse_lib_crypto-1.2/src/mse_lib_crypto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_lib_crypto-1.1/tests/test_xsalsa20_poly1305.py` & `mse_lib_crypto-1.2/tests/test_xsalsa20_poly1305.py`

 * *Files identical despite different names*

