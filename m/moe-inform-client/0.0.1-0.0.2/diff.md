# Comparing `tmp/moe-inform-client-0.0.1.tar.gz` & `tmp/moe-inform-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moe-inform-client-0.0.1.tar", last modified: Mon Jan 30 11:21:58 2023, max compression
+gzip compressed data, was "moe-inform-client-0.0.2.tar", last modified: Wed May 17 08:37:55 2023, max compression
```

## Comparing `moe-inform-client-0.0.1.tar` & `moe-inform-client-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-01-30 11:21:58.445785 moe-inform-client-0.0.1/
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     1060 2023-01-24 07:40:47.000000 moe-inform-client-0.0.1/LICENSE
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     5209 2023-01-30 11:21:58.444801 moe-inform-client-0.0.1/PKG-INFO
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     3391 2023-01-30 11:15:31.000000 moe-inform-client-0.0.1/README.md
-drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-01-30 11:21:58.416572 moe-inform-client-0.0.1/informclient/
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       46 2023-01-24 07:40:47.000000 moe-inform-client-0.0.1/informclient/__init__.py
-drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-01-30 11:21:58.405687 moe-inform-client-0.0.1/informclient/api/
-drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-01-30 11:21:58.420020 moe-inform-client-0.0.1/informclient/api/request/
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       79 2023-01-24 07:40:47.000000 moe-inform-client-0.0.1/informclient/api/request/__init__.py
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     1911 2023-01-24 07:40:47.000000 moe-inform-client-0.0.1/informclient/api/request/request_validator.py
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     1582 2023-01-24 07:44:36.000000 moe-inform-client-0.0.1/informclient/informclient.py
-drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-01-30 11:21:58.423819 moe-inform-client-0.0.1/informclient/utils/
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       73 2023-01-24 07:40:47.000000 moe-inform-client-0.0.1/informclient/utils/__init__.py
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       93 2023-01-24 07:40:47.000000 moe-inform-client-0.0.1/informclient/utils/api_description.py
-drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-01-30 11:21:58.443425 moe-inform-client-0.0.1/moe_inform_client.egg-info/
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     5209 2023-01-30 11:21:58.000000 moe-inform-client-0.0.1/moe_inform_client.egg-info/PKG-INFO
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)      436 2023-01-30 11:21:58.000000 moe-inform-client-0.0.1/moe_inform_client.egg-info/SOURCES.txt
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)        1 2023-01-30 11:21:58.000000 moe-inform-client-0.0.1/moe_inform_client.egg-info/dependency_links.txt
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       51 2023-01-30 11:21:58.000000 moe-inform-client-0.0.1/moe_inform_client.egg-info/requires.txt
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       13 2023-01-30 11:21:58.000000 moe-inform-client-0.0.1/moe_inform_client.egg-info/top_level.txt
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       38 2023-01-30 11:21:58.445941 moe-inform-client-0.0.1/setup.cfg
--rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     1383 2023-01-30 11:06:57.000000 moe-inform-client-0.0.1/setup.py
+drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-05-17 08:37:33.378266 moe-inform-client-0.0.2/
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     1060 2023-01-24 07:40:47.000000 moe-inform-client-0.0.2/LICENSE
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     5208 2023-05-17 08:37:55.766392 moe-inform-client-0.0.2/PKG-INFO
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     3390 2023-05-17 08:32:26.000000 moe-inform-client-0.0.2/README.md
+drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-05-17 08:37:33.266709 moe-inform-client-0.0.2/informclient/
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       46 2023-01-24 07:40:47.000000 moe-inform-client-0.0.2/informclient/__init__.py
+drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-05-17 08:37:33.210032 moe-inform-client-0.0.2/informclient/api/
+drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-05-17 08:37:33.281467 moe-inform-client-0.0.2/informclient/api/request/
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       79 2023-01-24 07:40:47.000000 moe-inform-client-0.0.2/informclient/api/request/__init__.py
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     1911 2023-01-24 07:40:47.000000 moe-inform-client-0.0.2/informclient/api/request/request_validator.py
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     1582 2023-01-24 07:44:36.000000 moe-inform-client-0.0.2/informclient/informclient.py
+drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-05-17 08:37:33.304249 moe-inform-client-0.0.2/informclient/utils/
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       73 2023-01-24 07:40:47.000000 moe-inform-client-0.0.2/informclient/utils/__init__.py
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       93 2023-01-24 07:40:47.000000 moe-inform-client-0.0.2/informclient/utils/api_description.py
+drwxr-xr-x   0 mohammadtariqueanjum   (501) staff       (20)        0 2023-05-17 08:37:55.764369 moe-inform-client-0.0.2/moe_inform_client.egg-info/
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     5208 2023-05-17 08:37:55.000000 moe-inform-client-0.0.2/moe_inform_client.egg-info/PKG-INFO
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)      436 2023-05-17 08:37:55.000000 moe-inform-client-0.0.2/moe_inform_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)        1 2023-05-17 08:37:55.000000 moe-inform-client-0.0.2/moe_inform_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       50 2023-05-17 08:37:55.000000 moe-inform-client-0.0.2/moe_inform_client.egg-info/requires.txt
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       13 2023-05-17 08:37:55.000000 moe-inform-client-0.0.2/moe_inform_client.egg-info/top_level.txt
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)       38 2023-05-17 08:37:55.773009 moe-inform-client-0.0.2/setup.cfg
+-rw-r--r--   0 mohammadtariqueanjum   (501) staff       (20)     1382 2023-05-17 08:35:06.000000 moe-inform-client-0.0.2/setup.py
```

### Comparing `moe-inform-client-0.0.1/LICENSE` & `moe-inform-client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moe-inform-client-0.0.1/PKG-INFO` & `moe-inform-client-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moe-inform-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: This Python Package helps you in sending notifications through MoEngage Inform
 Home-page: https://github.com/moengage/inform-client-python
 Author: MoEngage
 Author-email: inform@moengage.com
 Project-URL: Bug Tracker, https://github.com/moengage/inform-client-python/issues
 Keywords: MoEngage,Inform,MoEngage Inform,Customer Engagement,Transactional Alerts
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,15 @@
 ```
 
 python3.9 or later is required.
 
 ## Requirements
 ```text
   StrEnum~=0.4.9
-  urllib3~=1.26.13
+  urllib3~=1.26.5
   jsonschema~=4.17.3
 ```
 Note: Install these individually if any issue raises in installation of these requirements like this 
 ```shell
 $ pip install StrEnum~=0.4.9
 ```
```

### Comparing `moe-inform-client-0.0.1/README.md` & `moe-inform-client-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ```
 
 python3.9 or later is required.
 
 ## Requirements
 ```text
   StrEnum~=0.4.9
-  urllib3~=1.26.13
+  urllib3~=1.26.5
   jsonschema~=4.17.3
 ```
 Note: Install these individually if any issue raises in installation of these requirements like this 
 ```shell
 $ pip install StrEnum~=0.4.9
 ```
```

### Comparing `moe-inform-client-0.0.1/informclient/api/request/request_validator.py` & `moe-inform-client-0.0.2/informclient/api/request/request_validator.py`

 * *Files identical despite different names*

### Comparing `moe-inform-client-0.0.1/informclient/informclient.py` & `moe-inform-client-0.0.2/informclient/informclient.py`

 * *Files identical despite different names*

### Comparing `moe-inform-client-0.0.1/moe_inform_client.egg-info/PKG-INFO` & `moe-inform-client-0.0.2/moe_inform_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moe-inform-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: This Python Package helps you in sending notifications through MoEngage Inform
 Home-page: https://github.com/moengage/inform-client-python
 Author: MoEngage
 Author-email: inform@moengage.com
 Project-URL: Bug Tracker, https://github.com/moengage/inform-client-python/issues
 Keywords: MoEngage,Inform,MoEngage Inform,Customer Engagement,Transactional Alerts
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,15 @@
 ```
 
 python3.9 or later is required.
 
 ## Requirements
 ```text
   StrEnum~=0.4.9
-  urllib3~=1.26.13
+  urllib3~=1.26.5
   jsonschema~=4.17.3
 ```
 Note: Install these individually if any issue raises in installation of these requirements like this 
 ```shell
 $ pip install StrEnum~=0.4.9
 ```
```

### Comparing `moe-inform-client-0.0.1/setup.py` & `moe-inform-client-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 with open('LICENSE', 'r') as fh:
     long_description += fh.read()
 
 
 setup(
     name='moe-inform-client',
-    version='0.0.1',
+    version='0.0.2',
     author='MoEngage',
     author_email='inform@moengage.com',
     description='This Python Package helps you in sending notifications through MoEngage Inform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/moengage/inform-client-python',
     project_urls={
             'Bug Tracker': 'https://github.com/moengage/inform-client-python/issues',
     },
     install_requires=['StrEnum~=0.4.9',
-                      'urllib3~=1.26.13',
+                      'urllib3~=1.26.5',
                       'jsonschema~=4.17.3'
                       ],
     keywords=['MoEngage', 'Inform', 'MoEngage Inform', 'Customer Engagement', 'Transactional Alerts'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

