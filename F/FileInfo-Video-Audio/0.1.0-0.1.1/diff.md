# Comparing `tmp/FileInfo_Video_Audio-0.1.0.tar.gz` & `tmp/FileInfo_Video_Audio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileInfo_Video_Audio-0.1.0.tar", last modified: Wed May 17 10:57:22 2023, max compression
+gzip compressed data, was "FileInfo_Video_Audio-0.1.1.tar", last modified: Wed May 17 14:16:55 2023, max compression
```

## Comparing `FileInfo_Video_Audio-0.1.0.tar` & `FileInfo_Video_Audio-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1498 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1498 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1127 2023-05-17 10:56:40.000000 FileInfo_Video_Audio-0.1.0/README.md
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      816 2023-05-17 10:56:49.000000 FileInfo_Video_Audio-0.1.0/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:26:11.000000 FileInfo_Video_Audio-0.1.0/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.1.0/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.1.0/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3957 2023-05-15 11:49:26.000000 FileInfo_Video_Audio-0.1.0/source/main.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1498 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-17 14:16:55.000000 FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1498 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1127 2023-05-17 10:56:40.000000 FileInfo_Video_Audio-0.1.1/README.md
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      816 2023-05-17 14:16:31.000000 FileInfo_Video_Audio-0.1.1/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:26:11.000000 FileInfo_Video_Audio-0.1.1/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 14:16:55.188400 FileInfo_Video_Audio-0.1.1/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.1.1/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.1.1/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3875 2023-05-17 13:59:03.000000 FileInfo_Video_Audio-0.1.1/source/main.py
```

### Comparing `FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/PKG-INFO` & `FileInfo_Video_Audio-0.1.1/FileInfo_Video_Audio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileInfo-Video-Audio
-Version: 0.1.0
+Version: 0.1.1
 Summary: In this tool is help to get the properties of the Audio and Video files
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `FileInfo_Video_Audio-0.1.0/PKG-INFO` & `FileInfo_Video_Audio-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileInfo_Video_Audio
-Version: 0.1.0
+Version: 0.1.1
 Summary: In this tool is help to get the properties of the Audio and Video files
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `FileInfo_Video_Audio-0.1.0/README.md` & `FileInfo_Video_Audio-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FileInfo_Video_Audio-0.1.0/setup.py` & `FileInfo_Video_Audio-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = os.popen("/usr/local/bin/pipreqs main --print").read().splitlines()
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='FileInfo_Video_Audio',
-    version='0.1.0',
+    version='0.1.1',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
     description="In this tool is help to get the properties of the Audio and Video files",
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details',
     install_requires=requirements,
     long_description=long_description,
```

### Comparing `FileInfo_Video_Audio-0.1.0/source/lib/Argument.py` & `FileInfo_Video_Audio-0.1.1/source/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `FileInfo_Video_Audio-0.1.0/source/main.py` & `FileInfo_Video_Audio-0.1.1/source/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,58 +22,58 @@
                                 if option == i:
                                     print(f"{option} ==> {track[i]}")
                 else:
                     raise Exception("Unable to fetch the Tracks of your Source file")
             except ValueError as e:
                 print(e)
                 
-        # elif Argument.getoptionvalue('--type') and (Argument.hasOption(['--list_All_keys']) or Argument.hasOption(['-l'])):
-        #     file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
-        #     try:
-        #         if file_content["media"]["track"]:
-        #             for track in file_content["media"]["track"]:
-        #                 if(track['@type'] == Argument.getoptionvalue('--type')):
-        #                     for i in track.items():
-        #                         print(f"{i[0]}    ==> {i[1]}")
-        #         else:
-        #             raise Exception("Unable to fetch the Tracks of your Source file")
-        #     except ValueError as e:
-        #         print(e)
+        elif Argument.getoptionvalue('--type') and (Argument.hasOption(['--list_All_keys']) or Argument.hasOption(['-l'])):
+            file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
+            try:
+                if file_content["media"]["track"]:
+                    for track in file_content["media"]["track"]:
+                        if(track['@type'] == Argument.getoptionvalue('--type')):
+                            for i in track.items():
+                                print(f"{i[0]}    ==> {i[1]}")
+                else:
+                    raise Exception("Unable to fetch the Tracks of your Source file")
+            except ValueError as e:
+                print(e)
                             
-        # elif Argument.hasOption(['--type']) and (Argument.hasOption(['--help']) or Argument.hasOption(['-h'])):
-        #     file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
-        #     try:
-        #         if file_content["media"]["track"]:
-        #             for track in file_content["media"]["track"]:
-        #                 tracks = track['@type']
-        #                 if tracks =="General":
-        #                     print(f"{tracks}  ==> Show's the Files General properties" )
-        #                 if tracks =="Video":
-        #                     print(f"{tracks}    ==> Show's the Files Video properties" )
-        #                 if tracks =="Audio":
-        #                     print(f"{tracks}    ==> Show's the Files Audio properties" )
-        #         else:
-        #             raise Exception("Unable to fetch the Tracks of your Source file")
-        #     except ValueError as e:
-        #         print(e)
+        elif Argument.hasOption(['--type']) and (Argument.hasOption(['--help']) or Argument.hasOption(['-h'])):
+            file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
+            try:
+                if file_content["media"]["track"]:
+                    for track in file_content["media"]["track"]:
+                        tracks = track['@type']
+                        if tracks =="General":
+                            print(f"{tracks}  ==> Show's the Files General properties" )
+                        if tracks =="Video":
+                            print(f"{tracks}    ==> Show's the Files Video properties" )
+                        if tracks =="Audio":
+                            print(f"{tracks}    ==> Show's the Files Audio properties" )
+                else:
+                    raise Exception("Unable to fetch the Tracks of your Source file")
+            except ValueError as e:
+                print(e)
                     
                     
-        # elif Argument.getoptionvalue('--type') and  Argument.hasOption(['--options']):
-        #     file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
-        #     try:
-        #         if file_content["media"]["track"]:
-        #             for track in file_content["media"]["track"]:
-        #                 if(track['@type'] == Argument.getoptionvalue('--type')):
-        #                     type = Argument.getoptionvalue('--type')
-        #                     for i in track:
-        #                         print(f"{i}  ==> {i} of the Source File")
-        #         else:
-        #             raise Exception("Unable to fetch the Tracks of your Source file")
-        #     except ValueError as e:
-        #         print(e)
+        elif Argument.getoptionvalue('--type') and  Argument.hasOption(['--options']):
+            file_content = json.loads(os.popen('mediainfo --Output=JSON '+Argument.getoptionvalue('-file')).read())
+            try:
+                if file_content["media"]["track"]:
+                    for track in file_content["media"]["track"]:
+                        if(track['@type'] == Argument.getoptionvalue('--type')):
+                            type = Argument.getoptionvalue('--type')
+                            for i in track:
+                                print(f"{i}  ==> {i} of the Source File")
+                else:
+                    raise Exception("Unable to fetch the Tracks of your Source file")
+            except ValueError as e:
+                print(e)
       
     else:
         help()
         
 if __name__ == "__main__":
     main()
```

