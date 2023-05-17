# Comparing `tmp/rfmanalysis-0.1.6.tar.gz` & `tmp/rfmanalysis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfmanalysis-0.1.6.tar", last modified: Tue May 16 22:22:23 2023, max compression
+gzip compressed data, was "rfmanalysis-0.2.0.tar", last modified: Wed May 17 00:11:58 2023, max compression
```

## Comparing `rfmanalysis-0.1.6.tar` & `rfmanalysis-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:22:23.126325 rfmanalysis-0.1.6/
--rw-rw-rw-   0        0        0      184 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3690 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/HISTORY.rst
--rw-rw-rw-   0        0        0     1098 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5269 2023-05-16 22:22:23.126496 rfmanalysis-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4105 2023-05-16 18:42:22.000000 rfmanalysis-0.1.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 22:22:23.083829 rfmanalysis-0.1.6/docs/
--rw-rw-rw-   0        0        0      632 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/authors.rst
--rw-rw-rw-   0        0        0     5007 2023-05-16 21:26:34.000000 rfmanalysis-0.1.6/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/history.rst
--rw-rw-rw-   0        0        0      331 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/index.rst
--rw-rw-rw-   0        0        0     1206 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/readme.rst
--rw-rw-rw-   0        0        0       87 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 22:22:23.089070 rfmanalysis-0.1.6/rfmanalysis/
--rw-rw-rw-   0        0        0      206 2023-05-16 22:21:45.000000 rfmanalysis-0.1.6/rfmanalysis/__init__.py
--rw-rw-rw-   0        0        0    10559 2023-05-16 16:19:14.000000 rfmanalysis-0.1.6/rfmanalysis/rfmanalysis.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:22:23.118201 rfmanalysis-0.1.6/rfmanalysis.egg-info/
--rw-rw-rw-   0        0        0     5269 2023-05-16 22:22:22.000000 rfmanalysis-0.1.6/rfmanalysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-16 22:22:22.000000 rfmanalysis-0.1.6/rfmanalysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:22:22.000000 rfmanalysis-0.1.6/rfmanalysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 18:47:20.000000 rfmanalysis-0.1.6/rfmanalysis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-05-16 22:22:22.000000 rfmanalysis-0.1.6/rfmanalysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      454 2023-05-16 22:22:23.134770 rfmanalysis-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-16 22:21:59.000000 rfmanalysis-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:22:23.124605 rfmanalysis-0.1.6/tests/
--rw-rw-rw-   0        0        0       42 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0      589 2023-05-16 18:36:44.000000 rfmanalysis-0.1.6/tests/test_rfmanalysis.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:11:58.488520 rfmanalysis-0.2.0/
+-rw-rw-rw-   0        0        0      184 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3690 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1098 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5269 2023-05-17 00:11:58.489523 rfmanalysis-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4105 2023-05-16 18:42:22.000000 rfmanalysis-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 00:11:58.454275 rfmanalysis-0.2.0/docs/
+-rw-rw-rw-   0        0        0      632 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     5007 2023-05-16 21:26:34.000000 rfmanalysis-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/history.rst
+-rw-rw-rw-   0        0        0      331 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1206 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       87 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 00:11:58.461777 rfmanalysis-0.2.0/rfmanalysis/
+-rw-rw-rw-   0        0        0      206 2023-05-17 00:10:19.000000 rfmanalysis-0.2.0/rfmanalysis/__init__.py
+-rw-rw-rw-   0        0        0    11453 2023-05-17 00:08:36.000000 rfmanalysis-0.2.0/rfmanalysis/rfmanalysis.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:11:58.473820 rfmanalysis-0.2.0/rfmanalysis.egg-info/
+-rw-rw-rw-   0        0        0     5269 2023-05-17 00:11:58.000000 rfmanalysis-0.2.0/rfmanalysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-17 00:11:58.000000 rfmanalysis-0.2.0/rfmanalysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 00:11:58.000000 rfmanalysis-0.2.0/rfmanalysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 18:47:20.000000 rfmanalysis-0.2.0/rfmanalysis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-17 00:11:58.000000 rfmanalysis-0.2.0/rfmanalysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      454 2023-05-17 00:11:58.498105 rfmanalysis-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-17 00:10:31.000000 rfmanalysis-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:11:58.484524 rfmanalysis-0.2.0/tests/
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-05-16 18:36:44.000000 rfmanalysis-0.2.0/tests/test_rfmanalysis.py
```

### Comparing `rfmanalysis-0.1.6/CONTRIBUTING.rst` & `rfmanalysis-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.6/LICENSE` & `rfmanalysis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.6/PKG-INFO` & `rfmanalysis-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfmanalysis
-Version: 0.1.6
+Version: 0.2.0
 Summary: This repository contains a Python implementation of RFM (Recency, Frequency, Monetary) analysis, a customer segmentation technique used in marketing and customer relationship management. The RFM analysis helps identify customer segments based on their purchasing behavior, allowing businesses to tailor their marketing strategies and customer retention efforts.
 Home-page: https://github.com/emmayann/rfmanalysis
 Author: Emma Hovhannisyan
 Author-email: emmahovhannisyan02@gmail.com
 License: MIT license
 Keywords: rfmanalysis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rfmanalysis-0.1.6/README.rst` & `rfmanalysis-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.6/docs/Makefile` & `rfmanalysis-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.6/docs/conf.py` & `rfmanalysis-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.6/docs/installation.rst` & `rfmanalysis-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.6/docs/make.bat` & `rfmanalysis-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.6/rfmanalysis/rfmanalysis.py` & `rfmanalysis-0.2.0/rfmanalysis/rfmanalysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,29 @@
         """
 
         self.data = data
         self.id_col = id_col
         self.date_col = date_col
         self.revenue_col = revenue_col
         self.rfm_data = None
+    
+    def process_data(self):
+        """
+        Applies all the transformation to the given data.
+
+        """
+        methods = (self.create_rfm_columns, 
+                   self.scale_rfm_columns, 
+                   self.rfm_scores, 
+                   self.give_names_to_segments, 
+                   self.segments_distribution)
+       
+        for method in methods:
+            method()
+        
 
     def create_rfm_columns(self):
         """
         Creates the RFM columns (Recency, Frequency, Monetary) from the input data.
 
         """
 
@@ -112,30 +127,30 @@
 
         Returns:
             str: The segment name.
 
         """
 
         rfm_score = row['RFM_Score']
-
+        
         if rfm_score >= 9:
             return "Can't Lose Them"
-        elif 8 <= rfm_score < 9:
+        elif rfm_score >= 8:
             return "Champions"
-        elif 7 <= rfm_score < 8:
+        elif rfm_score >=7:
             return "Loyal/Committed"
-        elif 6 <= rfm_score < 7:
+        elif rfm_score >= 6:
             return "Potential"
-        elif 5 <= rfm_score < 6:
+        elif rfm_score >= 5:
             return "Promising"
-        elif 4 <= rfm_score < 5:
+        elif rfm_score >= 4:
             return "Requires Attention"
         else:
             return "Demands Activation"
-
+    
     def give_names_to_segments(self):
         """
         Assigns segment names to each customer based on RFM scores.
 
         """
 
         self.rfm_data['Segment_Name'] = self.rfm_data.apply(self.naming, axis=1)
@@ -176,30 +191,46 @@
         segment_boxplot(rfm_data):
             Creates box plots for each RFM variable, grouped by segment.
 
         segment_comparison(rfm_data):
             Creates bar plots to compare the mean values of RFM variables across segments.
 
     """
+    @classmethod
+    def visualize_data(cls,data):
+        """
+        Applies all the visualization to the given transformed data.
+
+        """
+        methods = (cls.plot_rfm, 
+                   cls.visualize_segments, 
+                   cls.segment_boxplot, 
+                   cls.segment_distribution_barplot, 
+                   cls.segment_comparison)
+       
+        for method in methods:
+            method(data)
+        
+
     @staticmethod
     def plot_rfm(rfm_data):
         """
         Plots the distribution of the RFM variables.
 
         Args:
             rfm_data (DataFrame): RFM analysis results.
 
         """
         plt.figure(figsize=(12, 10))
         plt.subplot(3, 1, 1)
-        sns.distplot(rfm_data['Recency'])
+        sns.histplot(rfm_data['Recency'], kde=True)
         plt.subplot(3, 1, 2)
-        sns.distplot(rfm_data['Frequency'])
+        sns.histplot(rfm_data['Frequency'], kde=True)
         plt.subplot(3, 1, 3)
-        sns.distplot(rfm_data['Monetary'])
+        sns.histplot(rfm_data['Monetary'], kde=True)
         plt.tight_layout()
         plt.show()
 
     @staticmethod
     def visualize_segments(rfm_data):
         """
         Visualizes the distribution of customers across RFM segments using a treemap.
```

### Comparing `rfmanalysis-0.1.6/rfmanalysis.egg-info/PKG-INFO` & `rfmanalysis-0.2.0/rfmanalysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfmanalysis
-Version: 0.1.6
+Version: 0.2.0
 Summary: This repository contains a Python implementation of RFM (Recency, Frequency, Monetary) analysis, a customer segmentation technique used in marketing and customer relationship management. The RFM analysis helps identify customer segments based on their purchasing behavior, allowing businesses to tailor their marketing strategies and customer retention efforts.
 Home-page: https://github.com/emmayann/rfmanalysis
 Author: Emma Hovhannisyan
 Author-email: emmahovhannisyan02@gmail.com
 License: MIT license
 Keywords: rfmanalysis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rfmanalysis-0.1.6/rfmanalysis.egg-info/SOURCES.txt` & `rfmanalysis-0.2.0/rfmanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.6/setup.py` & `rfmanalysis-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='rfmanalysis',
     name='rfmanalysis',
     packages=find_packages(include=['rfmanalysis', 'rfmanalysis.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/emmayann/rfmanalysis',
-    version='0.1.6',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `rfmanalysis-0.1.6/tests/test_rfmanalysis.py` & `rfmanalysis-0.2.0/tests/test_rfmanalysis.py`

 * *Files identical despite different names*

