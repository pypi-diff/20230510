# Comparing `tmp/tencentcloud-sdk-python-cam-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-cam-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cam-3.0.887.tar", last modified: Tue May  9 02:29:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cam-3.0.888.tar", last modified: Wed May 10 01:51:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cam-3.0.887.tar` & `tencentcloud-sdk-python-cam-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/
--rw-r--r--   0 root         (0) root         (0)    78006 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/cam_client.py
--rw-r--r--   0 root         (0) root         (0)    10965 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/__init__.py
--rw-r--r--   0 root         (0) root         (0)   188126 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 02:29:45.000000 tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/v20190116/
+-rw-r--r--   0 root         (0) root         (0)    78006 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/v20190116/cam_client.py
+-rw-r--r--   0 root         (0) root         (0)    10965 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/v20190116/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/v20190116/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   188385 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/v20190116/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud_sdk_python_cam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud_sdk_python_cam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud_sdk_python_cam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud_sdk_python_cam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 01:51:22.000000 tencentcloud-sdk-python-cam-3.0.888/tencentcloud_sdk_python_cam.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cam-3.0.887/README.rst` & `tencentcloud-sdk-python-cam-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cam-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/cam_client.py` & `tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/v20190116/cam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/errorcodes.py` & `tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/v20190116/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.887/tencentcloud/cam/v20190116/models.py` & `tencentcloud-sdk-python-cam-3.0.888/tencentcloud/cam/v20190116/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1885,33 +1885,38 @@
         r"""
         :param LoginFlag: 登录保护设置
         :type LoginFlag: :class:`tencentcloud.cam.v20190116.models.LoginActionFlag`
         :param ActionFlag: 敏感操作保护设置
         :type ActionFlag: :class:`tencentcloud.cam.v20190116.models.LoginActionFlag`
         :param OffsiteFlag: 异地登录保护设置
         :type OffsiteFlag: :class:`tencentcloud.cam.v20190116.models.OffsiteFlag`
+        :param PromptTrust: 是否提示信任设备1 ：提示 0: 不提示
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PromptTrust: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.LoginFlag = None
         self.ActionFlag = None
         self.OffsiteFlag = None
+        self.PromptTrust = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("LoginFlag") is not None:
             self.LoginFlag = LoginActionFlag()
             self.LoginFlag._deserialize(params.get("LoginFlag"))
         if params.get("ActionFlag") is not None:
             self.ActionFlag = LoginActionFlag()
             self.ActionFlag._deserialize(params.get("ActionFlag"))
         if params.get("OffsiteFlag") is not None:
             self.OffsiteFlag = OffsiteFlag()
             self.OffsiteFlag._deserialize(params.get("OffsiteFlag"))
+        self.PromptTrust = params.get("PromptTrust")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeSafeAuthFlagIntlRequest(AbstractModel):
     """DescribeSafeAuthFlagIntl请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-cam-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-cam-3.0.888/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cam
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Cam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cam-3.0.887/setup.py` & `tencentcloud-sdk-python-cam-3.0.888/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.887/tencentcloud_sdk_python_cam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cam-3.0.888/tencentcloud_sdk_python_cam.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cam
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Cam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

