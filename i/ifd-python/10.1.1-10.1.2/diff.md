# Comparing `tmp/ifd_python-10.1.1.tar.gz` & `tmp/ifd_python-10.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-10.1.1.tar", max compression
+gzip compressed data, was "ifd_python-10.1.2.tar", max compression
```

## Comparing `ifd_python-10.1.1.tar` & `ifd_python-10.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1093 2023-05-16 13:28:13.433655 ifd_python-10.1.1/LICENSE
--rw-r--r--   0        0        0      551 2023-05-16 13:28:13.433655 ifd_python-10.1.1/README.md
--rw-r--r--   0        0        0      283 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      630 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/BodyTicket.py
--rw-r--r--   0        0        0      734 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2303 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Image.py
--rw-r--r--   0        0        0      730 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Intervention.py
--rw-r--r--   0        0        0     1428 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      741 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Malfacon.py
--rw-r--r--   0        0        0      477 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Modele.py
--rw-r--r--   0        0        0      794 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/OCR.py
--rw-r--r--   0        0        0      529 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0     1033 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Tag.py
--rw-r--r--   0        0        0      423 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/Ticket.py
--rw-r--r--   0        0        0      400 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2161 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0     2215 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/repository/RestTicketRepository.py
--rw-r--r--   0        0        0      986 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/repository/SqlLogRepository.py
--rw-r--r--   0        0        0     2009 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/repository/SqlTicketRepository.py
--rw-r--r--   0        0        0      210 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/repository/__init__.py
--rw-r--r--   0        0        0      940 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/repository/abstract/AbsSqlRepository.py
--rw-r--r--   0        0        0       46 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/repository/abstract/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/spec.py
--rw-r--r--   0        0        0      526 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-05-16 13:28:13.433655 ifd_python-10.1.1/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 13:28:13.449655 ifd_python-10.1.1/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      407 2023-05-16 13:28:22.997777 ifd_python-10.1.1/pyproject.toml
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 ifd_python-10.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-16 13:28:13.433655 ifd_python-10.1.2/LICENSE
+-rw-r--r--   0        0        0      551 2023-05-16 13:28:13.433655 ifd_python-10.1.2/README.md
+-rw-r--r--   0        0        0      283 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/BodyTicket.py
+-rw-r--r--   0        0        0      734 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2303 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Image.py
+-rw-r--r--   0        0        0      730 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Intervention.py
+-rw-r--r--   0        0        0     1428 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      741 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Malfacon.py
+-rw-r--r--   0        0        0      477 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      794 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      529 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0     1033 2023-05-17 09:32:12.521357 ifd_python-10.1.2/ifd/entities/Tag.py
+-rw-r--r--   0        0        0      423 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/Ticket.py
+-rw-r--r--   0        0        0      400 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2161 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0     2215 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/repository/RestTicketRepository.py
+-rw-r--r--   0        0        0      986 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/repository/SqlLogRepository.py
+-rw-r--r--   0        0        0     2009 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/repository/SqlTicketRepository.py
+-rw-r--r--   0        0        0      210 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/repository/abstract/AbsSqlRepository.py
+-rw-r--r--   0        0        0       46 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/repository/abstract/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/spec.py
+-rw-r--r--   0        0        0      526 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-05-16 13:28:13.433655 ifd_python-10.1.2/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 09:32:12.537356 ifd_python-10.1.2/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-17 09:32:21.377277 ifd_python-10.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 ifd_python-10.1.2/PKG-INFO
```

### Comparing `ifd_python-10.1.1/LICENSE` & `ifd_python-10.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/README.md` & `ifd_python-10.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/Abstract/ADetection.py` & `ifd_python-10.1.2/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/BodyTicket.py` & `ifd_python-10.1.2/ifd/entities/BodyTicket.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/Classification.py` & `ifd_python-10.1.2/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/Detection.py` & `ifd_python-10.1.2/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/Image.py` & `ifd_python-10.1.2/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/Intervention.py` & `ifd_python-10.1.2/ifd/entities/Intervention.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/LogResult.py` & `ifd_python-10.1.2/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/Malfacon.py` & `ifd_python-10.1.2/ifd/entities/Malfacon.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/OCR.py` & `ifd_python-10.1.2/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/RabbitMqMessage.py` & `ifd_python-10.1.2/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/entities/Tag.py` & `ifd_python-10.1.2/ifd/entities/Tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def deserialize(self, data):
         for field in data:
             if data[field] is None:
                 pass
             elif field == "score":
                 self.score = data[field]
             elif field == "label":
-                self.score = data[field]
+                self.label = data[field]
             elif field == "description":
                 self.description = data[field]
             elif field == "modele":
                 self.modele = Modele().deserialize(data[field])
             elif field == "isMalfacon":
                 self.isMalfacon = data[field]
         return self
```

### Comparing `ifd_python-10.1.1/ifd/entities/bbox.py` & `ifd_python-10.1.2/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/repository/AmqpImageRepository.py` & `ifd_python-10.1.2/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/repository/RestTicketRepository.py` & `ifd_python-10.1.2/ifd/repository/RestTicketRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/repository/SqlLogRepository.py` & `ifd_python-10.1.2/ifd/repository/SqlLogRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/repository/SqlTicketRepository.py` & `ifd_python-10.1.2/ifd/repository/SqlTicketRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/repository/abstract/AbsSqlRepository.py` & `ifd_python-10.1.2/ifd/repository/abstract/AbsSqlRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/spec.py` & `ifd_python-10.1.2/ifd/spec.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/ifd/tools.py` & `ifd_python-10.1.2/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.1/PKG-INFO` & `ifd_python-10.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 10.1.1
+Version: 10.1.2
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

