# Comparing `tmp/find_old_large_files-0.2.1.tar.gz` & `tmp/find_old_large_files-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find_old_large_files-0.2.1.tar", last modified: Wed May 17 21:27:02 2023, max compression
+gzip compressed data, was "find_old_large_files-0.2.2.tar", last modified: Wed May 17 21:38:17 2023, max compression
```

## Comparing `find_old_large_files-0.2.1.tar` & `find_old_large_files-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:27:02.492610 find_old_large_files-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 21:26:46.000000 find_old_large_files-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 21:27:02.492610 find_old_large_files-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-17 21:26:46.000000 find_old_large_files-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:27:02.492610 find_old_large_files-0.2.1/find_old_large_files/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 21:26:46.000000 find_old_large_files-0.2.1/find_old_large_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-17 21:26:46.000000 find_old_large_files-0.2.1/find_old_large_files/find_old_large_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:27:02.492610 find_old_large_files-0.2.1/find_old_large_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 21:27:02.000000 find_old_large_files-0.2.1/find_old_large_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-17 21:27:02.000000 find_old_large_files-0.2.1/find_old_large_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:27:02.000000 find_old_large_files-0.2.1/find_old_large_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 21:27:02.000000 find_old_large_files-0.2.1/find_old_large_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 21:27:02.000000 find_old_large_files-0.2.1/find_old_large_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 21:27:02.000000 find_old_large_files-0.2.1/find_old_large_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:27:02.492610 find_old_large_files-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-17 21:26:46.000000 find_old_large_files-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:38:17.445464 find_old_large_files-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 21:38:17.445464 find_old_large_files-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:38:17.441464 find_old_large_files-0.2.2/find_old_large_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/find_old_large_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/find_old_large_files/find_old_large_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:38:17.445464 find_old_large_files-0.2.2/find_old_large_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 21:38:17.000000 find_old_large_files-0.2.2/find_old_large_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:38:17.445464 find_old_large_files-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-17 21:38:00.000000 find_old_large_files-0.2.2/setup.py
```

### Comparing `find_old_large_files-0.2.1/LICENSE` & `find_old_large_files-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.2.1/PKG-INFO` & `find_old_large_files-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find_old_large_files
-Version: 0.2.1
+Version: 0.2.2
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.2.1/README.md` & `find_old_large_files-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `find_old_large_files-0.2.1/find_old_large_files/find_old_large_files.py` & `find_old_large_files-0.2.2/find_old_large_files/find_old_large_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,17 @@
                     if (os.path.getsize(file_path) > self.size_limit and
                         self.file_age_in_days(file_path) > self.days_limit and
                         not Path(file_path).suffix in self.excluded_extensions):
                         self.files_to_move.append(file_path)  # Add to files to be moved
                         if file_handler is not None:
                             file_handler(file_path)
                 except FileNotFoundError:
-                    print(f"File not found: {file_path}, skipping.")
-
+                    #print(f"File not found: {file_path}, skipping.")
+                    pass
+                
     def move_files_to_trash(self):
         os.makedirs(self.trash_dir, exist_ok=True)
         with tqdm(total=len(self.files_to_move), desc='Moving files', ncols=70) as pbar:
             for file_path in self.files_to_move:
                 os.rename(file_path, os.path.join(self.trash_dir, os.path.basename(file_path)))
                 pbar.update()
```

### Comparing `find_old_large_files-0.2.1/find_old_large_files.egg-info/PKG-INFO` & `find_old_large_files-0.2.2/find_old_large_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: find-old-large-files
-Version: 0.2.1
+Version: 0.2.2
 Summary: A utility to find and remove large, old files.
 Home-page: http://github.com/PrinceDisant/find_old_large_files
 Author: Disant Upadhyay
 Author-email: disantupadhyay07@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `find_old_large_files-0.2.1/setup.py` & `find_old_large_files-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="find_old_large_files",
-    version="0.2.1",  # Increment the version here
+    version="0.2.2",  # Increment the version here
     packages=find_packages(),
     install_requires=["tqdm"],
     entry_points={
         'console_scripts': [
             'find_old_large_files=find_old_large_files:run',
         ],
     },
```

