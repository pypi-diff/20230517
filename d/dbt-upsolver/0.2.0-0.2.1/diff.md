# Comparing `tmp/dbt-upsolver-0.2.0.tar.gz` & `tmp/dbt-upsolver-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-0.2.0.tar", last modified: Tue May  2 14:39:28 2023, max compression
+gzip compressed data, was "dbt-upsolver-0.2.1.tar", last modified: Wed May 17 10:47:56 2023, max compression
```

## Comparing `dbt-upsolver-0.2.0.tar` & `dbt-upsolver-0.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.141591 dbt-upsolver-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-02 14:39:28.141591 dbt-upsolver-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.129591 dbt-upsolver-0.2.0/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.129591 dbt-upsolver-0.2.0/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.133592 dbt-upsolver-0.2.0/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.133592 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/materialized_view_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/table_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.129591 dbt-upsolver-0.2.0/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.133592 dbt-upsolver-0.2.0/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:39:27.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:39:28.141591 dbt-upsolver-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.315206 dbt-upsolver-0.2.1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.315206 dbt-upsolver-0.2.1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.315206 dbt-upsolver-0.2.1/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/materialized_view_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/table_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.315206 dbt-upsolver-0.2.1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/setup.py
```

### Comparing `dbt-upsolver-0.2.0/LICENSE` & `dbt-upsolver-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/PKG-INFO` & `dbt-upsolver-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 0.2.0
+Version: 0.2.1
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-0.2.0/README.md` & `dbt-upsolver-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-0.2.1/dbt/adapters/upsolver/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/adapters/upsolver/impl.py` & `dbt-upsolver-0.2.1/dbt/adapters/upsolver/impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dbt.adapters.upsolver.options.connection_options import Connection_options
 from dbt.adapters.upsolver.options.transformation_options import Transformation_options
 from dbt.adapters.upsolver.options.table_options import Table_options
 from dbt.adapters.upsolver.options.materialized_view_options import Materialized_view_options
 import agate
 import datetime
 import re
+import dbt
 
 logger = AdapterLogger("Upsolver")
 LIST_RELATION_MACRO_NAME = "list_relation_without_caching"
 
 
 class UpsolverAdapter(adapter_cls):
     """
@@ -40,18 +41,20 @@
         pass
 
     def drop_schema(self, relation: UpsolverRelation) -> None:
         pass
 
     @available
     def get_connection_from_sql(self, sql):
-        connection_identifier = re.search('"(.*)"', sql).group().split('.')[2] \
-                                  .translate(str.maketrans({'\"':'', '\'':''}))
-
-        return connection_identifier
+        try:
+            connection_identifier = re.search('"(.*)"', sql).group().split('.')[2] \
+                                      .translate(str.maketrans({'\"':'', '\'':''}))
+            return connection_identifier
+        except Exception:
+            raise dbt.exceptions.ParsingError(f"Error while parsing connection name from sql:\n{sql}")
 
     @available
     def get_columns_names_with_types(self, list_dict):
         res = []
         for col in list_dict:
             if col.get('type'):
                 res.append(f"{col['field']} {col['type']}")
@@ -73,16 +76,19 @@
     @available
     def enrich_options(self, config_options, source, options_type):
         options = self.get_options(source, options_type)
         enriched_options = {}
         for option, value in config_options.items():
             find_value = options.get(option.lower(), None)
             if find_value:
-                if options[option.lower()]['type'] == 'list' and isinstance(value, str):
-                    value = f"('{value}')"
+                if options[option.lower()]['type'] == 'list':
+                    if not isinstance(value, str):
+                        value = tuple(i for i in value)
+                    else:
+                        value = f"('{value}')"
                 enriched_options[option] = find_value
                 enriched_options[option]['value'] = value
             else:
                 logger.warning(f"Options not found: {option}")
         return enriched_options
 
     @available
@@ -99,24 +105,14 @@
             options = Table_options
         elif options_type == 'materialized_view_options':
             options = Materialized_view_options
         else:
             options = Copy_options[source.lower()][options_type]
         return options
 
-    @available
-    def get_delete_placeholder(self, sql, delete_condition):
-        if delete_condition:
-            delete_placeholder= re.search('(nettotal < 0 [as|AS,\s]*\w*)', sql)[1] \
-              .lower().replace(" ", "") \
-              .replace(f"{delete_condition.lower().replace(' ', '')}as", "")
-            return delete_placeholder
-        else:
-            return False
-
     def list_relations_without_caching(
         self,
         schema_relation: UpsolverRelation,
         ) -> List[UpsolverRelation]:
         materializations = ["table", "job", "connection", "view"]
         results = agate.Table([],[])
         for type in materializations:
```

### Comparing `dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/connection_options.py` & `dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/connection_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/copy_options.py` & `dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/copy_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,42 +12,39 @@
         "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
         "run_parallelism": {"type": "integer", "editable": True, "optional": True},
         "content_type": {"type": "value", "editable": True, "optional": True},
         "compression": {"type": "value", "editable": False, "optional": True},
         "comment": {"type": "text", "editable": True, "optional": True}
     }
   },
-  "my_sql": {
+  "mysql": {
     "source_options": {
-        "table_include_list": {"type": "text", "editable": True, "optional": True},
-        "column_exclude_list": {"type": "text", "editable": True, "optional": True}
+        "table_include_list": {"type": "list", "editable": True, "optional": True},
+        "column_exclude_list": {"type": "list", "editable": True, "optional": True}
     },
     "job_options": {
-        "skip_snapshots": {"value": "text", "editable": True, "optional": True},
+        "skip_snapshots": {"type": "boolean", "editable": True, "optional": True},
         "end_at": {"type": "value", "editable": True, "optional": True},
         "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
         "comment": {"type": "text", "editable": True, "optional": True}
     }
   },
-  "postgre_sql": {
+  "postgres": {
     "source_options": {
-        "bucket": {"type": "text", "editable": False, "optional": False},
-        "prefix": {"type": "text", "editable": False, "optional": True}
+        "table_include_list": {"type": "list", "editable": False, "optional": False},
+        "column_exclude_list": {"type": "list", "editable": False, "optional": True}
     },
     "job_options": {
-        "table_include_list": {"type": "text", "editable": False, "optional": True},
+        "heartbeat_table": {"type": "text", "editable": False, "optional": True},
         "skip_snapshots": {"type": "boolean", "editable": False, "optional": True},
-        "column_exclude_list": {"type": "text", "editable": False, "optional": True},
         "publication_name": {"type": "text", "editable": False, "optional": False},
-        "file_pattern": {"type": "text", "editable": False, "optional": True},
-        "delete_files_after_load": {"type": "boolean", "editable": False, "optional": True},
         "end_at": {"type": "value", "editable": True, "optional": True},
         "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
-        "run_parallelism": {"type": "integer", "editable": True, "optional": True},
-        "comment": {"type": "text", "editable": True, "optional": True}
+        "comment": {"type": "text", "editable": True, "optional": True},
+        "parse_json_columns": {"type": "boolean", "editable": False, "optional": False}
     }
   },
   "s3": {
     "source_options": {
         "location": {"type": "text", "editable": False, "optional": False}
     },
     "job_options": {
@@ -56,9 +53,25 @@
         "end_at": {"type": "value", "editable": True, "optional": True},
         "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
         "run_parallelism": {"type": "integer", "editable": True, "optional": True},
         "content_type": {"type": "value", "editable": True, "optional": True},
         "compression": {"type": "value", "editable": False, "optional": True},
         "comment": {"type": "text", "editable": True, "optional": True}
     }
-  }
+  },
+    "kinesis": {
+      "source_options": {
+          "stream": {"type": "text", "editable": False, "optional": False}
+      },
+      "job_options": {
+          "reader_shards": {"type": "integer", "editable": True, "optional": True},
+          "store_raw_data": {"type": "boolean", "editable": False, "optional": True},
+          "start_from": {"type": "value", "editable": False, "optional": True},
+          "end_at": {"type": "value", "editable": False, "optional": True},
+          "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
+          "run_parallelism": {"type": "integer", "editable": False, "optional": True},
+          "content_type": {"type": "value", "editable": True, "optional": True},
+          "compression": {"type": "value", "editable": False, "optional": True},
+          "comment": {"type": "text", "editable": True, "optional": True}
+      }
+    }
 }
```

### Comparing `dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/table_options.py` & `dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/table_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Table_options = {
     "globally_unique_keys": {"type": "boolean", "editable": False, "optional": True},
     "storage_connection": {"type": "identifier", "editable": False, "optional": True},
     "storage_location": {"type": "text", "editable": False, "optional": True},
     "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
     "compression": {"type": "value", "editable": True, "optional": True},
-    "compaction_processes": {"type": "list", "editable": True, "optional": True},
+    "compaction_processes": {"type": "integer", "editable": True, "optional": True},
     "disable_compaction": {"type": "boolean", "editable": True, "optional": True},
     "retention_date_partition": {"type": "text", "editable": True, "optional": True},
     "table_data_retention": {"type": "text", "editable": True, "optional": True},
     "column_data_retention": {"type": "text", "editable": True, "optional": True},
     "comment": {"type": "text", "editable": True, "optional": True}
 }
```

### Comparing `dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/transformation_options.py` & `dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/transformation_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-0.2.1/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/adapters.sql` & `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files 20% similar despite different names*

```diff
@@ -14,19 +14,14 @@
                                                 schema=schema,
                                                 database=database,
                                                 type="connection") -%}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
-  {{ log("Options: " ~ connection_options ) }}
-  {{ log("Enriched options: " ~ enriched_options ) }}
-  {{ log("Enriched options: " ~ enriched_options ) }}
-
-
   {% if old_relation %}
     {% call statement('main') %}
       ALTER {{ connection_type }} CONNECTION {{target_relation.identifier}}
         {{ render_options(enriched_editable_options, 'alter') }}
     {%- endcall %}
   {% else %}
     {% call statement('main') -%}
```

### Comparing `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql` & `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/incremental.sql` & `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/incremental.sql`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     {%- endcall %}
   {% else %}
     {% call statement('main') -%}
       {% if incremental_strategy == 'merge' %}
         {{ get_create_merge_job_sql(job_identifier, table_relation, sync,
                                     options, primary_key, delete_condition) }}
       {% elif incremental_strategy == 'insert' %}
-        {{ get_create_incert_job_sql(job_identifier,
+        {{ get_create_insert_job_sql(job_identifier,
                                     table_relation, sync, options,
                                     map_columns_by_name) }}
 
       {% else  %}
         {{ get_create_copy_job_sql(job_identifier, sql,
                                    table_relation, sync, options, source) }}
```

### Comparing `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/ater_job.sql` & `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/ater_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/create_table.sql` & `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/create_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/dbt_upsolver.egg-info/PKG-INFO` & `dbt-upsolver-0.2.1/dbt_upsolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 0.2.0
+Version: 0.2.1
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-0.2.0/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-0.2.1/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.0/setup.py` & `dbt-upsolver-0.2.1/setup.py`

 * *Files identical despite different names*

