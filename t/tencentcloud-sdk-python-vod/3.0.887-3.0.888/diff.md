# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.887.tar", last modified: Tue May  9 03:24:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.888.tar", last modified: Wed May 10 02:59:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.887.tar` & `tencentcloud-sdk-python-vod-3.0.888.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1171923 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:24:55.000000 tencentcloud-sdk-python-vod-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:59:31.000000 tencentcloud-sdk-python-vod-3.0.888/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   172410 2023-05-10 02:59:31.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1175809 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:59:31.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:59:31.000000 tencentcloud-sdk-python-vod-3.0.888/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:59:32.000000 tencentcloud-sdk-python-vod-3.0.888/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.887/README.rst` & `tencentcloud-sdk-python-vod-3.0.888/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.887/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.888/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14202,30 +14202,38 @@
         :param FillType: 填充方式，当视频流配置宽高参数与原始视频的宽高比不一致时，对转码的处理方式，即为“填充”。可选填充方式：
 <li> stretch：拉伸，对每一帧进行拉伸，填满整个画面，可能导致转码后的视频被“压扁“或者“拉长“；</li>
 <li> gauss：高斯模糊，保持视频宽高比不变，边缘剩余部分使用高斯模糊；</li>
 <li> white：留白，保持视频宽高比不变，边缘剩余部分使用白色填充；</li>
 <li> black：留黑，保持视频宽高比不变，边缘剩余部分使用黑色填充。</li>
 默认值：stretch 。
         :type FillType: str
+        :param CreateTime: 模板创建时间，使用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type CreateTime: str
+        :param UpdateTime: 模板最后修改时间，使用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type UpdateTime: str
         """
         self.Definition = None
         self.Name = None
         self.Comment = None
         self.HeadCandidateSet = None
         self.TailCandidateSet = None
         self.FillType = None
+        self.CreateTime = None
+        self.UpdateTime = None
 
 
     def _deserialize(self, params):
         self.Definition = params.get("Definition")
         self.Name = params.get("Name")
         self.Comment = params.get("Comment")
         self.HeadCandidateSet = params.get("HeadCandidateSet")
         self.TailCandidateSet = params.get("TailCandidateSet")
         self.FillType = params.get("FillType")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16477,36 +16485,44 @@
         :type Message: str
         :param Progress: 转自适应码流任务进度，取值范围 [0-100] 。
         :type Progress: int
         :param Input: 对视频转自适应码流任务的输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AdaptiveDynamicStreamingTaskInput`
         :param Output: 对视频转自适应码流任务的输出。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AdaptiveDynamicStreamingInfoItem`
+        :param BeginProcessTime: 转自适应码流任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 转自适应码流任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Progress = None
         self.Input = None
         self.Output = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         self.Progress = params.get("Progress")
         if params.get("Input") is not None:
             self.Input = AdaptiveDynamicStreamingTaskInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AdaptiveDynamicStreamingInfoItem()
             self.Output._deserialize(params.get("Output"))
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16530,36 +16546,44 @@
         :param Input: 转动图任务的输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AnimatedGraphicTaskInput`
         :param Output: 转动图任务的输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.MediaAnimatedGraphicsItem`
         :param Progress: 转动图任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 转动图任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 转动图任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AnimatedGraphicTaskInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = MediaAnimatedGraphicsItem()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16582,36 +16606,44 @@
         :type Message: str
         :param Input: 对视频截图做封面任务的输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.CoverBySnapshotTaskInput`
         :param Output: 对视频截图做封面任务的输出。
         :type Output: :class:`tencentcloud.vod.v20180717.models.CoverBySnapshotTaskOutput`
         :param Progress: 对视频截图做封面任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 截图做封面任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 截图做封面任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = CoverBySnapshotTaskInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = CoverBySnapshotTaskOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16635,36 +16667,44 @@
         :param Input: 对视频截雪碧图任务的输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.ImageSpriteTaskInput`
         :param Output: 对视频截雪碧图任务的输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.MediaImageSpriteItem`
         :param Progress: 对视频截雪碧图任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 截雪碧图任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 截雪碧图任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = ImageSpriteTaskInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = MediaImageSpriteItem()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16851,36 +16891,44 @@
         :param Input: 对视频做采样截图任务输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.SampleSnapshotTaskInput`
         :param Output: 对视频做采样截图任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.MediaSampleSnapshotItem`
         :param Progress: 对视频做采样截图任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 采样截图任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 采样截图任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = SampleSnapshotTaskInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = MediaSampleSnapshotItem()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -16904,36 +16952,44 @@
         :param Input: 对视频按指定时间点截图任务输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.SnapshotByTimeOffsetTaskInput`
         :param Output: 对视频按指定时间点截图任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.MediaSnapshotByTimeOffsetItem`
         :param Progress: 对视频按指定时间点截图任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 时间点截图任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 时间点截图任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = SnapshotByTimeOffsetTaskInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = MediaSnapshotByTimeOffsetItem()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vod-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.888/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.887/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.888/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.888/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.887
+Version: 3.0.888
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.887/setup.py` & `tencentcloud-sdk-python-vod-3.0.888/setup.py`

 * *Files identical despite different names*

