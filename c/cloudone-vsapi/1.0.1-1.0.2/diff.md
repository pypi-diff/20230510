# Comparing `tmp/cloudone-vsapi-1.0.1.tar.gz` & `tmp/cloudone-vsapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudone-vsapi-1.0.1.tar", last modified: Thu May  4 18:54:01 2023, max compression
+gzip compressed data, was "cloudone-vsapi-1.0.2.tar", last modified: Wed May 10 18:24:34 2023, max compression
```

## Comparing `cloudone-vsapi-1.0.1.tar` & `cloudone-vsapi-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/grpc/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/grpc/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/grpc/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/grpc/protos/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-04 18:53:58.000000 cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 18:53:58.000000 cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-04 18:53:58.000000 cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 18:54:01.413081 cloudone-vsapi-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-04 18:54:00.000000 cloudone-vsapi-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/grpc/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/grpc/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/amaas/grpc/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.898701 cloudone-vsapi-1.0.2/amaas/grpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-10 18:24:32.000000 cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-10 18:24:32.000000 cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-10 18:24:32.000000 cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 18:24:34.000000 cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-10 18:24:33.000000 cloudone-vsapi-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.902701 cloudone-vsapi-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 18:22:57.000000 cloudone-vsapi-1.0.2/tests/test_simple.py
```

### Comparing `cloudone-vsapi-1.0.1/LICENSE` & `cloudone-vsapi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.1/PKG-INFO` & `cloudone-vsapi-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudone-vsapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Trend Micro Cloud One VSAPI SDK for python
 Home-page: https://github.com/trendmicro/cloudone-antimalware-python-sdk
 Author: Trend Micro Cloud One Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,39 +13,86 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
-# Cloud One VSAPI SDK for Python
+# Trend Cloud One VSAPI SDK for Python
 
-Cloud One VSAPI is a Software Development Kit (SDK) for Python, which allows Python developers to write software that makes use of Cloud One Antimalware Service.
+Cloud One VSAPI is a Software Development Kit (SDK) for Python, which allows Python developers to write software that makes use of Cloud One Antimalware Service API.
 
-## Prerequisites
+## Requirements
 
+- Have an [Trend Cloud One Account](https://cloudone.trendmicro.com). [Sign up for free trial now](https://cloudone.trendmicro.com/trial) if it's not already the case!
+- A [Trend Cloud One API Key](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-api-key/#new-api-key)
+- A [Trend Cloud One Region](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-regions/) of choice
 - Python 3.7 or newer
-- [CloudOne API Key](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-api-key/)
+- A file or object to be scan
+
 
 
 ## Installation
 
 Install the VSAPI SDK package with pip:
 
    ```sh
    python -m pip install cloudone-vsapi
    ```
 
 ## Documentation
 
-Documentation for the client SDK is available on [Here]() and [Read the Docs](https://cloudone.trendmicro.com/docs/).
+Documentation for the client SDK is available on [Here](README.md) and [Read the Docs](https://cloudone.trendmicro.com/docs/).
 
 ## Run SDK
 
-### Example Usage
+### Run with Cloud One VSAPI examples
+
+1. Go to `/examples/` in current directory.
+
+   ```sh
+   cd examples/
+   ```
+
+2. There are two Python examples in the folder, one with regular file i/o and one with asynchronous file i/o
+   
+   ```
+   client_aio.py
+   client.py
+   ``` 
+3. Current Python examples support following command line arguments
+
+   | Command Line Arguments                 | Value                    | Optional |
+   | :------------------ | :----------------------- | :------- |
+   | --region or -r | [Trend Cloud One Region](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-regions/), such as: us-1 | Yes, either -r or -a
+   | --addr or -a   | Trend Cloud One Amaas server, such as: antimalware.us-1.cloudone.trendmicro.com:443 | Yes, either -r or -a      |
+   | --api_key      | Cloud One \<API KEY\>              | No       |
+   | --filename or -f |        File to be scanned            | No       |
+
+
+4. Run one of the examples.
+   
+   The example program needs to be configured with your Cloud One account's secret key which is available in your Cloud One Dashboard. Set `API_KEY` from corresponding Cloud One Region to its value and `FILENAME` to the target file:
+
+   ```sh
+   python3 client.py -f FILENAME -r us-1 --api_key API_KEY
+   ```
+   or
+   
+   using Antimalware Service server address `-a` instead of region `-r`:
+   ```sh
+   python3 client.py -f FILENAME -a antimalware.us-1.cloudone.trendmicro.com:443 --api_key API_KEY
+   ```
+   or
+   
+   using asynchronous IO example program:
+   ```sh
+   python3 client_aio.py -f FILENAME -a antimalware.us-1.cloudone.trendmicro.com:443 --api_key API_KEY
+   ```
+### Code Examples
 ```python:
 import json
 import amaas.grpc
 
 handle = amaas.grpc.init(YOUR_CLOUD_ONE_AMAAS_SERVER, YOUR_ClOUD_ONE_KEY, True)
 
 result = amaas.grpc.scan_file(args.filename, handle)
@@ -79,45 +126,11 @@
     await amaas.grpc.aio.quit(handle)
 
 
 asyncio.run(scan_files())
 
 ```
 
-### Run with Cloud One VSAPI examples
-
-1. Go to `/examples/` in current directory.
-
-   ```sh
-   cd examples/
-   ```
-
-
-2. There are two Python examples in the folder, one with regular file i/o and one with asynchronous file i/o
-   
-   ```
-   client_aio.py
-   client.py
-   ``` 
-3. Current Python examples support following command line arguments
-
-   | Command Line Arguments                 | Value                    | Optional |
-   | :------------------ | :----------------------- | :------- |
-   | --addr or -a   | antimalware.us-1.cloudone.trendmicro.com:443 | No       |
-   | --api_key      | Cloud One \<API KEY\>              | No       |
-   | --filename or -f |        File to be scanned            | No       |
-
-
-
-4. Run one of the examples.
-
-   ```sh
-   python3 client.py -f FILENAME -a ADDR --api_key API_KEY
-   ```
-   or
-   ```sh
-   python3 client_aio.py -f FILENAME -a ADDR --api_key API_KEY
-   ```
 ## More Resources
 - [License](LICENSE)
 - [Changelog](CHANGELOG.md)
-- [NOTICE](NOTICE)
+- [Notice](NOTICE)
```

### Comparing `cloudone-vsapi-1.0.1/README.md` & `cloudone-vsapi-1.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,79 @@
-# Cloud One VSAPI SDK for Python
+# Trend Cloud One VSAPI SDK for Python
 
-Cloud One VSAPI is a Software Development Kit (SDK) for Python, which allows Python developers to write software that makes use of Cloud One Antimalware Service.
+Cloud One VSAPI is a Software Development Kit (SDK) for Python, which allows Python developers to write software that makes use of Cloud One Antimalware Service API.
 
-## Prerequisites
+## Requirements
 
+- Have an [Trend Cloud One Account](https://cloudone.trendmicro.com). [Sign up for free trial now](https://cloudone.trendmicro.com/trial) if it's not already the case!
+- A [Trend Cloud One API Key](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-api-key/#new-api-key)
+- A [Trend Cloud One Region](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-regions/) of choice
 - Python 3.7 or newer
-- [CloudOne API Key](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-api-key/)
+- A file or object to be scan
+
 
 
 ## Installation
 
 Install the VSAPI SDK package with pip:
 
    ```sh
    python -m pip install cloudone-vsapi
    ```
 
 ## Documentation
 
-Documentation for the client SDK is available on [Here]() and [Read the Docs](https://cloudone.trendmicro.com/docs/).
+Documentation for the client SDK is available on [Here](README.md) and [Read the Docs](https://cloudone.trendmicro.com/docs/).
 
 ## Run SDK
 
-### Example Usage
+### Run with Cloud One VSAPI examples
+
+1. Go to `/examples/` in current directory.
+
+   ```sh
+   cd examples/
+   ```
+
+2. There are two Python examples in the folder, one with regular file i/o and one with asynchronous file i/o
+   
+   ```
+   client_aio.py
+   client.py
+   ``` 
+3. Current Python examples support following command line arguments
+
+   | Command Line Arguments                 | Value                    | Optional |
+   | :------------------ | :----------------------- | :------- |
+   | --region or -r | [Trend Cloud One Region](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-regions/), such as: us-1 | Yes, either -r or -a
+   | --addr or -a   | Trend Cloud One Amaas server, such as: antimalware.us-1.cloudone.trendmicro.com:443 | Yes, either -r or -a      |
+   | --api_key      | Cloud One \<API KEY\>              | No       |
+   | --filename or -f |        File to be scanned            | No       |
+
+
+4. Run one of the examples.
+   
+   The example program needs to be configured with your Cloud One account's secret key which is available in your Cloud One Dashboard. Set `API_KEY` from corresponding Cloud One Region to its value and `FILENAME` to the target file:
+
+   ```sh
+   python3 client.py -f FILENAME -r us-1 --api_key API_KEY
+   ```
+   or
+   
+   using Antimalware Service server address `-a` instead of region `-r`:
+   ```sh
+   python3 client.py -f FILENAME -a antimalware.us-1.cloudone.trendmicro.com:443 --api_key API_KEY
+   ```
+   or
+   
+   using asynchronous IO example program:
+   ```sh
+   python3 client_aio.py -f FILENAME -a antimalware.us-1.cloudone.trendmicro.com:443 --api_key API_KEY
+   ```
+### Code Examples
 ```python:
 import json
 import amaas.grpc
 
 handle = amaas.grpc.init(YOUR_CLOUD_ONE_AMAAS_SERVER, YOUR_ClOUD_ONE_KEY, True)
 
 result = amaas.grpc.scan_file(args.filename, handle)
@@ -60,45 +107,11 @@
     await amaas.grpc.aio.quit(handle)
 
 
 asyncio.run(scan_files())
 
 ```
 
-### Run with Cloud One VSAPI examples
-
-1. Go to `/examples/` in current directory.
-
-   ```sh
-   cd examples/
-   ```
-
-
-2. There are two Python examples in the folder, one with regular file i/o and one with asynchronous file i/o
-   
-   ```
-   client_aio.py
-   client.py
-   ``` 
-3. Current Python examples support following command line arguments
-
-   | Command Line Arguments                 | Value                    | Optional |
-   | :------------------ | :----------------------- | :------- |
-   | --addr or -a   | antimalware.us-1.cloudone.trendmicro.com:443 | No       |
-   | --api_key      | Cloud One \<API KEY\>              | No       |
-   | --filename or -f |        File to be scanned            | No       |
-
-
-
-4. Run one of the examples.
-
-   ```sh
-   python3 client.py -f FILENAME -a ADDR --api_key API_KEY
-   ```
-   or
-   ```sh
-   python3 client_aio.py -f FILENAME -a ADDR --api_key API_KEY
-   ```
 ## More Resources
 - [License](LICENSE)
 - [Changelog](CHANGELOG.md)
-- [NOTICE](NOTICE)
+- [Notice](NOTICE)
```

### Comparing `cloudone-vsapi-1.0.1/amaas/grpc/__init__.py` & `cloudone-vsapi-1.0.2/amaas/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.1/amaas/grpc/aio/__init__.py` & `cloudone-vsapi-1.0.2/amaas/grpc/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2.py` & `cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2.pyi` & `cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2_grpc.py` & `cloudone-vsapi-1.0.2/amaas/grpc/protos/scan_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/PKG-INFO` & `cloudone-vsapi-1.0.2/cloudone_vsapi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudone-vsapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Trend Micro Cloud One VSAPI SDK for python
 Home-page: https://github.com/trendmicro/cloudone-antimalware-python-sdk
 Author: Trend Micro Cloud One Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,39 +13,86 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
-# Cloud One VSAPI SDK for Python
+# Trend Cloud One VSAPI SDK for Python
 
-Cloud One VSAPI is a Software Development Kit (SDK) for Python, which allows Python developers to write software that makes use of Cloud One Antimalware Service.
+Cloud One VSAPI is a Software Development Kit (SDK) for Python, which allows Python developers to write software that makes use of Cloud One Antimalware Service API.
 
-## Prerequisites
+## Requirements
 
+- Have an [Trend Cloud One Account](https://cloudone.trendmicro.com). [Sign up for free trial now](https://cloudone.trendmicro.com/trial) if it's not already the case!
+- A [Trend Cloud One API Key](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-api-key/#new-api-key)
+- A [Trend Cloud One Region](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-regions/) of choice
 - Python 3.7 or newer
-- [CloudOne API Key](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-api-key/)
+- A file or object to be scan
+
 
 
 ## Installation
 
 Install the VSAPI SDK package with pip:
 
    ```sh
    python -m pip install cloudone-vsapi
    ```
 
 ## Documentation
 
-Documentation for the client SDK is available on [Here]() and [Read the Docs](https://cloudone.trendmicro.com/docs/).
+Documentation for the client SDK is available on [Here](README.md) and [Read the Docs](https://cloudone.trendmicro.com/docs/).
 
 ## Run SDK
 
-### Example Usage
+### Run with Cloud One VSAPI examples
+
+1. Go to `/examples/` in current directory.
+
+   ```sh
+   cd examples/
+   ```
+
+2. There are two Python examples in the folder, one with regular file i/o and one with asynchronous file i/o
+   
+   ```
+   client_aio.py
+   client.py
+   ``` 
+3. Current Python examples support following command line arguments
+
+   | Command Line Arguments                 | Value                    | Optional |
+   | :------------------ | :----------------------- | :------- |
+   | --region or -r | [Trend Cloud One Region](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-regions/), such as: us-1 | Yes, either -r or -a
+   | --addr or -a   | Trend Cloud One Amaas server, such as: antimalware.us-1.cloudone.trendmicro.com:443 | Yes, either -r or -a      |
+   | --api_key      | Cloud One \<API KEY\>              | No       |
+   | --filename or -f |        File to be scanned            | No       |
+
+
+4. Run one of the examples.
+   
+   The example program needs to be configured with your Cloud One account's secret key which is available in your Cloud One Dashboard. Set `API_KEY` from corresponding Cloud One Region to its value and `FILENAME` to the target file:
+
+   ```sh
+   python3 client.py -f FILENAME -r us-1 --api_key API_KEY
+   ```
+   or
+   
+   using Antimalware Service server address `-a` instead of region `-r`:
+   ```sh
+   python3 client.py -f FILENAME -a antimalware.us-1.cloudone.trendmicro.com:443 --api_key API_KEY
+   ```
+   or
+   
+   using asynchronous IO example program:
+   ```sh
+   python3 client_aio.py -f FILENAME -a antimalware.us-1.cloudone.trendmicro.com:443 --api_key API_KEY
+   ```
+### Code Examples
 ```python:
 import json
 import amaas.grpc
 
 handle = amaas.grpc.init(YOUR_CLOUD_ONE_AMAAS_SERVER, YOUR_ClOUD_ONE_KEY, True)
 
 result = amaas.grpc.scan_file(args.filename, handle)
@@ -79,45 +126,11 @@
     await amaas.grpc.aio.quit(handle)
 
 
 asyncio.run(scan_files())
 
 ```
 
-### Run with Cloud One VSAPI examples
-
-1. Go to `/examples/` in current directory.
-
-   ```sh
-   cd examples/
-   ```
-
-
-2. There are two Python examples in the folder, one with regular file i/o and one with asynchronous file i/o
-   
-   ```
-   client_aio.py
-   client.py
-   ``` 
-3. Current Python examples support following command line arguments
-
-   | Command Line Arguments                 | Value                    | Optional |
-   | :------------------ | :----------------------- | :------- |
-   | --addr or -a   | antimalware.us-1.cloudone.trendmicro.com:443 | No       |
-   | --api_key      | Cloud One \<API KEY\>              | No       |
-   | --filename or -f |        File to be scanned            | No       |
-
-
-
-4. Run one of the examples.
-
-   ```sh
-   python3 client.py -f FILENAME -a ADDR --api_key API_KEY
-   ```
-   or
-   ```sh
-   python3 client_aio.py -f FILENAME -a ADDR --api_key API_KEY
-   ```
 ## More Resources
 - [License](LICENSE)
 - [Changelog](CHANGELOG.md)
-- [NOTICE](NOTICE)
+- [Notice](NOTICE)
```

### Comparing `cloudone-vsapi-1.0.1/setup.py` & `cloudone-vsapi-1.0.2/setup.py`

 * *Files identical despite different names*

