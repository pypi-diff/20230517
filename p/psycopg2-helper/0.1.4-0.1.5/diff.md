# Comparing `tmp/psycopg2-helper-0.1.4.tar.gz` & `tmp/psycopg2-helper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg2-helper-0.1.4.tar", max compression
+gzip compressed data, was "psycopg2-helper-0.1.5.tar", max compression
```

## Comparing `psycopg2-helper-0.1.4.tar` & `psycopg2-helper-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      107 2023-02-12 06:04:12.693092 psycopg2-helper-0.1.4/psycopg2_helper/__init__.py
--rw-r--r--   0        0        0       45 2022-11-17 00:42:17.429880 psycopg2-helper-0.1.4/psycopg2_helper/bp/__init__.py
--rw-r--r--   0        0        0      987 2022-11-17 01:11:38.793882 psycopg2-helper-0.1.4/psycopg2_helper/bp/postgres_helper.py
--rw-r--r--   0        0        0       51 2022-11-17 00:31:12.401877 psycopg2-helper-0.1.4/psycopg2_helper/dmo/__init__.py
--rw-r--r--   0        0        0     2486 2022-11-17 01:04:46.085879 psycopg2-helper-0.1.4/psycopg2_helper/dmo/postgres_connector.py
--rw-r--r--   0        0        0      116 2022-11-17 01:11:30.764880 psycopg2-helper-0.1.4/psycopg2_helper/svc/__init__.py
--rw-r--r--   0        0        0     2481 2023-02-12 04:33:12.589175 psycopg2-helper-0.1.4/psycopg2_helper/svc/perform_runtime_crud.py
--rw-r--r--   0        0        0     3604 2023-02-12 06:04:53.161570 psycopg2-helper-0.1.4/psycopg2_helper/svc/perform_table_operations.py
--rw-r--r--   0        0        0     1433 2023-02-12 06:04:03.317589 psycopg2-helper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       35 2022-11-17 00:16:48.136379 psycopg2-helper-0.1.4/README.md
--rw-r--r--   0        0        0      802 2023-02-12 06:05:17.676509 psycopg2-helper-0.1.4/setup.py
--rw-r--r--   0        0        0      959 2023-02-12 06:05:17.676509 psycopg2-helper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      107 2023-02-12 06:04:12.693092 psycopg2-helper-0.1.5/psycopg2_helper/__init__.py
+-rw-r--r--   0        0        0       45 2022-11-17 00:42:17.429880 psycopg2-helper-0.1.5/psycopg2_helper/bp/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-17 05:46:27.769374 psycopg2-helper-0.1.5/psycopg2_helper/bp/postgres_helper.py
+-rw-r--r--   0        0        0       51 2022-11-17 00:31:12.401877 psycopg2-helper-0.1.5/psycopg2_helper/dmo/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-17 05:40:12.890373 psycopg2-helper-0.1.5/psycopg2_helper/dmo/postgres_connector.py
+-rw-r--r--   0        0        0      116 2022-11-17 01:11:30.764880 psycopg2-helper-0.1.5/psycopg2_helper/svc/__init__.py
+-rw-r--r--   0        0        0     2851 2023-05-17 05:46:29.710373 psycopg2-helper-0.1.5/psycopg2_helper/svc/perform_runtime_crud.py
+-rw-r--r--   0        0        0     3931 2023-05-17 05:46:29.712372 psycopg2-helper-0.1.5/psycopg2_helper/svc/perform_table_operations.py
+-rw-r--r--   0        0        0     1433 2023-05-17 05:37:30.420873 psycopg2-helper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-05-17 05:46:28.499873 psycopg2-helper-0.1.5/README.md
+-rw-r--r--   0        0        0      804 2023-05-17 05:47:54.934874 psycopg2-helper-0.1.5/setup.py
+-rw-r--r--   0        0        0      960 2023-05-17 05:47:54.934874 psycopg2-helper-0.1.5/PKG-INFO
```

### Comparing `psycopg2-helper-0.1.4/psycopg2_helper/dmo/postgres_connector.py` & `psycopg2-helper-0.1.5/psycopg2_helper/dmo/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `psycopg2-helper-0.1.4/psycopg2_helper/svc/perform_runtime_crud.py` & `psycopg2-helper-0.1.5/psycopg2_helper/svc/perform_runtime_crud.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     def __init__(self,
                  conn: connection):
         """ Change Log
 
         Created:
             16-Nov-2022
             craigtrim@gmail.com
+        Updated:
+            16-May-2023
+            craigtrim@gmail.com
+            *   make exception handling more consistent
         """
         BaseObject.__init__(self, __name__)
         self.conn = conn
 
     def read(self,
              sql: str) -> list:
 
@@ -33,60 +37,69 @@
 
             with self.conn.cursor() as cursor:
                 cursor.execute(sql)
                 rows = cursor.fetchall()
                 for row in rows:
                     results.append(row)
 
-        except Exception as err:
-            self.logger.error(err)
+        except Exception as e:
+            self.logger.error(e)
             raise ValueError(sql)
 
         return results
 
     def delete(self,
                sql: str, *args) -> None:
+        """ Delete Data
+
+        Args:
+            sql (str): a SQL statement
+
+        Raises:
+            ValueError: on any exception
+        """
         try:
 
             with self.conn.cursor() as cursor:
                 cursor.execute(sql, list(args))
                 self.conn.commit()
 
-        except Exception as err:
-            self.logger.error(err)
+        except Exception as e:
+            self.logger.error(e)
             raise ValueError(sql)
 
     def insert(self,
                schema_name: str,
                table_name: str,
                column_names: List[str],
                column_values: List[str]) -> None:
         """ Insert Data
 
         Args:
             schema_name (str): the schema name
             table_name (str): the table name
-            args (*): any values to insert
+            column_names (List[str]): column names for insertion
+            column_values (List[str]): column values for insertion
 
         Raises:
-            ValueError: _description_
+            ValueError: on any exception
         """
 
         def tostr(values: List[str]) -> str:
             return f"({', '.join([x for x in values])})"
 
         def todqots(values: List[str]) -> str:
             return f"({', '.join(['%s' for x in values])})"
 
-        insert_query = f"INSERT INTO {schema_name}.{table_name} #names VALUES #values"
+        insert_query = f'INSERT INTO {schema_name}.{table_name} #names VALUES #values'
         insert_query = insert_query.replace('#names', tostr(column_names))
         insert_query = insert_query.replace('#values', todqots(column_values))
 
         try:
 
             with self.conn.cursor() as cursor:
                 cursor.execute(insert_query, column_values)
                 self.conn.commit()
 
-        except Exception as err:
-            self.logger.error(err)
+        except Exception as e:
+            self.logger.error(e)
             raise ValueError(insert_query)
```

### Comparing `psycopg2-helper-0.1.4/psycopg2_helper/svc/perform_table_operations.py` & `psycopg2-helper-0.1.5/psycopg2_helper/svc/perform_table_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     def __init__(self,
                  conn: connection):
         """ Change Log
 
         Created:
             16-Nov-2022
             craigtrim@gmail.com
+        Updated:
+            16-May-2023
+            craigtrim@gmail.com
+            *   make exception handling more consistent
         """
         BaseObject.__init__(self, __name__)
         self.conn = conn
 
     def create_table(self,
                      create_table_ddl: str):
         """ Create a Table
@@ -33,17 +37,20 @@
                 Sample Input:
                     "CREATE TABLE test (id serial PRIMARY KEY, num integer, data varchar);"
         Raises:
             ValueError: Create Table Failure
         """
         cur = self.conn.cursor()
         try:
+
             cur.execute(create_table_ddl)
-        except:
-            raise ValueError("Create Table Failure")
+
+        except Exception as e:
+            self.logger.error(e)
+            raise ValueError('Create Table Failure')
 
         self.conn.commit()
 
     def delete_table(self,
                      name: str,
                      schema: str) -> None:
         """ Delete (Drop) a Table
@@ -54,68 +61,71 @@
 
         Returns:
             str: status message
 
         Raises:
             ValueError: Delete Table Failure
         """
-        sql = f"DROP TABLE IF EXISTS {schema}.{name} CASCADE;"
+        sql = f'DROP TABLE IF EXISTS {schema}.{name} CASCADE;'
 
         try:
 
             with self.conn.cursor() as cursor:
                 cursor.execute(sql)
                 self.conn.commit()
 
         except Exception as e:
             self.conn.rollback()
+            self.logger.error(e)
             raise ValueError(sql)
 
     def create_schema(self,
                       name: str) -> None:
         """ Create a Schema
 
         Args:
             name (str): Schema Name
 
         Raises:
             ValueError: Create Schema Failure
         """
-        sql = f"CREATE SCHEMA IF NOT EXISTS {name}"
+        sql = f'CREATE SCHEMA IF NOT EXISTS {name}'
 
         try:
 
             with self.conn.cursor() as cursor:
                 cursor.execute(sql)
                 self.conn.commit()
 
         except Exception as e:
             self.conn.rollback()
+            self.logger.error(e)
             raise ValueError(sql)
 
     def delete_schema(self,
                       name: str) -> None:
         """ Delete a Schema
 
         Args:
             name (str): Schema Name
 
         Raises:
             ValueError: Delete Schema Failure
         """
-        sql = f"DROP SCHEMA IF EXISTS {name}"
+        sql = f'DROP SCHEMA IF EXISTS {name}'
 
         try:
 
             with self.conn.cursor() as cursor:
                 cursor.execute(sql)
                 self.conn.commit()
 
         except Exception as e:
             self.conn.rollback()
+            self.logger.error(e)
             raise ValueError(sql)
 
     def get_table_names(self,
                         schema: str) -> List[str]:
         """ Get Table Names
 
         Args:
@@ -131,12 +141,13 @@
             with self.conn.cursor() as cursor:
 
                 cursor.execute(sql)
                 rows = cursor.fetchall()
                 for tup in rows:
                     values += [tup[0]]
 
-        except Exception:
+        except Exception as e:
             self.conn.rollback()
+            self.logger.error(e)
             raise ValueError(sql)
 
         return sorted(set(values), key=len, reverse=True)
```

### Comparing `psycopg2-helper-0.1.4/pyproject.toml` & `psycopg2-helper-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Helper Functions for Postgres"
 license = "MIT"
 name = "psycopg2-helper"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 keywords = ["postgres", "db", "rdb", "rdbms", "helper", "utility", "psycopg2"]
 repository = "https://github.com/craigtrim/psycopg2-helper"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `psycopg2-helper-0.1.4/setup.py` & `psycopg2-helper-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'psycopg2']
 
 setup_kwargs = {
     'name': 'psycopg2-helper',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Helper Functions for Postgres',
-    'long_description': '# Postgres Helper (psycopg2-helper)',
+    'long_description': '# Postgres Helper (psycopg2-helper)\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/psycopg2-helper',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `psycopg2-helper-0.1.4/PKG-INFO` & `psycopg2-helper-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg2-helper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Helper Functions for Postgres
 Home-page: https://github.com/craigtrim/psycopg2-helper
 License: MIT
 Keywords: postgres,db,rdb,rdbms,helper,utility,psycopg2
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
@@ -19,7 +19,8 @@
 Requires-Dist: baseblock
 Requires-Dist: psycopg2
 Project-URL: Bug Tracker, https://github.com/craigtrim/psycopg2-helper/issues
 Project-URL: Repository, https://github.com/craigtrim/psycopg2-helper
 Description-Content-Type: text/markdown
 
 # Postgres Helper (psycopg2-helper)
+
```

