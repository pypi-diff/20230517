# Comparing `tmp/feature_service_client-0.1.0.tar.gz` & `tmp/feature_service_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_service_client-0.1.0.tar", max compression
+gzip compressed data, was "feature_service_client-0.1.1.tar", max compression
```

## Comparing `feature_service_client-0.1.0.tar` & `feature_service_client-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4341 2023-05-08 18:13:02.350057 feature_service_client-0.1.0/README.md
--rw-r--r--   0        0        0      765 2023-05-08 15:55:30.112403 feature_service_client-0.1.0/feature_service_client/__init__.py
--rw-r--r--   0        0        0      226 2023-05-08 15:55:30.112817 feature_service_client-0.1.0/feature_service_client/api/__init__.py
--rw-r--r--   0        0        0    13954 2023-05-08 15:55:30.100933 feature_service_client-0.1.0/feature_service_client/api/default_api.py
--rw-r--r--   0        0        0    37545 2023-05-08 15:55:30.114842 feature_service_client-0.1.0/feature_service_client/api_client.py
--rw-r--r--   0        0        0      475 2023-05-08 15:55:30.119976 feature_service_client-0.1.0/feature_service_client/apis/__init__.py
--rw-r--r--   0        0        0    16165 2023-05-08 15:55:30.111742 feature_service_client-0.1.0/feature_service_client/configuration.py
--rw-r--r--   0        0        0     5023 2023-05-08 15:55:30.113366 feature_service_client-0.1.0/feature_service_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-05-08 15:55:30.119625 feature_service_client-0.1.0/feature_service_client/model/__init__.py
--rw-r--r--   0        0        0    11895 2023-05-08 15:55:30.055238 feature_service_client-0.1.0/feature_service_client/model/columnar_features_response.py
--rw-r--r--   0        0        0    11379 2023-05-08 15:55:30.065678 feature_service_client-0.1.0/feature_service_client/model/feature_column.py
--rw-r--r--   0        0        0    12048 2023-05-08 15:55:30.071040 feature_service_client-0.1.0/feature_service_client/model/feature_request_data.py
--rw-r--r--   0        0        0    11365 2023-05-08 15:55:30.075279 feature_service_client-0.1.0/feature_service_client/model/feature_value.py
--rw-r--r--   0        0        0    12455 2023-05-08 15:55:30.079466 feature_service_client-0.1.0/feature_service_client/model/features_request.py
--rw-r--r--   0        0        0    11661 2023-05-08 15:55:30.082859 feature_service_client-0.1.0/feature_service_client/model/seldon_features_request.py
--rw-r--r--   0        0        0    81853 2023-05-08 15:55:30.118637 feature_service_client-0.1.0/feature_service_client/model_utils.py
--rw-r--r--   0        0        0      857 2023-05-08 15:55:30.119235 feature_service_client-0.1.0/feature_service_client/models/__init__.py
--rw-r--r--   0        0        0    14155 2023-05-08 15:55:30.115802 feature_service_client-0.1.0/feature_service_client/rest.py
--rw-r--r--   0        0        0      373 2023-05-08 18:19:52.064793 feature_service_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4934 1970-01-01 00:00:00.000000 feature_service_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4012 2023-05-17 13:01:31.027746 feature_service_client-0.1.1/README.md
+-rw-r--r--   0        0        0      765 2023-05-16 17:08:59.486758 feature_service_client-0.1.1/feature_service_client/__init__.py
+-rw-r--r--   0        0        0      226 2023-05-16 17:08:59.486932 feature_service_client-0.1.1/feature_service_client/api/__init__.py
+-rw-r--r--   0        0        0    13954 2023-05-16 17:08:59.487091 feature_service_client-0.1.1/feature_service_client/api/default_api.py
+-rw-r--r--   0        0        0    37545 2023-05-16 17:08:59.487360 feature_service_client-0.1.1/feature_service_client/api_client.py
+-rw-r--r--   0        0        0      475 2023-05-16 17:08:59.487568 feature_service_client-0.1.1/feature_service_client/apis/__init__.py
+-rw-r--r--   0        0        0    16165 2023-05-16 17:08:59.487742 feature_service_client-0.1.1/feature_service_client/configuration.py
+-rw-r--r--   0        0        0     5023 2023-05-16 17:08:59.487877 feature_service_client-0.1.1/feature_service_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-05-16 17:08:59.488066 feature_service_client-0.1.1/feature_service_client/model/__init__.py
+-rw-r--r--   0        0        0    11895 2023-05-16 17:08:59.488200 feature_service_client-0.1.1/feature_service_client/model/columnar_features_response.py
+-rw-r--r--   0        0        0    11379 2023-05-16 17:08:59.488313 feature_service_client-0.1.1/feature_service_client/model/feature_column.py
+-rw-r--r--   0        0        0    12048 2023-05-16 17:08:59.488446 feature_service_client-0.1.1/feature_service_client/model/feature_request_data.py
+-rw-r--r--   0        0        0    11365 2023-05-16 17:08:59.488562 feature_service_client-0.1.1/feature_service_client/model/feature_value.py
+-rw-r--r--   0        0        0    12455 2023-05-16 17:08:59.488723 feature_service_client-0.1.1/feature_service_client/model/features_request.py
+-rw-r--r--   0        0        0    11661 2023-05-16 17:08:59.488861 feature_service_client-0.1.1/feature_service_client/model/seldon_features_request.py
+-rw-r--r--   0        0        0    81857 2023-05-16 17:08:59.489259 feature_service_client-0.1.1/feature_service_client/model_utils.py
+-rw-r--r--   0        0        0      857 2023-05-16 17:08:59.489467 feature_service_client-0.1.1/feature_service_client/models/__init__.py
+-rw-r--r--   0        0        0    14155 2023-05-16 17:08:59.489636 feature_service_client-0.1.1/feature_service_client/rest.py
+-rw-r--r--   0        0        0      373 2023-05-17 17:59:37.841119 feature_service_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 feature_service_client-0.1.1/PKG-INFO
```

### Comparing `feature_service_client-0.1.0/README.md` & `feature_service_client-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://gitlab.dev.tripadvisor.com/tamg-ml/feature-service-client.git
+pip install feature_service_client
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://gitlab.dev.tripadvisor.com/tamg-ml/feature-service-client.git`)
+(you may need to run `pip` with root permission: `sudo pip install feature_service_client`)
 
 Then import the package:
 ```python
 import feature_service_client
 ```
 
 ### Setuptools
@@ -42,52 +42,43 @@
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import time
 import feature_service_client
 from pprint import pprint
 from feature_service_client.api import default_api
 from feature_service_client.model.columnar_features_response import ColumnarFeaturesResponse
 from feature_service_client.model.features_request import FeaturesRequest
 from feature_service_client.model.seldon_features_request import SeldonFeaturesRequest
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = feature_service_client.Configuration(
-    host = "http://localhost"
+    host = "https://service.mlplat-service-sbx.tamg.cloud"
 )
-
-
-
 # Enter a context with an instance of the API client
-with feature_service_client.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = default_api.DefaultApi(api_client)
-    features_request = FeaturesRequest(
-        features=[
-            "features_example",
-        ],
-        entity_ids=[
-            "entity_ids_example",
-        ],
-        user_id="user_id_example",
-        facebook_id="facebook_id_example",
-        ta_unique_id="ta_unique_id_example",
-        context={},
-        client_name="client_name_example",
-    ) # FeaturesRequest | 
-
-    try:
-        api_response = api_instance.get_columnar_features(features_request)
-        pprint(api_response)
-    except feature_service_client.ApiException as e:
-        print("Exception when calling DefaultApi->get_columnar_features: %s\n" % e)
+api_client = feature_service_client.ApiClient(configuration)
+api_instance = default_api.DefaultApi(api_client)
+
+features_request = FeaturesRequest(
+    features=[
+        "TA_User_AdsolAudienceIds","TA_User_CompletedInstantBookingsLast28Days","TA_User_DatedSearchLast28Days"
+    ],
+    entity_ids=[],
+    user_id="",
+    facebook_id="",
+    ta_unique_id="f371a31f-6cc6-545a-9b8a-a270c4d7f884",
+    context={},
+    client_name="joao-test",
+) # FeaturesRequest | 
+    
+api_response = api_instance.get_columnar_features(features_request)
+pprint(api_response)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
```

### Comparing `feature_service_client-0.1.0/feature_service_client/__init__.py` & `feature_service_client-0.1.1/feature_service_client/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/api/default_api.py` & `feature_service_client-0.1.1/feature_service_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/api_client.py` & `feature_service_client-0.1.1/feature_service_client/api_client.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/configuration.py` & `feature_service_client-0.1.1/feature_service_client/configuration.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/exceptions.py` & `feature_service_client-0.1.1/feature_service_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/model/columnar_features_response.py` & `feature_service_client-0.1.1/feature_service_client/model/columnar_features_response.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/model/feature_column.py` & `feature_service_client-0.1.1/feature_service_client/model/feature_column.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/model/feature_request_data.py` & `feature_service_client-0.1.1/feature_service_client/model/feature_request_data.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/model/feature_value.py` & `feature_service_client-0.1.1/feature_service_client/model/feature_value.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/model/features_request.py` & `feature_service_client-0.1.1/feature_service_client/model/features_request.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/model/seldon_features_request.py` & `feature_service_client-0.1.1/feature_service_client/model/seldon_features_request.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/model_utils.py` & `feature_service_client-0.1.1/feature_service_client/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1437,20 +1437,20 @@
         ApiTypeError
         ApiValueError
         ApiKeyError
     """
     valid_classes_ordered = order_response_types(valid_classes)
     valid_classes_coercible = remove_uncoercible(
         valid_classes_ordered, input_value, spec_property_naming)
-    if not valid_classes_coercible or key_type:
+    #if not valid_classes_coercible or key_type:
         # we do not handle keytype errors, json will take care
         # of this for us
-        if configuration is None or not configuration.discard_unknown_keys:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=key_type)
+        #if configuration is None or not configuration.discard_unknown_keys:
+            #raise get_type_error(input_value, path_to_item, valid_classes,
+            #                     key_type=key_type)
     for valid_class in valid_classes_coercible:
         try:
             if issubclass(valid_class, OpenApiModel):
                 return deserialize_model(input_value, valid_class,
                                          path_to_item, check_type,
                                          configuration, spec_property_naming)
             elif valid_class == file_type:
```

### Comparing `feature_service_client-0.1.0/feature_service_client/models/__init__.py` & `feature_service_client-0.1.1/feature_service_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/feature_service_client/rest.py` & `feature_service_client-0.1.1/feature_service_client/rest.py`

 * *Files identical despite different names*

### Comparing `feature_service_client-0.1.0/PKG-INFO` & `feature_service_client-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-service-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: python client for talking to feature service
 Author: Long Yao
 Author-email: l2yao@tripadvisor.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -29,17 +29,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://gitlab.dev.tripadvisor.com/tamg-ml/feature-service-client.git
+pip install feature_service_client
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://gitlab.dev.tripadvisor.com/tamg-ml/feature-service-client.git`)
+(you may need to run `pip` with root permission: `sudo pip install feature_service_client`)
 
 Then import the package:
 ```python
 import feature_service_client
 ```
 
 ### Setuptools
@@ -58,52 +58,43 @@
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import time
 import feature_service_client
 from pprint import pprint
 from feature_service_client.api import default_api
 from feature_service_client.model.columnar_features_response import ColumnarFeaturesResponse
 from feature_service_client.model.features_request import FeaturesRequest
 from feature_service_client.model.seldon_features_request import SeldonFeaturesRequest
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = feature_service_client.Configuration(
-    host = "http://localhost"
+    host = "https://service.mlplat-service-sbx.tamg.cloud"
 )
-
-
-
 # Enter a context with an instance of the API client
-with feature_service_client.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = default_api.DefaultApi(api_client)
-    features_request = FeaturesRequest(
-        features=[
-            "features_example",
-        ],
-        entity_ids=[
-            "entity_ids_example",
-        ],
-        user_id="user_id_example",
-        facebook_id="facebook_id_example",
-        ta_unique_id="ta_unique_id_example",
-        context={},
-        client_name="client_name_example",
-    ) # FeaturesRequest | 
-
-    try:
-        api_response = api_instance.get_columnar_features(features_request)
-        pprint(api_response)
-    except feature_service_client.ApiException as e:
-        print("Exception when calling DefaultApi->get_columnar_features: %s\n" % e)
+api_client = feature_service_client.ApiClient(configuration)
+api_instance = default_api.DefaultApi(api_client)
+
+features_request = FeaturesRequest(
+    features=[
+        "TA_User_AdsolAudienceIds","TA_User_CompletedInstantBookingsLast28Days","TA_User_DatedSearchLast28Days"
+    ],
+    entity_ids=[],
+    user_id="",
+    facebook_id="",
+    ta_unique_id="f371a31f-6cc6-545a-9b8a-a270c4d7f884",
+    context={},
+    client_name="joao-test",
+) # FeaturesRequest | 
+    
+api_response = api_instance.get_columnar_features(features_request)
+pprint(api_response)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
```

