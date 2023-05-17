# Comparing `tmp/redis_elastic-1.0.1.tar.gz` & `tmp/redis_elastic-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_elastic-1.0.1.tar", last modified: Mon May  8 23:11:50 2023, max compression
+gzip compressed data, was "redis_elastic-1.0.2.tar", last modified: Wed May 17 15:36:12 2023, max compression
```

## Comparing `redis_elastic-1.0.1.tar` & `redis_elastic-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 23:11:50.741869 redis_elastic-1.0.1/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 23:11:50.737869 redis_elastic-1.0.1/Develop/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-04 19:00:06.000000 redis_elastic-1.0.1/Develop/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2682 2023-04-27 18:32:13.000000 redis_elastic-1.0.1/Develop/extract.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1323 2023-05-04 22:53:19.000000 redis_elastic-1.0.1/Develop/tools.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3082 2023-05-08 23:11:50.741869 redis_elastic-1.0.1/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2659 2023-05-08 23:10:51.000000 redis_elastic-1.0.1/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 23:11:50.737869 redis_elastic-1.0.1/Warehouse/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-1.0.1/Warehouse/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5089 2023-05-08 22:42:24.000000 redis_elastic-1.0.1/Warehouse/redis_elastic.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-08 23:11:50.741869 redis_elastic-1.0.1/redis_elastic.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3082 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      307 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       71 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       18 2023-05-08 23:11:50.000000 redis_elastic-1.0.1/redis_elastic.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-08 23:11:50.741869 redis_elastic-1.0.1/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      876 2023-05-08 23:10:51.000000 redis_elastic-1.0.1/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-17 15:36:12.377872 redis_elastic-1.0.2/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-17 15:36:12.377872 redis_elastic-1.0.2/Develop/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-04 19:00:06.000000 redis_elastic-1.0.2/Develop/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2682 2023-04-27 18:32:13.000000 redis_elastic-1.0.2/Develop/extract.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1434 2023-05-09 19:29:17.000000 redis_elastic-1.0.2/Develop/tools.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3830 2023-05-17 15:36:12.377872 redis_elastic-1.0.2/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3407 2023-05-09 17:45:16.000000 redis_elastic-1.0.2/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-17 15:36:12.377872 redis_elastic-1.0.2/Warehouse/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-1.0.2/Warehouse/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4983 2023-05-09 17:59:21.000000 redis_elastic-1.0.2/Warehouse/redis_elastic.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-17 15:36:12.377872 redis_elastic-1.0.2/redis_elastic.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3830 2023-05-17 15:36:12.000000 redis_elastic-1.0.2/redis_elastic.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      307 2023-05-17 15:36:12.000000 redis_elastic-1.0.2/redis_elastic.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-17 15:36:12.000000 redis_elastic-1.0.2/redis_elastic.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       77 2023-05-17 15:36:12.000000 redis_elastic-1.0.2/redis_elastic.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       18 2023-05-17 15:36:12.000000 redis_elastic-1.0.2/redis_elastic.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-17 15:36:12.377872 redis_elastic-1.0.2/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      894 2023-05-09 18:46:26.000000 redis_elastic-1.0.2/setup.py
```

### Comparing `redis_elastic-1.0.1/Develop/extract.py` & `redis_elastic-1.0.2/Develop/extract.py`

 * *Files identical despite different names*

### Comparing `redis_elastic-1.0.1/Develop/tools.py` & `redis_elastic-1.0.2/Develop/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import ast
 
 
 class Qa:
     def __init__(self):
         pass
 
-    def query_dates(self, the_database, query):
+    def get_query_dates(self, the_database, query):
         parameters = the_database
         conn = psycopg2.connect(**parameters)
         cur = conn.cursor()
         cur.execute(query)
 
         # Get column names from cursor description
         column_names = [desc[0] for desc in cur.description]
@@ -24,15 +24,15 @@
 
         dates = pd.DataFrame(resultados, columns=column_names)
         print(dates)
         print("""･*:.｡. .｡.:*･゜ﾟ･*:.｡. .｡.:*･゜COLUMNS NAMES ﾟ･*:.｡. .｡.:*･゜ﾟ･*:.｡. .｡.:*･""")
         print(column_names)
         return dates
 
-    def redis_dates(self, ip, port, collection):
+    def get_redis_dates(self, ip, port, collection):
         # conexión a la base de datos de Redis
         r = redis.Redis(host=ip, port=port, db=0)
 
         # obtener los valores de las claves
         cached_query_odoo = r.get(collection).decode('utf8')
 
         try:
@@ -42,8 +42,12 @@
         except Exception:
             data = json.loads(cached_query_odoo)
             df = pd.DataFrame.from_dict(data)
 
         print(df)
         return df
 
+    def send_dates_to_redis(self, database, query, name_collection_redis):
+        pass
+
 
+action = Qa()
```

### Comparing `redis_elastic-1.0.1/PKG-INFO` & `redis_elastic-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-Metadata-Version: 2.1
-Name: redis_elastic
-Version: 1.0.1
-Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
-Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
-Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
-Author: Carlos Garcia Garcia
-Author-email: carlos.garcia1.gr1@icloud.com
-License: MIT
-Description-Content-Type: text/markdown
-
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 1.0.1 (Stable release)
+version 1.0.2 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -31,15 +20,15 @@
 
 [Docker Postgres | 🐘](https://hub.docker.com/_/postgres)
 
 [Docker Redis | 💾](https://hub.docker.com/_/redis)
 
 [Docker Elasticsearch | ⚡](https://hub.docker.com/_/elasticsearch)
 
-## Example by execution
+### Example by execution
 
 ```python
 from Warehouse.redis_elastic import Settings_redis_elastic
 
 postgres = {
     "host": "127.0.0.1",
     "port": "5432",
@@ -81,10 +70,46 @@
 
 Position in the method **fusion**
 
 ```python
 my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database)
 ```
 
+## Mode debug
+
+### Example of the tools
+
+```python
+from Develop.tools import action
 
+postgres = {
+    "host": "127.0.0.1",
+    "port": "5432",
+    "user": "etl",
+    "password": "123",
+    "database": "customer"
+}
+
+query = """Select rp.id,rp.name,rp.code from res_partner rp"""
 
+action.get_query_dates(postgres, query)
+action.get_redis_dates("localhost", 6379, "cached_query_dates_test:():dict_items([])")
+``` 
+
+### Actions
+
+**get_query_dates**
+
+With this function you get the results of your query in a Dataframe and print the columns
+
+```python
+action.get_query_dates(my_database, my_query)
+```
+
+**get_redis_dates**
+
+Get the data from the Redis collection in a Dataframe
+
+```python
+action.get_redis_dates(my_ip, port, name_of_colection_redis)
+```
```

### Comparing `redis_elastic-1.0.1/README.md` & `redis_elastic-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+Metadata-Version: 2.1
+Name: redis_elastic
+Version: 1.0.2
+Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
+Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
+Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
+Author: Carlos Garcia Garcia
+Author-email: carlos.garcia1.gr1@icloud.com
+License: MIT
+Description-Content-Type: text/markdown
+
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 1.0.1 (Stable release)
+version 1.0.2 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -20,15 +31,15 @@
 
 [Docker Postgres | 🐘](https://hub.docker.com/_/postgres)
 
 [Docker Redis | 💾](https://hub.docker.com/_/redis)
 
 [Docker Elasticsearch | ⚡](https://hub.docker.com/_/elasticsearch)
 
-## Example by execution
+### Example by execution
 
 ```python
 from Warehouse.redis_elastic import Settings_redis_elastic
 
 postgres = {
     "host": "127.0.0.1",
     "port": "5432",
@@ -70,10 +81,46 @@
 
 Position in the method **fusion**
 
 ```python
 my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database)
 ```
 
+## Mode debug
+
+### Example of the tools
+
+```python
+from Develop.tools import action
 
+postgres = {
+    "host": "127.0.0.1",
+    "port": "5432",
+    "user": "etl",
+    "password": "123",
+    "database": "customer"
+}
+
+query = """Select rp.id,rp.name,rp.code from res_partner rp"""
 
+action.get_query_dates(postgres, query)
+action.get_redis_dates("localhost", 6379, "cached_query_dates_test:():dict_items([])")
+``` 
+
+### Actions
+
+**get_query_dates**
+
+With this function you get the results of your query in a Dataframe and print the columns
+
+```python
+action.get_query_dates(my_database, my_query)
+```
+
+**get_redis_dates**
+
+Get the data from the Redis collection in a Dataframe
+
+```python
+action.get_redis_dates(my_ip, port, name_of_colection_redis)
+```
```

### Comparing `redis_elastic-1.0.1/Warehouse/redis_elastic.py` & `redis_elastic-1.0.2/Warehouse/redis_elastic.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         # Decorador para cachear resultados de la función en Redis
         def cache_function_results(function):
             @functools.wraps(function)
             def wrapper(*args, **kwargs):
                 # Generamos la clave del caché
                 cache_key = f"{function.__name__}{redis_name}:{args}:{kwargs.items()}"
-                print("Key in Redis {}".format(cache_key))
+                print("[Key in Redis 🔑]: {}".format(cache_key))
                 # Intentamos obtener el resultado del caché
                 cached_result = redis_client.get(cache_key)
 
                 # Si existe el resultado en caché, lo devolvemos
                 if cached_result is not None:
                     return pd.read_json(cached_result)
 
@@ -93,27 +93,24 @@
             # convertir los datos de bytes a una cadena de caracteres y luego a un diccionario
             # En caso de no realizar el ast, lo parse a un json
             try:
                 cached_query_odoo = ast.literal_eval(cached_query_redis.decode())
                 df = pd.DataFrame(cached_query_odoo)
 
             except Exception:
-                if cached_query_redis is None:
-                    df = pd.DataFrame()
-                else:
-                    data = json.loads(cached_query_redis)
-                    df = pd.DataFrame.from_dict(data)
+                data = json.loads(cached_query_redis)
+                df = pd.DataFrame.from_dict(data)
             return df
 
         def elastic_indexation():
             client = Elasticsearch(self.url_elasticsearch)
 
             # Obtiene la variable de columnas de la función query dates
             get_list_columns = query_dates().columns.tolist()
-            print(get_list_columns)
+            # print(get_list_columns)
             docs = []
             for i, row in redis_dates().iterrows():
                 doc = {
                     '_index': elasticsearch_name,
                     '_id': i,
                     '_source': {field: row[field] for field in get_list_columns}
                 }
@@ -132,8 +129,8 @@
         # Convertir los datos de Redis
         redis_dates()
 
         # Elastic search envio de Redis
         while True:
             elastic_indexation()
             print("Agregando datos de Elastic")
-            time.sleep(time_elastic)
+            time.sleep(time_elastic)
```

### Comparing `redis_elastic-1.0.1/redis_elastic.egg-info/PKG-INFO` & `redis_elastic-1.0.2/redis_elastic.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: redis-elastic
-Version: 1.0.1
+Version: 1.0.2
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 1.0.1 (Stable release)
+version 1.0.2 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -31,15 +31,15 @@
 
 [Docker Postgres | 🐘](https://hub.docker.com/_/postgres)
 
 [Docker Redis | 💾](https://hub.docker.com/_/redis)
 
 [Docker Elasticsearch | ⚡](https://hub.docker.com/_/elasticsearch)
 
-## Example by execution
+### Example by execution
 
 ```python
 from Warehouse.redis_elastic import Settings_redis_elastic
 
 postgres = {
     "host": "127.0.0.1",
     "port": "5432",
@@ -81,10 +81,46 @@
 
 Position in the method **fusion**
 
 ```python
 my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database)
 ```
 
+## Mode debug
 
+### Example of the tools
 
+```python
+from Develop.tools import action
+
+postgres = {
+    "host": "127.0.0.1",
+    "port": "5432",
+    "user": "etl",
+    "password": "123",
+    "database": "customer"
+}
+
+query = """Select rp.id,rp.name,rp.code from res_partner rp"""
+
+action.get_query_dates(postgres, query)
+action.get_redis_dates("localhost", 6379, "cached_query_dates_test:():dict_items([])")
+``` 
+
+### Actions
+
+**get_query_dates**
+
+With this function you get the results of your query in a Dataframe and print the columns
+
+```python
+action.get_query_dates(my_database, my_query)
+```
+
+**get_redis_dates**
+
+Get the data from the Redis collection in a Dataframe
+
+```python
+action.get_redis_dates(my_ip, port, name_of_colection_redis)
+```
```

### Comparing `redis_elastic-1.0.1/setup.py` & `redis_elastic-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 
 setup(
     name="redis_elastic",
-    version="1.0.1",
+    version="1.0.2",
     description="Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch",
     install_requires=[
         "setuptools",
-        "psycopg2",
+        "wheel",
         "psycopg2-binary",
         "redis",
         "elasticsearch==7.13.4",
-        "pandas"
+        "pandas",
+        "psycopg2",
     ],
     long_description=readme.read(),
     long_description_content_type='text/markdown',
     author="Carlos Garcia Garcia",
     author_email="carlos.garcia1.gr1@icloud.com",
     # REPOSITORIO GIT
     url="https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE",
```

