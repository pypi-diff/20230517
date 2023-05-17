# Comparing `tmp/AISAPLibrary-1.0.6.tar.gz` & `tmp/AISAPLibrary-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-1bms58zz\AISAPLibrary-1.0.6.tar", last modified: Tue May 16 04:33:01 2023, max compression
+gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-wkgjr4ff\AISAPLibrary-1.0.7.tar", last modified: Tue May 16 09:41:22 2023, max compression
```

## Comparing `AISAPLibrary-1.0.6.tar` & `AISAPLibrary-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/
--rw-rw-rw-   0        0        0      310 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.6/README.md
--rw-rw-rw-   0        0        0      482 2023-05-16 04:32:41.000000 AISAPLibrary-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary/
--rw-rw-rw-   0        0        0    50334 2023-05-16 04:30:54.000000 AISAPLibrary-1.0.6/src/AISAPLibrary/AISAPLibrary.py
--rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.6/src/AISAPLibrary/__init__.py
--rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.6/src/AISAPLibrary/send_vkey_multithread.py
-drwxrwxrwx   0        0        0        0 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/
--rw-rw-rw-   0        0        0      310 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/
+-rw-rw-rw-   0        0        0      310 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.7/README.md
+-rw-rw-rw-   0        0        0      482 2023-05-16 09:40:24.000000 AISAPLibrary-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary/
+-rw-rw-rw-   0        0        0    54172 2023-05-16 09:39:48.000000 AISAPLibrary-1.0.7/src/AISAPLibrary/AISAPLibrary.py
+-rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.7/src/AISAPLibrary/__init__.py
+-rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.7/src/AISAPLibrary/send_vkey_multithread.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-16 09:41:22.000000 AISAPLibrary-1.0.7/src/AISAPLibrary.egg-info/top_level.txt
```

### Comparing `AISAPLibrary-1.0.6/src/AISAPLibrary/AISAPLibrary.py` & `AISAPLibrary-1.0.7/src/AISAPLibrary/AISAPLibrary.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,83 @@
         if self.connection.Description == connection_name:
             self.session = self.connection.children(0)
         else:
             self.take_screenshot()
             message = "No existing connection for '%s' found." % connection_name
             raise ValueError(message)
         
+    def get_value_other_session(self, element_id, session_num='1'):
+        element_type = self.get_element_type_other_session(element_id,session_num=session_num)
+        return_value = ""
+        if (element_type == "GuiTextField"
+                or element_type == "GuiCTextField"
+                or element_type == "GuiLabel"
+                or element_type == "GuiTitlebar"
+                or element_type == "GuiStatusbar"
+                or element_type == "GuiButton"
+                or element_type == "GuiTab"
+                or element_type == "GuiShell"):
+            self.set_focus_other_session(element_id,session_num=session_num)
+            return_value = self.connection.children(int(session_num)).findById(element_id).text
+        elif element_type == "GuiStatusPane":
+            return_value = self.connection.children(int(session_num)).findById(element_id).text
+        elif (element_type == "GuiCheckBox"
+              or element_type == "GuiRadioButton"):
+            actual_value = self.connection.children(int(session_num)).findById(element_id).selected
+            # In these situations we return check / unchecked, so we change these values here
+            if actual_value == True:
+                return_value = "checked"
+            elif actual_value == False:
+                return_value = "unchecked"
+        elif element_type == "GuiComboBox":
+            return_value = self.connection.children(int(session_num)).findById(element_id).text
+            # In comboboxes there are many spaces after the value. In order to check the value, we strip them away.
+            return_value = return_value.strip()
+        else:
+            # If we can't return the value for this element type, raise an assertion error
+            self.take_screenshot()
+            message = "Cannot get value for element type '%s'" % element_type
+            raise Warning(message)
+        return return_value
+        
+    def element_value_should_contain_other_session(self, element_id, expected_value, message=None, session_num='1'):
+        element_type = self.get_element_type_other_session(element_id,session_num=session_num)
+
+        # Breaking up the different element types so we can check the value the correct way
+        if (element_type == "GuiTextField"
+                or element_type == "GuiCTextField"
+                or element_type == "GuiComboBox"
+                or element_type == "GuiLabel"):
+            self.connection.children(int(session_num)).findById(element_id).setfocus()
+            actual_value = self.get_value_other_session(element_id, session_num=session_num)
+            time.sleep(self.explicit_wait)
+            # In these cases we can simply check the text value against the value of the element
+            if expected_value not in actual_value:
+                self.take_screenshot()
+                if message is None:
+                    message = "Element value '%s' does not contain '%s', (but was '%s')" % (
+                        element_id, expected_value, actual_value)
+                raise AssertionError(message)
+        else:
+            # When the element content can't be checked, raise an assertion error
+            self.take_screenshot()
+            message = "Cannot use keyword 'element value should contain' for element type '%s'" % element_type
+            raise Warning(message)
+        # Run explicit wait as last
+        time.sleep(self.explicit_wait)
+        
+    def set_focus_other_session(self, element_id, session_num='1'):
+
+        """Sets the focus to the given element.
+        """
+        element_type = self.get_element_type_other_session(element_id,session_num=session_num)
+        if element_type != "GuiStatusPane":
+            self.connection.children(int(session_num)).findById(element_id).setFocus()
+        time.sleep(self.explicit_wait)
+        
     def doubleclick_element_other_session(self, element_id, item_id, column_id, session_num='1'):
         """Performs a double-click on a given element. Used only for shell objects.
         """
 
         # Performing the correct method on an element, depending on the type of element
         element_type = self.get_element_type_other_session(element_id,session_num=session_num)
         if element_type == "GuiShell":
```

