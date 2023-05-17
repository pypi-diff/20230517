# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.892.tar", last modified: Tue May 16 00:41:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.893.tar", last modified: Wed May 17 03:36:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.892.tar` & `tencentcloud-sdk-python-mps-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)    89755 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13373 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)   798995 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/tencentcloud_sdk_python_mps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:41:21.000000 tencentcloud-sdk-python-mps-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)    89755 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13373 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   805554 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:36:05.000000 tencentcloud-sdk-python-mps-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mps-3.0.892/README.rst` & `tencentcloud-sdk-python-mps-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.893/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.892'
+__version__ = '3.0.893'
```

### Comparing `tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/v20190612/mps_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1243,15 +1243,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeTaskDetail(self, request):
-        """通过任务 ID 查询任务的执行状态和结果的详细信息（最多可以查询3天之内提交的任务）。
+        """通过任务 ID 查询任务的执行状态和结果的详细信息（最多可以查询7天之内提交的任务）。
 
         :param request: Request instance for DescribeTaskDetail.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeTaskDetailRequest`
         :rtype: :class:`tencentcloud.mps.v20190612.models.DescribeTaskDetailResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.892/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.893/tencentcloud/mps/v20190612/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1466,15 +1466,16 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type OcrWordsTask: :class:`tencentcloud.mps.v20190612.models.AiRecognitionTaskOcrWordsResult`
         :param OcrFullTextTask: 文本全文识别结果，当 Type 为
  OcrFullTextRecognition 时有效。
 注意：此字段可能返回 null，表示取不到有效值。
         :type OcrFullTextTask: :class:`tencentcloud.mps.v20190612.models.AiRecognitionTaskOcrFullTextResult`
         :param TransTextTask: 翻译结果，当 Type 为
- TransTextRecognition 时有效。
+
+TransTextRecognition 时有效。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TransTextTask: :class:`tencentcloud.mps.v20190612.models.AiRecognitionTaskTransTextResult`
         """
         self.Type = None
         self.FaceTask = None
         self.AsrWordsTask = None
         self.AsrFullTextTask = None
@@ -10313,24 +10314,31 @@
 
     def __init__(self):
         r"""
         :param OutputStorage: 编辑后文件的目标存储。
         :type OutputStorage: :class:`tencentcloud.mps.v20190612.models.TaskOutputStorage`
         :param Path: 编辑后的视频文件路径。
         :type Path: str
+        :param MetaData: 编辑后的视频文件元信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MetaData: :class:`tencentcloud.mps.v20190612.models.MediaMetaData`
         """
         self.OutputStorage = None
         self.Path = None
+        self.MetaData = None
 
 
     def _deserialize(self, params):
         if params.get("OutputStorage") is not None:
             self.OutputStorage = TaskOutputStorage()
             self.OutputStorage._deserialize(params.get("OutputStorage"))
         self.Path = params.get("Path")
+        if params.get("MetaData") is not None:
+            self.MetaData = MediaMetaData()
+            self.MetaData._deserialize(params.get("MetaData"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -12963,26 +12971,36 @@
         :param SamplingRate: 音频流的采样率，单位：hz。
         :type SamplingRate: int
         :param Codec: 音频流的编码格式，例如 aac。
         :type Codec: str
         :param Channel: 音频声道数，例如 2。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Channel: int
+        :param Codecs: 音频Codecs。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Codecs: str
+        :param Loudness: 音频响度。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Loudness: float
         """
         self.Bitrate = None
         self.SamplingRate = None
         self.Codec = None
         self.Channel = None
+        self.Codecs = None
+        self.Loudness = None
 
 
     def _deserialize(self, params):
         self.Bitrate = params.get("Bitrate")
         self.SamplingRate = params.get("SamplingRate")
         self.Codec = params.get("Codec")
         self.Channel = params.get("Channel")
+        self.Codecs = params.get("Codecs")
+        self.Loudness = params.get("Loudness")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13409,34 +13427,44 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 对视频转自适应码流任务的输入。
         :type Input: :class:`tencentcloud.mps.v20190612.models.AdaptiveDynamicStreamingTaskInput`
         :param Output: 对视频转自适应码流任务的输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.mps.v20190612.models.AdaptiveDynamicStreamingInfoItem`
+        :param BeginProcessTime: 任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BeginProcessTime: str
+        :param FinishTime: 任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
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
         
@@ -13458,34 +13486,44 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 转动图任务的输入。
         :type Input: :class:`tencentcloud.mps.v20190612.models.AnimatedGraphicTaskInput`
         :param Output: 转动图任务的输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.mps.v20190612.models.MediaAnimatedGraphicsItem`
+        :param BeginProcessTime: 任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BeginProcessTime: str
+        :param FinishTime: 任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
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
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13507,34 +13545,44 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 对视频截雪碧图任务的输入。
         :type Input: :class:`tencentcloud.mps.v20190612.models.ImageSpriteTaskInput`
         :param Output: 对视频截雪碧图任务的输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.mps.v20190612.models.MediaImageSpriteItem`
+        :param BeginProcessTime: 任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BeginProcessTime: str
+        :param FinishTime: 任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
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
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13703,34 +13751,44 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 对视频做采样截图任务输入。
         :type Input: :class:`tencentcloud.mps.v20190612.models.SampleSnapshotTaskInput`
         :param Output: 对视频做采样截图任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.mps.v20190612.models.MediaSampleSnapshotItem`
+        :param BeginProcessTime: 任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BeginProcessTime: str
+        :param FinishTime: 任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
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
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13752,34 +13810,44 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 对视频按指定时间点截图任务输入。
         :type Input: :class:`tencentcloud.mps.v20190612.models.SnapshotByTimeOffsetTaskInput`
         :param Output: 对视频按指定时间点截图任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.mps.v20190612.models.MediaSnapshotByTimeOffsetItem`
+        :param BeginProcessTime: 任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BeginProcessTime: str
+        :param FinishTime: 任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
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
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -14065,36 +14133,41 @@
         :type ColorSpace: str
         :param ColorTransfer: 色彩空间。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ColorTransfer: str
         :param HdrType: HDR类型。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HdrType: str
+        :param Codecs: 视频Codecs。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Codecs: str
         """
         self.Bitrate = None
         self.Height = None
         self.Width = None
         self.Codec = None
         self.Fps = None
         self.ColorPrimaries = None
         self.ColorSpace = None
         self.ColorTransfer = None
         self.HdrType = None
+        self.Codecs = None
 
 
     def _deserialize(self, params):
         self.Bitrate = params.get("Bitrate")
         self.Height = params.get("Height")
         self.Width = params.get("Width")
         self.Codec = params.get("Codec")
         self.Fps = params.get("Fps")
         self.ColorPrimaries = params.get("ColorPrimaries")
         self.ColorSpace = params.get("ColorSpace")
         self.ColorTransfer = params.get("ColorTransfer")
         self.HdrType = params.get("HdrType")
+        self.Codecs = params.get("Codecs")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -17919,21 +17992,29 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 分析任务的输入。
         :type Input: :class:`tencentcloud.mps.v20190612.models.AiAnalysisTaskInput`
         :param Output: 分析任务的输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: list of AiAnalysisResult
+        :param BeginProcessTime: 任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BeginProcessTime: str
+        :param FinishTime: 任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
@@ -17942,14 +18023,16 @@
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = []
             for item in params.get("Output"):
                 obj = AiAnalysisResult()
                 obj._deserialize(item)
                 self.Output.append(obj)
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -18020,21 +18103,29 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 识别任务的输入。
         :type Input: :class:`tencentcloud.mps.v20190612.models.AiRecognitionTaskInput`
         :param Output: 识别任务的输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: list of AiRecognitionResult
+        :param BeginProcessTime: 任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BeginProcessTime: str
+        :param FinishTime: 任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
@@ -18043,14 +18134,16 @@
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = []
             for item in params.get("Output"):
                 obj = AiRecognitionResult()
                 obj._deserialize(item)
                 self.Output.append(obj)
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -18072,21 +18165,29 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 审核任务的输入。
         :type Input: :class:`tencentcloud.mps.v20190612.models.AiContentReviewTaskInput`
         :param Output: 审核任务的输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: list of AiContentReviewResult
+        :param BeginProcessTime: 任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BeginProcessTime: str
+        :param FinishTime: 任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/862/37710#52)。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
@@ -18095,14 +18196,16 @@
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = []
             for item in params.get("Output"):
                 obj = AiContentReviewResult()
                 obj._deserialize(item)
                 self.Output.append(obj)
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -18760,15 +18863,16 @@
     """极速高清参数配置。
 
     """
 
     def __init__(self):
         r"""
         :param Type: 极速高清类型，可选值：
-<li>TEHD-100：极速高清-100。</li>
+<li>TEHD-100：极速高清-100（视频极速高清）。</li>
+<li>TEHD-200：极速高清-200（音频极速高清）。</li>
 不填代表不启用极速高清。
         :type Type: str
         :param MaxVideoBitrate: 视频码率上限，当 Type 指定了极速高清类型时有效。
 不填或填0表示不设视频码率上限。
         :type MaxVideoBitrate: int
         """
         self.Type = None
@@ -18791,15 +18895,16 @@
     """极速高清参数配置。
 
     """
 
     def __init__(self):
         r"""
         :param Type: 极速高清类型，可选值：
-<li>TEHD-100：极速高清-100。</li>
+<li>TEHD-100：极速高清-100（视频极速高清）。</li>
+<li>TEHD-200：极速高清-200（音频极速高清）。</li>
 不填代表不修改。
         :type Type: str
         :param MaxVideoBitrate: 视频码率上限，不填代表不修改。
         :type MaxVideoBitrate: int
         """
         self.Type = None
         self.MaxVideoBitrate = None
```

### Comparing `tencentcloud-sdk-python-mps-3.0.892/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.893/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.893/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.892/setup.py` & `tencentcloud-sdk-python-mps-3.0.893/setup.py`

 * *Files identical despite different names*

