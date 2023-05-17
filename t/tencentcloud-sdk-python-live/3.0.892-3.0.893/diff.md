# Comparing `tmp/tencentcloud-sdk-python-live-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.892.tar", last modified: Tue May 16 00:40:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.893.tar", last modified: Wed May 17 03:34:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.892.tar` & `tencentcloud-sdk-python-live-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137456 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   426940 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:40:11.000000 tencentcloud-sdk-python-live-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137459 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   431116 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:34:52.000000 tencentcloud-sdk-python-live-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.892/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.893/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.892/README.rst` & `tencentcloud-sdk-python-live-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/v20180801/live_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2535,15 +2535,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeUploadStreamNums(self, request):
-        """直播上行路数查询
+        """直播上行路数查询。
 
         :param request: Request instance for DescribeUploadStreamNums.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeUploadStreamNumsRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeUploadStreamNumsResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.892/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.893/tencentcloud/live/v20180801/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,17 @@
     """带宽信息
 
     """
 
     def __init__(self):
         r"""
         :param Time: 返回格式：
-yyyy-mm-dd HH:MM:SS
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
 根据粒度会有不同程度的缩减。
         :type Time: str
         :param Bandwidth: 带宽。
         :type Bandwidth: float
         """
         self.Time = None
         self.Bandwidth = None
@@ -420,21 +422,28 @@
 class BillDataInfo(AbstractModel):
     """带宽和流量信息。
 
     """
 
     def __init__(self):
         r"""
-        :param Time: 时间点，格式: yyyy-mm-dd HH:MM:SS。
+        :param Time: 时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type Time: str
         :param Bandwidth: 带宽，单位是 Mbps。
         :type Bandwidth: float
         :param Flux: 流量，单位是 MB。
         :type Flux: float
-        :param PeakTime: 峰值时间点，格式: yyyy-mm-dd HH:MM:SS，原始数据为5分钟粒度，如果查询小时和天粒度数据，则返回对应粒度内的带宽峰值时间点。
+        :param PeakTime: 峰值时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
+原始数据为5分钟粒度，如果查询小时和天粒度数据，则返回对应粒度内的带宽峰值时间点。
         :type PeakTime: str
         """
         self.Time = None
         self.Bandwidth = None
         self.Flux = None
         self.PeakTime = None
 
@@ -658,15 +667,18 @@
 class CdnPlayStatData(AbstractModel):
     """下行播放统计指标
 
     """
 
     def __init__(self):
         r"""
-        :param Time: 时间点，格式: yyyy-mm-dd HH:MM:SS。
+        :param Time: 时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type Time: str
         :param Bandwidth: 带宽，单位: Mbps。
         :type Bandwidth: float
         :param Flux: 流量，单位: MB。
         :type Flux: float
         :param Request: 新增请求数。
         :type Request: int
@@ -3570,17 +3582,22 @@
 class DescribeBillBandwidthAndFluxListRequest(AbstractModel):
     """DescribeBillBandwidthAndFluxList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param StartTime: 起始时间点，格式为yyyy-mm-dd HH:MM:SS。
+        :param StartTime: 起始时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
         :type StartTime: str
-        :param EndTime: 结束时间点，格式为yyyy-mm-dd HH:MM:SS，起始和结束时间跨度不支持超过31天。支持最近3年的数据查询
+        :param EndTime: 结束时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
+起始和结束时间跨度不支持超过31天。支持最近3年的数据查询
         :type EndTime: str
         :param PlayDomains: 直播播放域名，若不填，表示总体数据。
         :type PlayDomains: list of str
         :param MainlandOrOversea: 可选值：
 Mainland：查询国内数据，
 Oversea：则查询国外数据，
 默认：查询国内+国外的数据。
@@ -3635,19 +3652,23 @@
 class DescribeBillBandwidthAndFluxListResponse(AbstractModel):
     """DescribeBillBandwidthAndFluxList返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param PeakBandwidthTime: 峰值带宽所在时间点，格式为yyyy-mm-dd HH:MM:SS。
+        :param PeakBandwidthTime: 峰值带宽所在时间点，接口返回支持两种时间格式(与接口请求传递的时间格式一致)：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
         :type PeakBandwidthTime: str
         :param PeakBandwidth: 峰值带宽，单位是Mbps。
         :type PeakBandwidth: float
-        :param P95PeakBandwidthTime: 95峰值带宽所在时间点，格式为yyyy-mm-dd HH:MM:SS。
+        :param P95PeakBandwidthTime: 95峰值带宽所在时间点，接口返回支持两种时间格式(与接口请求传递的时间格式一致)：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
         :type P95PeakBandwidthTime: str
         :param P95PeakBandwidth: 95峰值带宽，单位是Mbps。
         :type P95PeakBandwidth: float
         :param SumFlux: 总流量，单位是MB。
         :type SumFlux: float
         :param DataInfoList: 明细数据信息。
         :type DataInfoList: list of BillDataInfo
@@ -3779,18 +3800,22 @@
     """
 
     def __init__(self):
         r"""
         :param LiveType: 直播类型，SlowLive：慢直播。
 NormalLive：普通直播。
         :type LiveType: str
-        :param StartTime: 起始时间，格式：yyyy-mm-dd HH:MM:SS。
+        :param StartTime: 起始时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
 可以查询最近180天的数据。
         :type StartTime: str
-        :param EndTime: 结束时间，格式：yyyy-mm-dd HH:MM:SS。
+        :param EndTime: 结束时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
 时间跨度最大支持31天。
         :type EndTime: str
         :param MainlandOrOversea: 如果为空，查询所有地区数据；如果为“Mainland”，查询国内数据；如果为“Oversea”，则查询国外数据。
         :type MainlandOrOversea: str
         :param PushDomains: 推流域名列表，不填表示总体数据。
         :type PushDomains: list of str
         """
@@ -3845,17 +3870,22 @@
 class DescribeDeliverBandwidthListRequest(AbstractModel):
     """DescribeDeliverBandwidthList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param StartTime: 起始时间，格式为%Y-%m-%d %H:%M:%S。
+        :param StartTime: 起始时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
         :type StartTime: str
-        :param EndTime: 结束时间，格式为%Y-%m-%d %H:%M:%S，支持最近三个月的数据查询，时间跨度最大是1个月。
+        :param EndTime: 结束时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
+支持最近三个月的数据查询，时间跨度最大是1个月。
         :type EndTime: str
         """
         self.StartTime = None
         self.EndTime = None
 
 
     def _deserialize(self, params):
@@ -6045,19 +6075,22 @@
 class DescribeLiveTranscodeTotalInfoRequest(AbstractModel):
     """DescribeLiveTranscodeTotalInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param StartTime: 开始时间，北京时间。
-格式：yyyy-mm-dd HH:MM:SS。
+        :param StartTime: 结束时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
         :type StartTime: str
-        :param EndTime: 结束时间，北京时间。
-格式：yyyy-mm-dd HH:MM:SS。
+        :param EndTime: 结束时间，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type EndTime: str
         :param PushDomains: 推流域名列表，若不填，表示查询所有域名总体数据。
 指定域名时返回1小时粒度数据。
         :type PushDomains: list of str
         :param MainlandOrOversea: 可选值：
 Mainland：查询中国大陆（境内）数据，
 Oversea：则查询国际/港澳台（境外）数据，
@@ -7015,17 +7048,22 @@
 class DescribeScreenShotSheetNumListRequest(AbstractModel):
     """DescribeScreenShotSheetNumList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param StartTime: utc起始时间，格式为yyyy-mm-ddTHH:MM:SSZ
+        :param StartTime: 起始时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
         :type StartTime: str
-        :param EndTime: utc结束时间，格式为yyyy-mm-ddTHH:MM:SSZ，支持查询最近1年数据。
+        :param EndTime: 结束时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
+支持查询最近1年的数据。
         :type EndTime: str
         :param Zone: 地域信息，可选值包括Mainland，Oversea，前者是查询中国大陆范围内的数据，后者是除中国大陆范围之外的数据，若不传该参数，则查询所有地区的数据。
         :type Zone: str
         :param PushDomains: 推流域名（支持查询2019年11 月1日之后的域名维度数据）。
         :type PushDomains: list of str
         :param Granularity: 数据维度，数据延迟1个半小时，可选值包括：1、Minute（5分钟粒度，最大支持查询时间范围是31天），2、Day（天粒度，默认值，按照北京时间做跨天处理，最大支持查询时间范围是186天当天）。
         :type Granularity: str
@@ -7698,17 +7736,22 @@
 class DescribeUploadStreamNumsRequest(AbstractModel):
     """DescribeUploadStreamNums请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param StartTime: 起始时间点，格式为yyyy-mm-dd HH:MM:SS。
+        :param StartTime: 起始时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
         :type StartTime: str
-        :param EndTime: 结束时间点，格式为yyyy-mm-dd HH:MM:SS，起始和结束时间跨度不支持超过31天。支持最近31天的数据查询
+        :param EndTime: 结束时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
+起始和结束时间跨度不支持超过31天。支持最近31天的数据查询
         :type EndTime: str
         :param Domains: 直播域名，若不填，表示总体数据。
         :type Domains: list of str
         :param Granularity: 数据粒度，支持如下粒度：
 5：5分钟粒度，（跨度不支持超过1天），
 1440：天粒度（跨度不支持超过一个月）。
 默认值：5。
@@ -12038,16 +12081,18 @@
 class TranscodeTotalInfo(AbstractModel):
     """转码总量数据
 
     """
 
     def __init__(self):
         r"""
-        :param Time: 时间点，北京时间，
-示例：2019-03-01 00:00:00。
+        :param Time: 时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type Time: str
         :param Duration: 转码时长，单位：分钟。
         :type Duration: int
         :param ModuleCodec: 编码方式，带模块，
 示例：
 liveprocessor_H264 =》直播转码-H264，
 liveprocessor_H265 =》 直播转码-H265，
```

### Comparing `tencentcloud-sdk-python-live-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.893/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.892/setup.py` & `tencentcloud-sdk-python-live-3.0.893/setup.py`

 * *Files identical despite different names*

