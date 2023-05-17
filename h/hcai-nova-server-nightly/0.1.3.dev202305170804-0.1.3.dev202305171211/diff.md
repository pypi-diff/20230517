# Comparing `tmp/hcai-nova-server-nightly-0.1.3.dev202305170804.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.3.dev202305171211.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.3.dev202305170804.tar", last modified: Wed May 17 08:04:45 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.3.dev202305171211.tar", last modified: Wed May 17 12:11:41 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804.tar` & `hcai-nova-server-nightly-0.1.3.dev202305171211.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:45.856681 hcai-nova-server-nightly-0.1.3.dev202305170804/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-17 08:04:45.856681 hcai-nova-server-nightly-0.1.3.dev202305170804/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:45.852681 hcai-nova-server-nightly-0.1.3.dev202305170804/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-17 08:04:45.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-17 08:04:45.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 08:04:45.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-17 08:04:45.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 08:04:45.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:45.852681 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/nova_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:45.856681 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9430 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7744 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:45.856681 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:45.856681 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11559 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 08:04:45.856681 hcai-nova-server-nightly-0.1.3.dev202305170804/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-17 08:04:37.000000 hcai-nova-server-nightly-0.1.3.dev202305170804/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:41.888597 hcai-nova-server-nightly-0.1.3.dev202305171211/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-17 12:11:41.888597 hcai-nova-server-nightly-0.1.3.dev202305171211/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:41.888597 hcai-nova-server-nightly-0.1.3.dev202305171211/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-05-17 12:11:41.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-05-17 12:11:41.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:11:41.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-17 12:11:41.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 12:11:41.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:41.888597 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/nova_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:41.888597 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7744 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:41.888597 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:41.888597 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12151 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 12:11:41.888597 hcai-nova-server-nightly-0.1.3.dev202305171211/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-17 12:11:33.000000 hcai-nova-server-nightly-0.1.3.dev202305171211/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/PKG-INFO` & `hcai-nova-server-nightly-0.1.3.dev202305171211/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.3.dev202305170804
+Version: 0.1.3.dev202305171211
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/README.md` & `hcai-nova-server-nightly-0.1.3.dev202305171211/README.md`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.3.dev202305171211/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.3.dev202305170804
+Version: 0.1.3.dev202305171211
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.3.dev202305171211/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/nova_backend.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/nova_backend.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/extract.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from nova_utils.ssi_utils.ssi_xml_utils import Chain, ChainLink
 from nova_utils.ssi_utils.ssi_stream_utils import Stream, Chunk, FileTypes, NPDataTypes
 from importlib.machinery import SourceFileLoader
 from hcai_datasets.hcai_nova_dynamic.hcai_nova_dynamic_iterable import (
     HcaiNovaDynamicIterable,
 )
 from soundfile import write
+import ffmpegio
+import numpy as np
 from nova_server.utils import db_utils
 
 
 extract = Blueprint("extract", __name__)
 
 
 @extract.route("/extract", methods=["POST"])
@@ -178,25 +180,27 @@
                 else:
                     logger.info("Write...")
 
                     for stream_id, (data_type, sr, data) in stream_dict.items():
 
                         suffix = request_form.get("suffix", "")
                         stream_id_sfx = stream_id + "_" + suffix if suffix else stream_id
+                        file_name_db = '.'.join(stream_id_sfx.split('.')[1:])
                         out_path = (
                             Path(ds_iter.nova_data_dir)
                             / ds_iter.dataset
                             / ds_iter.sessions[0]
                             / stream_id_sfx
                         )
 
                         logger.info(f"\t - {out_path}")
 
                         # SSI-Stream
                         if data_type == DataTypes.FEATURE:
+                            file_ex = '.stream'
                             ftype = FileTypes.BINARY
                             sr = sr
                             dim = data.shape[-1] if len(data.shape) > 1 else 1
                             dtype = NPDataTypes(type(data.dtype).type)
                             chunks = [
                                 Chunk(f=0, t=data.shape[0] / sr, b=0, n=data.shape[0])
                             ]
@@ -205,40 +209,42 @@
                                 sr=sr,
                                 dim=dim,
                                 byte=data.dtype.itemsize,
                                 dtype=dtype,
                                 data=data,
                                 chunks=chunks,
                             )
-
                             ssi_stream.save(out_path)
-                            # TODO: Add dimlabels from stream
-                            db_utils.write_stream_info_to_db(
-                                request_form = request_form,
-                                file_name = stream_id_sfx,
-                                file_ext = '.stream',
-                                stream_type = 'feature',
-                                is_valid = True,
-                                sr = sr,
-                                dimlables = []
-                            )
 
-                        # Audio Data
+                            # Audio Data
                         elif data_type == DataTypes.AUDIO:
-                            out_path = out_path.parent / (out_path.name + ".wav")
-                            write(file=out_path, data=data, samplerate=sr)
+                            file_ex = '.wav'
+                            out_path = out_path.parent / (out_path.name + file_ex)
+                            ffmpegio.audio.write(out_path, int(sr), np.swapaxes(np.hstack(data),0 , -1), overwrite=True)
 
                         # Video Data
                         elif data_type == DataTypes.VIDEO:
-                            raise NotImplementedError()
+                            file_ex = '.mp4'
+                            out_path = out_path.parent / (out_path.name + file_ex)
+                            ffmpegio.video.write(out_path, int(sr), np.vstack(data), overwrite=True)
                         else:
                             raise NotImplementedError(f"{data_type} is not supported.")
 
 
-
+                        # Add Stream info to Databases
+                        # TODO: Add dimlabels from stream
+                        db_utils.write_stream_info_to_db(
+                             request_form = request_form,
+                             file_name = file_name_db,
+                             file_ext = file_ex,
+                             stream_type = data_type.name.lower(),
+                             is_valid = True,
+                             sr = sr,
+                             dimlables = []
+                         )
 
                     logger.info("...done")
 
         logger.info("Extraction completed!")
         status_utils.update_status(key, status_utils.JobStatus.FINISHED)
 
         logger.info("Action 'Extract' finished.")
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/db_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,201 +15,223 @@
 roles = None
 
 
 # Format of results must be: {values: [value1, value2, value3, ...], confidences: [conf1, conf2, conf3, ...], start_frame: x, ...}
 def check_format(variable, logger):
     text = ""
     if type(variable) is not dict:
-        text = 'Result type must be a dictionary!'
+        text = "Result type must be a dictionary!"
     if "values" not in variable or "confidences" not in variable:
         text = 'Result type must contain "values" and "confidences" as keys.'
     if not type(variable["values"]) is list or not type(variable["confidences"]):
-        text = 'Results["values"] and Results["confidences"] must respectively be a list.'
+        text = (
+            'Results["values"] and Results["confidences"] must respectively be a list.'
+        )
 
     if text != "":
         logger.info(text)
         raise Exception(text)
 
 
-def write_stream_info_to_db(request_form: dict, file_name: str, file_ext: str, stream_type: str, is_valid: bool, sr: float, dimlables: list = None):
+def write_stream_info_to_db(
+    request_form: dict,
+    file_name: str,
+    file_ext: str,
+    stream_type: str,
+    is_valid: bool,
+    sr: float,
+    dimlables: list = None,
+):
     # TODO check if we really need to establish a new connection to the database
     db_config_dict = {
-        'ip': request_form["server"].split(':')[0],
-        'port': int(request_form["server"].split(':')[1]),
-        'user': request_form["username"],
-        'password': request_form["password"]
+        "ip": request_form["server"].split(":")[0],
+        "port": int(request_form["server"].split(":")[1]),
+        "user": request_form["username"],
+        "password": request_form["password"],
     }
 
     db_handler = NovaDBHandler(db_config_dict=db_config_dict)
-    database = request_form['database']
+    database = request_form["database"]
 
     db_handler.set_data_streams(
-        database= database,
-        file_name= file_name,
-        file_ext= file_ext,
-        stream_type= stream_type,
-        is_valid= is_valid,
-        sr= sr,
-        dimlabels= dimlables
+        database=database,
+        file_name=file_name,
+        file_ext=file_ext,
+        stream_type=stream_type,
+        is_valid=is_valid,
+        sr=sr,
+        dimlabels=dimlables,
+        overwrite=True,
     )
 
 
-
-
 def write_annotation_to_db(request_form, results: dict, logger):
     global database, scheme, session, annotator, roles
     check_format(results, logger)
 
     # TODO check if we really need to establish a new connection to the database
     db_config_dict = {
-        'ip': request_form["server"].split(':')[0],
-        'port': int(request_form["server"].split(':')[1]),
-        'user': request_form["username"],
-        'password': request_form["password"]
+        "ip": request_form["server"].split(":")[0],
+        "port": int(request_form["server"].split(":")[1]),
+        "user": request_form["username"],
+        "password": request_form["password"],
     }
 
     db_handler = NovaDBHandler(db_config_dict=db_config_dict)
-    database = request_form['database']
-    scheme = request_form['scheme']
-    session = request_form['sessions']
-    annotator = request_form['annotator']
-    roles = request_form['roles']
+    database = request_form["database"]
+    scheme = request_form["scheme"]
+    session = request_form["sessions"]
+    annotator = request_form["annotator"]
+    roles = request_form["roles"]
 
     if request_form["schemeType"] == "DISCRETE":
         write_discrete_to_db(request_form, results, db_handler, logger)
     elif request_form["schemeType"] == "FREE":
         write_freeform_to_db(request_form, results, db_handler, logger)
     elif request_form["schemeType"] == "CONTINUOUS":
         write_continuous_to_db(request_form, results, db_handler, logger)
     elif request_form["schemeType"] == "POINT":
         pass  # todo
-    elif request_form["schemeType"] == "DISCRETE_POLYGON" or request_form["schemeType"] == "POLYGON":
+    elif (
+        request_form["schemeType"] == "DISCRETE_POLYGON"
+        or request_form["schemeType"] == "POLYGON"
+    ):
         write_polygons_to_db(request_form, results, db_handler, logger)
 
 
 def write_freeform_to_db(request_form, results: dict, db_handler, logger):
-    '''
+    """
     Args:
         request_form ():
         results (dict): {
             'from_to' : {
                 <role>.<stream>: {
                     'name': <text>, 'conf': <confidence>
                 }
             }
         }
         db_handler ():
         logger ():
 
     Returns:
 
-    '''
+    """
     annotations = {}
     """Temp fix"""
-    results.pop('values', None)
-    results.pop('confidences', None)
+    results.pop("values", None)
+    results.pop("confidences", None)
 
     for frame, results in results.items():
-        frame_info = frame.split('_')
+        frame_info = frame.split("_")
         frame_from = float(frame_info[-2])
         frame_to = float(frame_info[-1])
         for stream_id, anno in results.items():
 
-            conf = anno['conf']
-            name = anno['name']
+            conf = anno["conf"]
+            name = anno["name"]
 
             if stream_id not in annotations.keys():
                 annotations[stream_id] = []
 
-            annotations[stream_id].append({
-                "from": frame_from,
-                "to": frame_to,
-                "conf": conf,
-                "name": name
-            })
+            annotations[stream_id].append(
+                {"from": frame_from, "to": frame_to, "conf": conf, "name": name}
+            )
 
     for anno_id, anno in annotations.items():
         # TODO does not work with flattened roles
-        role, stream = anno_id.split('.')
+        role, stream = anno_id.split(".")
 
         db_handler.set_annos(
             database=database,
             scheme=scheme,
             session=session,
             annotator=annotator,
             role=role,
             annos=anno,
         )
 
 
 def write_discrete_to_db(request_form, results: dict, db_handler, logger):
     # TODO: We only take one role into account in this case. Fix
-    #role = roles.split(';')[0]
-    role = results['roles']
-    frame_size = nova_data_utils.parse_time_string_to_ms(request_form['frameSize'])
+    # role = roles.split(';')[0]
+    role = results["roles"]
+    frame_size = nova_data_utils.parse_time_string_to_ms(request_form["frameSize"])
     mongo_scheme = db_handler.get_mongo_scheme(scheme, database)
     annos = []
     start_frame = 0
 
-    if request_form['startTime'] != '0':
-        annos_db = db_handler.get_annos(dataset=database, scheme=scheme, session=session, annotator=annotator,
-                                        roles=role)
+    if request_form["startTime"] != "0":
+        annos_db = db_handler.get_annos(
+            dataset=database,
+            scheme=scheme,
+            session=session,
+            annotator=annotator,
+            roles=role,
+        )
 
-        start_frame = float(request_form['startTime']) / 1000
-        annos = list(filter(lambda x: float(x['from']) < start_frame, annos_db))
+        start_frame = float(request_form["startTime"]) / 1000
+        annos = list(filter(lambda x: float(x["from"]) < start_frame, annos_db))
 
     last_label = None
     current_label_start = 1
 
     values = results["values"]
 
     for id, value in enumerate(values):
         # current label is different from the one before
         if not value == last_label and last_label is not None:
-            frame_from = str(start_frame + ((current_label_start * frame_size) / 1000.0))
+            frame_from = str(
+                start_frame + ((current_label_start * frame_size) / 1000.0)
+            )
             frame_to = str(start_frame + ((id * frame_size) / 1000.0))
-            if last_label < len(mongo_scheme[0]['labels']):
-                annos.append({
-                    'from': frame_from,
-                    'to': frame_to,
-                    'conf': results["confidences"][id],
-                    'id': int(last_label)
-                })
+            if last_label < len(mongo_scheme[0]["labels"]):
+                annos.append(
+                    {
+                        "from": frame_from,
+                        "to": frame_to,
+                        "conf": results["confidences"][id],
+                        "id": int(last_label),
+                    }
+                )
             current_label_start = id
         last_label = value
 
     db_handler.set_annos(
         database=database,
         scheme=scheme,
         session=session,
         annotator=annotator,
         role=role,
         annos=annos,
     )
 
 
 def write_continuous_to_db(request_form, results: dict, db_handler, logger):
-    role = results['roles']
-    #role = roles.split(';')[0]
+    role = results["roles"]
+    # role = roles.split(';')[0]
     annos = []
 
-    if request_form['startTime'] != '0':
-        annos_db = db_handler.get_annos(dataset=database, scheme=scheme, session=session, annotator=annotator,
-                                        roles=roles)
+    if request_form["startTime"] != "0":
+        annos_db = db_handler.get_annos(
+            dataset=database,
+            scheme=scheme,
+            session=session,
+            annotator=annotator,
+            roles=roles,
+        )
 
-        start_frame = int(int(request_form['startTime']) / int(request_form['frameSize'][:-2]) + 1)
+        start_frame = int(
+            int(request_form["startTime"]) / int(request_form["frameSize"][:-2]) + 1
+        )
         annos = annos_db[:start_frame]
 
-    #normalized = (results["values"] - min(results["values"])) / (max(results["values"]) - min(results["values"]))
+    # normalized = (results["values"] - min(results["values"])) / (max(results["values"]) - min(results["values"]))
 
     for value, confidence in zip(results["values"], results["confidences"]):
-        annos.append({
-            'score': value,
-            'conf': confidence
-        })
+        annos.append({"score": value, "conf": confidence})
 
     db_handler.set_annos(
         database=database,
         scheme=scheme,
         session=session,
         annotator=annotator,
         role=role,
@@ -234,57 +256,69 @@
 
     start_frame = int(float(results["start_frame"])) - 1
 
     mongo_data_id = None
     data_backup_id = None
     if mongo_annotations:
         if mongo_annotations[0]["isLocked"]:
-            warnings.warn(f"Can't overwrite locked annotation {str(mongo_annotations[0]['_id'])}")
+            warnings.warn(
+                f"Can't overwrite locked annotation {str(mongo_annotations[0]['_id'])}"
+            )
             return ""
         else:
             mongo_data_id = mongo_annotations[0]["data_id"]
             data_backup_id = mongo_annotations[0]["data_backup_id"]
     logger.info("...fetch documents...")
     # 1. Get the doc (will get merged if other docs are there are nextEntry ID's)
     main_docs = db_handler.get_data_docs_by_prop(mongo_data_id, "_id", database)
-    backup_doc = db_handler.get_docs_by_prop(mongo_data_id, "_id", database, db_handler.ANNOTATION_DATA_COLLECTION)[0]
+    backup_doc = db_handler.get_docs_by_prop(
+        mongo_data_id, "_id", database, db_handler.ANNOTATION_DATA_COLLECTION
+    )[0]
     logger.info("...fill documents...")
     # 2. Fill the doc with the Predictions
-    main_docs = update_polygon_doc(main_docs, results["values"], results["confidences"], start_frame)
+    main_docs = update_polygon_doc(
+        main_docs, results["values"], results["confidences"], start_frame
+    )
 
     # 3. Check if the doc is too large (if, separate it)
     if len(bson.BSON.encode(main_docs)) >= MAX_MONGO_DB_DOC_SIZE:
         main_docs = separate_doc(main_docs)
     if not isinstance(main_docs, list):
         main_docs = [main_docs]
-    main_docs[0]['_id'] = mongo_data_id
+    main_docs[0]["_id"] = mongo_data_id
 
     logger.info("...separate docs if necessary...")
     # 4 Delete old back-up (with tail-docs)
     db_handler.delete_doc_with_tail(data_backup_id, database)
 
     logger.info("...upload docs...")
     # 5. Update the backup ID
-    backup_doc['_id'] = data_backup_id
-    db_handler.insert_doc_by_prop(backup_doc, database, db_handler.ANNOTATION_DATA_COLLECTION)
-    db_handler.delete_doc_by_prop(mongo_data_id, "_id", database, db_handler.ANNOTATION_DATA_COLLECTION)
+    backup_doc["_id"] = data_backup_id
+    db_handler.insert_doc_by_prop(
+        backup_doc, database, db_handler.ANNOTATION_DATA_COLLECTION
+    )
+    db_handler.delete_doc_by_prop(
+        mongo_data_id, "_id", database, db_handler.ANNOTATION_DATA_COLLECTION
+    )
 
     # 6. Upload the doc(s)
     for doc in main_docs:
-        db_handler.insert_doc_by_prop(doc, database, db_handler.ANNOTATION_DATA_COLLECTION)
+        db_handler.insert_doc_by_prop(
+            doc, database, db_handler.ANNOTATION_DATA_COLLECTION
+        )
 
 
 def separate_doc(doc) -> list:
     left = copy.deepcopy(doc)
     left["_id"] = bson.objectid.ObjectId()
     right = copy.deepcopy(doc)
     right["_id"] = bson.objectid.ObjectId()
-    half_count = int(len(doc['labels']) / 2)
-    left['labels'] = left['labels'][0:half_count]
-    right['labels'] = right['labels'][half_count:]
+    half_count = int(len(doc["labels"]) / 2)
+    left["labels"] = left["labels"][0:half_count]
+    right["labels"] = right["labels"][half_count:]
 
     result_list = []
     if len(bson.BSON.encode(left)) >= MAX_MONGO_DB_DOC_SIZE:
         result_list += separate_doc(left)
     else:
         result_list.append(left)
 
@@ -294,31 +328,41 @@
         result_list.append(right)
 
     return result_list
 
 
 def update_polygon_doc(data_doc, polygons, confidences, start_frame):
     current_frame = -1
-    for frame_id, frame in enumerate(data_doc['labels']):
+    for frame_id, frame in enumerate(data_doc["labels"]):
         if frame_id >= start_frame + len(polygons):
             return data_doc
         if frame_id >= start_frame:
             polygons_per_frame = polygons[frame_id - start_frame]
             for label_id, polygons_per_label_type in enumerate(polygons_per_frame):
                 for polygon_id, polygon in enumerate(polygons_per_label_type):
                     label = label_id + 1
                     points_for_db = []
-                    points = np.reshape(polygon, newshape=[int(polygon.shape[0] / 2), 2])
+                    points = np.reshape(
+                        polygon, newshape=[int(polygon.shape[0] / 2), 2]
+                    )
                     for point in points:
-                        points_for_db.append({'x': int(point[0]), 'y': int(point[1])})
+                        points_for_db.append({"x": int(point[0]), "y": int(point[1])})
 
                     # delete the content of the current frame, the new prediction values have to be set
                     if current_frame != frame_id:
                         current_frame = frame_id
-                        data_doc['labels'][frame_id]['polygons'] = []
+                        data_doc["labels"][frame_id]["polygons"] = []
 
-                    data_doc['labels'][frame_id]['polygons'].append(
-                        {'label': label,
-                         'confidence': round(confidences[frame_id - start_frame][label_id][polygon_id], 2),
-                         'points': points_for_db})
+                    data_doc["labels"][frame_id]["polygons"].append(
+                        {
+                            "label": label,
+                            "confidence": round(
+                                confidences[frame_id - start_frame][label_id][
+                                    polygon_id
+                                ],
+                                2,
+                            ),
+                            "points": points_for_db,
+                        }
+                    )
 
     return data_doc
```

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.3.dev202305170804/setup.py` & `hcai-nova-server-nightly-0.1.3.dev202305171211/setup.py`

 * *Files identical despite different names*

