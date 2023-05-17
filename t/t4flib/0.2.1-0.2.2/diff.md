# Comparing `tmp/t4flib-0.2.1-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.2.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10739 bytes, number of entries: 12
+Zip file size: 10746 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
--rw-rw-r--  2.0 unx      891 b- defN 23-May-17 15:14 t4flib/config.py
+-rw-rw-r--  2.0 unx      892 b- defN 23-May-17 17:25 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
 -rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
 -rw-rw-r--  2.0 unx     4501 b- defN 23-May-17 15:49 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
 -rw-rw-r--  2.0 unx     3235 b- defN 23-May-17 15:49 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-17 15:14 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-17 17:14 t4flib-0.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-17 17:14 t4flib-0.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-17 17:14 t4flib-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 23-May-17 17:14 t4flib-0.2.1.dist-info/RECORD
-12 files, 26822 bytes uncompressed, 9207 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-17 17:38 t4flib-0.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-17 17:38 t4flib-0.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-17 17:38 t4flib-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 23-May-17 17:38 t4flib-0.2.2.dist-info/RECORD
+12 files, 26823 bytes uncompressed, 9214 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.2.1.dist-info/METADATA
+Filename: t4flib-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.2.1.dist-info/WHEEL
+Filename: t4flib-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.2.1.dist-info/top_level.txt
+Filename: t4flib-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.2.1.dist-info/RECORD
+Filename: t4flib-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/config.py

```diff
@@ -1,10 +1,10 @@
 import os
 from dotenv import load_dotenv
-from log_helper import logger
+from .log_helper import logger
 
 __envDir__ = os.path.abspath(os.path.join(os.path.abspath(os.path.join(__file__, os.pardir)), os.pardir))
 env = os.environ.get("MTM_ENV", "dev")
 __env_file__ = os.path.join(__envDir__, f".env.{env}")
 
 logger('DEBUG', f'Envrionnement = {env}')
 logger('DEBUG', f'Path environnement file : {__env_file__}')
```

## Comparing `t4flib-0.2.1.dist-info/METADATA` & `t4flib-0.2.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.2.1
+Version: 0.2.2
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.2.1.dist-info/RECORD` & `t4flib-0.2.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-t4flib/config.py,sha256=guQaLgqXO1fQH9PKMcllYd52LwdAwY6uFghGG1kHjuA,891
+t4flib/config.py,sha256=fHt2THXtajPzzV_gnHPZNVmez09ODLfIFrt4cTXgZsE,892
 t4flib/data_helper.py,sha256=SdKdv2U1EXtHJcfEff_I8zIlMWv56-xLZqczAw4kOUU,971
 t4flib/file_helper.py,sha256=NYIgOrA1iJBUcodtaRlDIsIHoivonLme4PmFZB1nQLw,6145
 t4flib/filetransfer_helper.py,sha256=GPDEUa0f-QmTH025pylJOAp0wyZtbhVzMWSjhM8KHxU,4501
 t4flib/functional_helper.py,sha256=CfbwrMufVRwCQNg9us9tujS3oeCmxql18vmo7B5lUAI,7420
 t4flib/gcloud_helper.py,sha256=sy5EpA2iVlcNlveP77N3iUCERNZXabSVOOcz8rifO6I,3235
 t4flib/log_helper.py,sha256=pu_y3m7iHWpkgYnxLYAlQjWjqknMGDcCDjHV6w4YYDc,876
-t4flib-0.2.1.dist-info/METADATA,sha256=_A5BQExizQyELHAilC3vAoXQy2OCWuWB-6yLIc6WgNA,1747
-t4flib-0.2.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.2.1.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.2.1.dist-info/RECORD,,
+t4flib-0.2.2.dist-info/METADATA,sha256=xDVGU3I3DmlAPEnGRsKhkjsLgj9bxIbBMWGdKuJKqtM,1747
+t4flib-0.2.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.2.2.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.2.2.dist-info/RECORD,,
```

