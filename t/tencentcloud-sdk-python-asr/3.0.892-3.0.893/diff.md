# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.892.tar", last modified: Tue May 16 00:28:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.893.tar", last modified: Wed May 17 03:22:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.892.tar` & `tencentcloud-sdk-python-asr-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:27:59.000000 tencentcloud-sdk-python-asr-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)    24780 2023-05-16 00:27:59.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-05-16 00:27:59.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:27:59.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64121 2023-05-16 00:27:59.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:27:59.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:27:59.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:27:59.000000 tencentcloud-sdk-python-asr-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:28:00.000000 tencentcloud-sdk-python-asr-3.0.892/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:22:39.000000 tencentcloud-sdk-python-asr-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)    24780 2023-05-17 03:22:39.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-05-17 03:22:39.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:22:39.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64128 2023-05-17 03:22:39.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:22:39.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:22:39.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:22:39.000000 tencentcloud-sdk-python-asr-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:22:40.000000 tencentcloud-sdk-python-asr-3.0.893/tencentcloud_sdk_python_asr.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-asr-3.0.892/README.rst` & `tencentcloud-sdk-python-asr-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.892/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.893/tencentcloud/asr/v20190614/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1264,29 +1264,29 @@
 • 8k_en：英文电话通用；
 
 非电话场景：
 • 16k_zh：中文通用；
 • 16k_zh-PY：中英粤;
 • 16k_zh_medical：中文医疗；
 • 16k_en：英语；
-• 16k_ca：粤语；
+• 16k_yue：粤语；
 • 16k_ja：日语；
 • 16k_ko：韩语；
 • 16k_vi：越南语；
 • 16k_ms：马来语；
 • 16k_id：印度尼西亚语；
 • 16k_fil：菲律宾语；
 • 16k_th：泰语；
 • 16k_pt：葡萄牙语；
 • 16k_tr：土耳其语；
 • 16k_zh_dialect：多方言，支持23种方言（上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话）；
         :type EngSerViceType: str
         :param SourceType: 语音数据来源。0：语音 URL；1：语音数据（post body）。
         :type SourceType: int
-        :param VoiceFormat: 识别音频的音频格式，支持wav、pcm、ogg-opus、speex、silk、mp3、m4a、aac。
+        :param VoiceFormat: 识别音频的音频格式，支持wav、pcm、ogg-opus、speex、silk、mp3、m4a、aac、amr。
         :type VoiceFormat: str
         :param ProjectId: 腾讯云项目 ID，废弃参数，填写0即可。
         :type ProjectId: int
         :param SubServiceType: 子服务类型。2： 一句话识别。
         :type SubServiceType: int
         :param Url: 语音的URL地址，需要公网环境浏览器可下载。当 SourceType 值为 0时须填写该字段，为 1 时不填。音频时长不能超过60s，音频文件大小不能超过3MB。
         :type Url: str
```

### Comparing `tencentcloud-sdk-python-asr-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.893/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.892/setup.py` & `tencentcloud-sdk-python-asr-3.0.893/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.892/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.893/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

