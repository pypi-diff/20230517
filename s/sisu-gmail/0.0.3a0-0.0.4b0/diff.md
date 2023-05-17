# Comparing `tmp/sisu_gmail-0.0.3a0.tar.gz` & `tmp/sisu_gmail-0.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sisu_gmail-0.0.3a0.tar", last modified: Thu Aug  4 02:53:24 2022, max compression
+gzip compressed data, was "sisu_gmail-0.0.4b0.tar", last modified: Wed May 17 21:52:33 2023, max compression
```

## Comparing `sisu_gmail-0.0.3a0.tar` & `sisu_gmail-0.0.4b0.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxrwxr-x   0 loren     (1001) loren     (1001)        0 2022-08-04 02:53:24.794157 sisu_gmail-0.0.3a0/
--rw-rw-r--   0 loren     (1001) loren     (1001)    35147 2022-03-07 22:19:50.000000 sisu_gmail-0.0.3a0/LICENSE
--rw-rw-r--   0 loren     (1001) loren     (1001)     1175 2022-08-04 02:53:24.794157 sisu_gmail-0.0.3a0/PKG-INFO
--rw-rw-r--   0 loren     (1001) loren     (1001)      573 2022-03-09 16:23:19.000000 sisu_gmail-0.0.3a0/README.md
--rw-rw-r--   0 loren     (1001) loren     (1001)      103 2022-03-05 15:10:45.000000 sisu_gmail-0.0.3a0/pyproject.toml
--rw-rw-r--   0 loren     (1001) loren     (1001)      672 2022-08-04 02:53:24.794157 sisu_gmail-0.0.3a0/setup.cfg
--rw-rw-r--   0 loren     (1001) loren     (1001)     1222 2022-08-04 02:52:21.000000 sisu_gmail-0.0.3a0/setup.py
-drwxrwxr-x   0 loren     (1001) loren     (1001)        0 2022-08-04 02:53:24.794157 sisu_gmail-0.0.3a0/src/
-drwxrwxr-x   0 loren     (1001) loren     (1001)        0 2022-08-04 02:53:24.794157 sisu_gmail-0.0.3a0/src/sisu_gmail/
--rw-rw-r--   0 loren     (1001) loren     (1001)      159 2022-03-09 15:28:51.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/__init__.py
--rw-rw-r--   0 loren     (1001) loren     (1001)     1975 2022-03-09 13:58:11.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/auth.py
--rw-rw-r--   0 loren     (1001) loren     (1001)      330 2022-08-04 02:49:47.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/create.py
--rw-rw-r--   0 loren     (1001) loren     (1001)      892 2022-03-09 15:51:28.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/delete.py
--rw-rw-r--   0 loren     (1001) loren     (1001)     2088 2022-03-09 17:07:09.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/label.py
--rw-rw-r--   0 loren     (1001) loren     (1001)      377 2022-03-16 08:05:52.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/read.py
--rw-rw-r--   0 loren     (1001) loren     (1001)     2592 2022-05-01 05:27:16.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/search.py
--rw-rw-r--   0 loren     (1001) loren     (1001)      387 2022-03-09 15:48:44.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/send.py
--rw-rw-r--   0 loren     (1001) loren     (1001)      295 2022-03-08 00:54:14.000000 sisu_gmail-0.0.3a0/src/sisu_gmail/user.py
-drwxrwxr-x   0 loren     (1001) loren     (1001)        0 2022-08-04 02:53:24.794157 sisu_gmail-0.0.3a0/src/sisu_gmail.egg-info/
--rw-rw-r--   0 loren     (1001) loren     (1001)     1175 2022-08-04 02:53:24.000000 sisu_gmail-0.0.3a0/src/sisu_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 loren     (1001) loren     (1001)      421 2022-08-04 02:53:24.000000 sisu_gmail-0.0.3a0/src/sisu_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 loren     (1001) loren     (1001)        1 2022-08-04 02:53:24.000000 sisu_gmail-0.0.3a0/src/sisu_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 loren     (1001) loren     (1001)       11 2022-08-04 02:53:24.000000 sisu_gmail-0.0.3a0/src/sisu_gmail.egg-info/top_level.txt
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:52:33.442846 sisu_gmail-0.0.4b0/
+-rw-rw-r--   0 loren     (1000) loren     (1000)    35147 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/LICENSE
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1106 2023-05-17 21:52:33.442846 sisu_gmail-0.0.4b0/PKG-INFO
+-rw-rw-r--   0 loren     (1000) loren     (1000)      573 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/README.md
+-rw-rw-r--   0 loren     (1000) loren     (1000)      103 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/pyproject.toml
+-rw-rw-r--   0 loren     (1000) loren     (1000)      657 2023-05-17 21:52:33.446846 sisu_gmail-0.0.4b0/setup.cfg
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:52:33.442846 sisu_gmail-0.0.4b0/src/
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:52:33.442846 sisu_gmail-0.0.4b0/src/sisu_gmail/
+-rw-rw-r--   0 loren     (1000) loren     (1000)      159 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/__init__.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1975 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/auth.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      330 2023-05-17 18:39:58.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/create.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      892 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/delete.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     2088 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/label.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      377 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/read.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     2405 2023-05-17 21:35:03.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/search.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      387 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/send.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      295 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/src/sisu_gmail/user.py
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:52:33.442846 sisu_gmail-0.0.4b0/src/sisu_gmail.egg-info/
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1106 2023-05-17 21:52:33.000000 sisu_gmail-0.0.4b0/src/sisu_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 loren     (1000) loren     (1000)      571 2023-05-17 21:52:33.000000 sisu_gmail-0.0.4b0/src/sisu_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 loren     (1000) loren     (1000)        1 2023-05-17 21:52:33.000000 sisu_gmail-0.0.4b0/src/sisu_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 loren     (1000) loren     (1000)       11 2023-05-17 21:52:33.000000 sisu_gmail-0.0.4b0/src/sisu_gmail.egg-info/top_level.txt
+drwxrwxr-x   0 loren     (1000) loren     (1000)        0 2023-05-17 21:52:33.442846 sisu_gmail-0.0.4b0/tests/
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1489 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/tests/test_auth.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      917 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/tests/test_create.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     2109 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/tests/test_delete.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     4416 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/tests/test_label.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      713 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/tests/test_read.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     2382 2023-05-17 21:36:11.000000 sisu_gmail-0.0.4b0/tests/test_search.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)     1336 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/tests/test_send.py
+-rw-rw-r--   0 loren     (1000) loren     (1000)      444 2023-05-17 18:27:11.000000 sisu_gmail-0.0.4b0/tests/test_user.py
```

### Comparing `sisu_gmail-0.0.3a0/LICENSE` & `sisu_gmail-0.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `sisu_gmail-0.0.3a0/PKG-INFO` & `sisu_gmail-0.0.4b0/src/sisu_gmail.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
-Name: sisu_gmail
-Version: 0.0.3a0
-Summary: sisu_email - some abstractions around the standard python email library
+Name: sisu-gmail
+Version: 0.0.4b0
+Summary: A package to simplify my gmail api life
 Home-page: https://github.com/loren-magnuson/sisu_gmail
 Author: Loren Magnuson
 Author-email: lorenjmagnuson@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/loren-magnuson/sisu_gmail/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,9 +30,7 @@
 6) The Gmail API auth flow should start, complete it.
 
 7) The auth token for your test email will be saved as token.json.
 
 8) Tests should now attempt to complete.
 
 9) Before your next test run, delete any leftover emails.
-
-
```

### Comparing `sisu_gmail-0.0.3a0/README.md` & `sisu_gmail-0.0.4b0/README.md`

 * *Files identical despite different names*

### Comparing `sisu_gmail-0.0.3a0/setup.cfg` & `sisu_gmail-0.0.4b0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-name = sisU_gmail_loren-magnuson
-version = 0.0.3a
+name = sisu_gmail
+version = 0.0.4b
 author = Loren Magnuson
 author_email = lorenjmagnuson@gmail.com
 description = A package to simplify my gmail api life
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/loren-magnuson/sisu_gmail
 project_urls =
```

### Comparing `sisu_gmail-0.0.3a0/src/sisu_gmail/auth.py` & `sisu_gmail-0.0.4b0/src/sisu_gmail/auth.py`

 * *Files identical despite different names*

### Comparing `sisu_gmail-0.0.3a0/src/sisu_gmail/delete.py` & `sisu_gmail-0.0.4b0/src/sisu_gmail/delete.py`

 * *Files identical despite different names*

### Comparing `sisu_gmail-0.0.3a0/src/sisu_gmail/label.py` & `sisu_gmail-0.0.4b0/src/sisu_gmail/label.py`

 * *Files identical despite different names*

### Comparing `sisu_gmail-0.0.3a0/src/sisu_gmail/search.py` & `sisu_gmail-0.0.4b0/src/sisu_gmail/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,38 +3,28 @@
 }
 
 
 class NoNextPageToken(KeyError):
     pass
 
 
-def next_page(resource, user_id, query, response, max_results=100):
+def next_page(resource, user_id, query, next_page_token, max_results=100):
     """Get next page of search results
 
     :param resource: Gmail API resource
     :param user_id: str, Gmail API userId
     :param query: str, Gmail API search query
-    :param response: dict, Gmail API search query response
+    :param next_page_token: str, token for next page
     :param max_results: int, number of results per request
     :return: list, dicts of gmail message_id message_ids and thread message_ids
     """
-    if not type(response) is dict:
-        raise TypeError(
-            'next_search_page requires dict as response param'
-        )
-    elif 'nextPageToken' not in response:
-        raise NoNextPageToken(
-            'next_search_page requires dict with nextPageToken key'
-        )
-
-    page_token = response['nextPageToken']
     return resource.users().messages().list(
         userId=user_id,
         q=query,
-        pageToken=page_token,
+        pageToken=next_page_token,
         maxResults=max_results
     ).execute()
 
 
 def search(resource, user_id, query, max_results=100):
     """Return search results response for a Gmail API query
 
@@ -55,25 +45,31 @@
     """Generator to return search results
 
     :param resource: Gmail API resource
     :param user_id: str, Gmail API userId
     :param query: str, Gmail API search query
     :return: dict, gmail message_id message_ids and thread message_ids
     """
+
+    do_next = True
     response = resource.users().messages().list(
         userId=user_id,
         q=query
     ).execute()
-
-    if 'messages' in response:
-        part = response['messages']
-        for index, result in enumerate(part, start=1):
-            yield result
-            if len(part) == index and 'nextPageToken' in response:
-                next_page(resource, user_id, response, query)
+    while do_next:
+        if 'messages' in response:
+            print(len(response['messages']))
+            for result in response['messages']:
+                yield result
+            if 'nextPageToken' in response:
+                response = next_page(resource, user_id, query, response['nextPageToken'])
+            else:
+                do_next = False
+        else:
+            break
 
 
 def search_by_address(resource, user_id, address):
     """Search gmail for messages by sender email address
 
     :param resource: Gmail API Resource
     :param user_id: str, Gmail API userId
```

### Comparing `sisu_gmail-0.0.3a0/src/sisu_gmail.egg-info/PKG-INFO` & `sisu_gmail-0.0.4b0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
-Name: sisu-gmail
-Version: 0.0.3a0
-Summary: sisu_email - some abstractions around the standard python email library
+Name: sisu_gmail
+Version: 0.0.4b0
+Summary: A package to simplify my gmail api life
 Home-page: https://github.com/loren-magnuson/sisu_gmail
 Author: Loren Magnuson
 Author-email: lorenjmagnuson@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/loren-magnuson/sisu_gmail/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -32,9 +30,7 @@
 6) The Gmail API auth flow should start, complete it.
 
 7) The auth token for your test email will be saved as token.json.
 
 8) Tests should now attempt to complete.
 
 9) Before your next test run, delete any leftover emails.
-
-
```

