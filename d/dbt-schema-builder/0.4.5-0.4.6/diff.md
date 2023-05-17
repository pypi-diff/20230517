# Comparing `tmp/dbt-schema-builder-0.4.5.tar.gz` & `tmp/dbt-schema-builder-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-schema-builder-0.4.5.tar", last modified: Thu Aug 18 07:06:20 2022, max compression
+gzip compressed data, was "dbt-schema-builder-0.4.6.tar", last modified: Wed May 17 13:42:58 2023, max compression
```

## Comparing `dbt-schema-builder-0.4.5.tar` & `dbt-schema-builder-0.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:06:20.917455 dbt-schema-builder-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (121)    35139 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-08-18 07:06:20.917455 dbt-schema-builder-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4022 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:06:20.913455 dbt-schema-builder-0.4.5/dbt_schema_builder/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/app.py
--rw-r--r--   0 runner    (1001) docker     (121)    24201 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/queries.py
--rw-r--r--   0 runner    (1001) docker     (121)     9210 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/schema_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/snowflake_keywords.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:06:20.917455 dbt-schema-builder-0.4.5/dbt_schema_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/templates/model_sql_pii.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/dbt_schema_builder/templates/model_sql_safe.tpl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:06:20.917455 dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-08-18 07:06:20.000000 dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-08-18 07:06:20.000000 dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 07:06:20.000000 dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-18 07:06:20.000000 dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 07:06:20.000000 dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-18 07:06:20.000000 dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-18 07:06:20.000000 dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 07:06:20.917455 dbt-schema-builder-0.4.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-08-18 07:06:20.917455 dbt-schema-builder-0.4.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     5314 2022-08-18 07:06:14.000000 dbt-schema-builder-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4022 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/dbt_schema_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6649 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24273 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9343 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/relation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3904 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2798 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/schema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/snowflake_keywords.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/dbt_schema_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/templates/model_sql_pii.tpl
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/dbt_schema_builder/templates/model_sql_safe.tpl
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4696 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-17 13:42:58.000000 dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:42:58.729180 dbt-schema-builder-0.4.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-17 13:42:58.733180 dbt-schema-builder-0.4.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5314 2023-05-17 13:42:50.000000 dbt-schema-builder-0.4.6/setup.py
```

### Comparing `dbt-schema-builder-0.4.5/LICENSE.txt` & `dbt-schema-builder-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/PKG-INFO` & `dbt-schema-builder-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-builder
-Version: 0.4.5
+Version: 0.4.6
 Summary: Automate management of PII redacted schemas for dbt projects.
 Home-page: https://github.com/edx/dbt-schema-builder
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx dbt schema builder
 Platform: UNKNOWN
```

### Comparing `dbt-schema-builder-0.4.5/README.rst` & `dbt-schema-builder-0.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/app.py` & `dbt-schema-builder-0.4.6/dbt_schema_builder/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,26 +126,34 @@
                     source["tables"].append(
                         {
                             "name": relation.relation,
                             "description": DEFAULT_DESCRIPTION,
                         }
                     )
 
-    def update_trifecta_models(self, relation):
+    def update_trifecta_models(self, relation, no_pii=False):
         """
         Given a relation, add it to the 'trifecta'. These are the PII and safe views
         constructed from the raw data.
         """
-        for relation_name in [
-            relation.new_pii_relation_name,
-            relation.new_safe_relation_name,
-        ]:
-            self.add_model_to_new_schema(
-                relation_name, relation.meta_data
-            )
+        if no_pii:
+            for relation_name in [
+                relation.new_safe_relation_name,
+            ]:
+                self.add_model_to_new_schema(
+                    relation_name, relation.meta_data
+                )
+        else:
+            for relation_name in [
+                relation.new_pii_relation_name,
+                relation.new_safe_relation_name,
+            ]:
+                self.add_model_to_new_schema(
+                    relation_name, relation.meta_data
+                )
 
     def add_model_to_new_schema(self, new_relation_name, model_meta_data):
         """
         Add models and their columns to a schema that is currently being generated.
         """
         # Add our table to the "models" list in the new schema
         self.new_schema["models"].append({"name": new_relation_name})
```

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/builder.py` & `dbt-schema-builder-0.4.6/dbt_schema_builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -471,15 +471,15 @@
             curr_table_cols.append(r["COLUMN_NAME"])
 
         if curr_table_name:
             selected_relations[schema][curr_table_name] = curr_table_cols
 
         return selected_relations
 
-    def build_app(self, app_name, app_config):
+    def build_app(self, app_name, app_config, no_pii=False):
         """
         Build the requested application schema from the raw schemas.
         """
         # Create an App object to represent the current Application
         # that we will be building schemas for
         app_destination_database = app_name.split('.')[0]
         app_destination_schema = app_name.split('.')[1]
@@ -551,21 +551,20 @@
                 ) = relation.find_in_current_sources(
                     current_raw_sources,
                     current_downstream_sources,
                 )
 
                 app_object.add_source_to_new_schema(current_raw_source, relation, app_source_database, raw_schema)
                 app_object.add_table_to_downstream_sources(relation, current_safe_source, current_pii_source)
-                app_object.update_trifecta_models(relation)
+                app_object.update_trifecta_models(relation, no_pii=no_pii)
 
                 ##############################
                 # Write out dbt models which are responsible for generating the views
                 ##############################
-                relation.write_sql(raw_schema)
-
+                relation.write_sql(raw_schema, no_pii=no_pii)
         app_object.write_app_schema(design_file_path)
 
         # Create source definitions pertaining to app database views in the downstream dbt
         # project, i.e. reporting.
         self.write_sources_for_downstream_project(
             downstream_sources_file_path,
             yaml.safe_dump(app_object.new_downstream_sources, sort_keys=False),
@@ -602,18 +601,18 @@
                 raise Exception(
                     "fatal: {} is not a dbt project. Does not exist or is missing a "
                     "dbt_project.yml file.".format(project_path)
                 )
 
         return source_project_path, destination_project_path
 
-    def run(self):
+    def run(self, no_pii=False):
         """
         Wraps the SchemaBuilder steps
         """
         with log_manager.applicationbound():
             os.chdir(self.builder.source_project_path)
 
             for app_name, app_config in self.builder.app_schema_configs.items():
                 logger.info('\n')
                 logger.info('------- {} -------'.format(app_name))
-                self.builder.build_app(app_name, app_config)
+                self.builder.build_app(app_name, app_config, no_pii=no_pii)
```

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/queries.py` & `dbt-schema-builder-0.4.6/dbt_schema_builder/queries.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/relation.py` & `dbt-schema-builder-0.4.6/dbt_schema_builder/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,28 +220,32 @@
     def write_sql_file(sql_file_path, sql):
         """
         Writes out the given SQL file with the given string.
         """
         with open(sql_file_path, "w") as f:
             f.write(sql)
 
-    def write_sql(self, raw_schema):
+    def write_sql(self, raw_schema, no_pii=False):
         """
         Renders the SQL for this relation and writes out.
         """
         relation_dict = self.prep_meta_data()
 
         if self.is_unmanaged:
             logger.info(
                 "{}.{} is an unmanaged table, skipping SQL generation.".format(
                     self.app, self.relation
                 )
             )
         else:
-            for view_type in ("SAFE", "PII"):
+            if no_pii:
+                view_types = ["SAFE"]
+            else:
+                view_types = ["SAFE", "PII"]
+            for view_type in view_types:
                 if view_type == "SAFE":
                     sql_path = os.path.join(self.app_path, self.app)
                 else:
                     sql_path = os.path.join(
                         self.app_path, "{}_{}".format(self.app, view_type)
                     )
```

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/schema.py` & `dbt-schema-builder-0.4.6/dbt_schema_builder/schema.py`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/schema_builder.py` & `dbt-schema-builder-0.4.6/dbt_schema_builder/schema_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,20 @@
     )
     base_subparser.add_argument(
         "--target",
         default=None,
         type=str,
         help="Which target to load for the given profile",
     )
-
+    base_subparser.add_argument(
+        "--nopii",
+        required=False,
+        action='store_true',
+        help="Whether or not to supress PII models and sources",
+    )
     subs = p.add_subparsers(title="Available sub-commands", dest="command")
 
     build_sub = subs.add_parser(
         "build",
         parents=[base_subparser],
         help="Creates or updates schema.yml files from database catalog",
     )
@@ -81,16 +86,20 @@
 def handle(args):
     """
     Execute the given command. Currently only "build" exists, but it can be expanded here.
     """
     parsed = parse_args(args)
 
     if parsed.command == "build":
-        task = SchemaBuilderTask(parsed)
-        task.run()
+        if parsed.nopii:
+            task = SchemaBuilderTask(parsed)
+            task.run(no_pii=True)
+        else:
+            task = SchemaBuilderTask(parsed)
+            task.run()
 
 
 def main(args=None):
     """
     Do main things.
     """
     if args is None:
```

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/snowflake_keywords.yml` & `dbt-schema-builder-0.4.6/dbt_schema_builder/snowflake_keywords.yml`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/templates/model_sql_pii.tpl` & `dbt-schema-builder-0.4.6/dbt_schema_builder/templates/model_sql_pii.tpl`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder/templates/model_sql_safe.tpl` & `dbt-schema-builder-0.4.6/dbt_schema_builder/templates/model_sql_safe.tpl`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/PKG-INFO` & `dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-builder
-Version: 0.4.5
+Version: 0.4.6
 Summary: Automate management of PII redacted schemas for dbt projects.
 Home-page: https://github.com/edx/dbt-schema-builder
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx dbt schema builder
 Platform: UNKNOWN
```

### Comparing `dbt-schema-builder-0.4.5/dbt_schema_builder.egg-info/SOURCES.txt` & `dbt-schema-builder-0.4.6/dbt_schema_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/requirements/constraints.txt` & `dbt-schema-builder-0.4.6/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `dbt-schema-builder-0.4.5/setup.py` & `dbt-schema-builder-0.4.6/setup.py`

 * *Files identical despite different names*

