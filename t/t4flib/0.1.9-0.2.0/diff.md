# Comparing `tmp/t4flib-0.1.9-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 7974 bytes, number of entries: 10
+Zip file size: 10736 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
--rw-rw-r--  2.0 unx      892 b- defN 23-May-11 18:20 t4flib/config.py
--rw-rw-r--  2.0 unx     6145 b- defN 23-May-16 10:28 t4flib/file_helper.py
--rw-rw-r--  2.0 unx     4508 b- defN 23-May-11 18:20 t4flib/filetransfer_helper.py
--rw-rw-r--  2.0 unx     3259 b- defN 23-May-11 18:20 t4flib/gcloud_helper.py
--rw-rw-r--  2.0 unx      753 b- defN 23-May-11 18:20 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-16 10:36 t4flib-0.1.9.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-16 10:36 t4flib-0.1.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-16 10:36 t4flib-0.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      758 b- defN 23-May-16 10:36 t4flib-0.1.9.dist-info/RECORD
-10 files, 18179 bytes uncompressed, 6690 bytes compressed:  63.2%
+-rw-rw-r--  2.0 unx      891 b- defN 23-May-17 15:14 t4flib/config.py
+-rw-rw-r--  2.0 unx      970 b- defN 23-May-17 15:14 t4flib/data_helper.py
+-rw-rw-r--  2.0 unx     6144 b- defN 23-May-17 15:14 t4flib/file_helper.py
+-rw-rw-r--  2.0 unx     4498 b- defN 23-May-17 15:14 t4flib/filetransfer_helper.py
+-rw-rw-r--  2.0 unx     7417 b- defN 23-May-17 15:14 t4flib/functional_helper.py
+-rw-rw-r--  2.0 unx     3233 b- defN 23-May-17 15:14 t4flib/gcloud_helper.py
+-rw-rw-r--  2.0 unx      876 b- defN 23-May-17 15:14 t4flib/log_helper.py
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-17 15:27 t4flib-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-17 15:27 t4flib-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-17 15:27 t4flib-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 23-May-17 15:27 t4flib-0.2.0.dist-info/RECORD
+12 files, 26812 bytes uncompressed, 9204 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,31 +1,37 @@
 Filename: t4flib/__init__.py
 Comment: 
 
 Filename: t4flib/config.py
 Comment: 
 
+Filename: t4flib/data_helper.py
+Comment: 
+
 Filename: t4flib/file_helper.py
 Comment: 
 
 Filename: t4flib/filetransfer_helper.py
 Comment: 
 
+Filename: t4flib/functional_helper.py
+Comment: 
+
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.1.9.dist-info/METADATA
+Filename: t4flib-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.1.9.dist-info/WHEEL
+Filename: t4flib-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.1.9.dist-info/top_level.txt
+Filename: t4flib-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.1.9.dist-info/RECORD
+Filename: t4flib-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/config.py

```diff
@@ -1,10 +1,10 @@
 import os
 from dotenv import load_dotenv
-from .log_helper import logger
+from log_helper import logger
 
 __envDir__ = os.path.abspath(os.path.join(os.path.abspath(os.path.join(__file__, os.pardir)), os.pardir))
 env = os.environ.get("MTM_ENV", "dev")
 __env_file__ = os.path.join(__envDir__, f".env.{env}")
 
 logger('DEBUG', f'Envrionnement = {env}')
 logger('DEBUG', f'Path environnement file : {__env_file__}')
```

## t4flib/file_helper.py

```diff
@@ -1,9 +1,9 @@
 import os
-from .log_helper import logger
+from log_helper import logger
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
-from t4flib.config import FT_PARAM_FILEPATH, FT_GRAVITEE_KEY, FT_GRAVITEE_URL
-from t4flib.log_helper import logger
-from t4flib.file_helper import get_all_file_by_filemask
+from config import FT_PARAM_FILEPATH, FT_GRAVITEE_KEY, FT_GRAVITEE_URL
+from log_helper import logger
+from file_helper import get_all_file_by_filemask
 import shutil
 import time
 import urllib3
 
 
 class ft_flow:
     flow_name = ''
@@ -99,15 +99,15 @@
 
             shutil.copy(str(file.absolute()), ft_flow_to_send.path_out)
 
             body_request = json.dumps({
                 "flow": ft_flow_to_send.flow_name,
                 "userId": ft_flow_to_send.server,
                 "authKey": ft_flow_to_send.ft_key,
-                "uri": str(file)
+                "uri": str(file.absolute())
             })
 
             try:
                 response = requests.post(FT_GRAVITEE_URL, headers=headers, data=body_request, verify=False)
                 ret = response.status_code
             except requests.exceptions.RequestException as e:
                 logger("Error", f"{e}")
```

## t4flib/gcloud_helper.py

```diff
@@ -1,20 +1,20 @@
 import shutil
 
 from google.cloud import bigquery
 from google.oauth2 import service_account
 from google.cloud import storage
 from google.api_core import exceptions as gcloud_ex
 import pandas as pd
-from .log_helper import logger
-from .config import GCP_ACCOUNT_SERVICE_FILE, ENVIRONEMENT, PROXY_AUCHAN, BQ_PROJECT_ID
+from log_helper import logger
+from config import GCP_ACCOUNT_SERVICE_FILE, ENVIRONEMENT, PROXY_AUCHAN, BQ_PROJECT_ID
 import os
 
 
-def run_bq_query(query) -> (int, pd.DataFrame):
+def run_bq_query(query):
     ENVIRONEMENT='dev'
     credentials = service_account.Credentials.from_service_account_file(GCP_ACCOUNT_SERVICE_FILE)
     if ENVIRONEMENT == 'dev':
         os.environ["HTTPS_PROXY"] = PROXY_AUCHAN
     try:
         logger('DEBUG', query)
         client = bigquery.Client(credentials=credentials)
@@ -55,14 +55,17 @@
     except gcloud_ex.GoogleAPIError as e:
         logger('ERROR', f"Une erreur s'est produite lors de l'exécution de la requête : {str(e)}")
         return 1, None
 
     except Exception as e:
         logger('ERROR', f'Une erreur non repertorié est survenue : {str(e)}')
         return 1, None
+    
+
+
 def upload_file_to_gcs(file_path, bucket_name, path_bucket):
     logger('INFO', f'Début de l\'upload du fichier {file_path} vers le bucket {bucket_name}')
     try:
         if ENVIRONEMENT == 'dev':
             os.environ["HTTPS_PROXY"] = PROXY_AUCHAN
 
         credentials = service_account.Credentials.from_service_account_file(GCP_ACCOUNT_SERVICE_FILE)
@@ -71,12 +74,12 @@
         blob = bucket.blob(path_bucket)
         blob.upload_from_filename(file_path)
 
         logger('INFO', f'Le fichier {file_path} a été envoyé à gs://{os.path.join(bucket_name,path_bucket)} avec succès' )
         return 0
 
     except FileNotFoundError as e:
-        logger('ERROR',f'Le fichier {nom_fichier_local} est introuvable : {e}')
+        logger('ERROR',f'Le fichier {file_path} est introuvable : {e}')
         return 1
     except Exception as e:
         logger('ERROR',f'Une erreur inattendue s\'est produite : {e}')
         return 1
```

## t4flib/log_helper.py

```diff
@@ -7,22 +7,26 @@
 import inspect
 
 
 def logger(severity, message):
     init()
     """Log un message avec une timestamp et une couleur selon la sévérité"""
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    frame_records = inspect.stack()[1:]
+    indent = len(frame_records)
+
+    indentation = '-' * 2 * indent
 
     if severity == 'INFO':
         color = Fore.GREEN
     elif severity == 'WARNING':
         color = Fore.YELLOW
     elif severity == 'ERROR':
         color = Fore.RED
     elif severity == 'DEBUG':
         color = Fore.BLUE
     else:
         color = Fore.WHITE
 
     print(
-        f"[{timestamp}] - [{Fore.CYAN}{inspect.stack()[1].function}{Fore.RESET}] - "
+        f"|{indentation} [{timestamp}] - [{Fore.CYAN}{inspect.stack()[1].function}{Fore.RESET}] - "
         f"[{color}{severity}{Fore.RESET}] {message}")
```

## Comparing `t4flib-0.1.9.dist-info/METADATA` & `t4flib-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.1.9
+Version: 0.2.0
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

