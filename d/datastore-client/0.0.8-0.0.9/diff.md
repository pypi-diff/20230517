# Comparing `tmp/datastore_client-0.0.8.tar.gz` & `tmp/datastore_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastore_client-0.0.8.tar", last modified: Thu Dec  5 13:00:19 2019, max compression
+gzip compressed data, was "datastore_client-0.0.9.tar", max compression
```

## Comparing `datastore_client-0.0.8.tar` & `datastore_client-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2144 2019-12-03 13:33:50.872827 datastore_client-0.0.8/README.md
--rw-r--r--   0        0        0        0 2019-04-05 14:59:24.118645 datastore_client-0.0.8/datastore_client/__init__.py
--rw-r--r--   0        0        0     1900 2019-12-05 12:58:15.383959 datastore_client-0.0.8/datastore_client/client.py
--rw-r--r--   0        0        0     2175 2019-12-03 13:33:50.874685 datastore_client-0.0.8/datastore_client/mock_client.py
--rw-r--r--   0        0        0      387 2019-12-05 12:58:15.384676 datastore_client-0.0.8/datastore_client/utils.py
--rw-r--r--   0        0        0      496 2019-12-05 12:58:15.386469 datastore_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 datastore_client-0.0.8/setup.py
--rw-r--r--   0        0        0     2710 1970-01-01 00:00:00.000000 datastore_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2144 2022-01-11 09:36:22.382405 datastore_client-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2022-01-11 09:36:22.382592 datastore_client-0.0.9/datastore_client/__init__.py
+-rw-r--r--   0        0        0     1900 2022-01-11 09:36:22.382771 datastore_client-0.0.9/datastore_client/client.py
+-rw-r--r--   0        0        0     2175 2022-01-11 09:36:22.382976 datastore_client-0.0.9/datastore_client/mock_client.py
+-rw-r--r--   0        0        0      387 2022-01-11 09:36:22.383154 datastore_client-0.0.9/datastore_client/utils.py
+-rw-r--r--   0        0        0      519 2022-01-11 11:45:49.301499 datastore_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2962 2022-01-11 11:46:05.642415 datastore_client-0.0.9/setup.py
+-rw-r--r--   0        0        0     2897 2022-01-11 11:46:05.642737 datastore_client-0.0.9/PKG-INFO
```

### Comparing `datastore_client-0.0.8/README.md` & `datastore_client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `datastore_client-0.0.8/datastore_client/client.py` & `datastore_client-0.0.9/datastore_client/client.py`

 * *Files identical despite different names*

### Comparing `datastore_client-0.0.8/datastore_client/mock_client.py` & `datastore_client-0.0.9/datastore_client/mock_client.py`

 * *Files identical despite different names*

### Comparing `datastore_client-0.0.8/setup.py` & `datastore_client-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
-from distutils.core import setup
+from setuptools import setup
 
 packages = \
 ['datastore_client']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['google-cloud-datastore>=1.9.0,<2.0.0']
+['google-cloud-datastore>=1.9,<3.0', 'grpcio>=1.43.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'datastore-client',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A simple Google DataStore client',
     'long_description': "# Simple DataStore Client\n\nA simple Google DataStore client that exposes 3 functions on the `DatastoreClient` class.\n\n```python\nclass DatastoreClient:\n    def __init__(self, namespace: str=None, **kwargs) -> None:\n        self.client = Client(namespace=namespace, **kwargs)\n\n    def set_key(\n        self,\n        entity_name: str,\n        key_name: str,\n        **properties: Any,\n    ) -> None:\n        ...\n\n    def get_key(\n        self,\n        entity_name: str,\n        key_name: str,\n    ) -> Optional[Entity]:\n        ...\n\n    def query_entity(\n        self,\n        entity_name: str,\n        *query_filters: Tuple[str, str, Any],\n        projection: List[str]=None,\n        limit: Optional[int]=None,\n    ) -> Iterator:\n        ...\n```\n\n## Examples\n\n### Changing the `namespace`\nYou can set the `namespace` for the client by passing it in to the constructor\n```python\nfrom datastore_client.client import DatastoreClient\n\nclient = DatastoreClient(namespace='namespace_A')\n```\n\nThe following will change the namespace for all subsequent function calls.\n\n```python\nfrom datastore_client.client import DatastoreClient\n\nclient = DatastoreClient()\nclient.client.namespace = 'specific_namespace'\n```\n\n### `set_key`\n\n```python\nfrom datastore_client.client import DatastoreClient\n\nclient = DatastoreClient()\nclient.set_key(\n    entity_name=RECHARGE_NOTES_ENTITY, \n    key_name=note_key, \n    username=username, \n    reference=reference, \n    note=notes,\n)\n\n# This can also be used in batch mode\nwith client.batch_update():\n    client.set_key(...)\n    client.set_key(...)\n\n# Both key updates will be done when the with block exits\n```\n\n### `get_key`\n\n```python\nfrom datastore_client.client import DatastoreClient\n\nclient = DatastoreClient()\nclient.get_key(LOGIN_ENTITY, username)\n```\n\n### `query_entity`\n\n```python\nfrom datastore_client.client import DatastoreClient\n\nclient = DatastoreClient()\nproduct_list = list(client.query_entity(\n    PRODUCT_ENTITY,\n    ('network', '=', network_name),\n    ('product_type', '=', product_code),\n    ('bundle_size', '=', denomination),\n    projection=['id'],\n    limit=1,\n))\n\nprint(product_list[0]['id'])\n```\n",
     'author': 'Jethro Muller',
     'author_email': 'git@jethromuller.co.za',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://github.com/Flickswitch/datastore-client',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `datastore_client-0.0.8/PKG-INFO` & `datastore_client-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: datastore-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple Google DataStore client
 Home-page: https://github.com/Flickswitch/datastore-client
 Author: Jethro Muller
 Author-email: git@jethromuller.co.za
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Dist: google-cloud-datastore (>=1.9.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: google-cloud-datastore (>=1.9,<3.0)
+Requires-Dist: grpcio (>=1.43.0,<2.0.0)
 Project-URL: Repository, https://github.com/Flickswitch/datastore-client
 Description-Content-Type: text/markdown
 
 # Simple DataStore Client
 
 A simple Google DataStore client that exposes 3 functions on the `DatastoreClient` class.
```

