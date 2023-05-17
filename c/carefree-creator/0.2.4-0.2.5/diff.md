# Comparing `tmp/carefree-creator-0.2.4.tar.gz` & `tmp/carefree-creator-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-creator-0.2.4.tar", last modified: Fri May 12 11:23:59 2023, max compression
+gzip compressed data, was "carefree-creator-0.2.5.tar", last modified: Wed May 17 13:25:15 2023, max compression
```

## Comparing `carefree-creator-0.2.4.tar` & `carefree-creator-0.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.014854 carefree-creator-0.2.4/
--rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4419 2023-05-12 11:23:59.013854 carefree-creator-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4117 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 11:23:58.990343 carefree-creator-0.2.4/carefree_creator.egg-info/
--rw-rw-rw-   0        0        0     4419 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      138 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.002855 carefree-creator-0.2.4/cfcreator/
--rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.4/cfcreator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.003855 carefree-creator-0.2.4/cfcreator/apis/
--rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.4/cfcreator/apis/config.yml
--rw-rw-rw-   0        0        0     9036 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/apis/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.006855 carefree-creator-0.2.4/cfcreator/apis/kafka/
--rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.4/cfcreator/apis/kafka/config.yml
--rw-rw-rw-   0        0        0    13717 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/apis/kafka/consumer.py
--rw-rw-rw-   0        0        0    12109 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/apis/kafka/producer.py
--rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/cli.py
--rw-rw-rw-   0        0        0    22741 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/common.py
--rw-rw-rw-   0        0        0    15062 2023-05-09 06:40:22.000000 carefree-creator-0.2.4/cfcreator/control.py
--rw-rw-rw-   0        0        0     2226 2023-05-09 07:17:42.000000 carefree-creator-0.2.4/cfcreator/control_multi.py
--rw-rw-rw-   0        0        0     8444 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/cos.py
--rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.4/cfcreator/cv.py
--rw-rw-rw-   0        0        0     2458 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/endpoints.py
--rw-rw-rw-   0        0        0    20523 2023-05-09 04:37:43.000000 carefree-creator-0.2.4/cfcreator/img2img.py
--rw-rw-rw-   0        0        0     1657 2023-05-09 04:37:43.000000 carefree-creator-0.2.4/cfcreator/img2txt.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.009854 carefree-creator-0.2.4/cfcreator/legacy/
--rw-rw-rw-   0        0        0        0 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/cfcreator/legacy/__init__.py
--rw-rw-rw-   0        0        0     2102 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/cfcreator/legacy/common.py
--rw-rw-rw-   0        0        0    13724 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/cfcreator/legacy/control.py
--rw-rw-rw-   0        0        0     3216 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/cfcreator/legacy/control_multi.py
--rw-rw-rw-   0        0        0     3298 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/parameters.py
--rw-rw-rw-   0        0        0     3431 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.012854 carefree-creator-0.2.4/cfcreator/sdks/
--rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.4/cfcreator/sdks/__init__.py
--rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/sdks/direct.py
--rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/sdks/kafka.py
--rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/sdks/utils.py
--rw-rw-rw-   0        0        0     7054 2023-05-09 04:37:43.000000 carefree-creator-0.2.4/cfcreator/txt2img.py
--rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/txt2txt.py
--rw-rw-rw-   0        0        0     4631 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-12 11:23:59.014854 carefree-creator-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-05-12 11:22:40.000000 carefree-creator-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.245986 carefree-creator-0.2.5/
+-rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4419 2023-05-17 13:25:15.245986 carefree-creator-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4117 2023-05-06 03:00:57.000000 carefree-creator-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.234023 carefree-creator-0.2.5/carefree_creator.egg-info/
+-rw-rw-rw-   0        0        0     4419 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.240006 carefree-creator-0.2.5/cfcreator/
+-rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.5/cfcreator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.241003 carefree-creator-0.2.5/cfcreator/apis/
+-rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.5/cfcreator/apis/config.yml
+-rw-rw-rw-   0        0        0     9028 2023-05-17 13:02:59.000000 carefree-creator-0.2.5/cfcreator/apis/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.241999 carefree-creator-0.2.5/cfcreator/apis/kafka/
+-rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.5/cfcreator/apis/kafka/config.yml
+-rw-rw-rw-   0        0        0    13714 2023-05-17 13:00:21.000000 carefree-creator-0.2.5/cfcreator/apis/kafka/consumer.py
+-rw-rw-rw-   0        0        0    12102 2023-05-17 13:02:27.000000 carefree-creator-0.2.5/cfcreator/apis/kafka/producer.py
+-rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/cli.py
+-rw-rw-rw-   0        0        0    23231 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/common.py
+-rw-rw-rw-   0        0        0    16085 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/control.py
+-rw-rw-rw-   0        0        0     2226 2023-05-09 07:17:42.000000 carefree-creator-0.2.5/cfcreator/control_multi.py
+-rw-rw-rw-   0        0        0     8444 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/cos.py
+-rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.5/cfcreator/cv.py
+-rw-rw-rw-   0        0        0     2458 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/endpoints.py
+-rw-rw-rw-   0        0        0    20523 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/img2img.py
+-rw-rw-rw-   0        0        0     1657 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/img2txt.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.243993 carefree-creator-0.2.5/cfcreator/legacy/
+-rw-rw-rw-   0        0        0        0 2023-05-06 03:00:57.000000 carefree-creator-0.2.5/cfcreator/legacy/__init__.py
+-rw-rw-rw-   0        0        0     2102 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/legacy/common.py
+-rw-rw-rw-   0        0        0    13724 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/legacy/control.py
+-rw-rw-rw-   0        0        0     3216 2023-05-06 03:00:57.000000 carefree-creator-0.2.5/cfcreator/legacy/control_multi.py
+-rw-rw-rw-   0        0        0     3298 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/parameters.py
+-rw-rw-rw-   0        0        0     3431 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.244989 carefree-creator-0.2.5/cfcreator/sdks/
+-rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.5/cfcreator/sdks/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/sdks/direct.py
+-rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/sdks/kafka.py
+-rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/sdks/utils.py
+-rw-rw-rw-   0        0        0     7087 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/txt2img.py
+-rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/txt2txt.py
+-rw-rw-rw-   0        0        0     5451 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 13:25:15.245986 carefree-creator-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-05-17 13:23:54.000000 carefree-creator-0.2.5/setup.py
```

### Comparing `carefree-creator-0.2.4/LICENSE` & `carefree-creator-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/PKG-INFO` & `carefree-creator-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-creator
-Version: 0.2.4
+Version: 0.2.5
 Summary: An AI-powered creator for everyone.
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 License-File: LICENSE
```

### Comparing `carefree-creator-0.2.4/README.md` & `carefree-creator-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/carefree_creator.egg-info/PKG-INFO` & `carefree-creator-0.2.5/carefree_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-creator
-Version: 0.2.4
+Version: 0.2.5
 Summary: An AI-powered creator for everyone.
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 License-File: LICENSE
```

### Comparing `carefree-creator-0.2.4/carefree_creator.egg-info/SOURCES.txt` & `carefree-creator-0.2.5/carefree_creator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/apis/config.yml` & `carefree-creator-0.2.5/cfcreator/apis/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/apis/interface.py` & `carefree-creator-0.2.5/cfcreator/apis/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 from pydantic import BaseModel
 from pkg_resources import get_distribution
 from cftool.array import tensor_dict_type
 from fastapi.openapi.utils import get_openapi
 from fastapi.middleware.cors import CORSMiddleware
 
 from cfclient.models import *
+from cftool.web import get_responses
+from cftool.web import get_image_response_kwargs
 from cfclient.core import HttpClient
 from cfclient.core import TritonClient
-from cfclient.utils import get_responses
 from cfclient.utils import run_algorithm
-from cfclient.utils import get_image_response_kwargs
 
 from cfcreator import *
 from cfcreator.utils import api_pool
 
 
 app = FastAPI()
 root = os.path.dirname(__file__)
```

### Comparing `carefree-creator-0.2.4/cfcreator/apis/kafka/config.yml` & `carefree-creator-0.2.5/cfcreator/apis/kafka/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/apis/kafka/consumer.py` & `carefree-creator-0.2.5/cfcreator/apis/kafka/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 from typing import Dict
 from typing import Union
 from fastapi import Response
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 
 from cfclient.models import *
+from cftool.misc import get_err_msg
 from cftool.misc import shallow_copy_dict
 from cfclient.core import HttpClient
 from cfclient.core import TritonClient
-from cfclient.utils import get_err_msg
 from cfclient.utils import run_algorithm
 
 # This is necessary to register the algorithms
 from cfcreator import *
 from cfcreator.legacy.control import ControlNetModel as LegacyControlNetModel
 from cfcreator.legacy.control_multi import ControlMultiModel as LegacyControlMultiModel
```

### Comparing `carefree-creator-0.2.4/cfcreator/apis/kafka/producer.py` & `carefree-creator-0.2.5/cfcreator/apis/kafka/producer.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 from fastapi import FastAPI
 from fastapi import Response
 from pydantic import Field
 from pydantic import BaseModel
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 from pkg_resources import get_distribution
-from cftool.misc import random_hash
 from fastapi.openapi.utils import get_openapi
 from fastapi.middleware.cors import CORSMiddleware
 
-from cfclient.utils import get_err_msg
-from cfclient.utils import get_responses
+from cftool.web import get_responses
+from cftool.misc import get_err_msg
+from cftool.misc import random_hash
 
 from cfcreator import *
 
 
 app = FastAPI()
 root = os.path.dirname(__file__)
```

### Comparing `carefree-creator-0.2.4/cfcreator/cli.py` & `carefree-creator-0.2.5/cfcreator/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/common.py` & `carefree-creator-0.2.5/cfcreator/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import Callable
 from typing import Optional
+from pathlib import Path
 from pydantic import Field
 from pydantic import BaseModel
 from functools import partial
 from cftool.cv import np_to_bytes
+from cflearn.zoo import DLZoo
+from cflearn.parameters import OPT
 from cfclient.models import TextModel
 from cfclient.models import ImageModel
 from cfclient.models import AlgorithmBase
-from cflearn.zoo import DLZoo
-from cflearn.parameters import OPT
+from safetensors.torch import load_file
 from cflearn.api.cv import SDVersions
 from cflearn.api.cv import DiffusionAPI
 from cflearn.api.cv import TranslatorAPI
 from cflearn.api.cv import ImageHarmonizationAPI
 from cflearn.api.cv import ControlledDiffusionAPI
 from cflearn.misc.toolkit import _get_file_size
 from cflearn.misc.toolkit import download_model
@@ -130,14 +132,17 @@
             else _get_file_size(converted_path)
         )
         if f_size is None or v_size != f_size:
             if f_size is not None:
                 print(f">> {version} has been converted but size mismatch")
             print(f">> converting {version}")
             model_path = os.path.join(external_folder, f"{version}.ckpt")
+            if not os.path.isfile(model_path):
+                st_path = os.path.join(external_folder, f"{version}.safetensors")
+                torch.save(load_file(st_path), model_path)
             d = cflearn.scripts.sd.convert(model_path, m, load=False)
             torch.save(d, converted_path)
             sizes[version] = _get_file_size(converted_path)
         m.sd_weights.register(version, converted_path)
     with open(converted_sizes_path, "w") as f:
         json.dump(sizes, f)
 
@@ -440,52 +445,59 @@
         description="Custom embeddings, often used in textual inversion.",
     )
     tome_info: TomeInfoModel = Field(TomeInfoModel(), description="tomesd settings.")
     lora_scales: Optional[Dict[str, float]] = Field(
         None,
         description="lora scales, key is the name, value is the weight.",
     )
+    lora_paths: Optional[List[str]] = Field(
+        None,
+        description="If provided, we will dynamically load lora from the given paths.",
+    )
 
 
 class ReturnArraysModel(BaseModel):
     return_arrays: bool = Field(
         False,
         description="Whether return List[np.ndarray] directly, only for internal usages.",
     )
 
 
 class CommonSDInpaintingModel(ReturnArraysModel):
     keep_original: bool = Field(
         False,
         description="Whether strictly keep the original image identical in the output image.",
     )
+    ref_mask_smooth: int = Field(
+        3,
+        description="The smoothness of the reference's mask, `0` means no smooth.",
+    )
     use_raw_inpainting: bool = Field(
         False,
         description="""
 Whether use the raw inpainting method.
 > This is useful when you want to apply inpainting with custom SD models.
 """,
     )
+    raw_inpainting_use_ref: bool = Field(
+        False,
+        description="Whether use input image as reference.",
+    )
     raw_inpainting_fidelity: float = Field(
         0.2,
         ge=0.0,
         le=1.0,
-        description="The fidelity of the input image when using raw inpainting.",
+        description="The fidelity of the input image when it is used as reference in raw inpainting.",
     )
-    ref_url: str = Field(
-        "",
-        description="""
-The `cdn` / `cos` url of the reference image.
-> `cos` url from cloud is preferred.
-> If empty string is provided, we will not use the reference feature.  
-""",
+    use_latent_guidance: bool = Field(
+        False,
+        description="Whether use the latent of the givent image to guide the generation.",
     )
-    ref_fidelity: float = Field(
-        0.2,
-        description="Fidelity of the reference image (if provided)",
+    reference_fidelity: float = Field(
+        0.0, description="Fidelity of the reference image."
     )
 
 
 class HighresModel(BaseModel):
     fidelity: float = Field(0.3, description="Fidelity of the original latent.")
     upscale_factor: float = Field(2.0, description="Upscale factor.")
     max_wh: int = Field(1024, description="Max width or height of the output image.")
@@ -504,15 +516,15 @@
 
 
 class ControlStrengthModel(BaseModel):
     control_strength: float = Field(1.0, description="The strength of the control.")
 
 
 class _ControlNetModel(BaseModel):
-    url: Optional[str] = Field(None, description="specify this to perform img2img")
+    url: Optional[str] = Field(None, description="specify this to do img2img")
     hint_url: str = Field(
         "",
         description="""
 The `cdn` / `cos` url of the user's hint image.
 > If empty string is provided, we will use `url` as `hint_url`.
 > `cos` url from `qcloud` is preferred.
 """,
@@ -533,30 +545,19 @@
     )
     guess_mode: bool = Field(False, description="Guess mode.")
     use_audit: bool = Field(False, description="Whether audit the outputs.")
     no_switch: bool = Field(
         False,
         description="Whether not to switch the ControlNet weights even when the base model has switched.",
     )
-
-
-# only useful when inpainting model is used
-class _InpaintingMixin(BaseModel):
-    use_latent_guidance: bool = Field(
-        False,
-        description="Whether use the latent of the givent image to guide the generation.",
-    )
-    reference_fidelity: float = Field(
-        0.0, description="Fidelity of the reference image."
-    )
+    mask_url: Optional[str] = Field(None, description="specify this to do inpainting")
 
 
 class ControlNetModel(
-    ReturnArraysModel,
-    _InpaintingMixin,
+    CommonSDInpaintingModel,
     DiffusionModel,
     MaxWHModel,
     _ControlNetModel,
 ):
     pass
 
 
@@ -611,14 +612,23 @@
         sampler=data.sampler,
         verbose=verbose(),
         clip_skip=clip_skip,
         custom_embeddings=data.custom_embeddings or None,
     )
 
 
+def handle_diffusion_inpainting_model(data: CommonSDInpaintingModel) -> Dict[str, Any]:
+    return dict(
+        ref_mask_smooth=data.ref_mask_smooth,
+        use_raw_inpainting=data.use_raw_inpainting,
+        raw_inpainting_use_ref=data.raw_inpainting_use_ref,
+        raw_inpainting_fidelity=data.raw_inpainting_fidelity,
+    )
+
+
 class GetPromptModel(BaseModel):
     text: str
     need_translate: bool = Field(
         True,
         description="Whether we need to translate the input text.",
     )
 
@@ -651,29 +661,14 @@
 
     async def download_with_retry(self, url: str) -> bytes:
         return await download_with_retry(self.http_client.session, url)
 
     async def download_image_with_retry(self, url: str) -> Image.Image:
         return await download_image_with_retry(self.http_client.session, url)
 
-    async def handle_diffusion_inpainting_model(
-        self,
-        data: CommonSDInpaintingModel,
-    ) -> Dict[str, Any]:
-        if not data.ref_url:
-            reference = None
-        else:
-            reference = await self.download_image_with_retry(data.ref_url)
-        return dict(
-            use_raw_inpainting=data.use_raw_inpainting,
-            raw_inpainting_fidelity=data.raw_inpainting_fidelity,
-            reference=reference,
-            reference_fidelity=data.ref_fidelity,
-        )
-
 
 # kafka
 
 
 class Status(str, Enum):
     PENDING = "pending"
     WORKING = "working"
@@ -685,24 +680,32 @@
 
 # shortcuts
 
 
 class SDParameters(BaseModel):
     is_anime: bool
     version: MergedVersions
+    lora_paths: Optional[List[str]]
 
 
 def get_sd_from(data: SDParameters) -> ControlledDiffusionAPI:
     if not data.is_anime:
         version = data.version
     else:
         version = data.version if data.version.startswith("anime") else "anime"
     sd: ControlledDiffusionAPI = api_pool.get(APIs.SD)
     sd.switch_sd(version)
     sd.disable_control()
+    if data.lora_paths is not None:
+        sd_m = sd.m
+        if not isinstance(sd_m, StableDiffusion):
+            raise ValueError("sd lora only works for StableDiffusion")
+        for lora_path in data.lora_paths:
+            key = Path(lora_path).stem
+            sd.load_sd_lora(key, path=lora_path)
     return sd
 
 
 __all__ = [
     "endpoint2algorithm",
     "DiffusionModel",
     "HighresModel",
```

### Comparing `carefree-creator-0.2.4/cfcreator/control.py` & `carefree-creator-0.2.5/cfcreator/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from PIL import Image
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import Tuple
-from typing import Union
 from typing import Optional
 from fastapi import Response
 from pydantic import Field
 from pydantic import BaseModel
 from cftool.cv import to_rgb
 from cftool.cv import to_uint8
 from cftool.cv import np_to_bytes
@@ -25,18 +24,20 @@
 from cfclient.models.core import ImageModel
 from cflearn.api.cv.diffusion import ControlNetHints
 from cflearn.api.cv.diffusion import ControlledDiffusionAPI
 
 from .utils import api_pool
 from .utils import to_canvas
 from .utils import resize_image
+from .utils import to_contrast_rgb
 from .utils import APIs
 from .common import BaseSDTag
 from .common import register_sd
 from .common import handle_diffusion_model
+from .common import handle_diffusion_inpainting_model
 from .common import IAlgorithm
 from .common import ControlNetModel
 from .common import ReturnArraysModel
 from .common import ControlStrengthModel
 
 
 root = os.path.dirname(__file__)
@@ -66,43 +67,62 @@
 TKey = Tuple[str, str, bool]
 
 
 def get_bundle_key(bundle: ControlNetBundle) -> TKey:
     return bundle.type, bundle.data.hint_url, bundle.data.bypass_annotator
 
 
+def get_hint_url_key(url: str) -> str:
+    return f"{url}-hint"
+
+
 async def apply_control(
     self: IAlgorithm,
     api_key: APIs,
     common: ControlNetModel,
     controls: List[ControlNetBundle],
     normalized_inpainting_mask: Optional[np.ndarray] = None,
 ) -> apply_response:
     api: ControlledDiffusionAPI = api_pool.get(api_key, no_change=True)
     need_change_device = api_pool.need_change_device(api_key)
     api.enable_control()
     # download images
-    urls = set() if common.url is None else {common.url}
+    urls = set()
+    is_hint = {}
+    is_global = {}
+    if common.url is not None:
+        urls.add(common.url)
+        is_global[common.url] = True
+    if common.mask_url is not None:
+        urls.add(common.mask_url)
+        is_global[common.mask_url] = True
     for bundle in controls:
         if not bundle.data.hint_url:
             raise ValueError("hint url should be provided in `controls`")
         urls.add(bundle.data.hint_url)
+        is_hint[bundle.data.hint_url] = True
     sorted_urls = sorted(urls)
     futures = [self.download_image_with_retry(url) for url in sorted_urls]
-    images = await asyncio.gather(*futures)
-    image_arrays = [np.array(to_rgb(image)) for image in images]
+    images: List[Image.Image] = await asyncio.gather(*futures)
     ## make sure that every image should have the same size
-    original_h, original_w = image_arrays[0].shape[:2]
-    for image_array in image_arrays[1:]:
-        h, w = image_array.shape[:2]
-        if h != original_h or w != original_w:
-            msg = f"image shape mismatch: {(original_h, original_w)} vs {(h, w)}"
+    original_w, original_h = images[0].size
+    for im in images[1:]:
+        w, h = im.size
+        if w != original_w or h != original_h:
+            msg = f"image size mismatch: {(original_w, original_h)} vs {(w, h)}"
             raise ValueError(msg)
     ## construct a lookup table
-    image_array_d = {url: array for url, array in zip(sorted_urls, image_arrays)}
+    image_array_d: Dict[str, np.ndarray] = {}
+    for url, image in zip(sorted_urls, images):
+        i_is_global = is_global.get(url, False)
+        i_is_hint = is_hint.get(url, False)
+        if i_is_global:
+            image_array_d[url] = np.array(to_rgb(image))
+        if i_is_hint:
+            image_array_d[get_hint_url_key(url)] = np.array(to_contrast_rgb(image))
     # gather detect resolution
     detect_resolutions = []
     for bundle in controls:
         detect_resolutions.append(getattr(bundle.data, "detect_resolution", None))
     # calculate suitable size
     resize_to_original = lambda array: cv2.resize(
         array,
@@ -126,15 +146,15 @@
     all_keys: List[TKey] = []
     ## Tensor for input, ndarray for results
     all_key_values: Dict[TKey, Tuple[torch.Tensor, np.ndarray]] = {}
     all_annotator_change_device_times = []
     for bundle, detect_resolution in zip(controls, detect_resolutions):
         i_type = bundle.type
         i_data = bundle.data
-        i_hint_image = image_array_d[i_data.hint_url]
+        i_hint_image = image_array_d[get_hint_url_key(i_data.hint_url)]
         i_bypass_annotator = i_data.bypass_annotator
         key = get_bundle_key(bundle)
         all_keys.append(key)
         i_value = all_key_values.get(key)
         if i_value is not None:
             continue
         if detect_resolution is not None and not i_bypass_annotator:
@@ -187,23 +207,32 @@
     kw["hint_start"] = [b.data.hint_start for b in controls]
     kw["max_wh"] = common.max_wh
     dt = time.time()
     if need_change_device:
         api.to("cuda:0", use_half=True, no_annotator=True)
     change_diffusion_device_time = time.time() - dt
     # inpainting workaround
-    if api.m.unet_kw["in_channels"] == 9:
+    common = common.copy()
+    is_sd_inpainting = api.m.unet_kw["in_channels"] == 9
+    common.use_raw_inpainting = not is_sd_inpainting
+    if common.mask_url is not None or is_sd_inpainting:
         if common.url is None:
             raise ValueError("`url` should be provided to inpainting")
-        if normalized_inpainting_mask is None:
-            raise ValueError("`normalized_input_mask` should be provided to inpainting")
+        if normalized_inpainting_mask is not None:
+            inpainting_mask = Image.fromarray(to_uint8(normalized_inpainting_mask))
+        else:
+            if common.mask_url is None:
+                raise ValueError(
+                    "either `mask_url` or `normalized_input_mask` "
+                    "should be provided to perform ControlNet inpainting"
+                )
+            inpainting_mask = Image.fromarray(image_array_d[common.mask_url])
+            inpainting_mask = inpainting_mask.convert("L")
         image = Image.fromarray(image_array_d[common.url])
-        inpainting_mask = Image.fromarray(to_uint8(normalized_inpainting_mask))
-        kw["use_latent_guidance"] = common.use_latent_guidance
-        kw["reference_fidelity"] = common.reference_fidelity
+        kw.update(handle_diffusion_inpainting_model(common))
         outs = api.txt2img_inpainting(cond, image, inpainting_mask, **kw)
     elif common.url is None:
         kw["size"] = w, h
         outs = api.txt2img(cond, **kw)
     else:
         init_image = cv2.resize(
             image_array_d[common.url],
```

### Comparing `carefree-creator-0.2.4/cfcreator/control_multi.py` & `carefree-creator-0.2.5/cfcreator/control_multi.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/cos.py` & `carefree-creator-0.2.5/cfcreator/cos.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/cv.py` & `carefree-creator-0.2.5/cfcreator/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/endpoints.py` & `carefree-creator-0.2.5/cfcreator/endpoints.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/img2img.py` & `carefree-creator-0.2.5/cfcreator/img2img.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/img2txt.py` & `carefree-creator-0.2.5/cfcreator/img2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/legacy/common.py` & `carefree-creator-0.2.5/cfcreator/legacy/common.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/legacy/control.py` & `carefree-creator-0.2.5/cfcreator/legacy/control.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/legacy/control_multi.py` & `carefree-creator-0.2.5/cfcreator/legacy/control_multi.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/parameters.py` & `carefree-creator-0.2.5/cfcreator/parameters.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/pipeline.py` & `carefree-creator-0.2.5/cfcreator/pipeline.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/sdks/direct.py` & `carefree-creator-0.2.5/cfcreator/sdks/direct.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/sdks/kafka.py` & `carefree-creator-0.2.5/cfcreator/sdks/kafka.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/sdks/utils.py` & `carefree-creator-0.2.5/cfcreator/sdks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/txt2img.py` & `carefree-creator-0.2.5/cfcreator/txt2img.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .utils import APIs
 from .common import register_sd
 from .common import register_sd_inpainting
 from .common import get_sd_from
 from .common import handle_diffusion_model
 from .common import get_bytes_from_diffusion
 from .common import get_normalized_arr_from_diffusion
+from .common import handle_diffusion_inpainting_model
 from .common import IAlgorithm
 from .common import HighresModel
 from .common import Txt2ImgModel
 from .common import ReturnArraysModel
 from .common import CommonSDInpaintingModel
 
 
@@ -130,15 +131,15 @@
             m = get_sd_from(data)
         else:
             api_key = APIs.SD_INPAINTING
             m = api_pool.get(api_key)
             m.disable_control()
         t2 = time.time()
         kwargs.update(handle_diffusion_model(m, data))
-        kwargs.update(await self.handle_diffusion_inpainting_model(data))
+        kwargs.update(handle_diffusion_inpainting_model(data))
         mask_arr = np.array(mask)
         mask_arr[..., -1] = np.where(mask_arr[..., -1] > 0, 255, 0)
         mask = Image.fromarray(mask_arr)
         img_arr = m.txt2img_inpainting(
             data.text,
             image,
             mask,
@@ -185,15 +186,15 @@
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         t1 = time.time()
         m = api_pool.get(APIs.SD_INPAINTING)
         m.disable_control()
         t2 = time.time()
         kwargs.update(handle_diffusion_model(m, data))
-        kwargs.update(await self.handle_diffusion_inpainting_model(data))
+        kwargs.update(handle_diffusion_inpainting_model(data))
         img_arr = m.outpainting(
             data.text,
             image,
             anchor=64,
             max_wh=data.max_wh,
             keep_original=data.keep_original,
             **kwargs,
```

### Comparing `carefree-creator-0.2.4/cfcreator/txt2txt.py` & `carefree-creator-0.2.5/cfcreator/txt2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.4/cfcreator/utils.py` & `carefree-creator-0.2.5/cfcreator/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import cv2
 import math
 import torch
 
 import numpy as np
 
+from PIL import Image
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Protocol
+from cftool.cv import to_rgb
 from cflearn.api.utils import ILoadableItem
 from cflearn.api.utils import ILoadablePool
 
 from .parameters import lazy_load
 from .parameters import pool_limit
 from .parameters import OPT
 
@@ -57,14 +59,38 @@
         iy = i // num_col
         ix = ix * w + ix * padding
         iy = iy * h + iy * padding
         canvas[iy : iy + h, ix : ix + w] = out
     return canvas
 
 
+def get_contrast_bg(rgba_image: Image.Image) -> int:
+    rgba = np.array(rgba_image)
+    rgb = rgba[..., :3]
+    alpha = rgba[..., -1]
+    target_mask = alpha >= 10
+    hls = cv2.cvtColor(rgb, cv2.COLOR_RGB2HLS)
+    lightness = hls[..., 1].astype(np.float32) / 255.0
+    target_lightness = lightness[target_mask]
+    mean = target_lightness.mean().item()
+    std = target_lightness.std().item()
+    if 0.45 <= mean <= 0.55 and std >= 0.25:
+        return 127
+    if mean <= 0.2 or 0.8 <= mean:
+        return 127
+    return 0 if mean >= 0.5 else 255
+
+
+def to_contrast_rgb(image: Image.Image) -> Image.Image:
+    if not image.mode == "RGBA":
+        return to_rgb(image)
+    bg = get_contrast_bg(image)
+    return to_rgb(image, (bg, bg, bg))
+
+
 class APIs(str, Enum):
     SD = "sd"
     SD_INPAINTING = "sd_inpainting"
     ESR = "esr"
     ESR_ANIME = "esr_anime"
     INPAINTING = "inpainting"
     LAMA = "lama"
```

### Comparing `carefree-creator-0.2.4/setup.py` & `carefree-creator-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.4"
+VERSION = "0.2.5"
 PACKAGE_NAME = "carefree-creator"
 
 DESCRIPTION = "An AI-powered creator for everyone."
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
@@ -12,16 +12,16 @@
     version=VERSION,
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     entry_points={"console_scripts": ["cfcreator = cfcreator.cli:main"]},
     install_requires=[
         "click>=8.1.3",
         "fastapi>=0.95.1",
-        "carefree-client>=0.1.9",
-        "carefree-learn[cv_full]>=0.4.3",
+        "carefree-client>=0.1.10",
+        "carefree-learn[cv_full]>=0.4.4",
     ],
     extras_require={
         "kafka": [
             "kafka-python",
             "redis[hiredis]",
             "cos-python-sdk-v5",
         ]
```

