# Comparing `tmp/mrfix-1.0.5.tar.gz` & `tmp/mrfix-1.0.6.tar.gz`

## Comparing `mrfix-1.0.5.tar` & `mrfix-1.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.5/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.5/src/mrfix/__init__.py
--rw-r--r--   0        0        0    14011 2020-02-02 00:00:00.000000 mrfix-1.0.5/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.5/.gitignore
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.5/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.6/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.6/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 mrfix-1.0.6/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.6/.gitignore
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.6/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.6/PKG-INFO
```

### Comparing `mrfix-1.0.5/LICENZE` & `mrfix-1.0.6/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.5/src/mrfix/mrfix.py` & `mrfix-1.0.6/src/mrfix/mrfix.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from selenium.webdriver.support import expected_conditions as EC
 import selenium.webdriver.support.ui as ui
 
 
 
 class MrFixUI :
 
+    def __init__(self, browser):
+        self.browser = browser
+
     def assertElementsIsPresentByXpatch(self, xpath_elements):
         try:
             elements = self.find_elements(By.XPATH, xpath_elements)
             return [True, len(elements)]
         except NoSuchElementException:
             return [False, 0]
```

### Comparing `mrfix-1.0.5/.gitignore` & `mrfix-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.5/README.md` & `mrfix-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.5/pyproject.toml` & `mrfix-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "1.0.5"
+version = "1.0.6"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mrfix-1.0.5/PKG-INFO` & `mrfix-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfix
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

