# Comparing `tmp/t4flib-0.2.0-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10736 bytes, number of entries: 12
+Zip file size: 10739 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      891 b- defN 23-May-17 15:14 t4flib/config.py
--rw-rw-r--  2.0 unx      970 b- defN 23-May-17 15:14 t4flib/data_helper.py
--rw-rw-r--  2.0 unx     6144 b- defN 23-May-17 15:14 t4flib/file_helper.py
--rw-rw-r--  2.0 unx     4498 b- defN 23-May-17 15:14 t4flib/filetransfer_helper.py
--rw-rw-r--  2.0 unx     7417 b- defN 23-May-17 15:14 t4flib/functional_helper.py
--rw-rw-r--  2.0 unx     3233 b- defN 23-May-17 15:14 t4flib/gcloud_helper.py
+-rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
+-rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
+-rw-rw-r--  2.0 unx     4501 b- defN 23-May-17 15:49 t4flib/filetransfer_helper.py
+-rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
+-rw-rw-r--  2.0 unx     3235 b- defN 23-May-17 15:49 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-17 15:14 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-17 15:27 t4flib-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-17 15:27 t4flib-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-17 15:27 t4flib-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 23-May-17 15:27 t4flib-0.2.0.dist-info/RECORD
-12 files, 26812 bytes uncompressed, 9204 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-17 17:14 t4flib-0.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-17 17:14 t4flib-0.2.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-17 17:14 t4flib-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 23-May-17 17:14 t4flib-0.2.1.dist-info/RECORD
+12 files, 26822 bytes uncompressed, 9207 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.2.0.dist-info/METADATA
+Filename: t4flib-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.2.0.dist-info/WHEEL
+Filename: t4flib-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.2.0.dist-info/top_level.txt
+Filename: t4flib-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.2.0.dist-info/RECORD
+Filename: t4flib-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/data_helper.py

```diff
@@ -1,8 +1,8 @@
-from log_helper import logger
+from .log_helper import logger
 
 import datetime
 
 def get_safety_positional_data(line : str, arr_index : list):
     try:
         if len(arr_index) == 2:
             index_start=arr_index[0]
```

## t4flib/file_helper.py

```diff
@@ -1,9 +1,9 @@
 import os
-from log_helper import logger
+from .log_helper import logger
 import shutil
 import fnmatch
 import datetime
 import pathlib
 import json
 import zipfile
 import glob
```

## t4flib/filetransfer_helper.py

```diff
@@ -1,16 +1,16 @@
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 import json
 import csv
 import os
-from config import FT_PARAM_FILEPATH, FT_GRAVITEE_KEY, FT_GRAVITEE_URL
-from log_helper import logger
-from file_helper import get_all_file_by_filemask
+from .config import FT_PARAM_FILEPATH, FT_GRAVITEE_KEY, FT_GRAVITEE_URL
+from .log_helper import logger
+from .file_helper import get_all_file_by_filemask
 import shutil
 import time
 import urllib3
 
 
 class ft_flow:
     flow_name = ''
```

## t4flib/functional_helper.py

```diff
@@ -1,10 +1,10 @@
-from log_helper import logger
-from file_helper import get_all_file_by_filemask
-from data_helper import verify_date_format, get_safety_positional_data
+from .log_helper import logger
+from .file_helper import get_all_file_by_filemask
+from .data_helper import verify_date_format, get_safety_positional_data
 import os
 import csv 
 from datetime import datetime
 
 
 __SCHEMA_HEADER_AP__= [[0,1 ],[1,11],[11,61],[61,76],[76,86],[86,106],[106,110],[110,210],[210,235],[235,265],[265,285],[285,315],[315,325],[325,345],[345,355],[355,405],[405,415],[415,425],[425,435],[435,460],[460,464],[464,494],[494,504],[504,514],[514,534],[534,544],[544,594],[594,609],[609,629],[629,639],[639,640],[640,660],[660,690],[690,720],[720,750],[750,780],[780,810],[810,840],[840,870],[870,900],[900,930],[930,960],[960,990],[990,1020],[1020,1050],[1050,1080],[1080,1110],[1110,1140],[1140,1170],[1170,1200],[1200,1230],[1230,1260],[1260,1290],[1290,1320],[1320,1350],[1350,1380],[1380,1410],[1410,1440],[1440,1480]]
 __SCHEMA_BODY_AP__ = [[0,1],[1,11],[11,61],[61,76],[76,91],[91,116],[116,136],[136,137],[137,147],[147,247],[247,262],[262,263],[263,264],[264,289],[289,339],[339,399],[399,424],[424,449],[449,474],[474,494],[494,514],[514,534],[534,554],[554,574],[574,594],[594,834],[834,854],[854,874],[874,894],[894,914],[914,915],[915,945],[945,970],[970,995],[995,102],[1020,1040],[1040,1041],[1041,1056],[1056,1057],[1057,1058],[1058,1088],[1088,1118],[1118,1148],[1148,1178],[1178,1208],[1208,1238],[1238,1268],[1268,1298],[1298,1328],[1328,1358],[1358,1388],[1388,1418],[1418,1448],[1448,1478],[1478,1508],[1508,1538],[1538,1568],[1568,1598],[1598,1628],[1628,1658],[1658,1688],[1688,1718],[1718,1748],[1748,1778],[1778,1808],[1808,1838],[1838,1868],[1868,1898],[1898,1928],[1928,1958],[1958,1988],[1988,2018],[2018,2048],[2048,2078],[2078,2108],[2108,2138],[2138,2175]]
```

## t4flib/gcloud_helper.py

```diff
@@ -1,16 +1,16 @@
 import shutil
 
 from google.cloud import bigquery
 from google.oauth2 import service_account
 from google.cloud import storage
 from google.api_core import exceptions as gcloud_ex
 import pandas as pd
-from log_helper import logger
-from config import GCP_ACCOUNT_SERVICE_FILE, ENVIRONEMENT, PROXY_AUCHAN, BQ_PROJECT_ID
+from .log_helper import logger
+from .config import GCP_ACCOUNT_SERVICE_FILE, ENVIRONEMENT, PROXY_AUCHAN, BQ_PROJECT_ID
 import os
 
 
 def run_bq_query(query):
     ENVIRONEMENT='dev'
     credentials = service_account.Credentials.from_service_account_file(GCP_ACCOUNT_SERVICE_FILE)
     if ENVIRONEMENT == 'dev':
```

## Comparing `t4flib-0.2.0.dist-info/METADATA` & `t4flib-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

