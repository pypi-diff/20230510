# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.887.tar", last modified: Tue May  9 02:50:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.888.tar", last modified: Wed May 10 02:13:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.887.tar` & `tencentcloud-sdk-python-essbasic-3.0.888.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15673 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50524 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230011 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 02:50:41.000000 tencentcloud-sdk-python-essbasic-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50895 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230011 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:13:30.000000 tencentcloud-sdk-python-essbasic-3.0.888/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.887'
+__version__ = '3.0.888'
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,22 @@
     _apiVersion = '2021-05-26'
     _endpoint = 'essbasic.tencentcloudapi.com'
     _service = 'essbasic'
 
 
     def ChannelBatchCancelFlows(self, request):
         """指定需要批量撤销的签署流程Id，批量撤销合同
-        客户指定需要撤销的签署流程Id，最多100个，超过100不处理；接口失败后返回错误信息
-        注意:
-        能撤回合同的只能是合同的发起人或者发起企业的超管、法人
+        客户指定需要撤销的签署流程Id，最多100个，超过100不处理；
+
+        **满足撤销条件的合同会发起异步撤销流程，不满足撤销条件的合同返回失败原因。**
+
+        **合同撤销成功后，会通过合同状态为 CANCEL 的回调消息通知调用方 [具体可参考回调消息](https://qian.tencent.com/developers/scenes/partner/callback_data_types#-%E5%90%88%E5%90%8C%E7%8A%B6%E6%80%81%E9%80%9A%E7%9F%A5---flowstatuschange)**
+
+        **注意:
+        能撤回合同的只能是合同的发起人或者发起企业的超管、法人**
 
         :param request: Request instance for ChannelBatchCancelFlows.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelBatchCancelFlowsRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelBatchCancelFlowsResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20210526/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.888/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.888/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.887/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.888/setup.py`

 * *Files identical despite different names*

