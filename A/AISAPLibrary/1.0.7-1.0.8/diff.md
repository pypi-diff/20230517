# Comparing `tmp/AISAPLibrary-1.0.7.tar.gz` & `tmp/AISAPLibrary-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-wkgjr4ff\AISAPLibrary-1.0.7.tar", last modified: Tue May 16 09:41:22 2023, max compression
+gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-8cy6s965\AISAPLibrary-1.0.8.tar", last modified: Wed May 17 01:44:51 2023, max compression
```

## Comparing `AISAPLibrary-1.0.7.tar` & `AISAPLibrary-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/
--rw-rw-rw-   0        0        0      310 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.7/README.md
--rw-rw-rw-   0        0        0      482 2023-05-16 09:40:24.000000 AISAPLibrary-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary/
--rw-rw-rw-   0        0        0    54172 2023-05-16 09:39:48.000000 AISAPLibrary-1.0.7/src/AISAPLibrary/AISAPLibrary.py
--rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.7/src/AISAPLibrary/__init__.py
--rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.7/src/AISAPLibrary/send_vkey_multithread.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/
--rw-rw-rw-   0        0        0      310 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/
+-rw-rw-rw-   0        0        0      310 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.8/README.md
+-rw-rw-rw-   0        0        0      482 2023-05-17 01:42:12.000000 AISAPLibrary-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary/
+-rw-rw-rw-   0        0        0    54413 2023-05-17 01:40:53.000000 AISAPLibrary-1.0.8/src/AISAPLibrary/AISAPLibrary.py
+-rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.8/src/AISAPLibrary/__init__.py
+-rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.8/src/AISAPLibrary/send_vkey_multithread.py
+drwxrwxrwx   0        0        0        0 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/top_level.txt
```

### Comparing `AISAPLibrary-1.0.7/src/AISAPLibrary/AISAPLibrary.py` & `AISAPLibrary-1.0.8/src/AISAPLibrary/AISAPLibrary.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,20 @@
         if self.connection.Description == connection_name:
             self.session = self.connection.children(0)
         else:
             self.take_screenshot()
             message = "No existing connection for '%s' found." % connection_name
             raise ValueError(message)
         
+    def check_busy_other_session(self,session_num='1'):
+        '''Function to check if session is busy or nots'''
+        while True :
+            if self.connection.children(int(session_num)).busy == False :
+                break
+        
     def get_value_other_session(self, element_id, session_num='1'):
         element_type = self.get_element_type_other_session(element_id,session_num=session_num)
         return_value = ""
         if (element_type == "GuiTextField"
                 or element_type == "GuiCTextField"
                 or element_type == "GuiLabel"
                 or element_type == "GuiTitlebar"
```

