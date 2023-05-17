# Comparing `tmp/Fletxible-0.4.2.tar.gz` & `tmp/Fletxible-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.4.2.tar", last modified: Mon May 15 13:41:39 2023, max compression
+gzip compressed data, was "Fletxible-0.5.0.tar", last modified: Wed May 17 16:18:12 2023, max compression
```

## Comparing `Fletxible-0.4.2.tar` & `Fletxible-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-15 13:41:39.313826 Fletxible-0.4.2/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-15 13:41:39.311269 Fletxible-0.4.2/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      326 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.4.2/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-15 13:41:39.313624 Fletxible-0.4.2/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.4.2/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-15 13:41:39.312741 Fletxible-0.4.2/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.4.2/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2168 2023-05-13 13:50:26.000000 Fletxible-0.4.2/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)      312 2023-05-14 11:02:33.000000 Fletxible-0.4.2/logic/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6485 2023-05-13 15:17:29.000000 Fletxible-0.4.2/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2304 2023-05-14 20:20:25.000000 Fletxible-0.4.2/logic/utilities.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-15 13:41:39.313898 Fletxible-0.4.2/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1110 2023-05-15 13:41:13.000000 Fletxible-0.4.2/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-15 13:41:39.313200 Fletxible-0.4.2/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.4.2/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-17 16:18:12.601059 Fletxible-0.5.0/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-17 16:18:12.597604 Fletxible-0.5.0/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      360 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-17 16:18:12.000000 Fletxible-0.5.0/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.0/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-17 16:18:12.600829 Fletxible-0.5.0/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.0/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-17 16:18:12.599946 Fletxible-0.5.0/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.5.0/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2251 2023-05-17 15:53:13.000000 Fletxible-0.5.0/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     7170 2023-05-17 15:50:13.000000 Fletxible-0.5.0/logic/controls.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      868 2023-05-17 15:48:21.000000 Fletxible-0.5.0/logic/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6505 2023-05-16 19:07:50.000000 Fletxible-0.5.0/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-05-17 15:50:39.000000 Fletxible-0.5.0/logic/styles.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4736 2023-05-17 15:57:08.000000 Fletxible-0.5.0/logic/utilities.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-17 16:18:12.601127 Fletxible-0.5.0/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1110 2023-05-17 16:17:33.000000 Fletxible-0.5.0/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-17 16:18:12.600378 Fletxible-0.5.0/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.0/tests/test_route.py
```

### Comparing `Fletxible-0.4.2/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.5.0/Fletxible.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.4.2
+Version: 0.5.0
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.4.2/LICENSE` & `Fletxible-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.4.2/PKG-INFO` & `Fletxible-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.4.2
+Version: 0.5.0
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.4.2/README.md` & `Fletxible-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.4.2/logic/cli.py` & `Fletxible-0.5.0/logic/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,15 +38,22 @@
         string = set_up_yaml_file()
         f.write(string)
 
     # Create 'logic' directory if it doesn't exist
     Path("logic").mkdir(exist_ok=True)
 
     # Define the list of files to be generated
-    file_list = ["__init__.py", "main.py", "script.py", "utilities.py"]
+    file_list = [
+        "__init__.py",
+        "main.py",
+        "script.py",
+        "utilities.py",
+        "styles.py",
+        "controls.py",
+    ]
 
     # Generate each file in the templates directory
     for file_name in file_list:
         file_path = Path("logic") / file_name
         file_path.touch()
 
         # Read the contents of the source file
```

### Comparing `Fletxible-0.4.2/logic/script.py` & `Fletxible-0.5.0/logic/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     set_app_route_method,
     set_app_default_pages,
     navigation_example_method,
 )
 
 #
 route_keys: dict = {}
+control_keys: list = []
 
 
 def open_yaml_script() -> dict:
     # Load the YAML file
     with open("flet_config.yml", "r") as file:
         docs = yaml.safe_load(file)
 
@@ -194,15 +195,15 @@
 
     # Next, we have to handle the page logic, which requires
     # several step. First, adding the default method into each page
     try:
         route_keys: dict = set_default_methods_script(docs)
 
         for keys, __ in route_keys.items():
-            page.views.append(route_keys[keys].loader.load_module().pageView())
+            page.views.append(route_keys[keys].loader.load_module().View())
 
         page.go("/index")
 
     except Exception as e:
         print(e)
 
     # Map out the .yml file into a python dict
```

### Comparing `Fletxible-0.4.2/setup.py` & `Fletxible-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.4.2",
+    version="0.5.0",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=["logic"],
-    install_requires=["click>=8.1.3", "flet>=0.6.2", "PyYAML>=6.0"],
+    install_requires=["click>=8.1.3", "flet>=0.7.1", "PyYAML>=6.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": ["fletxible-init=logic.cli:init"],
```

