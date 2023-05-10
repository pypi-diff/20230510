# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.887.tar", last modified: Tue May  9 03:06:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.888.tar", last modified: Wed May 10 02:18:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.887.tar` & `tencentcloud-sdk-python-lighthouse-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    25647 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89637 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   236708 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:06:51.000000 tencentcloud-sdk-python-lighthouse-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    25988 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92541 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240429 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:18:58.000000 tencentcloud-sdk-python-lighthouse-3.0.888/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,16 @@
 
 # 变更实例套餐失败。
 FAILEDOPERATION_MODIFYINSTANCESBUNDLEFAILED = 'FailedOperation.ModifyInstancesBundleFailed'
 
 # 变更资源属性失败，请稍后重新操作。
 FAILEDOPERATION_MODIFYRESOURCESATTRIBUTEFAILED = 'FailedOperation.ModifyResourcesAttributeFailed'
 
-# 续费实例失败。
-FAILEDOPERATION_RENEWINSTANCESFAILED = 'FailedOperation.RenewInstancesFailed'
+# 续费资源失败。
+FAILEDOPERATION_RENEWRESOURCESFAILED = 'FailedOperation.RenewResourcesFailed'
 
 # 请求错误。
 FAILEDOPERATION_REQUESTERROR = 'FailedOperation.RequestError'
 
 # 快照操作失败。
 FAILEDOPERATION_SNAPSHOTOPERATIONFAILED = 'FailedOperation.SnapshotOperationFailed'
 
@@ -259,14 +259,17 @@
 
 # 非法的套餐参数。
 INVALIDPARAMETERVALUE_INVALIDBUNDLE = 'InvalidParameterValue.InvalidBundle'
 
 # 控制台显示类型不合法。
 INVALIDPARAMETERVALUE_INVALIDCONSOLEDISPLAYTYPES = 'InvalidParameterValue.InvalidConsoleDisplayTypes'
 
+# 当前实例到期时间不能早于云硬盘到期时间。
+INVALIDPARAMETERVALUE_INVALIDCURINSTANCEDEADLINE = 'InvalidParameterValue.InvalidCurInstanceDeadline'
+
 # 参数值非法，磁盘 ID 格式非法。
 INVALIDPARAMETERVALUE_INVALIDDISKIDMALFORMED = 'InvalidParameterValue.InvalidDiskIdMalformed'
 
 # 云硬盘类型非法。
 INVALIDPARAMETERVALUE_INVALIDDISKTYPE = 'InvalidParameterValue.InvalidDiskType'
 
 # 设置是否使用默认密钥对登录的值不正确。
@@ -379,14 +382,17 @@
 
 # 超过快照配额。
 LIMITEXCEEDED_SNAPSHOTQUOTALIMITEXCEEDED = 'LimitExceeded.SnapshotQuotaLimitExceeded'
 
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
+# 必须传入参数Period或CurInstanceDeadline。
+MISSINGPARAMETER_MISSINGPARAMETERPERIODCURINSTANCEDEADLINE = 'MissingParameter.MissingParameterPeriodCurInstanceDeadline'
+
 # 该实例不支持升级套餐操作。
 OPERATIONDENIED_BUNDLENOTSUPPORTMODIFY = 'OperationDenied.BundleNotSupportModify'
 
 # 磁盘备份点忙，请稍后重新操作。
 OPERATIONDENIED_DISKBACKUPBUSY = 'OperationDenied.DiskBackupBusy'
 
 # 磁盘备份点正在操作过程中，请稍后重试。
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1392,14 +1392,42 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def IsolateDisks(self, request):
+        """本接口(IsolateDisks)用于退还一个或多个轻量应用服务器云硬盘。
+
+        只有状态为 UNATTACHED 的数据盘才可以进行此操作。
+        接口调用成功后，云硬盘会进入SHUTDOWN 状态。
+        支持批量操作。每次请求批量资源的上限为 20。
+        本接口为异步接口，请求发送成功后会返回一个 RequestId，此时操作并未立即完成。云硬盘操作结果可以通过调用 [DescribeDisks](https://cloud.tencent.com/document/product/1207/66093) 接口查询，如果云硬盘的最新操作状态（LatestOperationState）为“SUCCESS”，则代表操作成功。
+
+        :param request: Request instance for IsolateDisks.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.IsolateDisksRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.IsolateDisksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("IsolateDisks", params, headers=headers)
+            response = json.loads(body)
+            model = models.IsolateDisksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def IsolateInstances(self, request):
         """本接口(IsolateInstances)用于退还一个或多个轻量应用服务器实例。
         * 只有状态为 RUNNING 或 STOPPED 的实例才可以进行此操作。
         * 接口调用成功后，实例会进入SHUTDOWN 状态。
         * 支持批量操作。每次请求批量资源（包括实例与数据盘）的上限为 20。
         * 本接口为异步接口，请求发送成功后会返回一个 RequestId，此时操作并未立即完成。实例操作结果可以通过调用 DescribeInstances 接口查询，如果实例的最新操作状态（LatestOperationState）为“SUCCESS”，则代表操作成功。
 
@@ -1728,14 +1756,41 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def RenewDisks(self, request):
+        """本接口(RenewDisks)用于续费一个或多个轻量应用服务器云硬盘。
+
+        只有状态为 ATTACHED，UNATTACHED 或 SHUTDOWN 的数据盘才可以进行此操作。
+        支持批量操作。每次请求批量云硬盘的上限为 50。
+        本接口为异步接口，请求发送成功后会返回一个 RequestId，此时操作并未立即完成。云硬盘操作结果可以通过调用 [DescribeDisks](https://cloud.tencent.com/document/product/1207/66093) 接口查询，如果云硬盘的最新操作状态（LatestOperationState）为“SUCCESS”，则代表操作成功。
+
+        :param request: Request instance for RenewDisks.
+        :type request: :class:`tencentcloud.lighthouse.v20200324.models.RenewDisksRequest`
+        :rtype: :class:`tencentcloud.lighthouse.v20200324.models.RenewDisksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RenewDisks", params, headers=headers)
+            response = json.loads(body)
+            model = models.RenewDisksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def RenewInstances(self, request):
         """本接口(RenewInstances)用于续费一个或多个轻量应用服务器实例。
         * 只有状态为 RUNNING，STOPPED 或 SHUTDOWN 的实例才可以进行此操作。
         * 支持批量操作。每次请求批量实例的上限为 100。
         * 本接口为异步接口，请求发送成功后会返回一个 RequestId，此时操作并未立即完成。实例操作结果可以通过调用 DescribeInstances 接口查询，如果实例的最新操作状态（LatestOperationState）为“SUCCESS”，则代表操作成功。
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5073,14 +5073,55 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class IsolateDisksRequest(AbstractModel):
+    """IsolateDisks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DiskIds: 云硬盘ID列表。一个或多个待操作的云硬盘ID。可通过[DescribeDisks](https://cloud.tencent.com/document/product/1207/66093)接口返回值中的DiskId获取。每次请求退还数据盘数量总计上限为20。
+        :type DiskIds: list of str
+        """
+        self.DiskIds = None
+
+
+    def _deserialize(self, params):
+        self.DiskIds = params.get("DiskIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class IsolateDisksResponse(AbstractModel):
+    """IsolateDisks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class IsolateInstancesRequest(AbstractModel):
     """IsolateInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5944,21 +5985,25 @@
 class RenewDiskChargePrepaid(AbstractModel):
     """续费云硬盘包年包月相关参数设置
 
     """
 
     def __init__(self):
         r"""
-        :param Period: 新购周期。
+        :param Period: 续费周期。
         :type Period: int
-        :param RenewFlag: 续费标识。
+        :param RenewFlag: 续费标识。取值范围：
+
+NOTIFY_AND_AUTO_RENEW：通知过期且自动续费。 NOTIFY_AND_MANUAL_RENEW：通知过期不自动续费，用户需要手动续费。 DISABLE_NOTIFY_AND_AUTO_RENEW：不自动续费，且不通知。
+
+默认取值：NOTIFY_AND_MANUAL_RENEW。若该参数指定为NOTIFY_AND_AUTO_RENEW，在账户余额充足的情况下，云硬盘到期后将按月自动续费。
         :type RenewFlag: str
-        :param TimeUnit: 周期单位. 默认值: "m"。
+        :param TimeUnit: 周期单位。取值范围：“m”(月)。默认值: "m"。
         :type TimeUnit: str
-        :param CurInstanceDeadline: 当前实例到期时间。
+        :param CurInstanceDeadline: 当前实例到期时间。如“2018-01-01 00:00:00”。指定该参数即可对齐云硬盘所挂载的实例到期时间。该参数与Period必须指定其一，且不支持同时指定。
         :type CurInstanceDeadline: str
         """
         self.Period = None
         self.RenewFlag = None
         self.TimeUnit = None
         self.CurInstanceDeadline = None
 
@@ -5973,14 +6018,65 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RenewDisksRequest(AbstractModel):
+    """RenewDisks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DiskIds: 云硬盘ID列表。一个或多个待操作的云硬盘ID。可通过[DescribeDisks](https://cloud.tencent.com/document/product/1207/66093)接口返回值中的DiskId获取。每次请求续费数据盘数量总计上限为50。
+        :type DiskIds: list of str
+        :param RenewDiskChargePrepaid: 续费云硬盘包年包月相关参数设置。
+        :type RenewDiskChargePrepaid: :class:`tencentcloud.lighthouse.v20200324.models.RenewDiskChargePrepaid`
+        :param AutoVoucher: 是否自动使用代金券。默认不使用。
+        :type AutoVoucher: bool
+        """
+        self.DiskIds = None
+        self.RenewDiskChargePrepaid = None
+        self.AutoVoucher = None
+
+
+    def _deserialize(self, params):
+        self.DiskIds = params.get("DiskIds")
+        if params.get("RenewDiskChargePrepaid") is not None:
+            self.RenewDiskChargePrepaid = RenewDiskChargePrepaid()
+            self.RenewDiskChargePrepaid._deserialize(params.get("RenewDiskChargePrepaid"))
+        self.AutoVoucher = params.get("AutoVoucher")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RenewDisksResponse(AbstractModel):
+    """RenewDisks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class RenewInstancesRequest(AbstractModel):
     """RenewInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.888/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.888/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.887/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.888/setup.py`

 * *Files identical despite different names*

