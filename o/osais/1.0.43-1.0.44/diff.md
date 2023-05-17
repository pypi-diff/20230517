# Comparing `tmp/osais-1.0.43.tar.gz` & `tmp/osais-1.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-fc5li7s8\osais-1.0.43.tar", last modified: Mon May 15 18:23:03 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-wztvg7u7\osais-1.0.44.tar", last modified: Wed May 17 10:39:07 2023, max compression
```

## Comparing `osais-1.0.43.tar` & `osais-1.0.44.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 18:23:03.843987 osais-1.0.43/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.43/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-05-15 18:23:03.842988 osais-1.0.43/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.43/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 18:23:03.836915 osais-1.0.43/osais/
--rw-rw-rw-   0        0        0      962 2023-05-15 18:22:28.000000 osais-1.0.43/osais/__init__.py
--rw-rw-rw-   0        0        0    52377 2023-05-15 18:22:20.000000 osais-1.0.43/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-05-15 18:23:03.841988 osais-1.0.43/osais.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 18:23:03.000000 osais-1.0.43/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.43/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 18:23:03.843987 osais-1.0.43/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-05-15 18:22:48.000000 osais-1.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:39:07.357032 osais-1.0.44/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.44/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-05-17 10:39:07.356032 osais-1.0.44/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.44/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 10:39:07.351032 osais-1.0.44/osais/
+-rw-rw-rw-   0        0        0     1006 2023-05-17 10:38:31.000000 osais-1.0.44/osais/__init__.py
+-rw-rw-rw-   0        0        0    54100 2023-05-17 10:37:38.000000 osais-1.0.44/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:39:07.355031 osais-1.0.44/osais.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.44/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 10:39:07.357032 osais-1.0.44/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-05-17 10:38:49.000000 osais-1.0.44/setup.py
```

### Comparing `osais-1.0.43/LICENSE` & `osais-1.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.43/PKG-INFO` & `osais-1.0.44/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.43
+Version: 1.0.44
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.43/osais/__init__.py` & `osais-1.0.44/osais/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.43"
+__version__="1.0.44"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isDebug
 from .osais import osais_isDocker
 from .osais import osais_isLocal
 from .osais import osais_isVirtualAI
 from .osais import osais_loadConfig
 from .osais import osais_getEnv
 from .osais import osais_getHarwareInfo
 from .osais import osais_getDirectoryListing
 from .osais import osais_downloadImage
-from .osais import osais_uploadeFileToS3
+from .osais import osais_uploadFileToS3
+from .osais import osais_downloadFileFromS3
 from .osais import osais_getInfo
 from .osais import osais_getClientID
 from .osais import osais_resetGateway
 from .osais import osais_authenticateAI
 from .osais import osais_authenticateClient
 from .osais import osais_postRequest
 from .osais import osais_initParser
```

### Comparing `osais-1.0.43/osais/osais.py` & `osais-1.0.44/osais/osais.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.43"
+__version__="1.0.44"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -38,18 +38,15 @@
     def on_created(self, event):
 
         if event.is_directory:
             return
         if event.event_type == 'created':
             ## only notify if uid in the filename (otherwise we are getting notified of another AI's job !)
             if self._args["-uid"] in event.src_path:
-                self.fnOnFileCreated(os.path.dirname(event.src_path), os.path.basename(event.src_path), self._args)
-
-                ## also send to S3
-                osais_uploadeFileToS3(event.src_path, "output/")
+                self.fnOnFileCreated(os.path.dirname(event.src_path)+"/", os.path.basename(event.src_path), self._args)
 
 def start_observer_thread(path, fnOnFileCreated, _args):
 
     ## watch directory and call back if file was created
     def watch_directory(path, fnOnFileCreated, _args):    
 
         print ("=> starting a watch on path: "+path+"\r\n")
@@ -320,16 +317,29 @@
         "modules": get_list_of_modules()
     }
 
 ## ------------------------------------------------------------------------
 #       File / Image utils
 ## ------------------------------------------------------------------------
 
+def getS3BucketRoot () :
+    return "s3://osais/"
+
+def getS3BucketInputDir () :
+    return "input/"
+
+def getS3BucketOutputDir () :
+    return "output/"
+
 ## downloads an image as file from external URL
 def osais_downloadImage(url) :
+    root=getS3BucketRoot()
+    if root in url:
+        return osais_downloadFileFromS3(url, gInputDir)
+
     import urllib.request
 
     # Determine the file name and extension of the image based on the URL.
     file_name, file_extension = os.path.splitext(url)
     print ("will download image from "+url)
     
     # Define the local file path where the image will be saved.
@@ -341,31 +351,54 @@
     response = urllib.request.urlopen(url)
     image_data = response.read()
     with open(local_file_path, 'wb') as f:
         f.write(image_data)
 
     return f"{local_filename}{file_extension}"
 
-def osais_uploadeFileToS3(_filename, _dirS3): 
+def osais_uploadFileToS3(_filename, _dirS3): 
     global gS3
     global gS3Bucket
-
+    root=getS3BucketRoot()
     if gS3!=None:
         try:
             # Filename - File to upload
             # Bucket - Bucket to upload to (the top level directory under AWS S3)
             # Key - S3 object name (can contain subdirectories). If not specified then file_name is used
-            gS3.meta.client.upload_file(Filename=_filename, Bucket=gS3Bucket, Key=_dirS3+os.path.basename(_filename))
-            return True
+            _baseName=os.path.basename(_filename)
+            gS3.meta.client.upload_file(Filename=_filename, Bucket=gS3Bucket, Key=_dirS3+_baseName)
+            return root+_dirS3+_baseName
+            
         except Exception as err:
             consoleLog({"msg":"Could not upload file to S3"})
             raise err
         
     return False
 
+def osais_downloadFileFromS3(_filePath, _dir): 
+    global gS3
+    global gS3Bucket
+
+    if gS3!=None:
+        try:
+            # Filename - File to upload
+            # Bucket - Bucket to upload to (the top level directory under AWS S3)
+            # Key - S3 object name (can contain subdirectories). If not specified then file_name is used
+            _baseName=os.path.basename(_filePath)
+            local_file_path = _dir+_baseName
+
+            gS3.Bucket(gS3Bucket).download_file(_filePath, local_file_path)
+            return local_file_path
+        except Exception as err:
+            consoleLog({"msg":"Could not download file from S3"})
+            raise err
+        
+    return False
+
+
 ## ========================================================================
 ## 
 ##                      OSAIS starts here 
 ## 
 ## ========================================================================
 
 ## ------------------------------------------------------------------------
@@ -376,15 +409,15 @@
 import schedule
 import json
 import sys
 import base64
 from datetime import datetime
 import argparse
 
-##from osais import osais_initializeAI, osais_getInfo, osais_getHarwareInfo, osais_isDocker, osais_getClientID, osais_getDirectoryListing, osais_runAI, osais_authenticateAI, osais_isDebug, osais_authenticateClient, osais_postRequest, osais_downloadImage, osais_uploadeFileToS3
+##from osais import osais_initializeAI, osais_getInfo, osais_getHarwareInfo, osais_isDocker, osais_getClientID, osais_getDirectoryListing, osais_runAI, osais_authenticateAI, osais_isDebug, osais_authenticateClient, osais_postRequest, osais_downloadImage, osais_uploadFileToS3
 
 ## ------------------------------------------------------------------------
 #       all global vars
 ## ------------------------------------------------------------------------
 
 gVersionLibOSAIS=__version__    ## version of this library (to keep it latest everywhere)
 gUsername=None                  ## user owning this AI (necessary to claim VirtAI regs)
@@ -1009,27 +1042,30 @@
     global gOutputDir
     global gIsWarmup
 
     # Create the parser
     vq_parser = argparse.ArgumentParser(description='Arg parser init by OSAIS')
 
     # Add the AI Gateway / OpenSourceAIs arguments
-    vq_parser.add_argument("-orig",  "--origin", type=str, help="AI Gateway server origin", default=f"http://{gIPLocal}:{gPortGateway}/" , dest='OSAIS_origin')     ##  this is for comms with AI Gateway
-    vq_parser.add_argument("-t",  "--token", type=str, help="OpenSourceAIs token", default="0", dest='tokenAI')               ##  this is for comms with OpenSourceAIs
+    vq_parser.add_argument("-orig",  "--origin", type=str, help="Caller's origin", default=None , dest='OSAIS_origin')      ##  this is for comms with AI Gateway
+    vq_parser.add_argument("-t",  "--token", type=str, help="OpenSourceAIs token", default="0", dest='tokenAI')             ##  this is for comms with OpenSourceAIs
     vq_parser.add_argument("-u",  "--username", type=str, help="OpenSourceAIs username", default="", dest='username')       ##  this is for comms with OpenSourceAIs
     vq_parser.add_argument("-uid",  "--unique_id", type=int, help="Unique ID of this AI session", default=0, dest='uid')    ##  this is for comms with OpenSourceAIs
     vq_parser.add_argument("-odir", "--outdir", type=str, help="Output directory", default=gOutputDir, dest='outdir')
     vq_parser.add_argument("-idir", "--indir", type=str, help="input directory", default=gInputDir, dest='indir')
-    vq_parser.add_argument("-local", "--islocal", type=bool, help="is local or prod?", default=False, dest='isLocal')
     vq_parser.add_argument("-cycle", "--cycle", type=int, help="cycle", default=0, dest='cycle')
     vq_parser.add_argument("-filename", "--filename", type=str, help="filename", default="default", dest='filename')
     vq_parser.add_argument("-warmup", "--warmup", type=bool, help="warmup", default=False, dest='warmup')
 
     gArgsOSAIS = vq_parser.parse_args(aArg)
     gIsWarmup=(gArgsOSAIS.warmup==True or gArgsOSAIS.warmup=="True")
+    if gArgsOSAIS.OSAIS_origin!=None:
+        print("=> origin set to "+gArgsOSAIS.OSAIS_origin)
+    else:
+        print("=> origin set to None")
     return True
 
 ## PUBLIC - run the AI (at least try)
 def osais_runAI(*args):
     global gIsBusy
     global gAProcessed
     global gName 
@@ -1043,101 +1079,96 @@
 
     ## do not process twice same uid
     _uid=_args.get('-uid')
     if _uid in gAProcessed:
         consoleLog({"msg": "Not processing "+str(_uid)+", already tried!"})
         return  None
     
-    ## where is the caller?
-    _orig=None
-    try: 
-        if _args["-orig"]:
-            _orig=_args["-orig"]
-            print("=> origin set to "+_orig)
-    except:
-        _orig=None
-        print("=> origin set to Default")
+    ## process the filename and download it locally
+    try:
+        ## the filename of the locally downloaded "url_upload" url (or the S3 url)
+        _filename=_args.get('-filename')
+
+        # if file was in S3, download it
+        _isFileInS3= getS3BucketRoot() in _filename
+        if _isFileInS3:
+            try:
+                # download the file locally, reset dir to ours
+                _basename=_filename[11:]
+                _filename=osais_downloadFileFromS3(_basename, gInputDir)
+                _args["-filename"]=os.path.basename(_filename)
+                _args["-idir"]=gInputDir
+                _args["-odir"]=gOutputDir
+
+            except Exception as err:
+                consoleLog({"msg":"Could not download image from S3"})
+                raise err
+        else:
+            if not _args["-warmup"]:
+                raise ValueError("CRITICAL: require a upload url in S3 ")
+                
+    except Exception as err:
+        consoleLog({"msg":"did not get an upload url"})
+        raise err
 
     ## start time
     gIsBusy=True
     beg_date = datetime.utcnow()
-
+    
     ## reprocess AI args
     aArgForparserAI=_getArgs(_args)
-    args_ExclusiveOSAIS=['-orig', '-t', '-u', '-uid', '-local', '-cycle', '-warmup', "-filename"]
+    args_ExclusiveOSAIS=['-orig', '-t', '-u', '-uid', '-cycle', '-warmup']
     aArgForparserAI=_argsFromFilter(aArgForparserAI, args_ExclusiveOSAIS, False)
 
-    ## process the filename passed in dir (case localhost / AI Gateway), or download file from URL (case AI running as Virtual AI)
-    _input=None
-    _filename=None
-    _urlUpload=None
-    try:
-        ## the filename of the locally downloaded "url_upload" url 
-        _filename=_args.get('-filename')
-    except Exception as err:
-        consoleLog({"msg":"did not get a filename"})
-        raise err
-    
-    try:
-        _urlUpload=_args.get('url_upload')
-    except Exception as err:
-        consoleLog({"msg":"did not get an upload url"})
-        raise err
-
-    # only a urlUpload? => we need to download the file 
-    # note that lots can fail with 403 on download image from ext API, so we shall avoid this
-    if not _filename and _urlUpload:
-        try:
-            _input=osais_downloadImage(_urlUpload)
-            if _input:
-                aArgForparserAI.append("-filename")
-                aArgForparserAI.append(_input)
-                print("=> downloaded file "+_urlUpload)
-            else:
-                ## min requirements
-                consoleLog({"msg":"no file to process"})
-                return None
-        except Exception as err:
-            gIsBusy=False
-            consoleLog({"msg":"Could not download image"})
-            raise err
-
     ## Init OSAIS Params (from all args, keep only those for OSAIS)
     aArgForParserOSAIS=_getArgs(_args)
     args_ExclusiveOSAIS.append('-odir')
     args_ExclusiveOSAIS.append('-idir')
     aArgForParserOSAIS=_argsFromFilter(aArgForParserOSAIS, args_ExclusiveOSAIS, True)
     osais_initParser(aArgForParserOSAIS)
 
+    ## now that we have processed args, we keep them locally (avoid globals messup)
+    _localOrig=gArgsOSAIS.OSAIS_origin
+    _localT=gArgsOSAIS.tokenAI
+    _localU=gArgsOSAIS.username
+    _localUID=gArgsOSAIS.uid
+    _localODir=gArgsOSAIS.outdir
+    _localIDir=gArgsOSAIS.indir
+    _localCycle=gArgsOSAIS.cycle
+    _localFilename=gArgsOSAIS.filename
+
+    _isGateway=None
     if gIsWarmup:
         print("=> Warming up...")
     else:
+        ## req received from a gateway ot OSAIS?
+        _isGateway = not (_localOrig == "https://opensourceais.com/" or _localOrig == "https://opensourceais.com" or _localOrig[:5]== "http:")
         print("=> before run: processed args from url: "+str(aArgForparserAI)+"\r\n")
 
     ## notify OSAIS (Req received)
-    CredsParam=getCredsParams()
-    MorphingParam=getMorphingParams()
+    CredsParam=getCredsParams(_localT, _localU, _isGateway)
+    MorphingParam=getMorphingParams(_localUID, _localCycle, _localFilename)
     StageParam=getStageParams(AI_PROGRESS_REQRECEIVED, 0)
-    osais_notify(_orig, CredsParam, MorphingParam , StageParam)
+    osais_notify(_localOrig, CredsParam, MorphingParam , StageParam)
 
     ## processing accepted
     gLastProcessStart_at=datetime.utcnow()
     gAProcessed.append(_uid)
 
     ## notify OSAIS (start)
     StageParam=getStageParams(AI_PROGRESS_AI_STARTED, 0)
-    osais_notify(_orig, CredsParam, MorphingParam , StageParam)
+    osais_notify(_localOrig, CredsParam, MorphingParam , StageParam)
 
     ## start watch file creation
     _output=_getOutputDir()
     watch_directory(_output, osais_onNotifyFileCreated, _args)
     
     ## Notif OSAIS
     StageParam=getStageParams(AI_PROGRESS_INIT_IMAGE, 0)
-    osais_notify(_orig, CredsParam, MorphingParam , StageParam)
+    osais_notify(_localOrig, CredsParam, MorphingParam , StageParam)
 
     ## run AI
     response=None
     try:
         if len(args)==2:
             response=fn_run(aArgForparserAI)
         else:
@@ -1155,15 +1186,15 @@
     end_date = datetime.utcnow()
     delta=end_date - beg_date
     cost = int(delta.total_seconds()* 1000 + delta.microseconds / 1000)
     _addCost(cost)
 
     ## notify end
     StageParam=getStageParams(AI_PROGRESS_AI_STOPPED, cost)
-    osais_notify(_orig, CredsParam, MorphingParam , StageParam)
+    osais_notify(_localOrig, CredsParam, MorphingParam , StageParam)
 
     if gIsWarmup:
         _strDelta=str(delta)
         print("\r\n=> AI ready!")
         print("=> Able to process requests in "+_strDelta+" secs\r\n")
 
     ## default OK response if the AI does not send any
@@ -1171,32 +1202,31 @@
         response=True
     return response
 
 ## ------------------------------------------------------------------------
 #       get formatted params from AI current state
 ## ------------------------------------------------------------------------
 
-def getCredsParams() :
+def getCredsParams(_token, _username, _isGateway) :
     global gName
     global gArgsOSAIS
     return {
         "engine": gName, 
         "version": gVersion, 
-        "tokenAI": gArgsOSAIS.tokenAI,
-        "username": gArgsOSAIS.username,
-        "isLocal": gArgsOSAIS.isLocal
+        "tokenAI": _token,
+        "username": _username,
+        "isGateway": _isGateway
     } 
 
-def getMorphingParams() :
+def getMorphingParams(_localUID, _localCycle, _localFilename) :
     global gArgsOSAIS
     return {
-        "uid": gArgsOSAIS.uid,
-        "cycle": gArgsOSAIS.cycle,
-        "filename": gArgsOSAIS.filename, 
-        "odir": _getOutputDir()
+        "uid": _localUID,
+        "cycle": _localCycle,
+        "filename": _localFilename
     }
 
 def getStageParams(_stage, _cost) :
     global gArgsOSAIS
     if _stage==AI_PROGRESS_REQRECEIVED:
         return {"stage": AI_PROGRESS_REQRECEIVED, "descr":"Acknowledged request"}
     if _stage==AI_PROGRESS_ERROR:
@@ -1242,38 +1272,45 @@
     
     global gVAIAuthToken
     
     # lets go call OSAIS AI Gateway / or OSAIS itself
     headers = {
         "Content-Type": 'application/json', 
         'Accept': 'text/plain',
-        "Authorization": f"Bearer {gVAIAuthToken}"
     }
 
     api_url=f"{_origin}api/v1/public/upload"        
     payload = json.dumps(objParam)
     response = requests.post(api_url, headers=headers, data=payload )
     objRes=response.json()
     return objRes    
 
+## got notified of file creation (by watch)
 def osais_onNotifyFileCreated(_dir, _filename, _args):
     ## where is the caller?
-    _orig=None
+    _isGateway=None
+    _origin=_args.get('-orig')
+    if _origin!=None:
+        _isGateway = not (_origin == "https://opensourceais.com/" or _origin == "https://opensourceais.com" or _origin[:5]== "http:")
+
+    ## also send to S3
+    _fileS3=osais_uploadFileToS3(_dir+_filename, getS3BucketOutputDir())
+
+    # notify
+    _cycle=0
     try: 
-        if _args["-orig"]:
-            _orig=_args["-orig"]
+        if _args["-cycle"]:
+            _cycle=_args["-cycle"]
     except:
-        _orig=None
+        _cycle=0
 
-    # notify
-    gArgsOSAIS.filename=_filename
     _stageParam=getStageParams(AI_PROGRESS_DONE_IMAGE, 0)
-    _morphingParam=getMorphingParams()
-    _credsParam=getCredsParams()
-    osais_notify(_orig, _credsParam, _morphingParam, _stageParam)            # OSAIS Notification
+    _morphingParam=getMorphingParams(_args["-uid"], _cycle, _fileS3)
+    _credsParam=getCredsParams(_args["-t"], _args["-u"], _isGateway)
+    osais_notify(_origin, _credsParam, _morphingParam, _stageParam)            # OSAIS Notification
     return True
 
 def _notifyGateway(_origin, objParam):
     headers = {
         "Content-Type": "application/json"
     }
     api_url=f"{_origin}api/v1/public/notify"
@@ -1336,52 +1373,56 @@
         }
     }
 
     if "cost" in StageParam:
         objParam["response"]["cost"]= str(StageParam["cost"])
 
     ## Notify OSAIS (as Virtual AI)
-    if gIsVirtualAI:
+    if gIsVirtualAI and CredParam["isGateway"]==False:
         try: 
             objRes=_notifyOSAIS(objParam)
             _at=objRes["data"]["notified_at"]
-            print("\r\n ["+_at+"] => Notified OSAIS ("+str(StageParam["stage"])+"/ "+StageParam["descr"]+"): "+str(merged)+ " on: "+api_url)
+            print("\r\n ["+_at+"] => Notified OSAIS ("+str(StageParam["stage"])+"/ "+StageParam["descr"]+"): "+str(merged))
         except:
-            consoleLog({"msg": "Failed to notify stage ("+str(StageParam["stage"])+ " to OSAIS"})
+            consoleLog({"msg": "VAI Failed to notify stage ("+str(StageParam["stage"])+ ") to OSAIS"})
 
     ## Notify Gateway (as Local AI)
-    if gIsLocal:
+    if gIsLocal and CredParam["isGateway"]==True :
         try: 
             objRes=_notifyGateway(_origin, objParam)
             _at=objRes["data"]["notified_at"]
-            print("\r\n ["+_at+"] => Notified Gateway ("+str(StageParam["stage"])+"/ "+StageParam["descr"]+"): "+str(merged)+ " on: "+api_url)
+            print("\r\n ["+_at+"] => Notified Gateway ("+str(StageParam["stage"])+"/ "+StageParam["descr"]+"): "+str(merged)+ " on: "+_origin+"\r\n")
         except:
-            consoleLog({"msg": "Failed to notify stage ("+str(StageParam["stage"])+ " to local Gateway "+_origin})
+            consoleLog({"msg": "Local AI Failed to notify stage ("+str(StageParam["stage"])+ ") to local Gateway "+_origin})
 
     if StageParam["stage"]==AI_PROGRESS_DONE_IMAGE:
-        if gIsVirtualAI==True:
-            _dir=MorphingParam["odir"]
-            if _dir==None:
-                _dir=gOutputDir
-            _dirImage=_dir+_filename
-
-            with open(_dirImage, "rb") as image_file:
-                image_data = image_file.read()
-
-            im_b64 = base64.b64encode(image_data).decode("utf8")
-            param={
-                "image": im_b64,
-                "uid": str(MorphingParam["uid"]),
-                "cycle": str(MorphingParam["cycle"]),
-                "engine": CredParam["engine"],
-            }            
-            if CredParam["isLocal"]:
-                _uploadImageToGateway(_origin, param)
-            else:
-                _uploadImageToOSAIS(_origin, param)
+        # we do not need to upload if already in s3
+        if not getS3BucketRoot() in _filename:
+            if gIsVirtualAI==True:
+                _dir=MorphingParam["odir"]
+                if _dir==None:
+                    _dir=gOutputDir
+                _dirImage=_dir+_filename
+
+                with open(_dirImage, "rb") as image_file:
+                    image_data = image_file.read()
+
+                im_b64 = base64.b64encode(image_data).decode("utf8")
+                param={
+                    "image": im_b64,
+                    "uid": str(MorphingParam["uid"]),
+                    "cycle": str(MorphingParam["cycle"]),
+                    "engine": CredParam["engine"],
+                }   
+
+    #            if CredParam["isGateway"]==True:
+    #                _uploadImageToGateway(_origin, param)
+
+                if CredParam["isGateway"]==False:
+                    _uploadImageToOSAIS(_origin, param)
     return objRes
 
 ## ------------------------------------------------------------------------
 #       Init processing
 ## ------------------------------------------------------------------------
 
 ## PUBLIC - resetting who this AI is talking to (OSAIS prod and dbg)
@@ -1429,14 +1470,15 @@
     gOriginGateway=f"http://{gIPLocal}:{gPortGateway}/"         ## config for local gateway (local and not virtual)
 
     ## we set OSAIS location in all cases (even if in gateway) because this AI can generate it s own page for sending reqs (needs a client logged into OSAIS)
     if gIsDebug:
         osais_resetOSAIS(f"http://{gIPLocal}:{gPortLocalOSAIS}/")
     else:
         osais_resetOSAIS("https://opensourceais.com/")
+    
     if gIsVirtualAI:
         try:
             osais_authenticateAI()
         except Exception as err:
             print("=> CRITICAL: Could not connect virtual AI "+gName+ " to OSAIS")
             return None
```

### Comparing `osais-1.0.43/osais.egg-info/PKG-INFO` & `osais-1.0.44/osais.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.43
+Version: 1.0.44
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.43/setup.py` & `osais-1.0.44/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.43',
+    version='1.0.44',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

