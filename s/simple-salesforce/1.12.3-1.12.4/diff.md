# Comparing `tmp/simple-salesforce-1.12.3.tar.gz` & `tmp/simple-salesforce-1.12.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-salesforce-1.12.3.tar", last modified: Thu Jan 12 19:02:37 2023, max compression
+gzip compressed data, was "simple-salesforce-1.12.4.tar", last modified: Wed May 17 16:44:08 2023, max compression
```

## Comparing `simple-salesforce-1.12.3.tar` & `simple-salesforce-1.12.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-12 19:02:37.208685 simple-salesforce-1.12.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    26341 2023-01-12 19:02:37.208685 simple-salesforce-1.12.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    25278 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-01-12 19:02:37.208685 simple-salesforce-1.12.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-12 19:02:37.208685 simple-salesforce-1.12.3/simple_salesforce/
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      514 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/__version__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41193 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18038 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/bulk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3330 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/format.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10150 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/login.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3308 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23215 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   911649 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/metadata.wsdl
--rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-01-12 19:02:02.000000 simple-salesforce-1.12.3/simple_salesforce/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-12 19:02:37.208685 simple-salesforce-1.12.3/simple_salesforce.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    26341 2023-01-12 19:02:37.000000 simple-salesforce-1.12.3/simple_salesforce.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      576 2023-01-12 19:02:37.000000 simple-salesforce-1.12.3/simple_salesforce.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-01-12 19:02:37.000000 simple-salesforce-1.12.3/simple_salesforce.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2023-01-12 19:02:37.000000 simple-salesforce-1.12.3/simple_salesforce.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2023-01-12 19:02:37.000000 simple-salesforce-1.12.3/simple_salesforce.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-17 16:44:08.312248 simple-salesforce-1.12.4/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26741 2023-05-17 16:44:08.312248 simple-salesforce-1.12.4/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25678 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-05-17 16:44:08.312248 simple-salesforce-1.12.4/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1833 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-17 16:44:08.312248 simple-salesforce-1.12.4/simple_salesforce/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      514 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/__version__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41248 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18038 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/bulk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3330 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/format.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10160 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/login.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3308 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23350 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   911649 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/metadata.wsdl
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-05-17 16:43:07.000000 simple-salesforce-1.12.4/simple_salesforce/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-17 16:44:08.312248 simple-salesforce-1.12.4/simple_salesforce.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26741 2023-05-17 16:44:08.000000 simple-salesforce-1.12.4/simple_salesforce.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      576 2023-05-17 16:44:08.000000 simple-salesforce-1.12.4/simple_salesforce.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-17 16:44:08.000000 simple-salesforce-1.12.4/simple_salesforce.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2023-05-17 16:44:08.000000 simple-salesforce-1.12.4/simple_salesforce.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2023-05-17 16:44:08.000000 simple-salesforce-1.12.4/simple_salesforce.egg-info/top_level.txt
```

### Comparing `simple-salesforce-1.12.3/LICENSE.txt` & `simple-salesforce-1.12.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.3/PKG-INFO` & `simple-salesforce-1.12.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-salesforce
-Version: 1.12.3
+Version: 1.12.4
 Summary: A basic Salesforce.com REST API client.
 Home-page: https://github.com/simple-salesforce/simple-salesforce
 Author: Nick Catalano
 Author-email: nickcatal@gmail.com
 Maintainer: Jonathan Wobken
 Maintainer-email: jonathanwobken@gmail.com
 License: Apache 2.0
@@ -365,15 +365,15 @@
 
 .. code-block:: python
 
    result = sf.deploy("path/to/zip", sandbox=False, **kwargs)
    asyncId = result.get('asyncId')
    state = result.get('state')
 
-Both deploy and checkDeployStatus take keyword arguements. The single package arguement is not currently available to be set for deployments. More details on the deploy options can be found at https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_deploy.htm
+Both deploy and checkDeployStatus take keyword arguments. The single package argument is not currently available to be set for deployments. More details on the deploy options can be found at https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_deploy.htm
 
 You can check on the progress of the deploy which returns a dictionary with status, state_detail, deployment_detail, unit_test_detail:
 
 .. code-block:: python
 
    sf.checkDeployStatus(asyncId)
 
@@ -443,15 +443,15 @@
     for x in sf.describe()["sobjects"]:
       print x["label"]
 
 
 Using Bulk
 --------------------------
 
-You can use this library to access Bulk API functions. The data element can be a list of records of any size and by default batch sizes are 10,000 records and run in parrallel concurrency mode. To set the batch size for insert, upsert, delete, hard_delete, and update use the batch_size argument. To set the concurrency mode for the salesforce job the use_serial argument can be set to use_serial=True.
+You can use this library to access Bulk API functions. The data element can be a list of records of any size and by default batch sizes are 10,000 records and run in parallel concurrency mode. To set the batch size for insert, upsert, delete, hard_delete, and update use the batch_size argument. To set the concurrency mode for the salesforce job the use_serial argument can be set to use_serial=True.
 
 Create new records:
 
 .. code-block:: python
 
     data = [
           {'LastName':'Smith','Email':'example@example.com'},
@@ -467,15 +467,15 @@
     data = [
           {'Id': '0000000000AAAAA', 'Email': 'examplenew@example.com'},
           {'Id': '0000000000BBBBB', 'Email': 'testnew@test.com'}
         ]
 
     sf.bulk.Contact.update(data,batch_size=10000,use_serial=True)
 
- Update existing records and update lookup fields from an external id field:
+Update existing records and update lookup fields from an external id field:
 
 .. code-block:: python
 
     data = [
           {'Id': '0000000000AAAAA', 'Custom_Object__r': {'Email__c':'examplenew@example.com'}},
           {'Id': '0000000000BBBBB', 'Custom_Object__r': {'Email__c': 'testnew@test.com'}}
         ]
@@ -689,14 +689,21 @@
 
    import pandas as pd
 
    sf.bulk.Account.query("SELECT Id, Email FROM Contact")   
    df = pd.DataFrame.from_dict(data,orient='columns').drop('attributes',axis=1)
 
 
+YouTube Tutorial
+--------------------------
+Here is a helpful  `YouTube tutorial`_  which shows how you can manage records in bulk using a jupyter notebook, simple-salesforce and pandas. 
+
+This can be a effective way to manage records, and perform simple operations like reassigning accounts, deleting test records, inserting new records, etc...
+
+.. _YouTube tutorial: https://youtu.be/nPQFUgsk6Oo?t=282
 
 Authors & License
 --------------------------
 
 This package is released under an open source Apache 2.0 license. Simple-Salesforce was originally written by `Nick Catalano`_ but most newer features and bugfixes come from `community contributors`_. Pull requests submitted to the `GitHub Repo`_ are highly encouraged!
 
 Authentication mechanisms were adapted from Dave Wingate's `RestForce`_ and licensed under a MIT license
```

### Comparing `simple-salesforce-1.12.3/README.rst` & `simple-salesforce-1.12.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,15 @@
 
 .. code-block:: python
 
    result = sf.deploy("path/to/zip", sandbox=False, **kwargs)
    asyncId = result.get('asyncId')
    state = result.get('state')
 
-Both deploy and checkDeployStatus take keyword arguements. The single package arguement is not currently available to be set for deployments. More details on the deploy options can be found at https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_deploy.htm
+Both deploy and checkDeployStatus take keyword arguments. The single package argument is not currently available to be set for deployments. More details on the deploy options can be found at https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_deploy.htm
 
 You can check on the progress of the deploy which returns a dictionary with status, state_detail, deployment_detail, unit_test_detail:
 
 .. code-block:: python
 
    sf.checkDeployStatus(asyncId)
 
@@ -415,15 +415,15 @@
     for x in sf.describe()["sobjects"]:
       print x["label"]
 
 
 Using Bulk
 --------------------------
 
-You can use this library to access Bulk API functions. The data element can be a list of records of any size and by default batch sizes are 10,000 records and run in parrallel concurrency mode. To set the batch size for insert, upsert, delete, hard_delete, and update use the batch_size argument. To set the concurrency mode for the salesforce job the use_serial argument can be set to use_serial=True.
+You can use this library to access Bulk API functions. The data element can be a list of records of any size and by default batch sizes are 10,000 records and run in parallel concurrency mode. To set the batch size for insert, upsert, delete, hard_delete, and update use the batch_size argument. To set the concurrency mode for the salesforce job the use_serial argument can be set to use_serial=True.
 
 Create new records:
 
 .. code-block:: python
 
     data = [
           {'LastName':'Smith','Email':'example@example.com'},
@@ -439,15 +439,15 @@
     data = [
           {'Id': '0000000000AAAAA', 'Email': 'examplenew@example.com'},
           {'Id': '0000000000BBBBB', 'Email': 'testnew@test.com'}
         ]
 
     sf.bulk.Contact.update(data,batch_size=10000,use_serial=True)
     
- Update existing records and update lookup fields from an external id field:
+Update existing records and update lookup fields from an external id field:
 
 .. code-block:: python
 
     data = [
           {'Id': '0000000000AAAAA', 'Custom_Object__r': {'Email__c':'examplenew@example.com'}},
           {'Id': '0000000000BBBBB', 'Custom_Object__r': {'Email__c': 'testnew@test.com'}}
         ]
@@ -661,14 +661,21 @@
    
    import pandas as pd
    
    sf.bulk.Account.query("SELECT Id, Email FROM Contact")   
    df = pd.DataFrame.from_dict(data,orient='columns').drop('attributes',axis=1)
       
 
+YouTube Tutorial
+--------------------------
+Here is a helpful  `YouTube tutorial`_  which shows how you can manage records in bulk using a jupyter notebook, simple-salesforce and pandas. 
+
+This can be a effective way to manage records, and perform simple operations like reassigning accounts, deleting test records, inserting new records, etc...
+
+.. _YouTube tutorial: https://youtu.be/nPQFUgsk6Oo?t=282
 
 Authors & License
 --------------------------
 
 This package is released under an open source Apache 2.0 license. Simple-Salesforce was originally written by `Nick Catalano`_ but most newer features and bugfixes come from `community contributors`_. Pull requests submitted to the `GitHub Repo`_ are highly encouraged!
 
 Authentication mechanisms were adapted from Dave Wingate's `RestForce`_ and licensed under a MIT license
```

### Comparing `simple-salesforce-1.12.3/setup.py` & `simple-salesforce-1.12.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,37 +22,37 @@
     license=about['__license__'],
     description=about['__description__'],
     long_description=textwrap.dedent((here / 'README.rst').read_text()),
     long_description_content_type='text/x-rst',
     package_data={
         'simple_salesforce': ['metadata.wsdl'],
         },
-install_requires = [
-                       'requests>=2.22.0',
-                       'pyjwt',
-                       'zeep'
-                       ],
-                   tests_require = [
-                                       'pytest',
-                                       'pytz>=2014.1.1',
-                                       'responses>=0.5.1',
-                                       'cryptography<3.4',
-                                       ],
-                                   test_suite = 'simple_salesforce.tests',
-                                                keywords = about[
-                                                               '__keywords__'],
-                                                           classifiers = [
-    'Development Status :: 5 - Production/Stable',
-    'License :: OSI Approved :: Apache Software License',
-    'Intended Audience :: Developers',
-    'Intended Audience :: System Administrators',
-    'Operating System :: OS Independent',
-    'Topic :: Internet :: WWW/HTTP',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-    'Programming Language :: Python :: Implementation :: PyPy'
-    ]
-)
+    install_requires = [
+        'requests>=2.22.0',
+        'cryptography',
+        'zeep',
+        'pyjwt'
+        ],
+    tests_require = [
+        'pytest',
+        'pytz>=2014.1.1',
+        'responses>=0.5.1',
+        'cryptography<3.4',
+        ],
+    test_suite = 'simple_salesforce.tests',
+    keywords = about['__keywords__'],
+    classifiers = [
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: Apache Software License',
+        'Intended Audience :: Developers',
+        'Intended Audience :: System Administrators',
+        'Operating System :: OS Independent',
+        'Topic :: Internet :: WWW/HTTP',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: Implementation :: PyPy'
+        ]
+)
```

### Comparing `simple-salesforce-1.12.3/simple_salesforce/__init__.py` & `simple-salesforce-1.12.4/simple_salesforce/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.3/simple_salesforce/__version__.py` & `simple-salesforce-1.12.4/simple_salesforce/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Version details for simple-salesforce
 
 This file shamelessly taken from the requests library"""
 
 __title__ = 'simple-salesforce'
 __description__ = 'A basic Salesforce.com REST API client.'
 __url__ = 'https://github.com/simple-salesforce/simple-salesforce'
-__version__ = '1.12.3'
+__version__ = '1.12.4'
 __author__ = 'Nick Catalano'
 __author_email__ = 'nickcatal@gmail.com'
 __license__ = 'Apache 2.0'
 __maintainer__ = 'Jonathan Wobken'
 __maintainer_email__ = 'jonathanwobken@gmail.com'
 __keywords__ = 'python salesforce salesforce.com'
```

### Comparing `simple-salesforce-1.12.3/simple_salesforce/api.py` & `simple-salesforce-1.12.4/simple_salesforce/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,16 @@
         if name == 'bulk':
             # Deal with bulk API functions
             return SFBulkHandler(self.session_id, self.bulk_url, self.proxies,
                                  self.session)
 
         return SFType(
             name, self.session_id, self.sf_instance, sf_version=self.sf_version,
-            proxies=self.proxies, session=self.session, salesforce=self)
+            proxies=self.proxies, session=self.session, salesforce=self,
+            object_pairs_hook=self._object_pairs_hook)
 
     # User utility methods
     def set_password(self, user, password):
         """Sets the password of a user
         salesforce dev documentation link:
         https://www.salesforce.com/us/developer/docs/api_rest/Content
         /dome_sobject_user_password.htm
```

### Comparing `simple-salesforce-1.12.3/simple_salesforce/bulk.py` & `simple-salesforce-1.12.4/simple_salesforce/bulk.py`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.3/simple_salesforce/exceptions.py` & `simple-salesforce-1.12.4/simple_salesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.3/simple_salesforce/format.py` & `simple-salesforce-1.12.4/simple_salesforce/format.py`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.3/simple_salesforce/login.py` & `simple-salesforce-1.12.4/simple_salesforce/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 </soapenv:Envelope>"""
     elif username is not None and \
             consumer_key is not None and \
             (privatekey_file is not None or privatekey is not None):
         expiration = datetime.now(timezone.utc) + timedelta(minutes=3)
         payload = {
             'iss': consumer_key,
-            'sub': username,
+            'sub': unescape(username),
             'aud': f'https://{domain}.salesforce.com',
             'exp': f'{expiration.timestamp():.0f}'
             }
         if privatekey_file is not None:
             key = Path(privatekey_file).read_bytes()
         else:
             key = privatekey
```

### Comparing `simple-salesforce-1.12.3/simple_salesforce/messages.py` & `simple-salesforce-1.12.4/simple_salesforce/messages.py`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.3/simple_salesforce/metadata.py` & `simple-salesforce-1.12.4/simple_salesforce/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         """
         self._name = name
         self._service = service
         self._zeep_type = zeep_type
         self._session_header = session_header
 
     @staticmethod
+    # pylint: disable=broad-exception-raised
     def _handle_api_response(response):
         """
         Parses SaveResult and DeleteResult objects to identify if there was
         an error, and raises exception accordingly
 
         :param response: List of zeep.objects.SaveResult or
         zeep.objects.DeleteResult objects
@@ -322,14 +323,15 @@
         if hasattr(zipfile, 'read'):
             zipfile.seek(0)
             raw = zipfile.read()
         else:
             raw = Path(zipfile).read_bytes()
         return b64encode(raw).decode()
 
+    # pylint: disable=broad-exception-raised
     def _retrieve_deploy_result(self, async_process_id, **kwargs):
         """ Retrieves status for specified deployment id
         :param async_process_id:
         :type async_process_id:
         :param kwargs:
         :type kwargs:
         :return:
@@ -499,14 +501,15 @@
             self._XML_NAMESPACES).text
         state = ET.fromstring(res.text).find(
             'soapenv:Body/mt:retrieveResponse/mt:result/mt:state',
             self._XML_NAMESPACES).text
 
         return async_process_id, state
 
+    # pylint: disable=broad-exception-raised
     def retrieve_retrieve_result(self, async_process_id, include_zip, **kwargs):
         """ Retrieves status for specified retrieval id """
         client = kwargs.get('client', 'simple_salesforce_metahelper')
         attributes = {
             'client': client,
             'sessionId': self._session_id,
             'asyncProcessId': async_process_id,
```

### Comparing `simple-salesforce-1.12.3/simple_salesforce/metadata.wsdl` & `simple-salesforce-1.12.4/simple_salesforce/metadata.wsdl`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.3/simple_salesforce/util.py` & `simple-salesforce-1.12.4/simple_salesforce/util.py`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.3/simple_salesforce.egg-info/PKG-INFO` & `simple-salesforce-1.12.4/simple_salesforce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-salesforce
-Version: 1.12.3
+Version: 1.12.4
 Summary: A basic Salesforce.com REST API client.
 Home-page: https://github.com/simple-salesforce/simple-salesforce
 Author: Nick Catalano
 Author-email: nickcatal@gmail.com
 Maintainer: Jonathan Wobken
 Maintainer-email: jonathanwobken@gmail.com
 License: Apache 2.0
@@ -365,15 +365,15 @@
 
 .. code-block:: python
 
    result = sf.deploy("path/to/zip", sandbox=False, **kwargs)
    asyncId = result.get('asyncId')
    state = result.get('state')
 
-Both deploy and checkDeployStatus take keyword arguements. The single package arguement is not currently available to be set for deployments. More details on the deploy options can be found at https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_deploy.htm
+Both deploy and checkDeployStatus take keyword arguments. The single package argument is not currently available to be set for deployments. More details on the deploy options can be found at https://developer.salesforce.com/docs/atlas.en-us.api_meta.meta/api_meta/meta_deploy.htm
 
 You can check on the progress of the deploy which returns a dictionary with status, state_detail, deployment_detail, unit_test_detail:
 
 .. code-block:: python
 
    sf.checkDeployStatus(asyncId)
 
@@ -443,15 +443,15 @@
     for x in sf.describe()["sobjects"]:
       print x["label"]
 
 
 Using Bulk
 --------------------------
 
-You can use this library to access Bulk API functions. The data element can be a list of records of any size and by default batch sizes are 10,000 records and run in parrallel concurrency mode. To set the batch size for insert, upsert, delete, hard_delete, and update use the batch_size argument. To set the concurrency mode for the salesforce job the use_serial argument can be set to use_serial=True.
+You can use this library to access Bulk API functions. The data element can be a list of records of any size and by default batch sizes are 10,000 records and run in parallel concurrency mode. To set the batch size for insert, upsert, delete, hard_delete, and update use the batch_size argument. To set the concurrency mode for the salesforce job the use_serial argument can be set to use_serial=True.
 
 Create new records:
 
 .. code-block:: python
 
     data = [
           {'LastName':'Smith','Email':'example@example.com'},
@@ -467,15 +467,15 @@
     data = [
           {'Id': '0000000000AAAAA', 'Email': 'examplenew@example.com'},
           {'Id': '0000000000BBBBB', 'Email': 'testnew@test.com'}
         ]
 
     sf.bulk.Contact.update(data,batch_size=10000,use_serial=True)
 
- Update existing records and update lookup fields from an external id field:
+Update existing records and update lookup fields from an external id field:
 
 .. code-block:: python
 
     data = [
           {'Id': '0000000000AAAAA', 'Custom_Object__r': {'Email__c':'examplenew@example.com'}},
           {'Id': '0000000000BBBBB', 'Custom_Object__r': {'Email__c': 'testnew@test.com'}}
         ]
@@ -689,14 +689,21 @@
 
    import pandas as pd
 
    sf.bulk.Account.query("SELECT Id, Email FROM Contact")   
    df = pd.DataFrame.from_dict(data,orient='columns').drop('attributes',axis=1)
 
 
+YouTube Tutorial
+--------------------------
+Here is a helpful  `YouTube tutorial`_  which shows how you can manage records in bulk using a jupyter notebook, simple-salesforce and pandas. 
+
+This can be a effective way to manage records, and perform simple operations like reassigning accounts, deleting test records, inserting new records, etc...
+
+.. _YouTube tutorial: https://youtu.be/nPQFUgsk6Oo?t=282
 
 Authors & License
 --------------------------
 
 This package is released under an open source Apache 2.0 license. Simple-Salesforce was originally written by `Nick Catalano`_ but most newer features and bugfixes come from `community contributors`_. Pull requests submitted to the `GitHub Repo`_ are highly encouraged!
 
 Authentication mechanisms were adapted from Dave Wingate's `RestForce`_ and licensed under a MIT license
```

### Comparing `simple-salesforce-1.12.3/simple_salesforce.egg-info/SOURCES.txt` & `simple-salesforce-1.12.4/simple_salesforce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

