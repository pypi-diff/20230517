# Comparing `tmp/xmesh-0.4.0.tar.gz` & `tmp/xmesh-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmesh-0.4.0.tar", last modified: Mon May  8 13:41:22 2023, max compression
+gzip compressed data, was "xmesh-0.4.1.tar", last modified: Wed May 17 01:47:15 2023, max compression
```

## Comparing `xmesh-0.4.0.tar` & `xmesh-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-08 13:41:22.214871 xmesh-0.4.0/
--rw-r--r--   0 snowyang   (501) staff       (20)    11357 2022-09-16 03:55:08.000000 xmesh-0.4.0/LICENSE
--rw-r--r--   0 snowyang   (501) staff       (20)      984 2023-05-08 13:41:22.214933 xmesh-0.4.0/PKG-INFO
--rw-r--r--   0 snowyang   (501) staff       (20)      508 2022-09-16 03:55:08.000000 xmesh-0.4.0/README.md
--rw-r--r--   0 snowyang   (501) staff       (20)      104 2022-09-16 03:55:08.000000 xmesh-0.4.0/pyproject.toml
--rw-r--r--   0 snowyang   (501) staff       (20)      768 2023-05-08 13:41:22.215208 xmesh-0.4.0/setup.cfg
-drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-08 13:41:22.213019 xmesh-0.4.0/src/
-drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-08 13:41:22.213747 xmesh-0.4.0/src/xmesh/
--rw-r--r--   0 snowyang   (501) staff       (20)        0 2022-09-16 03:55:08.000000 xmesh-0.4.0/src/xmesh/__init__.py
--rw-r--r--   0 snowyang   (501) staff       (20)    35686 2023-05-08 13:40:36.000000 xmesh-0.4.0/src/xmesh/main.py
-drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-08 13:41:22.214769 xmesh-0.4.0/src/xmesh.egg-info/
--rw-r--r--   0 snowyang   (501) staff       (20)      984 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/PKG-INFO
--rw-r--r--   0 snowyang   (501) staff       (20)      282 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/SOURCES.txt
--rw-r--r--   0 snowyang   (501) staff       (20)        1 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/dependency_links.txt
--rw-r--r--   0 snowyang   (501) staff       (20)       42 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/entry_points.txt
--rw-r--r--   0 snowyang   (501) staff       (20)       14 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/requires.txt
--rw-r--r--   0 snowyang   (501) staff       (20)        6 2023-05-08 13:41:22.000000 xmesh-0.4.0/src/xmesh.egg-info/top_level.txt
+drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-17 01:47:15.965216 xmesh-0.4.1/
+-rw-r--r--   0 snowyang   (501) staff       (20)    11357 2022-09-16 03:55:08.000000 xmesh-0.4.1/LICENSE
+-rw-r--r--   0 snowyang   (501) staff       (20)      984 2023-05-17 01:47:15.965361 xmesh-0.4.1/PKG-INFO
+-rw-r--r--   0 snowyang   (501) staff       (20)      508 2022-09-16 03:55:08.000000 xmesh-0.4.1/README.md
+-rw-r--r--   0 snowyang   (501) staff       (20)      104 2022-09-16 03:55:08.000000 xmesh-0.4.1/pyproject.toml
+-rw-r--r--   0 snowyang   (501) staff       (20)      768 2023-05-17 01:47:15.965761 xmesh-0.4.1/setup.cfg
+drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-17 01:47:15.962028 xmesh-0.4.1/src/
+drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-17 01:47:15.963116 xmesh-0.4.1/src/xmesh/
+-rw-r--r--   0 snowyang   (501) staff       (20)        0 2022-09-16 03:55:08.000000 xmesh-0.4.1/src/xmesh/__init__.py
+-rw-r--r--   0 snowyang   (501) staff       (20)    35755 2023-05-17 01:46:31.000000 xmesh-0.4.1/src/xmesh/main.py
+drwxr-xr-x   0 snowyang   (501) staff       (20)        0 2023-05-17 01:47:15.964704 xmesh-0.4.1/src/xmesh.egg-info/
+-rw-r--r--   0 snowyang   (501) staff       (20)      984 2023-05-17 01:47:15.000000 xmesh-0.4.1/src/xmesh.egg-info/PKG-INFO
+-rw-r--r--   0 snowyang   (501) staff       (20)      282 2023-05-17 01:47:15.000000 xmesh-0.4.1/src/xmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 snowyang   (501) staff       (20)        1 2023-05-17 01:47:15.000000 xmesh-0.4.1/src/xmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 snowyang   (501) staff       (20)       42 2023-05-17 01:47:15.000000 xmesh-0.4.1/src/xmesh.egg-info/entry_points.txt
+-rw-r--r--   0 snowyang   (501) staff       (20)       14 2023-05-17 01:47:15.000000 xmesh-0.4.1/src/xmesh.egg-info/requires.txt
+-rw-r--r--   0 snowyang   (501) staff       (20)        6 2023-05-17 01:47:15.000000 xmesh-0.4.1/src/xmesh.egg-info/top_level.txt
```

### Comparing `xmesh-0.4.0/LICENSE` & `xmesh-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmesh-0.4.0/PKG-INFO` & `xmesh-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmesh
-Version: 0.4.0
+Version: 0.4.1
 Summary: xMesh sniffer.
 Home-page: https://github.com/smartsnow/xmesh
 Author: Snow Yang
 Author-email: snowyang.iot@outlook.com
 Project-URL: Bug Tracker, https://github.com/smartsnow/xmesh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xmesh-0.4.0/setup.cfg` & `xmesh-0.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xmesh
-version = 0.4.0
+version = 0.4.1
 author = Snow Yang
 author_email = snowyang.iot@outlook.com
 description = xMesh sniffer.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/smartsnow/xmesh
 project_urls =
```

### Comparing `xmesh-0.4.0/src/xmesh/main.py` & `xmesh-0.4.1/src/xmesh/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,15 @@
             ports = [port.device for port in portslist if 'MX0101' in port.device]
         elif type == 'proxy':
             ports = [port.device for port in portslist if port.device == '/dev/cu.usbserial-MX0201']
         elif type == 'cli':
             ports = [port.device for port in portslist if port.device == '/dev/cu.usbserial-MX0301']
     else:
         if type == 'sniffer':
-            ports = [port.device for port in portslist if port.serial_number == 'MX0101']
+            ports = [port.device for port in portslist if 'MX0101' in port.serial_number]
         elif type == 'proxy':
             ports = [port.device for port in portslist if port.serial_number == 'MX0201']
         elif type == 'cli':
             ports = [port.device for port in portslist if port.serial_number == 'MX0301']
 
     if len(ports) == 0:
       sys.stderr.write('ERROR: Dongle was not found!\n')
@@ -920,18 +920,19 @@
     miniterm.raw = True
     miniterm.set_rx_encoding('UTF-8')
     miniterm.set_tx_encoding('UTF-8')
     miniterm.type = args.type
 
     print(Panel.fit(
 f'''
-Hotkeys:
- - Exit         Ctrl + ]
- - Configure    Ctrl + R
- - Start        Ctrl + F''', title=f'xMesh Assistant v{get_distribution("xmesh").version}', style='green'))
+快捷键:
+  Ctrl + ]      退出
+  Ctrl + R      重启（并进入配置模式）    
+  Ctrl + F      启动抓包/扫描
+  Ctrl + N      切换模式''', title=f'xMesh Assistant v{get_distribution("xmesh").version}', style='green'))
 
     miniterm.start()
     try:
         miniterm.join(True)
     except KeyboardInterrupt:
         pass
     sys.stderr.write('\n--- exit ---\n')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xmesh-0.4.0/src/xmesh.egg-info/PKG-INFO` & `xmesh-0.4.1/src/xmesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmesh
-Version: 0.4.0
+Version: 0.4.1
 Summary: xMesh sniffer.
 Home-page: https://github.com/smartsnow/xmesh
 Author: Snow Yang
 Author-email: snowyang.iot@outlook.com
 Project-URL: Bug Tracker, https://github.com/smartsnow/xmesh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

