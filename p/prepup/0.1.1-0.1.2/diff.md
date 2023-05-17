# Comparing `tmp/prepup-0.1.1.tar.gz` & `tmp/prepup-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.1.1.tar", last modified: Wed May  3 18:44:57 2023, max compression
+gzip compressed data, was "prepup-0.1.2.tar", last modified: Wed May 17 04:35:50 2023, max compression
```

## Comparing `prepup-0.1.1.tar` & `prepup-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:44:57.597042 prepup-0.1.1/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4246 2023-05-03 18:44:57.595040 prepup-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3710 2023-05-03 18:43:20.000000 prepup-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 18:44:57.576451 prepup-0.1.1/prepup/
--rw-rw-rw-   0        0        0     7969 2023-05-03 18:15:40.000000 prepup-0.1.1/prepup/__init__.py
--rw-rw-rw-   0        0        0    33177 2023-05-03 18:14:07.000000 prepup-0.1.1/prepup/common.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:44:57.593027 prepup-0.1.1/prepup.egg-info/
--rw-rw-rw-   0        0        0     4246 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      220 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 18:44:57.598040 prepup-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1488 2023-05-03 18:44:52.000000 prepup-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 04:35:50.365737 prepup-0.1.2/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4255 2023-05-17 04:35:50.365737 prepup-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3719 2023-05-17 04:35:37.000000 prepup-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 04:35:50.349316 prepup-0.1.2/prepup/
+-rw-rw-rw-   0        0        0     7969 2023-05-17 04:35:41.000000 prepup-0.1.2/prepup/__init__.py
+-rw-rw-rw-   0        0        0    33833 2023-05-17 04:34:27.000000 prepup-0.1.2/prepup/common.py
+drwxrwxrwx   0        0        0        0 2023-05-17 04:35:50.361724 prepup-0.1.2/prepup.egg-info/
+-rw-rw-rw-   0        0        0     4255 2023-05-17 04:35:50.000000 prepup-0.1.2/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-17 04:35:50.000000 prepup-0.1.2/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 04:35:50.000000 prepup-0.1.2/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-17 04:35:50.000000 prepup-0.1.2/prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      220 2023-05-17 04:35:50.000000 prepup-0.1.2/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 04:35:50.000000 prepup-0.1.2/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-05-17 04:35:39.000000 prepup-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 04:35:50.365737 prepup-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-05-17 04:35:33.000000 prepup-0.1.2/setup.py
```

### Comparing `prepup-0.1.1/LICENSE` & `prepup-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.1.1/PKG-INFO` & `prepup-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -12,15 +12,15 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # prepup
 
 
 [![image](https://img.shields.io/pypi/v/prepup.svg)](https://pypi.python.org/pypi/prepup)
-[![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup)
+<!-- [![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup) -->
 
 
 
 ### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your windows/macOS terminal.
 
 ## Installation
 -   Prepup can be installed using the Pip package manager.
```

### Comparing `prepup-0.1.1/README.md` & `prepup-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # prepup
 
 
 [![image](https://img.shields.io/pypi/v/prepup.svg)](https://pypi.python.org/pypi/prepup)
-[![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup)
+<!-- [![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup) -->
 
 
 
 ### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your windows/macOS terminal.
 
 ## Installation
 -   Prepup can be installed using the Pip package manager.
```

### Comparing `prepup-0.1.1/prepup/__init__.py` & `prepup-0.1.2/prepup/__init__.py`

 * *Files identical despite different names*

### Comparing `prepup-0.1.1/prepup/common.py` & `prepup-0.1.2/prepup/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -415,15 +415,15 @@
         
             dataframe.write_csv(path)
             print("\nMissing Data Imputed and saved succesfully")
             print(colored(term_font.renderText("\nDone...")))
         elif choice == 3:
             dataframe = dataframe.to_pandas()
             for column in dataframe.columns:
-                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Date and dataframe[column].dtype != pl.Datetime and dataframe[column].dtype != pl.Duration and dataframe[column].dtype != pl.Time and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
                     dataframe[column] = dataframe[column].fillna(dataframe[column].mean())
             dataframe.to_parquet("missing_data.parquet")
             data_path = input("\nEnter path to save Imputed data : ")
             path = data_path  
             s = "\\"
             if s in path:
                 path = path.replace(os.sep, '/')
@@ -435,15 +435,15 @@
         
             dataframe.to_csv(path)
             print("\nMissing Data Imputed and saved succesfully")
             print(colored(term_font.renderText("\nDone...")))
         elif choice == 4:
             dataframe = dataframe.to_pandas()
             for column in dataframe.columns:
-                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Date and dataframe[column].dtype != pl.Datetime and dataframe[column].dtype != pl.Duration and dataframe[column].dtype != pl.Time and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
                     dataframe[column] = dataframe[column].fillna(dataframe[column].median())
             dataframe.to_parquet("missing_data.parquet")
             data_path = input("\nEnter path to save Imputed data : ")
             path = data_path  
             s = "\\"
             if s in path:
                 path = path.replace(os.sep, '/')
@@ -455,15 +455,15 @@
         
             dataframe.to_csv(path)
             print("\nMissing Data Imputed and saved succesfully")
             print(colored(term_font.renderText("\nDone...")))
         elif choice == 5:
             dataframe = dataframe.to_pandas()
             for column in dataframe.columns:
-                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Date and dataframe[column].dtype != pl.Datetime and dataframe[column].dtype != pl.Duration and dataframe[column].dtype != pl.Time and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
                     mean = dataframe[column].mean()
                     std = dataframe[column].std()
                     random_values = np.random.normal(loc=mean, scale=std, size=dataframe[column].isnull().sum())
                     dataframe[column] = dataframe[column].fillna(pd.Series(random_values,index=dataframe[column][dataframe[column].isnull()].index))
             dataframe.to_parquet("missing_data.parquet")
             data_path = input("\nEnter path to save Imputed data : ")
             path = data_path  
@@ -512,15 +512,15 @@
         
             dataframe.write_csv(path)
             print("\nMissing Data Imputed and saved succesfully")
             print(colored(term_font.renderText("\nDone...")))
         elif choice == 8: 
             dataframe = dataframe.to_pandas()
             for column in dataframe.columns:
-                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Date and dataframe[column].dtype != pl.Datetime and dataframe[column].dtype != pl.Duration and dataframe[column].dtype != pl.Time and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
                     missing_inds = dataframe[column].isnull()
                     non_missing_inds = ~missing_inds
                     non_missing_vals = dataframe[column][non_missing_inds]
                     closest_inds = np.abs(dataframe[column][missing_inds].values - non_missing_vals.values.reshape(-1,1)).argmin(axis=0)
                     dataframe.loc[missing_inds, column] = non_missing_vals.iloc[closest_inds].values
             dataframe.to_parquet("missing_data.parquet")
             data_path = input("\nEnter path to save Imputed data : ")
```

### Comparing `prepup-0.1.1/prepup.egg-info/PKG-INFO` & `prepup-0.1.2/prepup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -12,15 +12,15 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # prepup
 
 
 [![image](https://img.shields.io/pypi/v/prepup.svg)](https://pypi.python.org/pypi/prepup)
-[![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup)
+<!-- [![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup) -->
 
 
 
 ### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your windows/macOS terminal.
 
 ## Installation
 -   Prepup can be installed using the Pip package manager.
```

### Comparing `prepup-0.1.1/setup.py` & `prepup-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setuptools.setup(
     name="prepup",
-    version="0.1.1",
+    version="0.1.2",
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
     description="Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     entry_points={
```

