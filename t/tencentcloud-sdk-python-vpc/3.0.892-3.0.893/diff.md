# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.892.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.892.tar", last modified: Tue May 16 00:50:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.893.tar", last modified: Wed May 17 03:45:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.892.tar` & `tencentcloud-sdk-python-vpc-3.0.893.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   330068 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41334 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   844283 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-16 00:50:45.000000 tencentcloud-sdk-python-vpc-3.0.892/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332014 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41601 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   849420 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:45:12.000000 tencentcloud-sdk-python-vpc-3.0.893/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.892/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.893/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.892/README.rst` & `tencentcloud-sdk-python-vpc-3.0.893/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2420,14 +2420,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteTrafficPackages(self, request):
+        """删除共享带宽包（仅非活动状态的流量包可删除）。
+
+        :param request: Request instance for DeleteTrafficPackages.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteTrafficPackagesRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.DeleteTrafficPackagesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteTrafficPackages", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteTrafficPackagesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteVpc(self, request):
         """本接口（DeleteVpc）用于删除私有网络。
         * 删除前请确保 VPC 内已经没有相关资源，例如云服务器、云数据库、NoSQL、VPN网关、专线网关、负载均衡、对等连接、与之互通的基础网络设备等。
         * 删除私有网络是不可逆的操作，请谨慎处理。
 
         :param request: Request instance for DeleteVpc.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpcRequest`
@@ -3993,14 +4016,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeSubnetResourceDashboard(self, request):
+        """本接口(DescribeSubnetResourceDashboard)用于查看Subnet资源信息。
+
+        :param request: Request instance for DescribeSubnetResourceDashboard.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSubnetResourceDashboardRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeSubnetResourceDashboardResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeSubnetResourceDashboard", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeSubnetResourceDashboardResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSubnets(self, request):
         """本接口（DescribeSubnets）用于查询子网列表。
 
         :param request: Request instance for DescribeSubnets.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSubnetsRequest`
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,14 +394,20 @@
 
 # 无效参数值。参数值太长。
 INVALIDPARAMETERVALUE_TOOLONG = 'InvalidParameterValue.TooLong'
 
 # 该流量包ID不合法。
 INVALIDPARAMETERVALUE_TRAFFICPACKAGEIDMALFORMED = 'InvalidParameterValue.TrafficPackageIdMalformed'
 
+# 未查询到此流量包。
+INVALIDPARAMETERVALUE_TRAFFICPACKAGENOTFOUND = 'InvalidParameterValue.TrafficPackageNotFound'
+
+# 指定的流量包不支持此操作
+INVALIDPARAMETERVALUE_TRAFFICPACKAGENOTSUPPORTED = 'InvalidParameterValue.TrafficPackageNotSupported'
+
 # 该可用区不可用。
 INVALIDPARAMETERVALUE_UNAVAILABLEZONE = 'InvalidParameterValue.UnavailableZone'
 
 # 目的网段和当前VPC的CIDR冲突。
 INVALIDPARAMETERVALUE_VPCCIDRCONFLICT = 'InvalidParameterValue.VpcCidrConflict'
 
 # 当前功能不支持此专线网关。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7265,14 +7265,55 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteTrafficPackagesRequest(AbstractModel):
+    """DeleteTrafficPackages请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TrafficPackageIds: 待删除的流量包唯一ID数组
+        :type TrafficPackageIds: list of str
+        """
+        self.TrafficPackageIds = None
+
+
+    def _deserialize(self, params):
+        self.TrafficPackageIds = params.get("TrafficPackageIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteTrafficPackagesResponse(AbstractModel):
+    """DeleteTrafficPackages返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteVpcEndPointRequest(AbstractModel):
     """DeleteVpcEndPoint请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11683,14 +11724,64 @@
                 obj = SnapshotPolicy()
                 obj._deserialize(item)
                 self.SnapshotPolicySet.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeSubnetResourceDashboardRequest(AbstractModel):
+    """DescribeSubnetResourceDashboard请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SubnetIds: Subnet实例ID，例如：subnet-f1xjkw1b。
+        :type SubnetIds: list of str
+        """
+        self.SubnetIds = None
+
+
+    def _deserialize(self, params):
+        self.SubnetIds = params.get("SubnetIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeSubnetResourceDashboardResponse(AbstractModel):
+    """DescribeSubnetResourceDashboard返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ResourceStatisticsSet: 资源统计结果。
+        :type ResourceStatisticsSet: list of ResourceStatistics
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ResourceStatisticsSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("ResourceStatisticsSet") is not None:
+            self.ResourceStatisticsSet = []
+            for item in params.get("ResourceStatisticsSet"):
+                obj = ResourceStatistics()
+                obj._deserialize(item)
+                self.ResourceStatisticsSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeSubnetsRequest(AbstractModel):
     """DescribeSubnets请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -21087,14 +21178,87 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class ResourceStatistics(AbstractModel):
+    """资源统计信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpcId: Vpc实例ID，例如：vpc-f1xjkw1b。
+        :type VpcId: str
+        :param SubnetId: 子网实例ID，例如：subnet-bthucmmy。
+        :type SubnetId: str
+        :param Ip: 当前已使用的IP总数。
+        :type Ip: int
+        :param ResourceStatisticsItemSet: 资源统计信息。
+        :type ResourceStatisticsItemSet: list of ResourceStatisticsItem
+        """
+        self.VpcId = None
+        self.SubnetId = None
+        self.Ip = None
+        self.ResourceStatisticsItemSet = None
+
+
+    def _deserialize(self, params):
+        self.VpcId = params.get("VpcId")
+        self.SubnetId = params.get("SubnetId")
+        self.Ip = params.get("Ip")
+        if params.get("ResourceStatisticsItemSet") is not None:
+            self.ResourceStatisticsItemSet = []
+            for item in params.get("ResourceStatisticsItemSet"):
+                obj = ResourceStatisticsItem()
+                obj._deserialize(item)
+                self.ResourceStatisticsItemSet.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ResourceStatisticsItem(AbstractModel):
+    """资源统计项。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ResourceType: 资源类型。比如，CVM，ENI等。
+        :type ResourceType: str
+        :param ResourceName: 资源名称。
+        :type ResourceName: str
+        :param ResourceCount: 资源个数。
+        :type ResourceCount: int
+        """
+        self.ResourceType = None
+        self.ResourceName = None
+        self.ResourceCount = None
+
+
+    def _deserialize(self, params):
+        self.ResourceType = params.get("ResourceType")
+        self.ResourceName = params.get("ResourceName")
+        self.ResourceCount = params.get("ResourceCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class ResumeSnapshotInstanceRequest(AbstractModel):
     """ResumeSnapshotInstance请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.892/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.893/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.892/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.893/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.892
+Version: 3.0.893
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.892/setup.py` & `tencentcloud-sdk-python-vpc-3.0.893/setup.py`

 * *Files identical despite different names*

