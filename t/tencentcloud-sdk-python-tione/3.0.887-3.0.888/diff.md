# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.887.tar", last modified: Tue May  9 03:22:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.888.tar", last modified: Wed May 10 02:57:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.887.tar` & `tencentcloud-sdk-python-tione-3.0.888.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    10835 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   333554 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:22:50.000000 tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    11488 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   333554 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-10 02:57:20.000000 tencentcloud-sdk-python-tione-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:57:21.000000 tencentcloud-sdk-python-tione-3.0.888/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.887/README.rst` & `tencentcloud-sdk-python-tione-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,17 @@
 
 # 根据标签查询资源失败。
 FAILEDOPERATION_QUERYMODELSBYTAGSFAILED = 'FailedOperation.QueryModelsByTagsFailed'
 
 # 查询计费价格失败。
 FAILEDOPERATION_QUERYPRICEFAILED = 'FailedOperation.QueryPriceFailed'
 
+# 查询计费项详情失败。
+FAILEDOPERATION_QUERYRESOURCESPECFAILED = 'FailedOperation.QueryResourceSpecFailed'
+
 # 查询计费项失败。
 FAILEDOPERATION_QUERYSPECSFAILED = 'FailedOperation.QuerySpecsFailed'
 
 # 查询标签服务失败。
 FAILEDOPERATION_QUERYTAGFAIL = 'FailedOperation.QueryTagFail'
 
 # 记录不存在。
@@ -184,14 +187,17 @@
 
 # 获取HDFS存储信息失败。
 INTERNALERROR_QUERYHDFSINFOFAILED = 'InternalError.QueryHDFSInfoFailed'
 
 # 查询预付费资源组详情失败。
 INTERNALERROR_QUERYRESOURCEGROUPFAILED = 'InternalError.QueryResourceGroupFailed'
 
+# 查询资源套餐规格失败
+INTERNALERROR_QUERYRESOURCESPECFAILED = 'InternalError.QueryResourceSpecFailed'
+
 # 查询子网信息失败。
 INTERNALERROR_QUERYSUBNETINFOFAILED = 'InternalError.QuerySubnetInfoFailed'
 
 # 停止任务失败。
 INTERNALERROR_STOPJOBINSTANCEFAILED = 'InternalError.StopJobInstanceFailed'
 
 # 参数错误。
@@ -208,14 +214,17 @@
 
 # 请求参数校验失败。
 INVALIDPARAMETER_VALIDATEERROR = 'InvalidParameter.ValidateError'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
+# AI市场公共算法版本Id不存在
+INVALIDPARAMETERVALUE_AIMARKETPUBLICALGOVERSIONNOTEXIST = 'InvalidParameterValue.AIMarketPublicAlgoVersionNotExist'
+
 # 名称不合法。
 INVALIDPARAMETERVALUE_BADNAME = 'InvalidParameterValue.BadName'
 
 # 请设置日志集、日志主题ID。
 INVALIDPARAMETERVALUE_CLSCONFIGREQUIRED = 'InvalidParameterValue.ClsConfigRequired'
 
 # 存储库不存在。
@@ -259,14 +268,20 @@
 
 # 参数值数量超过限制。
 INVALIDPARAMETERVALUE_LIMITEXCEEDED = 'InvalidParameterValue.LimitExceeded'
 
 # 操作不允许。
 INVALIDPARAMETERVALUE_NOTALLOW = 'InvalidParameterValue.NotAllow'
 
+# 资源配置不合法
+INVALIDPARAMETERVALUE_RESOURCECONFIGILLEGAL = 'InvalidParameterValue.ResourceConfigIllegal'
+
+# 裸金属类型资源组不支持配置输入数据
+INVALIDPARAMETERVALUE_UNSUPPORTEDDATACONFIG = 'InvalidParameterValue.UnsupportedDataConfig'
+
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
 # 操作被拒绝。
```

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20211111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.888/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.887/setup.py` & `tencentcloud-sdk-python-tione-3.0.888/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.887/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.888/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

