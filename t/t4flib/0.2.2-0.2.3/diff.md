# Comparing `tmp/t4flib-0.2.2-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.2.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10746 bytes, number of entries: 12
+Zip file size: 10778 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      892 b- defN 23-May-17 17:25 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
 -rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
--rw-rw-r--  2.0 unx     4501 b- defN 23-May-17 15:49 t4flib/filetransfer_helper.py
+-rw-rw-r--  2.0 unx     4696 b- defN 23-May-17 18:05 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
 -rw-rw-r--  2.0 unx     3235 b- defN 23-May-17 15:49 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-17 15:14 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-17 17:38 t4flib-0.2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-17 17:38 t4flib-0.2.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-17 17:38 t4flib-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 23-May-17 17:38 t4flib-0.2.2.dist-info/RECORD
-12 files, 26823 bytes uncompressed, 9214 bytes compressed:  65.6%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-17 18:18 t4flib-0.2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-17 18:18 t4flib-0.2.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-17 18:18 t4flib-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 23-May-17 18:18 t4flib-0.2.3.dist-info/RECORD
+12 files, 27018 bytes uncompressed, 9246 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.2.2.dist-info/METADATA
+Filename: t4flib-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.2.2.dist-info/WHEEL
+Filename: t4flib-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.2.2.dist-info/top_level.txt
+Filename: t4flib-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.2.2.dist-info/RECORD
+Filename: t4flib-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/filetransfer_helper.py

```diff
@@ -49,74 +49,80 @@
         return None
     else:
         # L'index est valide, retourner l'élément correspondant
         return arr[index]
 
 
 def get_flow_attributes_in_file(flow_name):
-    logger('INFO', f'Vérification de l\' existance du flux {flow_name}')
 
-    if FT_PARAM_FILEPATH is not None and os.path.exists(FT_PARAM_FILEPATH):
-        with open(FT_PARAM_FILEPATH, 'r+', encoding='utf-8') as ft_param_file:
-            csv_reader = csv.reader(ft_param_file, delimiter=';')
-            for line_flow in csv_reader:
-                if get_element_safely(line_flow, 0) == flow_name:
-                    logger('INFO', f'le flux {flow_name} a été trouve')
-                    return ft_flow(
-                        get_element_safely(line_flow, 0),
-                        get_element_safely(line_flow, 1),
-                        get_element_safely(line_flow, 2),
-                        get_element_safely(line_flow, 3),
-                        get_element_safely(line_flow, 4),
-                        get_element_safely(line_flow, 5),
-                        get_element_safely(line_flow, 6),
-                    )
-            logger('ERROR', f'Le flux {flow_name} est introuvable')
-            return None
+    try:
 
-    else:
-        logger('ERROR', f'Le fichier de paramètre {FT_PARAM_FILEPATH} n\'existe pas ')
+        logger('INFO', f'Vérification de l\' existance du flux {flow_name}')
+        flows=[]
+
+        if FT_PARAM_FILEPATH is not None and os.path.exists(FT_PARAM_FILEPATH):
+            with open(FT_PARAM_FILEPATH, 'r+', encoding='utf-8') as ft_param_file:
+                csv_reader = csv.reader(ft_param_file, delimiter=';')
+                for line_flow in csv_reader:
+                    if get_element_safely(line_flow, 0) == flow_name:
+                        logger('INFO', f'le flux {flow_name} a été trouve')
+                        flows.append(ft_flow(
+                            get_element_safely(line_flow, 0),
+                            get_element_safely(line_flow, 1),
+                            get_element_safely(line_flow, 2),
+                            get_element_safely(line_flow, 3),
+                            get_element_safely(line_flow, 4),
+                            get_element_safely(line_flow, 5),
+                            get_element_safely(line_flow, 6),
+                        ))
+                logger('ERROR', f'Le flux {flow_name} est introuvable')
+        return flows
+
+    except Exception as e:
+        logger('ERROR', f'{str(e)}')
 
 
 def send_file_by_filetransfer(flow_name):
     logger('INFO', f'Envoi dans filetransfer du flux {flow_name}')
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-    ft_flow_to_send = get_flow_attributes_in_file(flow_name)
+    ft_flows_to_send = get_flow_attributes_in_file(flow_name)
 
-    if ft_flow_to_send is not None:
+    if len(ft_flows_to_send) > 0:
         session = requests.Session()
         retry = Retry(total=5, backoff_factor=0.1, status_forcelist=[401, 403, 404, 429, 500, 502, 503, 504])
         adapter = HTTPAdapter(max_retries=retry)
         session.mount('http://', adapter)
         session.mount('https://', adapter)
 
         headers = {
             "Content-type": "application/json",
             "X-Gravitee-api-Key": FT_GRAVITEE_KEY
         }
 
-        logger('DEBUG', ft_flow_to_send.path_to_get_file)
-        for file in get_all_file_by_filemask(ft_flow_to_send.path_to_get_file, ft_flow_to_send.filemask):
+        for ft_flow_to_send in ft_flows_to_send:
+
+            logger('DEBUG', ft_flow_to_send.path_to_get_file)
+            for file in get_all_file_by_filemask(ft_flow_to_send.path_to_get_file, ft_flow_to_send.filemask):
 
-            shutil.copy(str(file.absolute()), ft_flow_to_send.path_out)
+                shutil.copy(str(file.absolute()), ft_flow_to_send.path_out)
 
-            body_request = json.dumps({
-                "flow": ft_flow_to_send.flow_name,
-                "userId": ft_flow_to_send.server,
-                "authKey": ft_flow_to_send.ft_key,
-                "uri": str(file.absolute())
-            })
-
-            try:
-                response = requests.post(FT_GRAVITEE_URL, headers=headers, data=body_request, verify=False)
-                ret = response.status_code
-            except requests.exceptions.RequestException as e:
-                logger("Error", f"{e}")
-                ret = None
+                body_request = json.dumps({
+                    "flow": ft_flow_to_send.flow_name,
+                    "userId": ft_flow_to_send.server,
+                    "authKey": ft_flow_to_send.ft_key,
+                    "uri": str(file.absolute())
+                })
+
+                try:
+                    response = requests.post(FT_GRAVITEE_URL, headers=headers, data=body_request, verify=False)
+                    ret = response.status_code
+                except requests.exceptions.RequestException as e:
+                    logger("Error", f"{e}")
+                    ret = None
 
-            if ret in [202, 200]:
+                if ret in [202, 200]:
 
-                logger("INFO", f"Le flux {flow_name} contenant le fichier {str(file)} est parti")
-            else:
+                    logger("INFO", f"Le flux {flow_name} contenant le fichier {str(file)} est parti")
+                else:
 
-                logger('ERROR', f"Un code erreur API : {ret} a eu lieu")
-                logger('ERROR', f"Erreur lors de l'appel à l'API statut => {ret}")
+                    logger('ERROR', f"Un code erreur API : {ret} a eu lieu")
+                    logger('ERROR', f"Erreur lors de l'appel à l'API statut => {ret}")
```

## Comparing `t4flib-0.2.2.dist-info/METADATA` & `t4flib-0.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.2.2.dist-info/RECORD` & `t4flib-0.2.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 t4flib/config.py,sha256=fHt2THXtajPzzV_gnHPZNVmez09ODLfIFrt4cTXgZsE,892
 t4flib/data_helper.py,sha256=SdKdv2U1EXtHJcfEff_I8zIlMWv56-xLZqczAw4kOUU,971
 t4flib/file_helper.py,sha256=NYIgOrA1iJBUcodtaRlDIsIHoivonLme4PmFZB1nQLw,6145
-t4flib/filetransfer_helper.py,sha256=GPDEUa0f-QmTH025pylJOAp0wyZtbhVzMWSjhM8KHxU,4501
+t4flib/filetransfer_helper.py,sha256=e2s7Sd5uNA3NU4AQF7peUzawAiueACtL74Ol7-Uy-xY,4696
 t4flib/functional_helper.py,sha256=CfbwrMufVRwCQNg9us9tujS3oeCmxql18vmo7B5lUAI,7420
 t4flib/gcloud_helper.py,sha256=sy5EpA2iVlcNlveP77N3iUCERNZXabSVOOcz8rifO6I,3235
 t4flib/log_helper.py,sha256=pu_y3m7iHWpkgYnxLYAlQjWjqknMGDcCDjHV6w4YYDc,876
-t4flib-0.2.2.dist-info/METADATA,sha256=xDVGU3I3DmlAPEnGRsKhkjsLgj9bxIbBMWGdKuJKqtM,1747
-t4flib-0.2.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.2.2.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.2.2.dist-info/RECORD,,
+t4flib-0.2.3.dist-info/METADATA,sha256=dFWmmPjDZ4awQIOuFd5F0yxtAJ4cmhV6_K6x75P4iZg,1747
+t4flib-0.2.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.2.3.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.2.3.dist-info/RECORD,,
```

