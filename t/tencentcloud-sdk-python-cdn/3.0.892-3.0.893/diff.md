# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.892.tar", last modified: Tue May 16 00:30:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.893.tar", last modified: Wed May 17 03:25:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.892.tar` & `tencentcloud-sdk-python-cdn-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21972 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   568745 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:30:55.000000 tencentcloud-sdk-python-cdn-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   569936 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:25:34.000000 tencentcloud-sdk-python-cdn-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.892/README.rst` & `tencentcloud-sdk-python-cdn-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.892/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud/cdn/v20180606/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -957,15 +957,17 @@
         :type Action: str
         :param RedirectUrl: 动作为 redirect 时，重定向的url
 注意：此字段可能返回 null，表示取不到有效值。
         :type RedirectUrl: str
         :param Configure: 七层限频具体配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type Configure: list of ScdnSevenLayerRules
-        :param Switch: 是否开启改规则 on 开启，off关闭
+        :param Switch: 自定义cc规则配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.RuleName = None
         self.DetectionTime = None
         self.FrequencyLimit = None
         self.PunishmentSwitch = None
@@ -10877,14 +10879,15 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type Origins: list of str
         :param OriginType: 主源站类型
 入参支持以下几种类型：
 domain：域名类型
 domainv6：域名解析V6类型
 cos：对象存储源站
+third_party: 第三方存储源站
 ip：IP 列表作为源站
 ipv6：源站列表为一个单独的 IPv6 地址
 ip_ipv6：源站列表为多个 IPv4 地址和IPv6 地址
 ip_domain: 支持IP和域名形式源站混填（白名单功能）
 ip_domainv6：源站列表为多个 IPv4 地址以及域名解析v6地址
 ipv6_domain: 源站列表为多个 IPv6 地址以及域名
 ipv6_domainv6：源站列表为多个 IPv6 地址以及域名解析v6地址
@@ -10942,15 +10945,20 @@
         :type PathRules: list of PathRule
         :param PathBasedOrigin: 分路径回源配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type PathBasedOrigin: list of PathBasedOriginRule
         :param AdvanceHttps: HTTPS回源高级配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type AdvanceHttps: :class:`tencentcloud.cdn.v20180606.models.AdvanceHttps`
-        :param OriginCompany: 对象存储回源厂商
+        :param OriginCompany: 对象存储回源厂商，当源站类型为第三方存储源站(third_party)时必填，可选值包括以下:
+aws_s3: AWS S3
+ali_oss: 阿里云 OSS
+hw_obs: 华为 OBS
+qiniu_kodo: 七牛云 kodo
+others: 其它厂商对象存储,仅支持兼容以AWS签名算法的对象存储，如腾讯云金融专区COS
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginCompany: str
         """
         self.Origins = None
         self.OriginType = None
         self.ServerName = None
         self.CosPrivateAccess = None
@@ -11971,21 +11979,27 @@
 class QueryStringKey(AbstractModel):
     """组成CacheKey的一部分
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on | off CacheKey是否由QueryString组成
+        :param Switch: CacheKey是否由QueryString组成配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param Reorder: 是否重新排序
 注意：此字段可能返回 null，表示取不到有效值。
         :type Reorder: str
-        :param Action: includeAll | excludeAll | includeCustom | excludeCustom 使用/排除部分url参数
+        :param Action: 使用/排除部分url参数，取值有：
+includeAll：包含所有
+excludeAll：排除所有
+includeCustom：自定义包含
+excludeCustom：自定义排除
 注意：此字段可能返回 null，表示取不到有效值。
         :type Action: str
         :param Value: 使用/排除的url参数数组，';' 分割
 注意：此字段可能返回 null，表示取不到有效值。
         :type Value: str
         """
         self.Switch = None
@@ -13033,15 +13047,17 @@
         :type Qps: int
         :param DetectionTime: 探测时长
 注意：此字段可能返回 null，表示取不到有效值。
         :type DetectionTime: int
         :param FrequencyLimit: 限频阈值
 注意：此字段可能返回 null，表示取不到有效值。
         :type FrequencyLimit: int
-        :param PunishmentSwitch: IP 惩罚开关，可选on|off
+        :param PunishmentSwitch: IP 惩罚配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type PunishmentSwitch: str
         :param PunishmentTime: IP 惩罚时长
 注意：此字段可能返回 null，表示取不到有效值。
         :type PunishmentTime: int
         :param Action: 执行动作，intercept|redirect
 注意：此字段可能返回 null，表示取不到有效值。
@@ -13083,15 +13099,17 @@
 class ScdnConfig(AbstractModel):
     """cc的配置类型
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on | off
+        :param Switch: scdn cc配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param Rules: 自定义 cc 防护规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type Rules: list of ScdnCCRules
         :param AdvancedRules: 增强自定义 cc 防护规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type AdvancedRules: list of AdvancedCCRules
@@ -13137,15 +13155,17 @@
 class ScdnDdosConfig(AbstractModel):
     """ddos配置类型
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on|off
+        :param Switch: Scdn ddos配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
@@ -13674,32 +13694,38 @@
 class ScdnWafConfig(AbstractModel):
     """waf配置类型
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on|off
+        :param Switch: Scdn waf配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param Mode: intercept|observe，默认intercept
 注意：此字段可能返回 null，表示取不到有效值。
         :type Mode: str
         :param ErrorPage: 重定向的错误页面
 注意：此字段可能返回 null，表示取不到有效值。
         :type ErrorPage: :class:`tencentcloud.cdn.v20180606.models.ScdnErrorPage`
-        :param WebShellSwitch: webshell拦截开关，on|off，默认off
+        :param WebShellSwitch: webshell拦截配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type WebShellSwitch: str
         :param Rules: 类型拦截规则
 注意：此字段可能返回 null，表示取不到有效值。
         :type Rules: list of ScdnWafRule
         :param Level: waf规则等级，可取100|200|300
 注意：此字段可能返回 null，表示取不到有效值。
         :type Level: int
-        :param SubRuleSwitch: waf子规则开关
+        :param SubRuleSwitch: waf子规则配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type SubRuleSwitch: list of WafSubRuleStatus
         """
         self.Switch = None
         self.Mode = None
         self.ErrorPage = None
         self.WebShellSwitch = None
@@ -13768,15 +13794,17 @@
 class SchemeKey(AbstractModel):
     """作为CacheKey的一部分
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on | off 是否使用scheme作为cache key的一部分
+        :param Switch: scheme作为cache key配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
@@ -13872,15 +13900,17 @@
 class SecurityConfig(AbstractModel):
     """scdn相关的配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: on|off
+        :param Switch: scdn 安全配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
@@ -13896,15 +13926,15 @@
 class Seo(AbstractModel):
     """SEO 搜索引擎优化配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: SEO 配置开关
+        :param Switch: SEO 搜索引擎优化配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Switch = None
 
@@ -13985,22 +14015,24 @@
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ShareCname(AbstractModel):
     """ShareCname配置
+    ShareCname 为内测功能,如需使用,请联系腾讯云工程师开白.
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: ShareCname 配置开关, 开关为off时，域名使用默认CNAME，若需要使用共享CNAME，将开关置为on.
+        :param Switch: ShareCname 配置开关, 取值有：
+on：开启，使用共享CNAME
+off：关闭，使用默认CNAME
 
-* ShareCname 为内测功能,如需使用,请联系腾讯云工程师开白.
         :type Switch: str
         :param Cname: 设置共享CNAME.
 注意：此字段可能返回 null，表示取不到有效值。
         :type Cname: str
         """
         self.Switch = None
         self.Cname = None
@@ -14304,24 +14336,28 @@
         :type BpsThreshold: int
         :param CounterMeasure: 关闭方式 返回404:RETURN_404, dns回源：RESOLVE_DNS_TO_ORIGIN
 注意：此字段可能返回 null，表示取不到有效值。
         :type CounterMeasure: str
         :param AlertPercentage: 触发提醒阈值百分比
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlertPercentage: int
-        :param AlertSwitch: 提醒开关 on/off
+        :param AlertSwitch: 累计用量封顶告警配置，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type AlertSwitch: str
         :param Metric: 指标类型，流量flux或带宽bandwidth
 注意：此字段可能返回 null，表示取不到有效值。
         :type Metric: str
         :param Cycle: 检测周期，单位分钟，60或1440
 注意：此字段可能返回 null，表示取不到有效值。
         :type Cycle: int
-        :param Switch: 是否开启该选项，on/off
+        :param Switch: 累计用量封顶配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Type = None
         self.UnBlockTime = None
         self.BpsThreshold = None
         self.CounterMeasure = None
@@ -14354,15 +14390,15 @@
 class StatusCodeCache(AbstractModel):
     """状态码缓存过期配置，默认情况下会对 404 状态码缓存 10 秒
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 状态码缓存过期配置开关
+        :param Switch: 状态码缓存过期配置开关，取值有：
 on：开启
 off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param CacheRules: 状态码缓存过期规则明细
 注意：此字段可能返回 null，表示取不到有效值。
         :type CacheRules: list of StatusCodeCacheRule
@@ -14775,15 +14811,17 @@
 class TpgAdapter(AbstractModel):
     """图片优化-TpgAdapter配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关，"on/off"
+        :param Switch: 图片优化-TpgAdapter配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
@@ -15471,15 +15509,15 @@
 class UrlRedirect(AbstractModel):
     """访问URL重写配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 访问URL重写配置开关
+        :param Switch: 访问URL重写配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         :param PathRules: 访问URL重写规则，当Switch为on时必填，规则数量最大为10个。
 注意：此字段可能返回 null，表示取不到有效值。
         :type PathRules: list of UrlRedirectRule
         """
@@ -15549,15 +15587,17 @@
 class UserAgentFilter(AbstractModel):
     """UserAgent黑白名单配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关，on或off
+        :param Switch: UserAgent黑白名单配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         :param FilterRules: UA黑白名单生效规则列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type FilterRules: list of UserAgentFilterRule
         """
         self.Switch = None
@@ -15679,15 +15719,15 @@
 class VideoSeek(AbstractModel):
     """视频拖拽配置，默认为关闭状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 视频拖拽开关
+        :param Switch: 视频拖拽配置开关，取值有：
 on：开启
 off：关闭
         :type Switch: str
         """
         self.Switch = None
 
 
@@ -15754,15 +15794,17 @@
 class WafSubRuleStatus(AbstractModel):
     """Waf子规则开关状态
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 子规则状态，on|off
+        :param Switch: Waf子规则开关状态配置开关，取值有：
+on：开启
+off：关闭
         :type Switch: str
         :param SubIds: 规则id列表
         :type SubIds: list of int
         """
         self.Switch = None
         self.SubIds = None
 
@@ -15777,22 +15819,24 @@
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class WebSocket(AbstractModel):
     """WebSocket配置
+    WebSocket 为ECDN产品功能，如需使用请通过ECDN域名配置.
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: WebSocket 超时配置开关, 开关为off时，平台仍支持WebSocket连接，此时超时时间默认为15秒，若需要调整超时时间，将开关置为on.
+        :param Switch: WebSocket 超时配置开关，取值有：
+on：开启，可以调整超时时间
+off：关闭，平台仍支持WebSocket连接，此时超时时间默认为15秒
 
-* WebSocket 为ECDN产品功能，如需使用请通过ECDN域名配置.
         :type Switch: str
         :param Timeout: 设置超时时间，单位为秒，最大超时时间300秒。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Timeout: int
         """
         self.Switch = None
         self.Timeout = None
@@ -15813,15 +15857,17 @@
 class WebpAdapter(AbstractModel):
     """图片优化-WebpAdapter配置
 
     """
 
     def __init__(self):
         r"""
-        :param Switch: 开关，"on/off"
+        :param Switch: 图片优化-WebpAdapter配置开关，取值有：
+on：开启
+off：关闭
 注意：此字段可能返回 null，表示取不到有效值。
         :type Switch: str
         """
         self.Switch = None
 
 
     def _deserialize(self, params):
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.893/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.892/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.893/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.892/setup.py` & `tencentcloud-sdk-python-cdn-3.0.893/setup.py`

 * *Files identical despite different names*

