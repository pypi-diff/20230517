# Comparing `tmp/sspqdd-1.0.3.tar.gz` & `tmp/sspqdd-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspqdd-1.0.3.tar", last modified: Wed May 17 15:08:01 2023, max compression
+gzip compressed data, was "sspqdd-1.0.4.tar", last modified: Wed May 17 15:09:43 2023, max compression
```

## Comparing `sspqdd-1.0.3.tar` & `sspqdd-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:01.097679 sspqdd-1.0.3/
--rw-rw-rw-   0        0        0     1120 2023-05-17 15:08:01.096671 sspqdd-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6293 2023-04-14 13:52:05.000000 sspqdd-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 15:08:01.097679 sspqdd-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2459 2023-05-17 15:07:54.000000 sspqdd-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:01.084097 sspqdd-1.0.3/sspqdd/
--rw-rw-rw-   0        0        0        0 2023-05-17 10:19:04.000000 sspqdd-1.0.3/sspqdd/__init__.py
--rw-rw-rw-   0        0        0     3809 2023-05-17 11:25:56.000000 sspqdd-1.0.3/sspqdd/sspqdd_pkg.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:01.094217 sspqdd-1.0.3/sspqdd.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-05-17 15:08:00.000000 sspqdd-1.0.3/sspqdd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-17 15:08:01.000000 sspqdd-1.0.3/sspqdd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 15:08:00.000000 sspqdd-1.0.3/sspqdd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 15:08:00.000000 sspqdd-1.0.3/sspqdd.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 15:09:43.691419 sspqdd-1.0.4/
+-rw-rw-rw-   0        0        0     1290 2023-05-17 15:09:43.691419 sspqdd-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6293 2023-04-14 13:52:05.000000 sspqdd-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 15:09:43.691419 sspqdd-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2483 2023-05-17 15:09:35.000000 sspqdd-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:09:43.677083 sspqdd-1.0.4/sspqdd/
+-rw-rw-rw-   0        0        0        0 2023-05-17 10:19:04.000000 sspqdd-1.0.4/sspqdd/__init__.py
+-rw-rw-rw-   0        0        0     3809 2023-05-17 11:25:56.000000 sspqdd-1.0.4/sspqdd/sspqdd_pkg.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:09:43.688150 sspqdd-1.0.4/sspqdd.egg-info/
+-rw-rw-rw-   0        0        0     1290 2023-05-17 15:09:43.000000 sspqdd-1.0.4/sspqdd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-17 15:09:43.000000 sspqdd-1.0.4/sspqdd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:09:43.000000 sspqdd-1.0.4/sspqdd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 15:09:43.000000 sspqdd-1.0.4/sspqdd.egg-info/top_level.txt
```

### Comparing `sspqdd-1.0.3/PKG-INFO` & `sspqdd-1.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sspqdd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Single-Shot-Power-Quality-Disturbance-Detector
 Home-page: UNKNOWN
 Author: Carlos Iturrino-García
 Author-email: carlos.iturrino.garcia@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 
 Single-Shot-Power-Quality-Disturbance-Detector (SSPQDD) is a Python package that provides a comprehensive solution for detection and classification of power quality disturbances. It utilizes state-of-the-art deep learning algorithms to analyze power signals and identify various types of disturbances, such as voltagesags, swells, harmonics, transients, notch and interruptions. The SSPQDD is designed to empower engineers and researchers working in the field of power quality analysis. By leveraging deep learning techniques, it offers an efficient and accurate approach to automatically detect and classify power disturbances, saving time and effort compared to manual inspection. With the SSPQDD, users can gain valuable insights into power quality issues and make informed decisions for optimal system performance and reliability. 
- Features:
- - Detection and 
+ Features: 
+ - Detection and classification of power quality disturbances: SSPQDD provides an extensive library of pre-trained deep learning models capable of identifying various power disturbances
```

### Comparing `sspqdd-1.0.3/README.md` & `sspqdd-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sspqdd-1.0.3/setup.py` & `sspqdd-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup
 
 setup(
     name="sspqdd",
-    version="1.0.3",
+    version="1.0.4",
     description="Single-Shot-Power-Quality-Disturbance-Detector",
     author="Carlos Iturrino-García",
     author_email="carlos.iturrino.garcia@gmail.com",
     packages=["sspqdd"],
     long_description = "Single-Shot-Power-Quality-Disturbance-Detector (SSPQDD) is a Python package that provides a "
                        "comprehensive solution for detection and"
                        " classification of power quality disturbances. It utilizes state-of-the-art deep learning "
                        "algorithms to analyze power signals and identify various types of disturbances, such as voltage"
                        "sags, swells, harmonics, transients, notch and interruptions. The SSPQDD is designed to empower"
                        " engineers and researchers working in the field of power quality analysis. By leveraging "
                        "deep learning techniques, it offers an efficient and accurate approach to automatically detect "
                        "and classify power disturbances, saving time and effort compared to manual inspection. "
                        "With the SSPQDD, users can gain valuable insights into power quality issues and make informed "
-                       "decisions for optimal system performance and reliability. \n Features:\n - Detection and ",
-                       # "classification of power quality disturbances: SSPQDD provides an extensive library of "
-                       # "pre-trained deep learning models capable of identifying various power disturbances "
+                       "decisions for optimal system performance and reliability. \n Features: \n "
+                       "- Detection and "
+                       "classification of power quality disturbances: SSPQDD provides an extensive library of "
+                       "pre-trained deep learning models capable of identifying various power disturbances ",
                        # "with high precision. \n - Real-time monitoring: It enables real-time analysis of power signals,"
                        # "allowing for immediate detection and notification of disturbances as they occur.\n "
                        # "-Customizability: Users have the flexibility to fine-tune or retrain the models with their "
                        # "own datasets to cater to specific power quality analysis requirements. \n"
                        # "-Visualization and reporting: PowerQDetect offers interactive visualization "
                        # "tools and comprehensive reporting capabilities to help users interpret the detected disturbances "
                        # "and generate detailed reports.",
```

### Comparing `sspqdd-1.0.3/sspqdd/sspqdd_pkg.py` & `sspqdd-1.0.4/sspqdd/sspqdd_pkg.py`

 * *Files identical despite different names*

### Comparing `sspqdd-1.0.3/sspqdd.egg-info/PKG-INFO` & `sspqdd-1.0.4/sspqdd.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sspqdd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Single-Shot-Power-Quality-Disturbance-Detector
 Home-page: UNKNOWN
 Author: Carlos Iturrino-García
 Author-email: carlos.iturrino.garcia@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 
 Single-Shot-Power-Quality-Disturbance-Detector (SSPQDD) is a Python package that provides a comprehensive solution for detection and classification of power quality disturbances. It utilizes state-of-the-art deep learning algorithms to analyze power signals and identify various types of disturbances, such as voltagesags, swells, harmonics, transients, notch and interruptions. The SSPQDD is designed to empower engineers and researchers working in the field of power quality analysis. By leveraging deep learning techniques, it offers an efficient and accurate approach to automatically detect and classify power disturbances, saving time and effort compared to manual inspection. With the SSPQDD, users can gain valuable insights into power quality issues and make informed decisions for optimal system performance and reliability. 
- Features:
- - Detection and 
+ Features: 
+ - Detection and classification of power quality disturbances: SSPQDD provides an extensive library of pre-trained deep learning models capable of identifying various power disturbances
```

