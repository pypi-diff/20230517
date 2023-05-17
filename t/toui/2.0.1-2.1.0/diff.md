# Comparing `tmp/toui-2.0.1.tar.gz` & `tmp/toui-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-2.0.1.tar", last modified: Mon May 15 13:29:41 2023, max compression
+gzip compressed data, was "toui-2.1.0.tar", last modified: Wed May 17 05:44:24 2023, max compression
```

## Comparing `toui-2.0.1.tar` & `toui-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 13:29:41.044025 toui-2.0.1/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.0.1/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2994 2023-05-15 13:29:41.043010 toui-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 13:29:40.971705 toui-2.0.1/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.0.1/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.0.1/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.0.1/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.0.1/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.0.1/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.0.1/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.0.1/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.0.1/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.0.1/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:29:40.976830 toui-2.0.1/images/
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.0.1/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-05-15 13:29:41.044025 toui-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1517 2023-05-15 13:28:32.000000 toui-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:29:41.030373 toui-2.0.1/toui/
--rw-rw-rw-   0        0        0      234 2023-05-15 13:12:50.000000 toui-2.0.1/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.0.1/toui/_defaults.py
--rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.0.1/toui/_helpers.py
--rw-rw-rw-   0        0        0     9902 2023-05-15 13:04:45.000000 toui-2.0.1/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.0.1/toui/_signals.py
--rw-rw-rw-   0        0        0    26536 2023-05-15 13:04:45.000000 toui-2.0.1/toui/apps.py
--rw-rw-rw-   0        0        0    20537 2023-05-15 13:04:45.000000 toui-2.0.1/toui/elements.py
--rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.0.1/toui/exceptions.py
--rw-rw-rw-   0        0        0    17082 2023-05-15 13:04:45.000000 toui-2.0.1/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.0.1/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:29:41.042006 toui-2.0.1/toui.egg-info/
--rw-rw-rw-   0        0        0     2994 2023-05-15 13:29:40.000000 toui-2.0.1/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-15 13:29:40.000000 toui-2.0.1/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 13:29:40.000000 toui-2.0.1/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2023-05-15 13:29:40.000000 toui-2.0.1/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 13:29:40.000000 toui-2.0.1/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 05:44:24.461710 toui-2.1.0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2994 2023-05-17 05:44:24.460711 toui-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 05:44:24.343140 toui-2.1.0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.1.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.1.0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.1.0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.1.0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.1.0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.1.0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.1.0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.1.0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.1.0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:44:24.349137 toui-2.1.0/images/
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.1.0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-05-17 05:44:24.461710 toui-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1517 2023-05-15 13:28:32.000000 toui-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:44:24.449709 toui-2.1.0/toui/
+-rw-rw-rw-   0        0        0      266 2023-05-17 05:43:30.000000 toui-2.1.0/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.1.0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.1.0/toui/_helpers.py
+-rw-rw-rw-   0        0        0     9902 2023-05-15 13:04:45.000000 toui-2.1.0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.1.0/toui/_signals.py
+-rw-rw-rw-   0        0        0    27251 2023-05-17 05:39:09.000000 toui-2.1.0/toui/apps.py
+-rw-rw-rw-   0        0        0    20537 2023-05-15 13:04:45.000000 toui-2.1.0/toui/elements.py
+-rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.1.0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    17082 2023-05-15 13:04:45.000000 toui-2.1.0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.1.0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-17 05:44:24.459710 toui-2.1.0/toui.egg-info/
+-rw-rw-rw-   0        0        0     2994 2023-05-17 05:44:24.000000 toui-2.1.0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-17 05:44:24.000000 toui-2.1.0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 05:44:24.000000 toui-2.1.0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2023-05-17 05:44:24.000000 toui-2.1.0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-17 05:44:24.000000 toui-2.1.0/toui.egg-info/top_level.txt
```

### Comparing `toui-2.0.1/LICENSE` & `toui-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/PKG-INFO` & `toui-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.0.1
+Version: 2.1.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.0.1/README.md` & `toui-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/examples/advanced_example_1_toui_blueprint.py` & `toui-2.1.0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/examples/example_1_simple_website.py` & `toui-2.1.0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/examples/example_2_simple_desktop_app.py` & `toui-2.1.0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/examples/example_3_updating_page.py` & `toui-2.1.0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/examples/example_4_function_with_arg.py` & `toui-2.1.0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/examples/example_5_user_variables.py` & `toui-2.1.0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/images/logo.png` & `toui-2.1.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/setup.py` & `toui-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/toui/_helpers.py` & `toui-2.1.0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/toui/_javascript_templates.py` & `toui-2.1.0/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/toui/_signals.py` & `toui-2.1.0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/toui/apps.py` & `toui-2.1.0/toui/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -821,11 +821,44 @@
     """
     app = DesktopApp(name=name, assets_folder=assets_folder, secret_key=secret_key)
     page = Page(url=url, html_file=html_file, html_str=html_str)
     app.add_pages(page)
     return app
 
 
+def set_global_app(app):
+    """
+    Allows the app object to be shared across Python modules.
+
+    Examples
+    --------
+
+    Suppose you have two Python scripts, "main.py" and "home_page.py". In "main.py", you can create the app
+    and make it global:
+
+    >>> from toui import Website, set_global_app
+    >>> app = Website(__name__)
+    >>> set_global_app(app)
+
+    While in "home_page.py", you can get the shared app:
+
+    >>> from toui import get_global_app
+    >>> app = get_global_app()
+
+    """
+    global _global_app
+    _global_app = app
+
+
+def get_global_app():
+    """
+    Gets the shared app object.
+
+    See :py:meth:`set_global_app`.
+    """
+    return _global_app
+
+
 if __name__ == "__main__":
     import doctest
     results = doctest.testmod()
     print(results)
```

### Comparing `toui-2.0.1/toui/elements.py` & `toui-2.1.0/toui/elements.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/toui/pages.py` & `toui-2.1.0/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/toui/structure.py` & `toui-2.1.0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-2.0.1/toui.egg-info/PKG-INFO` & `toui-2.1.0/toui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.0.1
+Version: 2.1.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.0.1/toui.egg-info/SOURCES.txt` & `toui-2.1.0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

