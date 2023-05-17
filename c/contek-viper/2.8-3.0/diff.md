# Comparing `tmp/contek-viper-2.8.tar.gz` & `tmp/contek-viper-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contek-viper-2.8.tar", last modified: Wed May 17 03:23:56 2023, max compression
+gzip compressed data, was "contek-viper-3.0.tar", last modified: Thu Jun 16 03:24:07 2022, max compression
```

## Comparing `contek-viper-2.8.tar` & `contek-viper-3.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 03:23:56.190558 contek-viper-2.8/
--rw-rw-rw-   0        0        0      387 2023-05-17 03:23:56.189557 contek-viper-2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 03:23:56.177547 contek-viper-2.8/contek_viper/
--rw-rw-rw-   0        0        0        0 2022-12-28 05:15:12.000000 contek-viper-2.8/contek_viper/__init__.py
--rw-rw-rw-   0        0        0      778 2022-10-19 08:35:58.000000 contek-viper-2.8/contek_viper/account_session.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:23:56.187555 contek-viper-2.8/contek_viper/execution/
--rw-rw-rw-   0        0        0        0 2022-08-26 07:36:52.000000 contek-viper-2.8/contek_viper/execution/__init__.py
--rw-rw-rw-   0        0        0     3118 2023-05-17 03:23:08.000000 contek-viper-2.8/contek_viper/execution/execution_service_pb2.py
--rw-rw-rw-   0        0        0     2904 2023-05-17 03:23:08.000000 contek-viper-2.8/contek_viper/execution/execution_service_pb2_grpc.py
--rw-rw-rw-   0        0        0      694 2022-10-19 08:35:58.000000 contek-viper-2.8/contek_viper/trigger_api.py
--rw-rw-rw-   0        0        0      811 2022-10-19 08:35:58.000000 contek-viper-2.8/contek_viper/viper_client.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:23:56.184553 contek-viper-2.8/contek_viper.egg-info/
--rw-rw-rw-   0        0        0      387 2023-05-17 03:23:56.000000 contek-viper-2.8/contek_viper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-17 03:23:56.000000 contek-viper-2.8/contek_viper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 03:23:56.000000 contek-viper-2.8/contek_viper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-17 03:23:56.000000 contek-viper-2.8/contek_viper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 03:23:56.000000 contek-viper-2.8/contek_viper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 03:23:56.000000 contek-viper-2.8/contek_viper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-17 03:23:56.190558 contek-viper-2.8/setup.cfg
--rw-rw-rw-   0        0        0      936 2023-05-17 03:23:51.000000 contek-viper-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-16 03:24:07.300425 contek-viper-3.0/
+-rw-rw-rw-   0        0        0      387 2022-06-16 03:24:07.299425 contek-viper-3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-06-16 03:24:07.283410 contek-viper-3.0/contek_viper/
+-rw-rw-rw-   0        0        0        0 2022-03-30 08:22:37.000000 contek-viper-3.0/contek_viper/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-16 03:24:07.297423 contek-viper-3.0/contek_viper/execution/
+-rw-rw-rw-   0        0        0        0 2022-03-30 08:22:37.000000 contek-viper-3.0/contek_viper/execution/__init__.py
+-rw-rw-rw-   0        0        0     2797 2022-06-16 03:23:46.000000 contek-viper-3.0/contek_viper/execution/execution_service_pb2.py
+-rw-rw-rw-   0        0        0     2982 2022-06-16 03:23:46.000000 contek-viper-3.0/contek_viper/execution/execution_service_pb2_grpc.py
+-rw-rw-rw-   0        0        0     1470 2022-06-16 03:23:46.000000 contek-viper-3.0/contek_viper/execution/market_signal_pb2.py
+-rw-rw-rw-   0        0        0      963 2022-06-16 03:23:46.000000 contek-viper-3.0/contek_viper/viper_client.py
+drwxrwxrwx   0        0        0        0 2022-06-16 03:24:07.292418 contek-viper-3.0/contek_viper.egg-info/
+-rw-rw-rw-   0        0        0      387 2022-06-16 03:24:07.000000 contek-viper-3.0/contek_viper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2022-06-16 03:24:07.000000 contek-viper-3.0/contek_viper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-16 03:24:07.000000 contek-viper-3.0/contek_viper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2022-06-16 03:24:07.000000 contek-viper-3.0/contek_viper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-06-16 03:24:07.000000 contek-viper-3.0/contek_viper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-06-16 03:24:07.000000 contek-viper-3.0/contek_viper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2022-06-16 03:24:07.300425 contek-viper-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      895 2022-06-16 03:23:57.000000 contek-viper-3.0/setup.py
```

### Comparing `contek-viper-2.8/contek_viper/account_session.py` & `contek-viper-3.0/contek_viper/viper_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+from __future__ import annotations
+
 from typing import Iterable
 
-from contek_viper.execution.execution_service_pb2 import MarketSignal, SubmitMarketSignalsRequest
+import grpc
+
+from contek_viper.execution.execution_service_pb2 import SubmitMarketSignalsRequest
 from contek_viper.execution.execution_service_pb2_grpc import ExecutionServiceStub
+from contek_viper.execution.market_signal_pb2 import MarketSignal
 
 
-class AccountSession:
+class ViperClient:
 
-    def __init__(
-        self,
-        exchange: str,
-        account: str,
-        stub: ExecutionServiceStub,
-    ) -> None:
-        self._exchange = exchange
-        self._account = account
+    def __init__(self, stub: ExecutionServiceStub) -> None:
         self._stub = stub
 
-    def submit(self, market_signals: Iterable[MarketSignal]) -> None:
+    @classmethod
+    def create(cls, server_address: str) -> ViperClient:
+        channel = grpc.insecure_channel(server_address)
+        stub = ExecutionServiceStub(channel)
+        return cls(stub)
+
+    def submit(
+        self,
+        trigger_name: str,
+        market_signals: Iterable[MarketSignal],
+    ) -> None:
         self._stub.SubmitMarketSignals(
             SubmitMarketSignalsRequest(
+                trigger_name=trigger_name,
                 market_signal=list(market_signals),
-                exchange=self._exchange,
-                account=self._account,
             ))
```

### Comparing `contek-viper-2.8/contek_viper/execution/execution_service_pb2.py` & `contek-viper-3.0/contek_viper/execution/execution_service_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,51 +8,42 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from contek_viper.execution import market_signal_pb2 as contek__viper_dot_execution_dot_market__signal__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.contek_viper/execution/execution_service.proto\x12\x16\x63ontek_viper.execution\"p\n\x14SubmitTriggerRequest\x12\x14\n\x0ctrigger_name\x18\x01 \x01(\t\x12\x42\n\rmarket_signal\x18\x02 \x03(\x0b\x32+.contek_viper.execution.TriggerMarketSignal\"\x17\n\x15SubmitTriggerResponse\"5\n\x13TriggerMarketSignal\x12\x0e\n\x06market\x18\x01 \x01(\t\x12\x0e\n\x06signal\x18\x02 \x01(\x01\x32\x82\x01\n\x10\x45xecutionService\x12n\n\rSubmitTrigger\x12,.contek_viper.execution.SubmitTriggerRequest\x1a-.contek_viper.execution.SubmitTriggerResponse\"\x00\x42\x1d\n\x19io.contek.viper.executionP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.contek_viper/execution/execution_service.proto\x12\x16\x63ontek_viper.execution\x1a*contek_viper/execution/market_signal.proto\"o\n\x1aSubmitMarketSignalsRequest\x12\x14\n\x0ctrigger_name\x18\x01 \x01(\t\x12;\n\rmarket_signal\x18\x02 \x03(\x0b\x32$.contek_viper.execution.MarketSignal\"\x1d\n\x1bSubmitMarketSignalsResponse2\x95\x01\n\x10\x45xecutionService\x12\x80\x01\n\x13SubmitMarketSignals\x12\x32.contek_viper.execution.SubmitMarketSignalsRequest\x1a\x33.contek_viper.execution.SubmitMarketSignalsResponse\"\x00\x42\x1d\n\x19io.contek.viper.executionP\x01\x62\x06proto3')
 
 
 
-_SUBMITTRIGGERREQUEST = DESCRIPTOR.message_types_by_name['SubmitTriggerRequest']
-_SUBMITTRIGGERRESPONSE = DESCRIPTOR.message_types_by_name['SubmitTriggerResponse']
-_TRIGGERMARKETSIGNAL = DESCRIPTOR.message_types_by_name['TriggerMarketSignal']
-SubmitTriggerRequest = _reflection.GeneratedProtocolMessageType('SubmitTriggerRequest', (_message.Message,), {
-  'DESCRIPTOR' : _SUBMITTRIGGERREQUEST,
+_SUBMITMARKETSIGNALSREQUEST = DESCRIPTOR.message_types_by_name['SubmitMarketSignalsRequest']
+_SUBMITMARKETSIGNALSRESPONSE = DESCRIPTOR.message_types_by_name['SubmitMarketSignalsResponse']
+SubmitMarketSignalsRequest = _reflection.GeneratedProtocolMessageType('SubmitMarketSignalsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SUBMITMARKETSIGNALSREQUEST,
   '__module__' : 'contek_viper.execution.execution_service_pb2'
-  # @@protoc_insertion_point(class_scope:contek_viper.execution.SubmitTriggerRequest)
+  # @@protoc_insertion_point(class_scope:contek_viper.execution.SubmitMarketSignalsRequest)
   })
-_sym_db.RegisterMessage(SubmitTriggerRequest)
+_sym_db.RegisterMessage(SubmitMarketSignalsRequest)
 
-SubmitTriggerResponse = _reflection.GeneratedProtocolMessageType('SubmitTriggerResponse', (_message.Message,), {
-  'DESCRIPTOR' : _SUBMITTRIGGERRESPONSE,
+SubmitMarketSignalsResponse = _reflection.GeneratedProtocolMessageType('SubmitMarketSignalsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _SUBMITMARKETSIGNALSRESPONSE,
   '__module__' : 'contek_viper.execution.execution_service_pb2'
-  # @@protoc_insertion_point(class_scope:contek_viper.execution.SubmitTriggerResponse)
+  # @@protoc_insertion_point(class_scope:contek_viper.execution.SubmitMarketSignalsResponse)
   })
-_sym_db.RegisterMessage(SubmitTriggerResponse)
-
-TriggerMarketSignal = _reflection.GeneratedProtocolMessageType('TriggerMarketSignal', (_message.Message,), {
-  'DESCRIPTOR' : _TRIGGERMARKETSIGNAL,
-  '__module__' : 'contek_viper.execution.execution_service_pb2'
-  # @@protoc_insertion_point(class_scope:contek_viper.execution.TriggerMarketSignal)
-  })
-_sym_db.RegisterMessage(TriggerMarketSignal)
+_sym_db.RegisterMessage(SubmitMarketSignalsResponse)
 
 _EXECUTIONSERVICE = DESCRIPTOR.services_by_name['ExecutionService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\031io.contek.viper.executionP\001'
-  _SUBMITTRIGGERREQUEST._serialized_start=74
-  _SUBMITTRIGGERREQUEST._serialized_end=186
-  _SUBMITTRIGGERRESPONSE._serialized_start=188
-  _SUBMITTRIGGERRESPONSE._serialized_end=211
-  _TRIGGERMARKETSIGNAL._serialized_start=213
-  _TRIGGERMARKETSIGNAL._serialized_end=266
-  _EXECUTIONSERVICE._serialized_start=269
-  _EXECUTIONSERVICE._serialized_end=399
+  _SUBMITMARKETSIGNALSREQUEST._serialized_start=118
+  _SUBMITMARKETSIGNALSREQUEST._serialized_end=229
+  _SUBMITMARKETSIGNALSRESPONSE._serialized_start=231
+  _SUBMITMARKETSIGNALSRESPONSE._serialized_end=260
+  _EXECUTIONSERVICE._serialized_start=263
+  _EXECUTIONSERVICE._serialized_end=412
 # @@protoc_insertion_point(module_scope)
```

### Comparing `contek-viper-2.8/contek_viper/execution/execution_service_pb2_grpc.py` & `contek-viper-3.0/contek_viper/execution/execution_service_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,57 +10,57 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.SubmitTrigger = channel.unary_unary(
-                '/contek_viper.execution.ExecutionService/SubmitTrigger',
-                request_serializer=contek__viper_dot_execution_dot_execution__service__pb2.SubmitTriggerRequest.SerializeToString,
-                response_deserializer=contek__viper_dot_execution_dot_execution__service__pb2.SubmitTriggerResponse.FromString,
+        self.SubmitMarketSignals = channel.unary_unary(
+                '/contek_viper.execution.ExecutionService/SubmitMarketSignals',
+                request_serializer=contek__viper_dot_execution_dot_execution__service__pb2.SubmitMarketSignalsRequest.SerializeToString,
+                response_deserializer=contek__viper_dot_execution_dot_execution__service__pb2.SubmitMarketSignalsResponse.FromString,
                 )
 
 
 class ExecutionServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def SubmitTrigger(self, request, context):
+    def SubmitMarketSignals(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ExecutionServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'SubmitTrigger': grpc.unary_unary_rpc_method_handler(
-                    servicer.SubmitTrigger,
-                    request_deserializer=contek__viper_dot_execution_dot_execution__service__pb2.SubmitTriggerRequest.FromString,
-                    response_serializer=contek__viper_dot_execution_dot_execution__service__pb2.SubmitTriggerResponse.SerializeToString,
+            'SubmitMarketSignals': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubmitMarketSignals,
+                    request_deserializer=contek__viper_dot_execution_dot_execution__service__pb2.SubmitMarketSignalsRequest.FromString,
+                    response_serializer=contek__viper_dot_execution_dot_execution__service__pb2.SubmitMarketSignalsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'contek_viper.execution.ExecutionService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class ExecutionService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def SubmitTrigger(request,
+    def SubmitMarketSignals(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/contek_viper.execution.ExecutionService/SubmitTrigger',
-            contek__viper_dot_execution_dot_execution__service__pb2.SubmitTriggerRequest.SerializeToString,
-            contek__viper_dot_execution_dot_execution__service__pb2.SubmitTriggerResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/contek_viper.execution.ExecutionService/SubmitMarketSignals',
+            contek__viper_dot_execution_dot_execution__service__pb2.SubmitMarketSignalsRequest.SerializeToString,
+            contek__viper_dot_execution_dot_execution__service__pb2.SubmitMarketSignalsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `contek-viper-2.8/setup.py` & `contek-viper-3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,31 +8,29 @@
         import build_protos
         build_protos.rebuild()
         build_py.run(self)
 
 
 setup(
     name='contek-viper',
-    version='2.8',
+    version='3.0',
     description='Viper Python Client',
     url='https://contek.io',
     author='contek_bjy',
     author_email='bjy@contek.io',
     license='private',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         'License :: Other/Proprietary License',
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.6',
     py_modules=['contek_viper'],
     install_requires=[
-        'grpcio==1.48.2',
-        'protobuf==4.21.7',
-    ],
-    setup_requires=[
-        'grpcio-tools==1.48.2',
+        'grpcio',
+        'protobuf',
     ],
+    setup_requires=['grpcio-tools'],
     cmdclass={'build_py': _BuildProtos},
     zip_safe=True,
 )
```

