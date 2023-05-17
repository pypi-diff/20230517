# Comparing `tmp/drb-image-1.0.0.tar.gz` & `tmp/drb-image-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-image-1.0.0.tar", last modified: Tue Mar 14 22:46:35 2023, max compression
+gzip compressed data, was "drb-image-1.1.0.tar", last modified: Wed May 17 13:12:37 2023, max compression
```

## Comparing `drb-image-1.0.0.tar` & `drb-image-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 22:46:35.422627 drb-image-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-02-10 08:12:51.000000 drb-image-1.0.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-02-10 08:12:51.000000 drb-image-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3671 2023-03-14 22:46:35.422627 drb-image-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3259 2023-03-14 22:33:41.000000 drb-image-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 22:46:35.418627 drb-image-1.0.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 22:46:35.426627 drb-image-1.0.0/drb/image/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-02-10 08:12:51.000000 drb-image-1.0.0/drb/image/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-14 22:46:35.426627 drb-image-1.0.0/drb/image/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7306 2023-03-14 22:33:41.000000 drb-image-1.0.0/drb/image/image.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-03-09 15:59:22.000000 drb-image-1.0.0/drb/image/schema.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 22:46:35.422627 drb-image-1.0.0/drb_image.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3671 2023-03-14 22:46:35.000000 drb-image-1.0.0/drb_image.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      404 2023-03-14 22:46:35.000000 drb-image-1.0.0/drb_image.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 22:46:35.000000 drb-image-1.0.0/drb_image.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 22:46:35.000000 drb-image-1.0.0/drb_image.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       94 2023-03-14 22:46:35.000000 drb-image-1.0.0/drb_image.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-14 22:46:35.000000 drb-image-1.0.0/drb_image.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-02-10 08:12:51.000000 drb-image-1.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-02-10 08:12:51.000000 drb-image-1.0.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-03-14 22:46:35.426627 drb-image-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-02-10 08:12:51.000000 drb-image-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 22:46:35.422627 drb-image-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-03-14 22:33:41.000000 drb-image-1.0.0/tests/test_image_addon.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-02-10 08:12:51.000000 drb-image-1.0.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:12:37.535067 drb-image-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-03-31 08:56:49.000000 drb-image-1.1.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-03-31 08:56:49.000000 drb-image-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-05-17 13:12:37.535067 drb-image-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-03-31 12:35:30.000000 drb-image-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:12:37.519067 drb-image-1.1.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:12:37.535067 drb-image-1.1.0/drb/image/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-03-31 08:56:49.000000 drb-image-1.1.0/drb/image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 13:12:37.535067 drb-image-1.1.0/drb/image/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-05-17 11:57:02.000000 drb-image-1.1.0/drb/image/image.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-03-31 12:35:30.000000 drb-image-1.1.0/drb/image/schema.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:12:37.531067 drb-image-1.1.0/drb_image.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-05-17 13:12:37.000000 drb-image-1.1.0/drb_image.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-17 13:12:37.000000 drb-image-1.1.0/drb_image.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 13:12:37.000000 drb-image-1.1.0/drb_image.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 13:12:37.000000 drb-image-1.1.0/drb_image.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       74 2023-05-17 13:12:37.000000 drb-image-1.1.0/drb_image.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-17 13:12:37.000000 drb-image-1.1.0/drb_image.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-31 08:56:49.000000 drb-image-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-17 12:17:14.000000 drb-image-1.1.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-05-17 13:12:37.535067 drb-image-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-31 08:56:49.000000 drb-image-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:12:37.531067 drb-image-1.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6000 2023-03-31 12:35:30.000000 drb-image-1.1.0/tests/test_image_addon.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-03-31 08:56:50.000000 drb-image-1.1.0/versioneer.py
```

### Comparing `drb-image-1.0.0/LICENCE.txt` & `drb-image-1.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-image-1.0.0/PKG-INFO` & `drb-image-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-image
-Version: 1.0.0
+Version: 1.1.0
 Summary: DRB Image Extractor
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -33,48 +33,42 @@
      source:
       - <extractor>: <extractor_content>       # An extractor
 ---
 topic: <topic_uuid>                        # target topic
 default: <name>                            # Default nome to extract
 image:
   <name>:                                  # Variable name
-    freq: [270, 300]                       # Frequency of the image
     source:
       - <extractor>: <extractor_content>       # An extractor
   <name_2>:                                # Variable name
-    freq: [310, 405]                       # Frequency of the image
     source:
       - <extractor>: <extractor_content>       # An extractor
 ---
 topic: <topic_uuid>
 image:  
   <name>:                                  # Variable name
     source:
       - <extractor>: <extractor_content> # An extractor
-        resolution: <resolution>         # Add a resolution value
       - <extractor>: <extractor_content> # An extractor
-        resolution: <resolution>         # Add a resolution value
-        <another_otion> : ...            # Add another option
+        <another_options> : ...            # Add another option
 ```
 
 
 ### How to extract an image ?
 
 For the following addon description.
 
 ```yaml
 topic: b0dad6fa-9ae4-4694-b00b-449cd456d32a # Sentinel-1A Interferometric Wide Swath Level 1 S Product
 default: thumbnail
 image:  
   QuickLook:                                  
     source:
       - xquery: /preview/quick-look.png
-        resolution: 10m         
       - script: sentinel1.image_addon:my_method 
-        resolution: 20m
   thumbnail:
     source:
       - xquery: /thumbnail.png
 ```
 
 The different image node can be extract with this:
```

### Comparing `drb-image-1.0.0/README.md` & `drb-image-1.1.0/drb_image.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: drb-image
+Version: 1.1.0
+Summary: DRB Image Extractor
+Author: GAEL Systems
+Author-email: drb-python@gael.fr
+License: LGPLv3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
 # DRB Image Extractor
 It's an applicative part using DRB allowing to extract image from
 data according its topic.
 
 ## Metadata
 
 ### Packaging
@@ -19,48 +33,42 @@
      source:
       - <extractor>: <extractor_content>       # An extractor
 ---
 topic: <topic_uuid>                        # target topic
 default: <name>                            # Default nome to extract
 image:
   <name>:                                  # Variable name
-    freq: [270, 300]                       # Frequency of the image
     source:
       - <extractor>: <extractor_content>       # An extractor
   <name_2>:                                # Variable name
-    freq: [310, 405]                       # Frequency of the image
     source:
       - <extractor>: <extractor_content>       # An extractor
 ---
 topic: <topic_uuid>
 image:  
   <name>:                                  # Variable name
     source:
       - <extractor>: <extractor_content> # An extractor
-        resolution: <resolution>         # Add a resolution value
       - <extractor>: <extractor_content> # An extractor
-        resolution: <resolution>         # Add a resolution value
-        <another_otion> : ...            # Add another option
+        <another_options> : ...            # Add another option
 ```
 
 
 ### How to extract an image ?
 
 For the following addon description.
 
 ```yaml
 topic: b0dad6fa-9ae4-4694-b00b-449cd456d32a # Sentinel-1A Interferometric Wide Swath Level 1 S Product
 default: thumbnail
 image:  
   QuickLook:                                  
     source:
       - xquery: /preview/quick-look.png
-        resolution: 10m         
       - script: sentinel1.image_addon:my_method 
-        resolution: 20m
   thumbnail:
     source:
       - xquery: /thumbnail.png
 ```
 
 The different image node can be extract with this:
```

### Comparing `drb-image-1.0.0/drb/image/image.py` & `drb-image-1.1.0/drb/image/image.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,55 @@
 from __future__ import annotations
-from typing import Dict, List, Tuple, Optional
+
+from types import ModuleType
+from typing import Dict, List, Tuple, Optional, Union
 from uuid import UUID
 
-from drb.core.item_class import ItemClass
 from drb.core.node import DrbNode
 from drb.exceptions.core import DrbException
-from drb.metadata.metadata import _retrieve_cortex_file
 from drb.topics import resolver
+from drb.topics.dao import ManagerDao
+from drb.topics.topic import DrbTopic
 from drb.utils.plugins import get_entry_points
 from drb.extractor import Extractor
 from drb.extractor.extractor import __factories
-from drb.topics.resolver import ItemClassLoader
 import os
 import jsonschema
 import yaml
 import importlib
 import logging
 
 _logger = logging.getLogger('DrbImage')
 _schema = os.path.join(os.path.dirname(__file__), 'schema.yml')
 
 
+# FIXME Refactor this method in drb.utils.plugin
+def _retrieve_cortex_file(module: ModuleType) -> str:
+    """
+    Retrieves the metadata cortex file from the given module.
+
+    Parameters:
+        module (ModuleType): target module where the cortex metadata file will
+                             be search
+    Returns:
+        str - path to the cortex metadata file
+    Raises:
+        FileNotFound: If the metadata cortex file is not found
+    """
+    directory = os.path.dirname(module.__file__)
+    path = os.path.join(directory, 'cortex.yml')
+    if not os.path.exists(path):
+        path = os.path.join(directory, 'cortex.yaml')
+
+    if not os.path.exists(path):
+        raise FileNotFoundError(f'File not found: {path}')
+
+    return path
+
+
 def parse_extractor(data: dict):
     for key, value in data.items():
         return __factories[key](value)
 
 
 def validate_md_cortex_file(path: str) -> None:
     """
@@ -52,25 +77,20 @@
 
 
 def _load_image(yaml_data: dict) -> Tuple[UUID, list[Image], str]:
     uuid = UUID(yaml_data['topic'])
     names = list(yaml_data['image'].keys())
     res = []
     for name in names:
-        freq = []
-
-        if 'freq' in yaml_data['image'][name]:
-            freq = yaml_data['image'][name]['freq']
 
         for data in yaml_data['image'][name]['source']:
             if 'extractor' in data.keys():
                 extractor = parse_extractor(data['extractor'])
                 res.append(Image(name=name,
                                  extractor=extractor,
-                                 freq=freq,
                                  data=data)
                            )
 
     return uuid, res, yaml_data.get('default', None)
 
 
 def _load_all_image() -> Dict[UUID, Tuple[List[Image], str]]:
@@ -100,97 +120,99 @@
                 uuid, img, default = _load_image(data)
                 image[uuid] = (img, default)
     return image
 
 
 class Image:
     def __init__(self, name: str, extractor: Extractor,
-                 freq: str = None, data: dict = {}):
+                 data: dict = {}):
         self._name = name
         self.extractor = extractor
-        self._freq = freq
         self._data = data
+        self._node = None
 
     def __getattr__(self, item):
         if item in self._data.keys():
             return self._data[item]
         raise AttributeError
 
     @property
     def name(self) -> str:
         """
         Provide the name of the image.
         """
         return self._name
 
     @property
-    def freq(self) -> List:
-        """
-        Provide the frequency of the image with a list
-         of int, the default value is an empty list.
-        """
-        return self._freq
-
-    @property
     def addon_data(self) -> Optional[dict]:
         """
         Provide the raw data of the image addon,
         in the dict format.
         in the dict format.
         """
         return self._data
 
-    def node(self, node: DrbNode) -> DrbNode:  # DrbImageNode
+    @property
+    def node(self):
+        return self._node
+
+    @node.setter
+    def node(self, value: DrbNode) -> None:
+        self._node = value
+
+    def image_node(self) -> DrbNode:  # DrbImageNode
         """
         Provides the current image as a DrbNode
         """
-        return self.extractor.extract(node)
+        return self.extractor.extract(self.node)
+
+    def get_impl(self, impl):
+        return self.image_node().get_impl(impl)
 
 
 class AddonImage:
     @staticmethod
     def images(source) -> List[str]:
         """
         Returns available images list that can be generated
         Parameters:
-          source (DrbNode, Topic):
+          source (DrbNode, str, Topic):
         """
         _images = _load_all_image()
         res = []
 
         if isinstance(source, DrbNode) or isinstance(source, str):
             topic, node = resolver.resolve(source)
-        elif isinstance(source, ItemClass):
+        elif isinstance(source, DrbTopic):
             topic = source
         else:
             raise DrbException(
                 f"Cannont find any image addon corresponding to {source}")
 
         if topic.id in _images.keys():
             for e in _images[topic.id][0]:
                 res.append(e.name)
-        if topic.parent_class_id is not None and \
-                topic.parent_class_id in _images.keys():
-            res.append(AddonImage.images(
-                ItemClassLoader().get_item_class(topic.parent_class_id)
-            ))
+        if topic.subClassOf is not None:
+            for parent_id in topic.subClassOf:
+                if parent_id in _images.keys():
+                    res.append(AddonImage.images(
+                        ManagerDao().get_drb_topic(parent_id)
+                    ))
 
         return res
 
     @staticmethod
-    def create(node: DrbNode,
+    def create(node: Union[DrbNode, str],
                image_name: str = None,
-               freq: int = None, **kwargs) -> Image:
+               **kwargs) -> Image:
         """
         Create a new image representation on the node
         Parameters:
           node (DrbNode): an image will be generated from that node
           image_name (str): (default ``None``)
-          freq (int): (default ``None``)
-          resolution (str): (default ``None``)
         """
         _images = _load_all_image()
 
         topic, node = resolver.resolve(node)
 
         try:
             tmp = _images[topic.id]
@@ -203,42 +225,32 @@
         if image_name is not None:
             remove = []
             for t in res:
                 if t.name != image_name:
                     remove.append(t)
             res = list(set(res) - set(remove))
 
-        if freq is not None:
-            remove = []
-            freq = int(freq)
-            for t in res:
-                if len(t.freq) == 2:
-                    if not t.freq[0] <= freq <= t.freq[1]:
-                        remove.append(t)
-                else:
-                    remove.append(t)
-            res = list(set(res) - set(remove))
-
         if options:
             remove = []
             for opt in options:
                 for t in res:
                     try:
                         if t.__getattr__(opt) != kwargs[opt]:
                             remove.append(t)
                     except AttributeError:
                         pass
             res = list(set(res) - set(remove))
 
-        if image_name is None and freq is None and not kwargs:
+        if image_name is None and not kwargs:
             remove = []
             if tmp[1] is not None:
                 for t in res:
                     if t.name != tmp[1]:
                         remove.append(t)
                 res = list(set(res) - set(remove))
 
         try:
+            res[0].node = node
             return res[0]
         except IndexError:
             raise DrbException(f'No image descriptor found for '
-                               f'{image_name}, {freq}, {kwargs}')
+                               f'{image_name}, {kwargs}')
```

### Comparing `drb-image-1.0.0/drb/image/schema.yml` & `drb-image-1.1.0/drb/image/schema.yml`

 * *Files 18% similar despite different names*

```diff
@@ -26,20 +26,14 @@
     minProperties: 1
     maxProperties: 2
     additionalProperties: no
     properties:
       name: {
         type: string
       }
-      freq: {
-        type: array,
-        "items": {
-          "type": "number"
-        }
-      }
       extractor:
         type: object
         items: { $ref: '#/definitions/extractor' }
         minItems: 1
 properties:
   topic:
     type: string
```

### Comparing `drb-image-1.0.0/drb_image.egg-info/PKG-INFO` & `drb-image-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: drb-image
-Version: 1.0.0
-Summary: DRB Image Extractor
-Author: GAEL Systems
-Author-email: drb-python@gael.fr
-License: LGPLv3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Environment :: Plugins
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
 # DRB Image Extractor
 It's an applicative part using DRB allowing to extract image from
 data according its topic.
 
 ## Metadata
 
 ### Packaging
@@ -33,48 +19,42 @@
      source:
       - <extractor>: <extractor_content>       # An extractor
 ---
 topic: <topic_uuid>                        # target topic
 default: <name>                            # Default nome to extract
 image:
   <name>:                                  # Variable name
-    freq: [270, 300]                       # Frequency of the image
     source:
       - <extractor>: <extractor_content>       # An extractor
   <name_2>:                                # Variable name
-    freq: [310, 405]                       # Frequency of the image
     source:
       - <extractor>: <extractor_content>       # An extractor
 ---
 topic: <topic_uuid>
 image:  
   <name>:                                  # Variable name
     source:
       - <extractor>: <extractor_content> # An extractor
-        resolution: <resolution>         # Add a resolution value
       - <extractor>: <extractor_content> # An extractor
-        resolution: <resolution>         # Add a resolution value
-        <another_otion> : ...            # Add another option
+        <another_options> : ...            # Add another option
 ```
 
 
 ### How to extract an image ?
 
 For the following addon description.
 
 ```yaml
 topic: b0dad6fa-9ae4-4694-b00b-449cd456d32a # Sentinel-1A Interferometric Wide Swath Level 1 S Product
 default: thumbnail
 image:  
   QuickLook:                                  
     source:
       - xquery: /preview/quick-look.png
-        resolution: 10m         
       - script: sentinel1.image_addon:my_method 
-        resolution: 20m
   thumbnail:
     source:
       - xquery: /thumbnail.png
 ```
 
 The different image node can be extract with this:
```

### Comparing `drb-image-1.0.0/setup.cfg` & `drb-image-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-image-1.0.0/tests/test_image_addon.py` & `drb-image-1.1.0/tests/test_image_addon.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 
+import rasterio
 from drb.drivers.image import DrbImageBaseNode
 from drb.drivers.netcdf import DrbNetcdfNode
 from drb.exceptions.core import DrbException
 from drb.topics import resolver
 
 from drb.image import AddonImage
 from drb.image.image import Image
@@ -30,102 +31,104 @@
     def test_constant(self):
         node = resolver.create(self.S1)
         extract = AddonImage.create(node)
 
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('quicklook', extract.name)
-        self.assertEqual([], extract.freq)
 
-        base_node = extract.node(node=node)
+        base_node = extract.image_node()
         self.assertIsNotNone(base_node)
         self.assertIsInstance(base_node, DrbImageBaseNode)
 
     def test_python(self):
         node = resolver.create(self.S2)
 
         extract = AddonImage.create(node)
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('TrueColorImage', extract.name)
-        self.assertEqual([], extract.freq)
 
-        base_node = extract.node(node)
+        base_node = extract.image_node()
         self.assertIsNotNone(base_node)
         self.assertIsInstance(base_node, DrbImageBaseNode)
 
     def test_script(self):
         node = resolver.create(self.S5)
 
         extract = AddonImage.create(node)
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('index_354_388', extract.name)
-        self.assertEqual([310, 405], extract.freq)
+        self.assertEqual(310, extract.frequency)
 
-        base_node = extract.node(node)
+        base_node = extract.image_node()
         self.assertIsNotNone(base_node)
         self.assertIsInstance(base_node, DrbImageBaseNode)
 
     def test_resolutions(self):
         node = resolver.create(self.S1_LO)
 
         extract = AddonImage.create(node, resolution='10m')
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('bo4', extract.name)
         self.assertEqual('10m', extract.resolution)
-        self.assertEqual([205, 305], extract.freq)
+        self.assertEqual([205, 305], extract.frequency)
 
         extract = AddonImage.create(node, resolution='20m')
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('bo4', extract.name)
         self.assertEqual('20m', extract.resolution)
-        self.assertEqual([205, 305], extract.freq)
+        self.assertEqual([205, 305], extract.frequency)
 
     def test_freq(self):
         node = resolver.create(self.S5)
 
-        extract = AddonImage.create(node, freq='290')
+        extract = AddonImage.create(node, frequency=[270, 300])
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('index_340_380', extract.name)
-        self.assertEqual([270, 300], extract.freq)
+        self.assertEqual([270, 300], extract.frequency)
 
-        extract = AddonImage.create(node, freq='320')
+        extract = AddonImage.create(node, frequency=310)
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('index_354_388', extract.name)
-        self.assertEqual([310, 405], extract.freq)
+        self.assertEqual(310, extract.frequency)
+
+        with self.assertRaises(DrbException):
+            AddonImage.create(node, frequency=320)
 
     def test_filter(self):
         node = resolver.create(self.S5)
 
         extract = AddonImage.create(node,
                                     image_name='index_340_380',
                                     freq='290')
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('index_340_380', extract.name)
-        self.assertEqual([270, 300], extract.freq)
+        self.assertEqual([270, 300], extract.frequency)
 
         with self.assertRaises(DrbException):
-            AddonImage.create(node, image_name='index_354_388', freq='290')
+            AddonImage.create(node, image_name='index_354_388',
+                              frequency='290')
 
     def test_default(self):
         node = resolver.create(self.S5)
 
         extract = AddonImage.create(node, image_name='index_340_380')
         self.assertIsNotNone(extract)
         self.assertIsInstance(extract, Image)
         self.assertEqual('index_340_380', extract.name)
-        self.assertEqual([270, 300], extract.freq)
+        self.assertEqual([270, 300], extract.frequency)
 
-        base_node = extract.node(node)
+        base_node = extract.image_node()
         self.assertIsNotNone(base_node)
         self.assertIsInstance(base_node, DrbNetcdfNode)
 
         with self.assertRaises(DrbException):
             AddonImage.create(node, image_name='Wrong_name')
 
     def test_load_images(self):
@@ -150,7 +153,18 @@
         self.assertEqual(s1[0], 'quicklook')
 
         with self.assertRaises(DrbException):
             AddonImage.images(1)
 
         with self.assertRaises(TypeError):
             AddonImage.images()
+
+    def test_simpl_usage(self):
+        extract = AddonImage.create(self.S1)
+        self.assertIsNotNone(extract)
+        self.assertIsInstance(extract, Image)
+        impl = extract.get_impl(rasterio.DatasetReader)
+        self.assertIsInstance(impl, rasterio.io.DatasetReader)
+        self.assertEqual(
+            impl,
+            extract.image_node().get_impl(rasterio.DatasetReader)
+        )
```

### Comparing `drb-image-1.0.0/versioneer.py` & `drb-image-1.1.0/versioneer.py`

 * *Files identical despite different names*

