# Comparing `tmp/robothub_oak-1.1.2.tar.gz` & `tmp/robothub_oak-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub_oak-1.1.2.tar", last modified: Thu May 11 21:58:52 2023, max compression
+gzip compressed data, was "robothub_oak-1.2.0.tar", last modified: Wed May 17 17:54:08 2023, max compression
```

## Comparing `robothub_oak-1.1.2.tar` & `robothub_oak-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.798801 robothub_oak-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 21:58:52.798801 robothub_oak-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 21:58:52.798801 robothub_oak-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.786801 robothub_oak-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.790801 robothub_oak-1.1.2/src/robothub_oak/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.794801 robothub_oak-1.1.2/src/robothub_oak/components/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/imu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/components/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/device.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13350 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8584 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/src/robothub_oak/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.794801 robothub_oak-1.1.2/src/robothub_oak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 21:58:52.000000 robothub_oak-1.1.2/src/robothub_oak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-11 21:58:52.000000 robothub_oak-1.1.2/src/robothub_oak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:58:52.000000 robothub_oak-1.1.2/src/robothub_oak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 21:58:52.000000 robothub_oak-1.1.2/src/robothub_oak.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:52.794801 robothub_oak-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/tests/test_hub_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:58:23.000000 robothub_oak-1.1.2/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.436290 robothub_oak-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.436290 robothub_oak-1.2.0/src/robothub_oak/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/src/robothub_oak/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/imu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/stereo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/components/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/device.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13297 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8584 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/src/robothub_oak/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/src/robothub_oak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-17 17:54:08.000000 robothub_oak-1.2.0/src/robothub_oak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-17 17:54:08.000000 robothub_oak-1.2.0/src/robothub_oak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:54:08.000000 robothub_oak-1.2.0/src/robothub_oak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 17:54:08.000000 robothub_oak-1.2.0/src/robothub_oak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:54:08.440291 robothub_oak-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/tests/test_hub_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:53:39.000000 robothub_oak-1.2.0/tests/test_manager.py
```

### Comparing `robothub_oak-1.1.2/LICENSE` & `robothub_oak-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.2/PKG-INFO` & `robothub_oak-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub_oak
-Version: 1.1.2
+Version: 1.2.0
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.1.2/README.md` & `robothub_oak-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.2/setup.py` & `robothub_oak-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub_oak',
-    version='1.1.2',
+    version='1.2.0',
     description='RobotHub-OAK integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub robot hub connect agent depthai oak sdk',
     author='Luxonis',
```

### Comparing `robothub_oak-1.1.2/src/robothub_oak/callbacks.py` & `robothub_oak-1.2.0/src/robothub_oak/callbacks.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.2/src/robothub_oak/components/camera.py` & `robothub_oak-1.2.0/src/robothub_oak/components/camera.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from dataclasses import dataclass, replace
-from typing import Optional, Tuple, Union, Any, Dict
+from typing import Optional, Tuple, Union
 
 import depthai as dai
 
 from robothub_oak.components.streamable import Streamable
 
 __all__ = ['Camera']
 
+from robothub_oak.utils import _process_kwargs
+
 
 @dataclass
 class CameraConfig:
     """
     Dataclass representing the configuration of the camera.
     """
     interleaved: Optional[bool] = None
@@ -28,14 +30,15 @@
 
 
 class Camera(Streamable):
     """
     This component represents a single camera on the OAK, either color or mono one.
     The API provides a way to configure the camera, but it is not required to do so.
     """
+
     def __init__(self, name: str, resolution: Optional[str], fps: Optional[int]) -> None:
         super().__init__()
         self.name = name
         self.resolution = resolution
         self.fps = fps
 
         self.camera_component = None  # type: depthai_sdk.components.CameraComponent
@@ -56,15 +59,15 @@
                   sharpness: Optional[int] = None,
                   luma_denoise: Optional[int] = None,
                   chroma_denoise: Optional[int] = None,
                   ) -> None:
         """
         Configures the camera component.
         """
-        kwargs = self._process_kwargs(locals())
+        kwargs = _process_kwargs(locals())
 
         if len(kwargs) > 0:
             self.camera_config = replace(self.camera_config, **kwargs)
 
     def set_resolution(self, resolution: str) -> None:
         """
         Sets the resolution of the camera.
@@ -76,14 +79,7 @@
     def set_fps(self, fps: int) -> None:
         """
         Sets the FPS of the camera.
 
         :param fps: FPS to set as an integer.
         """
         self.fps = fps
-
-    @staticmethod
-    def _process_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
-        """Process the kwargs and remove all None values."""
-        kwargs.pop('self')
-        kwargs = {k: v for k, v in kwargs.items() if v is not None}
-        return kwargs
```

### Comparing `robothub_oak-1.1.2/src/robothub_oak/components/neural_network.py` & `robothub_oak-1.2.0/src/robothub_oak/components/neural_network.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.2/src/robothub_oak/components/stereo.py` & `robothub_oak-1.2.0/src/robothub_oak/components/stereo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,49 @@
+from dataclasses import dataclass, replace
 from enum import IntEnum
 from typing import Union, Optional
 
+import depthai as dai
+
 from robothub_oak.components.streamable import Streamable
 
 __all__ = ['Stereo', 'DepthQuality', 'DepthRange']
 
+from robothub_oak.utils import _process_kwargs
+
 
 class DepthQuality(IntEnum):
     FAST = 1  # nothing turned on
     DEFAULT = 2  # lr check, median filter
     QUALITY = 3  # lr check, subpixel
 
 
 class DepthRange(IntEnum):
     SHORT = 1  # extended disparity
     DEFAULT = 2  # no effect
     LONG = 3  # subpixel
 
 
+@dataclass
+class StereoConfig:
+    """
+    Dataclass representing the configuration of the stereo component.
+    """
+    depth_quality: Union[str, DepthQuality] = None
+    depth_range: Union[str, DepthRange] = None
+    align: Optional['Camera'] = None
+    confidence: Optional[int] = None
+    median: Union[None, int, dai.MedianFilter] = None
+    extended: Optional[bool] = None
+    subpixel: Optional[bool] = None
+    lr_check: Optional[bool] = None
+    sigma: Optional[int] = None
+    lr_check_threshold: Optional[int] = None
+
+
 class Stereo(Streamable):
     def __init__(self,
                  resolution: Optional[str],
                  fps: Optional[int],
                  left_camera: Optional['Camera'] = None,
                  right_camera: Optional['Camera'] = None):
         """
@@ -35,37 +57,52 @@
         super().__init__()
         self.resolution = resolution
         self.fps = fps
 
         self.left_camera = left_camera
         self.right_camera = right_camera
 
-        self.quality = DepthQuality.DEFAULT
-        self.range = DepthRange.DEFAULT
-
-        self.align = 'color'
+        self.stereo_config = StereoConfig()
         self.stereo_component = None  # type: depthai_sdk.components.StereoComponent
 
     def configure(self,
                   depth_quality: Union[str, DepthQuality] = None,
                   depth_range: Union[str, DepthRange] = None,
-                  align: str = None) -> None:
+                  align: 'Camera' = None,
+                  confidence: Optional[int] = None,
+                  median: Union[None, int, dai.MedianFilter] = None,
+                  extended: Optional[bool] = None,
+                  subpixel: Optional[bool] = None,
+                  lr_check: Optional[bool] = None,
+                  sigma: Optional[int] = None,
+                  lr_check_threshold: Optional[int] = None,
+                  ) -> None:
         """
         Configures the stereo component.
 
         :param depth_quality: Quality of the depth map. Can be one of 'fast', 'default' or 'quality'.
         :param depth_range: Working range of the stereo module. Can be one of 'short', 'default' or 'long'.
-        :param align: Alignment of the depth map. Can be one of 'color', 'left', 'right' or 'cama,c' (or similar). Defaults to 'color'.
+        :param align: Alignment of the depth map. Can be a camera component.
+        :param confidence: Confidence threshold for the depth map.
+        :param median: Median filter size. Can be one of 3, 5, 7, or None.
+        :param extended: Whether to use extended disparity.
+        :param subpixel: Whether to use subpixel disparity.
+        :param lr_check: Whether to use left-right check.
+        :param sigma: Sigma value for the median filter.
+        :param lr_check_threshold: Threshold for the left-right check.
         """
         if depth_quality:
-            self.quality = self._set_enum_value(DepthQuality, depth_quality)
+            depth_quality = self._set_enum_value(DepthQuality, depth_quality)
         if depth_range:
-            self.range = self._set_enum_value(DepthRange, depth_range)
-        if align:
-            self.align = align
+            depth_range = self._set_enum_value(DepthRange, depth_range)
+
+        kwargs = _process_kwargs(locals())
+
+        if len(kwargs) > 0:
+            self.stereo_config = replace(self.stereo_config, **kwargs)
 
     @staticmethod
     def _set_enum_value(enum, value):
         if isinstance(value, str):
             return enum[value.upper()]
         elif isinstance(value, enum):
             return value
```

### Comparing `robothub_oak-1.1.2/src/robothub_oak/device.py` & `robothub_oak-1.2.0/src/robothub_oak/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 import warnings
 from typing import Callable, Any, Optional, Dict
 
 from depthai import NNData
 
 from robothub_oak.commands import (
     CreateStereoCommand, CreateCameraCommand, CreateNeuralNetworkCommand,
@@ -45,15 +46,18 @@
         self.disconnect_callback: Callable[[Any], None] = lambda x: None
         self.connect_callback: Callable[[Any], None] = lambda x: None
 
         self._command_history = CommandHistory()
 
     def __eq__(self, other):
         if isinstance(other, Device):
-            return self.id == other.id or self.name == other.name or self.mxid == other.mxid or self.ip_address == other.ip_address
+            return (self.id and self.id == other.id) \
+                or (self.name and self.name == other.name) \
+                or (self.mxid and self.mxid == other.mxid) \
+                or (self.ip_address and self.ip_address == other.ip_address)
         elif isinstance(other, str):
             return self.id == other or self.name == other or self.mxid == other or self.ip_address == other
         else:
             return False
 
     def _start(self, hub_camera: HubCamera) -> bool:
         """
@@ -73,14 +77,15 @@
                     warnings.warn(f'Device {self.get_device_name()} does not support stereo, skipping stereo creation.')
                     continue
 
                 command.set_camera(hub_camera)
                 command.execute()
         except Exception as e:
             warnings.warn(f'Failed to start device {self.get_device_name()} with error: {e}')
+            traceback.print_exc()
             return False
 
         # Create streams
         for command in self._command_history:
             # Check if stream is enabled, if so, create a stream command and execute it
             component = command.get_component()
 
@@ -104,14 +109,15 @@
         try:
             if self.hub_camera:
                 self.hub_camera.stop()
                 self.hub_camera.oak_camera = self.hub_camera.init_oak_camera()
                 self._start(hub_camera=self.hub_camera)
         except Exception as e:
             warnings.warn(f'Failed to restart device {self.get_device_name()} with error: {e}')
+            traceback.print_exc()
             return False
 
         return True
 
     def get_camera(self, name: str, resolution: str = None, fps: int = None) -> Camera:
         """
         Creates a camera component.
@@ -152,17 +158,14 @@
         :return: The neural network.
         """
         if name in self.neural_networks:
             return self.neural_networks[name]
         elif not input:
             raise ValueError('Neural network must have an input')
 
-        if isinstance(input, NeuralNetwork):
-            raise NotImplementedError('Neural networks cannot be used as input for other neural networks yet')
-
         neural_network = NeuralNetwork(name=name,
                                        input=input,
                                        nn_type=nn_type,
                                        decode_fn=decode_fn,
                                        tracker=tracker,
                                        spatial=spatial)
         command = CreateNeuralNetworkCommand(self, neural_network)
```

### Comparing `robothub_oak-1.1.2/src/robothub_oak/hub_camera.py` & `robothub_oak-1.2.0/src/robothub_oak/hub_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
         :param right: Right camera component, optional.
         :return: Stereo component.
         """
         if not self.has_stereo:
             raise RuntimeError('Device does not have stereo cameras.')
 
         comp = self.oak_camera.create_stereo(resolution=resolution, fps=fps, left=left, right=right, encode='h264')
-        comp.set_colormap(dai.Colormap.STEREO_TURBO)
         return comp
 
     def create_stream(self,
                       component: Union[CameraComponent, NNComponent, StereoComponent],
                       unique_key: str,
                       name: str,
                       callback: Callable = None
```

### Comparing `robothub_oak-1.1.2/src/robothub_oak/manager.py` & `robothub_oak-1.2.0/src/robothub_oak/manager.py`

 * *Files identical despite different names*

### Comparing `robothub_oak-1.1.2/src/robothub_oak/packets.py` & `robothub_oak-1.2.0/src/robothub_oak/packets.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,18 @@
         raise NotImplementedError('Not implemented yet')
 
 
 class DetectionPacket(HubPacket):
     def __init__(self, device: 'Device', packet):
         super().__init__(device, packet)
         self.detections = packet.detections
+        try:
+            self.nn_data = packet.nnData
+        except AttributeError:
+            self.nn_data = None
 
     def upload_as_detection(self, title: str):
         try:
             # convert numpy array to jpg
             frame_bytes = cv2.imencode('.jpg', self._packet.frame)[1].tobytes()
 
             # TODO add metadata
```

### Comparing `robothub_oak-1.1.2/src/robothub_oak.egg-info/PKG-INFO` & `robothub_oak-1.2.0/src/robothub_oak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub-oak
-Version: 1.1.2
+Version: 1.2.0
 Summary: RobotHub-OAK integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub-oak/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub_oak-1.1.2/src/robothub_oak.egg-info/SOURCES.txt` & `robothub_oak-1.2.0/src/robothub_oak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

