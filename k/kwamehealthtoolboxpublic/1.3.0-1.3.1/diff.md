# Comparing `tmp/kwamehealthtoolboxpublic-1.3.0.tar.gz` & `tmp/kwamehealthtoolboxpublic-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwamehealthtoolboxpublic-1.3.0.tar", last modified: Wed May 17 02:55:39 2023, max compression
+gzip compressed data, was "kwamehealthtoolboxpublic-1.3.1.tar", last modified: Wed May 17 03:10:00 2023, max compression
```

## Comparing `kwamehealthtoolboxpublic-1.3.0.tar` & `kwamehealthtoolboxpublic-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 02:55:39.689786 kwamehealthtoolboxpublic-1.3.0/
--rw-rw-rw-   0        0        0     1220 2023-05-17 02:55:39.689786 kwamehealthtoolboxpublic-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      835 2023-03-15 09:38:11.000000 kwamehealthtoolboxpublic-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 02:55:39.623450 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/
--rw-rw-rw-   0        0        0        0 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/__init__.py
--rw-rw-rw-   0        0        0     2754 2023-03-15 09:30:17.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/createDocument.py
--rw-rw-rw-   0        0        0      876 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/getDateTime.py
--rw-rw-rw-   0        0        0    19681 2023-05-17 02:53:25.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/sendEmail.py
-drwxrwxrwx   0        0        0        0 2023-05-17 02:55:39.687632 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/
--rw-rw-rw-   0        0        0     1220 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-17 02:55:39.000000 kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      649 2023-05-17 02:54:20.000000 kwamehealthtoolboxpublic-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 02:55:39.689786 kwamehealthtoolboxpublic-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      724 2023-05-17 02:54:38.000000 kwamehealthtoolboxpublic-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:10:00.006398 kwamehealthtoolboxpublic-1.3.1/
+-rw-rw-rw-   0        0        0     1220 2023-05-17 03:10:00.005409 kwamehealthtoolboxpublic-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2023-03-15 09:38:11.000000 kwamehealthtoolboxpublic-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 03:09:59.974398 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic/
+-rw-rw-rw-   0        0        0        0 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic/__init__.py
+-rw-rw-rw-   0        0        0     2754 2023-03-15 09:30:17.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic/createDocument.py
+-rw-rw-rw-   0        0        0      876 2023-03-15 09:24:05.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic/getDateTime.py
+-rw-rw-rw-   0        0        0    19945 2023-05-17 03:08:17.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic/sendEmail.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:10:00.004402 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-05-17 03:09:59.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-05-17 03:09:59.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 03:09:59.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-17 03:09:59.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-17 03:09:59.000000 kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      649 2023-05-17 03:09:53.000000 kwamehealthtoolboxpublic-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 03:10:00.006398 kwamehealthtoolboxpublic-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-05-17 03:09:47.000000 kwamehealthtoolboxpublic-1.3.1/setup.py
```

### Comparing `kwamehealthtoolboxpublic-1.3.0/PKG-INFO` & `kwamehealthtoolboxpublic-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwamehealthtoolboxpublic
-Version: 1.3.0
+Version: 1.3.1
 Summary: Toolbox with custom functions
 Home-page: https://github.com/Kwame-Health/khtoolbox
 Author: Panashe Madzudzo
 Author-email: admin@kwame.health
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Kwame-Health/khtoolbox/issues
 Platform: UNKNOWN
```

### Comparing `kwamehealthtoolboxpublic-1.3.0/README.md` & `kwamehealthtoolboxpublic-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/createDocument.py` & `kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic/createDocument.py`

 * *Files identical despite different names*

### Comparing `kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/getDateTime.py` & `kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic/getDateTime.py`

 * *Files identical despite different names*

### Comparing `kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic/sendEmail.py` & `kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic/sendEmail.py`

 * *Files 8% similar despite different names*

```diff
@@ -400,38 +400,44 @@
     EMAIL_FROM = config.emailFrom
     EMAIL_TO = email
     password = config.password
     doNotReplyEmail = config.doNotReplyEmail
 
     if emailType == "NOTIFICATION":
         subject = service_name+" Notification"
+        subjectMain = subject
         EMAIL_BODY = data
         EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
 
     elif emailType == "ERROR_NOTIFICATION":
-        subject = service_name+" Error Notification"
-        EMAIL_BODY = """<p style="color:right">"""+data+"""</p>"""
+        subject = """<div style="color:red;">"""+service_name+" Error Notification"+"""</div>"""
+        subjectMain = subject
+        EMAIL_BODY = """<p style="color:red;">"""+data+"""</p>"""
         EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
 
     elif emailType == "NOTIFICATION_PATIENT_ADDED":
+        subjectMain = subject
         EMAIL_BODY = data
         EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
 
     elif emailType == "LETTER":
         subject = service_name+" "+data[0]
+        subjectMain = subject
         EMAIL_BODY = data[1]
         EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
 
     elif emailType == "referralLetter":
         subject = service_name+" Letter (Referrer): "+data[0]
+        subjectMain = subject
         EMAIL_BODY = data[1]
         EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
 
     elif emailType == "ACCOUNT-ADDED":
         subject = service_name+": Account Added"
+        subjectMain = subject
         EMAIL_BODY = """
             <p>Welcome """ + str(data["firstName"]) + """. You have been added to the """+str(service_name)+""" Dashboard</strong></p>
             <p>Please click the button below to activate your account</p>
             <p>Your login credentials to use after activation:</p>
             <p><strong>Username:</strong> """ + str(data["username"]) + """</p>
             <p><strong>Password:</strong> """ + str(data["password"]) + """</p>
             <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary">
@@ -456,14 +462,15 @@
         """
         EMAIL_BODY += """<br><br>Contact us at """+str(support_email)+""" for any assistance</p>"""
 
     else:
         first_name = data[0]
         active = data[1]
         subject = "Welcome "+str(first_name)+"...Start Your First Campaign with MusaEMR!"
+        subjectMain = subject
         EMAIL_BODY = """
             <p>Welcome """ + str(first_name) + """</strong></p>
             <p>Please click the button below to login to your account</p>
             <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary">
                 <tbody>
                     <tr>
                         <td align="center">
@@ -572,15 +579,15 @@
             </table>
     </body>
     </html>
     """
     msg_html_content = MIMEText(EMAIL_CONTENT, "html", "utf-8")
 
     msg = MIMEMultipart("alternative")
-    msg["Subject"] = Header(subject, "utf-8").encode()
+    msg["Subject"] = Header(subjectMain, "utf-8").encode()
     msg["From"] = str(fromName+" "+doNotReplyEmail) #this can change name from e.g. do-not-reply
     msg["To"] = EMAIL_TO
     msg['CC'] = ",".join(ccEmails)
     msg.attach(msg_html_content)
 
     if emailType == "LETTER" or emailType == "referralLetter":
         fileBytes = data[2]
```

### Comparing `kwamehealthtoolboxpublic-1.3.0/kwamehealthtoolboxpublic.egg-info/PKG-INFO` & `kwamehealthtoolboxpublic-1.3.1/kwamehealthtoolboxpublic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwamehealthtoolboxpublic
-Version: 1.3.0
+Version: 1.3.1
 Summary: Toolbox with custom functions
 Home-page: https://github.com/Kwame-Health/khtoolbox
 Author: Panashe Madzudzo
 Author-email: admin@kwame.health
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Kwame-Health/khtoolbox/issues
 Platform: UNKNOWN
```

### Comparing `kwamehealthtoolboxpublic-1.3.0/pyproject.toml` & `kwamehealthtoolboxpublic-1.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pyproject.toml
 name = "kwamehealthtoolboxpublic"
 description = "Kwame Health toolbox (public) with custom functions"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
     { name = "Panashe Madzudzo", email = "admin@kwame.health" }
 ]
 
 [build-system]
 requires = ["setuptools==58.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `kwamehealthtoolboxpublic-1.3.0/setup.py` & `kwamehealthtoolboxpublic-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages, __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="kwamehealthtoolboxpublic",
-    version="1.3.0",
+    version="1.3.1",
     author="Panashe Madzudzo",
     author_email="admin@kwame.health",
     description="Toolbox with custom functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kwame-Health/khtoolbox",
     project_urls = {
```

