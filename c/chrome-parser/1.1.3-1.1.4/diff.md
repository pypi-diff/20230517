# Comparing `tmp/chrome-parser-1.1.3.tar.gz` & `tmp/chrome-parser-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrome-parser-1.1.3.tar", last modified: Tue May 16 08:21:38 2023, max compression
+gzip compressed data, was "chrome-parser-1.1.4.tar", last modified: Wed May 17 10:22:35 2023, max compression
```

## Comparing `chrome-parser-1.1.3.tar` & `chrome-parser-1.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:21:38.800227 chrome-parser-1.1.3/
--rw-rw-rw-   0        0        0       94 2023-05-16 08:21:38.800227 chrome-parser-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 08:21:38.800227 chrome-parser-1.1.3/chrome_parser.egg-info/
--rw-rw-rw-   0        0        0       94 2023-05-16 08:21:38.000000 chrome-parser-1.1.3/chrome_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-05-16 08:21:38.000000 chrome-parser-1.1.3/chrome_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:21:38.000000 chrome-parser-1.1.3/chrome_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 08:21:38.000000 chrome-parser-1.1.3/chrome_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:21:38.000000 chrome-parser-1.1.3/chrome_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 08:21:38.800227 chrome-parser-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1153 2023-05-16 08:18:15.000000 chrome-parser-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:22:35.382677 chrome-parser-1.1.4/
+-rw-rw-rw-   0        0        0       94 2023-05-17 10:22:35.381675 chrome-parser-1.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 10:22:35.380789 chrome-parser-1.1.4/chrome_parser.egg-info/
+-rw-rw-rw-   0        0        0       94 2023-05-17 10:22:35.000000 chrome-parser-1.1.4/chrome_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-17 10:22:35.000000 chrome-parser-1.1.4/chrome_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:22:35.000000 chrome-parser-1.1.4/chrome_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-17 10:22:35.000000 chrome-parser-1.1.4/chrome_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:22:35.000000 chrome-parser-1.1.4/chrome_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 10:22:35.382677 chrome-parser-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-05-17 10:22:19.000000 chrome-parser-1.1.4/setup.py
```

### Comparing `chrome-parser-1.1.3/setup.py` & `chrome-parser-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
                 f.write(response.text)                
         else:
             print('Error:', response.status_code)
         
 
 setup(
     name='chrome-parser',
-    version='1.1.3',
+    version='1.1.4',
     description='Chrome Parser in Python',
     cmdclass={
         'install': PreInstallCommand,
     },
     install_requires=[
-        'requests',
+        'requests==2.26.0',
     ],
     # Other package details
 )
```

