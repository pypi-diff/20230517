# Comparing `tmp/iam_actions-1.2.20230516.tar.gz` & `tmp/iam_actions-1.2.20230517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230516.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230517.tar", max compression
```

## Comparing `iam_actions-1.2.20230516.tar` & `iam_actions-1.2.20230517.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/README.md
--rw-r--r--   0        0        0      228 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/__init__.py
--rw-r--r--   0        0        0  4254822 2023-05-16 02:29:44.205357 iam_actions-1.2.20230516/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-16 02:27:58.050835 iam_actions-1.2.20230516/iam_actions/generate/services.py
--rw-r--r--   0        0        0   547148 2023-05-16 02:29:44.205357 iam_actions-1.2.20230516/iam_actions/policies.json
--rw-r--r--   0        0        0   193861 2023-05-16 02:29:44.205357 iam_actions-1.2.20230516/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   530747 2023-05-16 02:29:44.205357 iam_actions-1.2.20230516/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-16 02:29:44.937375 iam_actions-1.2.20230516/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230516/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230516/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/README.md
+-rw-r--r--   0        0        0      228 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4256968 2023-05-17 02:30:00.911258 iam_actions-1.2.20230517/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-17 02:28:03.509560 iam_actions-1.2.20230517/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   547398 2023-05-17 02:30:00.911258 iam_actions-1.2.20230517/iam_actions/policies.json
+-rw-r--r--   0        0        0   193861 2023-05-17 02:30:00.911258 iam_actions-1.2.20230517/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   530991 2023-05-17 02:30:00.911258 iam_actions-1.2.20230517/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-17 02:30:01.775299 iam_actions-1.2.20230517/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230517/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230517/PKG-INFO
```

### Comparing `iam_actions-1.2.20230516/LICENSE` & `iam_actions-1.2.20230517/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/README.md` & `iam_actions-1.2.20230517/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/iam_actions/actions.json` & `iam_actions-1.2.20230517/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999229788925967%*

 * *Differences: {"'cloud9'": "{'GetMigrationExperiences': OrderedDict([('access_level', 'Undocumented'), "*

 * *             "('action', 'GetMigrationExperiences'), ('condition_keys', []), ('description', 'Not "*

 * *             "Documented by AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'ec2'": "{'GetVerifiedAccessInstanceWebAcl': OrderedDict([('access_level', 'Undocumented'), "*

 * *          "('action', 'GetVerifiedAccessInstanceWebAcl'), ('condition_keys', []), ('description', "*

 * *          "'Not Documented by AWS'), ('orphan',  […]*

```diff
@@ -17531,14 +17531,22 @@
             "condition_keys": [],
             "description": "Grants permission to get the AWS Cloud9 IDE settings for a specified environment member",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
+        "GetMigrationExperiences": {
+            "access_level": "Undocumented",
+            "action": "GetMigrationExperiences",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetUserPublicKey": {
             "access_level": "Read",
             "action": "GetUserPublicKey",
             "condition_keys": [
                 "cloud9:UserArn"
             ],
             "description": "Grants permission to get the user's public SSH key, which is used by AWS Cloud9 to connect to SSH development environments",
@@ -42277,14 +42285,22 @@
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to associate a branch network interface with a trunk network interface",
             "orphan": false,
             "resources": []
         },
+        "AssociateVerifiedAccessInstanceWebAcl": {
+            "access_level": "Undocumented",
+            "action": "AssociateVerifiedAccessInstanceWebAcl",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "AssociateVpcCidrBlock": {
             "access_level": "Write",
             "action": "AssociateVpcCidrBlock",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Ipv4IpamPoolId",
                 "ec2:Ipv6IpamPoolId",
@@ -47156,14 +47172,22 @@
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to describe the current logging configuration for the Verified Access instances",
             "orphan": false,
             "resources": []
         },
+        "DescribeVerifiedAccessInstanceWebAclAssociations": {
+            "access_level": "Undocumented",
+            "action": "DescribeVerifiedAccessInstanceWebAclAssociations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeVerifiedAccessInstances": {
             "access_level": "List",
             "action": "DescribeVerifiedAccessInstances",
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to describe the specified Verified Access instances or all Verified Access instances",
@@ -47930,14 +47954,22 @@
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to disassociate a branch network interface to a trunk network interface",
             "orphan": false,
             "resources": []
         },
+        "DisassociateVerifiedAccessInstanceWebAcl": {
+            "access_level": "Undocumented",
+            "action": "DisassociateVerifiedAccessInstanceWebAcl",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DisassociateVpcCidrBlock": {
             "access_level": "Write",
             "action": "DisassociateVpcCidrBlock",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
@@ -48822,14 +48854,22 @@
             ],
             "description": "Grants permission to show the contents of the Verified Access policy associated with the group",
             "orphan": false,
             "resources": [
                 "verified-access-group"
             ]
         },
+        "GetVerifiedAccessInstanceWebAcl": {
+            "access_level": "Undocumented",
+            "action": "GetVerifiedAccessInstanceWebAcl",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetVpnConnectionDeviceSampleConfiguration": {
             "access_level": "List",
             "action": "GetVpnConnectionDeviceSampleConfiguration",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}"
@@ -48847,14 +48887,30 @@
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to obtain a list of customer gateway devices for which sample configuration files can be provided",
             "orphan": false,
             "resources": []
         },
+        "GetVpnTunnelReplacementStatus": {
+            "access_level": "Undocumented",
+            "action": "GetVpnTunnelReplacementStatus",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ImportByoipCidrToIpam": {
+            "access_level": "Undocumented",
+            "action": "ImportByoipCidrToIpam",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ImportClientVpnClientCertificateRevocationList": {
             "access_level": "Write",
             "action": "ImportClientVpnClientCertificateRevocationList",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:ClientRootCertificateChainArn",
                 "ec2:CloudwatchLogGroupArn",
@@ -50825,14 +50881,22 @@
             "description": "Grants permission to replace a route in a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table"
             ]
         },
+        "ReplaceVpnTunnel": {
+            "access_level": "Undocumented",
+            "action": "ReplaceVpnTunnel",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ReportInstanceStatus": {
             "access_level": "Write",
             "action": "ReportInstanceStatus",
             "condition_keys": [
                 "ec2:Region"
             ],
             "description": "Grants permission to submit feedback about the status of an instance",
@@ -102043,20 +102107,22 @@
             "resources": [
                 "Link"
             ]
         }
     },
     "omics": {
         "AbortMultipartReadSetUpload": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AbortMultipartReadSetUpload",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to abort multipart read set uploads",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sequenceStore"
+            ]
         },
         "BatchDeleteReadSet": {
             "access_level": "Write",
             "action": "BatchDeleteReadSet",
             "condition_keys": [],
             "description": "Grants permission to batch delete Read Sets in the given Sequence Store",
             "orphan": false,
@@ -102091,36 +102157,40 @@
             "description": "Grants permission to cancel a Variant Import Job",
             "orphan": false,
             "resources": [
                 "VariantImportJob"
             ]
         },
         "CompleteMultipartReadSetUpload": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CompleteMultipartReadSetUpload",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to complete a multipart read set upload",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sequenceStore"
+            ]
         },
         "CreateAnnotationStore": {
             "access_level": "Write",
             "action": "CreateAnnotationStore",
             "condition_keys": [],
             "description": "Grants permission to create an Annotation Store",
             "orphan": false,
             "resources": []
         },
         "CreateMultipartReadSetUpload": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateMultipartReadSetUpload",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a multipart read set upload",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sequenceStore"
+            ]
         },
         "CreateReferenceStore": {
             "access_level": "Write",
             "action": "CreateReferenceStore",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -102449,20 +102519,22 @@
             "action": "ListAnnotationStores",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of information about Annotation Stores",
             "orphan": false,
             "resources": []
         },
         "ListMultipartReadSetUploads": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListMultipartReadSetUploads",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list multipart read set uploads",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sequenceStore"
+            ]
         },
         "ListReadSetActivationJobs": {
             "access_level": "List",
             "action": "ListReadSetActivationJobs",
             "condition_keys": [],
             "description": "Grants permission to list Read Set activation jobs for the given Sequence Store",
             "orphan": false,
@@ -102487,20 +102559,22 @@
             "description": "Grants permission to list Read Set import jobs for the given Sequence Store",
             "orphan": false,
             "resources": [
                 "sequenceStore"
             ]
         },
         "ListReadSetUploadParts": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListReadSetUploadParts",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list read set upload parts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sequenceStore"
+            ]
         },
         "ListReadSets": {
             "access_level": "List",
             "action": "ListReadSets",
             "condition_keys": [],
             "description": "Grants permission to list Read Sets in the given Sequence Store",
             "orphan": false,
@@ -102743,20 +102817,22 @@
             "description": "Grants permission to update workflow details",
             "orphan": false,
             "resources": [
                 "workflow"
             ]
         },
         "UploadReadSetPart": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UploadReadSetPart",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to upload read set parts",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sequenceStore"
+            ]
         }
     },
     "opsworks": {
         "AssignInstance": {
             "access_level": "Write",
             "action": "AssignInstance",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230516/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230517/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230517/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/iam_actions/generate/generate.py` & `iam_actions-1.2.20230517/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230517/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230517/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/iam_actions/generate/services.py` & `iam_actions-1.2.20230517/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/iam_actions/policies.json` & `iam_actions-1.2.20230517/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993029420825%*

 * *Differences: {"'serviceMap'": "{'Amazon EC2': {'Actions': {insert: [(29, "*

 * *                 "'AssociateVerifiedAccessInstanceWebAcl'), (347, "*

 * *                 "'DescribeVerifiedAccessInstanceWebAclAssociations'), (398, "*

 * *                 "'DisassociateVerifiedAccessInstanceWebAcl'), (459, "*

 * *                 "'GetVerifiedAccessInstanceWebAcl'), (462, 'GetVpnTunnelReplacementStatus'), "*

 * *                 "(463, 'ImportByoipCidrToIpam'), (566, 'ReplaceVpnTunnel')]}, 'conditionKeys': "*

 * *                 "{delete: [49, 24]}}, […]*

```diff
@@ -1410,14 +1410,15 @@
                 "DescribeEnvironmentMemberships",
                 "DescribeEnvironmentStatus",
                 "DescribeEnvironments",
                 "DescribeSSHRemote",
                 "GetEnvironmentConfig",
                 "GetEnvironmentSettings",
                 "GetMembershipSettings",
+                "GetMigrationExperiences",
                 "GetUserPublicKey",
                 "GetUserSettings",
                 "ListEnvironments",
                 "ListTagsForResource",
                 "ModifyTemporaryCredentialsOnEnvironmentEC2",
                 "TagResource",
                 "UntagResource",
@@ -11964,14 +11965,15 @@
                 "AssociateNatGatewayAddress",
                 "AssociateRouteTable",
                 "AssociateSubnetCidrBlock",
                 "AssociateTransitGatewayMulticastDomain",
                 "AssociateTransitGatewayPolicyTable",
                 "AssociateTransitGatewayRouteTable",
                 "AssociateTrunkInterface",
+                "AssociateVerifiedAccessInstanceWebAcl",
                 "AssociateVpcCidrBlock",
                 "AttachClassicLinkVpc",
                 "AttachInternetGateway",
                 "AttachNetworkInterface",
                 "AttachVerifiedAccessTrustProvider",
                 "AttachVolume",
                 "AttachVpnGateway",
@@ -12281,14 +12283,15 @@
                 "DescribeTransitGatewayRouteTables",
                 "DescribeTransitGatewayVpcAttachments",
                 "DescribeTransitGateways",
                 "DescribeTrunkInterfaceAssociations",
                 "DescribeVerifiedAccessEndpoints",
                 "DescribeVerifiedAccessGroups",
                 "DescribeVerifiedAccessInstanceLoggingConfigurations",
+                "DescribeVerifiedAccessInstanceWebAclAssociations",
                 "DescribeVerifiedAccessInstances",
                 "DescribeVerifiedAccessTrustProviders",
                 "DescribeVolumeAttribute",
                 "DescribeVolumeStatus",
                 "DescribeVolumes",
                 "DescribeVolumesModifications",
                 "DescribeVpcAttribute",
@@ -12331,14 +12334,15 @@
                 "DisassociateNatGatewayAddress",
                 "DisassociateRouteTable",
                 "DisassociateSubnetCidrBlock",
                 "DisassociateTransitGatewayMulticastDomain",
                 "DisassociateTransitGatewayPolicyTable",
                 "DisassociateTransitGatewayRouteTable",
                 "DisassociateTrunkInterface",
+                "DisassociateVerifiedAccessInstanceWebAcl",
                 "DisassociateVpcCidrBlock",
                 "EnableAddressTransfer",
                 "EnableAwsNetworkPerformanceMetricSubscription",
                 "EnableEbsEncryptionByDefault",
                 "EnableFastLaunch",
                 "EnableFastSnapshotRestores",
                 "EnableImageDeprecation",
@@ -12391,16 +12395,19 @@
                 "GetTransitGatewayPolicyTableAssociations",
                 "GetTransitGatewayPolicyTableEntries",
                 "GetTransitGatewayPrefixListReferences",
                 "GetTransitGatewayRouteTableAssociations",
                 "GetTransitGatewayRouteTablePropagations",
                 "GetVerifiedAccessEndpointPolicy",
                 "GetVerifiedAccessGroupPolicy",
+                "GetVerifiedAccessInstanceWebAcl",
                 "GetVpnConnectionDeviceSampleConfiguration",
                 "GetVpnConnectionDeviceTypes",
+                "GetVpnTunnelReplacementStatus",
+                "ImportByoipCidrToIpam",
                 "ImportClientVpnClientCertificateRevocationList",
                 "ImportImage",
                 "ImportInstance",
                 "ImportKeyPair",
                 "ImportSnapshot",
                 "ImportVolume",
                 "ListImagesInRecycleBin",
@@ -12495,14 +12502,15 @@
                 "ReleaseIpamPoolAllocation",
                 "ReplaceIamInstanceProfileAssociation",
                 "ReplaceNetworkAclAssociation",
                 "ReplaceNetworkAclEntry",
                 "ReplaceRoute",
                 "ReplaceRouteTableAssociation",
                 "ReplaceTransitGatewayRoute",
+                "ReplaceVpnTunnel",
                 "ReportInstanceStatus",
                 "RequestSpotFleet",
                 "RequestSpotInstances",
                 "ResetAddressAttribute",
                 "ResetEbsDefaultKmsKeyId",
                 "ResetFpgaImageAttribute",
                 "ResetImageAttribute",
@@ -12562,15 +12570,14 @@
                 "ec2:CloudwatchLogGroupArn",
                 "ec2:CloudwatchLogStreamArn",
                 "ec2:CreateAction",
                 "ec2:DPDTimeoutSeconds",
                 "ec2:DhcpOptionsID",
                 "ec2:DirectoryArn",
                 "ec2:Domain",
-                "ec2:DomainCertificateArn",
                 "ec2:EbsOptimized",
                 "ec2:ElasticGpuType",
                 "ec2:Encrypted",
                 "ec2:GatewayType",
                 "ec2:HostRecovery",
                 "ec2:IKEVersions",
                 "ec2:ImageID",
@@ -12587,15 +12594,14 @@
                 "ec2:Ipv4IpamPoolId",
                 "ec2:Ipv6IpamPoolId",
                 "ec2:IsLaunchTemplateResource",
                 "ec2:KeyPairName",
                 "ec2:KeyPairType",
                 "ec2:KmsKeyId",
                 "ec2:LaunchTemplate",
-                "ec2:LoadBalancerArn",
                 "ec2:MetadataHttpEndpoint",
                 "ec2:MetadataHttpPutResponseHopLimit",
                 "ec2:MetadataHttpTokens",
                 "ec2:NetworkAclID",
                 "ec2:NetworkInterfaceID",
                 "ec2:NewInstanceProfile",
                 "ec2:OutpostArn",
```

### Comparing `iam_actions-1.2.20230516/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230517/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230516/iam_actions/services.json` & `iam_actions-1.2.20230517/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999926993376897%*

 * *Differences: {"'cloud9'": "{'Actions': {insert: [(15, 'GetMigrationExperiences')]}}",*

 * * "'ec2'": "{'Actions': {insert: [(29, 'AssociateVerifiedAccessInstanceWebAcl'), (347, "*

 * *          "'DescribeVerifiedAccessInstanceWebAclAssociations'), (398, "*

 * *          "'DisassociateVerifiedAccessInstanceWebAcl'), (459, 'GetVerifiedAccessInstanceWebAcl'), "*

 * *          "(462, 'GetVpnTunnelReplacementStatus'), (463, 'ImportByoipCidrToIpam'), (566, "*

 * *          "'ReplaceVpnTunnel')]}, 'ConditionKeys': {delete: [49, 24]}}"}*

```diff
@@ -2705,14 +2705,15 @@
             "DescribeEnvironmentMemberships",
             "DescribeEnvironmentStatus",
             "DescribeEnvironments",
             "DescribeSSHRemote",
             "GetEnvironmentConfig",
             "GetEnvironmentSettings",
             "GetMembershipSettings",
+            "GetMigrationExperiences",
             "GetUserPublicKey",
             "GetUserSettings",
             "ListEnvironments",
             "ListTagsForResource",
             "ModifyTemporaryCredentialsOnEnvironmentEC2",
             "TagResource",
             "UntagResource",
@@ -6257,14 +6258,15 @@
             "AssociateNatGatewayAddress",
             "AssociateRouteTable",
             "AssociateSubnetCidrBlock",
             "AssociateTransitGatewayMulticastDomain",
             "AssociateTransitGatewayPolicyTable",
             "AssociateTransitGatewayRouteTable",
             "AssociateTrunkInterface",
+            "AssociateVerifiedAccessInstanceWebAcl",
             "AssociateVpcCidrBlock",
             "AttachClassicLinkVpc",
             "AttachInternetGateway",
             "AttachNetworkInterface",
             "AttachVerifiedAccessTrustProvider",
             "AttachVolume",
             "AttachVpnGateway",
@@ -6574,14 +6576,15 @@
             "DescribeTransitGatewayRouteTables",
             "DescribeTransitGatewayVpcAttachments",
             "DescribeTransitGateways",
             "DescribeTrunkInterfaceAssociations",
             "DescribeVerifiedAccessEndpoints",
             "DescribeVerifiedAccessGroups",
             "DescribeVerifiedAccessInstanceLoggingConfigurations",
+            "DescribeVerifiedAccessInstanceWebAclAssociations",
             "DescribeVerifiedAccessInstances",
             "DescribeVerifiedAccessTrustProviders",
             "DescribeVolumeAttribute",
             "DescribeVolumeStatus",
             "DescribeVolumes",
             "DescribeVolumesModifications",
             "DescribeVpcAttribute",
@@ -6624,14 +6627,15 @@
             "DisassociateNatGatewayAddress",
             "DisassociateRouteTable",
             "DisassociateSubnetCidrBlock",
             "DisassociateTransitGatewayMulticastDomain",
             "DisassociateTransitGatewayPolicyTable",
             "DisassociateTransitGatewayRouteTable",
             "DisassociateTrunkInterface",
+            "DisassociateVerifiedAccessInstanceWebAcl",
             "DisassociateVpcCidrBlock",
             "EnableAddressTransfer",
             "EnableAwsNetworkPerformanceMetricSubscription",
             "EnableEbsEncryptionByDefault",
             "EnableFastLaunch",
             "EnableFastSnapshotRestores",
             "EnableImageDeprecation",
@@ -6684,16 +6688,19 @@
             "GetTransitGatewayPolicyTableAssociations",
             "GetTransitGatewayPolicyTableEntries",
             "GetTransitGatewayPrefixListReferences",
             "GetTransitGatewayRouteTableAssociations",
             "GetTransitGatewayRouteTablePropagations",
             "GetVerifiedAccessEndpointPolicy",
             "GetVerifiedAccessGroupPolicy",
+            "GetVerifiedAccessInstanceWebAcl",
             "GetVpnConnectionDeviceSampleConfiguration",
             "GetVpnConnectionDeviceTypes",
+            "GetVpnTunnelReplacementStatus",
+            "ImportByoipCidrToIpam",
             "ImportClientVpnClientCertificateRevocationList",
             "ImportImage",
             "ImportInstance",
             "ImportKeyPair",
             "ImportSnapshot",
             "ImportVolume",
             "ListImagesInRecycleBin",
@@ -6788,14 +6795,15 @@
             "ReleaseIpamPoolAllocation",
             "ReplaceIamInstanceProfileAssociation",
             "ReplaceNetworkAclAssociation",
             "ReplaceNetworkAclEntry",
             "ReplaceRoute",
             "ReplaceRouteTableAssociation",
             "ReplaceTransitGatewayRoute",
+            "ReplaceVpnTunnel",
             "ReportInstanceStatus",
             "RequestSpotFleet",
             "RequestSpotInstances",
             "ResetAddressAttribute",
             "ResetEbsDefaultKmsKeyId",
             "ResetFpgaImageAttribute",
             "ResetImageAttribute",
@@ -6853,15 +6861,14 @@
             "ec2:CloudwatchLogGroupArn",
             "ec2:CloudwatchLogStreamArn",
             "ec2:CreateAction",
             "ec2:DPDTimeoutSeconds",
             "ec2:DhcpOptionsID",
             "ec2:DirectoryArn",
             "ec2:Domain",
-            "ec2:DomainCertificateArn",
             "ec2:EbsOptimized",
             "ec2:ElasticGpuType",
             "ec2:Encrypted",
             "ec2:GatewayType",
             "ec2:HostRecovery",
             "ec2:IKEVersions",
             "ec2:ImageID",
@@ -6878,15 +6885,14 @@
             "ec2:Ipv4IpamPoolId",
             "ec2:Ipv6IpamPoolId",
             "ec2:IsLaunchTemplateResource",
             "ec2:KeyPairName",
             "ec2:KeyPairType",
             "ec2:KmsKeyId",
             "ec2:LaunchTemplate",
-            "ec2:LoadBalancerArn",
             "ec2:MetadataHttpEndpoint",
             "ec2:MetadataHttpPutResponseHopLimit",
             "ec2:MetadataHttpTokens",
             "ec2:NetworkAclID",
             "ec2:NetworkInterfaceID",
             "ec2:NewInstanceProfile",
             "ec2:OutpostArn",
```

### Comparing `iam_actions-1.2.20230516/pyproject.toml` & `iam_actions-1.2.20230517/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230516"
+version = "1.2.20230517"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230516/setup.py` & `iam_actions-1.2.20230517/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230516',
+    'version': '1.2.20230517',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230516/PKG-INFO` & `iam_actions-1.2.20230517/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230516
+Version: 1.2.20230517
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

