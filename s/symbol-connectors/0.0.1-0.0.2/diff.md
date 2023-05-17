# Comparing `tmp/symbol-connectors-0.0.1.tar.gz` & `tmp/symbol_connectors-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol-connectors-0.0.1.tar", max compression
+gzip compressed data, was "symbol_connectors-0.0.2.tar", max compression
```

## Comparing `symbol-connectors-0.0.1.tar` & `symbol_connectors-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      193 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/README.md
--rw-r--r--   0        0        0      600 2023-05-16 17:59:52.986607 symbol-connectors-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/__init__.py
--rw-r--r--   0        0        0       10 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/bindings/.gitignore
--rw-r--r--   0        0        0        0 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/bindings/__init__.py
--rw-r--r--   0        0        0      241 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/bindings/openssl.py
--rw-r--r--   0        0        0     1113 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/connector/BasicConnector.py
--rw-r--r--   0        0        0     2413 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/connector/CatapultCertificateProcessor.py
--rw-r--r--   0        0        0     2028 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/connector/CertificateUtils.py
--rw-r--r--   0        0        0     2883 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/connector/NemConnector.py
--rw-r--r--   0        0        0     2831 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/connector/SymbolConnector.py
--rw-r--r--   0        0        0     5381 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/connector/SymbolPeerConnector.py
--rw-r--r--   0        0        0        0 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/connector/__init__.py
--rw-r--r--   0        0        0      563 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/model/Endpoint.py
--rw-r--r--   0        0        0      218 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/model/Exceptions.py
--rw-r--r--   0        0        0     2036 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/model/NodeInfo.py
--rw-r--r--   0        0        0     1465 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/model/PacketHeader.py
--rw-r--r--   0        0        0        0 2023-05-16 17:34:28.649624 symbol-connectors-0.0.1/symbolconnectors/model/__init__.py
--rw-r--r--   0        0        0     1050 2023-05-16 17:59:58.579709 symbol-connectors-0.0.1/setup.py
--rw-r--r--   0        0        0     1116 2023-05-16 17:59:58.579992 symbol-connectors-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/README.md
+-rw-r--r--   0        0        0      600 2023-05-17 18:17:54.210442 symbol_connectors-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/__init__.py
+-rw-r--r--   0        0        0       10 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/bindings/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/bindings/__init__.py
+-rw-r--r--   0        0        0      241 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/bindings/openssl.py
+-rw-r--r--   0        0        0     1113 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/connector/BasicConnector.py
+-rw-r--r--   0        0        0     2413 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/connector/CatapultCertificateProcessor.py
+-rw-r--r--   0        0        0     2028 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/connector/CertificateUtils.py
+-rw-r--r--   0        0        0     2883 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/connector/NemConnector.py
+-rw-r--r--   0        0        0     4377 2023-05-17 17:14:55.938684 symbol_connectors-0.0.2/symbolconnectors/connector/SymbolConnector.py
+-rw-r--r--   0        0        0     5381 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/connector/SymbolPeerConnector.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/connector/__init__.py
+-rw-r--r--   0        0        0      563 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/model/Endpoint.py
+-rw-r--r--   0        0        0      218 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/model/Exceptions.py
+-rw-r--r--   0        0        0     2036 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/model/NodeInfo.py
+-rw-r--r--   0        0        0     1465 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/model/PacketHeader.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:54:00.109828 symbol_connectors-0.0.2/symbolconnectors/model/__init__.py
+-rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 symbol_connectors-0.0.2/PKG-INFO
```

### Comparing `symbol-connectors-0.0.1/pyproject.toml` & `symbol_connectors-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'symbol-connectors'
-version = '0.0.1'
+version = '0.0.2'
 description = 'Symbol Connectors'
 authors = ['Symbol Contributors <contributors@symbol.dev>']
 maintainers = ['Symbol Contributors <contributors@symbol.dev>']
 license = 'MIT'
 
 readme = 'README.md'
```

### Comparing `symbol-connectors-0.0.1/symbolconnectors/connector/BasicConnector.py` & `symbol_connectors-0.0.2/symbolconnectors/connector/BasicConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-connectors-0.0.1/symbolconnectors/connector/CatapultCertificateProcessor.py` & `symbol_connectors-0.0.2/symbolconnectors/connector/CatapultCertificateProcessor.py`

 * *Files identical despite different names*

### Comparing `symbol-connectors-0.0.1/symbolconnectors/connector/CertificateUtils.py` & `symbol_connectors-0.0.2/symbolconnectors/connector/CertificateUtils.py`

 * *Files identical despite different names*

### Comparing `symbol-connectors-0.0.1/symbolconnectors/connector/NemConnector.py` & `symbol_connectors-0.0.2/symbolconnectors/connector/NemConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-connectors-0.0.1/symbolconnectors/connector/SymbolPeerConnector.py` & `symbol_connectors-0.0.2/symbolconnectors/connector/SymbolPeerConnector.py`

 * *Files identical despite different names*

### Comparing `symbol-connectors-0.0.1/symbolconnectors/model/Endpoint.py` & `symbol_connectors-0.0.2/symbolconnectors/model/Endpoint.py`

 * *Files identical despite different names*

### Comparing `symbol-connectors-0.0.1/symbolconnectors/model/NodeInfo.py` & `symbol_connectors-0.0.2/symbolconnectors/model/NodeInfo.py`

 * *Files identical despite different names*

### Comparing `symbol-connectors-0.0.1/symbolconnectors/model/PacketHeader.py` & `symbol_connectors-0.0.2/symbolconnectors/model/PacketHeader.py`

 * *Files identical despite different names*

### Comparing `symbol-connectors-0.0.1/PKG-INFO` & `symbol_connectors-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: symbol-connectors
-Version: 0.0.1
+Version: 0.0.2
 Summary: Symbol Connectors
 Home-page: https://github.com/symbol/product/tree/main/python/connectors
 License: MIT
 Keywords: symbol,connectors,Symbol Connectors
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 Maintainer: Symbol Contributors
 Maintainer-email: contributors@symbol.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: aiohttp (==3.8.4)
 Requires-Dist: symbol-sdk-python (==3.0.7)
 Requires-Dist: zenlog (==1.1)
 Project-URL: Repository, https://github.com/symbol/product/tree/main/python/connectors
 Description-Content-Type: text/markdown
 
 # Python Connectors
```

