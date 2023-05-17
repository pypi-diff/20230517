# Comparing `tmp/duckingit-0.0.4.tar.gz` & `tmp/duckingit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckingit-0.0.4.tar", last modified: Thu May  4 20:01:57 2023, max compression
+gzip compressed data, was "duckingit-0.0.5.tar", last modified: Wed May 17 19:33:55 2023, max compression
```

## Comparing `duckingit-0.0.4.tar` & `duckingit-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-05-04 20:01:57.600434 duckingit-0.0.4/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3989 2023-05-04 20:01:57.599905 duckingit-0.0.4/PKG-INFO
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3384 2023-04-24 18:02:10.000000 duckingit-0.0.4/README.md
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-05-04 20:01:57.597292 duckingit-0.0.4/duckingit/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       84 2023-04-16 18:57:16.000000 duckingit-0.0.4/duckingit/__init__.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     9646 2023-05-01 17:56:53.000000 duckingit-0.0.4/duckingit/_config.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     6041 2023-05-04 19:55:25.000000 duckingit-0.0.4/duckingit/_controller.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     5304 2023-05-04 18:24:11.000000 duckingit-0.0.4/duckingit/_dataset.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      281 2023-04-20 17:31:23.000000 duckingit-0.0.4/duckingit/_exceptions.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      624 2023-04-16 10:14:45.000000 duckingit-0.0.4/duckingit/_extensions.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     2940 2023-05-01 18:26:48.000000 duckingit-0.0.4/duckingit/_parser.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     9323 2023-05-04 19:43:48.000000 duckingit-0.0.4/duckingit/_planner.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3476 2023-05-01 17:56:53.000000 duckingit-0.0.4/duckingit/_session.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     4476 2023-05-01 18:02:27.000000 duckingit-0.0.4/duckingit/_utils.py
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-05-04 20:01:57.599268 duckingit-0.0.4/duckingit.egg-info/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3989 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/PKG-INFO
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      413 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)        1 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       29 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/requires.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       10 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/top_level.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      824 2023-05-04 20:01:15.000000 duckingit-0.0.4/pyproject.toml
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       38 2023-05-04 20:01:57.600594 duckingit-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:33:55.557663 duckingit-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 19:33:33.000000 duckingit-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-17 19:33:55.557663 duckingit-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-17 19:33:33.000000 duckingit-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:33:55.557663 duckingit-0.0.5/duckingit/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-17 19:33:33.000000 duckingit-0.0.5/duckingit/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:33:55.557663 duckingit-0.0.5/duckingit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 19:33:55.000000 duckingit-0.0.5/duckingit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-17 19:33:33.000000 duckingit-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:33:55.557663 duckingit-0.0.5/setup.cfg
```

### Comparing `duckingit-0.0.4/PKG-INFO` & `duckingit-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![logo](logo.png)
 
 A framework to leverage the endless capabilities of serverless computing powered by DuckDB.
 
 Please note that the framework currently supports only AWS Lambda functions. To use the framework, you must first create a Lambda layer of DuckDB that can be used within a Lambda function. Additionally, you must create a Lambda Executor function that can execute the actual DuckDB SQL. Once you've completed these setup steps, you can leverage the power of serverless functions through the SDK written in Python to perform analytics on a Data Lake.
 
@@ -51,15 +52,15 @@
 
 ```python
 from duckingit import DuckSession, DuckConfig
 
 query = "SELECT * FROM READ_PARQUET(['s3://BUCKET_NAME/2023/*'])"
 
 # Following command will print possible configurations
-DuckConfig.show_configurations
+DuckConfig.show_configurations()
 
 # Configuration
 conf = DuckConfig() \
         .set("aws_lambda.FunctionName", "TestFunc") \
         .set("aws_lambda.MemorySize", 256) \
         .set("aws_lambda.WarmUp", True)
```

### Comparing `duckingit-0.0.4/README.md` & `duckingit-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 ```python
 from duckingit import DuckSession, DuckConfig
 
 query = "SELECT * FROM READ_PARQUET(['s3://BUCKET_NAME/2023/*'])"
 
 # Following command will print possible configurations
-DuckConfig.show_configurations
+DuckConfig.show_configurations()
 
 # Configuration
 conf = DuckConfig() \
         .set("aws_lambda.FunctionName", "TestFunc") \
         .set("aws_lambda.MemorySize", 256) \
         .set("aws_lambda.WarmUp", True)
```

### Comparing `duckingit-0.0.4/duckingit/_config.py` & `duckingit-0.0.5/duckingit/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
 TODO: Perhaps remove hardcoded limits and let boto3 raise the exception
 Trade-off: Fast vs slow response
 """
-import typing as t
 import copy
+import typing as t
 from dataclasses import dataclass
 
-from duckingit.integrations import Providers
 from duckingit._exceptions import ConfigurationError, WrongInvokationType
 from duckingit._utils import cast_mapping_to_string_with_newlines
-
+from duckingit.providers import Providers
 
 CACHE_PREFIX = ".cache/duckingit"
 
 
 class ServiceConfig:
     def update(self) -> None:
         """Update the state of the ConfigSingleton"""
-        pass
 
 
 @dataclass
 class LambdaConfig(ServiceConfig):
     FunctionName: str = "DuckExecutor"
     MemorySize: int = 128
     Timeout: int = 30
@@ -42,17 +40,15 @@
                     f"`Timeout` must be between {lower_limit} and {upper_limit} seconds"
                 )
 
         elif name == "MemorySize":
             lower_limit = 128
             upper_limit = 10240
             if not ((lower_limit <= value <= upper_limit) and isinstance(value, int)):
-                raise ValueError(
-                    f"`MemorySize` must be between {lower_limit} and {upper_limit} MB"
-                )
+                raise ValueError(f"`MemorySize` must be between {lower_limit} and {upper_limit} MB")
 
         elif name == "WarmUp":
             if not isinstance(value, bool):
                 raise ValueError("`WarmUp` must be a boolean")
 
         elif name == "FunctionName":
             if not isinstance(value, str):
@@ -85,25 +81,21 @@
 
     # Configs on Queue itself
     DelaySeconds: int = 0
     MaximumMessageSize: int = 2056
     MessageRetentionPeriod: int = 900
 
     def __repr__(self) -> str:
-        repr = cast_mapping_to_string_with_newlines(
-            service_name="aws_sqs", mapping=self.__dict__
-        )
+        repr = cast_mapping_to_string_with_newlines(service_name="aws_sqs", mapping=self.__dict__)
         return repr
 
     def __setattr__(self, name: str, value: t.Any) -> None:
         if name == "MaxNumberOfMessages":
             if not ((value <= 10) and isinstance(value, int)):
-                raise ValueError(
-                    "`MaxNumberOfMessages` must be between 1 and 10 seconds"
-                )
+                raise ValueError("`MaxNumberOfMessages` must be between 1 and 10 seconds")
 
         elif name == "VisibilityTimeout":
             if not ((value <= 60) and isinstance(value, int)):
                 raise ValueError("`VisibilityTimeout` must be between 0 and 60 seconds")
 
         elif name == "WaitTimeSeconds":
             if not ((value <= 60) and isinstance(value, int)):
@@ -145,17 +137,15 @@
     def update(self) -> None:
         config_dict = {
             k: str(v)
             for k, v in self.__dict__.items()
             if k in ("DelaySeconds", "MaximumMessageSize", "MessageRetentionPeriod")
         }
         for name in [self.__dict__["QueueSuccess"], self.__dict__["QueueFailure"]]:
-            Providers.AWS.klass.update_sqs_configurations(
-                name=name, configs=config_dict
-            )
+            Providers.AWS.klass.update_sqs_configurations(name=name, configs=config_dict)
 
 
 # @dataclass
 # class AWSConfig(ServiceConfig):
 #     s3_region: str
 #     s3_access_key_id: str
 #     s3_secret_access_key: str
@@ -165,31 +155,27 @@
 class SessionConfig(ServiceConfig):
     cache_expiration_time: int = 15
     max_invokations: int | str = "auto"
     provider: Providers = Providers.AWS
     verbose: bool = False
 
     def __repr__(self) -> str:
-        repr = cast_mapping_to_string_with_newlines(
-            service_name="session", mapping=self.__dict__
-        )
+        repr = cast_mapping_to_string_with_newlines(service_name="session", mapping=self.__dict__)
         return repr
 
     def __setattr__(self, name: str, value: t.Any) -> None:
         if name == "cache_expiration_time":
             if not isinstance(value, int):
                 raise ValueError("`cache expiration time` must be an integer")
 
         elif name == "max_invokations":
             if not (isinstance(value, int) or isinstance(value, str)):
                 if isinstance(value, str):
                     if value != "auto":
-                        raise WrongInvokationType(
-                            "`value` can only be 'auto' or an integer"
-                        )
+                        raise WrongInvokationType("`value` can only be 'auto' or an integer")
                 raise ValueError("`max invokations` must be an integer")
 
         elif name == "provider":
             if not (isinstance(value, str) or isinstance(value, Providers)):
                 raise ValueError("`provider` must be a string")
 
             if isinstance(value, str):
@@ -207,17 +193,15 @@
 
 @dataclass
 class DuckDBConfig(ServiceConfig):
     database: str = ":memory:"
     read_only: bool = False
 
     def __repr__(self) -> str:
-        repr = cast_mapping_to_string_with_newlines(
-            service_name="duckdb", mapping=self.__dict__
-        )
+        repr = cast_mapping_to_string_with_newlines(service_name="duckdb", mapping=self.__dict__)
         return repr
 
     def __setattr__(self, name: str, value: t.Any) -> None:
         if name == "database":
             if not isinstance(value, str):
                 raise ValueError("`database` must be a string")
 
@@ -258,15 +242,14 @@
 
         except AttributeError:
             raise ConfigurationError(f"Configuration `{name}` doesn't exists")
 
         return attr
 
     @classmethod
-    @property
     def show_configurations(cls):
         repr = "\n".join(
             [
                 str(cls.aws_lambda_config),
                 str(cls.aws_sqs_config),
                 str(cls.session_config),
                 str(cls.duckdb_config),
@@ -286,15 +269,15 @@
     def session(self):
         return self.session_config
 
     @property
     def duckdb(self):
         return self.duckdb_config
 
-    services_to_be_updated = {}
+    services_to_be_updated: dict[str, t.Any] = {}
 
     def set(self, name: str, value: t.Any):
         keys = name.split(".")
 
         service = self
         attr = keys.pop()
```

### Comparing `duckingit-0.0.4/duckingit/_controller.py` & `duckingit-0.0.5/duckingit/_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import datetime
 import typing as t
 
-from duckingit._planner import Plan, Task, Stage, Stages
-from duckingit.integrations import Providers
-from duckingit._utils import scan_source_for_files
 from duckingit._exceptions import FailedLambdaFunctions
+from duckingit._planner import Plan, Stage, Stages, Task
+from duckingit._utils import scan_source_for_files
+from duckingit.providers import Providers
 
 if t.TYPE_CHECKING:
     from duckingit._session import DuckSession
 
 
-ITERATIONS_TO_CHECK_FAILED = 5
-WAIT_TIME_SUCCESS_QUEUE_SECONDS = [4] * ITERATIONS_TO_CHECK_FAILED
-WAIT_TIME_FAILURE_QUEUE_SECONDS = 5
+# TODO: define heuristics for this
+ITERATIONS_TO_CHECK_FAILED = 3
+WAIT_TIME_SUCCESS_QUEUE_SECONDS = [3] * ITERATIONS_TO_CHECK_FAILED
+WAIT_TIME_FAILURE_QUEUE_SECONDS = 1
 
 
 class Controller:
     """The purpose of the controller is to control the invokations of
     serverless functions, e.g. Lambda functions.
 
     It invokes and collects the data, as well as concatenate it altogether before it's
@@ -26,17 +27,15 @@
             Can be based on number of rows or byte size
     """
 
     def __init__(self, session: "DuckSession") -> None:
         self.session = session
 
         self._set_provider()
-        self.cache_expiration_time = getattr(
-            session.conf, "session.cache_expiration_time"
-        )
+        self.cache_expiration_time = getattr(session.conf, "session.cache_expiration_time")
 
         self.success_queue = getattr(self.session.conf, "aws_sqs.QueueSuccess")
         self.failure_queue = getattr(self.session.conf, "aws_sqs.QueueFailure")
         self.verbose = getattr(self.session.conf, "session.verbose")
 
     def _set_provider(self):
         self.provider = Providers.AWS.klass
@@ -75,56 +74,50 @@
                 last_executed_minutes < self.cache_expiration_time
                 and step.subquery_hashed in cached_objects
             ):
                 execution_stage.tasks.remove(step)
 
     def execute_plan(self, execution_plan: Plan, prefix: str, default_prefix: str):
         """Executes the execution plan"""
-        dependencies: dict[str, list[str]] = {}
         completed = set()
         queue = set(execution_plan.leaves)
+        # TODO: Can this be moved in the loop, so old dependencies are overwritten?
+        dependencies: dict[str, list[str]] = {}
 
         while queue:
             stage = queue.pop()
 
             for deb in stage.dependents:
-                if deb.stage_type == Stages.CTE:
-                    continue
                 if deb.id not in completed:
                     queue.add(deb)
 
-            # CREATE TASKS HERE BASED ON CONTEXT!!
+            # for _id in list(dependencies):
+            #     if _id not in stage.dependencies:
+            #         _ = dependencies.pop(_id)
+
             stage.create_tasks(dependencies=dependencies)
-            # TODO: Handle multi dependencies
-            # context[stage.id] = list(
-            #     prefix + "/" + i + ".parquet" for i in stage.output
-            # )
             if self.verbose:
                 print(f"RUNNING STAGE: [{stage}]")
 
             if stage.id == execution_plan.root.id and prefix != "":
                 default_prefix = prefix
 
-            dependencies["output"] = [
-                f"{default_prefix}/{i}.parquet" for i in stage.output
-            ]
+            dependencies[stage.id] = [f"{default_prefix}/{i}.parquet" for i in stage.output]
             # self.evaluate_execution_stage(execution_stage=stage, prefix=default_prefix)
 
             execution_time = datetime.datetime.now()
             if len(stage.tasks) > 0:
                 request_ids = self.provider.invoke(
                     execution_tasks=stage.tasks, prefix=default_prefix
                 )
 
                 self.check_status_of_invokations(request_ids=request_ids)
 
             completed.add(stage.id)
-            self.update_cache_metadata(
-                execution_stage=stage, execution_time=execution_time
-            )
+            self.update_cache_metadata(execution_stage=stage, execution_time=execution_time)
 
     def check_status_of_invokations(self, request_ids: dict[str, Task]):
         cnt = 0
 
         total_tasks = len(request_ids)
         while len(request_ids) > 0:
             # Logic to speed up fast queries
@@ -138,22 +131,18 @@
                 for message in messages:
                     try:
                         request_ids.pop(message.request_id)
                     except KeyError:
                         continue
 
                 entries = list(message.create_entry_payload() for message in messages)
-                self.provider.delete_messages_from_queue(
-                    name=self.success_queue, entries=entries
-                )
+                self.provider.delete_messages_from_queue(name=self.success_queue, entries=entries)
 
             if self.verbose:
-                print(
-                    f"\tTASKS COMPLETED: {total_tasks - len(request_ids)}/{total_tasks}"
-                )
+                print(f"\tTASKS COMPLETED: {total_tasks - len(request_ids)}/{total_tasks}")
 
             cnt += 1
 
             if cnt % ITERATIONS_TO_CHECK_FAILED == 0:
                 messages = self.provider.poll_messages_from_queue(
                     name=self.failure_queue,
                     wait_time_seconds=WAIT_TIME_FAILURE_QUEUE_SECONDS,
```

### Comparing `duckingit-0.0.4/duckingit/_dataset.py` & `duckingit-0.0.5/duckingit/_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing as t
 from enum import Enum
 
 import duckdb
 
-from duckingit._planner import Plan
-from duckingit._exceptions import DatasetExistError
+from duckingit._config import CACHE_PREFIX
 from duckingit._controller import Controller
+from duckingit._exceptions import DatasetExistError
+from duckingit._planner import Plan
 from duckingit._utils import scan_source_for_files
-from duckingit._config import CACHE_PREFIX
 
 if t.TYPE_CHECKING:
     from duckingit._session import DuckSession
 
 
 class Modes(Enum):
     """A collection of modes to apply when writing
@@ -44,15 +44,15 @@
 
         _funcs = {
             self.APPEND: append,
             self.OVERWRITE: overwrite,
             self.WRITE: write,
         }
 
-        return _funcs[self]
+        return _funcs[self]  # type: ignore
 
 
 # class Formats(Enum):
 #     DELTA = "delta"
 #     ICEBERG = "iceberg"
 #     HUDI = "hudi"
 
@@ -120,17 +120,15 @@
         Example:
             >>> dataset = session.sql(query)
             >>> dataset.write.save_as_temp_table(table_name="test")
         """
         assert isinstance(table_name, str), "`table_name` must be of type string"
         self._dataset._execute_plan()
 
-        self._create_tmp_table(
-            table_name=table_name, objects=self._dataset.stored_objects
-        )
+        self._create_tmp_table(table_name=table_name, objects=self._dataset.stored_objects)
 
         self._session.metadata[table_name] = self._dataset.execution_plan.query.sql
 
 
 class Dataset:
     """
     The mapping between data objects in buckets and physical. If cache, then in memory
@@ -177,10 +175,8 @@
             prefix=prefix,
             default_prefix=self.default_prefix,
         )
 
     def show(self) -> duckdb.DuckDBPyRelation:
         self._execute_plan(prefix=self.default_prefix)
 
-        return self._session.conn.sql(
-            f"SELECT * FROM READ_PARQUET({self.stored_objects})"
-        )
+        return self._session.conn.sql(f"SELECT * FROM READ_PARQUET({self.stored_objects})")
```

### Comparing `duckingit-0.0.4/duckingit/_parser.py` & `duckingit-0.0.5/duckingit/_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import copy
 import re
 import typing as t
-import copy
 from dataclasses import dataclass
 
 import sqlglot
 import sqlglot.expressions as exp
 
 from duckingit._exceptions import InvalidFilesystem, ParserError
 from duckingit._utils import create_hash_string, scan_source_for_prefixes
@@ -27,14 +27,17 @@
 
         return cls(
             sql=query,
             hashed=create_hash_string(query),
             ast=expression,
         )
 
+    def replace(self, old: str, new: str) -> None:
+        self.sql = self.sql.replace(old, new)
+
     @property
     def list_of_prefixes(self) -> list[str]:
         if self._list_of_prefixes is None:
             self._list_of_prefixes = scan_source_for_prefixes(source=self.source)
         return self._list_of_prefixes
 
     @property
```

### Comparing `duckingit-0.0.4/duckingit/_planner.py` & `duckingit-0.0.5/duckingit/_planner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import typing as t
-from enum import Enum
 import copy
+import typing as t
 from dataclasses import dataclass
+from enum import Enum
 
+import sqlglot
 import sqlglot.expressions as exp
 
 from duckingit._parser import Query
-from duckingit._utils import split_list_in_chunks, create_hash_string
+from duckingit._utils import create_hash_string, split_list_in_chunks
 
 
 class Stages(Enum):
     AGGREGATE = "AGGREGATE"
-    CTE = "CTE"
     JOIN = "JOIN"
     SCAN = "SCAN"
     UNION = "UNION"
     SORT = "SORT"
 
     def __str__(self) -> str:
         return f"{self.value}"
@@ -23,40 +23,42 @@
 
 @dataclass
 class Task:
     subquery: str
     subquery_hashed: str
 
     @classmethod
-    def create(cls, query: Query, files: list[str]):
+    def create(cls, query: Query, files: list[str] | None = None):
         """Creates a task to execute on a serverless function
 
         Args:
             query, Query: A query parsed by the Query class
             files, list[str]: A list of files to scan
 
         Returns:
             Task<SUBQUERY | SUBQUERY_HASHED>
 
         """
         subquery = query.copy().sql
-        for table in query.from_:
-            table = table.expressions[0]
-            alias = table.alias
-            table = str(table).replace("ARRAY", "LIST_VALUE")  # Current sqlglot bug
-
-            read_json = "READ_JSON_AUTO"
-            read_csv = "READ_CSV_AUTO"
-
-            if table[: len(read_json)] == read_json:
-                subquery = subquery.replace(table, f"READ_JSON_AUTO({files}) {alias}")
-            elif table[: len(read_csv)] == read_csv:
-                subquery = subquery.replace(table, f"READ_CSV_AUTO({files}) {alias}")
-            else:
-                subquery = subquery.replace(table, f"READ_PARQUET({files}) {alias}")
+
+        if files:
+            for table in query.from_:
+                table = table.expressions[0]
+                alias = table.alias
+                table = str(table).replace("ARRAY", "LIST_VALUE")  # Current sqlglot bug
+
+                read_json = "READ_JSON_AUTO"
+                read_csv = "READ_CSV_AUTO"
+
+                if table[: len(read_json)] == read_json:
+                    subquery = subquery.replace(table, f"{read_json}({files}) {alias}")
+                elif table[: len(read_csv)] == read_csv:
+                    subquery = subquery.replace(table, f"{read_csv}({files}) {alias}")
+                else:
+                    subquery = subquery.replace(table, f"READ_PARQUET({files}) {alias}")
 
         return cls(subquery=subquery, subquery_hashed=create_hash_string(subquery))
 
     def __hash__(self) -> int:
         return hash(self.subquery)
 
     def __repr__(self) -> str:
@@ -64,181 +66,206 @@
 
     def copy(self):
         """Returns a deep copy of the object itself"""
         return copy.deepcopy(self)
 
 
 class Stage:
-    stage_type = ""
+    stage_type: Stages
 
     @classmethod
     def from_ast(
         cls,
         ast: exp.Expression,
-        previous_stage: None = None,
-        root_stage: None = None,
+        previous_stage: t.Optional["Stage"] = None,
+        root_stage: t.Optional["Stage"] = None,
         cte_stages: dict = {},
     ):
         ast = ast.copy()
 
         with_ = ast.args.get("with")
-        try:
-            ast.find(exp.With).pop()
-        except AttributeError:
-            pass
-
         if with_:
+            ast.find(exp.With).pop()  # type: ignore
+
             cte_stages = cte_stages.copy()
             for cte in with_.expressions:
-                stage = select_stage_type(cte)
-                stage.id = create_hash_string(cte.sql(), digits=6)
-                stage.name = cte.alias
-                stage.alias = cte.alias
-                stage.from_ = cte.this.sql()
-                stage.sql = cte.sql()
-
                 stage = Stage.from_ast(
                     cte.this,
-                    previous_stage=stage,
+                    previous_stage=previous_stage,
                     root_stage=root_stage,
                     cte_stages=cte_stages,
                 )
+                stage.alias = cte.alias
 
                 cte_stages[cte.alias] = stage
 
         from_ = ast.args.get("from")
         if isinstance(ast, exp.Select) and from_:
             if len(from_.expressions) > 1:
                 raise NotImplementedError("Multi FROM isn't supported")
             expression = from_.expressions[0]
 
             if isinstance(expression, exp.Subquery):
                 stage = select_stage_type(ast)
-                stage.id = create_hash_string(ast.sql(), digits=6)
-                stage.from_ = expression.sql()
+                # id must begin with a character
+                stage.id = create_hash_string(ast.sql(), digits=6, first_char="$")
                 stage.alias = expression.alias
-                stage.sql = ast.sql()
+                stage.ast = ast.copy()  # type: ignore
 
                 if previous_stage is not None:
                     previous_stage.add_dependency(stage)
                 if root_stage is None:
                     root_stage = stage
 
+                assert expression.this
+
                 stage = Stage.from_ast(
                     expression.this,
                     previous_stage=stage,
                     root_stage=root_stage,
                     cte_stages=cte_stages,
                 )
+                stage._replace_node(child=expression, id=stage.id, alias=expression.alias)
 
-            elif isinstance(expression, exp.Union):
+            if isinstance(expression, exp.Union):
                 raise NotImplementedError("Cannot handle Unions yet")
 
             else:
-                table_name = expression.sql()
+                table_name = str(expression.this)
 
                 stage = select_stage_type(ast)
-                stage.id = create_hash_string(ast.sql(), digits=6)
+                stage.id = create_hash_string(ast.sql(), digits=6, first_char="$")
                 stage.alias = expression.alias
-                stage.from_ = table_name
-                stage.sql = ast.sql()
+                stage.ast = ast.copy()  # type: ignore
 
                 if table_name in cte_stages:
                     cte = cte_stages[table_name]
+                    stage._replace_node(child=expression, id=cte.id, alias=expression.alias)
                     stage.add_dependency(cte)
 
-                if previous_stage is not None:
-                    previous_stage.add_dependency(stage)
-
-                if root_stage is None:
-                    root_stage = stage
         else:
-            raise NotImplementedError()
+            stage = Scan()
+
+        joins = ast.args.get("joins")
+        if joins:
+            stage.stage_type = Stages.JOIN
+
+            for join in joins:
+                join = join.this
+                alias = join.alias
+
+                if isinstance(join, exp.Subquery):
+                    subquery_stage = Stage.from_ast(
+                        join.this,  # type: ignore
+                        previous_stage=previous_stage,
+                        root_stage=root_stage,
+                        cte_stages=cte_stages,
+                    )
+                    stage._replace_node(child=join, id=subquery_stage.id, alias=alias)
+                    stage.add_dependency(subquery_stage)
+
+                else:
+                    if (table_name := join.this.sql()) in cte_stages:
+                        cte = cte_stages[table_name]
+                        stage._replace_node(child=join, id=cte.id, alias=alias)
+                        stage.add_dependency(cte)
+
+        if previous_stage is not None:
+            previous_stage.add_dependency(stage)
+
+        if root_stage is None:
+            root_stage = stage
 
         return root_stage
 
     def __init__(self):
-        self.id = str = ""
+        self.id: str = ""
         self.name: str = ""
         self.alias: str = ""  # Properbly to be deleted
-        self.sql: str = ""
-        self.from_: str = ""
+        self.ast: exp.Expression | None = None
+        self._sql: str = ""
 
-        self.dependents = []
-        self.dependencies = []
+        self.dependents = set()
+        self.dependencies = set()
 
         self.tasks: t.Set[Task] = set()
 
     def __repr__(self) -> str:
         return f"{self.stage_type} - {self.id}: {self.sql}"
 
     def __len__(self) -> int:
         return len(self.tasks)
 
+    def _replace_node(self, child: exp.Expression, id: str, alias: str = "") -> None:
+        if self.ast is None:
+            raise ValueError
+
+        for node, *_ in self.ast.walk():
+            if node == child:
+                node.replace(sqlglot.parse_one(f"{id} {alias}"))
+
     @property
-    def name_or_sql(self) -> None:
-        if self.name == "":
-            return self.sql
-        return self.name
+    def sql(self) -> str:
+        if self.ast is None:
+            return ""
+        return self.ast.sql()
+
+    def alias_or_id(self) -> str:
+        if self.alias == "":
+            return self.id
+        return self.alias
 
     @property
     def output(self) -> list[str]:
         return list(task.subquery_hashed for task in self.tasks)
 
     def create_tasks(self, dependencies: dict[str, list[str]] = {}) -> None:
         # TODO: Focus on Stage ID in dependencies
         from duckingit._config import DuckConfig
 
+        # Wide operations can only have 1 invokation
+        # Narrow operations like SCAN can have multiple invokations
+        invokations = DuckConfig().session.max_invokations if self.stage_type == Stages.SCAN else 1
+
         query = Query.parse(self.sql)
         if dependencies:
-            files = dependencies["output"]
+            for _id, output in dependencies.items():
+                query.replace(_id, f"(SELECT * FROM READ_PARQUET({output}))")
+
+            self.tasks.add(Task.create(query=query))
+
         else:
             files = query.list_of_prefixes
 
-        # Wide operations can only have 1 invokation
-        # Narrow operations like SCAN can have multiple invokations
-        invokations = (
-            DuckConfig().session.max_invokations
-            if self.stage_type == Stages.SCAN
-            else 1
-        )
-
-        if isinstance(invokations, str):
-            invokations = len(files)
-
-        # TODO: Heuristic to divide the workload between the invokations based on size
-        # of prefixes / number of files etc. Or based on some deeper analysis of the query?
-        chunks_of_files = split_list_in_chunks(files, number_of_invokations=invokations)
-
-        for chunk in chunks_of_files:
-            self.tasks.add(Task.create(query=query, files=chunk))
-
-    def add_dependency(self, dependency: "Stage"):
-        self.dependencies.append(dependency)
-        dependency.dependents.append(self)
+            if isinstance(invokations, str):
+                invokations = len(files)
+
+            # TODO: Heuristic to divide the workload between the invokations based on size
+            # of prefixes / number of files etc. Or based on some deeper analysis of the query?
+            chunks_of_files = split_list_in_chunks(files, number_of_invokations=invokations)
+
+            for chunk in chunks_of_files:
+                self.tasks.add(Task.create(query=query, files=chunk))
+
+    def add_dependency(self, dependency: "Stage") -> None:
+        self.dependencies.add(dependency)
+        dependency.dependents.add(self)
 
     def copy(self):
-        """Returns a deep copy of the object itself"""
+        """Returns a deep copy of itself"""
         return copy.deepcopy(self)
 
 
 class Scan(Stage):
     stage_type = Stages.SCAN
 
     def __init__(self):
         super().__init__()
 
 
-class CTE(Stage):
-    stage_type = Stages.CTE
-
-    def __init__(self):
-        super().__init__()
-
-
 class Aggregate(Stage):
     stage_type = Stages.AGGREGATE
 
     def __init__(self):
         super().__init__()
 
 
@@ -260,70 +287,68 @@
     stage_type = Stages.UNION
 
     def __init__(self):
         super().__init__()
 
 
 def select_stage_type(ast: exp.Expression):
-    if isinstance(ast, exp.CTE):
-        return CTE()
-
     group = ast.args.get("group")
-    agg = list(i for i in ast.expressions if isinstance(i, exp.Count))
+    agg = list(i for i in ast.expressions if isinstance(i, exp.AggFunc))
     if group or agg:
         return Aggregate()
 
     sort = ast.args.get("order")
     if sort:
         return Sort()
 
-    join = ast.args.get("join")
-    if join:
-        raise NotImplementedError("Joins are not implemented yet")
-
     return Scan()
 
 
 class Plan:
     """Class to create an execution plan across nodes
 
-    The execution plan consists of a execution steps based on queries. Basically, the
-    class scan the bucket based on the query, divides the workload on the number of
-    invokations. Afterwards, its the Controller's job to execute the plan.
+    A execution consists of stages, and each stage consists of tasks. A stage is an actual
+    operation, such as Scan, Sort, Join, where a task is the actual DuckDB SQL query to run on
+    a serverless function
 
     Attributes:
+        query, Query: The main query parsed as in the Query class
+        root, Stage: The root operation, ie. last operation, in the DAG
+        dag, dict[Stage, Set(Stage)]: A DAG that represents the execution plan in nodes
+        leaves, list[Stage]: The leaves of stages in the DAG
 
     Methods:
-        from_query: Creates an execution plan that divides the workload between
-            nodes
+        from_query: Creates an execution plan from a query parsed in the Query class
     """
 
-    def __init__(
-        self, query: Query, root: Stage, dag: dict[Stage, t.Set[Stage]]
-    ) -> None:
+    def __init__(self, query: Query, root: Stage, dag: dict[Stage, t.Set[Stage]]) -> None:
         self.query = query
         self.root = root
         self.dag = dag
 
         self._length: int | None = None
 
     def __len__(self) -> int:
         if self._length is None:
             self._length = len([node for node, _ in self.dag.items()])
         return self._length
 
     @property
     def leaves(self) -> list[Stage]:
-        return [node for node, deps in self.dag.items() if not deps]
+        leaves = []
+        for node in self.dag:
+            if not self.dag[node]:
+                leaves.append(node)
+        return leaves
 
     @classmethod
     def from_query(cls, query: Query):
         root = Stage.from_ast(ast=query.ast)
 
-        dag = {}
+        dag: dict[Stage, t.Set[Stage]] = {root: set()}
         nodes = {root}
         while nodes:
             node = nodes.pop()
 
             dag[node] = set()
             for dep in node.dependencies:
                 dag[node].add(dep)
```

### Comparing `duckingit-0.0.4/duckingit/_session.py` & `duckingit-0.0.5/duckingit/_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import duckdb
 
 from duckingit._config import DuckConfig
 from duckingit._dataset import Dataset
 from duckingit._parser import Query
 from duckingit._planner import Plan
-from duckingit.integrations import Providers
+from duckingit.providers import Providers
 
 
 class DuckSession:
     """Entrypoint to a session of serverless DuckDB instances
 
     The main objective of this class is to handle the session and serve as the primary
     entrypoint to a cluster of serverless functions that utilize DuckDB. Its core
```

### Comparing `duckingit-0.0.4/duckingit/_utils.py` & `duckingit-0.0.5/duckingit/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import itertools
 import hashlib
+import itertools
 import typing as t
 import uuid
 from collections.abc import Iterable
 
 import duckdb
 
 T = t.TypeVar("T")
@@ -46,34 +46,33 @@
 
     # Must not invoke more functions than number of search queries
     if (size := len(_list)) < number_of_invokations:
         number_of_invokations = size
 
     k, m = divmod(len(_list), number_of_invokations)
     return [
-        _list[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)]
-        for i in range(number_of_invokations)
+        _list[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)] for i in range(number_of_invokations)
     ]
 
 
 def create_hash_string(
-    string: str, algorithm: str = "md5", digits: int | None = None
+    string: str, algorithm: str = "md5", digits: int | None = None, first_char: str = ""
 ) -> str:
     algo = getattr(hashlib, algorithm)
     val = algo(string.encode(), usedforsecurity=False).hexdigest()
     if digits is None:
-        return val
-    return val[:digits]
+        return first_char + val
+    return first_char + val[:digits]
 
 
 def create_unique_name(prefix: str = "__duckingit") -> str:
     return f"{prefix}_{uuid.uuid1().hex[:6]}"
 
 
-def ensure_iterable(value: T | t.Iterable[T]) -> list[T]:
+def ensure_iterable(value: T | t.Iterable[T]) -> Iterable[T]:
     """Ensure to return an iterable
 
     Args:
         value, T | Iterable[T]: An arbitrary value
 
     Returns:
         Returns a list of type T, if T is not an iterable
@@ -94,15 +93,15 @@
         return [value]
 
     return value
 
 
 def create_conn_with_httpfs_loaded() -> duckdb.DuckDBPyConnection:
     """Returns a in memory DuckDB connection with httpfs loaded"""
-    from duckingit.integrations import Providers
+    from duckingit.providers import Providers
 
     conn = duckdb.connect(":memory:")
     conn.execute("LOAD httpfs;")
     conn.execute(Providers.AWS.credentials)
 
     return conn
```

### Comparing `duckingit-0.0.4/duckingit.egg-info/PKG-INFO` & `duckingit-0.0.5/duckingit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![logo](logo.png)
 
 A framework to leverage the endless capabilities of serverless computing powered by DuckDB.
 
 Please note that the framework currently supports only AWS Lambda functions. To use the framework, you must first create a Lambda layer of DuckDB that can be used within a Lambda function. Additionally, you must create a Lambda Executor function that can execute the actual DuckDB SQL. Once you've completed these setup steps, you can leverage the power of serverless functions through the SDK written in Python to perform analytics on a Data Lake.
 
@@ -51,15 +52,15 @@
 
 ```python
 from duckingit import DuckSession, DuckConfig
 
 query = "SELECT * FROM READ_PARQUET(['s3://BUCKET_NAME/2023/*'])"
 
 # Following command will print possible configurations
-DuckConfig.show_configurations
+DuckConfig.show_configurations()
 
 # Configuration
 conf = DuckConfig() \
         .set("aws_lambda.FunctionName", "TestFunc") \
         .set("aws_lambda.MemorySize", 256) \
         .set("aws_lambda.WarmUp", True)
```

### Comparing `duckingit-0.0.4/pyproject.toml` & `duckingit-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "duckingit"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   {name="Tobias Egelund", email="egelundtobias@gmail.com" },
 ]
 description = "A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["Serverless", "DuckDB", "Data Engineering"]
```

