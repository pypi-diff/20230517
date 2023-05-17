# Comparing `tmp/pulumi_containerregistry-0.0.3.tar.gz` & `tmp/pulumi_containerregistry-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_containerregistry-0.0.3.tar", last modified: Wed May 17 12:57:33 2023, max compression
+gzip compressed data, was "pulumi_containerregistry-0.0.4.tar", last modified: Wed May 17 13:16:05 2023, max compression
```

## Comparing `pulumi_containerregistry-0.0.3.tar` & `pulumi_containerregistry-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:33.612567 pulumi_containerregistry-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 12:57:33.612567 pulumi_containerregistry-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:33.608567 pulumi_containerregistry-0.0.3/pulumi_containerregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:33.612567 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:57:33.612567 pulumi_containerregistry-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-17 12:57:33.000000 pulumi_containerregistry-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:16:05.206116 pulumi_containerregistry-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 13:16:05.206116 pulumi_containerregistry-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:16:05.202115 pulumi_containerregistry-0.0.4/pulumi_containerregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:16:05.206116 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:16:05.206116 pulumi_containerregistry-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/setup.py
```

### Comparing `pulumi_containerregistry-0.0.3/PKG-INFO` & `pulumi_containerregistry-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_containerregistry
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Pulumi package for creating and managing containerregistry cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/rhysmdnz/pulumi-containerregistry
 Keywords: pulumi containerregistry category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_containerregistry-0.0.3/README.md` & `pulumi_containerregistry-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.3/pulumi_containerregistry/__init__.py` & `pulumi_containerregistry-0.0.4/pulumi_containerregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.3/pulumi_containerregistry/_utilities.py` & `pulumi_containerregistry-0.0.4/pulumi_containerregistry/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return None
+	return "https://github.com/rhysmdnz/pulumi-containerregistry/releases/"
```

### Comparing `pulumi_containerregistry-0.0.3/pulumi_containerregistry/provider.py` & `pulumi_containerregistry-0.0.4/pulumi_containerregistry/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.3/pulumi_containerregistry/resource.py` & `pulumi_containerregistry-0.0.4/pulumi_containerregistry/resource.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,52 +10,52 @@
 from . import _utilities
 
 __all__ = ['ResourceArgs', 'Resource']
 
 @pulumi.input_type
 class ResourceArgs:
     def __init__(__self__, *,
-                 image_tarball: pulumi.Input[str],
                  image_tarball_hash: pulumi.Input[str],
+                 image_tarball: pulumi.Input[Union[pulumi.Asset, pulumi.Archive]],
                  remote_tag: pulumi.Input[str]):
         """
         The set of arguments for constructing a Resource resource.
-        :param pulumi.Input[str] image_tarball: Image tarball thing.
         :param pulumi.Input[str] image_tarball_hash: Hash of the image tarball.
+        :param pulumi.Input[Union[pulumi.Asset, pulumi.Archive]] image_tarball: Image tarball thing.
         :param pulumi.Input[str] remote_tag: The tag to save the image to.
         """
-        pulumi.set(__self__, "image_tarball", image_tarball)
         pulumi.set(__self__, "image_tarball_hash", image_tarball_hash)
+        pulumi.set(__self__, "image_tarball", image_tarball)
         pulumi.set(__self__, "remote_tag", remote_tag)
 
     @property
-    @pulumi.getter(name="imageTarball")
-    def image_tarball(self) -> pulumi.Input[str]:
-        """
-        Image tarball thing.
-        """
-        return pulumi.get(self, "image_tarball")
-
-    @image_tarball.setter
-    def image_tarball(self, value: pulumi.Input[str]):
-        pulumi.set(self, "image_tarball", value)
-
-    @property
     @pulumi.getter(name="imageTarballHash")
     def image_tarball_hash(self) -> pulumi.Input[str]:
         """
         Hash of the image tarball.
         """
         return pulumi.get(self, "image_tarball_hash")
 
     @image_tarball_hash.setter
     def image_tarball_hash(self, value: pulumi.Input[str]):
         pulumi.set(self, "image_tarball_hash", value)
 
     @property
+    @pulumi.getter
+    def image_tarball(self) -> pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]:
+        """
+        Image tarball thing.
+        """
+        return pulumi.get(self, "image_tarball")
+
+    @image_tarball.setter
+    def image_tarball(self, value: pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]):
+        pulumi.set(self, "image_tarball", value)
+
+    @property
     @pulumi.getter(name="remoteTag")
     def remote_tag(self) -> pulumi.Input[str]:
         """
         The tag to save the image to.
         """
         return pulumi.get(self, "remote_tag")
 
@@ -63,55 +63,55 @@
     def remote_tag(self, value: pulumi.Input[str]):
         pulumi.set(self, "remote_tag", value)
 
 
 @pulumi.input_type
 class _ResourceState:
     def __init__(__self__, *,
-                 image_tarball: Optional[pulumi.Input[str]] = None,
                  image_tarball_hash: Optional[pulumi.Input[str]] = None,
+                 image_tarball: Optional[pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]] = None,
                  remote_tag: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Resource resources.
-        :param pulumi.Input[str] image_tarball: Image tarball thing.
         :param pulumi.Input[str] image_tarball_hash: Hash of the image tarball.
+        :param pulumi.Input[Union[pulumi.Asset, pulumi.Archive]] image_tarball: Image tarball thing.
         :param pulumi.Input[str] remote_tag: The tag to save the image to.
         """
-        if image_tarball is not None:
-            pulumi.set(__self__, "image_tarball", image_tarball)
         if image_tarball_hash is not None:
             pulumi.set(__self__, "image_tarball_hash", image_tarball_hash)
+        if image_tarball is not None:
+            pulumi.set(__self__, "image_tarball", image_tarball)
         if remote_tag is not None:
             pulumi.set(__self__, "remote_tag", remote_tag)
 
     @property
-    @pulumi.getter(name="imageTarball")
-    def image_tarball(self) -> Optional[pulumi.Input[str]]:
-        """
-        Image tarball thing.
-        """
-        return pulumi.get(self, "image_tarball")
-
-    @image_tarball.setter
-    def image_tarball(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "image_tarball", value)
-
-    @property
     @pulumi.getter(name="imageTarballHash")
     def image_tarball_hash(self) -> Optional[pulumi.Input[str]]:
         """
         Hash of the image tarball.
         """
         return pulumi.get(self, "image_tarball_hash")
 
     @image_tarball_hash.setter
     def image_tarball_hash(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image_tarball_hash", value)
 
     @property
+    @pulumi.getter
+    def image_tarball(self) -> Optional[pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]]:
+        """
+        Image tarball thing.
+        """
+        return pulumi.get(self, "image_tarball")
+
+    @image_tarball.setter
+    def image_tarball(self, value: Optional[pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]]):
+        pulumi.set(self, "image_tarball", value)
+
+    @property
     @pulumi.getter(name="remoteTag")
     def remote_tag(self) -> Optional[pulumi.Input[str]]:
         """
         The tag to save the image to.
         """
         return pulumi.get(self, "remote_tag")
 
@@ -121,24 +121,24 @@
 
 
 class Resource(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 image_tarball: Optional[pulumi.Input[str]] = None,
                  image_tarball_hash: Optional[pulumi.Input[str]] = None,
+                 image_tarball: Optional[pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]] = None,
                  remote_tag: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Resource resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] image_tarball: Image tarball thing.
         :param pulumi.Input[str] image_tarball_hash: Hash of the image tarball.
+        :param pulumi.Input[Union[pulumi.Asset, pulumi.Archive]] image_tarball: Image tarball thing.
         :param pulumi.Input[str] remote_tag: The tag to save the image to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ResourceArgs,
@@ -156,85 +156,85 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 image_tarball: Optional[pulumi.Input[str]] = None,
                  image_tarball_hash: Optional[pulumi.Input[str]] = None,
+                 image_tarball: Optional[pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]] = None,
                  remote_tag: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ResourceArgs.__new__(ResourceArgs)
 
-            if image_tarball is None and not opts.urn:
-                raise TypeError("Missing required property 'image_tarball'")
-            __props__.__dict__["image_tarball"] = image_tarball
             if image_tarball_hash is None and not opts.urn:
                 raise TypeError("Missing required property 'image_tarball_hash'")
             __props__.__dict__["image_tarball_hash"] = image_tarball_hash
+            if image_tarball is None and not opts.urn:
+                raise TypeError("Missing required property 'image_tarball'")
+            __props__.__dict__["image_tarball"] = image_tarball
             if remote_tag is None and not opts.urn:
                 raise TypeError("Missing required property 'remote_tag'")
             __props__.__dict__["remote_tag"] = remote_tag
         super(Resource, __self__).__init__(
             'containerregistry:index/resource:Resource',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            image_tarball: Optional[pulumi.Input[str]] = None,
             image_tarball_hash: Optional[pulumi.Input[str]] = None,
+            image_tarball: Optional[pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]] = None,
             remote_tag: Optional[pulumi.Input[str]] = None) -> 'Resource':
         """
         Get an existing Resource resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] image_tarball: Image tarball thing.
         :param pulumi.Input[str] image_tarball_hash: Hash of the image tarball.
+        :param pulumi.Input[Union[pulumi.Asset, pulumi.Archive]] image_tarball: Image tarball thing.
         :param pulumi.Input[str] remote_tag: The tag to save the image to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ResourceState.__new__(_ResourceState)
 
-        __props__.__dict__["image_tarball"] = image_tarball
         __props__.__dict__["image_tarball_hash"] = image_tarball_hash
+        __props__.__dict__["image_tarball"] = image_tarball
         __props__.__dict__["remote_tag"] = remote_tag
         return Resource(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="imageTarball")
-    def image_tarball(self) -> pulumi.Output[str]:
-        """
-        Image tarball thing.
-        """
-        return pulumi.get(self, "image_tarball")
-
-    @property
     @pulumi.getter(name="imageTarballHash")
     def image_tarball_hash(self) -> pulumi.Output[str]:
         """
         Hash of the image tarball.
         """
         return pulumi.get(self, "image_tarball_hash")
 
     @property
+    @pulumi.getter
+    def image_tarball(self) -> pulumi.Output[Union[pulumi.Asset, pulumi.Archive]]:
+        """
+        Image tarball thing.
+        """
+        return pulumi.get(self, "image_tarball")
+
+    @property
     @pulumi.getter(name="remoteTag")
     def remote_tag(self) -> pulumi.Output[str]:
         """
         The tag to save the image to.
         """
         return pulumi.get(self, "remote_tag")
```

### Comparing `pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/PKG-INFO` & `pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-containerregistry
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Pulumi package for creating and managing containerregistry cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/rhysmdnz/pulumi-containerregistry
 Keywords: pulumi containerregistry category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_containerregistry-0.0.3/pulumi_containerregistry.egg-info/SOURCES.txt` & `pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.3/setup.py` & `pulumi_containerregistry-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.3"
-PLUGIN_VERSION = "0.0.3"
+VERSION = "0.0.4"
+PLUGIN_VERSION = "0.0.4"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'containerregistry', PLUGIN_VERSION])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'containerregistry', PLUGIN_VERSION, '--server', 'https://github.com/rhysmdnz/pulumi-containerregistry/releases/'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the containerregistry resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

