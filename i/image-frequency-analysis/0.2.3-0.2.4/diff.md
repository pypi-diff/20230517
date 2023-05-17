# Comparing `tmp/image_frequency_analysis-0.2.3.tar.gz` & `tmp/image_frequency_analysis-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_frequency_analysis-0.2.3.tar", last modified: Sun May 14 14:03:07 2023, max compression
+gzip compressed data, was "image_frequency_analysis-0.2.4.tar", last modified: Wed May 17 14:15:40 2023, max compression
```

## Comparing `image_frequency_analysis-0.2.3.tar` & `image_frequency_analysis-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:03:07.171125 image_frequency_analysis-0.2.3/
--rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     1495 2023-05-14 14:03:07.170125 image_frequency_analysis-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1209 2023-05-14 13:59:53.000000 image_frequency_analysis-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 14:03:07.161119 image_frequency_analysis-0.2.3/image_frequency_analysis/
--rw-rw-rw-   0        0        0       92 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.3/image_frequency_analysis/__init__.py
--rw-rw-rw-   0        0        0     6507 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.3/image_frequency_analysis/frequency_analysis.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:03:07.169125 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/
--rw-rw-rw-   0        0        0     1495 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 14:03:07.171125 image_frequency_analysis-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      562 2023-05-14 14:00:38.000000 image_frequency_analysis-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:15:40.196978 image_frequency_analysis-0.2.4/
+-rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     1495 2023-05-17 14:15:40.195845 image_frequency_analysis-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1209 2023-05-17 14:11:55.000000 image_frequency_analysis-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 14:15:40.174733 image_frequency_analysis-0.2.4/image_frequency_analysis/
+-rw-rw-rw-   0        0        0       92 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.4/image_frequency_analysis/__init__.py
+-rw-rw-rw-   0        0        0     6520 2023-05-17 14:13:41.000000 image_frequency_analysis-0.2.4/image_frequency_analysis/frequency_analysis.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:15:40.191848 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/
+-rw-rw-rw-   0        0        0     1495 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 14:15:40.198003 image_frequency_analysis-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      562 2023-05-17 14:13:41.000000 image_frequency_analysis-0.2.4/setup.py
```

### Comparing `image_frequency_analysis-0.2.3/LICENSE` & `image_frequency_analysis-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.2.3/PKG-INFO` & `image_frequency_analysis-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_frequency_analysis
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package to perform image frequency analysis using the Fourier Transform method
 Author: M Thivagar
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `image_frequency_analysis-0.2.3/README.md` & `image_frequency_analysis-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.2.3/image_frequency_analysis/frequency_analysis.py` & `image_frequency_analysis-0.2.4/image_frequency_analysis/frequency_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         )
 
     def plot_graph(self, frequency_shift_magnitude, image):
         plt.figure(figsize=(20, 10))
 
         plt.subplot(1, 3, 1)
         plt.title("Original Image")
-        plt.imshow(self.image)
+        plt.imshow(self.image, cmap="gray")
 
         plt.subplot(1, 3, 2)
         plt.title("Frequency Shifted Mask")
         plt.imshow(frequency_shift_magnitude, cmap="gray")
 
         plt.subplot(1, 3, 3)
         filter_type = "Low Pass filter" if self.low_pass_filter else "High Pass Filter"
```

### Comparing `image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/PKG-INFO` & `image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-frequency-analysis
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package to perform image frequency analysis using the Fourier Transform method
 Author: M Thivagar
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `image_frequency_analysis-0.2.3/setup.py` & `image_frequency_analysis-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="image_frequency_analysis",
-    version="0.2.3",
+    version="0.2.4",
     author="M Thivagar",
     packages=find_packages(),
     install_requires=["opencv-python", "numpy", "pandas", "matplotlib"],
     python_requires=">=3.6",
     description="A package to perform image frequency analysis using the Fourier Transform method",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

