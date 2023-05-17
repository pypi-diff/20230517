# Comparing `tmp/levi-0.1.0.tar.gz` & `tmp/levi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "levi-0.1.0.tar", max compression
+gzip compressed data, was "levi-0.2.0.tar", max compression
```

## Comparing `levi-0.1.0.tar` & `levi-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-03-06 15:12:43.834601 levi-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      999 2023-03-06 15:12:43.834760 levi-0.1.0/README.md
--rw-r--r--   0        0        0     1987 2023-03-06 15:12:43.834990 levi-0.1.0/levi/__init__.py
--rw-r--r--   0        0        0      386 2023-03-06 15:12:43.835449 levi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 levi-0.1.0/setup.py
--rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 levi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-06 15:12:43.834601 levi-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1909 2023-05-17 11:56:45.930406 levi-0.2.0/README.md
+-rw-r--r--   0        0        0     3213 2023-05-17 11:56:45.930577 levi-0.2.0/levi/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-17 11:56:45.930946 levi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2379 1970-01-01 00:00:00.000000 levi-0.2.0/PKG-INFO
```

### Comparing `levi-0.1.0/LICENSE.md` & `levi-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `levi-0.1.0/levi/__init__.py` & `levi-0.2.0/levi/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,53 @@
 import re
+from deltalake import DeltaTable
 
 
-def delta_file_sizes(delta_table, boundaries=None):
+def skipped_stats(delta_table, filters):
+    df = delta_table.get_add_actions(flatten=True).to_pandas()
+    total_files = len(df)
+    total_bytes = df["size_bytes"].sum()
+    res = df.query(filters_to_sql(filters))
+    num_files_skipped = total_files - len(res)
+    num_bytes_skipped = total_bytes - res["size_bytes"].sum()
+    return {
+        "num_files": total_files,
+        "num_files_skipped": num_files_skipped,
+        "num_bytes_skipped": num_bytes_skipped
+    }
+
+
+def filters_to_sql(filters):
+    res = []
+    for filter in filters:
+        res.append(filter_to_sql(filter))
+    return " and ".join(res)
+
+
+def filter_to_sql(filter):
+    col, operator, val = filter
+    if operator == "=":
+        return f"(`min.{col}` <= {val} and `max.{col}` >= {val})"
+    elif operator == "<":
+        return f"(`min.{col}` < {val})"
+    elif operator == "<=":
+        return f"(`min.{col}` <= {val})"
+    elif operator == ">":
+        return f"(`max.{col}` > {val})"
+    elif operator == ">=":
+        return f"(`max.{col}` >= {val})"
+    else:
+        raise ValueError(f"{filter} cannot be parsed.")
+
+
+def latest_version(delta_table: DeltaTable):
+    return delta_table.version()
+
+
+def delta_file_sizes(delta_table: DeltaTable, boundaries=None):
     if boundaries is None:
         boundaries = ["<1mb", "1mb-500mb", "500mb-1gb", "1gb-2gb", ">2gb"]
     df = delta_table.get_add_actions(flatten=True).to_pandas()
     res = {}
     for boundary in boundaries:
         min, max = boundary_parser(boundary)
         count = len(df[df['size_bytes'].between(min, max)])
```

### Comparing `levi-0.1.0/PKG-INFO` & `levi-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: levi
-Version: 0.1.0
+Version: 0.2.0
 Summary: Delta Lake helper methods
 Author: Matthew Powers
 Author-email: matthewkevinpowers@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: deltalake (==0.7.0)
+Requires-Dist: deltalake[pandas] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Levi
 
 Delta Lake helper methods.  No Spark dependency.
 
 ## Installation
@@ -45,7 +45,45 @@
 
 You can also specify the boundaries when you invoke the function to get a custom result:
 
 ```python
 levi.delta_file_sizes(dt, ["<1mb", "1mb-200mb", "200mb-800mb", "800mb-2gb", ">2gb"])
 ```
 
+## Skipped stats
+
+Provides information on the number of files and number of bytes that are skipped for a given set of predicates.
+
+```python
+import levi
+
+dt = DeltaTable("some_folder/some_table")
+levi.skipped_stats(dt, filters=[('a_float', '=', 4.5)])
+
+# return value
+{
+    'num_files': 2,
+    'num_files_skipped': 1,
+    'num_bytes_skipped': 996
+}
+```
+
+This predicate will skip one file and 996 bytes of data.
+
+You can use `skipped_stats` to figure out the percentage of files that get skipped.  You can also use this information to see if you should Z ORDER your data or otherwise rearrange it to allow for better file skipping. 
+
+## Get Latest Delta Table Version
+
+The `latest_version` function gets the most current Delta Table version number and returns it.
+
+```python
+import levi
+from deltalake import DeltaTable
+
+dt = DeltaTable("some_folder/some_table")
+levi.latest_version(dt)
+
+# return value
+2
+```
+
+
```

