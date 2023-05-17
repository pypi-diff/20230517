# Comparing `tmp/bloodyAD-1.0.1.tar.gz` & `tmp/bloodyAD-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloodyAD-1.0.1.tar", last modified: Wed Apr 19 12:34:00 2023, max compression
+gzip compressed data, was "bloodyAD-1.0.2.tar", last modified: Wed May 17 12:32:15 2023, max compression
```

## Comparing `bloodyAD-1.0.1.tar` & `bloodyAD-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/
--rwxrwx---   0 silver    (1000) silver    (1001)     1068 2022-09-07 15:23:19.000000 bloodyAD-1.0.1/LICENSE
--rw-r--r--   0 silver    (1000) silver    (1001)     7763 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/PKG-INFO
--rw-r--r--   0 silver    (1000) silver    (1001)     7016 2023-04-17 09:41:24.000000 bloodyAD-1.0.1/README.md
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/
--rw-r--r--   0 silver    (1000) silver    (1001)      108 2023-03-28 10:43:06.000000 bloodyAD-1.0.1/bloodyAD/__init__.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/cli_modules/
--rw-r--r--   0 silver    (1000) silver    (1001)        0 2022-12-26 08:53:44.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/__init__.py
--rw-r--r--   0 silver    (1000) silver    (1001)    16389 2023-04-19 11:41:32.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/add.py
--rw-r--r--   0 silver    (1000) silver    (1001)    10912 2023-04-19 11:40:41.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/get.py
--rw-r--r--   0 silver    (1000) silver    (1001)     9087 2023-04-19 11:40:41.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/remove.py
--rw-r--r--   0 silver    (1000) silver    (1001)     3332 2023-04-16 20:41:09.000000 bloodyAD-1.0.1/bloodyAD/cli_modules/set.py
--rw-r--r--   0 silver    (1000) silver    (1001)     1920 2023-03-18 13:00:15.000000 bloodyAD-1.0.1/bloodyAD/exceptions.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/formatters/
--rw-r--r--   0 silver    (1000) silver    (1001)        0 2023-02-10 15:42:23.000000 bloodyAD-1.0.1/bloodyAD/formatters/__init__.py
--rw-r--r--   0 silver    (1000) silver    (1001)     5952 2023-04-12 13:41:14.000000 bloodyAD-1.0.1/bloodyAD/formatters/accesscontrol.py
--rw-r--r--   0 silver    (1000) silver    (1001)   118418 2023-04-16 20:41:10.000000 bloodyAD-1.0.1/bloodyAD/formatters/adschema.py
--rw-r--r--   0 silver    (1000) silver    (1001)     2594 2023-04-16 20:41:09.000000 bloodyAD-1.0.1/bloodyAD/formatters/common.py
--rw-r--r--   0 silver    (1000) silver    (1001)     5021 2023-04-19 11:40:41.000000 bloodyAD-1.0.1/bloodyAD/formatters/cryptography.py
--rw-r--r--   0 silver    (1000) silver    (1001)     8547 2023-04-16 20:24:41.000000 bloodyAD-1.0.1/bloodyAD/formatters/dns.py
--rw-r--r--   0 silver    (1000) silver    (1001)     1771 2023-04-17 09:30:32.000000 bloodyAD-1.0.1/bloodyAD/formatters/formatters.py
--rw-r--r--   0 silver    (1000) silver    (1001)     2016 2023-04-16 20:41:10.000000 bloodyAD-1.0.1/bloodyAD/formatters/helpers.py
--rw-r--r--   0 silver    (1000) silver    (1001)    16246 2023-03-18 13:05:44.000000 bloodyAD-1.0.1/bloodyAD/formatters/ldaptypes.py
--rw-r--r--   0 silver    (1000) silver    (1001)    23266 2023-01-16 17:02:26.000000 bloodyAD-1.0.1/bloodyAD/formatters/structure.py
--rwxrwx---   0 silver    (1000) silver    (1001)   486395 2023-03-18 13:06:07.000000 bloodyAD-1.0.1/bloodyAD/formatters/winerror.py
--rwxr-xr-x   0 silver    (1000) silver    (1001)     7019 2023-04-19 11:40:41.000000 bloodyAD-1.0.1/bloodyAD/main.py
--rw-r--r--   0 silver    (1000) silver    (1001)     3950 2023-02-08 15:01:35.000000 bloodyAD-1.0.1/bloodyAD/md4.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/network/
--rw-r--r--   0 silver    (1000) silver    (1001)     2537 2023-03-18 13:00:15.000000 bloodyAD-1.0.1/bloodyAD/network/config.py
--rw-r--r--   0 silver    (1000) silver    (1001)     8680 2023-04-16 20:57:57.000000 bloodyAD-1.0.1/bloodyAD/network/ldap.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD/patch/
--rw-r--r--   0 silver    (1000) silver    (1001)    47840 2023-03-18 13:05:45.000000 bloodyAD-1.0.1/bloodyAD/patch/ldap3_patch.py
--rw-r--r--   0 silver    (1000) silver    (1001)    16673 2023-04-17 19:14:34.000000 bloodyAD-1.0.1/bloodyAD/utils.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/bloodyAD.egg-info/
--rw-r--r--   0 silver    (1000) silver    (1001)     7763 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/PKG-INFO
--rw-r--r--   0 silver    (1000) silver    (1001)      902 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/SOURCES.txt
--rw-r--r--   0 silver    (1000) silver    (1001)        1 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/dependency_links.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       48 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/entry_points.txt
--rw-r--r--   0 silver    (1000) silver    (1001)      190 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/requires.txt
--rw-r--r--   0 silver    (1000) silver    (1001)        9 2023-04-19 12:34:00.000000 bloodyAD-1.0.1/bloodyAD.egg-info/top_level.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       38 2023-04-19 12:34:00.854369 bloodyAD-1.0.1/setup.cfg
--rw-r--r--   0 silver    (1000) silver    (1001)     1365 2023-04-19 11:40:34.000000 bloodyAD-1.0.1/setup.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-05-17 12:32:15.666422 bloodyAD-1.0.2/
+-rwxrwx---   0 silver    (1000) silver    (1001)     1068 2022-09-07 15:23:19.000000 bloodyAD-1.0.2/LICENSE
+-rw-r--r--   0 silver    (1000) silver    (1001)     7763 2023-05-17 12:32:15.666422 bloodyAD-1.0.2/PKG-INFO
+-rw-r--r--   0 silver    (1000) silver    (1001)     7016 2023-04-17 09:41:24.000000 bloodyAD-1.0.2/README.md
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-05-17 12:32:15.663089 bloodyAD-1.0.2/bloodyAD/
+-rw-r--r--   0 silver    (1000) silver    (1001)      108 2023-03-28 10:43:06.000000 bloodyAD-1.0.2/bloodyAD/__init__.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-05-17 12:32:15.663089 bloodyAD-1.0.2/bloodyAD/cli_modules/
+-rw-r--r--   0 silver    (1000) silver    (1001)        0 2022-12-26 08:53:44.000000 bloodyAD-1.0.2/bloodyAD/cli_modules/__init__.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16389 2023-04-19 11:41:32.000000 bloodyAD-1.0.2/bloodyAD/cli_modules/add.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    11000 2023-05-17 12:25:16.000000 bloodyAD-1.0.2/bloodyAD/cli_modules/get.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     9087 2023-04-19 11:40:41.000000 bloodyAD-1.0.2/bloodyAD/cli_modules/remove.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     3332 2023-04-16 20:41:09.000000 bloodyAD-1.0.2/bloodyAD/cli_modules/set.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     1920 2023-03-18 13:00:15.000000 bloodyAD-1.0.2/bloodyAD/exceptions.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-05-17 12:32:15.666422 bloodyAD-1.0.2/bloodyAD/formatters/
+-rw-r--r--   0 silver    (1000) silver    (1001)        0 2023-02-10 15:42:23.000000 bloodyAD-1.0.2/bloodyAD/formatters/__init__.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     5952 2023-04-12 13:41:14.000000 bloodyAD-1.0.2/bloodyAD/formatters/accesscontrol.py
+-rw-r--r--   0 silver    (1000) silver    (1001)   118425 2023-05-17 12:30:18.000000 bloodyAD-1.0.2/bloodyAD/formatters/adschema.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     2594 2023-04-16 20:41:09.000000 bloodyAD-1.0.2/bloodyAD/formatters/common.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     5021 2023-04-19 11:40:41.000000 bloodyAD-1.0.2/bloodyAD/formatters/cryptography.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     8547 2023-04-16 20:24:41.000000 bloodyAD-1.0.2/bloodyAD/formatters/dns.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     1771 2023-04-17 09:30:32.000000 bloodyAD-1.0.2/bloodyAD/formatters/formatters.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     2016 2023-04-16 20:41:10.000000 bloodyAD-1.0.2/bloodyAD/formatters/helpers.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16246 2023-03-18 13:05:44.000000 bloodyAD-1.0.2/bloodyAD/formatters/ldaptypes.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    23266 2023-01-16 17:02:26.000000 bloodyAD-1.0.2/bloodyAD/formatters/structure.py
+-rwxrwx---   0 silver    (1000) silver    (1001)   486395 2023-03-18 13:06:07.000000 bloodyAD-1.0.2/bloodyAD/formatters/winerror.py
+-rwxr-xr-x   0 silver    (1000) silver    (1001)     7019 2023-04-19 11:40:41.000000 bloodyAD-1.0.2/bloodyAD/main.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     3950 2023-02-08 15:01:35.000000 bloodyAD-1.0.2/bloodyAD/md4.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-05-17 12:32:15.666422 bloodyAD-1.0.2/bloodyAD/network/
+-rw-r--r--   0 silver    (1000) silver    (1001)     2537 2023-03-18 13:00:15.000000 bloodyAD-1.0.2/bloodyAD/network/config.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     8680 2023-04-16 20:57:57.000000 bloodyAD-1.0.2/bloodyAD/network/ldap.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-05-17 12:32:15.666422 bloodyAD-1.0.2/bloodyAD/patch/
+-rw-r--r--   0 silver    (1000) silver    (1001)    47840 2023-03-18 13:05:45.000000 bloodyAD-1.0.2/bloodyAD/patch/ldap3_patch.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16728 2023-05-17 12:30:17.000000 bloodyAD-1.0.2/bloodyAD/utils.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-05-17 12:32:15.663089 bloodyAD-1.0.2/bloodyAD.egg-info/
+-rw-r--r--   0 silver    (1000) silver    (1001)     7763 2023-05-17 12:32:15.000000 bloodyAD-1.0.2/bloodyAD.egg-info/PKG-INFO
+-rw-r--r--   0 silver    (1000) silver    (1001)      902 2023-05-17 12:32:15.000000 bloodyAD-1.0.2/bloodyAD.egg-info/SOURCES.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)        1 2023-05-17 12:32:15.000000 bloodyAD-1.0.2/bloodyAD.egg-info/dependency_links.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       48 2023-05-17 12:32:15.000000 bloodyAD-1.0.2/bloodyAD.egg-info/entry_points.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)      190 2023-05-17 12:32:15.000000 bloodyAD-1.0.2/bloodyAD.egg-info/requires.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)        9 2023-05-17 12:32:15.000000 bloodyAD-1.0.2/bloodyAD.egg-info/top_level.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       38 2023-05-17 12:32:15.666422 bloodyAD-1.0.2/setup.cfg
+-rw-r--r--   0 silver    (1000) silver    (1001)     1365 2023-05-17 12:30:14.000000 bloodyAD-1.0.2/setup.py
```

### Comparing `bloodyAD-1.0.1/LICENSE` & `bloodyAD-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/PKG-INFO` & `bloodyAD-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bloodyAD
-Version: 1.0.1
+Version: 1.0.2
 Summary: AD Privesc Swiss Army Knife
 Home-page: https://github.com/CravateRouge/bloodyAD
-Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.2.tar.gz
 Author: CravateRouge
 Author-email: baptiste.crepin@ntymail.com
 License: MIT
 Keywords: Active Directory,Privilege Escalation
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bloodyAD-1.0.1/README.md` & `bloodyAD-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/cli_modules/add.py` & `bloodyAD-1.0.2/bloodyAD/cli_modules/add.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/cli_modules/get.py` & `bloodyAD-1.0.2/bloodyAD/cli_modules/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,16 @@
             generator=True,
         ):
             for attr_name in entry:
                 if attr_name not in attr_params:
                     continue
                 key_names = attr_params[attr_name]["lambda"](entry[attr_name])
                 for name in key_names:
+                    if name == "distinguishedName":
+                        name = "dn"
                     if name not in right_entry:
                         right_entry[name] = []
                     right_entry[name].append(attr_params[attr_name]["right"])
 
             if right_entry:
                 yield {
                     **{"distinguishedName": entry["distinguishedName"]},
```

### Comparing `bloodyAD-1.0.1/bloodyAD/cli_modules/remove.py` & `bloodyAD-1.0.2/bloodyAD/cli_modules/remove.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/cli_modules/set.py` & `bloodyAD-1.0.2/bloodyAD/cli_modules/set.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/exceptions.py` & `bloodyAD-1.0.2/bloodyAD/exceptions.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/accesscontrol.py` & `bloodyAD-1.0.2/bloodyAD/formatters/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/adschema.py` & `bloodyAD-1.0.2/bloodyAD/formatters/adschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1801,14 +1801,14 @@
     "bf967ab7-0de6-11d0-a285-00aa003049e2": "Top",
     "bf967ab8-0de6-11d0-a285-00aa003049e2": "Trusted-Domain",
     "281416e2-1968-11d0-a28f-00aa003049e2": "Type-Library",
     "bf967aba-0de6-11d0-a285-00aa003049e2": "User",
     "bf967abb-0de6-11d0-a285-00aa003049e2": "Volume",
 }
 
-OBJECT_TYPES = (
-    VALIDATED_RIGHTS
-    | CONTROL_ACCESS_RIGHTS
-    | PROPERTY_SETS
-    | SCHEMA_ATTRIBUTES
-    | SCHEMA_CLASSES
-)
+OBJECT_TYPES = {
+    **VALIDATED_RIGHTS,
+    **CONTROL_ACCESS_RIGHTS,
+    **PROPERTY_SETS,
+    **SCHEMA_ATTRIBUTES,
+    **SCHEMA_CLASSES,
+}
```

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/common.py` & `bloodyAD-1.0.2/bloodyAD/formatters/common.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/cryptography.py` & `bloodyAD-1.0.2/bloodyAD/formatters/cryptography.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/dns.py` & `bloodyAD-1.0.2/bloodyAD/formatters/dns.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/formatters.py` & `bloodyAD-1.0.2/bloodyAD/formatters/formatters.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/helpers.py` & `bloodyAD-1.0.2/bloodyAD/formatters/helpers.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/ldaptypes.py` & `bloodyAD-1.0.2/bloodyAD/formatters/ldaptypes.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/structure.py` & `bloodyAD-1.0.2/bloodyAD/formatters/structure.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/formatters/winerror.py` & `bloodyAD-1.0.2/bloodyAD/formatters/winerror.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/main.py` & `bloodyAD-1.0.2/bloodyAD/main.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/md4.py` & `bloodyAD-1.0.2/bloodyAD/md4.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/network/config.py` & `bloodyAD-1.0.2/bloodyAD/network/config.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/network/ldap.py` & `bloodyAD-1.0.2/bloodyAD/network/ldap.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/patch/ldap3_patch.py` & `bloodyAD-1.0.2/bloodyAD/patch/ldap3_patch.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/bloodyAD/utils.py` & `bloodyAD-1.0.2/bloodyAD/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,52 +247,53 @@
 
 
 class Control:
     def __init__(self, control_enum):
         self.control_enum = control_enum
 
     def __str__(self):
-        flag_str = str(self.control_enum).split(".")[1]
+        flag_str = repr(self.control_enum).split(".")[1].split(":")[0]
         flag_str = flag_str.replace("SE_", "")
         return flag_str
 
 
 class AceType:
     def __init__(self, acetype_enum):
         self.acetype_enum = acetype_enum
 
     def __eq__(self, o):
         if not isinstance(o, AceType):
             return NotImplemented
         return self.acetype_enum == o.acetype_enum
 
     def __str__(self):
-        flag_str = str(self.acetype_enum).split(".")[1]
+        flag_str = repr(self.acetype_enum).split(".")[1].split(":")[0]
         flag_str = flag_str.replace("ACCESS_", "")
         flag_str = flag_str.replace("SYSTEM_", "")
         flag_str = flag_str.replace("_ACE_TYPE", "")
         return f"== {flag_str} =="
 
 
 class AceFlag:
     def __init__(self, aceflag_enum):
         self.aceflag_enum = aceflag_enum
 
     def __str__(self):
-        flag_str = str(self.aceflag_enum).split(".")[1]
+        flag_str = repr(self.aceflag_enum).split(".")[1].split(":")[0]
         flag_str = flag_str.replace("_ACE_FLAG", "")
         flag_str = flag_str.replace("_ACE", "")
         return flag_str
 
 
 class LazyAdSchema:
     guids = set()
     sids = set()
-    guid_dict = adschema.OBJECT_TYPES | {
-        "Self": "Self"
+    guid_dict = {
+        **adschema.OBJECT_TYPES,
+        "Self": "Self",
     }  # Special object to design rule applies to self
     sid_dict = dtyp.sid.well_known_sids_sid_name_map
     isResolved = False
 
     def _resolveAll(self):
         if self.isResolved:
             return
```

### Comparing `bloodyAD-1.0.1/bloodyAD.egg-info/PKG-INFO` & `bloodyAD-1.0.2/bloodyAD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bloodyAD
-Version: 1.0.1
+Version: 1.0.2
 Summary: AD Privesc Swiss Army Knife
 Home-page: https://github.com/CravateRouge/bloodyAD
-Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.1.tar.gz
+Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.2.tar.gz
 Author: CravateRouge
 Author-email: baptiste.crepin@ntymail.com
 License: MIT
 Keywords: Active Directory,Privilege Escalation
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bloodyAD-1.0.1/bloodyAD.egg-info/SOURCES.txt` & `bloodyAD-1.0.2/bloodyAD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bloodyAD-1.0.1/setup.py` & `bloodyAD-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="bloodyAD",
-    version="1.0.1",
+    version="1.0.2",
     description="AD Privesc Swiss Army Knife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="CravateRouge",
     author_email="baptiste.crepin@ntymail.com",
     url="https://github.com/CravateRouge/bloodyAD",
     download_url=(
-        "https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.1.tar.gz"
+        "https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.2.tar.gz"
     ),
     license="MIT",
     install_requires=[
         "cryptography>=37.0.2",
         "ldap3>=2.9.1",
         "winacl>=0.1.7",
         'gssapi>=1.8.1 ; platform_system=="Linux" or platform_system=="Darwin"',
```

