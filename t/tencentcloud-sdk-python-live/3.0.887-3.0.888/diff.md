# Comparing `tmp/tencentcloud-sdk-python-live-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.887.tar", last modified: Tue May  9 03:07:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.888.tar", last modified: Wed May 10 02:19:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.887.tar` & `tencentcloud-sdk-python-live-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-09 03:07:01.000000 tencentcloud-sdk-python-live-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   136457 2023-05-09 03:07:01.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-05-09 03:07:01.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:07:01.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   422078 2023-05-09 03:07:01.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:07:01.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:07:01.000000 tencentcloud-sdk-python-live-3.0.887/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-09 03:07:01.000000 tencentcloud-sdk-python-live-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:07:02.000000 tencentcloud-sdk-python-live-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137456 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   426940 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:19:06.000000 tencentcloud-sdk-python-live-3.0.888/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.887/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.888/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.887/README.rst` & `tencentcloud-sdk-python-live-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/v20180801/live_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2111,14 +2111,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeLiveXP2PDetailInfoList(self, request):
+        """P2P流数据查询接口，用来获取流量、卡播和起播信息。
+
+        :param request: Request instance for DescribeLiveXP2PDetailInfoList.
+        :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveXP2PDetailInfoListRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLiveXP2PDetailInfoListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLiveXP2PDetailInfoList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLiveXP2PDetailInfoListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeLogDownloadList(self, request):
         """批量获取日志URL。
 
         :param request: Request instance for DescribeLogDownloadList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLogDownloadListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLogDownloadListResponse`
```

### Comparing `tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.887/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.888/tencentcloud/live/v20180801/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6222,14 +6222,79 @@
             for item in params.get("WatermarkList"):
                 obj = WatermarkInfo()
                 obj._deserialize(item)
                 self.WatermarkList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLiveXP2PDetailInfoListRequest(AbstractModel):
+    """DescribeLiveXP2PDetailInfoList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param QueryTime: utc分钟粒度查询时间，查询某一分钟的用量数据，格式为：yyyy-mm-ddTHH:MM:00Z，参考https://cloud.tencent.com/document/product/266/11732#I，
+例如：北京时间2019-01-08 10:00:00，对应utc时间为：2019-01-08T10:00:00+08:00。
+
+支持最近六个月的查询。
+        :type QueryTime: str
+        :param Type: 类型数组，分直播live和点播vod，不传默认查全部。
+        :type Type: list of str
+        :param StreamNames: 查询流数组，不传默认查所有流。
+        :type StreamNames: list of str
+        :param Dimension: 查询维度，不传该参数则默认查询流维度的数据，传递该参数则只查对应维度的数据，和返回值的字段相关，目前支持AppId维度查询。
+        :type Dimension: list of str
+        """
+        self.QueryTime = None
+        self.Type = None
+        self.StreamNames = None
+        self.Dimension = None
+
+
+    def _deserialize(self, params):
+        self.QueryTime = params.get("QueryTime")
+        self.Type = params.get("Type")
+        self.StreamNames = params.get("StreamNames")
+        self.Dimension = params.get("Dimension")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeLiveXP2PDetailInfoListResponse(AbstractModel):
+    """DescribeLiveXP2PDetailInfoList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataInfoList: P2P流统计信息。
+        :type DataInfoList: list of XP2PDetailInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DataInfoList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("DataInfoList") is not None:
+            self.DataInfoList = []
+            for item in params.get("DataInfoList"):
+                obj = XP2PDetailInfo()
+                obj._deserialize(item)
+                self.DataInfoList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeLogDownloadListRequest(AbstractModel):
     """DescribeLogDownloadList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12181,8 +12246,75 @@
         self.Height = params.get("Height")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class XP2PDetailInfo(AbstractModel):
+    """央视P2P流信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CdnBytes: CDN流量。
+        :type CdnBytes: int
+        :param P2pBytes: P2P流量。
+        :type P2pBytes: int
+        :param StuckPeople: 卡播人数。
+        :type StuckPeople: int
+        :param StuckTimes: 卡播次数。
+        :type StuckTimes: int
+        :param OnlinePeople: 在线人数。
+        :type OnlinePeople: int
+        :param Request: 起播请求次数
+        :type Request: int
+        :param RequestSuccess: 起播成功次数
+        :type RequestSuccess: int
+        :param Time: 时间，一分钟粒度，utc格式：yyyy-mm-ddTHH:MM:SSZ，参考https://cloud.tencent.com/document/product/266/11732#I。。
+        :type Time: str
+        :param Type: 类型，分live和vod两种。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param StreamName: 流ID。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StreamName: str
+        :param AppId: AppId。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: str
+        """
+        self.CdnBytes = None
+        self.P2pBytes = None
+        self.StuckPeople = None
+        self.StuckTimes = None
+        self.OnlinePeople = None
+        self.Request = None
+        self.RequestSuccess = None
+        self.Time = None
+        self.Type = None
+        self.StreamName = None
+        self.AppId = None
+
+
+    def _deserialize(self, params):
+        self.CdnBytes = params.get("CdnBytes")
+        self.P2pBytes = params.get("P2pBytes")
+        self.StuckPeople = params.get("StuckPeople")
+        self.StuckTimes = params.get("StuckTimes")
+        self.OnlinePeople = params.get("OnlinePeople")
+        self.Request = params.get("Request")
+        self.RequestSuccess = params.get("RequestSuccess")
+        self.Time = params.get("Time")
+        self.Type = params.get("Type")
+        self.StreamName = params.get("StreamName")
+        self.AppId = params.get("AppId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-live-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.888/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.887/setup.py` & `tencentcloud-sdk-python-live-3.0.888/setup.py`

 * *Files identical despite different names*

