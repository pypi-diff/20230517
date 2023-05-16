# Comparing `tmp/app_transport_framework_library-0.1.0.tar.gz` & `tmp/app_transport_framework_library-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_transport_framework_library-0.1.0.tar", max compression
+gzip compressed data, was "app_transport_framework_library-0.1.1.tar", max compression
```

## Comparing `app_transport_framework_library-0.1.0.tar` & `app_transport_framework_library-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1836 2023-05-16 21:00:23.693895 app_transport_framework_library-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-16 20:50:56.861597 app_transport_framework_library-0.1.0/app_transport_framework_library/__init__.py
--rw-r--r--   0        0        0     6555 2023-05-16 21:05:07.926034 app_transport_framework_library-0.1.0/app_transport_framework_library/atf_bundle_processor.py
--rw-r--r--   0        0        0      826 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.0/app_transport_framework_library/base_use_case_handler.py
--rw-r--r--   0        0        0      279 2023-05-16 21:02:55.215837 app_transport_framework_library-0.1.0/app_transport_framework_library/models/bundle_focus_content.py
--rw-r--r--   0        0        0      393 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.0/app_transport_framework_library/models/empfangsbestaetigung.py
--rw-r--r--   0        0        0      350 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.0/app_transport_framework_library/models/event.py
--rw-r--r--   0        0        0      295 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.0/app_transport_framework_library/models/message_to_send.py
--rw-r--r--   0        0        0     1138 2023-05-16 21:02:46.011962 app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/message_bundle_creator.py
--rw-r--r--   0        0        0     1197 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/message_header_creator.py
--rw-r--r--   0        0        0     1780 2023-05-16 21:03:31.391345 app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py
--rw-r--r--   0        0        0      838 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/operation_outcome_creator.py
--rw-r--r--   0        0        0     3905 2023-05-16 21:06:16.989096 app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/test_message_creator.py
--rw-r--r--   0        0        0     1698 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.0/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py
--rw-r--r--   0        0        0     1933 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.0/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py
--rw-r--r--   0        0        0      377 2023-05-16 20:53:03.255879 app_transport_framework_library-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 app_transport_framework_library-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3797 2023-05-16 21:57:35.169929 app_transport_framework_library-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 20:50:56.861597 app_transport_framework_library-0.1.1/app_transport_framework_library/__init__.py
+-rw-r--r--   0        0        0     6555 2023-05-16 21:05:07.926034 app_transport_framework_library-0.1.1/app_transport_framework_library/atf_bundle_processor.py
+-rw-r--r--   0        0        0      824 2023-05-16 21:36:51.746182 app_transport_framework_library-0.1.1/app_transport_framework_library/base_use_case_handler.py
+-rw-r--r--   0        0        0      279 2023-05-16 21:02:55.215837 app_transport_framework_library-0.1.1/app_transport_framework_library/models/bundle_focus_content.py
+-rw-r--r--   0        0        0      393 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.1/app_transport_framework_library/models/empfangsbestaetigung.py
+-rw-r--r--   0        0        0      350 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.1/app_transport_framework_library/models/event.py
+-rw-r--r--   0        0        0      295 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.1/app_transport_framework_library/models/message_to_send.py
+-rw-r--r--   0        0        0     1138 2023-05-16 21:02:46.011962 app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/message_bundle_creator.py
+-rw-r--r--   0        0        0     1197 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/message_header_creator.py
+-rw-r--r--   0        0        0     1780 2023-05-16 21:03:31.391345 app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py
+-rw-r--r--   0        0        0      838 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/operation_outcome_creator.py
+-rw-r--r--   0        0        0     3905 2023-05-16 21:06:16.989096 app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/test_message_creator.py
+-rw-r--r--   0        0        0     1613 2023-05-16 21:38:28.224802 app_transport_framework_library-0.1.1/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py
+-rw-r--r--   0        0        0     1931 2023-05-16 21:39:27.990263 app_transport_framework_library-0.1.1/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py
+-rw-r--r--   0        0        0      377 2023-05-16 22:01:15.012015 app_transport_framework_library-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 app_transport_framework_library-0.1.1/PKG-INFO
```

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/atf_bundle_processor.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/atf_bundle_processor.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/base_use_case_handler.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/base_use_case_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from abc import ABC, abstractmethod
-from typing import Tuple
+from typing import List, Tuple
 from fhir.resources.messageheader import MessageHeader, MessageHeaderSource
 from fhir.resources.bundle import Bundle, BundleEntry
 from fhir.resources.fhirtypes import ReferenceType
 
 from fhir.resources.operationoutcome import OperationOutcomeIssue
 
-from atf_message_library.atf_message_processor.models.event import Event
+from app_transport_framework_library.models.event import Event
+
+
 
 
 class BaseUseCaseHandler(ABC):
     def __init__(self, sender: ReferenceType, source: MessageHeaderSource):
         self.sender = sender
         self.source = source
         self.bundleEntries = []
         self.issues = []
         self.received_Empfangsbestaetigung_event = Event()
 
     @abstractmethod
-    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[list[BundleEntry], list[OperationOutcomeIssue]]:
+    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[List[BundleEntry], List[OperationOutcomeIssue]]:
         pass
```

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/message_bundle_creator.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/message_bundle_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/message_header_creator.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/message_header_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/operation_outcome_creator.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/operation_outcome_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/ressource_creators/test_message_creator.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/ressource_creators/test_message_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from typing import Tuple
+from typing import List, Tuple
 from fhir.resources.bundle import Bundle
 from fhir.resources.operationoutcome import OperationOutcome, OperationOutcomeIssue
 from fhir.resources.messageheader import MessageHeader
 from fhir.resources.bundle import BundleEntry
 
-from atf_message_library.atf_message_processor.base_use_case_handler import BaseUseCaseHandler
-from atf_message_library.atf_message_processor.models.empfangsbestaetigung import Empfangsbestaetigung
-from atf_message_library.atf_message_processor.models.event import Event
+from app_transport_framework_library.base_use_case_handler import BaseUseCaseHandler
+from app_transport_framework_library.models.empfangsbestaetigung import Empfangsbestaetigung
+
+
 
 
 class EmpfangsbestaetigungHandler(BaseUseCaseHandler):
 
     def resolve_reference(self, reference_str: str, bundle: Bundle):
         for entry in bundle.entry:
             if entry.resource.id == reference_str.split('urn:uuid:')[-1]:
                 return entry.resource
         return None
 
-    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[list[BundleEntry], list[OperationOutcomeIssue]]:
+    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[List[BundleEntry], List[OperationOutcomeIssue]]:
         self.bundleEntries = []
         self.issues = []
         message_header = self.get_ressource_by_type(bundle, MessageHeader)
         outcome = self.get_ressource_by_type(bundle, OperationOutcome)
         message_id = outcome.extension[0].valueString.split(
             'urn:uuid:')[-1]
         empfangsbestaetigung = Empfangsbestaetigung(
```

### Comparing `app_transport_framework_library-0.1.0/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py` & `app_transport_framework_library-0.1.1/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from typing import Tuple
+from typing import List, Tuple
 from fhir.resources.messageheader import MessageHeader
 from fhir.resources.bundle import Bundle
 from fhir.resources.bundle import Bundle
 from fhir.resources.operationoutcome import OperationOutcome, OperationOutcomeIssue
 from fhir.resources.messageheader import MessageHeader
 from fhir.resources.communication import Communication
 from fhir.resources.bundle import BundleEntry
 
-from atf_message_library.atf_message_processor.base_use_case_handler import BaseUseCaseHandler
+from app_transport_framework_library.base_use_case_handler import BaseUseCaseHandler
+
+
 
 
 class SelbsttestLieferungHandler(BaseUseCaseHandler):
     def resolve_reference(self, reference_str: str, bundle: Bundle):
         for entry in bundle.entry:
             if entry.resource.id == reference_str.split('urn:uuid:')[-1]:
                 return entry.resource
         return None
 
-    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[list[BundleEntry], list[OperationOutcomeIssue]]:
+    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[List[BundleEntry], List[OperationOutcomeIssue]]:
         self.bundleEntries = []
         self.issues = []
         if not any([isinstance(self.resolve_reference(focus_ref.reference, Bundle.parse_raw(bundle.json())), Communication) for focus_ref in message_header.focus]):
             self.issues.append(
                 OperationOutcomeIssue(
                     severity="fatal",
                     code="invalid",
```

