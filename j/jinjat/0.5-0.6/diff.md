# Comparing `tmp/jinjat-0.5.tar.gz` & `tmp/jinjat-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjat-0.5.tar", max compression
+gzip compressed data, was "jinjat-0.6.tar", max compression
```

## Comparing `jinjat-0.5.tar` & `jinjat-0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-05-14 01:24:40.914393 jinjat-0.5/LICENSE
--rw-r--r--   0        0        0     1347 2023-05-14 01:24:40.914393 jinjat-0.5/README.md
--rw-r--r--   0        0        0     2783 2023-05-14 01:24:53.338441 jinjat-0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/__init__.py
--rw-r--r--   0        0        0       93 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/__main__.py
--rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/dbt/__init__.py
--rw-r--r--   0        0        0     2601 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/dbt/config.py
--rw-r--r--   0        0        0    23560 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/dbt/dbt_project.py
--rw-r--r--   0        0        0      878 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/exceptions.py
--rw-r--r--   0        0        0     4486 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/generator.py
--rw-r--r--   0        0        0     2641 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/log_controller.py
--rw-r--r--   0        0        0     5381 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/models.py
--rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/routes/__init__.py
--rw-r--r--   0        0        0     8917 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/routes/admin.py
--rw-r--r--   0        0        0     9399 2023-05-14 01:24:53.338441 jinjat-0.5/src/jinjat/core/routes/analysis.py
--rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/schema/__init__.py
--rw-r--r--   0        0        0      693 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/schema/validator.py
--rw-r--r--   0        0        0     6220 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/server.py
--rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/util/__init__.py
--rw-r--r--   0        0        0     8166 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/util/api.py
--rw-r--r--   0        0        0     1068 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/util/filesystem.py
--rw-r--r--   0        0        0     2068 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/util/jmespath.py
--rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/deploy/__init__.py
--rw-r--r--   0        0        0       32 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/deploy/cloud-run.py
--rw-r--r--   0        0        0      944 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/deploy/fal.py
--rw-r--r--   0        0        0      338 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/deploy/modal-client.py
--rw-r--r--   0        0        0    12288 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/jaffle_shop.duckdb
--rw-r--r--   0        0        0     6058 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/main.py
--rw-r--r--   0        0        0    10094 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/playground.py
--rw-r--r--   0        0        0      210 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/requirements.txt
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 jinjat-0.5/setup.py
--rw-r--r--   0        0        0     4168 1970-01-01 00:00:00.000000 jinjat-0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 23:48:05.972207 jinjat-0.6/LICENSE
+-rw-r--r--   0        0        0     1347 2023-05-16 23:48:05.972207 jinjat-0.6/README.md
+-rw-r--r--   0        0        0     2783 2023-05-16 23:48:21.396324 jinjat-0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/dbt/__init__.py
+-rw-r--r--   0        0        0     2601 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/dbt/config.py
+-rw-r--r--   0        0        0    23560 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/dbt/dbt_project.py
+-rw-r--r--   0        0        0      878 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/exceptions.py
+-rw-r--r--   0        0        0     4486 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/generator.py
+-rw-r--r--   0        0        0     2641 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/log_controller.py
+-rw-r--r--   0        0        0     5381 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/models.py
+-rw-r--r--   0        0        0        0 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/routes/__init__.py
+-rw-r--r--   0        0        0     8917 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/routes/admin.py
+-rw-r--r--   0        0        0     9452 2023-05-16 23:48:21.400323 jinjat-0.6/src/jinjat/core/routes/analysis.py
+-rw-r--r--   0        0        0        0 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/schema/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/schema/validator.py
+-rw-r--r--   0        0        0     6220 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/server.py
+-rw-r--r--   0        0        0        0 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/util/__init__.py
+-rw-r--r--   0        0        0     8166 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/util/api.py
+-rw-r--r--   0        0        0     1068 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/util/filesystem.py
+-rw-r--r--   0        0        0     2068 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/core/util/jmespath.py
+-rw-r--r--   0        0        0        0 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/deploy/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-16 23:48:05.972207 jinjat-0.6/src/jinjat/deploy/cloud-run.py
+-rw-r--r--   0        0        0      944 2023-05-16 23:48:05.976207 jinjat-0.6/src/jinjat/deploy/fal.py
+-rw-r--r--   0        0        0      338 2023-05-16 23:48:05.976207 jinjat-0.6/src/jinjat/deploy/modal-client.py
+-rw-r--r--   0        0        0    12288 2023-05-16 23:48:05.976207 jinjat-0.6/src/jinjat/jaffle_shop.duckdb
+-rw-r--r--   0        0        0     6058 2023-05-16 23:48:05.976207 jinjat-0.6/src/jinjat/main.py
+-rw-r--r--   0        0        0    10094 2023-05-16 23:48:05.976207 jinjat-0.6/src/jinjat/playground.py
+-rw-r--r--   0        0        0      210 2023-05-16 23:48:05.976207 jinjat-0.6/src/jinjat/requirements.txt
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 jinjat-0.6/setup.py
+-rw-r--r--   0        0        0     4168 1970-01-01 00:00:00.000000 jinjat-0.6/PKG-INFO
```

### Comparing `jinjat-0.5/LICENSE` & `jinjat-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/README.md` & `jinjat-0.6/README.md`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/pyproject.toml` & `jinjat-0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jinjat"
-version = "0.5"
+version = "0.6"
 description = "A low-code data application framework that uses dbt Core and OpenAPI"
 authors = ["buremba <emrekabakci@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `jinjat-0.5/src/jinjat/core/dbt/config.py` & `jinjat-0.6/src/jinjat/core/dbt/config.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/dbt/dbt_project.py` & `jinjat-0.6/src/jinjat/core/dbt/dbt_project.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/exceptions.py` & `jinjat-0.6/src/jinjat/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/generator.py` & `jinjat-0.6/src/jinjat/core/generator.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/log_controller.py` & `jinjat-0.6/src/jinjat/core/log_controller.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/models.py` & `jinjat-0.6/src/jinjat/core/models.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/routes/admin.py` & `jinjat-0.6/src/jinjat/core/routes/admin.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/routes/analysis.py` & `jinjat-0.6/src/jinjat/core/routes/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                   include_in_schema=False)
 
     # api.add_route("/elements", functools.partial(elements_html, CustomButton("Admin APIs", "/")),
     #               include_in_schema=False)
 
     async def custom_openapi(req: Request) -> JSONResponse:
         extract_path = req.query_params.get("jmespath")
-        servers = [{"url": str(req.url).strip('/openapi.json')}]
+        servers = [{"url": f"{req.scope.get('scheme')}://{req.scope.get('server')[0]}:{req.scope.get('server')[1]}"}]
 
         if api.openapi_schema:
             api.openapi_schema['servers'] = servers
             return JSONResponse(extract_jmespath(extract_path, api.openapi_schema, project))
 
         openapi_schema = get_openapi(title=project.project_name,
                                      version=project.config.version,
```

### Comparing `jinjat-0.5/src/jinjat/core/schema/validator.py` & `jinjat-0.6/src/jinjat/core/schema/validator.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/server.py` & `jinjat-0.6/src/jinjat/core/server.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/util/api.py` & `jinjat-0.6/src/jinjat/core/util/api.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/util/filesystem.py` & `jinjat-0.6/src/jinjat/core/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/core/util/jmespath.py` & `jinjat-0.6/src/jinjat/core/util/jmespath.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/deploy/fal.py` & `jinjat-0.6/src/jinjat/deploy/fal.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/main.py` & `jinjat-0.6/src/jinjat/main.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/src/jinjat/playground.py` & `jinjat-0.6/src/jinjat/playground.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.5/setup.py` & `jinjat-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 'feedparser>=6.0.10,<7.0.0']}
 
 entry_points = \
 {'console_scripts': ['jinjat = jinjat.main:cli']}
 
 setup_kwargs = {
     'name': 'jinjat',
-    'version': '0.5',
+    'version': '0.6',
     'description': 'A low-code data application framework that uses dbt Core and OpenAPI',
     'long_description': '# Jinjat\n\n## Develop data applications with dbt, SQL, and OpenAPI\n\n### Installation\n\n```commandline\npip install jinjat\n```\n\n### Create your first API\n\nCreate an [analysis]() in `analysis/my_first_api.sql`:\n```sql\n{%- set query = request().query %}\n\nselect \'{{query.example}}\' as col1\n```\n\nAnd create a YML file in `analysis/schema.yml`:\n\n```yml\nversion: 2\n\nanalyses:\n  - name: my_first_api\n    config:\n      jinjat:\n        method: get\n        openapi:\n          parameters:\n            - in: query\n              name: example\n              schema:\n                type: number\n```\n\nStart Jinjat as follows:\n\n```commandline\njinjat serve --project-dir [YOUR_DBT_PROJECT_DIRECTORY]\n```\n\nAnd then run the following CURL command to test the API:\n\n```commandline\ncurl -XGET \'http://127.0.0.1:8581?example=value\'\n```\n\nIt should return the following response:\n\n```json\n[\n  "col1": "3"\n]\n```\n\nJinjat uses OpenAPI to validate the requests and create an API documentation automatically for your API.\n\n## Integrations\n\npoetry install --extras "duckdb"\n\n### Playground\n\npoetry install --extras "playground"\n\n\n#### Installation\n\n```commandline\npip install jinjat[playground]\n```\n\nJinjat Playground is a Streamlit app that lets you develop APIs in your browser.\nOnce you write the template, you can save it to your dbt project as an analysis and expose the API.',
     'author': 'buremba',
     'author_email': 'emrekabakci@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jinjat-data/jinjat',
```

### Comparing `jinjat-0.5/PKG-INFO` & `jinjat-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjat
-Version: 0.5
+Version: 0.6
 Summary: A low-code data application framework that uses dbt Core and OpenAPI
 Home-page: https://github.com/jinjat-data/jinjat
 License: Apache 2.0
 Keywords: dbt,server,streamlit,git,refine,data-app,snowflake
 Author: buremba
 Author-email: emrekabakci@gmail.com
 Requires-Python: >=3.8.1,<4
```

