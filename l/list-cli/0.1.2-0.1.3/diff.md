# Comparing `tmp/list-cli-0.1.2.tar.gz` & `tmp/list-cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list-cli-0.1.2.tar", last modified: Mon May 15 18:51:20 2023, max compression
+gzip compressed data, was "list-cli-0.1.3.tar", last modified: Wed May 17 03:59:02 2023, max compression
```

## Comparing `list-cli-0.1.2.tar` & `list-cli-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:51:20.758345 list-cli-0.1.2/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.2/LICENSE
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-15 18:51:20.758444 list-cli-0.1.2/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.2/README.md
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:51:20.757376 list-cli-0.1.2/list_cli/
--rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.2/list_cli/__init__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)     1490 2023-05-15 18:28:42.000000 list-cli-0.1.2/list_cli/__main__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-15 18:50:54.000000 list-cli-0.1.2/list_cli/__version__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)    10642 2023-05-15 18:48:30.000000 list-cli-0.1.2/list_cli/processors.py
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:51:20.758191 list-cli-0.1.2/list_cli.egg-info/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)      288 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/entry_points.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-15 18:51:20.000000 list-cli-0.1.2/list_cli.egg-info/top_level.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-15 18:51:20.758663 list-cli-0.1.2/setup.cfg
--rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.2/setup.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-17 03:59:02.770222 list-cli-0.1.3/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.3/LICENSE
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-17 03:59:02.770298 list-cli-0.1.3/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.3/README.md
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-17 03:59:02.769414 list-cli-0.1.3/list_cli/
+-rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.3/list_cli/__init__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1659 2023-05-17 03:52:05.000000 list-cli-0.1.3/list_cli/__main__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-17 03:58:31.000000 list-cli-0.1.3/list_cli/__version__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)    12165 2023-05-17 03:54:01.000000 list-cli-0.1.3/list_cli/processors.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)      786 2023-05-17 03:52:47.000000 list-cli-0.1.3/list_cli/results.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-17 03:59:02.770083 list-cli-0.1.3/list_cli.egg-info/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)      308 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/top_level.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-17 03:59:02.770512 list-cli-0.1.3/setup.cfg
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.3/setup.py
```

### Comparing `list-cli-0.1.2/LICENSE` & `list-cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.2/PKG-INFO` & `list-cli-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.2/README.md` & `list-cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.2/list_cli/__main__.py` & `list-cli-0.1.3/list_cli/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from os import (
     environ,
     getcwd,
     getenv
 )
 from os.path import isfile, join as path_join
 from sys import argv, exit
+from typing import List
 
 from list_cli.processors import MultiProcessor, Processor
 
 
-def _env_list_value(key, default=''):
+def _env_list_value(key, default='') -> List[str]:
     return list(filter(None, getenv(key, default).split(',')))
 
 
-def _get_database_file_paths():
+def _get_database_file_paths() -> List[str]:
     database_file_paths = _env_list_value('DATABASE_FILE_PATHS')
     if database_file_paths:
         return database_file_paths
     database_file_path = getenv('DATABASE_FILE_PATH')
     if database_file_path:
         return [database_file_path]
     database_names = _env_list_value('DATABASE_NAMES')
@@ -34,23 +35,24 @@
                 '.list',
                 database_name
             )
         )
     return database_file_paths
 
 
-def _get_processor():
-    database_file_paths = _get_database_file_paths()
-    if not database_file_paths:
-        exit(1)
-    elif len(database_file_paths) > 1:
+def _get_processor(database_file_paths: List[str]) -> MultiProcessor | Processor:
+    if len(database_file_paths) > 1:
         return MultiProcessor(database_file_paths)
     return Processor(database_file_paths[0])
 
 
 def main():
-    if not _get_processor().process(*argv[1:]):
+    database_file_paths = _get_database_file_paths()
+    if not database_file_paths:
+        exit(1)
+    process_result = _get_processor(database_file_paths).process(*argv[1:])
+    if process_result.had_error:
         exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `list-cli-0.1.2/list_cli/processors.py` & `list-cli-0.1.3/list_cli/processors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,33 @@
+from abc import ABC, abstractmethod
 from getpass import getuser
 from os import linesep, makedirs
 from os.path import (
     dirname,
     isdir,
-    isfile,
+    isfile
 )
 from re import match
 from time import time
 from uuid import UUID, uuid1
 
+from list_cli.results import (
+    ErrorResult,
+    Result,
+    SuccessResult
+)
 
-class MultiProcessor():
-    def __init__(
-        self,
-        database_file_paths,
-        output_file_paths=True
-    ):
-        self._database_file_paths = database_file_paths
-        self._output_file_paths = output_file_paths
 
-    def process(self, *args):
-        had_error = False
-        for index, database_file_path in enumerate(self._database_file_paths):
-            processor = Processor(
-                database_file_path,
-                database_index=index,
-                output_file_path=self._output_file_paths
-            )
-            if not processor.process(*args):
-                had_error = True
-        return not had_error
+class BaseProcessor(ABC):
+    @abstractmethod
+    def process(self, *args) -> Result:
+        pass
 
 
-class Processor():
+class Processor(BaseProcessor):
     ADDED_BUCKET = 'a'
     ADD_OPERATIONS = {'a', 'add'}
     BUCKET_PATTERN = r'^(a|added|d|done|h|handed_off|m|moved|r|removed)$'
     DEFAULT_PARENT_ID = UUID('00000000-0000-0000-0000-000000000000')
     DONE_BUCKET = 'd'
     DONE_OPERATIONS = {'d', 'done'}
     EDIT_OPERATIONS = {'e', 'edit'}
@@ -50,60 +41,58 @@
     REMOVE_OPERATIONS = {'r', 'remove'}
     TOUCH_OPERATIONS = {'t', 'touch'}
     VALID_BUCKETS = {
         ADDED_BUCKET,
         DONE_BUCKET,
         HANDED_OFF_BUCKET,
         MOVED_BUCKET,
-        REMOVED_BUCKET,
+        REMOVED_BUCKET
     }
 
     def __init__(
         self,
         database_file_path,
-        database_index=0,
         output_file_path=False
     ):
         self._database_file_path = database_file_path
         self._ensure_database_exists()
-        self._database_index = database_index
         self._output_file_path = output_file_path
 
     @property
-    def _database(self):
+    def _database(self) -> dict:
         if not hasattr(self, '_database_'):
             self._database_ = self._get_database()
         return self._database_
 
     @property
-    def _timestamp(self):
+    def _timestamp(self) -> int:
         if not hasattr(self, '_timestamp_'):
             self._timestamp_ = self._get_timestamp()
         return self._timestamp_
 
     @property
-    def _user(self):
+    def _user(self) -> str:
         if not hasattr(self, '_user_'):
             self._user_ = self._get_user()
         return self._user_
 
-    def process(self, *args):
+    def process(self, *args) -> Result:
         if not args:
             return self._render(self.ADDED_BUCKET)
         elif match(self.BUCKET_PATTERN, args[0]):
             return self._render(args[0][0])
         elif not match(self.INDEX_PATTERN, args[0]):
             return self._add(message=' '.join(args))
         index = int(args[0]) - 1
         if (
             index < 0 or
             not args[1:] or
             not match(self.OPERATION_PATTERN, args[1])
         ):
-            return False
+            return ErrorResult()
         operation = args[1]
         if operation in self.ADD_OPERATIONS:
             return self._add(message=' '.join(args[1:]))
         elif operation in self.DONE_OPERATIONS:
             return self._done(index)
         elif operation in self.EDIT_OPERATIONS:
             return self._edit(index, ' '.join(args[2:]))
@@ -111,87 +100,88 @@
             return self._handoff(index)
         elif operation in self.MOVE_OPERATIONS:
             return self._move(index)
         elif operation in self.REMOVE_OPERATIONS:
             return self._remove(index)
         elif operation in self.TOUCH_OPERATIONS:
             return self._touch(index)
-        return False
+        return ErrorResult()
 
     def _add(
         self,
         parent_id=None,
         message=None
-    ):
+    ) -> Result:
         if not message:
-            return False
+            return ErrorResult()
         datum = {
             'id': uuid1(),
             'parent_id': parent_id or self.DEFAULT_PARENT_ID,
             'created_by_user': self._user,
             'updated_by_user': self._user,
             'created_timestamp': self._timestamp,
             'updated_timestamp': self._timestamp,
             'bucket': self.ADDED_BUCKET,
-            'message': message,
+            'message': message
         }
         self._database.append(datum)
-        return self._write_database()
+        return SuccessResult() if self._write_database() else ErrorResult()
 
-    def _done(self, index=None):
+    def _done(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
-            return False
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.DONE_BUCKET
-            return self._write_database()
-        return False
+            return SuccessResult() if self._write_database() else ErrorResult()
+        return ErrorResult()
 
     def _edit(
         self,
         index=None,
         message=None
-    ):
+    ) -> Result:
         if not message:
-            return False
+            return ErrorResult()
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
-            return False
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['message'] = message
-            return self._write_database()
-        return False
+            return SuccessResult() if self._write_database() else ErrorResult()
+        return ErrorResult()
 
-    def _ensure_database_exists(self):
+    def _ensure_database_exists(self) -> bool:
         database_file_path = self._database_file_path
         database_dirname = dirname(database_file_path)
         if database_dirname and not isdir(database_dirname):
             makedirs(database_dirname)
         if not isfile(database_file_path):
             open(database_file_path, 'w').close()
+        return True
 
-    def _get_bucket(self, bucket):
+    def _get_bucket(self, bucket) -> list:
         return sorted(
             (
                 datum
                 for datum in self._database
                 if datum['bucket'] == bucket
             ),
             key=lambda datum: datum['updated_timestamp']
         )
 
-    def _get_database(self):
+    def _get_database(self) -> dict:
         database = []
         with open(self._database_file_path) as database_file:
             for line in database_file:
                 line_parts = line.rstrip("\r\n").split("\t")
                 if not line_parts:
                     continue
                 id_ = line_parts[0]
@@ -223,96 +213,139 @@
                         'id': UUID(id_),
                         'parent_id': UUID(parent_id),
                         'created_by_user': created_by_user,
                         'updated_by_user': updated_by_user,
                         'created_timestamp': int(created_timestamp),
                         'updated_timestamp': int(updated_timestamp),
                         'bucket': bucket,
-                        'message': message,
+                        'message': message
                     }
                 )
         return database
 
-    def _get_timestamp(self):
+    def _get_timestamp(self) -> int:
         return int(time())
 
-    def _get_user(self):
+    def _get_user(self) -> str:
         return getuser()
 
-    def _handoff(self, index=None):
+    def _handoff(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
-            return False
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.HANDED_OFF_BUCKET
-            return self._write_database()
-        return False
+            return SuccessResult() if self._write_database() else ErrorResult()
+        return ErrorResult()
 
-    def _move(self, index=None):
+    def _move(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
-            return False
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.MOVED_BUCKET
-            return self._write_database()
-        return False
+            return SuccessResult() if self._write_database() else ErrorResult()
+        return ErrorResult()
 
-    def _remove(self, index=None):
+    def _remove(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
-            return False
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.REMOVED_BUCKET
-            return self._write_database()
-        return False
+            return SuccessResult() if self._write_database() else ErrorResult()
+        return ErrorResult()
 
-    def _render(self, bucket):
+    def _render(self, bucket) -> Result:
         bucket = self._get_bucket(bucket)
         if not bucket:
-            return bucket != self.ADDED_BUCKET
+            return Result(had_error=bucket != self.ADDED_BUCKET, had_output=False)
         if self._output_file_path:
-            print(f'{linesep if self._database_index else ""}{self._database_file_path}:{linesep}')
+            print(f'{self._database_file_path}:{linesep}')
         for datum_index, datum in enumerate(bucket):
             print('%3d. %s' % (datum_index + 1, datum['message']))
-        return True
+        return SuccessResult(had_output=True)
 
-    def _touch(self, index=None):
+    def _touch(self, index=None) -> Result:
         bucket = self._get_bucket(self.ADDED_BUCKET)
         if not bucket:
-            return False
+            return ErrorResult()
         for datum_index, datum in enumerate(bucket):
             if datum_index != index:
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
-            return self._write_database()
-        return False
+            return SuccessResult() if self._write_database() else ErrorResult()
+        return ErrorResult()
 
-    def _write_database(self):
+    def _write_database(self) -> bool:
         with open(self._database_file_path, 'w') as database_file:
             for datum in self._database:
                 database_file.write(
                     "%s\t%s\t%s\t%s\t%d\t%d\t%s\t%s%s" % (
                         datum['id'],
                         datum['parent_id'],
                         datum['created_by_user'],
                         datum['updated_by_user'],
                         datum['created_timestamp'],
                         datum['updated_timestamp'],
                         datum['bucket'],
                         datum['message'],
-                        linesep,
+                        linesep
                     )
                 )
         return True
+
+
+class MultiProcessor(BaseProcessor):
+    def __init__(
+        self,
+        database_file_paths,
+        output_file_paths=True
+    ):
+        self._database_file_paths = database_file_paths
+        self._output_file_paths = output_file_paths
+        self._had_error = False
+        self._had_output = False
+
+    def process(self, *args) -> Result:
+        for database_file_index, database_file_path in enumerate(self._database_file_paths):
+            process_result = self._process_one(
+                database_file_index,
+                database_file_path,
+                *args
+            )
+            if (
+                self._output_file_paths and
+                process_result.had_output and
+                database_file_index != len(self._database_file_paths) - 1
+            ):
+                print()
+        return Result(had_error=self._had_error, had_output=self._had_output)
+
+    def _get_processor(self, database_file_path) -> Processor:
+        return Processor(database_file_path, output_file_path=self._output_file_paths)
+
+    def _process_one(
+        self,
+        database_file_index,
+        database_file_path,
+        *args
+    ) -> Result:
+        process_result = self._get_processor(database_file_path).process(*args)
+        if process_result.had_error:
+            self._had_error = True
+        if process_result.had_output:
+            self._had_output = True
+        return process_result
```

### Comparing `list-cli-0.1.2/list_cli.egg-info/PKG-INFO` & `list-cli-0.1.3/list_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.2/setup.py` & `list-cli-0.1.3/setup.py`

 * *Files identical despite different names*

