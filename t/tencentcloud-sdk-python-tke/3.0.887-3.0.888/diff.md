# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.887.tar", last modified: Tue May  9 03:23:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.888.tar", last modified: Wed May 10 02:57:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.887.tar` & `tencentcloud-sdk-python-tke-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   180345 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19455 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   649612 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:23:07.000000 tencentcloud-sdk-python-tke-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   180345 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   650054 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:57:39.000000 tencentcloud-sdk-python-tke-3.0.888/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.887/README.rst` & `tencentcloud-sdk-python-tke-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.887/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.888/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10700,14 +10700,17 @@
         :type AutoUpgradeClusterLevel: bool
         :param ChargeType: 集群付费模式，支持POSTPAID_BY_HOUR或者PREPAID
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChargeType: str
         :param EdgeVersion: 边缘集群组件的版本
 注意：此字段可能返回 null，表示取不到有效值。
         :type EdgeVersion: str
+        :param TagSpecification: 集群绑定的云标签
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TagSpecification: :class:`tencentcloud.tke.v20180525.models.TagSpecification`
         """
         self.ClusterId = None
         self.ClusterName = None
         self.VpcId = None
         self.PodCIDR = None
         self.ServiceCIDR = None
         self.K8SVersion = None
@@ -10717,14 +10720,15 @@
         self.EdgeClusterVersion = None
         self.MaxNodePodNum = None
         self.ClusterAdvancedSettings = None
         self.Level = None
         self.AutoUpgradeClusterLevel = None
         self.ChargeType = None
         self.EdgeVersion = None
+        self.TagSpecification = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.VpcId = params.get("VpcId")
         self.PodCIDR = params.get("PodCIDR")
@@ -10738,14 +10742,17 @@
         if params.get("ClusterAdvancedSettings") is not None:
             self.ClusterAdvancedSettings = EdgeClusterAdvancedSettings()
             self.ClusterAdvancedSettings._deserialize(params.get("ClusterAdvancedSettings"))
         self.Level = params.get("Level")
         self.AutoUpgradeClusterLevel = params.get("AutoUpgradeClusterLevel")
         self.ChargeType = params.get("ChargeType")
         self.EdgeVersion = params.get("EdgeVersion")
+        if params.get("TagSpecification") is not None:
+            self.TagSpecification = TagSpecification()
+            self.TagSpecification._deserialize(params.get("TagSpecification"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tke-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.888/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.887/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.888/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.887/setup.py` & `tencentcloud-sdk-python-tke-3.0.888/setup.py`

 * *Files identical despite different names*

