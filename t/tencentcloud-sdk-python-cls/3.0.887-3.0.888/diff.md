# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.887.tar", last modified: Tue May  9 02:37:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.888.tar", last modified: Wed May 10 02:01:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.887.tar` & `tencentcloud-sdk-python-cls-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8559 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252909 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67925 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 02:37:09.000000 tencentcloud-sdk-python-cls-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8559 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   253451 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67925 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.887/README.rst` & `tencentcloud-sdk-python-cls-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2070,26 +2070,32 @@
         :type Partition: str
         :param Compress: 投递日志的压缩配置
         :type Compress: :class:`tencentcloud.cls.v20201016.models.CompressInfo`
         :param Content: 投递日志的内容格式配置
         :type Content: :class:`tencentcloud.cls.v20201016.models.ContentInfo`
         :param FilenameMode: 投递文件命名配置，0：随机数命名，1：投递时间命名，默认0（随机数命名）
         :type FilenameMode: int
+        :param StartTime: 投递数据范围的开始时间点，不能超出日志主题的生命周期起点。如果用户不填写，默认为用户新建投递任务的时间。
+        :type StartTime: int
+        :param EndTime: 投递数据范围的结束时间点，不能填写未来时间。如果用户不填写，默认为持续投递，即无限。
+        :type EndTime: int
         """
         self.TopicId = None
         self.Bucket = None
         self.Prefix = None
         self.ShipperName = None
         self.Interval = None
         self.MaxSize = None
         self.FilterRules = None
         self.Partition = None
         self.Compress = None
         self.Content = None
         self.FilenameMode = None
+        self.StartTime = None
+        self.EndTime = None
 
 
     def _deserialize(self, params):
         self.TopicId = params.get("TopicId")
         self.Bucket = params.get("Bucket")
         self.Prefix = params.get("Prefix")
         self.ShipperName = params.get("ShipperName")
@@ -2105,14 +2111,16 @@
         if params.get("Compress") is not None:
             self.Compress = CompressInfo()
             self.Compress._deserialize(params.get("Compress"))
         if params.get("Content") is not None:
             self.Content = ContentInfo()
             self.Content._deserialize(params.get("Content"))
         self.FilenameMode = params.get("FilenameMode")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.887/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.887/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.888/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.887/setup.py` & `tencentcloud-sdk-python-cls-3.0.888/setup.py`

 * *Files identical despite different names*

