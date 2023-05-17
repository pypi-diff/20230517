# Comparing `tmp/platinumtools-0.2.tar.gz` & `tmp/platinumtools-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platinumtools-0.2.tar", last modified: Wed May 17 19:51:35 2023, max compression
+gzip compressed data, was "platinumtools-0.3.tar", last modified: Wed May 17 20:05:44 2023, max compression
```

## Comparing `platinumtools-0.2.tar` & `platinumtools-0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 19:51:35.099927 platinumtools-0.2/
--rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.2/LICENSE
--rw-rw-rw-   0        0        0      861 2023-05-17 19:51:35.098932 platinumtools-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 19:51:35.019116 platinumtools-0.2/platinumtools/
--rw-rw-rw-   0        0        0      423 2023-05-16 18:33:49.000000 platinumtools-0.2/platinumtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:51:35.076929 platinumtools-0.2/platinumtools/aws_classes/
--rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.2/platinumtools/aws_classes/CommonProcesor.py
--rw-rw-rw-   0        0        0     2408 2023-05-16 18:16:53.000000 platinumtools-0.2/platinumtools/aws_classes/JobListener.py
--rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 platinumtools-0.2/platinumtools/aws_classes/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.2/platinumtools/aws_classes/class_adapters.py
--rw-rw-rw-   0        0        0    28031 2023-05-17 19:49:36.000000 platinumtools-0.2/platinumtools/aws_classes/class_enhancement.py
--rw-rw-rw-   0        0        0     2296 2023-02-16 19:18:53.000000 platinumtools-0.2/platinumtools/aws_classes/class_guardian.py
--rw-rw-rw-   0        0        0    15737 2023-05-17 15:12:57.000000 platinumtools-0.2/platinumtools/aws_classes/class_helpers.py
--rw-rw-rw-   0        0        0     1789 2023-02-21 20:05:33.000000 platinumtools-0.2/platinumtools/aws_classes/class_scheduling.py
--rw-rw-rw-   0        0        0     7191 2023-05-17 16:26:56.000000 platinumtools-0.2/platinumtools/aws_classes/config_mapper.py
--rw-rw-rw-   0        0        0    19732 2023-05-17 16:45:45.000000 platinumtools-0.2/platinumtools/aws_classes/config_mapper_df.py
--rw-rw-rw-   0        0        0    20802 2023-05-17 16:22:55.000000 platinumtools-0.2/platinumtools/dda_constants.py
--rw-rw-rw-   0        0        0     8070 2023-05-17 15:42:43.000000 platinumtools-0.2/platinumtools/dda_models.py
--rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.2/platinumtools/etl_functions.py
--rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 platinumtools-0.2/platinumtools/help.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:51:35.059413 platinumtools-0.2/platinumtools.egg-info/
--rw-rw-rw-   0        0        0      861 2023-05-17 19:51:34.000000 platinumtools-0.2/platinumtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-05-17 19:51:34.000000 platinumtools-0.2/platinumtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 19:51:34.000000 platinumtools-0.2/platinumtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-17 19:51:34.000000 platinumtools-0.2/platinumtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 19:51:35.100924 platinumtools-0.2/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-05-17 19:51:23.000000 platinumtools-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:51:35.097931 platinumtools-0.2/test_scenarios/
--rw-rw-rw-   0        0        0     4592 2023-05-17 18:21:56.000000 platinumtools-0.2/test_scenarios/JobListener.py
--rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.2/test_scenarios/__init__.py
--rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 platinumtools-0.2/test_scenarios/test_adapters.py
--rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.2/test_scenarios/test_code.py
--rw-rw-rw-   0        0        0     4167 2023-05-17 15:35:30.000000 platinumtools-0.2/test_scenarios/test_common_processing.py
--rw-rw-rw-   0        0        0    26979 2023-05-17 15:29:56.000000 platinumtools-0.2/test_scenarios/test_enhancement.py
--rw-rw-rw-   0        0        0    20476 2023-05-17 15:34:29.000000 platinumtools-0.2/test_scenarios/test_event_normalization.py
--rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.2/test_scenarios/test_guardian.py
--rw-rw-rw-   0        0        0     4605 2023-05-17 15:23:32.000000 platinumtools-0.2/test_scenarios/test_helpers.py
--rw-rw-rw-   0        0        0     5427 2023-05-17 15:23:32.000000 platinumtools-0.2/test_scenarios/test_scheduling.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:05:44.637893 platinumtools-0.3/
+-rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.3/LICENSE
+-rw-rw-rw-   0        0        0      861 2023-05-17 20:05:44.635864 platinumtools-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 20:05:44.540978 platinumtools-0.3/platinumtools/
+-rw-rw-rw-   0        0        0      423 2023-05-16 18:33:49.000000 platinumtools-0.3/platinumtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:05:44.608231 platinumtools-0.3/platinumtools/aws_classes/
+-rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.3/platinumtools/aws_classes/CommonProcesor.py
+-rw-rw-rw-   0        0        0     2408 2023-05-16 18:16:53.000000 platinumtools-0.3/platinumtools/aws_classes/JobListener.py
+-rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 platinumtools-0.3/platinumtools/aws_classes/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.3/platinumtools/aws_classes/class_adapters.py
+-rw-rw-rw-   0        0        0    28035 2023-05-17 20:04:01.000000 platinumtools-0.3/platinumtools/aws_classes/class_enhancement.py
+-rw-rw-rw-   0        0        0     2296 2023-02-16 19:18:53.000000 platinumtools-0.3/platinumtools/aws_classes/class_guardian.py
+-rw-rw-rw-   0        0        0    16271 2023-05-17 20:00:11.000000 platinumtools-0.3/platinumtools/aws_classes/class_helpers.py
+-rw-rw-rw-   0        0        0     1789 2023-02-21 20:05:33.000000 platinumtools-0.3/platinumtools/aws_classes/class_scheduling.py
+-rw-rw-rw-   0        0        0     7191 2023-05-17 16:26:56.000000 platinumtools-0.3/platinumtools/aws_classes/config_mapper.py
+-rw-rw-rw-   0        0        0    19732 2023-05-17 16:45:45.000000 platinumtools-0.3/platinumtools/aws_classes/config_mapper_df.py
+-rw-rw-rw-   0        0        0    20802 2023-05-17 16:22:55.000000 platinumtools-0.3/platinumtools/dda_constants.py
+-rw-rw-rw-   0        0        0     8070 2023-05-17 15:42:43.000000 platinumtools-0.3/platinumtools/dda_models.py
+-rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.3/platinumtools/etl_functions.py
+-rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 platinumtools-0.3/platinumtools/help.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:05:44.577339 platinumtools-0.3/platinumtools.egg-info/
+-rw-rw-rw-   0        0        0      861 2023-05-17 20:05:43.000000 platinumtools-0.3/platinumtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2023-05-17 20:05:44.000000 platinumtools-0.3/platinumtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 20:05:43.000000 platinumtools-0.3/platinumtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-17 20:05:43.000000 platinumtools-0.3/platinumtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 20:05:44.638894 platinumtools-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-05-17 20:05:18.000000 platinumtools-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:05:44.633350 platinumtools-0.3/test_scenarios/
+-rw-rw-rw-   0        0        0     4592 2023-05-17 18:21:56.000000 platinumtools-0.3/test_scenarios/JobListener.py
+-rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.3/test_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 platinumtools-0.3/test_scenarios/test_adapters.py
+-rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.3/test_scenarios/test_code.py
+-rw-rw-rw-   0        0        0     4203 2023-05-17 19:56:18.000000 platinumtools-0.3/test_scenarios/test_common_processing.py
+-rw-rw-rw-   0        0        0    26979 2023-05-17 15:29:56.000000 platinumtools-0.3/test_scenarios/test_enhancement.py
+-rw-rw-rw-   0        0        0    20476 2023-05-17 15:34:29.000000 platinumtools-0.3/test_scenarios/test_event_normalization.py
+-rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.3/test_scenarios/test_guardian.py
+-rw-rw-rw-   0        0        0     4605 2023-05-17 15:23:32.000000 platinumtools-0.3/test_scenarios/test_helpers.py
+-rw-rw-rw-   0        0        0     5427 2023-05-17 15:23:32.000000 platinumtools-0.3/test_scenarios/test_scheduling.py
```

### Comparing `platinumtools-0.2/LICENSE` & `platinumtools-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/PKG-INFO` & `platinumtools-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.2
+Version: 0.3
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.2/platinumtools/aws_classes/CommonProcesor.py` & `platinumtools-0.3/platinumtools/aws_classes/CommonProcesor.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools/aws_classes/JobListener.py` & `platinumtools-0.3/platinumtools/aws_classes/JobListener.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools/aws_classes/class_adapters.py` & `platinumtools-0.3/platinumtools/aws_classes/class_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools/aws_classes/class_enhancement.py` & `platinumtools-0.3/platinumtools/aws_classes/class_enhancement.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,16 @@
                 title=event["title"] if "title" in event else "",
                 url=event["url"] if "url" in event else "",
                 attachments=event["files"] if  "files" in event else {},
                 action_origin=eventActiveStatus(event),
                 span_guid=span_guid,
                 root_reference= "IS_ROOT" if is_root else root_reference,
                 root_duration=total_duration if is_root else 0,
-                root_start = event["startTime"] if is_root and "startTime" in event else "",
-                root_end = event["endTime"] if is_root and "endTime" in event else "",
+                root_start = event["startTime"] if is_root and "startTime" in event else None,
+                root_end = event["endTime"] if is_root and "endTime" in event else None,
             )
 
             new_details.append(fileEvent.to_dict())
 
         management_api.details = new_details # Replace with updated interfaces
 
         return management_api.to_dict()
```

### Comparing `platinumtools-0.2/platinumtools/aws_classes/class_guardian.py` & `platinumtools-0.3/platinumtools/aws_classes/class_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools/aws_classes/class_helpers.py` & `platinumtools-0.3/platinumtools/aws_classes/class_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,23 +127,32 @@
 
         import json
         from typing import List
 
         def cleanQueryArgument(queryArgument):
             # If the queryArg is a list or dict, format it into a way that is query insertable
             if isinstance(queryArgument, (dict)):
+                # If the is List and the first element is a dict, then it is a list of objects
                 return json.dumps(queryArgument)
+            if isinstance(queryArgument, List) and len(queryArgument) >0 and isinstance(queryArgument[0], dict):
+                # return an array of strings of the json
+                for(i, item) in enumerate(queryArgument):
+                    queryArgument[i] = cleanQueryArgument(item)
+            
             return queryArgument
 
         for row in events:
             values = []
             for col in column_names:
                 value = row.get(col, None)
                 values.append(cleanQueryArgument(value))
-            self.cursor.execute(insert_sql, values)
+            try:
+                self.cursor.execute(insert_sql, values)
+            except Exception as e:
+                print("Exception at publish:", e, "values:", values)
         self.connection.commit()
 
     
     def getOne(self, key_value, key_column: str = "guid"):
         """Gets one
         Expected parameters to have under settings:
         - TABLENAME
```

### Comparing `platinumtools-0.2/platinumtools/aws_classes/class_scheduling.py` & `platinumtools-0.3/platinumtools/aws_classes/class_scheduling.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools/aws_classes/config_mapper.py` & `platinumtools-0.3/platinumtools/aws_classes/config_mapper.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools/aws_classes/config_mapper_df.py` & `platinumtools-0.3/platinumtools/aws_classes/config_mapper_df.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools/dda_constants.py` & `platinumtools-0.3/platinumtools/dda_constants.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools/dda_models.py` & `platinumtools-0.3/platinumtools/dda_models.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/platinumtools.egg-info/PKG-INFO` & `platinumtools-0.3/platinumtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.2
+Version: 0.3
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.2/platinumtools.egg-info/SOURCES.txt` & `platinumtools-0.3/platinumtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/setup.py` & `platinumtools-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2'
+VERSION = '0.3'
 DESCRIPTION = 'DDAPP Modules'
 LONG_DESCRIPTION = 'Common Constants, classes and methods for ETL and other python projects'
 
 # Setting up
 #nenewang08
 setup(
     name="platinumtools",
```

### Comparing `platinumtools-0.2/test_scenarios/JobListener.py` & `platinumtools-0.3/test_scenarios/JobListener.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/test_scenarios/test_adapters.py` & `platinumtools-0.3/test_scenarios/test_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/test_scenarios/test_common_processing.py` & `platinumtools-0.3/test_scenarios/test_common_processing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import pytest
 from platinumtools.aws_classes.class_enhancement import *
 from platinumtools.dda_constants import *
 
 
 
 
-@pytest.fixture
-def common_processor_using_mock():
+# def common_processor_using_mock():
 
-    publisher_credentials = {}
-    publisher_settings = {}
+#     publisher_credentials = {}
+#     publisher_settings = {}
 
-    organizationDBProvider = MockOrganizationQuerier
-    publishingDBProvider = MockStagingDatabaseProviderWithChrome(credentials=publisher_credentials, settings=publisher_settings)
-    processor = BetterCommonProcessor(
-        job_parameters={"guid": "387a26ff-ceed-5015-a6c9-a2cad90329c0" },
-        organization_provider=organizationDBProvider,
-        publishingDBProvider=publishingDBProvider
-    ) # Should expect for transformation Strategies to be automatically updated
+#     organizationDBProvider = MockOrganizationQuerier
+#     publishingDBProvider = MockStagingDatabaseProviderWithChrome(credentials=publisher_credentials, settings=publisher_settings)
+#     processor = BetterCommonProcessor(
+#         job_parameters={"guid": "387a26ff-ceed-5015-a6c9-a2cad90329c0" },
+#         organization_provider=organizationDBProvider,
+#         publishingDBProvider=publishingDBProvider
+#     ) # Should expect for transformation Strategies to be automatically updated
 
-    return processor
+#     return processor
 
-# def test_picks_chrome_enhancement_instantiation(common_processor_using_mock):
-#     processor = common_processor_using_mock
-#     processor.runJobs() # Should also post at the Mock Database
+# # def test_picks_chrome_enhancement_instantiation(common_processor_using_mock):
+# #     processor = common_processor_using_mock
+# #     processor.runJobs() # Should also post at the Mock Database
 
 
-def test_picks_salesforce_enhancement():
+# def test_picks_salesforce_enhancement():
     
-    organizationDBProvider = MockOrganizationQuerier
-    publishingDBProvider = MockStagingDatabaseProviderWithChrome(credentials={}, settings={})
-    processor = BetterCommonProcessor(
-        job_parameters={"guid": "f27ecb0c-975d-dbac-82af-152b68e89902" },
-        organization_provider=organizationDBProvider,
-        publishingDBProvider=publishingDBProvider
-    ) # Should expect for transformation Strategies to be automatically updated
+#     organizationDBProvider = MockOrganizationQuerier
+#     publishingDBProvider = MockStagingDatabaseProviderWithChrome(credentials={}, settings={})
+#     processor = BetterCommonProcessor(
+#         job_parameters={"guid": "f27ecb0c-975d-dbac-82af-152b68e89902" },
+#         organization_provider=organizationDBProvider,
+#         publishingDBProvider=publishingDBProvider
+#     ) # Should expect for transformation Strategies to be automatically updated
     
-    processor.runJobs() # Should also post at the Mock Database
+#     processor.runJobs() # Should also post at the Mock Database
 
 
 def test_picks_real_job():
     
     organizationDBProvider = MockOrganizationQuerier
     
     credentials = {
@@ -100,14 +99,14 @@
                         "root_duration"
                         ]
 
     }
     publishingDBProvider = PostgreSQLProvider(credentials=credentials, settings=settings)
 
     processor = BetterCommonProcessor(
-        job_parameters={"guid": "17eee0ff-053f-025a-8913-257f761cb002",
+        job_parameters={"guid": "387a26ff-ceed-5015-a6c9-adasd45sdasd1a2saas",
                        },
         organization_provider=organizationDBProvider,
         publishingDBProvider=publishingDBProvider
     ) 
     
     processor.runJobs() # Should also post at the Mock Database
```

### Comparing `platinumtools-0.2/test_scenarios/test_enhancement.py` & `platinumtools-0.3/test_scenarios/test_enhancement.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/test_scenarios/test_event_normalization.py` & `platinumtools-0.3/test_scenarios/test_event_normalization.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/test_scenarios/test_guardian.py` & `platinumtools-0.3/test_scenarios/test_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/test_scenarios/test_helpers.py` & `platinumtools-0.3/test_scenarios/test_helpers.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.2/test_scenarios/test_scheduling.py` & `platinumtools-0.3/test_scenarios/test_scheduling.py`

 * *Files identical despite different names*

