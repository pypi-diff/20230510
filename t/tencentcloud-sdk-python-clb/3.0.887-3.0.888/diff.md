# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.887.tar", last modified: Tue May  9 02:36:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.888.tar", last modified: Wed May 10 02:01:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.887.tar` & `tencentcloud-sdk-python-clb-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)     3269 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89842 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)   328567 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/tencentcloud_sdk_python_clb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 02:36:38.000000 tencentcloud-sdk-python-clb-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89842 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   329256 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:01:16.000000 tencentcloud-sdk-python-clb-3.0.888/setup.cfg
```

### Comparing `tencentcloud-sdk-python-clb-3.0.887/README.rst` & `tencentcloud-sdk-python-clb-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.887/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.888/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4807,15 +4807,19 @@
 
     def __init__(self):
         r"""
         :param InternetChargeType: TRAFFIC_POSTPAID_BY_HOUR 按流量按小时后计费 ; BANDWIDTH_POSTPAID_BY_HOUR 按带宽按小时后计费;
 BANDWIDTH_PACKAGE 按带宽包计费;
 注意：此字段可能返回 null，表示取不到有效值。
         :type InternetChargeType: str
-        :param InternetMaxBandwidthOut: 最大出带宽，单位Mbps，范围支持0到2048，仅对公网属性的LB生效，默认值 10
+        :param InternetMaxBandwidthOut: 最大出带宽，单位Mbps，仅对公网属性的共享型、性能容量型和独占型 CLB 实例、以及内网属性的性能容量型 CLB 实例生效。
+- 对于公网属性的共享型和独占型 CLB 实例，最大出带宽的范围为1Mbps-2048Mbps。
+- 对于公网属性和内网属性的性能容量型 CLB实例
+  - 当您开通了普通规格的性能容量型时，最大出带宽的范围为1Mbps-10240Mbps。普通规格的性能容量型正在内测中，请提交 [内测申请](https://cloud.tencent.com/apply/p/hf45esx99lf)。
+  - 当您开通了超大型规格的性能容量型时，最大出带宽的范围为1Mbps-61440Mbps。超大型规格的性能容量型正在内测中，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category)。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InternetMaxBandwidthOut: int
         :param BandwidthpkgSubType: 带宽包的类型，如SINGLEISP
 注意：此字段可能返回 null，表示取不到有效值。
         :type BandwidthpkgSubType: str
         """
         self.InternetChargeType = None
```

### Comparing `tencentcloud-sdk-python-clb-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.887/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.888/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.888/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.887/setup.py` & `tencentcloud-sdk-python-clb-3.0.888/setup.py`

 * *Files identical despite different names*

