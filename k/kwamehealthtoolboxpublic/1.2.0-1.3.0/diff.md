# Comparing `tmp/kwamehealthtoolboxpublic-1.2.0.tar.gz` & `tmp/kwamehealthtoolboxpublic-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwamehealthtoolboxpublic-1.2.0.tar", last modified: Wed Mar 15 09:36:51 2023, max compression
+gzip compressed data, was "kwamehealthtoolboxpublic-1.3.0.tar", last modified: Wed May 17 02:55:39 2023, max compression
```

## Comparing `kwamehealthtoolboxpublic-1.2.0.tar` & `kwamehealthtoolboxpublic-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 09:36:51.756408 kwamehealthtoolboxpublic-1.2.0/
--rw-rw-rw-   0        0        0     1233 2023-03-15 09:36:51.753410 kwamehealthtoolboxpublic-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      835 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 09:36:51.734402 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic/
--rw-rw-rw-   0        0        0        0 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic/__init__.py
--rw-rw-rw-   0        0        0     2754 2023-03-15 09:30:17.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic/createDocument.py
--rw-rw-rw-   0        0        0      876 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic/getDateTime.py
--rw-rw-rw-   0        0        0    19411 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic/sendEmail.py
-drwxrwxrwx   0        0        0        0 2023-03-15 09:36:51.751410 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic.egg-info/
--rw-rw-rw-   0        0        0     1233 2023-03-15 09:36:51.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-03-15 09:36:51.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 09:36:51.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-03-15 09:36:51.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-03-15 09:36:51.000000 kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      649 2023-03-15 09:36:04.000000 kwamehealthtoolboxpublic-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-15 09:36:51.756408 kwamehealthtoolboxpublic-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-03-15 09:36:16.000000 kwamehealthtoolboxpublic-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:55:39.689786 kwamehealthtoolboxpublic-1.3.0/
+-rw-rw-rw-   0        0        0     1220 2023-05-17 02:55:39.689786 kwamehealthtoolboxpublic-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2023-03-15 09:38:11.000000 kwamehealthtoolboxpublic-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 02:55:39.623450 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/
+-rw-rw-rw-   0        0        0        0 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/__init__.py
+-rw-rw-rw-   0        0        0     2754 2023-03-15 09:30:17.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/createDocument.py
+-rw-rw-rw-   0        0        0      876 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/getDateTime.py
+-rw-rw-rw-   0        0        0    19681 2023-05-17 02:53:25.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/sendEmail.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:55:39.687632 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      649 2023-05-17 02:54:20.000000 kwamehealthtoolboxpublic-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 02:55:39.689786 kwamehealthtoolboxpublic-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-05-17 02:54:38.000000 kwamehealthtoolboxpublic-1.3.0/setup.py
```

### Comparing `kwamehealthtoolboxpublic-1.2.0/PKG-INFO` & `kwamehealthtoolboxpublic-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kwamehealthtoolboxpublic
-Version: 1.2.0
-Summary: Kwame Health toolbox with custom functions
+Version: 1.3.0
+Summary: Toolbox with custom functions
 Home-page: https://github.com/Kwame-Health/khtoolbox
 Author: Panashe Madzudzo
 Author-email: admin@kwame.health
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Kwame-Health/khtoolbox/issues
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `kwamehealthtoolboxpublic-1.2.0/README.md` & `kwamehealthtoolboxpublic-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic/createDocument.py` & `kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/createDocument.py`

 * *Files identical despite different names*

### Comparing `kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic/getDateTime.py` & `kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/getDateTime.py`

 * *Files identical despite different names*

### Comparing `kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic/sendEmail.py` & `kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/sendEmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,14 +403,19 @@
     doNotReplyEmail = config.doNotReplyEmail
 
     if emailType == "NOTIFICATION":
         subject = service_name+" Notification"
         EMAIL_BODY = data
         EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
 
+    elif emailType == "ERROR_NOTIFICATION":
+        subject = service_name+" Error Notification"
+        EMAIL_BODY = """<p style="color:right">"""+data+"""</p>"""
+        EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
+
     elif emailType == "NOTIFICATION_PATIENT_ADDED":
         EMAIL_BODY = data
         EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
 
     elif emailType == "LETTER":
         subject = service_name+" "+data[0]
         EMAIL_BODY = data[1]
```

### Comparing `kwamehealthtoolboxpublic-1.2.0/kwamehealthtoolboxpublic.egg-info/PKG-INFO` & `kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kwamehealthtoolboxpublic
-Version: 1.2.0
-Summary: Kwame Health toolbox with custom functions
+Version: 1.3.0
+Summary: Toolbox with custom functions
 Home-page: https://github.com/Kwame-Health/khtoolbox
 Author: Panashe Madzudzo
 Author-email: admin@kwame.health
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Kwame-Health/khtoolbox/issues
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `kwamehealthtoolboxpublic-1.2.0/pyproject.toml` & `kwamehealthtoolboxpublic-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pyproject.toml
 name = "kwamehealthtoolboxpublic"
 description = "Kwame Health toolbox (public) with custom functions"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
     { name = "Panashe Madzudzo", email = "admin@kwame.health" }
 ]
 
 [build-system]
 requires = ["setuptools==58.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `kwamehealthtoolboxpublic-1.2.0/setup.py` & `kwamehealthtoolboxpublic-1.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages, __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="kwamehealthtoolboxpublic",
-    version="1.2.0",
+    version="1.3.0",
     author="Panashe Madzudzo",
     author_email="admin@kwame.health",
-    description="Kwame Health toolbox with custom functions",
+    description="Toolbox with custom functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kwame-Health/khtoolbox",
     project_urls = {
         "Bug Tracker": "https://github.com/Kwame-Health/khtoolbox/issues"
     },
     packages=["kwamehealthtoolboxpublic"],
```

