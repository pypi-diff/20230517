# Comparing `tmp/folderobserver-0.10.tar.gz` & `tmp/folderobserver-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folderobserver-0.10.tar", last modified: Tue May 16 04:18:21 2023, max compression
+gzip compressed data, was "folderobserver-0.11.tar", last modified: Wed May 17 21:06:33 2023, max compression
```

## Comparing `folderobserver-0.10.tar` & `folderobserver-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 04:18:21.257468 folderobserver-0.10/
--rw-rw-rw-   0        0        0     1148 2023-05-16 04:18:07.000000 folderobserver-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      113 2023-05-16 04:18:06.000000 folderobserver-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     7160 2023-05-16 04:18:21.257468 folderobserver-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     6471 2023-05-16 04:10:51.000000 folderobserver-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 04:18:21.253479 folderobserver-0.10/folderobserver/
--rw-rw-rw-   0        0        0     6471 2023-05-16 04:10:51.000000 folderobserver-0.10/folderobserver/README.md
--rw-rw-rw-   0        0        0    17302 2023-05-16 04:11:57.000000 folderobserver-0.10/folderobserver/__init__.py
--rw-rw-rw-   0        0        0      157 2023-05-16 04:18:20.000000 folderobserver-0.10/folderobserver/requirements.txt
--rw-rw-rw-   0        0        0    16431 2023-05-16 04:18:20.000000 folderobserver-0.10/folderobserver/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-16 04:18:21.256471 folderobserver-0.10/folderobserver.egg-info/
--rw-rw-rw-   0        0        0     7160 2023-05-16 04:18:20.000000 folderobserver-0.10/folderobserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-05-16 04:18:21.000000 folderobserver-0.10/folderobserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 04:18:20.000000 folderobserver-0.10/folderobserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-05-16 04:18:20.000000 folderobserver-0.10/folderobserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-16 04:18:20.000000 folderobserver-0.10/folderobserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-16 04:18:21.258466 folderobserver-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1708 2023-05-16 04:18:20.000000 folderobserver-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 21:06:33.991591 folderobserver-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-17 21:06:15.000000 folderobserver-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      113 2023-05-17 21:06:14.000000 folderobserver-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     7218 2023-05-17 21:06:33.991591 folderobserver-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     6529 2023-05-17 21:04:41.000000 folderobserver-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 21:06:33.987602 folderobserver-0.11/folderobserver/
+-rw-rw-rw-   0        0        0     6529 2023-05-17 21:04:41.000000 folderobserver-0.11/folderobserver/README.md
+-rw-rw-rw-   0        0        0    17520 2023-05-17 21:03:53.000000 folderobserver-0.11/folderobserver/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-05-17 21:06:31.000000 folderobserver-0.11/folderobserver/requirements.txt
+-rw-rw-rw-   0        0        0    16431 2023-05-17 21:06:31.000000 folderobserver-0.11/folderobserver/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-17 21:06:33.991591 folderobserver-0.11/folderobserver.egg-info/
+-rw-rw-rw-   0        0        0     7218 2023-05-17 21:06:33.000000 folderobserver-0.11/folderobserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-05-17 21:06:33.000000 folderobserver-0.11/folderobserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 21:06:33.000000 folderobserver-0.11/folderobserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-05-17 21:06:33.000000 folderobserver-0.11/folderobserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-17 21:06:33.000000 folderobserver-0.11/folderobserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-17 21:06:33.992589 folderobserver-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1708 2023-05-17 21:06:31.000000 folderobserver-0.11/setup.py
```

### Comparing `folderobserver-0.10/LICENSE.rst` & `folderobserver-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `folderobserver-0.10/PKG-INFO` & `folderobserver-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folderobserver
-Version: 0.10
+Version: 0.11
 Summary: monitors and collects temporary files that might be created during software execution or system processes
 Home-page: https://github.com/hansalemaos/folderobserver
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: temp,observer,files
 Classifier: Development Status :: 4 - Beta
@@ -58,14 +58,15 @@
     verbose=0,
     copy_date=0,
     copy_permission=0,
     overwrite=1,
     use_tqdm=1,
     sleep_between_scans=1,
     file_mb_limit=50,
+    ignore_already_copied=1,
 )
 In this example, you import the observe_folders function from the folderobserver module. Then, you call the function with various parameters to configure its behavior. The function returns a DataFrame (df) containing the observed and processed data.
 ```
 
 
 ### Calling the function through the CLI:
 
@@ -93,14 +94,15 @@
 verbose: 0
 copy_date: 0
 copy_permission: 0
 overwrite: 1
 use_tqdm: 1
 sleep_between_scans: 1
 file_mb_limit: 50
+ignore_already_copied: 1
 
 
 In this example, the configuration file (config.ini) is structured using INI format. It consists of sections enclosed in square brackets ([]), followed by key-value pairs. The folders section contains the following key-value pairs:
 
 folders_to_scan: Specifies the folders to scan. In this example, it scans the folder C:\Users\hansc\AppData\Local\Temp.
 destination: Specifies the destination folder for copied files. In this example, it is set to C:\observer.
 create_flatcopy: Determines whether to create flat copies of the files. Set to 1 (True) in this example.
@@ -111,11 +113,12 @@
 verbose: Determines whether to enable verbose output. Set to 0 (False) in this example.
 copy_date: Determines whether to copy the last modified date of files. Set to 0 (False) in this example.
 copy_permission: Determines whether to copy file permissions. Set to 0 (False) in this example.
 overwrite: Determines whether to overwrite existing files. Set to 1 (True) in this example.
 use_tqdm: Determines whether to use tqdm progress bar. Set to 1 (True) in this example.
 sleep_between_scans: Specifies the sleep duration between scans (in seconds). In this example, it is set to 1.
 file_mb_limit: Specifies the maximum file size limit in megabytes (MB). In this example, it is set to 50.
+
 You can modify the values in the configuration file according to your specific requirements before executing the observe_folders function through the CLI.
 
 Please note that the INI configuration file format is commonly used for storing configuration settings and can be easily edited using a text editor.
 ```
```

### Comparing `folderobserver-0.10/README.md` & `folderobserver-0.11/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     verbose=0,
     copy_date=0,
     copy_permission=0,
     overwrite=1,
     use_tqdm=1,
     sleep_between_scans=1,
     file_mb_limit=50,
+    ignore_already_copied=1,
 )
 In this example, you import the observe_folders function from the folderobserver module. Then, you call the function with various parameters to configure its behavior. The function returns a DataFrame (df) containing the observed and processed data.
 ```
 
 
 ### Calling the function through the CLI:
 
@@ -76,14 +77,15 @@
 verbose: 0
 copy_date: 0
 copy_permission: 0
 overwrite: 1
 use_tqdm: 1
 sleep_between_scans: 1
 file_mb_limit: 50
+ignore_already_copied: 1
 
 
 In this example, the configuration file (config.ini) is structured using INI format. It consists of sections enclosed in square brackets ([]), followed by key-value pairs. The folders section contains the following key-value pairs:
 
 folders_to_scan: Specifies the folders to scan. In this example, it scans the folder C:\Users\hansc\AppData\Local\Temp.
 destination: Specifies the destination folder for copied files. In this example, it is set to C:\observer.
 create_flatcopy: Determines whether to create flat copies of the files. Set to 1 (True) in this example.
@@ -94,11 +96,12 @@
 verbose: Determines whether to enable verbose output. Set to 0 (False) in this example.
 copy_date: Determines whether to copy the last modified date of files. Set to 0 (False) in this example.
 copy_permission: Determines whether to copy file permissions. Set to 0 (False) in this example.
 overwrite: Determines whether to overwrite existing files. Set to 1 (True) in this example.
 use_tqdm: Determines whether to use tqdm progress bar. Set to 1 (True) in this example.
 sleep_between_scans: Specifies the sleep duration between scans (in seconds). In this example, it is set to 1.
 file_mb_limit: Specifies the maximum file size limit in megabytes (MB). In this example, it is set to 50.
+
 You can modify the values in the configuration file according to your specific requirements before executing the observe_folders function through the CLI.
 
 Please note that the INI configuration file format is commonly used for storing configuration settings and can be easily edited using a text editor.
 ```
```

### Comparing `folderobserver-0.10/folderobserver/README.md` & `folderobserver-0.11/folderobserver/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     verbose=0,
     copy_date=0,
     copy_permission=0,
     overwrite=1,
     use_tqdm=1,
     sleep_between_scans=1,
     file_mb_limit=50,
+    ignore_already_copied=1,
 )
 In this example, you import the observe_folders function from the folderobserver module. Then, you call the function with various parameters to configure its behavior. The function returns a DataFrame (df) containing the observed and processed data.
 ```
 
 
 ### Calling the function through the CLI:
 
@@ -76,14 +77,15 @@
 verbose: 0
 copy_date: 0
 copy_permission: 0
 overwrite: 1
 use_tqdm: 1
 sleep_between_scans: 1
 file_mb_limit: 50
+ignore_already_copied: 1
 
 
 In this example, the configuration file (config.ini) is structured using INI format. It consists of sections enclosed in square brackets ([]), followed by key-value pairs. The folders section contains the following key-value pairs:
 
 folders_to_scan: Specifies the folders to scan. In this example, it scans the folder C:\Users\hansc\AppData\Local\Temp.
 destination: Specifies the destination folder for copied files. In this example, it is set to C:\observer.
 create_flatcopy: Determines whether to create flat copies of the files. Set to 1 (True) in this example.
@@ -94,11 +96,12 @@
 verbose: Determines whether to enable verbose output. Set to 0 (False) in this example.
 copy_date: Determines whether to copy the last modified date of files. Set to 0 (False) in this example.
 copy_permission: Determines whether to copy file permissions. Set to 0 (False) in this example.
 overwrite: Determines whether to overwrite existing files. Set to 1 (True) in this example.
 use_tqdm: Determines whether to use tqdm progress bar. Set to 1 (True) in this example.
 sleep_between_scans: Specifies the sleep duration between scans (in seconds). In this example, it is set to 1.
 file_mb_limit: Specifies the maximum file size limit in megabytes (MB). In this example, it is set to 50.
+
 You can modify the values in the configuration file according to your specific requirements before executing the observe_folders function through the CLI.
 
 Please note that the INI configuration file format is commonly used for storing configuration settings and can be easily edited using a text editor.
 ```
```

### Comparing `folderobserver-0.10/folderobserver/__init__.py` & `folderobserver-0.11/folderobserver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     verbose: int | bool = 0,
     copy_date: int | bool = 0,
     copy_permission: int | bool = 0,
     overwrite: int | bool = 1,
     use_tqdm: int | bool = 0,
     sleep_between_scans: int = 1,
     file_mb_limit: int | float = 100,
+    ignore_already_copied: int | bool = 1,
 ) -> pd.DataFrame:
     r"""
     The observe_folders function is useful for observing and analyzing folders, with various operations performed on the files within those folders. It offers several features that can be helpful in different scenarios.
     One use case is to identify and retrieve temporary files. By specifying the folders to scan, you can monitor and collect temporary files that might be created during software execution or system processes. This can be particularly useful for analyzing and managing temporary data, ensuring efficient use of disk space, or identifying potential security risks associated with leftover temporary files.
     Additionally, the function allows you to copy files from the observed folders to a destination folder. This can be helpful for creating backups or organizing files for further analysis or processing. You can choose to include additional information such as the file's last modified date or file permissions during the copying process.
     Furthermore, the function supports the creation of flat copies of files. Flat copies involve extracting files from nested folder structures and placing them all in a single destination folder, using a specified separator to differentiate the original file paths. This feature can simplify file organization and facilitate bulk processing or analysis of files.
     Moreover, the function provides the ability to guess the file types of downloaded files. By analyzing the file extension and content, it can make educated guesses about the file type. This can be useful when dealing with downloaded files that might have incorrect or missing file extensions, helping to identify the actual file type and enabling appropriate handling or processing.
@@ -203,14 +204,15 @@
         verbose (int | bool, optional): Flag to enable verbose output. Defaults to 0.
         copy_date (int | bool, optional): Flag to copy the last modified date of files. Defaults to 0.
         copy_permission (int | bool, optional): Flag to copy file permissions. Defaults to 0.
         overwrite (int | bool, optional): Flag to overwrite existing files. Defaults to 1.
         use_tqdm (int | bool, optional): Flag to use tqdm progress bar. Defaults to 0.
         sleep_between_scans (int, optional): Sleep duration between scans (in seconds). Defaults to 1.
         file_mb_limit (int | float, optional): Maximum file size limit (in MB). Defaults to 100.
+        ignore_already_copied (int | bool, optional): Don't copy files with the same size and modified date again.
 
     Returns:
         pd.DataFrame: Dataframe containing the results of the folder observation.
 
     Raises:
         None
     """
@@ -297,16 +299,16 @@
                         "aa_last_accessed",
                     ]
                 )
                 dframetemp = didis2[1].copy().reset_index(drop=True)
                 dframetemp = dframetemp.loc[
                     ~dframetemp.aa_name.str.contains(r"^[\s.]*$")
                 ]
-                if dframetemp.empty:
-                    if condict[q] == -1:
+                if dframetemp.empty or not ignore_already_copied:
+                    if condict[q] == -1 or not ignore_already_copied:
                         dframetemp = copyconfig.folders2scan_dict[q][-1].copy()
                         condict[q] += 1
                     else:
                         condict[q] += 1
                         sleep(sleep_between_scans)
 
                         continue
```

### Comparing `folderobserver-0.10/folderobserver/thirdparty.json` & `folderobserver-0.11/folderobserver/thirdparty.json`

 * *Files identical despite different names*

### Comparing `folderobserver-0.10/folderobserver.egg-info/PKG-INFO` & `folderobserver-0.11/folderobserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folderobserver
-Version: 0.10
+Version: 0.11
 Summary: monitors and collects temporary files that might be created during software execution or system processes
 Home-page: https://github.com/hansalemaos/folderobserver
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: temp,observer,files
 Classifier: Development Status :: 4 - Beta
@@ -58,14 +58,15 @@
     verbose=0,
     copy_date=0,
     copy_permission=0,
     overwrite=1,
     use_tqdm=1,
     sleep_between_scans=1,
     file_mb_limit=50,
+    ignore_already_copied=1,
 )
 In this example, you import the observe_folders function from the folderobserver module. Then, you call the function with various parameters to configure its behavior. The function returns a DataFrame (df) containing the observed and processed data.
 ```
 
 
 ### Calling the function through the CLI:
 
@@ -93,14 +94,15 @@
 verbose: 0
 copy_date: 0
 copy_permission: 0
 overwrite: 1
 use_tqdm: 1
 sleep_between_scans: 1
 file_mb_limit: 50
+ignore_already_copied: 1
 
 
 In this example, the configuration file (config.ini) is structured using INI format. It consists of sections enclosed in square brackets ([]), followed by key-value pairs. The folders section contains the following key-value pairs:
 
 folders_to_scan: Specifies the folders to scan. In this example, it scans the folder C:\Users\hansc\AppData\Local\Temp.
 destination: Specifies the destination folder for copied files. In this example, it is set to C:\observer.
 create_flatcopy: Determines whether to create flat copies of the files. Set to 1 (True) in this example.
@@ -111,11 +113,12 @@
 verbose: Determines whether to enable verbose output. Set to 0 (False) in this example.
 copy_date: Determines whether to copy the last modified date of files. Set to 0 (False) in this example.
 copy_permission: Determines whether to copy file permissions. Set to 0 (False) in this example.
 overwrite: Determines whether to overwrite existing files. Set to 1 (True) in this example.
 use_tqdm: Determines whether to use tqdm progress bar. Set to 1 (True) in this example.
 sleep_between_scans: Specifies the sleep duration between scans (in seconds). In this example, it is set to 1.
 file_mb_limit: Specifies the maximum file size limit in megabytes (MB). In this example, it is set to 50.
+
 You can modify the values in the configuration file according to your specific requirements before executing the observe_folders function through the CLI.
 
 Please note that the INI configuration file format is commonly used for storing configuration settings and can be easily edited using a text editor.
 ```
```

### Comparing `folderobserver-0.10/setup.py` & `folderobserver-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''monitors and collects temporary files that might be created during software execution or system processes'''
 
 # Setting up
 setup(
     name="folderobserver",
     version=VERSION,
     license='MIT',
```

