# Comparing `tmp/servicex_databinder-0.4.0b5.tar.gz` & `tmp/servicex_databinder-0.4.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_databinder-0.4.0b5.tar", last modified: Fri Dec 16 10:48:12 2022, max compression
+gzip compressed data, was "servicex_databinder-0.4.0b6.tar", last modified: Tue Dec 20 03:08:36 2022, max compression
```

## Comparing `servicex_databinder-0.4.0b5.tar` & `servicex_databinder-0.4.0b6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-16 10:48:12.156223 servicex_databinder-0.4.0b5/
--rw-r--r--   0 kchoi      (501) staff       (20)     1521 2021-09-10 04:56:21.000000 servicex_databinder-0.4.0b5/LICENSE
--rw-r--r--   0 kchoi      (501) staff       (20)     9151 2022-12-16 10:48:12.155627 servicex_databinder-0.4.0b5/PKG-INFO
--rw-r--r--   0 kchoi      (501) staff       (20)     8403 2022-12-08 01:38:00.000000 servicex_databinder-0.4.0b5/README.md
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-16 10:48:12.152881 servicex_databinder-0.4.0b5/servicex_databinder/
--rw-r--r--   0 kchoi      (501) staff       (20)      194 2022-12-16 10:42:44.000000 servicex_databinder-0.4.0b5/servicex_databinder/__init__.py
--rw-r--r--   0 kchoi      (501) staff       (20)     4265 2022-12-09 02:05:25.000000 servicex_databinder-0.4.0b5/servicex_databinder/configuration.py
--rw-r--r--   0 kchoi      (501) staff       (20)     4980 2022-12-15 06:43:06.000000 servicex_databinder-0.4.0b5/servicex_databinder/get_servicex_data.py
--rw-r--r--   0 kchoi      (501) staff       (20)     3135 2022-11-11 14:54:29.000000 servicex_databinder-0.4.0b5/servicex_databinder/old_frontend.py
--rw-r--r--   0 kchoi      (501) staff       (20)    14312 2022-11-10 06:04:16.000000 servicex_databinder-0.4.0b5/servicex_databinder/old_output.py
--rw-r--r--   0 kchoi      (501) staff       (20)     9347 2022-12-15 06:52:56.000000 servicex_databinder-0.4.0b5/servicex_databinder/output_handler.py
--rw-r--r--   0 kchoi      (501) staff       (20)     4604 2022-12-09 02:38:51.000000 servicex_databinder-0.4.0b5/servicex_databinder/request.py
--rw-r--r--   0 kchoi      (501) staff       (20)     1401 2022-12-15 06:52:50.000000 servicex_databinder-0.4.0b5/servicex_databinder/servicex_databinder.py
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-16 10:48:12.155112 servicex_databinder-0.4.0b5/servicex_databinder.egg-info/
--rw-r--r--   0 kchoi      (501) staff       (20)     9151 2022-12-16 10:48:11.000000 servicex_databinder-0.4.0b5/servicex_databinder.egg-info/PKG-INFO
--rw-r--r--   0 kchoi      (501) staff       (20)      532 2022-12-16 10:48:12.000000 servicex_databinder-0.4.0b5/servicex_databinder.egg-info/SOURCES.txt
--rw-r--r--   0 kchoi      (501) staff       (20)        1 2022-12-16 10:48:11.000000 servicex_databinder-0.4.0b5/servicex_databinder.egg-info/dependency_links.txt
--rw-r--r--   0 kchoi      (501) staff       (20)      136 2022-12-16 10:48:11.000000 servicex_databinder-0.4.0b5/servicex_databinder.egg-info/requires.txt
--rw-r--r--   0 kchoi      (501) staff       (20)       20 2022-12-16 10:48:11.000000 servicex_databinder-0.4.0b5/servicex_databinder.egg-info/top_level.txt
--rw-r--r--   0 kchoi      (501) staff       (20)       38 2022-12-16 10:48:12.156375 servicex_databinder-0.4.0b5/setup.cfg
--rw-r--r--   0 kchoi      (501) staff       (20)     2148 2022-12-09 05:22:58.000000 servicex_databinder-0.4.0b5/setup.py
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-20 03:08:36.504110 servicex_databinder-0.4.0b6/
+-rw-r--r--   0 kchoi      (501) staff       (20)     1521 2021-09-10 04:56:21.000000 servicex_databinder-0.4.0b6/LICENSE
+-rw-r--r--   0 kchoi      (501) staff       (20)     9151 2022-12-20 03:08:36.503654 servicex_databinder-0.4.0b6/PKG-INFO
+-rw-r--r--   0 kchoi      (501) staff       (20)     8403 2022-12-08 01:38:00.000000 servicex_databinder-0.4.0b6/README.md
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-20 03:08:36.501079 servicex_databinder-0.4.0b6/servicex_databinder/
+-rw-r--r--   0 kchoi      (501) staff       (20)      194 2022-12-20 03:00:41.000000 servicex_databinder-0.4.0b6/servicex_databinder/__init__.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     4265 2022-12-09 02:05:25.000000 servicex_databinder-0.4.0b6/servicex_databinder/configuration.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     4980 2022-12-15 06:43:06.000000 servicex_databinder-0.4.0b6/servicex_databinder/get_servicex_data.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     3135 2022-11-11 14:54:29.000000 servicex_databinder-0.4.0b6/servicex_databinder/old_frontend.py
+-rw-r--r--   0 kchoi      (501) staff       (20)    14312 2022-11-10 06:04:16.000000 servicex_databinder-0.4.0b6/servicex_databinder/old_output.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     9487 2022-12-20 02:53:17.000000 servicex_databinder-0.4.0b6/servicex_databinder/output_handler.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     4604 2022-12-09 02:38:51.000000 servicex_databinder-0.4.0b6/servicex_databinder/request.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     1401 2022-12-15 06:52:50.000000 servicex_databinder-0.4.0b6/servicex_databinder/servicex_databinder.py
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-20 03:08:36.503176 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/
+-rw-r--r--   0 kchoi      (501) staff       (20)     9151 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/PKG-INFO
+-rw-r--r--   0 kchoi      (501) staff       (20)      532 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/SOURCES.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)        1 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/dependency_links.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)      136 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/requires.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)       20 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/top_level.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)       38 2022-12-20 03:08:36.504217 servicex_databinder-0.4.0b6/setup.cfg
+-rw-r--r--   0 kchoi      (501) staff       (20)     2148 2022-12-09 05:22:58.000000 servicex_databinder-0.4.0b6/setup.py
```

### Comparing `servicex_databinder-0.4.0b5/LICENSE` & `servicex_databinder-0.4.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/PKG-INFO` & `servicex_databinder-0.4.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex_databinder
-Version: 0.4.0b5
+Version: 0.4.0b6
 Summary: ServiceX data management using a configuration file
 Home-page: https://github.com/kyungeonchoi/ServiceXDataBinder
 Author: KyungEon Choi (UT Austin)
 Author-email: kyungeonchoi@utexas.edu
 License: BSD 3-clause
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `servicex_databinder-0.4.0b5/README.md` & `servicex_databinder-0.4.0b6/README.md`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder/configuration.py` & `servicex_databinder-0.4.0b6/servicex_databinder/configuration.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder/get_servicex_data.py` & `servicex_databinder-0.4.0b6/servicex_databinder/get_servicex_data.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder/old_frontend.py` & `servicex_databinder-0.4.0b6/servicex_databinder/old_frontend.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder/old_output.py` & `servicex_databinder-0.4.0b6/servicex_databinder/old_output.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder/output_handler.py` & `servicex_databinder-0.4.0b6/servicex_databinder/output_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import yaml
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any, Dict, List
 import time
+from filecmp import cmp
 from shutil import rmtree
 from aioshutil import copy
 
 import pyarrow.parquet as pq
 import awkward as ak
 import uproot
 
@@ -62,37 +63,42 @@
             outfile.close()
 
 
     #################################
     ### Copy, update and clean up ###
     #################################
     
-    async def copy_files(self, req, files):
+    async def copy_files(self, req, files: List[Path]):
         if (self._backend, self._outputformat) == ('uproot', 'root'):
             target_path = Path(self.output_path, req['Sample'], req['tree'])
             if not target_path.exists():
                 target_path.mkdir(parents=True, exist_ok=True)
                 for file in files:
                     outfile = Path(target_path, Path(file).name)
                     await copy(file, outfile)
                 return f"  {req['Sample']} | {req['tree']} | {str(req['dataset'])[:100]} is delivered"
             else: # target directory exists
                 servicex_files = {Path(file).name for file in files}
                 local_files = {Path(file).name for file in list(target_path.glob("*"))}
-                if servicex_files == local_files: # one RucioDID for this sample and files are already there
-                    return f"  {req['Sample']} | {req['tree']} | {str(req['dataset'])[:100]} is already delivered"
-                else:
-                    # copy files in servicex but not in local
-                    files_not_in_local = servicex_files.difference(local_files)
-                    if files_not_in_local:
-                        for file in files_not_in_local:
-                            await copy(Path(Path(files[0]).parent, file), Path(target_path, file))
-                        return f"  {req['Sample']} | {req['tree']} | {str(req['dataset'])[:100]} is delivered"
-                    else:
-                        return f"  {req['Sample']} | {req['tree']} | {str(req['dataset'])[:100]} is already delivered"
+                servicex_file_path = Path(files[0]).parent
+                
+                # copy files in servicex but not in local
+                files_not_in_local = servicex_files.difference(local_files)
+                if files_not_in_local:
+                    for file in files_not_in_local:
+                        await copy(Path(servicex_file_path, file), Path(target_path, file))
+
+                # copy updated files                
+                files_intersect = servicex_files.intersection(local_files)
+                if files_intersect:
+                    for file in files_intersect:
+                        if not cmp(Path(servicex_file_path, file), Path(target_path, file)):
+                            await copy(Path(servicex_file_path, file), Path(target_path, file))
+                        
+                return f"  {req['Sample']} | {req['tree']} | {str(req['dataset'])[:100]} is delivered"                
 
 
     def clean_up_files_not_in_requests(self, out_paths_dict):
 
         samples_in_requests = out_paths_dict.keys()
         samples_local = [sa.name for sa in self.output_path.iterdir() if sa.is_dir()]
```

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder/request.py` & `servicex_databinder-0.4.0b6/servicex_databinder/request.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder/servicex_databinder.py` & `servicex_databinder-0.4.0b6/servicex_databinder/servicex_databinder.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder.egg-info/PKG-INFO` & `servicex_databinder-0.4.0b6/servicex_databinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex-databinder
-Version: 0.4.0b5
+Version: 0.4.0b6
 Summary: ServiceX data management using a configuration file
 Home-page: https://github.com/kyungeonchoi/ServiceXDataBinder
 Author: KyungEon Choi (UT Austin)
 Author-email: kyungeonchoi@utexas.edu
 License: BSD 3-clause
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `servicex_databinder-0.4.0b5/servicex_databinder.egg-info/SOURCES.txt` & `servicex_databinder-0.4.0b6/servicex_databinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b5/setup.py` & `servicex_databinder-0.4.0b6/setup.py`

 * *Files identical despite different names*

