# Comparing `tmp/spswarehouse-0.1.0.tar.gz` & `tmp/spswarehouse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse-0.1.0.tar", last modified: Mon May  8 23:35:07 2023, max compression
+gzip compressed data, was "spswarehouse-0.1.1.tar", last modified: Tue May  9 16:10:50 2023, max compression
```

## Comparing `spswarehouse-0.1.0.tar` & `spswarehouse-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:35:07.814081 spswarehouse-0.1.0/
--rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8200 2023-05-08 23:35:07.812086 spswarehouse-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 23:35:07.814081 spswarehouse-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-05-08 23:34:09.000000 spswarehouse-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:35:07.797666 spswarehouse-0.1.0/spswarehouse/
--rw-rw-rw-   0        0        0      576 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/__init__.py
--rw-rw-rw-   0        0        0    28240 2023-05-08 23:04:57.000000 spswarehouse-0.1.0/spswarehouse/calpads.py
--rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.1.0/spswarehouse/credentials.py.template
--rw-rw-rw-   0        0        0     2037 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/googledrive.py
--rw-rw-rw-   0        0        0     1923 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/googlesheets.py
--rw-rw-rw-   0        0        0     1957 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/googleslides.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:35:07.810128 spswarehouse-0.1.0/spswarehouse/powerschool/
--rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.1.0/spswarehouse/powerschool/__init__.py
--rw-rw-rw-   0        0        0    19518 2023-05-08 23:32:25.000000 spswarehouse-0.1.0/spswarehouse/powerschool/powerschool.py
--rw-rw-rw-   0        0        0    25294 2023-05-08 22:51:29.000000 spswarehouse-0.1.0/spswarehouse/powerschool/powerschool_calpads.py
--rw-rw-rw-   0        0        0      300 2023-05-08 22:51:29.000000 spswarehouse-0.1.0/spswarehouse/requirements.txt
--rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/table_names.py
--rw-rw-rw-   0        0        0     7878 2023-01-04 22:56:50.000000 spswarehouse-0.1.0/spswarehouse/table_utils.py
--rw-rw-rw-   0        0        0     4685 2022-12-01 20:45:52.000000 spswarehouse-0.1.0/spswarehouse/warehouse.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:35:07.804854 spswarehouse-0.1.0/spswarehouse.egg-info/
--rw-rw-rw-   0        0        0     8200 2023-05-08 23:35:07.000000 spswarehouse-0.1.0/spswarehouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2023-05-08 23:35:07.000000 spswarehouse-0.1.0/spswarehouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:35:07.000000 spswarehouse-0.1.0/spswarehouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 23:35:07.000000 spswarehouse-0.1.0/spswarehouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 16:10:50.132898 spswarehouse-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8200 2023-05-09 16:10:50.131790 spswarehouse-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 16:10:50.133780 spswarehouse-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-05-09 16:09:22.000000 spswarehouse-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:10:50.105562 spswarehouse-0.1.1/spswarehouse/
+-rw-rw-rw-   0        0        0      561 2023-05-09 15:39:49.000000 spswarehouse-0.1.1/spswarehouse/__init__.py
+-rw-rw-rw-   0        0        0    28358 2023-05-09 15:44:44.000000 spswarehouse-0.1.1/spswarehouse/calpads.py
+-rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.1.1/spswarehouse/credentials.py.template
+-rw-rw-rw-   0        0        0     2090 2023-05-09 15:48:20.000000 spswarehouse-0.1.1/spswarehouse/googledrive.py
+-rw-rw-rw-   0        0        0     1980 2023-05-09 15:48:34.000000 spswarehouse-0.1.1/spswarehouse/googlesheets.py
+-rw-rw-rw-   0        0        0     2013 2023-05-09 15:50:01.000000 spswarehouse-0.1.1/spswarehouse/googleslides.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:10:50.128343 spswarehouse-0.1.1/spswarehouse/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.1.1/spswarehouse/powerschool/__init__.py
+-rw-rw-rw-   0        0        0    19636 2023-05-09 15:45:15.000000 spswarehouse-0.1.1/spswarehouse/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0    25294 2023-05-08 22:51:29.000000 spswarehouse-0.1.1/spswarehouse/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0      300 2023-05-08 22:51:29.000000 spswarehouse-0.1.1/spswarehouse/requirements.txt
+-rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.1.1/spswarehouse/table_names.py
+-rw-rw-rw-   0        0        0     7809 2023-05-09 15:47:54.000000 spswarehouse-0.1.1/spswarehouse/table_utils.py
+-rw-rw-rw-   0        0        0     4689 2023-05-09 15:45:39.000000 spswarehouse-0.1.1/spswarehouse/warehouse.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:10:50.118886 spswarehouse-0.1.1/spswarehouse.egg-info/
+-rw-rw-rw-   0        0        0     8200 2023-05-09 16:10:49.000000 spswarehouse-0.1.1/spswarehouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2023-05-09 16:10:49.000000 spswarehouse-0.1.1/spswarehouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 16:10:49.000000 spswarehouse-0.1.1/spswarehouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-09 16:10:49.000000 spswarehouse-0.1.1/spswarehouse.egg-info/top_level.txt
```

### Comparing `spswarehouse-0.1.0/LICENSE` & `spswarehouse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.1.0/PKG-INFO` & `spswarehouse-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.1.0
+Version: 0.1.1
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.1.0/README.md` & `spswarehouse-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.1.0/setup.py` & `spswarehouse-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spswarehouse",
-    version="0.1.0",
+    version="0.1.1",
     author="Summit Public Schools; Harry Li Consulting, LLC",
     author_email="warehouse@summitps.org",
     description="Summit Public Schools Snowflake warehouse",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SummitPublicSchools/spswarehouse",
     packages=setuptools.find_packages(),
```

### Comparing `spswarehouse-0.1.0/spswarehouse/__init__.py` & `spswarehouse-0.1.1/spswarehouse/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pandas as pd
-import numpy as np
-import seaborn as sns
-
-from sqlalchemy import *
-from sqlalchemy.sql import label, select, literal_column
-from sqlalchemy.sql.expression import cast
-
-import datetime
-
-now = datetime.datetime.now
-timedelta = datetime.timedelta
-
-# from .googlesheets import GoogleSheets, get_google_service_account_email
-# from .warehouse import describe, Warehouse
-# from .table_names import public, wild_west
-
-from matplotlib import pyplot
-
-# To avoid missing font warnings, set a default font that exists
-sns.set(font="DejaVu Sans")
+import pandas as pd
+import numpy as np
+# import seaborn as sns
+
+from sqlalchemy import *
+from sqlalchemy.sql import label, select, literal_column
+from sqlalchemy.sql.expression import cast
+
+import datetime
+
+now = datetime.datetime.now
+timedelta = datetime.timedelta
+
+# from .googlesheets import GoogleSheets, get_google_service_account_email
+# from .warehouse import describe, Warehouse
+# from .table_names import public, wild_west
+
+# from matplotlib import pyplot
+
+# To avoid missing font warnings, set a default font that exists
+# sns.set(font="DejaVu Sans")
```

### Comparing `spswarehouse-0.1.0/spswarehouse/calpads.py` & `spswarehouse-0.1.1/spswarehouse/calpads.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 from selenium.common.exceptions import (
     TimeoutException,
     NoSuchElementException,
     ElementNotInteractableException
 )
 
 from ducttape.utils import DriverBuilder
-from .credentials import calpads_config
+try:
+    from .credentials import calpads_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
 
 class CALPADS():
     
     def __init__(
         self,
         config=None,
         username=None,
```

### Comparing `spswarehouse-0.1.0/spswarehouse/credentials.py.template` & `spswarehouse-0.1.1/spswarehouse/credentials.py.template`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.1.0/spswarehouse/googledrive.py` & `spswarehouse-0.1.1/spswarehouse/googleslides.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import os
-import pickle
-
-from .credentials import google_config
-
-from pydrive2.auth import GoogleAuth
-from pydrive2.drive import GoogleDrive
-
-from oauth2client.service_account import ServiceAccountCredentials
-
-def get_google_service_account_email():
-    """
-    Returns the service account email to share Drive files with.
-    """
-    return google_config['service-account']['client_email']
-
-def initialize_credentials():
-    """
-    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
-
-    Returns credentials that allows you to access your Google Drive &
-    Sheets using the Google Sheets API.
-
-    You still need to share spreadsheets with the service account email.
-    """
-
-    # This prevents us from erroring out trying to construct credentials
-    # from incomplete information.
-    service_account = google_config.get('service-account', {})
-    private_key = service_account.get('private_key', None)
-    if not private_key:
-        print(
-            "You're missing Google service account credentials",
-            "in credentials.py.",
-            "To access your Google Drive data,",
-            "fill out the Google service account information."
-        )
-        return None
-
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
-        google_config['service-account'],
-        scopes=google_config['scopes'],
-    )
-    print(
-        'To access your Google Drive file, share the file with {email}'
-        .format(email=get_google_service_account_email())
-    )
-    return credentials
-
-def create_client(credentials):
-    """
-    create_engine:
-
-    Sets up Google Drive API access using credentials (see above).
-    """
-    gauth = GoogleAuth()
-    gauth.credentials = credentials
-    drive = GoogleDrive(gauth)
-    return drive
-
-# Set up credentials
-credentials = initialize_credentials()
-
-# This is a wrapper for pydrive.GoogleDrive
-GoogleDrive = None if credentials is None else create_client(credentials)
+import os
+import pickle
+
+try:
+    from .credentials import google_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from googleapiclient.discovery import build
+
+from oauth2client.service_account import ServiceAccountCredentials
+
+def get_google_service_account_email():
+    """
+    Returns the service account email to share slides with.
+    """
+    return google_config['service-account']['client_email']
+
+def initialize_credentials():
+    """
+    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
+
+    Returns credentials that allows you to access your Google Slides
+    using the Google Sheets API.
+
+    You still need to share slides with the service account email.
+    """
+
+    # This prevents us from erroring out trying to construct credentials
+    # from incomplete information.
+    service_account = google_config.get('service-account', {})
+    private_key = service_account.get('private_key', None)
+    if not private_key:
+        print(
+            "You're missing Google service account credentials",
+            "in credentials.py.",
+            "To access your Google Slides,",
+            "fill out the Google service account information."
+        )
+        return None
+
+    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
+        google_config['service-account'],
+        scopes=google_config['scopes'],
+    )
+    print(
+        'To access your Google Slides, share the file with {email}'
+        .format(email=get_google_service_account_email())
+    )
+    return credentials
+
+def create_client(credentials):
+    """
+    create_engine:
+
+    Sets up Google Drive API access using credentials (see above).
+    """
+    slides = build('slides', 'v1', credentials=credentials)
+    return slides
+
+# Set up credentials
+credentials = initialize_credentials()
+
+# This is a wrapper for a standard Google Slides engine
+GoogleSlides = None if credentials is None else create_client(credentials)
```

### Comparing `spswarehouse-0.1.0/spswarehouse/googlesheets.py` & `spswarehouse-0.1.1/spswarehouse/googlesheets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-import gspread
-import os
-import pickle
-
-from .credentials import google_config
-
-from oauth2client.service_account import ServiceAccountCredentials
-
-def get_google_service_account_email():
-    """
-    Returns the service account email to share spreadsheets with.
-    """
-    return google_config['service-account']['client_email']
-
-def initialize_credentials():
-    """
-    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
-
-    Returns credentials that allows you to access your Google Drive &
-    Sheets using the Google Sheets API.
-
-    You still need to share spreadsheets with the service account email.
-    """
-
-    # This prevents us from erroring out trying to construct credentials
-    # from incomplete information.
-    service_account = google_config.get('service-account', {})
-    private_key = service_account.get('private_key', None)
-    if not private_key:
-        print(
-            "You're missing Google service account credentials",
-            "in credentials.py.",
-            "To access your Google spreadsheet data,",
-            "fill out the Google service account information."
-        )
-        return None
-
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
-        google_config['service-account'],
-        scopes=google_config['scopes'],
-    )
-    print(
-        'To access your Google files, share the file with {email}'
-        .format(email=get_google_service_account_email())
-    )
-    return credentials
-
-def create_client(credentials):
-    """
-    create_engine:
-
-    Sets up Google Sheets API access using credentials (see above).
-    """
-    client = gspread.authorize(credentials)
-    return client
-
-# Set up credentials
-credentials = initialize_credentials()
-
-# This is a wrapper for gspread.Client
-GoogleSheets = None if credentials is None else create_client(credentials)
+import gspread
+import os
+import pickle
+
+try:
+    from .credentials import google_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from oauth2client.service_account import ServiceAccountCredentials
+
+def get_google_service_account_email():
+    """
+    Returns the service account email to share spreadsheets with.
+    """
+    return google_config['service-account']['client_email']
+
+def initialize_credentials():
+    """
+    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
+
+    Returns credentials that allows you to access your Google Drive &
+    Sheets using the Google Sheets API.
+
+    You still need to share spreadsheets with the service account email.
+    """
+
+    # This prevents us from erroring out trying to construct credentials
+    # from incomplete information.
+    service_account = google_config.get('service-account', {})
+    private_key = service_account.get('private_key', None)
+    if not private_key:
+        print(
+            "You're missing Google service account credentials",
+            "in credentials.py.",
+            "To access your Google spreadsheet data,",
+            "fill out the Google service account information."
+        )
+        return None
+
+    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
+        google_config['service-account'],
+        scopes=google_config['scopes'],
+    )
+    print(
+        'To access your Google files, share the file with {email}'
+        .format(email=get_google_service_account_email())
+    )
+    return credentials
+
+def create_client(credentials):
+    """
+    create_engine:
+
+    Sets up Google Sheets API access using credentials (see above).
+    """
+    client = gspread.authorize(credentials)
+    return client
+
+# Set up credentials
+credentials = initialize_credentials()
+
+# This is a wrapper for gspread.Client
+GoogleSheets = None if credentials is None else create_client(credentials)
```

### Comparing `spswarehouse-0.1.0/spswarehouse/googleslides.py` & `spswarehouse-0.1.1/spswarehouse/googledrive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,68 @@
-import os
-import pickle
-
-from .credentials import google_config
-
-from googleapiclient.discovery import build
-
-from oauth2client.service_account import ServiceAccountCredentials
-
-def get_google_service_account_email():
-    """
-    Returns the service account email to share slides with.
-    """
-    return google_config['service-account']['client_email']
-
-def initialize_credentials():
-    """
-    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
-
-    Returns credentials that allows you to access your Google Slides
-    using the Google Sheets API.
-
-    You still need to share slides with the service account email.
-    """
-
-    # This prevents us from erroring out trying to construct credentials
-    # from incomplete information.
-    service_account = google_config.get('service-account', {})
-    private_key = service_account.get('private_key', None)
-    if not private_key:
-        print(
-            "You're missing Google service account credentials",
-            "in credentials.py.",
-            "To access your Google Slides,",
-            "fill out the Google service account information."
-        )
-        return None
-
-    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
-        google_config['service-account'],
-        scopes=google_config['scopes'],
-    )
-    print(
-        'To access your Google Slides, share the file with {email}'
-        .format(email=get_google_service_account_email())
-    )
-    return credentials
-
-def create_client(credentials):
-    """
-    create_engine:
-
-    Sets up Google Drive API access using credentials (see above).
-    """
-    slides = build('slides', 'v1', credentials=credentials)
-    return slides
-
-# Set up credentials
-credentials = initialize_credentials()
-
-# This is a wrapper for a standard Google Slides engine
-GoogleSlides = None if credentials is None else create_client(credentials)
+import os
+import pickle
+
+try:
+    from .credentials import google_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+
+from pydrive2.auth import GoogleAuth
+from pydrive2.drive import GoogleDrive
+
+from oauth2client.service_account import ServiceAccountCredentials
+
+def get_google_service_account_email():
+    """
+    Returns the service account email to share Drive files with.
+    """
+    return google_config['service-account']['client_email']
+
+def initialize_credentials():
+    """
+    initialize_credentials: -> oauth2client.service_account.ServiceAccountCredentials
+
+    Returns credentials that allows you to access your Google Drive &
+    Sheets using the Google Sheets API.
+
+    You still need to share spreadsheets with the service account email.
+    """
+
+    # This prevents us from erroring out trying to construct credentials
+    # from incomplete information.
+    service_account = google_config.get('service-account', {})
+    private_key = service_account.get('private_key', None)
+    if not private_key:
+        print(
+            "You're missing Google service account credentials",
+            "in credentials.py.",
+            "To access your Google Drive data,",
+            "fill out the Google service account information."
+        )
+        return None
+
+    credentials = ServiceAccountCredentials.from_json_keyfile_dict(
+        google_config['service-account'],
+        scopes=google_config['scopes'],
+    )
+    print(
+        'To access your Google Drive file, share the file with {email}'
+        .format(email=get_google_service_account_email())
+    )
+    return credentials
+
+def create_client(credentials):
+    """
+    create_engine:
+
+    Sets up Google Drive API access using credentials (see above).
+    """
+    gauth = GoogleAuth()
+    gauth.credentials = credentials
+    drive = GoogleDrive(gauth)
+    return drive
+
+# Set up credentials
+credentials = initialize_credentials()
+
+# This is a wrapper for pydrive.GoogleDrive
+GoogleDrive = None if credentials is None else create_client(credentials)
```

### Comparing `spswarehouse-0.1.0/spswarehouse/powerschool/powerschool.py` & `spswarehouse-0.1.1/spswarehouse/powerschool/powerschool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import logging
 import time
 import os
 
-from spswarehouse.credentials import powerschool_config
+try:
+    from spswarehouse.credentials import powerschool_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
 
 from ducttape.utils import (
     DriverBuilder,
     get_most_recent_file_in_dir,
 )
```

### Comparing `spswarehouse-0.1.0/spswarehouse/powerschool/powerschool_calpads.py` & `spswarehouse-0.1.1/spswarehouse/powerschool/powerschool_calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.1.0/spswarehouse/table_names.py` & `spswarehouse-0.1.1/spswarehouse/table_names.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.1.0/spswarehouse/table_utils.py` & `spswarehouse-0.1.1/spswarehouse/table_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pandas as pd
 import numpy as np
 import os
 import random
 import string
 
-from .credentials import snowflake_config
 from .warehouse import Warehouse
 from .googledrive import GoogleDrive
 
 DEFAULT_ENCODING='utf-8'
 DEFAULT_BATCH_SIZE=200
 
 # Copied from https://stackoverflow.com/questions/40774787/renaming-columns-in-a-pandas-dataframe-with-duplicate-column-names
@@ -67,15 +66,15 @@
             guess = data_types[df.dtypes[col_name]]
         col_types[col_name.lower()] = guess
 
     return col_types
 
 def create_table_stmt(
     table_name,
-    schema=snowflake_config['schema'],
+    schema,
     comment='',
     # We'll use "columns" as-is
     columns=None, # {column name: column type}
     encoding=DEFAULT_ENCODING, # text encoding, e.g. 'utf-8' or 'latin-1'
     # We'll try to guess what the column types are if you pass in one of the rest
     dataframe=None, # pandas.DataFrame
     csv_filename=None, # string
```

### Comparing `spswarehouse-0.1.0/spswarehouse/warehouse.py` & `spswarehouse-0.1.1/spswarehouse/warehouse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,119 +1,123 @@
-import pandas
-
-from .credentials import snowflake_config
-from sqlalchemy.engine.url import URL
-from sqlalchemy import create_engine, MetaData, Table
-from sqlalchemy.engine import reflection
-from snowflake.sqlalchemy import VARIANT
-
-from datetime import date
-
-def describe(table):
-    for c in table.columns:
-        tipe = c.type
-        if isinstance(tipe, VARIANT):
-             tipe = 'VARIANT'
-        print('{}: {}'.format(c.name, tipe))
-
-class Warehouse:
-    """
-    This class is an abstraction that allows you to connect to the Snowflake Warehouse.
-    It has several methods that allow for easy access to the warehouse.
-    -- execute: run some arbitrary SQL in the warehouse. totally safe!
-    -- read_sql: execute a SELECT statement and return results as a pandas.DataFrame
-    -- reflect: return a SQLAlchemy Table object containing metadata about the table
-
-    This class also has a couple of SQLAlchemy-based instance variables
-    - engine: contains information about how to connect to the warehouse
-    - insp: a SQLAlchemy inspector object that lets query metadata about the warehouse
-            e.g., Snowflake.insp.get_table_names('wild_west')
-    """
-    def __init__(self, engine):
-        self.engine = engine
-        self.meta = MetaData(bind=engine)
-        self._insp = None
-        self._conn = None
-        self.loaded_tables = {}   # dictionary of Table objects keyed by "schema.table_name"
-
-    @property
-    def insp(self):
-        if self._insp is None:
-            self._insp = reflection.Inspector.from_engine(self.engine)
-        return self._insp
-
-    @property
-    def conn(self):
-        if self._conn is None:
-            self._conn = self.engine.connect()
-        return self._conn
-
-    # caller is responsible for closing the connection when done
-    def execute(self, sql):
-        """
-        execute: SQL statement -> (connection, proxy)
-
-        Running the execute method sends the SQL string to the warehouse using
-        this object's connection object. The return value is a tuple of the
-        connection object and the SQLAlchemy proxy object returned from executing
-        the SQL.
-        """
-        return self.conn, self.conn.execute(sql)
-
-    def read_sql(self, sql):
-        """
-        read_sql: 'SELECT ...' -> pandas.DataFrame
-        read_sql: SQLAlchemy select object -> pandas.DataFrame
-
-        The warehouse read_sql method is a minimalist wrapper around the pandas.read_sql
-        method. The sole argument to this method can either be a string (typically a SELECT statement)
-        or an object constructed using SQLAlchemy's select method.
-        """
-        return pandas.read_sql(sql, self.engine)
-
-    def reflect(self, table_or_view, schema=snowflake_config['schema']):
-        """
-        reflect: table name, schema name (optional) -> SQLAlchemy Table object
-        reflect: view name,  schema name (optional) -> SQLAlchemy Table object
-
-        The reflect method is useful to grab the underlying metadata for a table in the warehouse.
-        Using the returned value, you can print out the column names and types using the describe method.
-
-        Note that if the table or view name has a '.' in it, then this method will try to infer the schema name
-        and ignore the passed in argument
-
-        t_table = Snowflake.reflect('users', schema='staging_scrapes')
-        describe(t_table)
-        """
-        name_with_schema = '{schema}.{table_or_view}'.format(
-            schema=schema,
-            table_or_view=table_or_view
-        )
-
-        # if it's already been loaded, why bother loading it again? just return it
-        table = self.loaded_tables.get(name_with_schema, None)
-        if table is not None:
-            return table
-
-        table = Table(table_or_view, self.meta, autoload=True, schema=schema)
-
-        # sets the column names explicitly on the instance so that tab-completion is easy
-        for c in table.columns:
-            setattr(table, 'c_{}'.format(c.name), c)
-
-        # save so we don't have to load it again later
-        self.loaded_tables[name_with_schema] = table
-
-        return table
-
-Warehouse = Warehouse(
-    create_engine(
-        'snowflake://{user}:{password}@{account}/{db}/{schema}?warehouse={warehouse}'.format(
-            user=snowflake_config['user'],
-            password=snowflake_config['password'],
-            account=snowflake_config['account'],
-            db=snowflake_config['db'],
-            schema=snowflake_config['schema'],
-            warehouse=snowflake_config['warehouse']),
-        pool_size=1
-    )
-)
+import pandas
+
+try:
+    from .credentials import snowflake_config
+except ModuleNotFoundError:
+    print("No credentials file found in spswarehouse. This could cause issues.")
+    
+from sqlalchemy.engine.url import URL
+from sqlalchemy import create_engine, MetaData, Table
+from sqlalchemy.engine import reflection
+from snowflake.sqlalchemy import VARIANT
+
+from datetime import date
+
+def describe(table):
+    for c in table.columns:
+        tipe = c.type
+        if isinstance(tipe, VARIANT):
+             tipe = 'VARIANT'
+        print('{}: {}'.format(c.name, tipe))
+
+class Warehouse:
+    """
+    This class is an abstraction that allows you to connect to the Snowflake Warehouse.
+    It has several methods that allow for easy access to the warehouse.
+    -- execute: run some arbitrary SQL in the warehouse. totally safe!
+    -- read_sql: execute a SELECT statement and return results as a pandas.DataFrame
+    -- reflect: return a SQLAlchemy Table object containing metadata about the table
+
+    This class also has a couple of SQLAlchemy-based instance variables
+    - engine: contains information about how to connect to the warehouse
+    - insp: a SQLAlchemy inspector object that lets query metadata about the warehouse
+            e.g., Snowflake.insp.get_table_names('wild_west')
+    """
+    def __init__(self, engine):
+        self.engine = engine
+        self.meta = MetaData(bind=engine)
+        self._insp = None
+        self._conn = None
+        self.loaded_tables = {}   # dictionary of Table objects keyed by "schema.table_name"
+
+    @property
+    def insp(self):
+        if self._insp is None:
+            self._insp = reflection.Inspector.from_engine(self.engine)
+        return self._insp
+
+    @property
+    def conn(self):
+        if self._conn is None:
+            self._conn = self.engine.connect()
+        return self._conn
+
+    # caller is responsible for closing the connection when done
+    def execute(self, sql):
+        """
+        execute: SQL statement -> (connection, proxy)
+
+        Running the execute method sends the SQL string to the warehouse using
+        this object's connection object. The return value is a tuple of the
+        connection object and the SQLAlchemy proxy object returned from executing
+        the SQL.
+        """
+        return self.conn, self.conn.execute(sql)
+
+    def read_sql(self, sql):
+        """
+        read_sql: 'SELECT ...' -> pandas.DataFrame
+        read_sql: SQLAlchemy select object -> pandas.DataFrame
+
+        The warehouse read_sql method is a minimalist wrapper around the pandas.read_sql
+        method. The sole argument to this method can either be a string (typically a SELECT statement)
+        or an object constructed using SQLAlchemy's select method.
+        """
+        return pandas.read_sql(sql, self.engine)
+
+    def reflect(self, table_or_view, schema=snowflake_config['schema']):
+        """
+        reflect: table name, schema name (optional) -> SQLAlchemy Table object
+        reflect: view name,  schema name (optional) -> SQLAlchemy Table object
+
+        The reflect method is useful to grab the underlying metadata for a table in the warehouse.
+        Using the returned value, you can print out the column names and types using the describe method.
+
+        Note that if the table or view name has a '.' in it, then this method will try to infer the schema name
+        and ignore the passed in argument
+
+        t_table = Snowflake.reflect('users', schema='staging_scrapes')
+        describe(t_table)
+        """
+        name_with_schema = '{schema}.{table_or_view}'.format(
+            schema=schema,
+            table_or_view=table_or_view
+        )
+
+        # if it's already been loaded, why bother loading it again? just return it
+        table = self.loaded_tables.get(name_with_schema, None)
+        if table is not None:
+            return table
+
+        table = Table(table_or_view, self.meta, autoload=True, schema=schema)
+
+        # sets the column names explicitly on the instance so that tab-completion is easy
+        for c in table.columns:
+            setattr(table, 'c_{}'.format(c.name), c)
+
+        # save so we don't have to load it again later
+        self.loaded_tables[name_with_schema] = table
+
+        return table
+
+Warehouse = Warehouse(
+    create_engine(
+        'snowflake://{user}:{password}@{account}/{db}/{schema}?warehouse={warehouse}'.format(
+            user=snowflake_config['user'],
+            password=snowflake_config['password'],
+            account=snowflake_config['account'],
+            db=snowflake_config['db'],
+            schema=snowflake_config['schema'],
+            warehouse=snowflake_config['warehouse']),
+        pool_size=1
+    )
+)
```

### Comparing `spswarehouse-0.1.0/spswarehouse.egg-info/PKG-INFO` & `spswarehouse-0.1.1/spswarehouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.1.0
+Version: 0.1.1
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.1.0/spswarehouse.egg-info/SOURCES.txt` & `spswarehouse-0.1.1/spswarehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

