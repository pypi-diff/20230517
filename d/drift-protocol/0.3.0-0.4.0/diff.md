# Comparing `tmp/drift_protocol-0.3.0-py3-none-any.whl.zip` & `tmp/drift_protocol-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 12043 bytes, number of entries: 14
--rw-r--r--  2.0 unx      285 b- defN 22-Nov-30 16:04 drift_protocol/__init__.py
--rw-r--r--  2.0 unx       96 b- defN 22-Nov-30 16:04 drift_protocol/common/__init__.py
--rw-r--r--  2.0 unx     2580 b- defN 22-Nov-30 16:04 drift_protocol/common/data_payload_pb2.py
--rw-r--r--  2.0 unx     5909 b- defN 22-Nov-30 16:04 drift_protocol/common/drift_package_pb2.py
--rw-r--r--  2.0 unx     4542 b- defN 22-Nov-30 16:04 drift_protocol/common/status_code_pb2.py
--rw-r--r--  2.0 unx       29 b- defN 22-Nov-30 16:04 drift_protocol/meta/__init__.py
--rw-r--r--  2.0 unx    24799 b- defN 22-Nov-30 16:04 drift_protocol/meta/meta_info_pb2.py
--rw-r--r--  2.0 unx       79 b- defN 22-Nov-30 16:04 drift_protocol/trigger_service/__init__.py
--rw-r--r--  2.0 unx     3454 b- defN 22-Nov-30 16:04 drift_protocol/trigger_service/interval_trigger_message_pb2.py
--rw-r--r--  2.0 unx     2622 b- defN 22-Nov-30 16:04 drift_protocol/trigger_service/trigger_message_pb2.py
--rw-r--r--  2.0 unx     1805 b- defN 22-Nov-30 16:04 drift_protocol-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-30 16:04 drift_protocol-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 22-Nov-30 16:04 drift_protocol-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1296 b- defN 22-Nov-30 16:04 drift_protocol-0.3.0.dist-info/RECORD
-14 files, 47603 bytes uncompressed, 9833 bytes compressed:  79.3%
+Zip file size: 12243 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      285 b- defN 23-May-17 14:53 drift_protocol/__init__.py
+-rw-r--r--  2.0 unx       96 b- defN 23-May-17 14:53 drift_protocol/common/__init__.py
+-rw-r--r--  2.0 unx     2580 b- defN 23-May-17 14:53 drift_protocol/common/data_payload_pb2.py
+-rw-r--r--  2.0 unx     8282 b- defN 23-May-17 14:53 drift_protocol/common/drift_package_pb2.py
+-rw-r--r--  2.0 unx     4542 b- defN 23-May-17 14:53 drift_protocol/common/status_code_pb2.py
+-rw-r--r--  2.0 unx       29 b- defN 23-May-17 14:53 drift_protocol/meta/__init__.py
+-rw-r--r--  2.0 unx    24799 b- defN 23-May-17 14:53 drift_protocol/meta/meta_info_pb2.py
+-rw-r--r--  2.0 unx       79 b- defN 23-May-17 14:53 drift_protocol/trigger_service/__init__.py
+-rw-r--r--  2.0 unx     3454 b- defN 23-May-17 14:53 drift_protocol/trigger_service/interval_trigger_message_pb2.py
+-rw-r--r--  2.0 unx     2622 b- defN 23-May-17 14:53 drift_protocol/trigger_service/trigger_message_pb2.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-May-17 14:53 drift_protocol-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 14:53 drift_protocol-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-17 14:53 drift_protocol-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1296 b- defN 23-May-17 14:53 drift_protocol-0.4.0.dist-info/RECORD
+14 files, 49978 bytes uncompressed, 10033 bytes compressed:  79.9%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: drift_protocol/trigger_service/interval_trigger_message_pb2.py
 Comment: 
 
 Filename: drift_protocol/trigger_service/trigger_message_pb2.py
 Comment: 
 
-Filename: drift_protocol-0.3.0.dist-info/METADATA
+Filename: drift_protocol-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: drift_protocol-0.3.0.dist-info/WHEEL
+Filename: drift_protocol-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: drift_protocol-0.3.0.dist-info/top_level.txt
+Filename: drift_protocol-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: drift_protocol-0.3.0.dist-info/RECORD
+Filename: drift_protocol-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drift_protocol/__init__.py

```diff
@@ -1,8 +1,8 @@
 """ Auto-generated file for package with generated protobuf bindings
 """
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 import google.protobuf as protobuf
 
 if protobuf.__version__ < '3.12.4':
     raise RuntimeError(f'Version of protobuf PIP package must be >=3.12.4. However you have {protobuf.__version__}')
```

## drift_protocol/common/drift_package_pb2.py

```diff
@@ -19,21 +19,59 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='drift_protocol/common/drift_package.proto',
   package='drift.proto.common',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n)drift_protocol/common/drift_package.proto\x12\x12\x64rift.proto.common\x1a\x19google/protobuf/any.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\'drift_protocol/common/status_code.proto\x1a#drift_protocol/meta/meta_info.proto\"\x85\x02\n\x0c\x44riftPackage\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x34\n\x10source_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11publish_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x06status\x18\x04 \x01(\x0e\x32\x1e.drift.proto.common.StatusCode\x12\"\n\x04\x64\x61ta\x18\x05 \x03(\x0b\x32\x14.google.protobuf.Any\x12(\n\x04meta\x18\x06 \x01(\x0b\x32\x1a.drift.proto.meta.MetaInfob\x06proto3'
+  serialized_pb=b'\n)drift_protocol/common/drift_package.proto\x12\x12\x64rift.proto.common\x1a\x19google/protobuf/any.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\'drift_protocol/common/status_code.proto\x1a#drift_protocol/meta/meta_info.proto\"\xe2\x02\n\x0c\x44riftPackage\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x34\n\x10source_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11publish_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x06status\x18\x04 \x01(\x0e\x32\x1e.drift.proto.common.StatusCode\x12\"\n\x04\x64\x61ta\x18\x05 \x03(\x0b\x32\x14.google.protobuf.Any\x12(\n\x04meta\x18\x06 \x01(\x0b\x32\x1a.drift.proto.meta.MetaInfo\x12\x36\n\x06labels\x18\x07 \x03(\x0b\x32&.drift.proto.common.DriftPackage.Label\x1a#\n\x05Label\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\tb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_any__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,drift__protocol_dot_common_dot_status__code__pb2.DESCRIPTOR,drift__protocol_dot_meta_dot_meta__info__pb2.DESCRIPTOR,])
 
 
 
 
+_DRIFTPACKAGE_LABEL = _descriptor.Descriptor(
+  name='Label',
+  full_name='drift.proto.common.DriftPackage.Label',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='drift.proto.common.DriftPackage.Label.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='drift.proto.common.DriftPackage.Label.value', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=523,
+  serialized_end=558,
+)
+
 _DRIFTPACKAGE = _descriptor.Descriptor(
   name='DriftPackage',
   full_name='drift.proto.common.DriftPackage',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -76,40 +114,57 @@
     _descriptor.FieldDescriptor(
       name='meta', full_name='drift.proto.common.DriftPackage.meta', index=5,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='labels', full_name='drift.proto.common.DriftPackage.labels', index=6,
+      number=7, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_DRIFTPACKAGE_LABEL, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=204,
-  serialized_end=465,
+  serialized_end=558,
 )
 
+_DRIFTPACKAGE_LABEL.containing_type = _DRIFTPACKAGE
 _DRIFTPACKAGE.fields_by_name['source_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DRIFTPACKAGE.fields_by_name['publish_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DRIFTPACKAGE.fields_by_name['status'].enum_type = drift__protocol_dot_common_dot_status__code__pb2._STATUSCODE
 _DRIFTPACKAGE.fields_by_name['data'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _DRIFTPACKAGE.fields_by_name['meta'].message_type = drift__protocol_dot_meta_dot_meta__info__pb2._METAINFO
+_DRIFTPACKAGE.fields_by_name['labels'].message_type = _DRIFTPACKAGE_LABEL
 DESCRIPTOR.message_types_by_name['DriftPackage'] = _DRIFTPACKAGE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 DriftPackage = _reflection.GeneratedProtocolMessageType('DriftPackage', (_message.Message,), {
+
+  'Label' : _reflection.GeneratedProtocolMessageType('Label', (_message.Message,), {
+    'DESCRIPTOR' : _DRIFTPACKAGE_LABEL,
+    '__module__' : 'drift_protocol.common.drift_package_pb2'
+    # @@protoc_insertion_point(class_scope:drift.proto.common.DriftPackage.Label)
+    })
+  ,
   'DESCRIPTOR' : _DRIFTPACKAGE,
   '__module__' : 'drift_protocol.common.drift_package_pb2'
   # @@protoc_insertion_point(class_scope:drift.proto.common.DriftPackage)
   })
 _sym_db.RegisterMessage(DriftPackage)
+_sym_db.RegisterMessage(DriftPackage.Label)
 
 
 # @@protoc_insertion_point(module_scope)
```

## Comparing `drift_protocol-0.3.0.dist-info/METADATA` & `drift_protocol-0.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: drift-protocol
-Version: 0.3.0
+Version: 0.4.0
 Summary: Protobuf Libraries to encode message in Drift infrastructure
 Home-page: https://github.com/panda-official/DriftProtocol/
 Author: PANDA, GmbH
 Author-email: info@panda.technology
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: protobuf (<=3.20,>=3.12.4)
+Requires-Dist: protobuf (<=3.20.3,>=3.12.4)
 
 # Drift Protocol for Python
 
 A Python Protobuf library to encode message in Drift infrastructure.
 It provides pre-generated Protobuf messages so that you don't need to install protobuf compiler and generate them
 yourself.
```

## Comparing `drift_protocol-0.3.0.dist-info/RECORD` & `drift_protocol-0.4.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-drift_protocol/__init__.py,sha256=tcGdIJyOdlwTO5uf9NKRBqekJNVior37Sfp43tyZAf8,285
+drift_protocol/__init__.py,sha256=wO6ilg3tO-Y1IXZ2HPfiGn1lc-Oj8NFABf_bvmlGCOg,285
 drift_protocol/common/__init__.py,sha256=5h0oJrSznVY4PQHVPf3-nsV5-A_UKFawOS8x0JCShAw,96
 drift_protocol/common/data_payload_pb2.py,sha256=JRVWR043i9CKok3Lo_twtyKMgLiPLYpysVCqrYR17nU,2580
-drift_protocol/common/drift_package_pb2.py,sha256=x7Rm3GH8v2roIuOBSO54tn7WMAmmS8fhVjj8n2l27es,5909
+drift_protocol/common/drift_package_pb2.py,sha256=Lgf7_HNKqGzA_3dtCALDlAlLJ1h7oCwhVyXtBilQb5M,8282
 drift_protocol/common/status_code_pb2.py,sha256=P2qnFsTCcx7hugviaA2yV5nM2PWKEMyjgVzVRoJawOo,4542
 drift_protocol/meta/__init__.py,sha256=qu7lcUVJvYebLqo4tSmTX66klkF9333pFiqjZaTaPQA,29
 drift_protocol/meta/meta_info_pb2.py,sha256=Rki1STfRa8hFqOkZITb9MSpvpoxStv2Vq7H1tJA-CV4,24799
 drift_protocol/trigger_service/__init__.py,sha256=BqR5M-dhiYxaAeEpZWnNxiq1OM9tTZ951mCt4XcM054,79
 drift_protocol/trigger_service/interval_trigger_message_pb2.py,sha256=93LNGo2Uf3s47bZ5mcBV6HlOcDbjEaxIHo1JhOl_GQk,3454
 drift_protocol/trigger_service/trigger_message_pb2.py,sha256=wbPLot0W6_msZifQGulaElWaqp05eb9hPPbw35CZW2U,2622
-drift_protocol-0.3.0.dist-info/METADATA,sha256=N55XPAVEbSUySQGJDij1lKbXkfZAbqM_E-QnYTTDWLI,1805
-drift_protocol-0.3.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-drift_protocol-0.3.0.dist-info/top_level.txt,sha256=DbRiBVI9rCZ4d5UjXFR8gRrV-dJuSoWEsiNhNA8wcns,15
-drift_protocol-0.3.0.dist-info/RECORD,,
+drift_protocol-0.4.0.dist-info/METADATA,sha256=vBZVHv3KlaxgheUg_zmhvLOKUZ5RXxmb0QCiiLZXt4s,1807
+drift_protocol-0.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+drift_protocol-0.4.0.dist-info/top_level.txt,sha256=DbRiBVI9rCZ4d5UjXFR8gRrV-dJuSoWEsiNhNA8wcns,15
+drift_protocol-0.4.0.dist-info/RECORD,,
```

