# Comparing `tmp/FileInfo_Video_Audio-0.0.5.tar.gz` & `tmp/FileInfo_Video_Audio-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileInfo_Video_Audio-0.0.5.tar", last modified: Mon May 15 11:54:53 2023, max compression
+gzip compressed data, was "FileInfo_Video_Audio-0.1.0.tar", last modified: Wed May 17 10:57:22 2023, max compression
```

## Comparing `FileInfo_Video_Audio-0.0.5.tar` & `FileInfo_Video_Audio-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-15 11:54:53.888154 FileInfo_Video_Audio-0.0.5/
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-15 11:54:53.888154 FileInfo_Video_Audio-0.0.5/FileInfo_Video_Audio.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1474 2023-05-15 11:54:53.000000 FileInfo_Video_Audio-0.0.5/FileInfo_Video_Audio.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-15 11:54:53.000000 FileInfo_Video_Audio-0.0.5/FileInfo_Video_Audio.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-15 11:54:53.000000 FileInfo_Video_Audio-0.0.5/FileInfo_Video_Audio.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-15 11:54:53.000000 FileInfo_Video_Audio-0.0.5/FileInfo_Video_Audio.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-15 11:54:53.000000 FileInfo_Video_Audio-0.0.5/FileInfo_Video_Audio.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1474 2023-05-15 11:54:53.888154 FileInfo_Video_Audio-0.0.5/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1103 2023-05-15 11:52:16.000000 FileInfo_Video_Audio-0.0.5/README.md
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-15 11:54:53.888154 FileInfo_Video_Audio-0.0.5/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      816 2023-05-15 11:54:18.000000 FileInfo_Video_Audio-0.0.5/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-15 11:54:53.888154 FileInfo_Video_Audio-0.0.5/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:26:11.000000 FileInfo_Video_Audio-0.0.5/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-15 11:54:53.888154 FileInfo_Video_Audio-0.0.5/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.0.5/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.0.5/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3957 2023-05-15 11:49:26.000000 FileInfo_Video_Audio-0.0.5/source/main.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1498 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-17 10:57:22.000000 FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1498 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1127 2023-05-17 10:56:40.000000 FileInfo_Video_Audio-0.1.0/README.md
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      816 2023-05-17 10:56:49.000000 FileInfo_Video_Audio-0.1.0/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-14 18:26:11.000000 FileInfo_Video_Audio-0.1.0/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-17 10:57:22.251906 FileInfo_Video_Audio-0.1.0/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.1.0/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-14 14:25:10.000000 FileInfo_Video_Audio-0.1.0/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3957 2023-05-15 11:49:26.000000 FileInfo_Video_Audio-0.1.0/source/main.py
```

### Comparing `FileInfo_Video_Audio-0.0.5/FileInfo_Video_Audio.egg-info/PKG-INFO` & `FileInfo_Video_Audio-0.1.0/FileInfo_Video_Audio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: FileInfo-Video-Audio
-Version: 0.0.5
+Version: 0.1.0
 Summary: In this tool is help to get the properties of the Audio and Video files
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-## A  Wrapper for mediainfo tool
+## GetFileinfo_Audio_Video A  Wrapper for mediainfo tool
 
 #### Prerequisites
 
 This tool needs mediainfo to be installed inorder to work properly.
 
 On Ubuntu/Debian:
```

### Comparing `FileInfo_Video_Audio-0.0.5/PKG-INFO` & `FileInfo_Video_Audio-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: FileInfo_Video_Audio
-Version: 0.0.5
+Version: 0.1.0
 Summary: In this tool is help to get the properties of the Audio and Video files
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-## A  Wrapper for mediainfo tool
+## GetFileinfo_Audio_Video A  Wrapper for mediainfo tool
 
 #### Prerequisites
 
 This tool needs mediainfo to be installed inorder to work properly.
 
 On Ubuntu/Debian:
```

### Comparing `FileInfo_Video_Audio-0.0.5/README.md` & `FileInfo_Video_Audio-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## A  Wrapper for mediainfo tool
+## GetFileinfo_Audio_Video A  Wrapper for mediainfo tool
 
 #### Prerequisites
 
 This tool needs mediainfo to be installed inorder to work properly.
 
 On Ubuntu/Debian:
```

### Comparing `FileInfo_Video_Audio-0.0.5/setup.py` & `FileInfo_Video_Audio-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = os.popen("/usr/local/bin/pipreqs main --print").read().splitlines()
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='FileInfo_Video_Audio',
-    version='0.0.5',
+    version='0.1.0',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
     description="In this tool is help to get the properties of the Audio and Video files",
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details',
     install_requires=requirements,
     long_description=long_description,
```

### Comparing `FileInfo_Video_Audio-0.0.5/source/lib/Argument.py` & `FileInfo_Video_Audio-0.1.0/source/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `FileInfo_Video_Audio-0.0.5/source/main.py` & `FileInfo_Video_Audio-0.1.0/source/main.py`

 * *Files identical despite different names*

