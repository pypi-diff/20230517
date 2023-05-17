# Comparing `tmp/yotpy-0.0.85.tar.gz` & `tmp/yotpy-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.85.tar", last modified: Tue May 16 00:42:07 2023, max compression
+gzip compressed data, was "yotpy-0.0.86.tar", last modified: Wed May 17 18:40:42 2023, max compression
```

## Comparing `yotpy-0.0.85.tar` & `yotpy-0.0.86.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.85/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.85/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.85/LICENSE
--rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.85/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.85/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.85/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.85/docs/yotpy.html
--rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.85/pyproject.toml
--rw-r--r--   0        0        0      318 2023-05-16 00:40:49.101718 yotpy-0.0.85/yotpy/__init__.py
--rw-r--r--   0        0        0    32578 2023-05-16 00:40:41.423561 yotpy-0.0.85/yotpy/core.py
--rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.85/yotpy/exceptions.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.85/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.86/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.86/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.86/LICENSE
+-rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.86/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.86/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.86/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.86/docs/yotpy.html
+-rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.86/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-05-17 18:32:02.176845 yotpy-0.0.86/yotpy/__init__.py
+-rw-r--r--   0        0        0    33804 2023-05-17 18:33:54.895065 yotpy-0.0.86/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.86/yotpy/exceptions.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 yotpy-0.0.86/PKG-INFO
```

### Comparing `yotpy-0.0.85/.github/workflows/static.yml` & `yotpy-0.0.86/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.85/LICENSE` & `yotpy-0.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.85/docs/search.js` & `yotpy-0.0.86/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.85/docs/yotpy.html` & `yotpy-0.0.86/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.85/pyproject.toml` & `yotpy-0.0.86/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.85/yotpy/core.py` & `yotpy-0.0.86/yotpy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 import asyncio
 import aiohttp
 
 from json import loads as json_loads
 from csv import DictWriter
+from openpyxl import Workbook
 from io import StringIO, BytesIO, TextIOWrapper
 from typing import AsyncGenerator, Iterator, Union, Optional, Callable, Union
 from html import unescape
 from urllib.parse import urlencode
 from math import ceil
 from itertools import chain
 from .exceptions import CustomException, SessionNotCreatedError, FailedToGetTokenError, PreflightException, UploadException, SendException, UserNotFound, AppNotFound
@@ -347,14 +348,51 @@
         csv_bytesio = csv_textio.detach()
 
         # Reset the BytesIO object's position to the beginning
         csv_bytesio.seek(0)
 
         return csv_bytesio
 
+    @staticmethod
+    def to_xlsx_bytesio(headers: set, rows: list[dict]) -> BytesIO:
+        """
+        Convert a list of rows into a Excel formatted BytesIO object.
+
+        This method takes a list of rows (dictionaries) and a set of headers, and writes them into
+        an Excel formatted BytesIO object. It can be used to create an Excel file-like object without
+        creating an actual file on the filesystem.
+
+        Args:
+            headers (set): A set of headers to use for the Excel data.
+            rows (list[dict]): A list of rows to convert into an Excel formatted BytesIO object.
+
+        Returns:
+            BytesIO: An Excel formatted BytesIO object.
+        """
+        # Create a Workbook object
+        wb = Workbook()
+        ws = wb.active
+
+        # Write headers
+        ws.append(list(headers))
+
+        # Write rows
+        for row in rows:
+            ws.append([row[h] for h in headers])
+
+        # Save workbook to a BytesIO object
+        xlsx_bytesio = BytesIO()
+        wb.save(xlsx_bytesio)
+
+        # Reset the BytesIO object's position to the beginning
+        xlsx_bytesio.seek(0)
+
+        return xlsx_bytesio
+
+
 class YotpoAPIWrapper:
     # NOTE: Update docstring if more methods are added to account for any added functionality outside of the defined scope.
     """
     A class for interacting with the Yotpo API to fetch app and account information, review data, and send manual review requests.
 
     The YotpoAPIWrapper uses the provided app_key and secret for authentication and constructs the necessary API endpoints for making requests.
```

### Comparing `yotpy-0.0.85/yotpy/exceptions.py` & `yotpy-0.0.86/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.85/PKG-INFO` & `yotpy-0.0.86/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.85
+Version: 0.0.86
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

