# Comparing `tmp/basedosdados-2.0.0b2.tar.gz` & `tmp/basedosdados-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basedosdados-2.0.0b2.tar", max compression
+gzip compressed data, was "basedosdados-2.0.0b3.tar", max compression
```

## Comparing `basedosdados-2.0.0b2.tar` & `basedosdados-2.0.0b3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2514 2023-05-04 15:04:40.695846 basedosdados-2.0.0b2/README.md
--rw-r--r--   0        0        0      827 2023-05-12 22:53:21.043886 basedosdados-2.0.0b2/basedosdados/__init__.py
--rw-r--r--   0        0        0      156 2023-05-10 00:48:26.910378 basedosdados-2.0.0b2/basedosdados/__main__.py
--rw-r--r--   0        0        0     8865 2023-05-15 20:52:16.710589 basedosdados-2.0.0b2/basedosdados/backend/__init__.py
--rw-r--r--   0        0        0     6737 2023-05-12 22:20:15.182110 basedosdados-2.0.0b2/basedosdados/cli/cli.py
--rw-r--r--   0        0        0      277 2023-05-10 18:22:29.189209 basedosdados-2.0.0b2/basedosdados/configs/config.toml
--rw-r--r--   0        0        0      469 2022-02-13 03:48:24.650258 basedosdados-2.0.0b2/basedosdados/configs/templates/dataset/README.md
--rw-r--r--   0        0        0      856 2022-02-13 03:48:24.650328 basedosdados-2.0.0b2/basedosdados/configs/templates/dataset/dataset_description.txt
--rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.650411 basedosdados-2.0.0b2/basedosdados/configs/templates/table/publish.sql
--rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.504177 basedosdados-2.0.0b2/basedosdados/configs/templates/table/table_description.txt
--rw-r--r--   0        0        0      895 2023-05-10 00:48:26.956830 basedosdados-2.0.0b2/basedosdados/constants.py
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650584 basedosdados-2.0.0b2/basedosdados/download/__init__.py
--rw-r--r--   0        0        0     1641 2023-05-10 00:48:26.938508 basedosdados-2.0.0b2/basedosdados/download/base.py
--rw-r--r--   0        0        0    17788 2023-05-10 00:48:27.143327 basedosdados-2.0.0b2/basedosdados/download/download.py
--rw-r--r--   0        0        0    13689 2023-05-10 00:48:27.186769 basedosdados-2.0.0b2/basedosdados/download/metadata.py
--rw-r--r--   0        0        0     3903 2023-05-10 00:48:26.993068 basedosdados-2.0.0b2/basedosdados/exceptions.py
--rw-r--r--   0        0        0     6779 2023-05-04 15:04:40.696211 basedosdados-2.0.0b2/basedosdados/schemas/columns_schema.json
--rw-r--r--   0        0        0    65118 2023-05-04 15:04:40.696404 basedosdados-2.0.0b2/basedosdados/schemas/dataset_schema.json
--rw-r--r--   0        0        0    30753 2023-05-04 15:04:40.696511 basedosdados-2.0.0b2/basedosdados/schemas/table_schema.json
--rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650914 basedosdados-2.0.0b2/basedosdados/upload/__init__.py
--rw-r--r--   0        0        0    15586 2023-05-12 22:28:30.811753 basedosdados-2.0.0b2/basedosdados/upload/base.py
--rw-r--r--   0        0        0     4957 2023-05-10 01:30:14.254761 basedosdados-2.0.0b2/basedosdados/upload/connection.py
--rw-r--r--   0        0        0     9399 2023-05-15 18:47:56.098568 basedosdados-2.0.0b2/basedosdados/upload/dataset.py
--rw-r--r--   0        0        0     3228 2023-05-12 21:24:41.585549 basedosdados-2.0.0b2/basedosdados/upload/datatypes.py
--rw-r--r--   0        0        0    18917 2023-05-12 21:58:31.960998 basedosdados-2.0.0b2/basedosdados/upload/storage.py
--rw-r--r--   0        0        0    30950 2023-05-15 20:52:19.557521 basedosdados-2.0.0b2/basedosdados/upload/table.py
--rw-r--r--   0        0        0     3434 2023-05-12 22:26:30.059112 basedosdados-2.0.0b2/basedosdados/upload/utils.py
--rw-r--r--   0        0        0     1453 2023-05-15 20:55:29.190003 basedosdados-2.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 basedosdados-2.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     2514 2023-05-04 15:04:40.695846 basedosdados-2.0.0b3/README.md
+-rw-r--r--   0        0        0      827 2023-05-12 22:53:21.043886 basedosdados-2.0.0b3/basedosdados/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-10 00:48:26.910378 basedosdados-2.0.0b3/basedosdados/__main__.py
+-rw-r--r--   0        0        0     9207 2023-05-16 00:09:29.179404 basedosdados-2.0.0b3/basedosdados/backend/__init__.py
+-rw-r--r--   0        0        0     6737 2023-05-12 22:20:15.182110 basedosdados-2.0.0b3/basedosdados/cli/cli.py
+-rw-r--r--   0        0        0      277 2023-05-10 18:22:29.189209 basedosdados-2.0.0b3/basedosdados/configs/config.toml
+-rw-r--r--   0        0        0      469 2022-02-13 03:48:24.650258 basedosdados-2.0.0b3/basedosdados/configs/templates/dataset/README.md
+-rw-r--r--   0        0        0      856 2022-02-13 03:48:24.650328 basedosdados-2.0.0b3/basedosdados/configs/templates/dataset/dataset_description.txt
+-rw-r--r--   0        0        0     1036 2022-02-13 03:48:24.650411 basedosdados-2.0.0b3/basedosdados/configs/templates/table/publish.sql
+-rw-r--r--   0        0        0     2511 2022-03-17 20:15:08.504177 basedosdados-2.0.0b3/basedosdados/configs/templates/table/table_description.txt
+-rw-r--r--   0        0        0      895 2023-05-10 00:48:26.956830 basedosdados-2.0.0b3/basedosdados/constants.py
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650584 basedosdados-2.0.0b3/basedosdados/download/__init__.py
+-rw-r--r--   0        0        0     1641 2023-05-10 00:48:26.938508 basedosdados-2.0.0b3/basedosdados/download/base.py
+-rw-r--r--   0        0        0    17788 2023-05-10 00:48:27.143327 basedosdados-2.0.0b3/basedosdados/download/download.py
+-rw-r--r--   0        0        0    13689 2023-05-10 00:48:27.186769 basedosdados-2.0.0b3/basedosdados/download/metadata.py
+-rw-r--r--   0        0        0     3903 2023-05-10 00:48:26.993068 basedosdados-2.0.0b3/basedosdados/exceptions.py
+-rw-r--r--   0        0        0     6779 2023-05-04 15:04:40.696211 basedosdados-2.0.0b3/basedosdados/schemas/columns_schema.json
+-rw-r--r--   0        0        0    65118 2023-05-04 15:04:40.696404 basedosdados-2.0.0b3/basedosdados/schemas/dataset_schema.json
+-rw-r--r--   0        0        0    30753 2023-05-04 15:04:40.696511 basedosdados-2.0.0b3/basedosdados/schemas/table_schema.json
+-rw-r--r--   0        0        0        0 2022-02-13 03:48:24.650914 basedosdados-2.0.0b3/basedosdados/upload/__init__.py
+-rw-r--r--   0        0        0    15586 2023-05-12 22:28:30.811753 basedosdados-2.0.0b3/basedosdados/upload/base.py
+-rw-r--r--   0        0        0     4957 2023-05-10 01:30:14.254761 basedosdados-2.0.0b3/basedosdados/upload/connection.py
+-rw-r--r--   0        0        0     9399 2023-05-15 18:47:56.098568 basedosdados-2.0.0b3/basedosdados/upload/dataset.py
+-rw-r--r--   0        0        0     3228 2023-05-12 21:24:41.585549 basedosdados-2.0.0b3/basedosdados/upload/datatypes.py
+-rw-r--r--   0        0        0    18917 2023-05-12 21:58:31.960998 basedosdados-2.0.0b3/basedosdados/upload/storage.py
+-rw-r--r--   0        0        0    30950 2023-05-15 20:52:19.557521 basedosdados-2.0.0b3/basedosdados/upload/table.py
+-rw-r--r--   0        0        0     3434 2023-05-12 22:26:30.059112 basedosdados-2.0.0b3/basedosdados/upload/utils.py
+-rw-r--r--   0        0        0     1453 2023-05-16 00:17:44.182373 basedosdados-2.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 basedosdados-2.0.0b3/PKG-INFO
```

### Comparing `basedosdados-2.0.0b2/README.md` & `basedosdados-2.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/__init__.py` & `basedosdados-2.0.0b3/basedosdados/__init__.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/backend/__init__.py` & `basedosdados-2.0.0b3/basedosdados/backend/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,21 @@
         Returns:
             Dict: GraphQL response.
         """
         if not client:
             client = self._get_client(
                 headers=headers, fetch_schema_from_transport=fetch_schema_from_transport
             )
-        return client.execute(gql(query), variable_values=variables)
+        try:
+            return client.execute(gql(query), variable_values=variables)
+        except Exception as e:
+            msg = f"The API URL in the config.toml file may be incorrect or the API might be temporarily unavailable!\
+                Error executing query: {e}."
+            logger.error(msg)
+            return None
 
     def _get_dataset_id_from_slug(self, dataset_slug):
         query = """
             query ($slug: String!){
                 allDataset(slug: $slug) {
                     edges {
                         node {
@@ -89,17 +95,17 @@
                         }
                     }
                 }
             }
         """
         variables = {"slug": dataset_slug}
         response = self._execute_query(query=query, variables=variables)
-        r = self._simplify_graphql_response(response)
-        if r["allDataset"] != []:
-            return r["allDataset"][0]["_id"]
+        r = {} if response is None else self._simplify_graphql_response(response)
+        if r.get("allDataset", []) != []:
+            return r.get("allDataset")[0]["_id"]
         msg = f"{dataset_slug} not found. Please create the metadata first in {self.graphql_url}"
         logger.info(msg)
         return None
 
     def _get_table_id_from_slug(self, dataset_slug, table_slug):
         query = """
             query ($dataset_Id: ID!, $table_slug: String!){
@@ -117,16 +123,16 @@
         if dataset_id:
             variables = {
                 "dataset_Id": dataset_id,
                 "table_slug": table_slug,
             }
 
             response = self._execute_query(query=query, variables=variables)
-            r = self._simplify_graphql_response(response)
-            if r["allTable"] != []:
+            r = {} if response is None else self._simplify_graphql_response(response)
+            if r.get("allTable", []) != []:
                 return r["allTable"][0]["_id"]
         msg = f"No table {table_slug} found in {dataset_slug}. Please create in {self.graphql_url}"
         logger.info(msg)
         return None
 
     def get_dataset_config(self, dataset_id: str) -> Dict[str, Any]:
         """
```

### Comparing `basedosdados-2.0.0b2/basedosdados/cli/cli.py` & `basedosdados-2.0.0b3/basedosdados/cli/cli.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/configs/templates/dataset/dataset_description.txt` & `basedosdados-2.0.0b3/basedosdados/configs/templates/dataset/dataset_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/configs/templates/table/publish.sql` & `basedosdados-2.0.0b3/basedosdados/configs/templates/table/publish.sql`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/configs/templates/table/table_description.txt` & `basedosdados-2.0.0b3/basedosdados/configs/templates/table/table_description.txt`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/constants.py` & `basedosdados-2.0.0b3/basedosdados/constants.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/download/base.py` & `basedosdados-2.0.0b3/basedosdados/download/base.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/download/download.py` & `basedosdados-2.0.0b3/basedosdados/download/download.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/download/metadata.py` & `basedosdados-2.0.0b3/basedosdados/download/metadata.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/exceptions.py` & `basedosdados-2.0.0b3/basedosdados/exceptions.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/schemas/columns_schema.json` & `basedosdados-2.0.0b3/basedosdados/schemas/columns_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/schemas/dataset_schema.json` & `basedosdados-2.0.0b3/basedosdados/schemas/dataset_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/schemas/table_schema.json` & `basedosdados-2.0.0b3/basedosdados/schemas/table_schema.json`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/upload/base.py` & `basedosdados-2.0.0b3/basedosdados/upload/base.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/upload/connection.py` & `basedosdados-2.0.0b3/basedosdados/upload/connection.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/upload/dataset.py` & `basedosdados-2.0.0b3/basedosdados/upload/dataset.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/upload/datatypes.py` & `basedosdados-2.0.0b3/basedosdados/upload/datatypes.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/upload/storage.py` & `basedosdados-2.0.0b3/basedosdados/upload/storage.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/upload/table.py` & `basedosdados-2.0.0b3/basedosdados/upload/table.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/basedosdados/upload/utils.py` & `basedosdados-2.0.0b3/basedosdados/upload/utils.py`

 * *Files identical despite different names*

### Comparing `basedosdados-2.0.0b2/pyproject.toml` & `basedosdados-2.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 license = "MIT"
 name = "basedosdados"
 packages = [
   {include = "basedosdados"},
 ]
 readme = "README.md"
 repository = "https://github.com/base-dos-dados/bases"
-version = "2.0.0-beta.2"
+version = "2.0.0-beta.3"
 
 [tool.poetry.scripts]
 basedosdados = 'basedosdados.cli.cli:cli'
 
 [tool.poetry.dependencies]
 google-api-python-client = "^2.86.0"
 google-cloud-bigquery = "^3.10.0"
@@ -28,16 +28,16 @@
 loguru = "^0.7.0"
 pandas = "^2.0.1"
 pandas-gbq = "^0.19.2"
 pandavro = "^1.7.2"
 pydata-google-auth = "^1.8.0"
 python = ">=3.8, <3.11"
 requests-toolbelt = "^1.0.0"
-tqdm = "^4.65.0"
 tomlkit = "^0.11.8"
+tqdm = "^4.65.0"
 
 [tool.black]
 # Use the more relaxed max line length permitted in PEP8.
 exclude = '''
 /(
     \.eggs
   | \.git
```

### Comparing `basedosdados-2.0.0b2/PKG-INFO` & `basedosdados-2.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basedosdados
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: Organizar e facilitar o acesso a dados brasileiros através de tabelas públicas no BigQuery.
 Home-page: https://github.com/base-dos-dados/bases
 License: MIT
 Author: Joao Carabetta
 Author-email: joao.carabetta@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

