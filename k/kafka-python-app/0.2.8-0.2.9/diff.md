# Comparing `tmp/kafka_python_app-0.2.8.tar.gz` & `tmp/kafka_python_app-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_python_app-0.2.8.tar", last modified: Sat Mar 25 03:39:46 2023, max compression
+gzip compressed data, was "kafka_python_app-0.2.9.tar", last modified: Sat Mar 25 21:41:57 2023, max compression
```

## Comparing `kafka_python_app-0.2.8.tar` & `kafka_python_app-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2023-03-25 03:39:46.838997 kafka_python_app-0.2.8/
--rw-rw-r--   0 doc       (1000) doc       (1000)     1070 2022-04-11 01:45:36.000000 kafka_python_app-0.2.8/LICENSE.md
--rw-rw-r--   0 doc       (1000) doc       (1000)    11649 2023-03-25 03:39:46.838997 kafka_python_app-0.2.8/PKG-INFO
--rw-rw-r--   0 doc       (1000) doc       (1000)    11229 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/README.md
-drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2023-03-25 03:39:46.838997 kafka_python_app-0.2.8/kafka_python_app/
--rw-rw-r--   0 doc       (1000) doc       (1000)      723 2022-04-11 01:26:35.000000 kafka_python_app-0.2.8/kafka_python_app/__init__.py
--rw-rw-r--   0 doc       (1000) doc       (1000)    22107 2023-03-25 03:38:40.000000 kafka_python_app-0.2.8/kafka_python_app/app.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     6079 2023-03-07 23:38:19.000000 kafka_python_app-0.2.8/kafka_python_app/connector.py
-drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2023-03-25 03:39:46.838997 kafka_python_app-0.2.8/kafka_python_app.egg-info/
--rw-rw-r--   0 doc       (1000) doc       (1000)    11649 2023-03-25 03:39:46.000000 kafka_python_app-0.2.8/kafka_python_app.egg-info/PKG-INFO
--rw-rw-r--   0 doc       (1000) doc       (1000)      603 2023-03-25 03:39:46.000000 kafka_python_app-0.2.8/kafka_python_app.egg-info/SOURCES.txt
--rw-rw-r--   0 doc       (1000) doc       (1000)        1 2023-03-25 03:39:46.000000 kafka_python_app-0.2.8/kafka_python_app.egg-info/dependency_links.txt
--rw-rw-r--   0 doc       (1000) doc       (1000)       55 2023-03-25 03:39:46.000000 kafka_python_app-0.2.8/kafka_python_app.egg-info/requires.txt
--rw-rw-r--   0 doc       (1000) doc       (1000)       17 2023-03-25 03:39:46.000000 kafka_python_app-0.2.8/kafka_python_app.egg-info/top_level.txt
--rw-rw-r--   0 doc       (1000) doc       (1000)       38 2023-03-25 03:39:46.842997 kafka_python_app-0.2.8/setup.cfg
--rw-rw-r--   0 doc       (1000) doc       (1000)      846 2023-03-25 03:39:38.000000 kafka_python_app-0.2.8/setup.py
-drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2023-03-25 03:39:46.838997 kafka_python_app-0.2.8/tests/
--rw-rw-r--   0 doc       (1000) doc       (1000)     4450 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/tests/test_kafka_app.py
--rw-rw-r--   0 doc       (1000) doc       (1000)    13098 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/tests/test_kafka_app_emit_with_response.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     4513 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/tests/test_kafka_app_event_topic_filter.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     4359 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/tests/test_kafka_app_msg_key_as_event.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     6828 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/tests/test_kafka_app_pipelines.py
--rw-rw-r--   0 doc       (1000) doc       (1000)    15737 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/tests/test_kafka_app_pipelines_pipe_events.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     4437 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/tests/test_kafka_app_raw_msg.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     3148 2023-03-11 01:51:45.000000 kafka_python_app-0.2.8/tests/test_kafka_listener.py
+drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2023-03-25 21:41:57.857004 kafka_python_app-0.2.9/
+-rw-rw-r--   0 doc       (1000) doc       (1000)     1070 2022-04-11 01:45:36.000000 kafka_python_app-0.2.9/LICENSE.md
+-rw-rw-r--   0 doc       (1000) doc       (1000)    11649 2023-03-25 21:41:57.857004 kafka_python_app-0.2.9/PKG-INFO
+-rw-rw-r--   0 doc       (1000) doc       (1000)    11229 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/README.md
+drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2023-03-25 21:41:57.853004 kafka_python_app-0.2.9/kafka_python_app/
+-rw-rw-r--   0 doc       (1000) doc       (1000)      723 2022-04-11 01:26:35.000000 kafka_python_app-0.2.9/kafka_python_app/__init__.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)    21682 2023-03-25 21:20:30.000000 kafka_python_app-0.2.9/kafka_python_app/app.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     6079 2023-03-07 23:38:19.000000 kafka_python_app-0.2.9/kafka_python_app/connector.py
+drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2023-03-25 21:41:57.853004 kafka_python_app-0.2.9/kafka_python_app.egg-info/
+-rw-rw-r--   0 doc       (1000) doc       (1000)    11649 2023-03-25 21:41:57.000000 kafka_python_app-0.2.9/kafka_python_app.egg-info/PKG-INFO
+-rw-rw-r--   0 doc       (1000) doc       (1000)      603 2023-03-25 21:41:57.000000 kafka_python_app-0.2.9/kafka_python_app.egg-info/SOURCES.txt
+-rw-rw-r--   0 doc       (1000) doc       (1000)        1 2023-03-25 21:41:57.000000 kafka_python_app-0.2.9/kafka_python_app.egg-info/dependency_links.txt
+-rw-rw-r--   0 doc       (1000) doc       (1000)       55 2023-03-25 21:41:57.000000 kafka_python_app-0.2.9/kafka_python_app.egg-info/requires.txt
+-rw-rw-r--   0 doc       (1000) doc       (1000)       17 2023-03-25 21:41:57.000000 kafka_python_app-0.2.9/kafka_python_app.egg-info/top_level.txt
+-rw-rw-r--   0 doc       (1000) doc       (1000)       38 2023-03-25 21:41:57.857004 kafka_python_app-0.2.9/setup.cfg
+-rw-rw-r--   0 doc       (1000) doc       (1000)      846 2023-03-25 21:23:37.000000 kafka_python_app-0.2.9/setup.py
+drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2023-03-25 21:41:57.857004 kafka_python_app-0.2.9/tests/
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4450 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/tests/test_kafka_app.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)    13098 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/tests/test_kafka_app_emit_with_response.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4513 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/tests/test_kafka_app_event_topic_filter.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4359 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/tests/test_kafka_app_msg_key_as_event.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     6828 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/tests/test_kafka_app_pipelines.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)    15737 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/tests/test_kafka_app_pipelines_pipe_events.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4437 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/tests/test_kafka_app_raw_msg.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     3148 2023-03-11 01:51:45.000000 kafka_python_app-0.2.9/tests/test_kafka_listener.py
```

### Comparing `kafka_python_app-0.2.8/LICENSE.md` & `kafka_python_app-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/PKG-INFO` & `kafka_python_app-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka_python_app
-Version: 0.2.8
+Version: 0.2.9
 Summary: kafka application endpoint
 Home-page: https://github.com/doctor3030/kafka-python-app.git
 Author: Dmitry Amanov
 Author-email: dmitry.amanov@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kafka_python_app-0.2.8/README.md` & `kafka_python_app-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/kafka_python_app/__init__.py` & `kafka_python_app-0.2.9/kafka_python_app/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/kafka_python_app/app.py` & `kafka_python_app-0.2.9/kafka_python_app/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     pipe_to_topic: str
     with_response_options: Optional[TransactionPipeWithReturnOptions]
 
 
 class MessageTransaction(pydantic.BaseModel):
     fnc: Callable
     args: Optional[Dict]
-    pipe_result_options: Optional[Union[Callable, TransactionPipeResultOptions]]
+    pipe_result_options: Optional[TransactionPipeResultOptions]
 
 
 class MessagePipeline(pydantic.BaseModel):
     transactions: List[MessageTransaction]
     app_id: Optional[str]
     logger: Optional[Any]
 
@@ -64,24 +64,19 @@
                 else:
                     if tx.args:
                         message = tx.fnc(message, self.logger, **{**tx.args, **kwargs})
                     else:
                         message = tx.fnc(message, self.logger, **kwargs)
 
                 if tx.pipe_result_options:
-                    if inspect.isfunction(tx.pipe_result_options):
-                        pipe_result_options: TransactionPipeResultOptions = tx.pipe_result_options(message, self.logger,
-                                                                                                   **kwargs)
-                    else:
-                        pipe_result_options: TransactionPipeResultOptions = tx.pipe_result_options
-                    if pipe_result_options.with_response_options:
+                    if tx.pipe_result_options.with_response_options:
                         message = await self.pipe_event_with_response(message, emitter, message_key_as_event,
-                                                                      pipe_result_options, **kwargs)
+                                                                      tx.pipe_result_options, **kwargs)
                     else:
-                        self.pipe_event(message, emitter, message_key_as_event, pipe_result_options, **kwargs)
+                        self.pipe_event(message, emitter, message_key_as_event, tx.pipe_result_options, **kwargs)
         except Exception as e:
             self.logger.error(f'execute => Exception: '
                               f'type: {sys.exc_info()[0]}; '
                               f'line#: {sys.exc_info()[2].tb_lineno}; '
                               f'msg: {str(e)}')
 
     def pipe_event(
@@ -466,15 +461,15 @@
                         await asyncio.sleep(0.001)
                     else:
                         raise TimeoutError(f'Emit event with response timeout: '
                                            # f'emitted event: {message.key if self.config.message_key_as_event else message.value["event"]}; '
                                            f'to: {topic}; '
                                            f'event_id: {event_id}')
         except Exception as e:
-            self.logger.error(f'txn_es_common => Exception: '
+            self.logger.error(f'emit_with_response => Exception: '
                               f'type: {sys.exc_info()[0]}; '
                               f'line#: {sys.exc_info()[2].tb_lineno}; '
                               f'msg: {str(e)}')
 
     async def process_sync_tasks(self):
         while True:
             if self.stop:
```

### Comparing `kafka_python_app-0.2.8/kafka_python_app/connector.py` & `kafka_python_app-0.2.9/kafka_python_app/connector.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/kafka_python_app.egg-info/PKG-INFO` & `kafka_python_app-0.2.9/kafka_python_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-python-app
-Version: 0.2.8
+Version: 0.2.9
 Summary: kafka application endpoint
 Home-page: https://github.com/doctor3030/kafka-python-app.git
 Author: Dmitry Amanov
 Author-email: dmitry.amanov@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kafka_python_app-0.2.8/kafka_python_app.egg-info/SOURCES.txt` & `kafka_python_app-0.2.9/kafka_python_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/setup.py` & `kafka_python_app-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ROOOT = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (ROOOT / "README.md").read_text()
 
 setup(
     name='kafka_python_app',
-    version="0.2.8",
+    version="0.2.9",
     author="Dmitry Amanov",
     author_email="dmitry.amanov@gmail.com",
     description="kafka application endpoint",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/doctor3030/kafka-python-app.git",
     license="MIT",
```

### Comparing `kafka_python_app-0.2.8/tests/test_kafka_app.py` & `kafka_python_app-0.2.9/tests/test_kafka_app.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/tests/test_kafka_app_emit_with_response.py` & `kafka_python_app-0.2.9/tests/test_kafka_app_emit_with_response.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/tests/test_kafka_app_event_topic_filter.py` & `kafka_python_app-0.2.9/tests/test_kafka_app_event_topic_filter.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/tests/test_kafka_app_msg_key_as_event.py` & `kafka_python_app-0.2.9/tests/test_kafka_app_msg_key_as_event.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/tests/test_kafka_app_pipelines.py` & `kafka_python_app-0.2.9/tests/test_kafka_app_pipelines.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/tests/test_kafka_app_pipelines_pipe_events.py` & `kafka_python_app-0.2.9/tests/test_kafka_app_pipelines_pipe_events.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/tests/test_kafka_app_raw_msg.py` & `kafka_python_app-0.2.9/tests/test_kafka_app_raw_msg.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.2.8/tests/test_kafka_listener.py` & `kafka_python_app-0.2.9/tests/test_kafka_listener.py`

 * *Files identical despite different names*

