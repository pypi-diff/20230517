# Comparing `tmp/basedosdados-2.0.0b3.tar.gz` & `tmp/basedosdados-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basedosdados-2.0.0b3.tar", max compression
+gzip compressed data, was "basedosdados-2.0.0b4.tar", max compression
```

## Comparing `basedosdados-2.0.0b3.tar` & `basedosdados-2.0.0b4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2514 2023-05-04 15:04:40.695846 basedosdados-2.0.0b3/README.md
--rw-r--r--   0        0        0      827 2023-05-12 22:53:21.043886 basedosdados-2.0.0b3/basedosdados/__init__.py
--rw-r--r--   0        0        0      156 2023-05-10 00:48:26.910378 basedosdados-2.0.0b3/basedosdados/__main__.py
--rw-r--r--   0        0        0     9207 2023-05-16 00:09:29.179404 basedosdados-2.0.0b3/basedosdados/backend/__init__.py
--rw-r--r--   0        0        0     6737 2023-05-12 22:20:15.182110 basedosdados-2.0.0b3/basedosdados/cli/cli.py
--rw-r--r--   0        0        0      277 2023-05-10 18:22:29.189209 basedosdados-2.0.0b3/basedosdados/configs/config.toml
--rw-r--r--   0        0        0      469 2022-02-13 03:48:24.650258 basedosdados-2.0.0b3/basedosdados/configs/templates/dataset/README.md
--rw-r--r--   0        0        0      856 2022-02-13 03:48:24.650328 basedosdados-2.0.0b3/basedosdados/configs/templates/dataset/dataset_description.txt
--rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.650411 basedosdados-2.0.0b3/basedosdados/configs/templates/table/publish.sql
--rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.504177 basedosdados-2.0.0b3/basedosdados/configs/templates/table/table_description.txt
--rw-r--r--   0        0        0      895 2023-05-10 00:48:26.956830 basedosdados-2.0.0b3/basedosdados/constants.py
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650584 basedosdados-2.0.0b3/basedosdados/download/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-10 00:48:26.938508 basedosdados-2.0.0b3/basedosdados/download/base.py
--rw-r--r--   0        0        0    17788 2023-05-10 00:48:27.143327 basedosdados-2.0.0b3/basedosdados/download/download.py
--rw-r--r--   0        0        0    13689 2023-05-10 00:48:27.186769 basedosdados-2.0.0b3/basedosdados/download/metadata.py
--rw-r--r--   0        0        0     3903 2023-05-10 00:48:26.993068 basedosdados-2.0.0b3/basedosdados/exceptions.py
--rw-r--r--   0        0        0     6779 2023-05-04 15:04:40.696211 basedosdados-2.0.0b3/basedosdados/schemas/columns_schema.json
--rw-r--r--   0        0        0    65118 2023-05-04 15:04:40.696404 basedosdados-2.0.0b3/basedosdados/schemas/dataset_schema.json
--rw-r--r--   0        0        0    30753 2023-05-04 15:04:40.696511 basedosdados-2.0.0b3/basedosdados/schemas/table_schema.json
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650914 basedosdados-2.0.0b3/basedosdados/upload/__init__.py
--rw-r--r--   0        0        0    15586 2023-05-12 22:28:30.811753 basedosdados-2.0.0b3/basedosdados/upload/base.py
--rw-r--r--   0        0        0     4957 2023-05-10 01:30:14.254761 basedosdados-2.0.0b3/basedosdados/upload/connection.py
--rw-r--r--   0        0        0     9399 2023-05-15 18:47:56.098568 basedosdados-2.0.0b3/basedosdados/upload/dataset.py
--rw-r--r--   0        0        0     3228 2023-05-12 21:24:41.585549 basedosdados-2.0.0b3/basedosdados/upload/datatypes.py
--rw-r--r--   0        0        0    18917 2023-05-12 21:58:31.960998 basedosdados-2.0.0b3/basedosdados/upload/storage.py
--rw-r--r--   0        0        0    30950 2023-05-15 20:52:19.557521 basedosdados-2.0.0b3/basedosdados/upload/table.py
--rw-r--r--   0        0        0     3434 2023-05-12 22:26:30.059112 basedosdados-2.0.0b3/basedosdados/upload/utils.py
--rw-r--r--   0        0        0     1453 2023-05-16 00:17:44.182373 basedosdados-2.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 basedosdados-2.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0     2514 2023-05-17 15:25:36.766063 basedosdados-2.0.0b4/README.md
+-rw-r--r--   0        0        0      827 2023-05-17 15:25:36.766653 basedosdados-2.0.0b4/basedosdados/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-17 15:25:36.767118 basedosdados-2.0.0b4/basedosdados/__main__.py
+-rw-r--r--   0        0        0     9545 2023-05-17 16:26:49.793959 basedosdados-2.0.0b4/basedosdados/backend/__init__.py
+-rw-r--r--   0        0        0     6737 2023-05-17 15:25:36.767842 basedosdados-2.0.0b4/basedosdados/cli/cli.py
+-rw-r--r--   0        0        0      277 2023-05-17 15:25:36.768671 basedosdados-2.0.0b4/basedosdados/configs/config.toml
+-rw-r--r--   0        0        0      469 2022-02-13 03:48:24.650258 basedosdados-2.0.0b4/basedosdados/configs/templates/dataset/README.md
+-rw-r--r--   0        0        0      856 2022-02-13 03:48:24.650328 basedosdados-2.0.0b4/basedosdados/configs/templates/dataset/dataset_description.txt
+-rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.650411 basedosdados-2.0.0b4/basedosdados/configs/templates/table/publish.sql
+-rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.504177 basedosdados-2.0.0b4/basedosdados/configs/templates/table/table_description.txt
+-rw-r--r--   0        0        0      895 2023-05-17 15:25:36.768974 basedosdados-2.0.0b4/basedosdados/constants.py
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650584 basedosdados-2.0.0b4/basedosdados/download/__init__.py
+-rw-r--r--   0        0        0     1641 2023-05-17 15:25:36.769303 basedosdados-2.0.0b4/basedosdados/download/base.py
+-rw-r--r--   0        0        0    17788 2023-05-17 15:25:36.769667 basedosdados-2.0.0b4/basedosdados/download/download.py
+-rw-r--r--   0        0        0    13689 2023-05-17 15:25:36.770079 basedosdados-2.0.0b4/basedosdados/download/metadata.py
+-rw-r--r--   0        0        0     3903 2023-05-17 15:25:36.770604 basedosdados-2.0.0b4/basedosdados/exceptions.py
+-rw-r--r--   0        0        0     6779 2023-05-17 15:25:36.771132 basedosdados-2.0.0b4/basedosdados/schemas/columns_schema.json
+-rw-r--r--   0        0        0    65118 2023-05-17 15:25:36.771553 basedosdados-2.0.0b4/basedosdados/schemas/dataset_schema.json
+-rw-r--r--   0        0        0    30753 2023-05-17 15:25:36.771686 basedosdados-2.0.0b4/basedosdados/schemas/table_schema.json
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650914 basedosdados-2.0.0b4/basedosdados/upload/__init__.py
+-rw-r--r--   0        0        0    15586 2023-05-17 15:25:36.772065 basedosdados-2.0.0b4/basedosdados/upload/base.py
+-rw-r--r--   0        0        0     4957 2023-05-17 15:25:36.772254 basedosdados-2.0.0b4/basedosdados/upload/connection.py
+-rw-r--r--   0        0        0     9399 2023-05-17 15:25:36.772612 basedosdados-2.0.0b4/basedosdados/upload/dataset.py
+-rw-r--r--   0        0        0     3228 2023-05-17 15:25:36.773037 basedosdados-2.0.0b4/basedosdados/upload/datatypes.py
+-rw-r--r--   0        0        0    18917 2023-05-17 15:25:36.773769 basedosdados-2.0.0b4/basedosdados/upload/storage.py
+-rw-r--r--   0        0        0    30950 2023-05-17 16:21:47.259880 basedosdados-2.0.0b4/basedosdados/upload/table.py
+-rw-r--r--   0        0        0     3434 2023-05-17 15:25:36.774605 basedosdados-2.0.0b4/basedosdados/upload/utils.py
+-rw-r--r--   0        0        0     1453 2023-05-17 16:27:15.203997 basedosdados-2.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 basedosdados-2.0.0b4/PKG-INFO
```

### Comparing `basedosdados-2.0.0b3/README.md` & `basedosdados-2.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/__init__.py` & `basedosdados-2.0.0b4/basedosdados/__init__.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/backend/__init__.py` & `basedosdados-2.0.0b4/basedosdados/backend/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,65 +76,70 @@
         if not client:
             client = self._get_client(
                 headers=headers, fetch_schema_from_transport=fetch_schema_from_transport
             )
         try:
             return client.execute(gql(query), variable_values=variables)
         except Exception as e:
-            msg = f"The API URL in the config.toml file may be incorrect or the API might be temporarily unavailable!\
-                Error executing query: {e}."
+            msg = f"The API URL in the config.toml file may be incorrect or the API might be temporarily unavailable!\nError executing query: {e}."
             logger.error(msg)
             return None
 
-    def _get_dataset_id_from_slug(self, dataset_slug):
+    def _get_dataset_id_from_name(self, gcp_dataset_id):
         query = """
-            query ($slug: String!){
-                allDataset(slug: $slug) {
+            query ($gcp_dataset_id: String!){
+                allCloudtable(gcpDatasetId: $gcp_dataset_id) {
                     edges {
                         node {
-                            _id,
+                                table {
+                                    dataset {
+                                        _id
+                                    }
+                            }
                         }
                     }
                 }
             }
         """
-        variables = {"slug": dataset_slug}
+
+        variables = {"gcp_dataset_id": gcp_dataset_id}
         response = self._execute_query(query=query, variables=variables)
         r = {} if response is None else self._simplify_graphql_response(response)
-        if r.get("allDataset", []) != []:
-            return r.get("allDataset")[0]["_id"]
-        msg = f"{dataset_slug} not found. Please create the metadata first in {self.graphql_url}"
+        if r.get("allCloudtable", []) != []:
+            return r.get("allCloudtable")[0].get("table").get("dataset").get("_id")
+        msg = f"{gcp_dataset_id} not found. Please create the metadata first in {self.graphql_url}"
         logger.info(msg)
         return None
 
-    def _get_table_id_from_slug(self, dataset_slug, table_slug):
+    def _get_table_id_from_name(self, gcp_dataset_id, gcp_table_id):
         query = """
-            query ($dataset_Id: ID!, $table_slug: String!){
-                allTable (dataset_Id:$dataset_Id slug:$table_slug){
+            query ($gcp_dataset_id: String!, $gcp_table_id: String!){
+                allCloudtable(gcpDatasetId: $gcp_dataset_id, gcpTableId: $gcp_table_id) {
                     edges {
                         node {
-                            _id
+                                table {
+                                    _id
+                            }
                         }
                     }
                 }
             }
         """
-        dataset_id = self._get_dataset_id_from_slug(dataset_slug)
 
-        if dataset_id:
+        if gcp_dataset_id:
             variables = {
-                "dataset_Id": dataset_id,
-                "table_slug": table_slug,
+                "gcp_dataset_id": gcp_dataset_id,
+                "gcp_table_id": gcp_table_id,
             }
 
             response = self._execute_query(query=query, variables=variables)
             r = {} if response is None else self._simplify_graphql_response(response)
-            if r.get("allTable", []) != []:
-                return r["allTable"][0]["_id"]
-        msg = f"No table {table_slug} found in {dataset_slug}. Please create in {self.graphql_url}"
+            if r.get("allCloudtable", []) != []:
+                return r.get("allCloudtable")[0].get("table").get("_id")
+        msg = f"No table {gcp_table_id} found in {gcp_dataset_id}. Please create in {self.graphql_url}"
         logger.info(msg)
         return None
 
     def get_dataset_config(self, dataset_id: str) -> Dict[str, Any]:
         """
         Get dataset configuration.
 
@@ -173,15 +178,15 @@
                             }
                         }
                     }
                 }
             }
         
         """
-        dataset_id = self._get_dataset_id_from_slug(dataset_id)
+        dataset_id = self._get_dataset_id_from_name(dataset_id)
         if dataset_id:
             variables = {"dataset_id": dataset_id}
             response = self._execute_query(query=query, variables=variables)
             return self._simplify_graphql_response(response).get("allDataset")[0]
         else:
             return {}
 
@@ -226,16 +231,16 @@
                             }
                         }
                     }
                 }
                 }
             }    
         """
-        table_id = self._get_table_id_from_slug(
-            dataset_slug=dataset_id, table_slug=table_id
+        table_id = self._get_table_id_from_name(
+            gcp_dataset_id=dataset_id, gcp_table_id=table_id
         )
 
         if table_id:
             variables = {"table_id": table_id}
             response = self._execute_query(query=query, variables=variables)
             return self._simplify_graphql_response(response).get("allTable")[0]
         else:
```

### Comparing `basedosdados-2.0.0b3/basedosdados/cli/cli.py` & `basedosdados-2.0.0b4/basedosdados/cli/cli.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/configs/templates/dataset/dataset_description.txt` & `basedosdados-2.0.0b4/basedosdados/configs/templates/dataset/dataset_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/configs/templates/table/publish.sql` & `basedosdados-2.0.0b4/basedosdados/configs/templates/table/publish.sql`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/configs/templates/table/table_description.txt` & `basedosdados-2.0.0b4/basedosdados/configs/templates/table/table_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/constants.py` & `basedosdados-2.0.0b4/basedosdados/constants.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/download/base.py` & `basedosdados-2.0.0b4/basedosdados/download/base.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/download/download.py` & `basedosdados-2.0.0b4/basedosdados/download/download.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/download/metadata.py` & `basedosdados-2.0.0b4/basedosdados/download/metadata.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/exceptions.py` & `basedosdados-2.0.0b4/basedosdados/exceptions.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/schemas/columns_schema.json` & `basedosdados-2.0.0b4/basedosdados/schemas/columns_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/schemas/dataset_schema.json` & `basedosdados-2.0.0b4/basedosdados/schemas/dataset_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/schemas/table_schema.json` & `basedosdados-2.0.0b4/basedosdados/schemas/table_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/upload/base.py` & `basedosdados-2.0.0b4/basedosdados/upload/base.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/upload/connection.py` & `basedosdados-2.0.0b4/basedosdados/upload/connection.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/upload/dataset.py` & `basedosdados-2.0.0b4/basedosdados/upload/dataset.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/upload/datatypes.py` & `basedosdados-2.0.0b4/basedosdados/upload/datatypes.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/upload/storage.py` & `basedosdados-2.0.0b4/basedosdados/upload/storage.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/upload/table.py` & `basedosdados-2.0.0b4/basedosdados/upload/table.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/basedosdados/upload/utils.py` & `basedosdados-2.0.0b4/basedosdados/upload/utils.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b3/pyproject.toml` & `basedosdados-2.0.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 license = "MIT"
 name = "basedosdados"
 packages = [
   {include = "basedosdados"},
 ]
 readme = "README.md"
 repository = "https://github.com/base-dos-dados/bases"
-version = "2.0.0-beta.3"
+version = "2.0.0-beta.4"
 
 [tool.poetry.scripts]
 basedosdados = 'basedosdados.cli.cli:cli'
 
 [tool.poetry.dependencies]
 google-api-python-client = "^2.86.0"
 google-cloud-bigquery = "^3.10.0"
```

### Comparing `basedosdados-2.0.0b3/PKG-INFO` & `basedosdados-2.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basedosdados
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Organizar e facilitar o acesso a dados brasileiros através de tabelas públicas no BigQuery.
 Home-page: https://github.com/base-dos-dados/bases
 License: MIT
 Author: Joao Carabetta
 Author-email: joao.carabetta@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

