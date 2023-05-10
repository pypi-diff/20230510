# Comparing `tmp/pymongocrypt-1.5.2.tar.gz` & `tmp/pymongocrypt-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongocrypt-1.5.2.tar", last modified: Wed Apr 12 21:57:19 2023, max compression
+gzip compressed data, was "pymongocrypt-1.6.0.tar", last modified: Wed May 10 18:44:23 2023, max compression
```

## Comparing `pymongocrypt-1.5.2.tar` & `pymongocrypt-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-04-12 21:57:19.230714 pymongocrypt-1.5.2/
--rw-r--r--   0 mci        (500) admin       (80)    11357 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/LICENSE
--rw-r--r--   0 mci        (500) admin       (80)     8823 2023-04-12 21:57:19.230465 pymongocrypt-1.5.2/PKG-INFO
--rw-r--r--   0 mci        (500) admin       (80)     7381 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/README.rst
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-04-12 21:57:19.228023 pymongocrypt-1.5.2/pymongocrypt/
--rw-r--r--   0 mci        (500) admin       (80)      687 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/__init__.py
--rw-r--r--   0 mci        (500) admin       (80)     2053 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/auto_encrypter.py
--rw-r--r--   0 mci        (500) admin       (80)     3156 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/binary.py
--rw-r--r--   0 mci        (500) admin       (80)    56936 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/binding.py
--rw-r--r--   0 mci        (500) admin       (80)     2073 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/compat.py
--rw-r--r--   0 mci        (500) admin       (80)     5119 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/credentials.py
--rw-r--r--   0 mci        (500) admin       (80)     6157 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/crypto.py
--rw-r--r--   0 mci        (500) admin       (80)     1393 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/errors.py
--rw-r--r--   0 mci        (500) admin       (80)    11125 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/explicit_encrypter.py
--rw-r--r--   0 mci        (500) admin       (80)    32890 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/mongocrypt.py
--rw-r--r--   0 mci        (500) admin       (80)     4850 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/state_machine.py
--rw-r--r--   0 mci        (500) admin       (80)      642 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/pymongocrypt/version.py
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-04-12 21:57:19.229454 pymongocrypt-1.5.2/pymongocrypt.egg-info/
--rw-r--r--   0 mci        (500) admin       (80)     8823 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/PKG-INFO
--rw-r--r--   0 mci        (500) admin       (80)      622 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/SOURCES.txt
--rw-r--r--   0 mci        (500) admin       (80)        1 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/dependency_links.txt
--rw-r--r--   0 mci        (500) admin       (80)        1 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/not-zip-safe
--rw-r--r--   0 mci        (500) admin       (80)      148 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/requires.txt
--rw-r--r--   0 mci        (500) admin       (80)       13 2023-04-12 21:57:19.000000 pymongocrypt-1.5.2/pymongocrypt.egg-info/top_level.txt
--rw-r--r--   0 mci        (500) admin       (80)       38 2023-04-12 21:57:19.230773 pymongocrypt-1.5.2/setup.cfg
--rw-r--r--   0 mci        (500) admin       (80)     3560 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/setup.py
-drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-04-12 21:57:19.230132 pymongocrypt-1.5.2/test/
--rw-r--r--   0 mci        (500) admin       (80)     2398 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/test/test_binding.py
--rw-r--r--   0 mci        (500) admin       (80)     3479 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/test/test_crypto.py
--rw-r--r--   0 mci        (500) admin       (80)    35775 2023-04-12 21:57:15.000000 pymongocrypt-1.5.2/test/test_mongocrypt.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-05-10 18:44:23.959134 pymongocrypt-1.6.0/
+-rw-r--r--   0 mci        (500) admin       (80)    11357 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/LICENSE
+-rw-r--r--   0 mci        (500) admin       (80)     8580 2023-05-10 18:44:23.958857 pymongocrypt-1.6.0/PKG-INFO
+-rw-r--r--   0 mci        (500) admin       (80)     7362 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/README.rst
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-05-10 18:44:23.956191 pymongocrypt-1.6.0/pymongocrypt/
+-rw-r--r--   0 mci        (500) admin       (80)      687 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/__init__.py
+-rw-r--r--   0 mci        (500) admin       (80)     2053 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/auto_encrypter.py
+-rw-r--r--   0 mci        (500) admin       (80)     3156 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/binary.py
+-rw-r--r--   0 mci        (500) admin       (80)    55615 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/binding.py
+-rw-r--r--   0 mci        (500) admin       (80)     1027 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/compat.py
+-rw-r--r--   0 mci        (500) admin       (80)     5119 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/credentials.py
+-rw-r--r--   0 mci        (500) admin       (80)     6157 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/crypto.py
+-rw-r--r--   0 mci        (500) admin       (80)     1393 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/errors.py
+-rw-r--r--   0 mci        (500) admin       (80)    11125 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/explicit_encrypter.py
+-rw-r--r--   0 mci        (500) admin       (80)    32003 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/mongocrypt.py
+-rw-r--r--   0 mci        (500) admin       (80)     4850 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/state_machine.py
+-rw-r--r--   0 mci        (500) admin       (80)      642 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/pymongocrypt/version.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-05-10 18:44:23.957777 pymongocrypt-1.6.0/pymongocrypt.egg-info/
+-rw-r--r--   0 mci        (500) admin       (80)     8580 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/PKG-INFO
+-rw-r--r--   0 mci        (500) admin       (80)      622 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 mci        (500) admin       (80)        1 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 mci        (500) admin       (80)        1 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/not-zip-safe
+-rw-r--r--   0 mci        (500) admin       (80)      148 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/requires.txt
+-rw-r--r--   0 mci        (500) admin       (80)       13 2023-05-10 18:44:23.000000 pymongocrypt-1.6.0/pymongocrypt.egg-info/top_level.txt
+-rw-r--r--   0 mci        (500) admin       (80)       38 2023-05-10 18:44:23.959192 pymongocrypt-1.6.0/setup.cfg
+-rw-r--r--   0 mci        (500) admin       (80)     3439 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/setup.py
+drwxr-xr-x   0 mci        (500) admin       (80)        0 2023-05-10 18:44:23.958539 pymongocrypt-1.6.0/test/
+-rw-r--r--   0 mci        (500) admin       (80)     2398 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/test/test_binding.py
+-rw-r--r--   0 mci        (500) admin       (80)     3479 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/test/test_crypto.py
+-rw-r--r--   0 mci        (500) admin       (80)    35736 2023-05-10 18:44:21.000000 pymongocrypt-1.6.0/test/test_mongocrypt.py
```

### Comparing `pymongocrypt-1.5.2/LICENSE` & `pymongocrypt-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/PKG-INFO` & `pymongocrypt-1.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: pymongocrypt
-Version: 1.5.2
+Version: 1.6.0
 Summary: Python bindings for libmongocrypt
 Home-page: https://github.com/mongodb/libmongocrypt/tree/master/bindings/python
 Author: Shane Harvey
 Author-email: mongodb-user@googlegroups.com
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,pymongocrypt,pymongo,mongocrypt,bson
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+Requires-Python: >=3.7
 License-File: LICENSE
 
 ============
 PyMongoCrypt
 ============
 :Info: Python bindings for libmongocrypt. See
        `GitHub <https://github.com/mongodb/libmongocrypt/tree/master/bindings/python>`_
@@ -41,15 +37,15 @@
 About
 =====
 
 Python wrapper library for libmongocrypt that supports client side encryption
 in drivers. PyMongoCrypt uses `cffi <https://pypi.org/project/cffi/>`_ and
 `cryptography <https://pypi.org/project/cryptography/>`_.
 
-PyMongoCrypt supports Python 2.7, 3.4+, and PyPy3.5+.
+PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 Support / Feedback
 ==================
 
 For issues with, questions about, or feedback for PyMongoCrypt, please look into
 our `support channels <http://www.mongodb.org/about/support>`_. Please
 do not email any of the PyMongoCrypt developers directly with issues or
@@ -173,15 +169,15 @@
   $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/rhel-62-64-bit/nocrypto/lib64/libmongocrypt.so
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
   1.2.1
 
 Dependencies
 ============
 
-PyMongoCrypt supports CPython 2.7, 3.4+, PyPy, and PyPy3.5+.
+PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 PyMongoCrypt requires `cffi <https://pypi.org/project/cffi/>`_ and
 `cryptography <https://pypi.org/project/cryptography/>`_.
 
 If not installed using one of the official wheels, PyMongoCrypt also requires
 libmongocrypt to be installed on your system. If libmongocrypt is not
 installed you will see an error like this:
```

### Comparing `pymongocrypt-1.5.2/README.rst` & `pymongocrypt-1.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 About
 =====
 
 Python wrapper library for libmongocrypt that supports client side encryption
 in drivers. PyMongoCrypt uses `cffi <https://pypi.org/project/cffi/>`_ and
 `cryptography <https://pypi.org/project/cryptography/>`_.
 
-PyMongoCrypt supports Python 2.7, 3.4+, and PyPy3.5+.
+PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 Support / Feedback
 ==================
 
 For issues with, questions about, or feedback for PyMongoCrypt, please look into
 our `support channels <http://www.mongodb.org/about/support>`_. Please
 do not email any of the PyMongoCrypt developers directly with issues or
@@ -141,15 +141,15 @@
   $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/rhel-62-64-bit/nocrypto/lib64/libmongocrypt.so
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
   1.2.1
 
 Dependencies
 ============
 
-PyMongoCrypt supports CPython 2.7, 3.4+, PyPy, and PyPy3.5+.
+PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 PyMongoCrypt requires `cffi <https://pypi.org/project/cffi/>`_ and
 `cryptography <https://pypi.org/project/cryptography/>`_.
 
 If not installed using one of the official wheels, PyMongoCrypt also requires
 libmongocrypt to be installed on your system. If libmongocrypt is not
 installed you will see an error like this:
```

### Comparing `pymongocrypt-1.5.2/pymongocrypt/__init__.py` & `pymongocrypt-1.6.0/pymongocrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/pymongocrypt/auto_encrypter.py` & `pymongocrypt-1.6.0/pymongocrypt/auto_encrypter.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/pymongocrypt/binary.py` & `pymongocrypt-1.6.0/pymongocrypt/binary.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/pymongocrypt/binding.py` & `pymongocrypt-1.6.0/pymongocrypt/binding.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,15 @@
 
 /**
  * Returns the version string for libmongocrypt.
  *
  * @param[out] len  An optional length of the returned string. May be NULL.
  * @returns a NULL terminated version string for libmongocrypt.
  */
-const char *
-mongocrypt_version (uint32_t *len);
+const char *mongocrypt_version(uint32_t *len);
 
 /**
  * A non-owning view of a byte buffer.
  *
  * When constructing a mongocrypt_binary_t it is the responsibility of the
  * caller to maintain the lifetime of the viewed data. However, all public
  * functions that take a mongocrypt_binary_t as an argument will make a copy of
@@ -95,58 +94,53 @@
 /**
  * Create a new non-owning view of a buffer (data + length).
  *
  * Use this to create a mongocrypt_binary_t used for output parameters.
  *
  * @returns A new mongocrypt_binary_t.
  */
-mongocrypt_binary_t *
-mongocrypt_binary_new (void);
+mongocrypt_binary_t *mongocrypt_binary_new(void);
 
 /**
  * Create a new non-owning view of a buffer (data + length).
  *
  * @param[in] data A pointer to an array of bytes. This data is not copied. @p
  * data must outlive the binary object.
  * @param[in] len The length of the @p data byte array.
  *
  * @returns A new @ref mongocrypt_binary_t.
  */
-mongocrypt_binary_t *
-mongocrypt_binary_new_from_data (uint8_t *data, uint32_t len);
+mongocrypt_binary_t *mongocrypt_binary_new_from_data(uint8_t *data, uint32_t len);
 
 /**
  * Get a pointer to the viewed data.
  *
  * @param[in] binary The @ref mongocrypt_binary_t.
  *
  * @returns A pointer to the viewed data.
  */
-uint8_t *
-mongocrypt_binary_data (const mongocrypt_binary_t *binary);
+uint8_t *mongocrypt_binary_data(const mongocrypt_binary_t *binary);
 
 /**
  * Get the length of the viewed data.
  *
  * @param[in] binary The @ref mongocrypt_binary_t.
  *
  * @returns The length of the viewed data.
  */
-uint32_t
-mongocrypt_binary_len (const mongocrypt_binary_t *binary);
+uint32_t mongocrypt_binary_len(const mongocrypt_binary_t *binary);
 
 /**
  * Free the @ref mongocrypt_binary_t.
  *
  * This does not free the viewed data.
  *
  * @param[in] binary The mongocrypt_binary_t destroy.
  */
-void
-mongocrypt_binary_destroy (mongocrypt_binary_t *binary);
+void mongocrypt_binary_destroy(mongocrypt_binary_t *binary);
 
 /**
  * Indicates success or contains error information.
  *
  * Functions like @ref mongocrypt_ctx_encrypt_init follow a pattern to expose a
  * status. A boolean is returned. True indicates success, and false indicates
  * failure. On failure a status on the handle is set, and is accessible with a
@@ -154,31 +148,30 @@
  */
 typedef struct _mongocrypt_status_t mongocrypt_status_t;
 
 /**
  * Indicates the type of error.
  */
 typedef enum {
-   MONGOCRYPT_STATUS_OK = 0,
-   MONGOCRYPT_STATUS_ERROR_CLIENT = 1,
-   MONGOCRYPT_STATUS_ERROR_KMS = 2,
-   MONGOCRYPT_STATUS_ERROR_CRYPT_SHARED = 3,
+    MONGOCRYPT_STATUS_OK = 0,
+    MONGOCRYPT_STATUS_ERROR_CLIENT = 1,
+    MONGOCRYPT_STATUS_ERROR_KMS = 2,
+    MONGOCRYPT_STATUS_ERROR_CRYPT_SHARED = 3,
 } mongocrypt_status_type_t;
 
 /**
  * Create a new status object.
  *
  * Use a new status object to retrieve the status from a handle by passing
  * this as an out-parameter to functions like @ref mongocrypt_ctx_status.
  * When done, destroy it with @ref mongocrypt_status_destroy.
  *
  * @returns A new status object.
  */
-mongocrypt_status_t *
-mongocrypt_status_new (void);
+mongocrypt_status_t *mongocrypt_status_new(void);
 
 /**
  * Set a status object with message, type, and code.
  *
  * Use this to set the @ref mongocrypt_status_t given in the crypto hooks.
  *
  * @param[in] type The status type.
@@ -188,96 +181,87 @@
  * of @p message (which differs from other functions accepting string
  * arguments).
  * Alternatively, if message is NULL terminated this may be -1 to tell
  * mongocrypt
  * to determine the string's length with strlen.
  *
  */
-void
-mongocrypt_status_set (mongocrypt_status_t *status,
-                       mongocrypt_status_type_t type,
-                       uint32_t code,
-                       const char *message,
-                       int32_t message_len);
+void mongocrypt_status_set(mongocrypt_status_t *status,
+                           mongocrypt_status_type_t type,
+                           uint32_t code,
+                           const char *message,
+                           int32_t message_len);
 
 /**
  * Indicates success or the type of error.
  *
  * @param[in] status The status object.
  *
  * @returns A @ref mongocrypt_status_type_t.
  */
-mongocrypt_status_type_t
-mongocrypt_status_type (mongocrypt_status_t *status);
+mongocrypt_status_type_t mongocrypt_status_type(mongocrypt_status_t *status);
 
 /**
  * Get an error code or 0.
  *
  * @param[in] status The status object.
  *
  * @returns An error code.
  */
-uint32_t
-mongocrypt_status_code (mongocrypt_status_t *status);
+uint32_t mongocrypt_status_code(mongocrypt_status_t *status);
 
 /**
  * Get the error message associated with a status or NULL.
  *
  * @param[in] status The status object.
  * @param[out] len An optional length of the returned string (excluding the
  * trailing NULL byte). May be NULL.
  *
  * @returns A NULL terminated error message or NULL.
  */
-const char *
-mongocrypt_status_message (mongocrypt_status_t *status, uint32_t *len);
+const char *mongocrypt_status_message(mongocrypt_status_t *status, uint32_t *len);
 
 /**
  * Returns true if the status indicates success.
  *
  * @param[in] status The status to check.
  *
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_status_ok (mongocrypt_status_t *status);
+bool mongocrypt_status_ok(mongocrypt_status_t *status);
 
 /**
  * Free the memory for a status object.
  *
  * @param[in] status The status to destroy.
  */
-void
-mongocrypt_status_destroy (mongocrypt_status_t *status);
+void mongocrypt_status_destroy(mongocrypt_status_t *status);
 
 /**
  * Indicates the type of log message.
  */
 typedef enum {
-   MONGOCRYPT_LOG_LEVEL_FATAL = 0,
-   MONGOCRYPT_LOG_LEVEL_ERROR = 1,
-   MONGOCRYPT_LOG_LEVEL_WARNING = 2,
-   MONGOCRYPT_LOG_LEVEL_INFO = 3,
-   MONGOCRYPT_LOG_LEVEL_TRACE = 4
+    MONGOCRYPT_LOG_LEVEL_FATAL = 0,
+    MONGOCRYPT_LOG_LEVEL_ERROR = 1,
+    MONGOCRYPT_LOG_LEVEL_WARNING = 2,
+    MONGOCRYPT_LOG_LEVEL_INFO = 3,
+    MONGOCRYPT_LOG_LEVEL_TRACE = 4
 } mongocrypt_log_level_t;
 
 /**
  * A log callback function. Set a custom log callback with @ref
  * mongocrypt_setopt_log_handler.
  *
  * @param[in] message A NULL terminated message.
  * @param[in] message_len The length of message.
  * @param[in] ctx A context provided by the caller of @ref
  * mongocrypt_setopt_log_handler.
  */
-typedef void (*mongocrypt_log_fn_t) (mongocrypt_log_level_t level,
-                                     const char *message,
-                                     uint32_t message_len,
-                                     void *ctx);
+typedef void (*mongocrypt_log_fn_t)(mongocrypt_log_level_t level, const char *message, uint32_t message_len, void *ctx);
 
 /**
  * The top-level handle to libmongocrypt.
  *
  * Create a mongocrypt_t handle to perform operations within libmongocrypt:
  * encryption, decryption, registering log callbacks, etc.
  *
@@ -294,33 +278,29 @@
  *
  * Set options using mongocrypt_setopt_* functions, then initialize with @ref
  * mongocrypt_init. When done with the @ref mongocrypt_t, free with @ref
  * mongocrypt_destroy.
  *
  * @returns A new @ref mongocrypt_t object.
  */
-mongocrypt_t *
-mongocrypt_new (void);
+mongocrypt_t *mongocrypt_new(void);
 
 /**
  * Set a handler on the @ref mongocrypt_t object to get called on every log
  * message.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
  * @param[in] log_fn The log callback.
  * @param[in] log_ctx A context passed as an argument to the log callback every
  * invocation.
  * @pre @ref mongocrypt_init has not been called on @p crypt.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_setopt_log_handler (mongocrypt_t *crypt,
-                               mongocrypt_log_fn_t log_fn,
-                               void *log_ctx);
+bool mongocrypt_setopt_log_handler(mongocrypt_t *crypt, mongocrypt_log_fn_t log_fn, void *log_ctx);
 
 /**
  * Configure an AWS KMS provider on the @ref mongocrypt_t object.
  *
  * This has been superseded by the more flexible:
  * @ref mongocrypt_setopt_kms_providers
  *
@@ -335,20 +315,19 @@
  * @param[in] aws_secret_access_key_len The string length (in bytes) of @p
  * aws_secret_access_key. Pass -1 to determine the string length with strlen
  * (must be NULL terminated).
  * @pre @ref mongocrypt_init has not been called on @p crypt.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_setopt_kms_provider_aws (mongocrypt_t *crypt,
-                                    const char *aws_access_key_id,
-                                    int32_t aws_access_key_id_len,
-                                    const char *aws_secret_access_key,
-                                    int32_t aws_secret_access_key_len);
+bool mongocrypt_setopt_kms_provider_aws(mongocrypt_t *crypt,
+                                        const char *aws_access_key_id,
+                                        int32_t aws_access_key_id_len,
+                                        const char *aws_secret_access_key,
+                                        int32_t aws_secret_access_key_len);
 
 /**
  * Configure a local KMS provider on the @ref mongocrypt_t object.
  *
  * This has been superseded by the more flexible:
  * @ref mongocrypt_setopt_kms_providers
  *
@@ -356,64 +335,56 @@
  * @param[in] key A 96 byte master key used to encrypt and decrypt key vault
  * keys. The viewed data is copied. It is valid to destroy @p key with @ref
  * mongocrypt_binary_destroy immediately after.
  * @pre @ref mongocrypt_init has not been called on @p crypt.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_setopt_kms_provider_local (mongocrypt_t *crypt,
-                                      mongocrypt_binary_t *key);
+bool mongocrypt_setopt_kms_provider_local(mongocrypt_t *crypt, mongocrypt_binary_t *key);
 
 /**
  * Configure KMS providers with a BSON document.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
  * @param[in] kms_providers A BSON document mapping the KMS provider names
  * to credentials. Set a KMS provider value to an empty document to supply
  * credentials on-demand with @ref mongocrypt_ctx_provide_kms_providers.
  * @pre @ref mongocrypt_init has not been called on @p crypt.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_setopt_kms_providers (mongocrypt_t *crypt,
-                                 mongocrypt_binary_t *kms_providers);
+bool mongocrypt_setopt_kms_providers(mongocrypt_t *crypt, mongocrypt_binary_t *kms_providers);
 
 /**
  * Set a local schema map for encryption.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
  * @param[in] schema_map A BSON document representing the schema map supplied by
  * the user. The keys are collection namespaces and values are JSON schemas. The
  * viewed data copied. It is valid to destroy @p schema_map with @ref
  * mongocrypt_binary_destroy immediately after.
  * @pre @p crypt has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_status
  */
-bool
-mongocrypt_setopt_schema_map (mongocrypt_t *crypt,
-                              mongocrypt_binary_t *schema_map);
+bool mongocrypt_setopt_schema_map(mongocrypt_t *crypt, mongocrypt_binary_t *schema_map);
 
 /**
  * Set a local EncryptedFieldConfigMap for encryption.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
  * @param[in] efc_map A BSON document representing the EncryptedFieldConfigMap
  * supplied by the user. The keys are collection namespaces and values are
  * EncryptedFieldConfigMap documents. The viewed data copied. It is valid to
  * destroy @p efc_map with @ref mongocrypt_binary_destroy immediately after.
  * @pre @p crypt has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_status
  */
-bool
-mongocrypt_setopt_encrypted_field_config_map (mongocrypt_t *crypt,
-                                              mongocrypt_binary_t *efc_map);
+bool mongocrypt_setopt_encrypted_field_config_map(mongocrypt_t *crypt, mongocrypt_binary_t *efc_map);
 
 /**
  * @brief Append an additional search directory to the search path for loading
  * the crypt_shared dynamic library.
  *
  * @param[in] crypt The @ref mongocrypt_t object to update
  * @param[in] path A null-terminated sequence of bytes for the search path. On
@@ -435,17 +406,15 @@
  * the library wasn't found otherwise. If one does not ever append "$SYSTEM",
  * then the system's library-search mechanism will never be consulted.
  *
  * @note If an absolute path to the library is specified using
  * @ref mongocrypt_setopt_set_crypt_shared_lib_path_override, then paths
  * appended here will have no effect.
  */
-void
-mongocrypt_setopt_append_crypt_shared_lib_search_path (mongocrypt_t *crypt,
-                                                       const char *path);
+void mongocrypt_setopt_append_crypt_shared_lib_search_path(mongocrypt_t *crypt, const char *path);
 
 /**
  * @brief Set a single override path for loading the crypt_shared dynamic
  * library.
  *
  * @param[in] crypt The @ref mongocrypt_t object to update
  * @param[in] path A null-terminated sequence of bytes for a path to the
@@ -462,17 +431,15 @@
  * paths given to @ref mongocrypt_setopt_append_crypt_shared_lib_search_path
  * will be consulted when opening the crypt_shared library.
  *
  * @note If a path is provided via this API and @ref mongocrypt_init fails to
  * initialize a valid crypt_shared library instance for the path specified, then
  * the initialization of mongocrypt_t will fail with an error.
  */
-void
-mongocrypt_setopt_set_crypt_shared_lib_path_override (mongocrypt_t *crypt,
-                                                      const char *path);
+void mongocrypt_setopt_set_crypt_shared_lib_path_override(mongocrypt_t *crypt, const char *path);
 
 /**
  * @brief Opt-into handling the MONGOCRYPT_CTX_NEED_KMS_CREDENTIALS state.
  *
  * If set, before entering the MONGOCRYPT_CTX_NEED_KMS state,
  * contexts may enter the MONGOCRYPT_CTX_NEED_KMS_CREDENTIALS state
  * and then wait for credentials to be supplied through
@@ -480,52 +447,48 @@
  *
  * A context will only enter MONGOCRYPT_CTX_NEED_KMS_CREDENTIALS
  * if an empty document was set for a KMS provider in @ref
  * mongocrypt_setopt_kms_providers.
  *
  * @param[in] crypt The @ref mongocrypt_t object to update
  */
-void
-mongocrypt_setopt_use_need_kms_credentials_state (mongocrypt_t *crypt);
+void mongocrypt_setopt_use_need_kms_credentials_state(mongocrypt_t *crypt);
 
 /**
  * Initialize new @ref mongocrypt_t object.
  *
  * Set options before using @ref mongocrypt_setopt_kms_provider_local, @ref
  * mongocrypt_setopt_kms_provider_aws, or @ref mongocrypt_setopt_log_handler.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
  *
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status Failure may occur if previously
  * set
  * options are invalid.
  */
-bool
-mongocrypt_init (mongocrypt_t *crypt);
+bool mongocrypt_init(mongocrypt_t *crypt);
 
 /**
  * Get the status associated with a @ref mongocrypt_t object.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
  * @param[out] status Receives the status.
  *
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_status (mongocrypt_t *crypt, mongocrypt_status_t *status);
+bool mongocrypt_status(mongocrypt_t *crypt, mongocrypt_status_t *status);
 
 /**
  * Destroy the @ref mongocrypt_t object.
  *
  * @param[in] crypt The @ref mongocrypt_t object to destroy.
  */
-void
-mongocrypt_destroy (mongocrypt_t *crypt);
+void mongocrypt_destroy(mongocrypt_t *crypt);
 
 /**
  * Obtain a nul-terminated version string of the loaded crypt_shared dynamic
  * library, if available.
  *
  * If no crypt_shared was successfully loaded, this function returns NULL.
  *
@@ -537,17 +500,15 @@
  *
  * @return A nul-terminated string of the dynamically loaded crypt_shared
  * library.
  *
  * @note For a numeric value that can be compared against, use
  * @ref mongocrypt_crypt_shared_lib_version.
  */
-const char *
-mongocrypt_crypt_shared_lib_version_string (const mongocrypt_t *crypt,
-                                            uint32_t *len);
+const char *mongocrypt_crypt_shared_lib_version_string(const mongocrypt_t *crypt, uint32_t *len);
 
 /**
  * @brief Obtain a 64-bit constant encoding the version of the loaded
  * crypt_shared library, if available.
  *
  * @param[in] crypt The mongocrypt_t object after a successul call to
  * mongocrypt_init.
@@ -560,16 +521,15 @@
  * - Major version
  * - Minor version
  * - Revision
  * - Reserved
  *
  * For example, version 6.2.1 would be encoded as: 0x0006'0002'0001'0000
  */
-uint64_t
-mongocrypt_crypt_shared_lib_version (const mongocrypt_t *crypt);
+uint64_t mongocrypt_crypt_shared_lib_version(const mongocrypt_t *crypt);
 
 /**
  * Manages the state machine for encryption or decryption.
  */
 typedef struct _mongocrypt_ctx_t mongocrypt_ctx_t;
 
 /**
@@ -577,30 +537,28 @@
  *
  * Initialize the context with functions like @ref mongocrypt_ctx_encrypt_init.
  * When done, destroy it with @ref mongocrypt_ctx_destroy.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
  * @returns A new context.
  */
-mongocrypt_ctx_t *
-mongocrypt_ctx_new (mongocrypt_t *crypt);
+mongocrypt_ctx_t *mongocrypt_ctx_new(mongocrypt_t *crypt);
 
 /**
  * Get the status associated with a @ref mongocrypt_ctx_t object.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[out] status Receives the status.
  *
  * @returns True if the output is an ok status, false if it is an error
  * status.
  *
  * @see mongocrypt_status_ok
  */
-bool
-mongocrypt_ctx_status (mongocrypt_ctx_t *ctx, mongocrypt_status_t *status);
+bool mongocrypt_ctx_status(mongocrypt_ctx_t *ctx, mongocrypt_status_t *status);
 
 /**
  * Set the key id to use for explicit encryption.
  *
  * It is an error to set both this and the key alt name.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
@@ -608,17 +566,15 @@
  * key to use from the key vault collection. Note, the UUID must be encoded with
  * RFC-4122 byte order. The viewed data is copied. It is valid to destroy
  * @p key_id with @ref mongocrypt_binary_destroy immediately after.
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_key_id (mongocrypt_ctx_t *ctx,
-                              mongocrypt_binary_t *key_id);
+bool mongocrypt_ctx_setopt_key_id(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *key_id);
 
 /**
  * Set the keyAltName to use for explicit encryption or
  * data key creation.
  *
  * Pass the binary encoding a BSON document like the following:
  *
@@ -634,17 +590,15 @@
  * @param[in] key_alt_name The name to use. The viewed data is copied. It is
  * valid to destroy @p key_alt_name with @ref mongocrypt_binary_destroy
  * immediately after.
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_key_alt_name (mongocrypt_ctx_t *ctx,
-                                    mongocrypt_binary_t *key_alt_name);
+bool mongocrypt_ctx_setopt_key_alt_name(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *key_alt_name);
 
 /**
  * Set the keyMaterial to use for encrypting data.
  *
  * Pass the binary encoding of a BSON document like the following:
  *
  *   { "keyMaterial" : (BSON BINARY value) }
@@ -653,17 +607,15 @@
  * @param[in] key_material The data encryption key to use. The viewed data is
  * copied. It is valid to destroy @p key_material with @ref
  * mongocrypt_binary_destroy immediately after.
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_key_material (mongocrypt_ctx_t *ctx,
-                                    mongocrypt_binary_t *key_material);
+bool mongocrypt_ctx_setopt_key_material(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *key_material);
 
 /**
  * Set the algorithm used for encryption to either
  * deterministic or random encryption. This value
  * should only be set when using explicit encryption.
  *
  * If -1 is passed in for "len", then "algorithm" is
@@ -677,18 +629,15 @@
  * @param[in] algorithm A string specifying the algorithm to
  * use for encryption.
  * @param[in] len The length of the algorithm string.
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_algorithm (mongocrypt_ctx_t *ctx,
-                                 const char *algorithm,
-                                 int len);
+bool mongocrypt_ctx_setopt_algorithm(mongocrypt_ctx_t *ctx, const char *algorithm, int len);
 
 /// String constant for setopt_algorithm "Deterministic" encryption
 /// String constant for setopt_algorithm "Random" encryption
 /// String constant for setopt_algorithm "Indexed" explicit encryption
 /// String constant for setopt_algorithm "Unindexed" explicit encryption
 /// String constant for setopt_algorithm "rangePreview" explicit encryption
 /// NOTE: The RangePreview algorithm is experimental only. It is not intended
@@ -708,20 +657,19 @@
  * (CMK).
  * @param[in] cmk_len The string length of @p cmk_len. Pass -1 to determine the
  * string length with strlen (must be NULL terminated).
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_masterkey_aws (mongocrypt_ctx_t *ctx,
-                                     const char *region,
-                                     int32_t region_len,
-                                     const char *cmk,
-                                     int32_t cmk_len);
+bool mongocrypt_ctx_setopt_masterkey_aws(mongocrypt_ctx_t *ctx,
+                                         const char *region,
+                                         int32_t region_len,
+                                         const char *cmk,
+                                         int32_t cmk_len);
 
 /**
  * Identify a custom AWS endpoint when creating a data key.
  * This is used internally to construct the correct HTTP request
  * (with the Host header set to this endpoint). This endpoint
  * is persisted in the new data key, and will be returned via
  * @ref mongocrypt_kms_ctx_endpoint.
@@ -732,31 +680,27 @@
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] endpoint The endpoint.
  * @param[in] endpoint_len The string length of @p endpoint. Pass -1 to
  * determine the string length with strlen (must be NULL terminated).
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_masterkey_aws_endpoint (mongocrypt_ctx_t *ctx,
-                                              const char *endpoint,
-                                              int32_t endpoint_len);
+bool mongocrypt_ctx_setopt_masterkey_aws_endpoint(mongocrypt_ctx_t *ctx, const char *endpoint, int32_t endpoint_len);
 
 /**
  * Set the master key to "local" for creating a data key.
  * This has been superseded by the more flexible:
  * @ref mongocrypt_ctx_setopt_key_encryption_key
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_masterkey_local (mongocrypt_ctx_t *ctx);
+bool mongocrypt_ctx_setopt_masterkey_local(mongocrypt_ctx_t *ctx);
 
 /**
  * Set key encryption key document for creating a data key or for rewrapping
  * datakeys.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] bin BSON representing the key encryption key document with
@@ -801,17 +745,15 @@
  *    endpoint: <string>
  * }
  *
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status.
  */
-bool
-mongocrypt_ctx_setopt_key_encryption_key (mongocrypt_ctx_t *ctx,
-                                          mongocrypt_binary_t *bin);
+bool mongocrypt_ctx_setopt_key_encryption_key(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *bin);
 
 /**
  * Initialize a context to create a data key.
  *
  * Associated options:
  * - @ref mongocrypt_ctx_setopt_masterkey_aws
  * - @ref mongocrypt_ctx_setopt_masterkey_aws_endpoint
@@ -819,16 +761,15 @@
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  * @pre A master key option has been set, and an associated KMS provider
  * has been set on the parent @ref mongocrypt_t.
  */
-bool
-mongocrypt_ctx_datakey_init (mongocrypt_ctx_t *ctx);
+bool mongocrypt_ctx_datakey_init(mongocrypt_ctx_t *ctx);
 
 /**
  * Initialize a context for encryption.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] db The database name.
  * @param[in] db_len The byte length of @p db. Pass -1 to determine the string
@@ -836,19 +777,15 @@
  * be NULL terminated).
  * @param[in] cmd The BSON command to be encrypted. The viewed data is copied.
  * It is valid to destroy @p cmd with @ref mongocrypt_binary_destroy immediately
  * after.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_encrypt_init (mongocrypt_ctx_t *ctx,
-                             const char *db,
-                             int32_t db_len,
-                             mongocrypt_binary_t *cmd);
+bool mongocrypt_ctx_encrypt_init(mongocrypt_ctx_t *ctx, const char *db, int32_t db_len, mongocrypt_binary_t *cmd);
 
 /**
  * Explicit helper method to encrypt a single BSON object. Contexts
  * created for explicit encryption will not go through mongocryptd.
  *
  * To specify a key_id, algorithm, or iv to use, please use the
  * corresponding mongocrypt_setopt methods before calling this.
@@ -877,17 +814,15 @@
  * @param[in] ctx A @ref mongocrypt_ctx_t.
  * @param[in] msg A @ref mongocrypt_binary_t the plaintext BSON value. The
  * viewed data is copied. It is valid to destroy @p msg with @ref
  * mongocrypt_binary_destroy immediately after.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_explicit_encrypt_init (mongocrypt_ctx_t *ctx,
-                                      mongocrypt_binary_t *msg);
+bool mongocrypt_ctx_explicit_encrypt_init(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *msg);
 
 /**
  * Explicit helper method to encrypt a Match Expression or Aggregate Expression.
  * Contexts created for explicit encryption will not go through mongocryptd.
  * Requires query_type to be "rangePreview".
  * NOTE: The RangePreview algorithm is experimental only. It is not intended for
  * public use.
@@ -925,92 +860,84 @@
  * @param[in] ctx A @ref mongocrypt_ctx_t.
  * @param[in] msg A @ref mongocrypt_binary_t the plaintext BSON value. The
  * viewed data is copied. It is valid to destroy @p msg with @ref
  * mongocrypt_binary_destroy immediately after.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_explicit_encrypt_expression_init (mongocrypt_ctx_t *ctx,
-                                                 mongocrypt_binary_t *msg);
+bool mongocrypt_ctx_explicit_encrypt_expression_init(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *msg);
 
 /**
  * Initialize a context for decryption.
  *
  * This method expects the passed-in BSON to be of the form:
  * { "v" : BSON value to encrypt }
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] doc The document to be decrypted. The viewed data is copied. It is
  * valid to destroy @p doc with @ref mongocrypt_binary_destroy immediately
  * after.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_decrypt_init (mongocrypt_ctx_t *ctx, mongocrypt_binary_t *doc);
+bool mongocrypt_ctx_decrypt_init(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *doc);
 
 /**
  * Explicit helper method to decrypt a single BSON object.
  *
  * Pass the binary encoding of a BSON document containing the BSON value to
  * encrypt like the following:
  *
  *   { "v" : (BSON BINARY value of subtype 6) }
  *
  * @param[in] ctx A @ref mongocrypt_ctx_t.
  * @param[in] msg A @ref mongocrypt_binary_t the encrypted BSON. The viewed data
  * is copied. It is valid to destroy @p msg with @ref mongocrypt_binary_destroy
  * immediately after.
  */
-bool
-mongocrypt_ctx_explicit_decrypt_init (mongocrypt_ctx_t *ctx,
-                                      mongocrypt_binary_t *msg);
+bool mongocrypt_ctx_explicit_decrypt_init(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *msg);
 
 /**
  * @brief Initialize a context to rewrap datakeys.
  *
  * Associated options:
  * - @ref mongocrypt_ctx_setopt_key_encryption_key
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] filter The filter to use for the find command on the key vault
  * collection to retrieve datakeys to rewrap.
  * @return A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status.
  */
-bool
-mongocrypt_ctx_rewrap_many_datakey_init (mongocrypt_ctx_t *ctx,
-                                         mongocrypt_binary_t *filter);
+bool mongocrypt_ctx_rewrap_many_datakey_init(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *filter);
 
 /**
  * Indicates the state of the @ref mongocrypt_ctx_t. Each state requires
  * different handling. See [the integration
  * guide](https://github.com/mongodb/libmongocrypt/blob/master/integrating.md#state-machine)
  * for information on what to do for each state.
  */
 typedef enum {
-   MONGOCRYPT_CTX_ERROR = 0,
-   MONGOCRYPT_CTX_NEED_MONGO_COLLINFO = 1, /* run on main MongoClient */
-   MONGOCRYPT_CTX_NEED_MONGO_MARKINGS = 2, /* run on mongocryptd. */
-   MONGOCRYPT_CTX_NEED_MONGO_KEYS = 3,     /* run on key vault */
-   MONGOCRYPT_CTX_NEED_KMS = 4,
-   MONGOCRYPT_CTX_NEED_KMS_CREDENTIALS = 7, /* fetch/renew KMS credentials */
-   MONGOCRYPT_CTX_READY = 5, /* ready for encryption/decryption */
-   MONGOCRYPT_CTX_DONE = 6,
+    MONGOCRYPT_CTX_ERROR = 0,
+    MONGOCRYPT_CTX_NEED_MONGO_COLLINFO = 1, /* run on main MongoClient */
+    MONGOCRYPT_CTX_NEED_MONGO_MARKINGS = 2, /* run on mongocryptd. */
+    MONGOCRYPT_CTX_NEED_MONGO_KEYS = 3,     /* run on key vault */
+    MONGOCRYPT_CTX_NEED_KMS = 4,
+    MONGOCRYPT_CTX_NEED_KMS_CREDENTIALS = 7, /* fetch/renew KMS credentials */
+    MONGOCRYPT_CTX_READY = 5,                /* ready for encryption/decryption */
+    MONGOCRYPT_CTX_DONE = 6,
 } mongocrypt_ctx_state_t;
 
 /**
  * Get the current state of a context.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @returns A @ref mongocrypt_ctx_state_t.
  */
-mongocrypt_ctx_state_t
-mongocrypt_ctx_state (mongocrypt_ctx_t *ctx);
+mongocrypt_ctx_state_t mongocrypt_ctx_state(mongocrypt_ctx_t *ctx);
 
 /**
  * Get BSON necessary to run the mongo operation when mongocrypt_ctx_t
  * is in MONGOCRYPT_CTX_NEED_MONGO_* states.
  *
  * @p op_bson is a BSON document to be used for the operation.
  * - For MONGOCRYPT_CTX_NEED_MONGO_COLLINFO it is a listCollections filter.
@@ -1024,16 +951,15 @@
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[out] op_bson A BSON document for the MongoDB operation. The data
  * viewed by @p op_bson is guaranteed to be valid until @p ctx is destroyed with
  * @ref mongocrypt_ctx_destroy.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_mongo_op (mongocrypt_ctx_t *ctx, mongocrypt_binary_t *op_bson);
+bool mongocrypt_ctx_mongo_op(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *op_bson);
 
 /**
  * Feed a BSON reply or result when mongocrypt_ctx_t is in
  * MONGOCRYPT_CTX_NEED_MONGO_* states. This may be called multiple times
  * depending on the operation.
  *
  * reply is a BSON document result being fed back for this operation.
@@ -1049,26 +975,24 @@
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] reply A BSON document for the MongoDB operation. The viewed data
  * is copied. It is valid to destroy @p reply with @ref
  * mongocrypt_binary_destroy immediately after.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_mongo_feed (mongocrypt_ctx_t *ctx, mongocrypt_binary_t *reply);
+bool mongocrypt_ctx_mongo_feed(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *reply);
 
 /**
  * Call when done feeding the reply (or replies) back to the context.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_mongo_done (mongocrypt_ctx_t *ctx);
+bool mongocrypt_ctx_mongo_done(mongocrypt_ctx_t *ctx);
 
 /**
  * Manages a single KMS HTTP request/response.
  */
 typedef struct _mongocrypt_kms_ctx_t mongocrypt_kms_ctx_t;
 
 /**
@@ -1080,33 +1004,30 @@
  *
  * If KMS handles are being handled synchronously, the driver can reuse the same
  * TLS socket to send HTTP requests and receive responses.
  *
  * @param[in] ctx A @ref mongocrypt_ctx_t.
  * @returns a new @ref mongocrypt_kms_ctx_t or NULL.
  */
-mongocrypt_kms_ctx_t *
-mongocrypt_ctx_next_kms_ctx (mongocrypt_ctx_t *ctx);
+mongocrypt_kms_ctx_t *mongocrypt_ctx_next_kms_ctx(mongocrypt_ctx_t *ctx);
 
 /**
  * Get the HTTP request message for a KMS handle.
  *
  * The lifetime of @p msg is tied to the lifetime of @p kms. It is valid
  * until @ref mongocrypt_ctx_kms_done is called.
  *
  * @param[in] kms A @ref mongocrypt_kms_ctx_t.
  * @param[out] msg The HTTP request to send to KMS. The data viewed by @p msg is
  * guaranteed to be valid until the call of @ref mongocrypt_ctx_kms_done of the
  * parent @ref mongocrypt_ctx_t.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_kms_ctx_status
  */
-bool
-mongocrypt_kms_ctx_message (mongocrypt_kms_ctx_t *kms,
-                            mongocrypt_binary_t *msg);
+bool mongocrypt_kms_ctx_message(mongocrypt_kms_ctx_t *kms, mongocrypt_binary_t *msg);
 
 /**
  * Get the hostname from which to connect over TLS.
  *
  * The storage for @p endpoint is not owned by the caller, but
  * is valid until calling @ref mongocrypt_ctx_kms_done.
  *
@@ -1114,52 +1035,47 @@
  * @param[out] endpoint The output endpoint as a NULL terminated string.
  * The endpoint consists of a hostname and port separated by a colon.
  * E.g. "example.com:123". A port is always present.
  *
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_kms_ctx_status
  */
-bool
-mongocrypt_kms_ctx_endpoint (mongocrypt_kms_ctx_t *kms, const char **endpoint);
+bool mongocrypt_kms_ctx_endpoint(mongocrypt_kms_ctx_t *kms, const char **endpoint);
 
 /**
  * Indicates how many bytes to feed into @ref mongocrypt_kms_ctx_feed.
  *
  * @param[in] kms The @ref mongocrypt_kms_ctx_t.
  * @returns The number of requested bytes.
  */
-uint32_t
-mongocrypt_kms_ctx_bytes_needed (mongocrypt_kms_ctx_t *kms);
+uint32_t mongocrypt_kms_ctx_bytes_needed(mongocrypt_kms_ctx_t *kms);
 
 /**
  * Feed bytes from the HTTP response.
  *
  * Feeding more bytes than what has been returned in @ref
  * mongocrypt_kms_ctx_bytes_needed is an error.
  *
  * @param[in] kms The @ref mongocrypt_kms_ctx_t.
  * @param[in] bytes The bytes to feed. The viewed data is copied. It is valid to
  * destroy @p bytes with @ref mongocrypt_binary_destroy immediately after.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_kms_ctx_status
  */
-bool
-mongocrypt_kms_ctx_feed (mongocrypt_kms_ctx_t *kms, mongocrypt_binary_t *bytes);
+bool mongocrypt_kms_ctx_feed(mongocrypt_kms_ctx_t *kms, mongocrypt_binary_t *bytes);
 
 /**
  * Get the status associated with a @ref mongocrypt_kms_ctx_t object.
  *
  * @param[in] kms The @ref mongocrypt_kms_ctx_t object.
  * @param[out] status Receives the status.
  *
  * @returns A boolean indicating success. If false, an error status is set.
  */
-bool
-mongocrypt_kms_ctx_status (mongocrypt_kms_ctx_t *kms,
-                           mongocrypt_status_t *status);
+bool mongocrypt_kms_ctx_status(mongocrypt_kms_ctx_t *kms, mongocrypt_status_t *status);
 
 /**
  * Get the KMS provider identifier associated with this KMS request.
  *
  * This is used to conditionally configure TLS connections based on the KMS
  * request. It is useful for KMIP, which authenticates with a client
  * certificate.
@@ -1168,27 +1084,25 @@
  * @param[out] len Receives the length of the returned string. It may be NULL.
  * If it is not NULL, it is set to the length of the returned string without
  * the NULL terminator.
  *
  * @returns One of the NULL terminated static strings: "aws", "azure", "gcp", or
  * "kmip".
  */
-const char *
-mongocrypt_kms_ctx_get_kms_provider (mongocrypt_kms_ctx_t *kms, uint32_t *len);
+const char *mongocrypt_kms_ctx_get_kms_provider(mongocrypt_kms_ctx_t *kms, uint32_t *len);
 
 /**
  * Call when done handling all KMS contexts.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  *
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_kms_done (mongocrypt_ctx_t *ctx);
+bool mongocrypt_ctx_kms_done(mongocrypt_ctx_t *ctx);
 
 /**
  * Call in response to the MONGOCRYPT_CTX_NEED_KMS_CREDENTIALS state
  * to set per-context KMS provider settings. These follow the same format
  * as @ref mongocrypt_setopt_kms_providers. If no keys are present in the
  * BSON input, the KMS provider settings configured for the @ref mongocrypt_t
  * at initialization are used.
@@ -1196,17 +1110,15 @@
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] kms_providers_definition A BSON document mapping the KMS provider
  * names to credentials.
  *
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status.
  */
-bool
-mongocrypt_ctx_provide_kms_providers (
-   mongocrypt_ctx_t *ctx, mongocrypt_binary_t *kms_providers_definition);
+bool mongocrypt_ctx_provide_kms_providers(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *kms_providers_definition);
 
 /**
  * Perform the final encryption or decryption.
  *
  * @param[in] ctx A @ref mongocrypt_ctx_t.
  * @param[out] out The final BSON. The data viewed by @p out is guaranteed
  * to be valid until @p ctx is destroyed with @ref mongocrypt_ctx_destroy.
@@ -1236,24 +1148,22 @@
  * where each BSON document in the array contains the updated fields of a
  * rewrapped datakey to be bulk-updated into the key vault collection.
  * Note: the updateDate field should be updated using the $currentDate operator.
  *
  * @returns a bool indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_finalize (mongocrypt_ctx_t *ctx, mongocrypt_binary_t *out);
+bool mongocrypt_ctx_finalize(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *out);
 
 /**
  * Destroy and free all memory associated with a @ref mongocrypt_ctx_t.
  *
  * @param[in] ctx A @ref mongocrypt_ctx_t.
  */
-void
-mongocrypt_ctx_destroy (mongocrypt_ctx_t *ctx);
+void mongocrypt_ctx_destroy(mongocrypt_ctx_t *ctx);
 
 /**
  * An crypto AES-256-CBC encrypt or decrypt function.
  *
  * Note, @p in is already padded. Encrypt with padding disabled.
  * @param[in] ctx An optional context object that may have been set when hooks
  * were enabled.
@@ -1264,21 +1174,21 @@
  * mongocrypt_binary_data.
  * @param[out] bytes_written Set this to the number of bytes written to @p out.
  * @param[out] status An optional status to pass error messages. See @ref
  * mongocrypt_status_set.
  * @returns A boolean indicating success. If returning false, set @p status
  * with a message indiciating the error using @ref mongocrypt_status_set.
  */
-typedef bool (*mongocrypt_crypto_fn) (void *ctx,
-                                      mongocrypt_binary_t *key,
-                                      mongocrypt_binary_t *iv,
-                                      mongocrypt_binary_t *in,
-                                      mongocrypt_binary_t *out,
-                                      uint32_t *bytes_written,
-                                      mongocrypt_status_t *status);
+typedef bool (*mongocrypt_crypto_fn)(void *ctx,
+                                     mongocrypt_binary_t *key,
+                                     mongocrypt_binary_t *iv,
+                                     mongocrypt_binary_t *in,
+                                     mongocrypt_binary_t *out,
+                                     uint32_t *bytes_written,
+                                     mongocrypt_status_t *status);
 
 /**
  * A crypto signature or HMAC function.
  *
  * Currently used in callbacks for HMAC SHA-512, HMAC SHA-256, and RSA SHA-256
  * signature.
  *
@@ -1289,65 +1199,61 @@
  * @param[out] out A preallocated byte array for the output. See @ref
  * mongocrypt_binary_data.
  * @param[out] status An optional status to pass error messages. See @ref
  * mongocrypt_status_set.
  * @returns A boolean indicating success. If returning false, set @p status
  * with a message indiciating the error using @ref mongocrypt_status_set.
  */
-typedef bool (*mongocrypt_hmac_fn) (void *ctx,
-                                    mongocrypt_binary_t *key,
-                                    mongocrypt_binary_t *in,
-                                    mongocrypt_binary_t *out,
-                                    mongocrypt_status_t *status);
+typedef bool (*mongocrypt_hmac_fn)(void *ctx,
+                                   mongocrypt_binary_t *key,
+                                   mongocrypt_binary_t *in,
+                                   mongocrypt_binary_t *out,
+                                   mongocrypt_status_t *status);
 
 /**
  * A crypto hash (SHA-256) function.
  *
  * @param[in] ctx An optional context object that may have been set when hooks
  * were enabled.
  * @param[in] in The input.
  * @param[out] out A preallocated byte array for the output. See @ref
  * mongocrypt_binary_data.
  * @param[out] status An optional status to pass error messages. See @ref
  * mongocrypt_status_set.
  * @returns A boolean indicating success. If returning false, set @p status
  * with a message indiciating the error using @ref mongocrypt_status_set.
  */
-typedef bool (*mongocrypt_hash_fn) (void *ctx,
-                                    mongocrypt_binary_t *in,
-                                    mongocrypt_binary_t *out,
-                                    mongocrypt_status_t *status);
+typedef bool (*mongocrypt_hash_fn)(void *ctx,
+                                   mongocrypt_binary_t *in,
+                                   mongocrypt_binary_t *out,
+                                   mongocrypt_status_t *status);
 
 /**
  * A crypto secure random function.
  *
  * @param[in] ctx An optional context object that may have been set when hooks
  * were enabled.
  * @param[out] out A preallocated byte array for the output. See @ref
  * mongocrypt_binary_data.
  * @param[in] count The number of random bytes requested.
  * @param[out] status An optional status to pass error messages. See @ref
  * mongocrypt_status_set.
  * @returns A boolean indicating success. If returning false, set @p status
  * with a message indiciating the error using @ref mongocrypt_status_set.
  */
-typedef bool (*mongocrypt_random_fn) (void *ctx,
-                                      mongocrypt_binary_t *out,
-                                      uint32_t count,
-                                      mongocrypt_status_t *status);
-
-bool
-mongocrypt_setopt_crypto_hooks (mongocrypt_t *crypt,
-                                mongocrypt_crypto_fn aes_256_cbc_encrypt,
-                                mongocrypt_crypto_fn aes_256_cbc_decrypt,
-                                mongocrypt_random_fn random,
-                                mongocrypt_hmac_fn hmac_sha_512,
-                                mongocrypt_hmac_fn hmac_sha_256,
-                                mongocrypt_hash_fn sha_256,
-                                void *ctx);
+typedef bool (*mongocrypt_random_fn)(void *ctx, mongocrypt_binary_t *out, uint32_t count, mongocrypt_status_t *status);
+
+bool mongocrypt_setopt_crypto_hooks(mongocrypt_t *crypt,
+                                    mongocrypt_crypto_fn aes_256_cbc_encrypt,
+                                    mongocrypt_crypto_fn aes_256_cbc_decrypt,
+                                    mongocrypt_random_fn random,
+                                    mongocrypt_hmac_fn hmac_sha_512,
+                                    mongocrypt_hmac_fn hmac_sha_256,
+                                    mongocrypt_hash_fn sha_256,
+                                    void *ctx);
 
 /**
  * Set a crypto hook for the AES256-CTR operations.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
  * @param[in] aes_256_ctr_encrypt The crypto callback function for encrypt
  * operation.
@@ -1356,19 +1262,18 @@
  * @param[in] ctx A context passed as an argument to the crypto callback
  * every invocation.
  * @pre @ref mongocrypt_init has not been called on @p crypt.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_status
  *
  */
-bool
-mongocrypt_setopt_aes_256_ctr (mongocrypt_t *crypt,
-                               mongocrypt_crypto_fn aes_256_ctr_encrypt,
-                               mongocrypt_crypto_fn aes_256_ctr_decrypt,
-                               void *ctx);
+bool mongocrypt_setopt_aes_256_ctr(mongocrypt_t *crypt,
+                                   mongocrypt_crypto_fn aes_256_ctr_encrypt,
+                                   mongocrypt_crypto_fn aes_256_ctr_decrypt,
+                                   void *ctx);
 
 /**
  * Set an AES256-ECB crypto hook for the AES256-CTR operations. If CTR hook was
  * configured using @ref mongocrypt_setopt_aes_256_ctr, ECB hook will be
  * ignored.
  *
  * @param[in] crypt The @ref mongocrypt_t object.
@@ -1377,18 +1282,15 @@
  * @param[in] ctx A context passed as an argument to the crypto callback
  * every invocation.
  * @pre @ref mongocrypt_init has not been called on @p crypt.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_status
  *
  */
-bool
-mongocrypt_setopt_aes_256_ecb (mongocrypt_t *crypt,
-                               mongocrypt_crypto_fn aes_256_ecb_encrypt,
-                               void *ctx);
+bool mongocrypt_setopt_aes_256_ecb(mongocrypt_t *crypt, mongocrypt_crypto_fn aes_256_ecb_encrypt, void *ctx);
 
 /**
  * Set a crypto hook for the RSASSA-PKCS1-v1_5 algorithm with a SHA-256 hash.
  *
  * See: https://tools.ietf.org/html/rfc3447#section-8.2
  *
  * Note: this function has the wrong name. It should be:
@@ -1399,45 +1301,40 @@
  * @param[in] sign_ctx A context passed as an argument to the crypto callback
  * every invocation.
  * @pre @ref mongocrypt_init has not been called on @p crypt.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_status
  *
  */
-bool
-mongocrypt_setopt_crypto_hook_sign_rsaes_pkcs1_v1_5 (
-   mongocrypt_t *crypt,
-   mongocrypt_hmac_fn sign_rsaes_pkcs1_v1_5,
-   void *sign_ctx);
+bool mongocrypt_setopt_crypto_hook_sign_rsaes_pkcs1_v1_5(mongocrypt_t *crypt,
+                                                         mongocrypt_hmac_fn sign_rsaes_pkcs1_v1_5,
+                                                         void *sign_ctx);
 
 /**
  * @brief Opt-into skipping query analysis.
  *
  * If opted in:
  * - The crypt_shared library will not attempt to be loaded.
  * - A mongocrypt_ctx_t will never enter the MONGOCRYPT_CTX_NEED_MARKINGS state.
  *
  * @param[in] crypt The @ref mongocrypt_t object to update
  */
-void
-mongocrypt_setopt_bypass_query_analysis (mongocrypt_t *crypt);
+void mongocrypt_setopt_bypass_query_analysis(mongocrypt_t *crypt);
 
 /**
  * Set the contention factor used for explicit encryption.
  * The contention factor is only used for indexed Queryable Encryption.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] contention_factor
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status.
  */
-bool
-mongocrypt_ctx_setopt_contention_factor (mongocrypt_ctx_t *ctx,
-                                         int64_t contention_factor);
+bool mongocrypt_ctx_setopt_contention_factor(mongocrypt_ctx_t *ctx, int64_t contention_factor);
 
 /**
  * Set the index key id to use for explicit Queryable Encryption.
  *
  * If the index key id not set, the key id from @ref
  * mongocrypt_ctx_setopt_key_id is used.
  *
@@ -1446,32 +1343,27 @@
  * key to use from the key vault collection. Note, the UUID must be encoded with
  * RFC-4122 byte order. The viewed data is copied. It is valid to destroy
  * @p key_id with @ref mongocrypt_binary_destroy immediately after.
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_index_key_id (mongocrypt_ctx_t *ctx,
-                                    mongocrypt_binary_t *key_id);
+bool mongocrypt_ctx_setopt_index_key_id(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *key_id);
 
 /**
  * Set the query type to use for explicit Queryable Encryption.
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] query_type The query type string
  * @param[in] len The length of query_type, or -1 for automatic
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_query_type (mongocrypt_ctx_t *ctx,
-                                  const char *query_type,
-                                  int len);
+bool mongocrypt_ctx_setopt_query_type(mongocrypt_ctx_t *ctx, const char *query_type, int len);
 
 /**
  * Set options for explicit encryption with the "rangePreview" algorithm.
  * NOTE: The RangePreview algorithm is experimental only. It is not intended for
  * public use.
  *
  * @p opts is a BSON document of the form:
@@ -1484,17 +1376,15 @@
  *
  * @param[in] ctx The @ref mongocrypt_ctx_t object.
  * @param[in] opts BSON.
  * @pre @p ctx has not been initialized.
  * @returns A boolean indicating success. If false, an error status is set.
  * Retrieve it with @ref mongocrypt_ctx_status
  */
-bool
-mongocrypt_ctx_setopt_algorithm_range (mongocrypt_ctx_t *ctx,
-                                       mongocrypt_binary_t *opts);
+bool mongocrypt_ctx_setopt_algorithm_range(mongocrypt_ctx_t *ctx, mongocrypt_binary_t *opts);
 
 /// String constants for setopt_query_type
 // NOTE: The RangePreview algorithm is experimental only. It is not intended for
 // public use.
 """)
 
 if PY3:
```

### Comparing `pymongocrypt-1.5.2/pymongocrypt/credentials.py` & `pymongocrypt-1.6.0/pymongocrypt/credentials.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/pymongocrypt/crypto.py` & `pymongocrypt-1.6.0/pymongocrypt/crypto.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/pymongocrypt/errors.py` & `pymongocrypt-1.6.0/pymongocrypt/errors.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/pymongocrypt/explicit_encrypter.py` & `pymongocrypt-1.6.0/pymongocrypt/explicit_encrypter.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/pymongocrypt/mongocrypt.py` & `pymongocrypt-1.6.0/pymongocrypt/mongocrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 import copy
 
 
 from pymongocrypt.binary import (MongoCryptBinaryIn,
                                  MongoCryptBinaryOut)
 from pymongocrypt.binding import ffi, lib, _to_string
-from pymongocrypt.compat import (safe_bytearray_or_base64, str_to_bytes,
-                                 unicode_type)
+from pymongocrypt.compat import str_to_bytes, unicode_type
 from pymongocrypt.credentials import _ask_for_kms_credentials
 from pymongocrypt.errors import MongoCryptError
 from pymongocrypt.state_machine import MongoCryptCallback
 
 from pymongocrypt.crypto import (aes_256_cbc_encrypt,
                                  aes_256_cbc_decrypt,
                                  aes_256_ctr_decrypt,
@@ -44,20 +43,18 @@
         :Parameters:
           - `kms_providers`: Map of KMS provider options. The kms_providers
             map values differ by provider:
               - `aws`: Map with "accessKeyId" and "secretAccessKey" as strings,
                  and optionally a "sessionToken" for temporary credentials.
               - `azure`: Map with "clientId" and "clientSecret" as strings.
               - `gcp`: Map with "email" as a string and "privateKey" as
-                a byte array or a base64-encoded string. On Python 2,
-                base64-encoded strings must be passed as unicode literals.
+                a byte array or a base64-encoded string.
               - `kmip`: Map with "endpoint" as a string.
               - `local`: Map with "key" as a 96-byte array or the equivalent
-                base64-encoded string. On Python 2, base64-encoded strings
-                must be passed as unicode literals.
+                base64-encoded string.
           - `schema_map`: Optional map of collection namespace ("db.coll") to
             JSON Schema.  By default, a collection's JSONSchema is periodically
             polled with the listCollections command. But a JSONSchema may be
             specified locally with the schemaMap option.
 
             Supplying a `schema_map` provides more security than relying on
             JSON Schemas obtained from the server. It protects against a
@@ -121,16 +118,15 @@
             if len(gcp):
                 if 'email' not in gcp or 'privateKey' not in gcp:
                     raise ValueError("kms_providers['gcp'] must contain "
                                      "'email' and 'privateKey'")
                 if not isinstance(kms_providers['gcp']['privateKey'],
                                   (bytes, unicode_type)):
                     raise TypeError("kms_providers['gcp']['privateKey'] must "
-                                    "be an instance of bytes or str "
-                                    "(unicode in Python 2)")
+                                    "be an instance of bytes or str")
 
         if 'kmip' in kms_providers:
             kmip = kms_providers['kmip']
             if not isinstance(kmip, dict):
                 raise ValueError("kms_providers['kmip'] must be a dict")
             if 'endpoint' not in kmip:
                 raise ValueError("kms_providers['kmip'] must contain "
@@ -145,16 +141,15 @@
             if not isinstance(local, dict):
                 raise ValueError("kms_providers['local'] must be a dict")
             if 'key' not in local:
                 raise ValueError("kms_providers['local'] must contain 'key'")
             if not isinstance(kms_providers['local']['key'],
                               (bytes, unicode_type)):
                 raise TypeError("kms_providers['local']['key'] must be an "
-                                "instance of bytes or str (unicode in "
-                                "Python 2)")
+                                "instance of bytes or str")
 
         if schema_map is not None and not isinstance(schema_map, bytes):
             raise TypeError("schema_map must be bytes or None")
 
         if encrypted_fields_map is not None and not isinstance(encrypted_fields_map, bytes):
             raise TypeError("encrypted_fields_map must be bytes or None")
 
@@ -196,25 +191,14 @@
             # Destroy the mongocrypt object on error.
             self.close()
             raise
 
     def __init(self):
         """Internal init helper."""
         kms_providers = self.__opts.kms_providers
-
-        # Make fields that can be passed as binary or string safe to
-        # encode to BSON.
-        base64_or_bytes_fields = [("local", "key"), ("gcp", "privateKey")]
-        for f1, f2 in base64_or_bytes_fields:
-            value = kms_providers.get(f1, {}).get(f2, None)
-            if value is not None:
-                safe_value = safe_bytearray_or_base64(value)
-                if value != safe_value:
-                    kms_providers = copy.deepcopy(kms_providers)
-                    kms_providers[f1][f2] = safe_value
         with MongoCryptBinaryIn(
                 self.__callback.bson_encode(kms_providers)) as kmsopt:
             if not lib.mongocrypt_setopt_kms_providers(
                     self.__crypt, kmsopt.bin):
                 self.__raise_from_status()
 
         schema_map = self.__opts.schema_map
```

### Comparing `pymongocrypt-1.5.2/pymongocrypt/state_machine.py` & `pymongocrypt-1.6.0/pymongocrypt/state_machine.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/pymongocrypt/version.py` & `pymongocrypt-1.6.0/pymongocrypt/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.5.2'
+__version__ = '1.6.0'
 
-_MIN_LIBMONGOCRYPT_VERSION = '1.7.0'
+_MIN_LIBMONGOCRYPT_VERSION = '1.8.0'
```

### Comparing `pymongocrypt-1.5.2/pymongocrypt.egg-info/PKG-INFO` & `pymongocrypt-1.6.0/pymongocrypt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: pymongocrypt
-Version: 1.5.2
+Version: 1.6.0
 Summary: Python bindings for libmongocrypt
 Home-page: https://github.com/mongodb/libmongocrypt/tree/master/bindings/python
 Author: Shane Harvey
 Author-email: mongodb-user@googlegroups.com
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,pymongocrypt,pymongo,mongocrypt,bson
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+Requires-Python: >=3.7
 License-File: LICENSE
 
 ============
 PyMongoCrypt
 ============
 :Info: Python bindings for libmongocrypt. See
        `GitHub <https://github.com/mongodb/libmongocrypt/tree/master/bindings/python>`_
@@ -41,15 +37,15 @@
 About
 =====
 
 Python wrapper library for libmongocrypt that supports client side encryption
 in drivers. PyMongoCrypt uses `cffi <https://pypi.org/project/cffi/>`_ and
 `cryptography <https://pypi.org/project/cryptography/>`_.
 
-PyMongoCrypt supports Python 2.7, 3.4+, and PyPy3.5+.
+PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 Support / Feedback
 ==================
 
 For issues with, questions about, or feedback for PyMongoCrypt, please look into
 our `support channels <http://www.mongodb.org/about/support>`_. Please
 do not email any of the PyMongoCrypt developers directly with issues or
@@ -173,15 +169,15 @@
   $ export PYMONGOCRYPT_LIB=$(pwd)/libmongocrypt-all/rhel-62-64-bit/nocrypto/lib64/libmongocrypt.so
   $ python -c "import pymongocrypt; print(pymongocrypt.libmongocrypt_version())"
   1.2.1
 
 Dependencies
 ============
 
-PyMongoCrypt supports CPython 2.7, 3.4+, PyPy, and PyPy3.5+.
+PyMongoCrypt supports Python 3.7+ and PyPy3.7+.
 
 PyMongoCrypt requires `cffi <https://pypi.org/project/cffi/>`_ and
 `cryptography <https://pypi.org/project/cryptography/>`_.
 
 If not installed using one of the official wheels, PyMongoCrypt also requires
 libmongocrypt to be installed on your system. If libmongocrypt is not
 installed you will see an error like this:
```

### Comparing `pymongocrypt-1.5.2/pymongocrypt.egg-info/SOURCES.txt` & `pymongocrypt-1.6.0/pymongocrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/setup.py` & `pymongocrypt-1.6.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 import sys
 
 from setuptools import setup, find_packages
 
+if sys.version_info[:3] < (3, 7):
+    raise RuntimeError("pymongocrypt requires Python version >= 3.7")
+
 # Make our Windows and macOS wheels platform specific because we embed
 # libmongocrypt. On Linux we ship manylinux2010 wheels which cannot do this or
 # else auditwheel raises the following error:
 # RuntimeError: Invalid binary wheel, found the following shared
 # library/libraries in purelib folder:
 # 	libmongocrypt.so
 # The wheel has to be platlib compliant in order to be repaired by auditwheel.
@@ -18,16 +21,16 @@
 
             def finalize_options(self):
                 _bdist_wheel.finalize_options(self)
                 self.root_is_pure = False
 
             def get_tag(self):
                 python, abi, plat = _bdist_wheel.get_tag(self)
-                # Our python source is py2/3 compatible.
-                python, abi = 'py2.py3', 'none'
+                # Our python source is py3 compatible.
+                python, abi = 'py3', 'none'
                 return python, abi, plat
 
         cmdclass['bdist_wheel'] = bdist_wheel
     except ImportError:
         # Version of wheel is too old, use None to fail a bdist_wheel attempt.
         cmdclass['bdist_wheel'] = None
 
@@ -60,28 +63,24 @@
     author="Shane Harvey",
     author_email="mongodb-user@googlegroups.com",
     url="https://github.com/mongodb/libmongocrypt/tree/master/bindings/python",
     keywords=["mongo", "mongodb", "pymongocrypt", "pymongo", "mongocrypt",
               "bson"],
     test_suite="test",
     license="Apache License, Version 2.0",
-    python_requires=">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*",
+    python_requires=">=3.7",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
```

### Comparing `pymongocrypt-1.5.2/test/test_binding.py` & `pymongocrypt-1.6.0/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/test/test_crypto.py` & `pymongocrypt-1.6.0/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `pymongocrypt-1.5.2/test/test_mongocrypt.py` & `pymongocrypt-1.6.0/test/test_mongocrypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,19 +133,19 @@
                 {'aws': {'secretAccessKey': 'foo'}}]:
             with self.assertRaisesRegex(
                     ValueError, r"kms_providers\['aws'\] must contain "
                                 "'accessKeyId' and 'secretAccessKey'"):
                 MongoCryptOptions(invalid_kms_providers)
         with self.assertRaisesRegex(
                 TypeError, r"kms_providers\['local'\]\['key'\] must be an "
-                           r"instance of bytes or str \(unicode in Python 2\)"):
+                           r"instance of bytes or str"):
             MongoCryptOptions({'local': {'key': None}})
         with self.assertRaisesRegex(
                 TypeError, r"kms_providers\['gcp'\]\['privateKey'\] must be an "
-                           r"instance of bytes or str \(unicode in Python 2\)"):
+                           r"instance of bytes or str"):
             MongoCryptOptions({'gcp': {'email': "foo@bar.baz",
                                        "privateKey": None}})
 
         valid_kms = {'aws': {'accessKeyId': '', 'secretAccessKey': ''}}
         with self.assertRaisesRegex(
                 TypeError, "schema_map must be bytes or None"):
             MongoCryptOptions(valid_kms, schema_map={})
@@ -778,17 +778,17 @@
         key_path = 'keys/ABCDEFAB123498761234123456789012-local-document.json'
         key_id = json_data(key_path)['_id']
         encrypter = ExplicitEncrypter(MockCallback(
             key_docs=[bson_data(key_path)],
             kms_reply=http_data('kms-reply.txt')), self.mongo_crypt_opts())
         self.addCleanup(encrypter.close)
 
-        range_opts = bson_data("fle2-find-range-explicit/int32/rangeopts.json")
-        value = bson_data("fle2-find-range-explicit/int32/value-to-encrypt.json")
-        expected = json_data("fle2-find-range-explicit/int32/encrypted-payload.json")
+        range_opts = bson_data("fle2-find-range-explicit-v2/int32/rangeopts.json")
+        value = bson_data("fle2-find-range-explicit-v2/int32/value-to-encrypt.json")
+        expected = json_data("fle2-find-range-explicit-v2/int32/encrypted-payload.json")
         encrypted = encrypter.encrypt(
             value, "rangePreview", key_id=key_id, query_type="rangePreview",
             contention_factor=4, range_opts=range_opts, is_expression=True)
         encrypted_val = bson.decode(encrypted, OPTS)
         self.assertEqual(encrypted_val, expected)
```

