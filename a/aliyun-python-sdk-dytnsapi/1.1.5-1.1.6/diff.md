# Comparing `tmp/aliyun-python-sdk-dytnsapi-1.1.5.tar.gz` & `tmp/aliyun-python-sdk-dytnsapi-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dytnsapi-1.1.5.tar", last modified: Fri Apr 28 05:45:10 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dytnsapi-1.1.6.tar", last modified: Wed May 10 08:26:54 2023, max compression
```

## Comparing `aliyun-python-sdk-dytnsapi-1.1.5.tar` & `aliyun-python-sdk-dytnsapi-1.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/
--rw-r--r--   0 root         (0) root         (0)     2667 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2466 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2677 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:26:54.000000 aliyun-python-sdk-dytnsapi-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-05-10 08:26:54.000000 aliyun-python-sdk-dytnsapi-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:26:54.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyun_python_sdk_dytnsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyun_python_sdk_dytnsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyun_python_sdk_dytnsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyun_python_sdk_dytnsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:26:54.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:26:54.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:26:54.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-10 08:26:54.000000 aliyun-python-sdk-dytnsapi-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-05-10 08:26:53.000000 aliyun-python-sdk-dytnsapi-1.1.6/setup.py
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/LICENSE` & `aliyun-python-sdk-dytnsapi-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/PKG-INFO` & `aliyun-python-sdk-dytnsapi-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dytnsapi
-Version: 1.1.5
+Version: 1.1.6
 Summary: The dytnsapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dytnsapi
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/README.rst` & `aliyun-python-sdk-dytnsapi-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dytnsapi
-Version: 1.1.5
+Version: 1.1.6
 Summary: The dytnsapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dytnsapi
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/endpoint.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribePhoneNumberOperatorAttributeRequest(RpcRequest):
+class InvalidPhoneNumberFilterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberOperatorAttribute')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'InvalidPhoneNumberFilter')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class InvalidPhoneNumberFilterRequest(RpcRequest):
+class PhoneNumberEncryptRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'InvalidPhoneNumberFilter')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberEncrypt')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class PhoneNumberEncryptRequest(RpcRequest):
+class PhoneNumberStatusForAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberEncrypt')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForAccount')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class PhoneNumberStatusForAccountRequest(RpcRequest):
+class PhoneNumberStatusForVoiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForAccount')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForVoice')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class PhoneNumberStatusForVoiceRequest(RpcRequest):
+class DescribePhoneNumberOperatorAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForVoice')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberOperatorAttribute')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.6/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.5/setup.py` & `aliyun-python-sdk-dytnsapi-1.1.6/setup.py`

 * *Files identical despite different names*

