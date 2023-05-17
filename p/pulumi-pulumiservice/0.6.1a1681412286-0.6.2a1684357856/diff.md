# Comparing `tmp/pulumi_pulumiservice-0.6.1a1681412286.tar.gz` & `tmp/pulumi_pulumiservice-0.6.2a1684357856.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_pulumiservice-0.6.1a1681412286.tar", last modified: Thu Apr 13 19:01:27 2023, max compression
+gzip compressed data, was "dist/pulumi_pulumiservice-0.6.2a1684357856.tar", last modified: Wed May 17 21:14:13 2023, max compression
```

## Comparing `pulumi_pulumiservice-0.6.1a1681412286.tar` & `pulumi_pulumiservice-0.6.2a1684357856.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/config/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/deployment_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/org_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/stack_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/team_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/team_stack_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-13 19:01:27.000000 pulumi_pulumiservice-0.6.1a1681412286/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/deployment_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/org_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/stack_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/team_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/team_stack_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:14:13.000000 pulumi_pulumiservice-0.6.2a1684357856/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-17 21:14:11.000000 pulumi_pulumiservice-0.6.2a1684357856/setup.py
```

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/PKG-INFO` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_pulumiservice
-Version: 0.6.1a1681412286
+Name: pulumi-pulumiservice
+Version: 0.6.2a1684357856
 Summary: A native Pulumi package for creating and managing Pulumi Service constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
 Description: # Pulumi Service Provider
         
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
```

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/README.md` & `pulumi_pulumiservice-0.6.2a1684357856/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/__init__.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/_inputs.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/_utilities.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/access_token.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/config/vars.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/deployment_settings.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/deployment_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/org_access_token.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/org_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/provider.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/stack_tag.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/stack_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/team.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/team_access_token.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/team_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/team_stack_permission.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/team_stack_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice/webhook.py` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice/webhook.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,37 @@
 @pulumi.input_type
 class WebhookArgs:
     def __init__(__self__, *,
                  active: pulumi.Input[bool],
                  display_name: pulumi.Input[str],
                  organization_name: pulumi.Input[str],
                  payload_url: pulumi.Input[str],
-                 secret: Optional[pulumi.Input[str]] = None):
+                 project_name: Optional[pulumi.Input[str]] = None,
+                 secret: Optional[pulumi.Input[str]] = None,
+                 stack_name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Webhook resource.
         :param pulumi.Input[bool] active: Indicates whether this webhook is enabled or not.
         :param pulumi.Input[str] display_name: The friendly name displayed in the Pulumi Service.
         :param pulumi.Input[str] organization_name: Name of the organization.
         :param pulumi.Input[str] payload_url: URL to send request to.
+        :param pulumi.Input[str] project_name: Name of the project. Only needed if this is a stack webhook.
         :param pulumi.Input[str] secret: Optional. secret used as the HMAC key. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#headers) for more information.
+        :param pulumi.Input[str] stack_name: Name of the stack. Only needed if this is a stack webhook.
         """
         pulumi.set(__self__, "active", active)
         pulumi.set(__self__, "display_name", display_name)
         pulumi.set(__self__, "organization_name", organization_name)
         pulumi.set(__self__, "payload_url", payload_url)
+        if project_name is not None:
+            pulumi.set(__self__, "project_name", project_name)
         if secret is not None:
             pulumi.set(__self__, "secret", secret)
+        if stack_name is not None:
+            pulumi.set(__self__, "stack_name", stack_name)
 
     @property
     @pulumi.getter
     def active(self) -> pulumi.Input[bool]:
         """
         Indicates whether this webhook is enabled or not.
         """
@@ -79,47 +87,75 @@
         return pulumi.get(self, "payload_url")
 
     @payload_url.setter
     def payload_url(self, value: pulumi.Input[str]):
         pulumi.set(self, "payload_url", value)
 
     @property
+    @pulumi.getter(name="projectName")
+    def project_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the project. Only needed if this is a stack webhook.
+        """
+        return pulumi.get(self, "project_name")
+
+    @project_name.setter
+    def project_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_name", value)
+
+    @property
     @pulumi.getter
     def secret(self) -> Optional[pulumi.Input[str]]:
         """
         Optional. secret used as the HMAC key. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#headers) for more information.
         """
         return pulumi.get(self, "secret")
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
+    @property
+    @pulumi.getter(name="stackName")
+    def stack_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the stack. Only needed if this is a stack webhook.
+        """
+        return pulumi.get(self, "stack_name")
+
+    @stack_name.setter
+    def stack_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "stack_name", value)
+
 
 class Webhook(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  payload_url: Optional[pulumi.Input[str]] = None,
+                 project_name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
+                 stack_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Pulumi Webhooks allow you to notify external services of events happening within your Pulumi organization or stack. For example, you can trigger a notification whenever a stack is updated. Whenever an event occurs, Pulumi will send an HTTP POST request to all registered webhooks. The webhook can then be used to emit some notification, start running integration tests, or even update additional stacks.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Indicates whether this webhook is enabled or not.
         :param pulumi.Input[str] display_name: The friendly name displayed in the Pulumi Service.
         :param pulumi.Input[str] organization_name: Name of the organization.
         :param pulumi.Input[str] payload_url: URL to send request to.
+        :param pulumi.Input[str] project_name: Name of the project. Only needed if this is a stack webhook.
         :param pulumi.Input[str] secret: Optional. secret used as the HMAC key. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#headers) for more information.
+        :param pulumi.Input[str] stack_name: Name of the stack. Only needed if this is a stack webhook.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: WebhookArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -141,15 +177,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  payload_url: Optional[pulumi.Input[str]] = None,
+                 project_name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
+                 stack_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -163,15 +201,17 @@
             __props__.__dict__["display_name"] = display_name
             if organization_name is None and not opts.urn:
                 raise TypeError("Missing required property 'organization_name'")
             __props__.__dict__["organization_name"] = organization_name
             if payload_url is None and not opts.urn:
                 raise TypeError("Missing required property 'payload_url'")
             __props__.__dict__["payload_url"] = payload_url
+            __props__.__dict__["project_name"] = project_name
             __props__.__dict__["secret"] = None if secret is None else pulumi.Output.secret(secret)
+            __props__.__dict__["stack_name"] = stack_name
             __props__.__dict__["name"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["secret"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Webhook, __self__).__init__(
             'pulumiservice:index:Webhook',
             resource_name,
             __props__,
@@ -194,15 +234,17 @@
         __props__ = WebhookArgs.__new__(WebhookArgs)
 
         __props__.__dict__["active"] = None
         __props__.__dict__["display_name"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["organization_name"] = None
         __props__.__dict__["payload_url"] = None
+        __props__.__dict__["project_name"] = None
         __props__.__dict__["secret"] = None
+        __props__.__dict__["stack_name"] = None
         return Webhook(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def active(self) -> pulumi.Output[Optional[bool]]:
         """
         Indicates whether this webhook is enabled or not.
@@ -238,14 +280,30 @@
     def payload_url(self) -> pulumi.Output[Optional[str]]:
         """
         URL to send request to.
         """
         return pulumi.get(self, "payload_url")
 
     @property
+    @pulumi.getter(name="projectName")
+    def project_name(self) -> pulumi.Output[Optional[str]]:
+        """
+        Name of the project. Only specified if this is a stack webhook.
+        """
+        return pulumi.get(self, "project_name")
+
+    @property
     @pulumi.getter
     def secret(self) -> pulumi.Output[Optional[str]]:
         """
         Optional. secret used as the HMAC key. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#headers) for more information.
         """
         return pulumi.get(self, "secret")
 
+    @property
+    @pulumi.getter(name="stackName")
+    def stack_name(self) -> pulumi.Output[Optional[str]]:
+        """
+        Name of the stack. Only specified if this is a stack webhook.
+        """
+        return pulumi.get(self, "stack_name")
+
```

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/PKG-INFO` & `pulumi_pulumiservice-0.6.2a1684357856/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-pulumiservice
-Version: 0.6.1a1681412286
+Name: pulumi_pulumiservice
+Version: 0.6.2a1684357856
 Summary: A native Pulumi package for creating and managing Pulumi Service constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
 Description: # Pulumi Service Provider
         
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
```

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/pulumi_pulumiservice.egg-info/SOURCES.txt` & `pulumi_pulumiservice-0.6.2a1684357856/pulumi_pulumiservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.6.1a1681412286/setup.py` & `pulumi_pulumiservice-0.6.2a1684357856/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.6.1a1681412286"
-PLUGIN_VERSION = "0.6.1-alpha.1681412286+7a6a83ba"
+VERSION = "0.6.2a1684357856"
+PLUGIN_VERSION = "0.6.2-alpha.1684357856+cbb4ab6b"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'pulumiservice', PLUGIN_VERSION])
         except OSError as error:
```

