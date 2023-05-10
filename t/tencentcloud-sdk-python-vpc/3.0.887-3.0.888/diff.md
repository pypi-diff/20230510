# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.887.tar", last modified: Tue May  9 03:25:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.888.tar", last modified: Wed May 10 02:59:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.887.tar` & `tencentcloud-sdk-python-vpc-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   328818 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    40929 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   839190 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:25:02.000000 tencentcloud-sdk-python-vpc-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   328827 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41072 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   839291 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.887/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.887/README.rst` & `tencentcloud-sdk-python-vpc-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1949,15 +1949,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteFlowLog(self, request):
-        """本接口（DeleteFlowLog）用于删除流日志
+        """本接口（DeleteFlowLog）用于删除流日志。
 
         :param request: Request instance for DeleteFlowLog.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteFlowLogRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DeleteFlowLogResponse`
 
         """
         try:
@@ -3163,15 +3163,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeFlowLog(self, request):
-        """本接口（DescribeFlowLog）用于查询流日志实例信息
+        """本接口（DescribeFlowLog）用于查询流日志实例信息。
 
         :param request: Request instance for DescribeFlowLog.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeFlowLogRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeFlowLogResponse`
 
         """
         try:
@@ -5715,15 +5715,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyFlowLogAttribute(self, request):
-        """本接口（ModifyFlowLogAttribute）用于修改流日志属性
+        """本接口（ModifyFlowLogAttribute）用于修改流日志属性。
 
         :param request: Request instance for ModifyFlowLogAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyFlowLogAttributeRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.ModifyFlowLogAttributeResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,14 +457,17 @@
 
 # 分配IP地址数量达到上限。
 LIMITEXCEEDED_ADDRESS = 'LimitExceeded.Address'
 
 # 租户申请的弹性IP超过上限。
 LIMITEXCEEDED_ADDRESSQUOTALIMITEXCEEDED = 'LimitExceeded.AddressQuotaLimitExceeded'
 
+# 实例关联快照策略数量达到上限。
+LIMITEXCEEDED_ATTACHEDSNAPSHOTPOLICYEXCEEDED = 'LimitExceeded.AttachedSnapshotPolicyExceeded'
+
 # 带宽包配额超过限制。
 LIMITEXCEEDED_BANDWIDTHPACKAGEQUOTA = 'LimitExceeded.BandwidthPackageQuota'
 
 # 超过更换IP配额。
 LIMITEXCEEDED_CHANGEADDRESSQUOTA = 'LimitExceeded.ChangeAddressQuota'
 
 # VPC分配网段数量达到上限。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6388,15 +6388,15 @@
 class DeleteFlowLogRequest(AbstractModel):
     """DeleteFlowLog请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param FlowLogId: 流日志唯一ID
+        :param FlowLogId: 流日志唯一ID。
         :type FlowLogId: str
         :param VpcId: 私用网络ID或者统一ID，建议使用统一ID，删除云联网流日志时，可不填，其他流日志类型必填。
         :type VpcId: str
         """
         self.FlowLogId = None
         self.VpcId = None
 
@@ -9219,17 +9219,17 @@
 class DescribeFlowLogRequest(AbstractModel):
     """DescribeFlowLog请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param VpcId: 私用网络ID或者统一ID，建议使用统一ID
+        :param VpcId: 私用网络ID或者统一ID，建议使用统一ID。
         :type VpcId: str
-        :param FlowLogId: 流日志唯一ID
+        :param FlowLogId: 流日志唯一ID。
         :type FlowLogId: str
         """
         self.VpcId = None
         self.FlowLogId = None
 
 
     def _deserialize(self, params):
@@ -9247,15 +9247,15 @@
 class DescribeFlowLogResponse(AbstractModel):
     """DescribeFlowLog返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param FlowLog: 流日志信息
+        :param FlowLog: 流日志信息。
         :type FlowLog: list of FlowLog
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.FlowLog = None
         self.RequestId = None
 
@@ -14769,15 +14769,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Name: 属性名称, 若存在多个Filter时，Filter间的关系为逻辑与（AND）关系。
         :type Name: str
-        :param Values: 属性值, 若同一个Filter存在多个Values，同一Filter下Values间的关系为逻辑或（OR）关系。
+        :param Values: 属性值, 若同一个Filter存在多个Values，同一Filter下Values间的关系为逻辑或（OR）关系。当值类型为布尔类型时，可直接取值为字符串"TRUE"或 "FALSE"。
         :type Values: list of str
         """
         self.Name = None
         self.Values = None
 
 
     def _deserialize(self, params):
@@ -16953,21 +16953,21 @@
 class ModifyFlowLogAttributeRequest(AbstractModel):
     """ModifyFlowLogAttribute请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param FlowLogId: 流日志唯一ID
+        :param FlowLogId: 流日志唯一ID。
         :type FlowLogId: str
         :param VpcId: 私用网络ID或者统一ID，建议使用统一ID，修改云联网流日志属性时可不填，其他流日志类型必填。
         :type VpcId: str
-        :param FlowLogName: 流日志实例名字
+        :param FlowLogName: 流日志实例名字。
         :type FlowLogName: str
-        :param FlowLogDescription: 流日志实例描述
+        :param FlowLogDescription: 流日志实例描述。
         :type FlowLogDescription: str
         """
         self.FlowLogId = None
         self.VpcId = None
         self.FlowLogName = None
         self.FlowLogDescription = None
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.888/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.887/setup.py` & `tencentcloud-sdk-python-vpc-3.0.888/setup.py`

 * *Files identical despite different names*

