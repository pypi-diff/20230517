# Comparing `tmp/azurify-0.6.tar.gz` & `tmp/azurify-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurify-0.6.tar", last modified: Tue May 16 11:04:55 2023, max compression
+gzip compressed data, was "azurify-0.7.tar", last modified: Wed May 17 18:02:05 2023, max compression
```

## Comparing `azurify-0.6.tar` & `azurify-0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-16 11:04:55.777759 azurify-0.6/
--rw-r--r--   0 deniz      (501) staff       (20)     1067 2023-05-15 16:05:12.000000 azurify-0.6/LICENSE
--rw-r--r--   0 deniz      (501) staff       (20)     3026 2023-05-16 11:04:55.777077 azurify-0.6/PKG-INFO
-drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-16 11:04:55.764272 azurify-0.6/azurify/
--rw-r--r--   0 deniz      (501) staff       (20)      108 2023-05-15 16:05:12.000000 azurify-0.6/azurify/__init__.py
--rw-r--r--   0 deniz      (501) staff       (20)     1627 2023-05-15 16:05:12.000000 azurify-0.6/azurify/azconverter.py
--rw-r--r--   0 deniz      (501) staff       (20)     4511 2023-05-16 10:29:00.000000 azurify-0.6/azurify/azkeyvault.py
--rw-r--r--   0 deniz      (501) staff       (20)     3556 2023-05-15 16:05:12.000000 azurify-0.6/azurify/azsecrets.py
--rw-r--r--   0 deniz      (501) staff       (20)     3014 2023-05-15 16:05:12.000000 azurify-0.6/azurify/azstorage.py
--rw-r--r--   0 deniz      (501) staff       (20)      547 2023-05-15 16:05:12.000000 azurify-0.6/azurify/test_azconverter.py
--rw-r--r--   0 deniz      (501) staff       (20)     1393 2023-05-15 16:05:12.000000 azurify-0.6/azurify/test_azkeyvault.py
--rw-r--r--   0 deniz      (501) staff       (20)     3679 2023-05-15 16:05:12.000000 azurify-0.6/azurify/test_azsecrets.py
--rw-r--r--   0 deniz      (501) staff       (20)        0 2023-05-15 16:05:12.000000 azurify-0.6/azurify/test_azstorage.py
-drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-16 11:04:55.773603 azurify-0.6/azurify.egg-info/
--rw-r--r--   0 deniz      (501) staff       (20)     3026 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/PKG-INFO
--rw-r--r--   0 deniz      (501) staff       (20)      414 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/SOURCES.txt
--rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/dependency_links.txt
--rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-16 09:30:41.000000 azurify-0.6/azurify.egg-info/not-zip-safe
--rw-r--r--   0 deniz      (501) staff       (20)      133 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/requires.txt
--rw-r--r--   0 deniz      (501) staff       (20)        8 2023-05-16 11:04:55.000000 azurify-0.6/azurify.egg-info/top_level.txt
--rw-r--r--   0 deniz      (501) staff       (20)       38 2023-05-16 11:04:55.778591 azurify-0.6/setup.cfg
--rw-r--r--   0 deniz      (501) staff       (20)      997 2023-05-16 10:49:32.000000 azurify-0.6/setup.py
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-17 18:02:05.853052 azurify-0.7/
+-rw-r--r--   0 deniz      (501) staff       (20)     1067 2023-05-15 16:05:12.000000 azurify-0.7/LICENSE
+-rw-r--r--   0 deniz      (501) staff       (20)     3026 2023-05-17 18:02:05.852466 azurify-0.7/PKG-INFO
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-17 18:02:05.847750 azurify-0.7/azurify/
+-rw-r--r--   0 deniz      (501) staff       (20)      108 2023-05-15 16:05:12.000000 azurify-0.7/azurify/__init__.py
+-rw-r--r--   0 deniz      (501) staff       (20)     1627 2023-05-15 16:05:12.000000 azurify-0.7/azurify/azconverter.py
+-rw-r--r--   0 deniz      (501) staff       (20)     5348 2023-05-17 16:40:38.000000 azurify-0.7/azurify/azkeyvault.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3542 2023-05-17 11:43:21.000000 azurify-0.7/azurify/azsecrets.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3014 2023-05-15 16:05:12.000000 azurify-0.7/azurify/azstorage.py
+-rw-r--r--   0 deniz      (501) staff       (20)      547 2023-05-15 16:05:12.000000 azurify-0.7/azurify/test_azconverter.py
+-rw-r--r--   0 deniz      (501) staff       (20)     2113 2023-05-17 16:34:50.000000 azurify-0.7/azurify/test_azkeyvault.py
+-rw-r--r--   0 deniz      (501) staff       (20)     3507 2023-05-17 17:55:01.000000 azurify-0.7/azurify/test_azsecrets.py
+-rw-r--r--   0 deniz      (501) staff       (20)        0 2023-05-15 16:05:12.000000 azurify-0.7/azurify/test_azstorage.py
+drwxr-xr-x   0 deniz      (501) staff       (20)        0 2023-05-17 18:02:05.851732 azurify-0.7/azurify.egg-info/
+-rw-r--r--   0 deniz      (501) staff       (20)     3026 2023-05-17 18:02:05.000000 azurify-0.7/azurify.egg-info/PKG-INFO
+-rw-r--r--   0 deniz      (501) staff       (20)      414 2023-05-17 18:02:05.000000 azurify-0.7/azurify.egg-info/SOURCES.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-17 18:02:05.000000 azurify-0.7/azurify.egg-info/dependency_links.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        1 2023-05-16 09:30:41.000000 azurify-0.7/azurify.egg-info/not-zip-safe
+-rw-r--r--   0 deniz      (501) staff       (20)      133 2023-05-17 18:02:05.000000 azurify-0.7/azurify.egg-info/requires.txt
+-rw-r--r--   0 deniz      (501) staff       (20)        8 2023-05-17 18:02:05.000000 azurify-0.7/azurify.egg-info/top_level.txt
+-rw-r--r--   0 deniz      (501) staff       (20)       38 2023-05-17 18:02:05.853211 azurify-0.7/setup.cfg
+-rw-r--r--   0 deniz      (501) staff       (20)      997 2023-05-17 18:00:19.000000 azurify-0.7/setup.py
```

### Comparing `azurify-0.6/LICENSE` & `azurify-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `azurify-0.6/PKG-INFO` & `azurify-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurify
-Version: 0.6
+Version: 0.7
 Summary: Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.
 Home-page: https://github.com/zinyosrim/azurify
 Author: Zin Yosrim
 Author-email: zinyosrim@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `azurify-0.6/azurify/azconverter.py` & `azurify-0.7/azurify/azconverter.py`

 * *Files identical despite different names*

### Comparing `azurify-0.6/azurify/azsecrets.py` & `azurify-0.7/azurify/azsecrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,18 @@
         ...
 
     def get_secret(self, key):
         ...
 
 
 class AzureSecrets:
-    def __init__(self, vault_url: str, credential):
+    """Shopify secrets management on Azure. Create, get, delete secrets, load from file
+    """
+
+    def __init__(self, vault_url: str, credential=DefaultAzureCredential()):
         """Populate secrets dict with Keys/Values from the Azure KeyVault and create
         an instance attribute for each secret
 
         Args:
             vault_url (str): _description_
             credential (_type_): _description_
         """
@@ -51,15 +54,15 @@
             key = secret.name
             value = self._secret_client.get_secret(secret.name).value
             # create entry in secrets dict
             self._secrets[key] = value
             # create instance attribute
             setattr(self, key, value)
 
-    def load_jsonfile(self, path: str) -> None:
+    def load_json(self, path: str) -> None:
         """Load secrets from file
 
         Args:
             path (str): JSON path
         """
         with open(path) as json_data:
             config_secrets = json.load(json_data)
@@ -123,10 +126,8 @@
 
     print(secrets.SHOPDOMAIN)
 
 
 if __name__ == "__main__":
     main()
 
-    """
-    secrets = AzureSecrets(vault_url="https://kv-langerchen.vault.azure.net/", credential=DefaultAzureCredential(),)
-    """
+
```

### Comparing `azurify-0.6/azurify/azstorage.py` & `azurify-0.7/azurify/azstorage.py`

 * *Files identical despite different names*

### Comparing `azurify-0.6/azurify/test_azconverter.py` & `azurify-0.7/azurify/test_azconverter.py`

 * *Files identical despite different names*

### Comparing `azurify-0.6/azurify/test_azsecrets.py` & `azurify-0.7/azurify/test_azsecrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,31 @@
 from azsecrets import AzureSecrets
 
 
 class TestAzureSecrets(unittest.TestCase):
     def setUp(self):
         # Create randomized keyvault name and keyvault
         _random_str = "".join(random.choices(string.ascii_lowercase, k=10))
-        _keyvault_name = f"kv-test-{_random_str}"
-        Keyvault(tresor_name=_keyvault_name, keyvault_client=keyvault_client()).create()
+        self._keyvault_name = f"kv-test-{_random_str}"
+        Keyvault(kv_name=self._keyvault_name).create()
 
         # create secrets management object
         self.azsecrets = AzureSecrets(
-            vault_url=f"https://{_keyvault_name}.vault.azure.net/",
+            vault_url=f"https://{self._keyvault_name}.vault.azure.net/",
             credential=DefaultAzureCredential(),
         )
 
         # test data
         self.test_data = {
             "SHOPDOMAIN": "dcboard.myshopify.com",
             "APIVERSION": "2023-04",
             "APIACCESSTOKEN": "111",
             "APICLIENTSECRETKEY": "222",
             "AZSTORAGECONNSTR": "abc",
         }
-        self.azsecrets.load_json("test_data.json")
 
         # test-data with invalid keys
         self.test_data_incorrect_keys = {
             "SHOP_DOMAIN": "dcboard.myshopify.com",
             "API_VERSION": "2023-04",
             "APIACCESSTOKEN": "111",
             "APICLIENTSECRETKEY": "222",
@@ -48,22 +47,20 @@
         # create json files
         with open("test_data.json", "w") as outfile:
             outfile.write(json_object)
 
         with open("test_data_incorrect_keys.json", "w") as outfile:
             outfile.write(json_object_incorrect)
 
+        self.azsecrets.load_json("test_data.json")
+
     def test_load_jsonfile(self):
         # read secrets data from file
-        secrets = AzureSecrets(
-            vault_url=f"https://{self._keyvault_name}.vault.azure.net/",
-            credential=DefaultAzureCredential(),
-        )
-        secrets.load_json("test_data.json")
-        assert secrets.SHOPDOMAIN == "dcboard.myshopify.com"
+        #self.azsecrets.load_json("test_data.json")
+        assert self.azsecrets.SHOPDOMAIN == "dcboard.myshopify.com"
 
     def test_load_file_with_wrong_keys(self):
         secrets = AzureSecrets(
             vault_url=f"https://{self._keyvault_name}.vault.azure.net/",
             credential=DefaultAzureCredential(),
         )
         secrets.load_json("test_data_incorrect_keys.json")
```

### Comparing `azurify-0.6/azurify.egg-info/PKG-INFO` & `azurify-0.7/azurify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurify
-Version: 0.6
+Version: 0.7
 Summary: Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.
 Home-page: https://github.com/zinyosrim/azurify
 Author: Zin Yosrim
 Author-email: zinyosrim@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `azurify-0.6/setup.py` & `azurify-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="azurify",
-    version="0.6",
+    version="0.7",
     description="Access to Azure Storage/Secrets/Keyvault for Shopify Apps built with Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zinyosrim/azurify",
     author="Zin Yosrim",
     author_email="zinyosrim@gmail.com",
     license="MIT",
```

