# Comparing `tmp/openpolicedata-0.5.2.tar.gz` & `tmp/openpolicedata-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpolicedata-0.5.2.tar", last modified: Fri Apr 21 12:22:15 2023, max compression
+gzip compressed data, was "openpolicedata-0.5.3.tar", last modified: Wed May 17 11:30:29 2023, max compression
```

## Comparing `openpolicedata-0.5.2.tar` & `openpolicedata-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 12:22:15.306262 openpolicedata-0.5.2/
--rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.2/LICENSE
--rw-rw-rw-   0        0        0    12140 2023-04-21 12:22:15.307252 openpolicedata-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    11024 2023-02-11 13:57:45.000000 openpolicedata-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 12:22:15.283528 openpolicedata-0.5.2/openpolicedata/
--rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.2/openpolicedata/__init__.py
--rw-rw-rw-   0        0        0       21 2023-04-17 23:24:30.000000 openpolicedata-0.5.2/openpolicedata/_version.py
--rw-rw-rw-   0        0        0    30772 2023-04-20 11:21:06.000000 openpolicedata-0.5.2/openpolicedata/data.py
--rw-rw-rw-   0        0        0    72813 2023-04-21 11:39:12.000000 openpolicedata-0.5.2/openpolicedata/data_loaders.py
--rw-rw-rw-   0        0        0    10387 2023-02-14 01:01:36.000000 openpolicedata-0.5.2/openpolicedata/datasets.py
--rw-rw-rw-   0        0        0     8616 2023-04-17 11:23:17.000000 openpolicedata-0.5.2/openpolicedata/defs.py
--rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.2/openpolicedata/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 12:22:15.292920 openpolicedata-0.5.2/openpolicedata.egg-info/
--rw-rw-rw-   0        0        0    12140 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-21 12:22:15.000000 openpolicedata-0.5.2/openpolicedata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      426 2023-02-11 00:12:22.000000 openpolicedata-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0     1318 2023-04-21 12:22:15.309253 openpolicedata-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 12:22:15.304252 openpolicedata-0.5.2/tests/
--rw-rw-rw-   0        0        0    20542 2023-04-17 23:25:34.000000 openpolicedata-0.5.2/tests/test_data_loaders.py
--rw-rw-rw-   0        0        0     9035 2023-04-17 11:23:01.000000 openpolicedata-0.5.2/tests/test_datasets.py
--rw-rw-rw-   0        0        0    11163 2023-04-19 23:02:19.000000 openpolicedata-0.5.2/tests/test_opd_data1.py
--rw-rw-rw-   0        0        0     7811 2023-04-18 23:05:43.000000 openpolicedata-0.5.2/tests/test_opd_data2.py
--rw-rw-rw-   0        0        0    11428 2023-04-21 12:15:02.000000 openpolicedata-0.5.2/tests/test_opd_data3.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:30:29.701840 openpolicedata-0.5.3/
+-rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0    14926 2023-05-17 11:30:29.701840 openpolicedata-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13810 2023-05-17 11:28:27.000000 openpolicedata-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 11:30:29.674685 openpolicedata-0.5.3/openpolicedata/
+-rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.3/openpolicedata/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-17 11:28:49.000000 openpolicedata-0.5.3/openpolicedata/_version.py
+-rw-rw-rw-   0        0        0    27852 2023-05-15 18:51:42.000000 openpolicedata-0.5.3/openpolicedata/data.py
+-rw-rw-rw-   0        0        0    76281 2023-05-15 22:48:16.000000 openpolicedata-0.5.3/openpolicedata/data_loaders.py
+-rw-rw-rw-   0        0        0    10789 2023-05-16 01:27:28.000000 openpolicedata-0.5.3/openpolicedata/datasets.py
+-rw-rw-rw-   0        0        0     8688 2023-05-15 14:13:51.000000 openpolicedata-0.5.3/openpolicedata/defs.py
+-rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.3/openpolicedata/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:30:29.685684 openpolicedata-0.5.3/openpolicedata.egg-info/
+-rw-rw-rw-   0        0        0    14926 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      426 2023-02-11 00:12:22.000000 openpolicedata-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1318 2023-05-17 11:30:29.702841 openpolicedata-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:30:29.698841 openpolicedata-0.5.3/tests/
+-rw-rw-rw-   0        0        0    21379 2023-05-15 20:54:33.000000 openpolicedata-0.5.3/tests/test_data_loaders.py
+-rw-rw-rw-   0        0        0     9154 2023-05-15 21:25:37.000000 openpolicedata-0.5.3/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    11203 2023-05-16 01:20:33.000000 openpolicedata-0.5.3/tests/test_opd_data1.py
+-rw-rw-rw-   0        0        0     7997 2023-05-15 18:44:53.000000 openpolicedata-0.5.3/tests/test_opd_data2.py
+-rw-rw-rw-   0        0        0    11428 2023-05-04 00:15:34.000000 openpolicedata-0.5.3/tests/test_opd_data3.py
```

### Comparing `openpolicedata-0.5.2/LICENSE` & `openpolicedata-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.2/PKG-INFO` & `openpolicedata-0.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,12 @@
-Metadata-Version: 2.1
-Name: openpolicedata
-Version: 0.5.2
-Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
-Home-page: https://github.com/openpolicedata/openpolicedata
-Author: Matt Sowd
-Author-email: openpolicedata@gmail.com
-Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
-Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)
 
 # OpenPoliceData
-OpenPoliceData is a Python package that provides easy access to 288 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python package that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
 
@@ -46,18 +25,66 @@
 ```
 pip install openpolicedata
 ``` 
 
 Additionally, [geopandas](https://geopandas.org/en/stable/getting_started/install.html) can be installed to enable downloaded data tables to be returned as geopandas DataFrames instead of pandas DataFrames when there is geographic data. It is recommended to use [conda](https://docs.conda.io/en/latest/) to install geopandas.
 
 ## Examples
-[Jupyter notebooks](https://jupyter.org/) demonstrating example usage of OpenPoliceData can be found in the [opd-examples](https://github.com/openpolicedata/opd-examples) repo. 
-
 **[You can try out OpenPoliceData and run examples online on Binder.](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)**
 
+Basic usage of OpenPoliceData simply involves:
+1. Finding datasets
+2. Loading datasets
+
+The query function is used to find data. To get all available datasets, query can be used with no inputs. To get all police stops datasets in Virginia, try the following:
+```
+> import openpolicedata as opd
+> datasets = opd.datasets.query(state="Virginia", table_type="STOPS")
+> datasets
+```
+| **State**  | **SourceName** | **Agency** | **TableType** | **coverage_start** | **coverage_end** |
+|------------|----------------|------------------|---------------|----------|----------|
+| Virginia | Dumfries        | Dumfries          | STOPS | 2021-07-01    | 2023-03-31
+| Virginia | Virginia    | MULTIPLE      | STOPS | 2021-07-01    | 2023-03-31
+
+(only 1st 6 columns shown above)
+
+There are 2 stops (containing pedestrian and traffic stops) datasets in Virginia: 1 for the town of Dumfries and 1 for every police department in Virginia (indicated by Agency being MULTIPLE). Let's load in data from the state data with `load_data_from_url`. To do this, we will first need to create a `Source`:
+
+```
+> src = opd.Source("Virginia")
+```
+If we are only interested in data from a single police department, we will need to set the optional agency input for load_data_from_url if we do not want to load data from all police departments in the state. `get_agencies` can be used to find the exact department name (if it is not known) by searching for agencies containing the `partial_name` input ("Arlington" in this case).
+```
+> agencies = src.get_agencies(table_type="STOPS", partial_name="Arlington")
+> agencies
+["Arlington County Sheriff's Office", 'Arlington County Police Department']
+```
+Now, we are ready to load the data.
+```
+> tbl = src.load_from_url(year=2021, table_type="STOPS", agency="Arlington County Police Department")
+> tbl.table.head(n=3)
+```
+
+| **incident_date**  | **agency_name** | **agency** | **reason_for_stop** | **race** | **ethnicity** |
+|------------|----------------|------------------|---------------|----------|----------|
+| 2021-01-01 | Arlington County Police Department        | ARLINGTON CO          | OTHER | WHITE    | HISPANIC    |
+| 2021-01-01 | Arlington County Police Department    | ARLINGTON CO      | EQUIPMENT VIOLATION | WHITE    | NON-HISPANIC    |
+| 2021-01-01 | Arlington County Police Department    | ARLINGTON CO      | TRAFFIC VIOLATION | BLACK OR AFRICAN AMERICAN    | NON-HISPANIC    |
+
+(only 1st 6 columns shown above)
+
+`tbl.table` is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html) and therefore, can be analyzed directly in Python using the powerful [pandas analysis library](https://pandas.pydata.org/). Alternatively, the table can be exported to a CSV file to analyze with your favorite tool:
+
+```
+> tbl.to_csv()
+```
+
+More examples can be found in the [opd-examples](https://github.com/openpolicedata/opd-examples) repo. 
+
 ## Contributing
 If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD)
 
 ## Import
 ```
 > import openpolicedata as opd
 ```
```

### Comparing `openpolicedata-0.5.2/README.md` & `openpolicedata-0.5.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: openpolicedata
+Version: 0.5.3
+Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
+Home-page: https://github.com/openpolicedata/openpolicedata
+Author: Matt Sowd
+Author-email: openpolicedata@gmail.com
+Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
+Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)
 
 # OpenPoliceData
-OpenPoliceData is a Python package that provides easy access to 288 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python package that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
 
@@ -25,18 +46,66 @@
 ```
 pip install openpolicedata
 ``` 
 
 Additionally, [geopandas](https://geopandas.org/en/stable/getting_started/install.html) can be installed to enable downloaded data tables to be returned as geopandas DataFrames instead of pandas DataFrames when there is geographic data. It is recommended to use [conda](https://docs.conda.io/en/latest/) to install geopandas.
 
 ## Examples
-[Jupyter notebooks](https://jupyter.org/) demonstrating example usage of OpenPoliceData can be found in the [opd-examples](https://github.com/openpolicedata/opd-examples) repo. 
-
 **[You can try out OpenPoliceData and run examples online on Binder.](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)**
 
+Basic usage of OpenPoliceData simply involves:
+1. Finding datasets
+2. Loading datasets
+
+The query function is used to find data. To get all available datasets, query can be used with no inputs. To get all police stops datasets in Virginia, try the following:
+```
+> import openpolicedata as opd
+> datasets = opd.datasets.query(state="Virginia", table_type="STOPS")
+> datasets
+```
+| **State**  | **SourceName** | **Agency** | **TableType** | **coverage_start** | **coverage_end** |
+|------------|----------------|------------------|---------------|----------|----------|
+| Virginia | Dumfries        | Dumfries          | STOPS | 2021-07-01    | 2023-03-31
+| Virginia | Virginia    | MULTIPLE      | STOPS | 2021-07-01    | 2023-03-31
+
+(only 1st 6 columns shown above)
+
+There are 2 stops (containing pedestrian and traffic stops) datasets in Virginia: 1 for the town of Dumfries and 1 for every police department in Virginia (indicated by Agency being MULTIPLE). Let's load in data from the state data with `load_data_from_url`. To do this, we will first need to create a `Source`:
+
+```
+> src = opd.Source("Virginia")
+```
+If we are only interested in data from a single police department, we will need to set the optional agency input for load_data_from_url if we do not want to load data from all police departments in the state. `get_agencies` can be used to find the exact department name (if it is not known) by searching for agencies containing the `partial_name` input ("Arlington" in this case).
+```
+> agencies = src.get_agencies(table_type="STOPS", partial_name="Arlington")
+> agencies
+["Arlington County Sheriff's Office", 'Arlington County Police Department']
+```
+Now, we are ready to load the data.
+```
+> tbl = src.load_from_url(year=2021, table_type="STOPS", agency="Arlington County Police Department")
+> tbl.table.head(n=3)
+```
+
+| **incident_date**  | **agency_name** | **agency** | **reason_for_stop** | **race** | **ethnicity** |
+|------------|----------------|------------------|---------------|----------|----------|
+| 2021-01-01 | Arlington County Police Department        | ARLINGTON CO          | OTHER | WHITE    | HISPANIC    |
+| 2021-01-01 | Arlington County Police Department    | ARLINGTON CO      | EQUIPMENT VIOLATION | WHITE    | NON-HISPANIC    |
+| 2021-01-01 | Arlington County Police Department    | ARLINGTON CO      | TRAFFIC VIOLATION | BLACK OR AFRICAN AMERICAN    | NON-HISPANIC    |
+
+(only 1st 6 columns shown above)
+
+`tbl.table` is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html) and therefore, can be analyzed directly in Python using the powerful [pandas analysis library](https://pandas.pydata.org/). Alternatively, the table can be exported to a CSV file to analyze with your favorite tool:
+
+```
+> tbl.to_csv()
+```
+
+More examples can be found in the [opd-examples](https://github.com/openpolicedata/opd-examples) repo. 
+
 ## Contributing
 If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD)
 
 ## Import
 ```
 > import openpolicedata as opd
 ```
```

### Comparing `openpolicedata-0.5.2/openpolicedata/__init__.py` & `openpolicedata-0.5.3/openpolicedata/__init__.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.2/openpolicedata/data.py` & `openpolicedata-0.5.3/openpolicedata/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -231,62 +231,76 @@
         -------
         list
             List containing types of data available from source
         '''
         return list(self.datasets["TableType"].unique())
 
 
-    def get_years(self, table_type, force=False):
+    def get_years(self, table_type, force=False, manual=False):
         '''Get years available for 1 or more datasets
 
         Parameters
         ----------
         table_type - str or TableType enum
             Only returns years for requested table type
         force - bool
             (Optional) Some data types such as CSV files require reading the whole file to filter for years. By default, an error will be thrown that indicates running load_from_url may be more efficient. For these cases, set force=True to run get_years without error.
+        manual - bool
+            (Optional) If True, for datasets that contain multiple years, the years will be determined by making requests to the dataset rather than using the years stored in the dataset table. The default is False, which runs faster.
 
         Returns
         -------
         list
             List of years available for 1 or more datasets
         '''
         dfs = self.__find_datasets(table_type)
 
+        cur_year = datetime.now().year
         all_years = list(dfs["Year"])
         years = set()
         for k in range(len(all_years)):
             if all_years[k] != MULTI:
                 years.add(all_years[k])
             else:
                 df = dfs.iloc[k]
                 _check_version(df)
                 data_type =DataType(df["DataType"])
                 url = df["URL"]
                 date_field = df["date_field"] if pd.notnull(df["date_field"]) else None
                 
                 loader = self.__get_loader(data_type, url, dataset_id=df["dataset_id"], date_field=date_field)
-                new_years = loader.get_years(force=force)
 
-                years.update(new_years)
+                check = None
+                if not manual and pd.notnull(df["coverage_start"]) and pd.notnull(df["coverage_end"]) and \
+                    hasattr(df["coverage_start"], 'year') and hasattr(df["coverage_end"], 'year'):
+                    years.update(range(df["coverage_start"].year, df["coverage_end"].year+1))
+                    if df["coverage_end"].year >= cur_year-2:
+                        # Check for updates
+                        check = [x for x in range(df["coverage_end"].year+1,cur_year+1)]
+                        if len(check)>0:
+                            new_years = loader.get_years(force=force, check=check)
+                            years.update(new_years)
+                else:
+                    new_years = loader.get_years(force=force)
+                    years.update(new_years)
             
         years = list(years)
         years.sort()
 
         return years
 
 
     def get_agencies(self, table_type=None, year=None, partial_name=None):
         '''Get agencies available for 1 or more datasets
 
         Parameters
         ----------
         table_type - str or TableType enum
             (Optional) If set, only returns agencies for requested table type
-        year - int or the string "MULTI" or "N/A"
+        year - int or the strings opd.defs.MULTI or opd.defs.NONE
             (Optional)  If set, only returns agencies for requested year
         table_type - str or TableType enum
             (Optional) If set, only returns agencies for requested table type
         partial_name - str
             (Optional)  If set, only returns agencies containing the substring
             partial_name for datasets that contain multiple agencies
 
@@ -302,15 +316,15 @@
             src = src[src["Year"] == year]
 
         if len(src) == 1:
             src = src.iloc[0]
         else:
             raise ValueError("table_type and year inputs must filter for a single source")            
 
-        # If year is multi, need to use self._agencyField to query URL
+        # If year is opd.defs.MULTI, need to use self._agencyField to query URL
         # Otherwise return self.agency
         if src["Agency"] == MULTI:
             _check_version(src)
             data_type =DataType(src["DataType"])
             loader = self.__get_loader(data_type, src["URL"], dataset_id=src["dataset_id"], date_field=src["date_field"], agency_field=src["agency_field"])
             if data_type ==DataType.CSV:
                 raise NotImplementedError(f"Unable to get agencies for {data_type}")
@@ -335,15 +349,15 @@
 
 
     def get_count(self, year=None, table_type=None, agency=None, force=False):
         '''Get number of records for a data request
 
         Parameters
         ----------
-        year (Optional) - int or length 2 list or the string "MULTI" or "N/A"
+        year (Optional) - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
             the return data for a specific year (int input) or a range of years
             [X,Y] to return data for years X to Y
         table_type - str or TableType enum
             (Optional) If set, requested dataset will be of this type
         agency - str
@@ -364,15 +378,15 @@
     
     
     def load_from_url_gen(self, year, table_type=None, agency=None, pbar=False, nbatch=10000, offset=0, force=False):
         '''Get generator to load data from URL in batches
 
         Parameters
         ----------
-        year - int or length 2 list or the string "MULTI" or "N/A"
+        year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
             the return data for a specific year (int input) or a range of years
             [X,Y] to return data for years X to Y
         table_type - str or TableType enum
             (Optional) If set, requested dataset will be of this type
         agency - str
@@ -402,15 +416,15 @@
         
 
     def load_from_url(self, year, table_type=None, agency=None, pbar=True, nrows=None, offset=0):
         '''Load data from URL
 
         Parameters
         ----------
-        year - int or length 2 list or the string "MULTI" or "N/A"
+        year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
             the return data for a specific year (int input) or a range of years
             [X,Y] to return data for years X to Y
         table_type - str or TableType enum
             (Optional) If set, requested dataset will be of this type
         agency - str
@@ -471,15 +485,15 @@
             if len(src) == 0:
                 raise ValueError(f"There are no sources matching tableType {table_type} and year {year}")
             elif len(src) > 1:
                 raise ValueError(f"There is more than one source matching tableType {table_type} and year {year}")
             else:
                 src = src.iloc[0]
 
-        # Load data from URL. For year or agency equal to multi, filtering can be done
+        # Load data from URL. For year or agency equal to opd.defs.MULTI, filtering can be done
         data_type =DataType(src["DataType"])
         url = src["URL"]
 
         if filter_by_year:
             year_filter = year
         else:
             year_filter = None
@@ -528,15 +542,15 @@
 
 
     def load_from_csv(self, year, output_dir=None, table_type=None, agency=None):
         '''Load data from previously saved CSV file
         
         Parameters
         ----------
-        year - int or length 2 list or the string "MULTI" or "N/A"
+        year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
             the return data for a specific year (int input) or a range of years
             [X,Y] to return data for years X to Y
         output_dir - str
             (output_dirOptional) Directory where CSV file is stored
         table_type - str or TableType enum
@@ -563,15 +577,15 @@
         return table
 
     def get_csv_filename(self, year, output_dir=None, table_type=None, agency=None):
         '''Get auto-generated CSV filename
         
         Parameters
         ----------
-        year - int or length 2 list or the string "MULTI" or "N/A"
+        year - int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
             Used to identify the requested dataset if equal to its year value
             Otherwise, for datasets containing multiple years, this filters 
             the return data for a specific year (int input) or a range of years
             [X,Y] to return data for years X to Y
         output_dir - str
             (Optional) Directory where CSV file is stored
         table_type - str or TableType enum
@@ -660,18 +674,18 @@
         Name of state
     source_name - str
         Name of source
     agency - str
         Name of agency
     table_type - str or TableType enum
         Type of data
-    year = int or length 2 list or the string "MULTI" or "N/A"
+    year = int or length 2 list or the string opd.defs.MULTI or opd.defs.NONE
         Year of data to load, range of years of data to load as a list [X,Y]
         to load years X to Y, or a string to indicate all of multiple year data
-        ("MULTI") or a dataset that has no year filtering ("N/A")
+        (opd.defs.MULTI) or a dataset that has no year filtering ("N/A")
 
     Returns
     -------
     str
         Default CSV filename
     '''
     if isinstance(table_type, TableType):
@@ -706,107 +720,7 @@
                     "It will be made available in a future release"
             )
         elif version.parse(__version__) < version.parse(min_version):
             raise exceptions.OPD_MinVersionError(
                 f"Year {year} {table_type} data for {src_name} in {state} cannot be loaded in version {__version__} of openpolicedata. " + \
                     f"Update OpenPoliceData to at least version {min_version} to access this data."
             )
-
-
-if __name__ == '__main__':
-    istart = 182
-    from datetime import date
-    datasets = _datasets.datasets_query()
-    max_num_stanford = 1
-    num_stanford = 0
-    prev_sources = []
-    prev_tables = []
-    output_dir = ".\\data"
-    action = "standardize"
-    issue_datasets = ["Austin", "Chapel Hill", "Fayetteville", "San Diego"]
-    is_austin = datasets["SourceName"].apply(lambda x : x in issue_datasets)
-    not_austin = datasets["SourceName"].apply(lambda x : x not in issue_datasets)
-    # Austin has unknown race values. Emailed dataset owner.
-    datasets = pd.concat([datasets[not_austin], datasets[is_austin]])
-    for i in range(istart, len(datasets)):
-        if "stanford.edu" in datasets.iloc[i]["URL"]:
-            num_stanford += 1
-            if num_stanford > max_num_stanford:
-                continue
-
-        srcName = datasets.iloc[i]["SourceName"]
-        state = datasets.iloc[i]["State"]
-
-        if datasets.iloc[i]["Agency"] == MULTI and srcName == "Virginia":
-            # Reduce size of data load by filtering by agency
-            agency = "Fairfax County Police Department"
-        else:
-            agency = None
-
-        skip = False
-        for k in range(len(prev_sources)):
-            if srcName == prev_sources[k] and datasets.iloc[i]["TableType"] ==prev_tables[k]:
-                skip = True
-
-        if skip:
-            continue
-
-        prev_sources.append(srcName)
-        prev_tables.append(datasets.iloc[i]["TableType"])
-
-        table_print = datasets.iloc[i]["TableType"]
-        now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
-        print(f"{now} Saving CSV for dataset {i} of {len(datasets)}: {srcName} {table_print} table")
-
-        src = Source(srcName, state=state)
-
-        if action == "standardize":
-            if datasets.iloc[i]["DataType"] ==DataType.CSV.value:
-                table = src.load_from_csv(datasets.iloc[i]["Year"], table_type=datasets.iloc[i]["TableType"])
-            else:
-                year = date.today().year
-                table = None
-                for y in range(year, year-20, -1):
-                    try:
-                        csv_filename = src.get_csv_filename(y, output_dir, datasets.iloc[i]["TableType"], 
-                            agency=agency)
-                    except ValueError as e:
-                        if "There are no sources matching tableType" in e.args[0]:
-                            continue
-                        else:
-                            raise
-                    except:
-                        raise
-                    
-                    if path.exists(csv_filename):
-                        table = src.load_from_csv(y, table_type=datasets.iloc[i]["TableType"], 
-                            agency=agency,output_dir=output_dir)
-                        break
-
-            table.standardize()
-        else:
-            if datasets.iloc[i]["DataType"] ==DataType.CSV.value:
-                csv_filename = src.get_csv_filename(datasets.iloc[i]["Year"], output_dir, datasets.iloc[i]["TableType"])
-                if path.exists(csv_filename):
-                    continue
-                table = src.load_from_url(datasets.iloc[i]["Year"], datasets.iloc[i]["TableType"])
-            else:
-                years = src.get_years(datasets.iloc[i]["TableType"])
-                
-                if len(years)>1:
-                    # It is preferred to to not use first or last year that start and stop of year are correct
-                    year = years[-2]
-                else:
-                    year = years[0]
-
-                csv_filename = src.get_csv_filename(year, output_dir, datasets.iloc[i]["TableType"], 
-                                        agency=agency)
-
-                if path.exists(csv_filename):
-                    continue
-
-                table = src.load_from_url(year, datasets.iloc[i]["TableType"], 
-                                        agency=agency)
-
-            table.to_csv(".\\data")
-
-    print("data main function complete")
```

### Comparing `openpolicedata-0.5.2/openpolicedata/data_loaders.py` & `openpolicedata-0.5.3/openpolicedata/data_loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from io import BytesIO
 import numbers
 import os
 import tempfile
 from datetime import date
 import pandas as pd
+from pandas.api.types import is_numeric_dtype
+from pandas.api.types import is_datetime64_any_dtype as is_datetime
 from numpy import nan
 import requests
 import urllib
 import urllib3
 import ssl
 from abc import ABC, abstractmethod
 from sodapy import Socrata as SocrataClient
@@ -100,23 +102,26 @@
     load(year=None, nrows=None, pbar=True, agency=None, opt_filter=None, select=None, output_type=None)
         Load data for query
     get_count(year=None, agency=None, force=False, opt_filter=None, where=None)
         Get number of records/rows generated by query
     get_years(nrows=1)
         Get years contained in data set
     """
+
+    _last_count = None
+
     @abstractmethod
     def get_count(self, year=None, *, agency=None, force=False, opt_filter=None, where=None):
         pass
 
     @abstractmethod
     def load(self, year=None, nrows=None, offset=0, *, pbar=True, agency=None, opt_filter=None, select=None, output_type=None):
         pass
 
-    def get_years(self, *, nrows=1, **kwargs):
+    def get_years(self, *, nrows=1, check=None, **kwargs):
         '''Get years contained in data set
         
         Parameters
         ----------
         nrows : int
             (Optional) Number of records to load when checking each year
             
@@ -125,15 +130,25 @@
         list
             list containing years in data set
         '''
 
         if self.date_field==None:
             raise ValueError("A date field is required to get years")
 
-        year = date.today().year
+        check_input = check is not None
+
+        if check_input and len(check)==0:
+            return []
+
+        if check_input:
+            check = check.copy()
+            check.sort(reverse=True)
+            year = check.pop(0)
+        else:
+            year = date.today().year
 
         oldest_recent = 20
         max_misses_gap = 10
         max_misses = oldest_recent
         misses = 0
         years = []
         while misses < max_misses:
@@ -145,14 +160,20 @@
                 misses = 0
                 max_misses = max_misses_gap
                 years.append(year)
 
             sleep(sleep_time)
 
             year-=1
+            if check_input:
+                if len(check)==0:
+                    break
+                while year not in check:
+                    year-=1
+                check.remove(year)
 
         return years
 
 
 class Csv(Data_Loader):
     """
     A class for accessing data from CSV download URLs
@@ -208,35 +229,38 @@
             
         Returns
         -------
         int
             Record count or number of rows in data request
         '''
 
-        if ".zip" not in self.url and year==None and agency==None:            
+        if self._last_count is not None and self._last_count[0] == (self.url, year, agency):
+            return self._last_count[1]
+        if ".zip" not in self.url and year==None and agency==None:
             count = 0
             with requests.get(self.url, stream=True) as r:
                 for chunk in r.iter_content(chunk_size=2**16):
                     count += chunk.count(b"\n")
 
             # Subtract off trailing newlines in last row
             newline = int.from_bytes(b"\n", "big")
             for c in reversed(chunk):
                 if c==newline:
                     count-=1
                 else:
                     break
-
-            return count
         elif force:
-            return len(self.load(year=year, agency=agency))
+            count = len(self.load(year=year, agency=agency))
         else:
             raise ValueError("Extracting the number of records for a single year of a CSV file requires reading the whole file in. In most cases, "+
                 "running load() with a year argument to load in the data and manually finding the record count will be more "
                 "efficient. If running get_count with a year argument is still desired, set force=True")
+        
+        self._last_count = ((self.url, year, agency), count)
+        return count
 
 
     def load(self, year=None, nrows=None, offset=0, *, pbar=True, agency=None, **kwargs):
         '''Download CSV file to pandas DataFrame
         
         Parameters
         ----------
@@ -264,25 +288,45 @@
                 try:
                     table = pd.read_csv(self.url, encoding_errors='surrogateescape')
                 except urllib.error.HTTPError as e:
                     raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
                 except Exception as e:
                     raise e
         else:
-            r = requests.head(self.url)
-            if r.status_code==404:
-                # Try get instead
-                r = requests.get(self.url)
+            use_legacy = False
             try:
-                r.raise_for_status()
-            except requests.exceptions.HTTPError as e:
-                raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
+                r = requests.head(self.url)
+            except requests.exceptions.SSLError as e:
+                if "[SSL: UNSAFE_LEGACY_RENEGOTIATION_DISABLED] unsafe legacy renegotiation disabled" in str(e.args[0]) or \
+                    "[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate" in str(e.args[0]):
+                    use_legacy = True
+                else:
+                    raise e
             except Exception as e:
-                raise e
-            with requests.get(self.url, params=None, stream=True) as resp:
+                raise
+                
+            if not use_legacy:
+                if r.status_code==404:
+                    # Try get instead
+                    r = requests.get(self.url)
+                try:
+                    r.raise_for_status()
+                    r.close()
+                except requests.exceptions.HTTPError as e:
+                    raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
+                except Exception as e:
+                    raise e
+            
+            def get(url, use_legacy):
+                if use_legacy:
+                    return get_legacy_session().get(url, params=None, stream=True)
+                else:
+                    return requests.get(url, params=None, stream=True)
+                
+            with get(self.url, use_legacy) as resp:
                 try:
                     table = pd.read_csv(TqdmReader(resp, pbar=pbar), nrows=offset+nrows if nrows is not None else None, encoding_errors='surrogateescape')
                 except (urllib.error.HTTPError, pd.errors.ParserError) as e:
                     raise OPD_DataUnavailableError(*e.args, _url_error_msg.format(self.url))
                 except Exception as e:
                     raise e
 
@@ -426,16 +470,20 @@
             
         Returns
         -------
         int
             Record count or number of rows in data request
         '''
 
-        if force:
-            return len(self.load(year=year, agency=agency))
+        if self._last_count is not None and self._last_count[0]==(self.url, year, agency):
+            return self._last_count[1]
+        elif force:
+            count = len(self.load(year=year, agency=agency))
+            self._last_count = ((self.url, year, agency), count)
+            return count
         else:
             raise ValueError("Extracting the number of records for an Excel file requires reading the whole file in. In most cases, "+
                 "running load() to load in the data and manually finding the record count will be more "
                 "efficient. If running get_count with a year argument is still desired, set force=True")
 
 
     def __get_sheets(self):
@@ -647,15 +695,20 @@
             raise ValueError("Extracting the years of a Excel file requires reading the whole file in. In most cases, "+
                 "running load() with no arguments to load in the whole CSV file and manually finding the years will be more "
                 "efficient. If running get_years is still desired, set force=True")
         else:
             if self.date_field==None:
                 raise ValueError("No date field provided to access year information")
             df = self.load()
-            years = list(df[self.date_field].dt.year.dropna().unique())
+            if is_datetime(df[self.date_field]):
+                years = list(df[self.date_field].dt.year.dropna().unique())
+            elif is_numeric_dtype(df[self.date_field]):
+                years = list(df[self.date_field].dropna().unique())
+            else:
+                raise TypeError("Unknown date column format")
             return [int(x) for x in years]
 
 
 class Arcgis(Data_Loader):
     """
     A class for accessing data from ArcGIS clients
 
@@ -788,31 +841,37 @@
             
         Returns
         -------
         int
             Record count or number of rows in data request
         '''
         
-        if where==None:
-            where, record_count = self.__construct_where(year)
+        if self._last_count is not None and self._last_count[0]==(year,where):
+            record_count = self._last_count[1]
+            where_query = self._last_count[2]
+        elif where==None:
+            where_query, record_count = self.__construct_where(year)
         else:
+            where_query = where
             try:
                 record_count = self.__request(where=where, return_count=True)["count"]
                 if self.verify:
                     record_count_orig = self.__active_layer.query(where=where, return_count_only=True)
                     if record_count_orig!=record_count:
                         raise ValueError(f"Record count of {record_count} does not equal count from arcgis package of {record_count_orig}")
             except Exception as e:
                 if len(e.args)>0 and "Error Code: 429" in e.args[0]:
                     raise OPD_TooManyRequestsError(self.url, *e.args, _url_error_msg.format(self.url))
                 else:
                     raise
             except:
                 raise
 
+        self._last_count = ((year,where), record_count, where_query)
+
         return record_count
 
 
     def __request(self, where=None, return_count=False, out_fields="*", out_type="json", offset=0, count=None, sp_ref=None):
         
         # Running with no inputs or just an out_type will return metadata only
         url = self.url + "/"
@@ -858,15 +917,18 @@
         except: raise
         
         return r.json()
 
 
     def __construct_where(self, year=None):
         where_query = ""
-        if self.date_field!=None and year!=None:
+        if self._last_count is not None and self._last_count[0]==(year,None):
+            record_count = self._last_count[1]
+            where_query = self._last_count[2]
+        elif self.date_field!=None and year!=None:
             where_query, record_count = self._build_date_query(year)
         else:
             where_query = '1=1'
             try:
                 record_count = self.__request(where=where_query, return_count=True)["count"]
                 if self.verify:
                     record_count_orig = self.__active_layer.query(where=where_query, return_count_only=True)
@@ -876,14 +938,16 @@
                 if len(e.args)>0 and "Error Code: 429" in e.args[0]:
                     raise OPD_TooManyRequestsError(self.url, *e.args, _url_error_msg.format(self.url))
                 else:
                     raise
             except:
                 raise
 
+        self._last_count = ((year,None), record_count, where_query)
+
         return where_query, record_count
 
     
     def _build_date_query(self, year):
 
         # List of error messages that can occur for bad queries as we search for the right query format
         query_err_msg = ["Unable to complete operation", "Failed to execute query", "Unable to perform query", "Database error has occurred", 
@@ -1091,15 +1155,15 @@
                 bar.update(len(data["features"]))
 
         if pbar:
             bar.close()
 
         df = pd.DataFrame.from_records([x["attributes"] for x in features])
         for col in date_cols:
-            df[col] = pd.to_datetime(df[col], unit="ms")
+            df[col] = pd.to_datetime(df[col], unit="ms", errors='coerce')
 
         if len(df) > 0:
             has_point_geometry = any("geometry" in x and "x" in x["geometry"] for x in features)
             if not self.is_table and has_point_geometry:
                 if _use_gpd_force is not None:
                     if not _has_gpd and _use_gpd_force:
                         raise ValueError("User cannot force GeoPandas usage when it is not installed")
@@ -1199,19 +1263,25 @@
             (Optional) Either the year or the year range [first_year, last_year] for the data that is being requested.  None value returns data for all years.
             
         Returns
         -------
         int
             Record count or number of rows in data request
         '''
-        
-        where = self.__construct_where(year)
-        json = self.__request(where=where, return_count=True)
 
-        return json["rows"][0]["count"]
+        if self._last_count is not None and self._last_count[0]==year:
+            return self._last_count[1]
+        else:
+            where = self.__construct_where(year)
+            json = self.__request(where=where, return_count=True)
+            count = json["rows"][0]["count"]
+
+        self._last_count = (year, count, where)
+
+        return count
 
 
     def __request(self, where=None, return_count=False, out_fields="*", out_type="GeoJSON", offset=0, count=None):
 
         query = "SELECT "
         params = {}
         if return_count:
@@ -1275,17 +1345,22 @@
             
         Returns
         -------
         pandas or geopandas DataFrame
             DataFrame containing downloaded
         '''
         
-        where_query = self.__construct_where(year)
-        json = self.__request(where=where_query, return_count=True)
-        record_count = json["rows"][0]["count"]
+        if self._last_count is not None and self._last_count[0]==year:
+            record_count = self._last_count[1]
+            where_query = self._last_count[2]
+        else:
+            where_query = self.__construct_where(year)
+            json = self.__request(where=where_query, return_count=True)
+            record_count = json["rows"][0]["count"]
+            self._last_count = (year, record_count, where_query)
 
         record_count-=offset
         if record_count<=0:
             return None
 
         batch_size = _default_limit
         nrows = nrows if nrows!=None and record_count>=nrows else record_count
@@ -1446,31 +1521,37 @@
         int
             Record count or number of rows in data request
         '''
 
         if where==None:
             where = self.__construct_where(year, opt_filter)
 
+        if self._last_count is not None and self._last_count[0]==(year, opt_filter, where):
+            return self._last_count[1]
+
         try:
             results = self.client.get(self.data_set, where=where, select="count(*)")
-        except requests.HTTPError as e:
+        except (requests.HTTPError, requests.exceptions.ReadTimeout) as e:
             raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.url))
         except Exception as e: 
             if len(e.args)>0 and (e.args[0]=='Unknown response format: text/html' or \
                 "Read timed out" in e.args[0]):
                 raise OPD_SocrataHTTPError(self.url, self.data_set, *e.args, _url_error_msg.format(self.url))
             else:
                 raise e  
             
         try:
             num_rows = float(results[0]["count"])
         except:
             num_rows = float(results[0]["count_1"]) # Value used in VT Shootings data
 
-        return int(num_rows)
+        count = int(num_rows)
+        self._last_count = ((year, opt_filter, where),count)
+
+        return count
 
 
     def load(self, year=None, nrows=None, offset=0, *, pbar=True, opt_filter=None, select=None, output_type=None, **kwargs):
         '''Download table from Socrata to pandas or geopandas DataFrame
         
         Parameters
         ----------
```

### Comparing `openpolicedata-0.5.2/openpolicedata/datasets.py` & `openpolicedata-0.5.3/openpolicedata/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,23 +40,24 @@
         df.rename(columns={
             "Jurisdiction" : "Agency",
             "jurisdiction_field" : "agency_field"
         }, inplace=True)
 
     # Convert years to int
     df["Year"] = [int(x) if x.isdigit() else x for x in df["Year"]]
+    df["Year"] = df["Year"].apply(lambda x: "MULTIPLE" if x=="MULTI" else x)
     df["SourceName"] = df["SourceName"].str.replace("Police Department", "")
-    df["Agency"] = df["Agency"].str.replace("Police Department", "")
+    df["Agency"] = df["Agency"].str.replace("Police Department", "").apply(lambda x: "MULTIPLE" if x=="MULTI" else x)
 
     for col in df.columns:
         df[col] = [x.strip() if type(x)==str else x for x in df[col]]
 
     # ArcGIS datasets should have a URL ending in either /FeatureServer/# or /MapServer/#
     # Where # is a layer #
-    urls = df["URL"]
+    urls = list(df["URL"])
     p = re.compile(r"(MapServer|FeatureServer)/\d+")
     for i,url in enumerate(urls):
         if df.iloc[i]["DataType"] == defs.DataType.ArcGIS.value:
             result = p.search(url)
             urls[i] = url[:result.span()[1]]
 
     df["URL"] = urls
@@ -65,15 +66,19 @@
     not_state = df["State"].apply(lambda x: x not in defs.states)
     if not_state.any():
         misspelled = df["State"][not_state]
         raise ValueError(f"{len(misspelled)} states are misspelled in the data sources table including {misspelled.iloc[0]} at index {misspelled.index[0]}")
 
     key_vals = ['State', 'SourceName', 'Agency', 'TableType','Year']
     df.drop_duplicates(subset=key_vals, inplace=True)
-    # df.sort_values(by=keyVals, inplace=True, ignore_index=True)
+
+    if "coverage_start" in df:
+        p = re.compile(r"\d{1,2}/\d{1,2}/\d{4}")
+        df["coverage_start"] = df["coverage_start"].apply(lambda x: pd.to_datetime(x) if pd.notnull(x) and p.search(x) else x)
+        df["coverage_end"] = df["coverage_end"].apply(lambda x: pd.to_datetime(x) if pd.notnull(x) and p.search(x) else x)
 
     return df
 
 
 datasets = _build(csv_file)
 
 def query(source_name=None, state=None, agency=None, table_type=None):
```

### Comparing `openpolicedata-0.5.2/openpolicedata/defs.py` & `openpolicedata-0.5.3/openpolicedata/defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         "civilians and vehicles may be involved in an incident. This table contains information on non-motorists involved in a crash.")
     CRASHES_VEHICLES = ("CRASHES - VEHICLES",
         "Crash data may be split into several tables due to the possibility that multiple "+
         "civilians and vehicles may be involved in an incident. This table contains data on vehicles    .")
     EMPLOYEE = ("EMPLOYEE","Demographic data of the police workforce")
     FIELD_CONTACTS = ("FIELD CONTACTS", "Consensual contacts between officers and the community.")
     INCIDENTS = ("INCIDENTS", "Crime incident reports")
+    LAWSUITS = ("LAWSUITS", "Lawsuits against a police department")
     PEDESTRIAN = ("PEDESTRIAN STOPS","Stops of pedestrians based on 'reasonable suspicion'. May lead to a frisk.")
     PEDESTRIAN_ARRESTS = ("PEDESTRIAN ARRESTS","Pedestrian stops leading to an arrest")
     PEDESTRIAN_CITATIONS = ("PEDESTRIAN CITATIONS","Pedestrian stops leading to a citation")
     PEDESTRIAN_WARNINGS = ("PEDESTRIAN WARNINGS","Pedestrian stops leading to a warning")
     SHOOTINGS = ("OFFICER-INVOLVED SHOOTINGS","Shootings by officers")
     SHOOTINGS_CIVILIANS = ("OFFICER-INVOLVED SHOOTINGS - CIVILIANS",
         "Officer-involved shootings data may be split into several tables due to the possibility that multiple "+
@@ -94,15 +95,15 @@
         "Use of force data may be split into several tables due to the possibility that multiple "+
         "civilians and officers may be involved in an incident. This table contains data on civilians and officers.")
     VEHICLE_PURSUITS = ("VEHICLE PURSUITS","Attempts by officers in vehicles to pursue vehicles where the operator " + 
         "is believed to be aware that they are being signaled to stop but who is fleeing or ignoring the officer's attempt "+
         "to stop them.")
 
 # Constants used in dataset parameters
-MULTI = "MULTI"    # For data sets that put multiple years or agencies in 1 dataset
+MULTI = "MULTIPLE"    # For data sets that put multiple years or agencies in 1 dataset
 NA = "NONE"         # None = not applicable (pandas converts "N/A" to NaN)
 
 states = {
     "Alabama": "AL",
     "Alaska": "AK",
     "Arizona": "AZ",
     "Arkansas": "AR",
```

### Comparing `openpolicedata-0.5.2/openpolicedata/exceptions.py` & `openpolicedata-0.5.3/openpolicedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.2/openpolicedata.egg-info/PKG-INFO` & `openpolicedata-0.5.3/openpolicedata.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.2
+Version: 0.5.3
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)
 
 # OpenPoliceData
-OpenPoliceData is a Python package that provides easy access to 288 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
+OpenPoliceData is a Python package that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions. 
 
 Users request data by department name and type of data, and the data is returned as a pandas DataFrame. There is no need to manually find the data online or to know how to work with open data APIs (ArcGIS, Socrata, etc.).
 
 ![alt text](https://github.com/openpolicedata/opd-data/blob/main/OPD_Datasets_Map.png?raw=true)
 
 **[Installation](#installation)**
 
@@ -46,18 +46,66 @@
 ```
 pip install openpolicedata
 ``` 
 
 Additionally, [geopandas](https://geopandas.org/en/stable/getting_started/install.html) can be installed to enable downloaded data tables to be returned as geopandas DataFrames instead of pandas DataFrames when there is geographic data. It is recommended to use [conda](https://docs.conda.io/en/latest/) to install geopandas.
 
 ## Examples
-[Jupyter notebooks](https://jupyter.org/) demonstrating example usage of OpenPoliceData can be found in the [opd-examples](https://github.com/openpolicedata/opd-examples) repo. 
-
 **[You can try out OpenPoliceData and run examples online on Binder.](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)**
 
+Basic usage of OpenPoliceData simply involves:
+1. Finding datasets
+2. Loading datasets
+
+The query function is used to find data. To get all available datasets, query can be used with no inputs. To get all police stops datasets in Virginia, try the following:
+```
+> import openpolicedata as opd
+> datasets = opd.datasets.query(state="Virginia", table_type="STOPS")
+> datasets
+```
+| **State**  | **SourceName** | **Agency** | **TableType** | **coverage_start** | **coverage_end** |
+|------------|----------------|------------------|---------------|----------|----------|
+| Virginia | Dumfries        | Dumfries          | STOPS | 2021-07-01    | 2023-03-31
+| Virginia | Virginia    | MULTIPLE      | STOPS | 2021-07-01    | 2023-03-31
+
+(only 1st 6 columns shown above)
+
+There are 2 stops (containing pedestrian and traffic stops) datasets in Virginia: 1 for the town of Dumfries and 1 for every police department in Virginia (indicated by Agency being MULTIPLE). Let's load in data from the state data with `load_data_from_url`. To do this, we will first need to create a `Source`:
+
+```
+> src = opd.Source("Virginia")
+```
+If we are only interested in data from a single police department, we will need to set the optional agency input for load_data_from_url if we do not want to load data from all police departments in the state. `get_agencies` can be used to find the exact department name (if it is not known) by searching for agencies containing the `partial_name` input ("Arlington" in this case).
+```
+> agencies = src.get_agencies(table_type="STOPS", partial_name="Arlington")
+> agencies
+["Arlington County Sheriff's Office", 'Arlington County Police Department']
+```
+Now, we are ready to load the data.
+```
+> tbl = src.load_from_url(year=2021, table_type="STOPS", agency="Arlington County Police Department")
+> tbl.table.head(n=3)
+```
+
+| **incident_date**  | **agency_name** | **agency** | **reason_for_stop** | **race** | **ethnicity** |
+|------------|----------------|------------------|---------------|----------|----------|
+| 2021-01-01 | Arlington County Police Department        | ARLINGTON CO          | OTHER | WHITE    | HISPANIC    |
+| 2021-01-01 | Arlington County Police Department    | ARLINGTON CO      | EQUIPMENT VIOLATION | WHITE    | NON-HISPANIC    |
+| 2021-01-01 | Arlington County Police Department    | ARLINGTON CO      | TRAFFIC VIOLATION | BLACK OR AFRICAN AMERICAN    | NON-HISPANIC    |
+
+(only 1st 6 columns shown above)
+
+`tbl.table` is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html) and therefore, can be analyzed directly in Python using the powerful [pandas analysis library](https://pandas.pydata.org/). Alternatively, the table can be exported to a CSV file to analyze with your favorite tool:
+
+```
+> tbl.to_csv()
+```
+
+More examples can be found in the [opd-examples](https://github.com/openpolicedata/opd-examples) repo. 
+
 ## Contributing
 If you're interesting in helping out, see our [Contributing Guide](https://github.com/openpolicedata/openpolicedata/blob/main/CONTRIBUTING.MD)
 
 ## Import
 ```
 > import openpolicedata as opd
 ```
```

### Comparing `openpolicedata-0.5.2/openpolicedata.egg-info/SOURCES.txt` & `openpolicedata-0.5.3/openpolicedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.2/setup.cfg` & `openpolicedata-0.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.2/tests/test_data_loaders.py` & `openpolicedata-0.5.3/tests/test_data_loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 
         r = requests.get(f"https://phl.carto.com/api/v2/sql?q=SELECT count(*) FROM {dataset} WHERE {date_field} >= '{year}-01-01' AND {date_field} < '{year+1}-01-01'")
         r.raise_for_status()
         assert count==r.json()["rows"][0]["count"]
 
         df = loader.load(year=year, pbar=False)
 
+        assert len(df)==count
+
         offset = 1
         nrows = count - 2
         df_offset = loader.load(year=year, nrows=nrows, offset=1, pbar=False)
 
         assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
 
         df_offset = loader.load(year=year, offset=1, pbar=False)
@@ -119,14 +121,16 @@
         gis = data_loaders.Arcgis(url)
         # Confirm that verfication is not set
         with pytest.raises(AttributeError):
             gis._Arcgis__active_layer
         df = gis.load()
         count = gis.get_count()
 
+        assert len(df)==count
+
         offset = 1
         nrows = count-offset
         df_offset = gis.load(nrows=nrows, offset=offset)
         assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
 
         df_offset = gis.load(offset=offset)
         assert df_offset.equals(df.iloc[offset:].reset_index(drop=True))
@@ -221,14 +225,19 @@
         count = gis.get_count(year=year_filter)
         # Reset
         data_loaders._use_gpd_force = None
 
         assert type(df) == pd.DataFrame
         assert len(df) == count
 
+        count2 = gis.get_count(year=year_filter+1)
+
+        # Ensure that count updates properly with different call (most recent count is cached)
+        assert count!=count2
+
     def test_socrata_geopandas(self, csvfile, source, last, skip, loghtml):
         if _has_gpd:
             url = "data.montgomerycountymd.gov"
             data_set = "4mse-ku6q"
             date_field = "date_of_stop"
             year = 2020
             nrows = 1000
@@ -250,23 +259,30 @@
 
         # Reset
         data_loaders._use_gpd_force = None
 
         assert type(df) == pd.DataFrame
         assert len(df) == count
 
+        count2 = loader.get_count(year=year+1)
+
+        # Ensure that count updates properly with different call (most recent count is cached)
+        assert count!=count2
+
     def test_socrata(self, csvfile, source, last, skip, loghtml):
         lim = data_loaders._default_limit
         data_loaders._default_limit = 500
         url = "data.austintexas.gov"
         data_set = "sc8s-w4ka"
         loader = data_loaders.Socrata(url, data_set)
         df =loader.load(pbar=False)
         count = loader.get_count()
 
+        assert len(df)==count
+
         offset = 1
         nrows = len(df)-offset-1
         df_offset = loader.load(offset=offset,nrows=nrows, pbar=False)
         assert set(df.columns)==set(df_offset.columns)
         df_offset = df_offset[df.columns]
         assert df_offset.equals(df.iloc[offset:nrows+offset].reset_index(drop=True))
 
@@ -300,14 +316,16 @@
 
         df_comp = pd.read_csv(url)
         df_comp = df_comp.astype({date_field: 'datetime64[ns]'})
         df = df.astype({date_field: 'datetime64[ns]'})
 
         count = loader.get_count()
         assert len(df_comp) == count
+        # Test using cached value
+        assert count == loader.get_count()
 
         assert df_comp.equals(df)
 
         with pytest.raises(ValueError):
             loader.get_years()
 
         years = loader.get_years(force=True)
@@ -329,14 +347,19 @@
         df = loader.load(year=year, pbar=False)
         with pytest.raises(ValueError):
             count = loader.get_count(year=year)
 
         count = loader.get_count(year=year, force=True)
         assert len(df) == count
 
+        count2 = loader.get_count(year=year+1, force=True)
+
+        # Ensure that count updates properly with different call (most recent count is cached)
+        assert count!=count2
+
 
     def test_excel(self, csvfile, source, last, skip, loghtml):
         url = "https://www.norristown.org/DocumentCenter/View/1789/2017-2018-Use-of-Force"
         date_field = "Date"
         loader = data_loaders.Excel(url, date_field=date_field)
         df = loader.load(pbar=False)
 
@@ -353,14 +376,17 @@
         df_comp.columns = [x.strip() if isinstance(x, str) else x for x in df_comp.columns]
 
         with pytest.raises(ValueError):
             count = loader.get_count()
         count = loader.get_count(force=True)
         assert len(df_comp) == count
 
+        # Testing 2nd call which should used cached value
+        assert count == loader.get_count(force=True)
+
         assert df_comp.equals(df)
 
         with pytest.raises(ValueError):
             loader.get_years()
 
         years = loader.get_years(force=True)
 
@@ -503,12 +529,12 @@
     # tp.test_csv_year_filter(None,None,None,None,None)
     # tp.test_process_date_input_empty(None,None,None,None,None)
     # tp.test_process_date_too_many(None,None,None,None,None)
     # tp.test_process_dates_year_input_wrong_order(None,None,None,None,None)
     # tp.test_socrata(None,None,None,None,None)
     # tp.test_socrata_geopandas(None,None,None,None,None)
     # tp.test_socrata_pandas(None,None,None,None,None)
-    # tp.test_excel(None,None,None,None,None)
-    # tp.test_excel_year_sheets(None,None,None,None,None)
-    # tp.test_excel_header(None,None,None,None,None)
+    tp.test_excel(None,None,None,None,None)
+    tp.test_excel_year_sheets(None,None,None,None,None)
+    tp.test_excel_header(None,None,None,None,None)
     tp.test_excel_xls(None,None,None,None,None)
     tp.test_excel_xls_protected(None,None,None,None,None)
```

### Comparing `openpolicedata-0.5.2/tests/test_datasets.py` & `openpolicedata-0.5.3/tests/test_datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
         datasets = get_datasets(csvfile)
 
         for key in columns.keys():
             assert key in datasets
 
     def test_table_for_nulls(self, csvfile, source, last, skip, loghtml):
-        can_have_nulls = ["Description", "date_field", "dataset_id", "agency_field", "Year","readme","min_version","AgencyFull"]
+        can_have_nulls = ["Description", "date_field", "dataset_id", "agency_field", "Year","readme","min_version","AgencyFull","source_url","coverage_start","coverage_end"]
         datasets = get_datasets(csvfile)
         for col in datasets.columns:
             if not col in can_have_nulls:
                 assert pd.isnull(datasets[col]).sum() == 0
 
     
     def test_check_state_names(self, csvfile, source, last, skip, loghtml):
@@ -194,9 +194,10 @@
             opd.datasets.summary_by_table_type()
         
         
 
 if __name__ == "__main__":
     csvfile = None
     csvfile = "C:\\Users\\matth\\repos\\opd-data\\opd_source_table.csv"
-    TestDatasets().test_years_multi(csvfile,None,None,None,None)
-    TestDatasets().test_table_types(csvfile,None,None,None,None)
+    TestDatasets().test_table_for_nulls(csvfile,None,None,None,None)
+    # TestDatasets().test_years_multi(csvfile,None,None,None,None)
+    # TestDatasets().test_table_types(csvfile,None,None,None,None)
```

### Comparing `openpolicedata-0.5.2/tests/test_opd_data1.py` & `openpolicedata-0.5.3/tests/test_opd_data1.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 		ds["min_version"] = "0.0"
 		data._check_version(ds)
 		ds["min_version"] = pd.NA
 		data._check_version(ds)
 
 
 	def test_offsets_and_nrows(self, csvfile, source, last, skip, loghtml):
+		get_datasets(csvfile)
 		src = data.Source("Philadelphia")
 		df = src.load_from_url(year=2019, table_type="Officer-Involved Shootings").table
 		offset = 1
 		nrows = len(df)-2
 		df_offset = src.load_from_url(year=2019, table_type="Officer-Involved Shootings", offset=offset, nrows=nrows).table
 		assert df_offset.equals(df.iloc[offset:offset+nrows].reset_index(drop=True))
 		
@@ -196,15 +197,15 @@
 		year = 2021
 		assert loader.get_count(year=year) == src.get_count(year=year, table_type=TableType.STOPS)
 		year = [2020,2022]
 		assert loader.get_count(year=year) == src.get_count(year=year, table_type=TableType.STOPS)
 
 	def test_load_gen(self, csvfile, source, last, skip, loghtml):
 		datasets = [("Norristown",2016,"USE OF FORCE", 100),
-	      ("Denver", "MULTI", "OFFICER-INVOLVED SHOOTINGS",50),
+	      ("Denver", "MULTIPLE", "OFFICER-INVOLVED SHOOTINGS",50),
 	      ("Philadelphia", 2019, "OFFICER-INVOLVED SHOOTINGS", 500),
 	      ("Charlotte-Mecklenburg", "NONE", "Employee", 1000),
 		  ("Austin", 2012, "USE OF FORCE", 1000)]
 
 		for ds in datasets:
 			src = data.Source(ds[0])
 			df = src.load_from_url(ds[1], ds[2]).table
@@ -283,21 +284,22 @@
 					f.write("\n")
 
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
-	csvfile = r"..\opd-data\opd_source_table.csv"
+	csvfile = os.path.join("..", "opd-data", "opd_source_table.csv")
 	last = None
-	# last = 863-784+1
+	last = 873-290+1
 	skip = None
-	# skip = "Fayetteville,Seattle"
+	# skip = "Bloomington"
 	source = None
 	# source = "Mesa"
 	# tp.check_table_type_warning(csvfile, source, last, skip, None) 
-	# tp.test_source_download_limitable(csvfile, source, last, skip, None) 
-	tp.test_check_version(csvfile, None, last, skip, None) 
-	# tp.test_get_count(csvfile, None, last, skip, None)
 	# tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
+	# tp.test_check_version(csvfile, None, last, skip, None) #
+	tp.test_source_download_limitable(csvfile, source, last, skip, None) 
+	
+	# tp.test_get_count(csvfile, None, last, skip, None)
 	# tp.test_load_gen(csvfile, source, last, skip, None)
```

### Comparing `openpolicedata-0.5.2/tests/test_opd_data2.py` & `openpolicedata-0.5.3/tests/test_opd_data2.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,38 +34,45 @@
 		datasets = get_datasets(csvfile)
 		caught_exceptions = []
 		caught_exceptions_warn = []
 		if skip != None:
 			skip = skip.split(",")
 			skip = [x.strip() for x in skip]
 
+		already_ran = []
 		for i in range(len(datasets)):
 			if source != None and datasets.iloc[i]["SourceName"] != source:
 				continue
 			if skip != None and datasets.iloc[i]["SourceName"] in skip:
 				continue
 			if i < len(datasets) - last:
 				continue
 			if is_filterable(datasets.iloc[i]["DataType"]) or datasets.iloc[i]["Year"] != MULTI or \
 				datasets.iloc[i]["DataType"] == DataType.EXCEL.value:  # If Excel, we can possibly check
 				srcName = datasets.iloc[i]["SourceName"]
 				state = datasets.iloc[i]["State"]
+
+				if (srcName, state, datasets.iloc[i]["TableType"]) in already_ran:
+					continue
+
 				src = data.Source(srcName, state=state)
 
 				if datasets.iloc[i]["DataType"] == DataType.EXCEL.value:
 					loader = opd.data_loaders.Excel(datasets.iloc[i]["URL"])
 					has_year_sheets = loader._Excel__get_sheets()[1]
 					if not has_year_sheets:
 						continue
 
 
 				table_print = datasets.iloc[i]["TableType"]
 				now = datetime.now().strftime("%d.%b %Y %H:%M:%S")
 				print(f"{now} Testing {i+1} of {len(datasets)}: {srcName} {table_print} table")
 
+				already_ran.append((srcName, state, datasets.iloc[i]["TableType"]))
+
 				try:
 					years = src.get_years(datasets.iloc[i]["TableType"], force=True)
 				except warn_errors as e:
 					e.prepend(f"Iteration {i}", srcName, datasets.iloc[i]["TableType"])
 					caught_exceptions_warn.append(e)
 					continue
 				except (OPD_TooManyRequestsError, OPD_arcgisAuthInfoError) as e:
@@ -229,15 +236,15 @@
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
 	csvfile = os.path.join("..","opd-data","opd_source_table.csv")
 	last = None
-	last = 863-791+1
+	last = 873-857+1
 	source = None
 	# source = "Washington D.C."
 	skip = None
 	# skip = "Fayetteville,Seattle"
 	tp.test_get_years(csvfile, source, last, skip, None)
 	# tp.test_get_agencies(csvfile, None, None, skip, None)
 	# tp.test_get_agencies_name_match(csvfile, None, None, skip, None)
```

### Comparing `openpolicedata-0.5.2/tests/test_opd_data3.py` & `openpolicedata-0.5.3/tests/test_opd_data3.py`

 * *Files identical despite different names*

