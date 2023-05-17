# Comparing `tmp/filesystem-dict-0.1.4.tar.gz` & `tmp/filesystem-dict-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filesystem-dict-0.1.4.tar", last modified: Wed May 17 09:45:25 2023, max compression
+gzip compressed data, was "filesystem-dict-0.1.5.tar", last modified: Wed May 17 12:22:50 2023, max compression
```

## Comparing `filesystem-dict-0.1.4.tar` & `filesystem-dict-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/
--rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-15 20:22:54.000000 filesystem-dict-0.1.4/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      834 2023-05-17 08:45:31.000000 filesystem-dict-0.1.4/README.md
--rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-15 20:55:49.000000 filesystem-dict-0.1.4/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 09:45:25.521004 filesystem-dict-0.1.4/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-17 09:45:25.000000 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-17 09:45:25.000000 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-17 09:45:25.000000 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-17 09:45:25.000000 filesystem-dict-0.1.4/src/filesystem_dict.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 09:45:25.524337 filesystem-dict-0.1.4/src/fsdict/
--rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-16 07:52:47.000000 filesystem-dict-0.1.4/src/fsdict/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5021 2023-05-17 09:43:21.000000 filesystem-dict-0.1.4/src/fsdict/fsdict.py
--rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-16 08:07:12.000000 filesystem-dict-0.1.4/src/fsdict/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:22:50.439175 filesystem-dict-0.1.5/
+-rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-15 20:22:54.000000 filesystem-dict-0.1.5/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-17 12:22:50.439175 filesystem-dict-0.1.5/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      834 2023-05-17 08:45:31.000000 filesystem-dict-0.1.5/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-17 12:22:50.439175 filesystem-dict-0.1.5/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-15 20:55:49.000000 filesystem-dict-0.1.5/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:22:50.439175 filesystem-dict-0.1.5/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:22:50.439175 filesystem-dict-0.1.5/src/filesystem_dict.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-17 12:22:50.000000 filesystem-dict-0.1.5/src/filesystem_dict.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-17 12:22:50.000000 filesystem-dict-0.1.5/src/filesystem_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-17 12:22:50.000000 filesystem-dict-0.1.5/src/filesystem_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-17 12:22:50.000000 filesystem-dict-0.1.5/src/filesystem_dict.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 12:22:50.439175 filesystem-dict-0.1.5/src/fsdict/
+-rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-16 07:52:47.000000 filesystem-dict-0.1.5/src/fsdict/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5056 2023-05-17 12:21:54.000000 filesystem-dict-0.1.5/src/fsdict/fsdict.py
+-rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-16 08:07:12.000000 filesystem-dict-0.1.5/src/fsdict/utils.py
```

### Comparing `filesystem-dict-0.1.4/LICENSE.txt` & `filesystem-dict-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.4/PKG-INFO` & `filesystem-dict-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.4
+Version: 0.1.5
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
```

### Comparing `filesystem-dict-0.1.4/README.md` & `filesystem-dict-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.4/src/filesystem_dict.egg-info/PKG-INFO` & `filesystem-dict-0.1.5/src/filesystem_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.4
+Version: 0.1.5
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
```

### Comparing `filesystem-dict-0.1.4/src/fsdict/fsdict.py` & `filesystem-dict-0.1.5/src/fsdict/fsdict.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,20 @@
         self.path = Path(path) if path else None
         self.overwrite = overwrite
         if self.path != None:
             if not self.path.exists():
                 self.path.mkdir()
             assert self.path.is_dir()
 
+    def __contains__(self, key):
+        assert not self.dangling()
+        assert isinstance(key, str)
+        key_path = self.__get_path(key)
+        return key_path.exists()
+
     def __getitem__(self, selector):
         assert not self.dangling()
         if isinstance(selector, str):
             return self.__get_item(selector)
         elif isinstance(selector, types.FunctionType):
             return self.__get_items(selector)
 
@@ -118,19 +124,14 @@
                 continue
             if lazy:
                 dictionary[key] = LazyValue(key_path)
             else:
                 dictionary[key] = self[key]
         return dictionary
 
-    def has_key(self, key):
-        assert not self.dangling()
-        key_path = self.__get_path(key)
-        return key_path.exists()
-
     def keys(self, lazy=False):
         assert not self.dangling()
         keys = (keypath.name for keypath in self.__get_paths())
         if lazy:
             return keys
         else:
             return list(keys)
@@ -160,11 +161,11 @@
 
     def __get_paths(self):
         assert not self.dangling()
         return self.path.glob("*")
 
     def __is_fsdict(self, key):
         assert not self.dangling()
-        if not self.has_key(key):
+        if not key in self:
             raise KeyError(key)
         key_path = self.path / key
         return key_path.is_dir()
```

### Comparing `filesystem-dict-0.1.4/src/fsdict/utils.py` & `filesystem-dict-0.1.5/src/fsdict/utils.py`

 * *Files identical despite different names*

