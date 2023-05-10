# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.886.tar", last modified: Mon May  8 03:12:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.887.tar", last modified: Tue May  9 02:42:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.886.tar` & `tencentcloud-sdk-python-cynosdb-3.0.887.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-08 03:12:11.000000 tencentcloud-sdk-python-cynosdb-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:12:11.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)    74122 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)     9834 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   273887 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:12:11.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-08 03:12:11.000000 tencentcloud-sdk-python-cynosdb-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:12:12.000000 tencentcloud-sdk-python-cynosdb-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)    74122 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   274129 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 02:42:39.000000 tencentcloud-sdk-python-cynosdb-3.0.887/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.886/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6240,38 +6240,43 @@
         :type Description: str
         :param WanIP: 外网IP
 注意：此字段可能返回 null，表示取不到有效值。
         :type WanIP: str
         :param WanStatus: 外网状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type WanStatus: str
+        :param InstanceGroupId: 实例组ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceGroupId: str
         """
         self.Vip = None
         self.Vport = None
         self.WanDomain = None
         self.WanPort = None
         self.NetType = None
         self.UniqSubnetId = None
         self.UniqVpcId = None
         self.Description = None
         self.WanIP = None
         self.WanStatus = None
+        self.InstanceGroupId = None
 
 
     def _deserialize(self, params):
         self.Vip = params.get("Vip")
         self.Vport = params.get("Vport")
         self.WanDomain = params.get("WanDomain")
         self.WanPort = params.get("WanPort")
         self.NetType = params.get("NetType")
         self.UniqSubnetId = params.get("UniqSubnetId")
         self.UniqVpcId = params.get("UniqVpcId")
         self.Description = params.get("Description")
         self.WanIP = params.get("WanIP")
         self.WanStatus = params.get("WanStatus")
+        self.InstanceGroupId = params.get("InstanceGroupId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.886'
+__version__ = '3.0.887'
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.886/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.887/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.887/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.886/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.887/setup.py`

 * *Files identical despite different names*

