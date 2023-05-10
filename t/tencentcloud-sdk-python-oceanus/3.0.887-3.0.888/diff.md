# Comparing `tmp/tencentcloud-sdk-python-oceanus-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-oceanus-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.887.tar", last modified: Tue May  9 03:09:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.888.tar", last modified: Wed May 10 02:24:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-oceanus-3.0.887.tar` & `tencentcloud-sdk-python-oceanus-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)     9176 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/v20190422/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)   108322 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)    23497 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud_sdk_python_oceanus.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:09:19.000000 tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/v20190422/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111986 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)    23497 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud_sdk_python_oceanus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:24:18.000000 tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.887/README.rst` & `tencentcloud-sdk-python-oceanus-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/v20190422/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,20 +341,117 @@
 
 
 class CopyJobItem(AbstractModel):
     """复制作业单条明细
 
     """
 
+    def __init__(self):
+        r"""
+        :param SourceId: 需要复制的作业serial id
+        :type SourceId: str
+        :param TargetClusterId: 目标集群的cluster serial id
+        :type TargetClusterId: str
+        :param SourceName: 需要复制的作业名称
+        :type SourceName: str
+        :param TargetName: 新作业的名称
+        :type TargetName: str
+        :param TargetFolderId: 新作业的目录id
+        :type TargetFolderId: str
+        :param JobType: 源作业类型
+        :type JobType: int
+        """
+        self.SourceId = None
+        self.TargetClusterId = None
+        self.SourceName = None
+        self.TargetName = None
+        self.TargetFolderId = None
+        self.JobType = None
+
+
+    def _deserialize(self, params):
+        self.SourceId = params.get("SourceId")
+        self.TargetClusterId = params.get("TargetClusterId")
+        self.SourceName = params.get("SourceName")
+        self.TargetName = params.get("TargetName")
+        self.TargetFolderId = params.get("TargetFolderId")
+        self.JobType = params.get("JobType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
 
 class CopyJobResult(AbstractModel):
     """复制作业单条明细结果
 
     """
 
+    def __init__(self):
+        r"""
+        :param JobId: 原作业id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobId: str
+        :param JobName: 原作业名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobName: str
+        :param TargetJobName: 新作业名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TargetJobName: str
+        :param TargetJobId: 新作业id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TargetJobId: str
+        :param Message: 失败时候的信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param Result: 0 成功  -1 失败
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Result: int
+        :param ClusterName: 目标集群名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterName: str
+        :param ClusterId: 目标集群id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterId: str
+        :param JobType: 作业类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobType: int
+        """
+        self.JobId = None
+        self.JobName = None
+        self.TargetJobName = None
+        self.TargetJobId = None
+        self.Message = None
+        self.Result = None
+        self.ClusterName = None
+        self.ClusterId = None
+        self.JobType = None
+
+
+    def _deserialize(self, params):
+        self.JobId = params.get("JobId")
+        self.JobName = params.get("JobName")
+        self.TargetJobName = params.get("TargetJobName")
+        self.TargetJobId = params.get("TargetJobId")
+        self.Message = params.get("Message")
+        self.Result = params.get("Result")
+        self.ClusterName = params.get("ClusterName")
+        self.ClusterId = params.get("ClusterId")
+        self.JobType = params.get("JobType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
 
 class CopyJobsRequest(AbstractModel):
     """CopyJobs请求参数结构体
 
     """
 
     def __init__(self):
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.888/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.887/setup.py` & `tencentcloud-sdk-python-oceanus-3.0.888/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.887/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.888/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

