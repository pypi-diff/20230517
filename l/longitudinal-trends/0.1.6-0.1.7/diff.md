# Comparing `tmp/longitudinal_trends-0.1.6.tar.gz` & `tmp/longitudinal_trends-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longitudinal_trends-0.1.6.tar", last modified: Sat May 13 10:28:05 2023, max compression
+gzip compressed data, was "longitudinal_trends-0.1.7.tar", last modified: Wed May 17 16:31:31 2023, max compression
```

## Comparing `longitudinal_trends-0.1.6.tar` & `longitudinal_trends-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-13 10:28:05.799192 longitudinal_trends-0.1.6/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.6/LICENSE
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.6/MANIFEST.in
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-13 10:28:05.792192 longitudinal_trends-0.1.6/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9719 2023-05-05 08:12:31.000000 longitudinal_trends-0.1.6/README.md
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-13 10:28:05.445888 longitudinal_trends-0.1.6/longitudinal_trends/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17774 2023-05-13 10:20:57.000000 longitudinal_trends-0.1.6/longitudinal_trends/__init__.py
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-13 10:28:05.725513 longitudinal_trends-0.1.6/longitudinal_trends.egg-info/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-13 10:28:04.000000 longitudinal_trends-0.1.6/longitudinal_trends.egg-info/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-05-13 10:28:05.000000 longitudinal_trends-0.1.6/longitudinal_trends.egg-info/SOURCES.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-05-13 10:28:04.000000 longitudinal_trends-0.1.6/longitudinal_trends.egg-info/dependency_links.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-05-13 10:28:04.000000 longitudinal_trends-0.1.6/longitudinal_trends.egg-info/requires.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-05-13 10:28:04.000000 longitudinal_trends-0.1.6/longitudinal_trends.egg-info/top_level.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-05-13 10:26:02.000000 longitudinal_trends-0.1.6/pyproject.toml
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.6/requirements.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-05-13 10:28:05.802196 longitudinal_trends-0.1.6/setup.cfg
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-17 16:31:31.356108 longitudinal_trends-0.1.7/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.7/LICENSE
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.7/MANIFEST.in
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-17 16:31:31.340478 longitudinal_trends-0.1.7/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9719 2023-05-05 08:12:31.000000 longitudinal_trends-0.1.7/README.md
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-17 16:31:30.991709 longitudinal_trends-0.1.7/longitudinal_trends/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    19451 2023-05-16 17:25:26.000000 longitudinal_trends-0.1.7/longitudinal_trends/__init__.py
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-17 16:31:31.277980 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/SOURCES.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/dependency_links.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/requires.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/top_level.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-05-17 16:30:52.000000 longitudinal_trends-0.1.7/pyproject.toml
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.7/requirements.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-05-17 16:31:31.356108 longitudinal_trends-0.1.7/setup.cfg
```

### Comparing `longitudinal_trends-0.1.6/LICENSE` & `longitudinal_trends-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.6/PKG-INFO` & `longitudinal_trends-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longitudinal_trends
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
```

### Comparing `longitudinal_trends-0.1.6/README.md` & `longitudinal_trends-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.6/longitudinal_trends/__init__.py` & `longitudinal_trends-0.1.7/longitudinal_trends/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+# # import datetime as dt
+
+# # from longitudinal_trends import RequestTrends
+
+# # day_data = RequestTrends('UBI', 'UBI', 'UBI_folder', dt.datetime(2012, 1, 1), dt.datetime(2022,12,31), 'daily') #4017 days
+
+# # day_data.time_series(reference_geo_code=" ")
+
+# import datetime as dt
+# from longitudinal_trends import RequestTrends
+
+# # # day_data = RequestTrends('Anxiety', '/m/0k_9', dt.datetime(2021, 11, 1), dt.datetime(2022,10,24), 'daily') #358 Days
+# # day_data = RequestTrends('UBI', 'UBI', 'UBI_folder', dt.datetime(2012, 1, 1), dt.datetime(2022,12,31), 'daily') #4017 days
+# # week_data = RequestTrends('Anxiety', '/m/0k_9', dt.datetime(2016,11,21), dt.datetime(2022,10,24), 'weekly') #2163 Days | 309 Weeks
+# month_data = RequestTrends('UBI', 'universal basic income', 'UBI_folder', dt.datetime(2012, 1, 1), dt.datetime(2022,12,31), 'monthly') #1890 Days | 63 Months
+
+# # day_data.cross_section('US')
+# # day_data.cross_section('US-AL')
+# # week_data.one_click_function('US-AL')
+# # week_data = RequestTrends('UBI', 'UBI', dt.datetime(2016,11,21), dt.datetime(2022,10,24), 'weekly') #2163 Days | 310 Weeks
+# # week_data.all_in_one_method()
+# # day_data.all_in_one_method(reference_geo_code="IT")
+# # week_data.convert_cross_section("US-AK")
+# # day_data.convert_cross_section("US-AL")
+# # day_data.time_series(reference_geo_code=" ")
+# # start, end = dt.datetime(2012, 1, 1), dt.datetime(2022,12,31)
+# # print(end-start)
+# month_data.time_series(reference_geo_code='IT')
+
 import pandas as pd
 import os
 import glob
 import json
 
 import requests
 from pytrends.exceptions import ResponseError
@@ -108,30 +137,33 @@
         
 
     # This method is intended to create necessary directories at each discretion
     def __create_required_directory(self, folder):
         if not os.path.exists(folder):
             os.mkdir(folder)
 
-
     # This method provides list of time periods to fetch data for
     def __determine_time_periods(self):
         timeperiod = ceil(self.__num_of_days/self.TIME_WINDOW)
 
         self.__times = [self.start_date + dt.timedelta(days=x*self.TIME_WINDOW) for x in range(0, timeperiod+1)]
         self.__times[-1] = self.end_date
 
 
     def cross_section(self, geo: str="", resolution: str="COUNTRY"):
         self.__logger.info("Collecting Cross Section Data now")
 
         res = ["COUNTRY", "REGION", "CITY"]
+
+        print(geo, " Before")
         if (not geo.strip() and resolution != "COUNTRY") or (geo.strip() and resolution not in res):
             self.__logger.info("Incorrect Resolution Provided. Defaulting to 'COUNTRY'")
-            resolution = "COUNTRY"    
+            resolution = "COUNTRY" 
+
+        print(geo, " After")
 
         self.__create_required_directory("{}/{}/by_region".format(self.folder_name, self.data_format))
 
         if self.data_format == 'daily':
             chng_delta = relativedelta(days=1)
             end_delta = relativedelta(days=0)
             form = 'day'
@@ -155,28 +187,29 @@
                 if (self.data_format == 'weekly' and current_time >= self.end_date) or (self.data_format != 'weekly' and current_time > self.end_date):
                     stats.stop()
                     break
 
                 current_end_time = current_time + end_delta
                 # print("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.folder_name, self.data_format,  form, i+1, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d")))
                 if os.path.exists("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.folder_name, self.data_format,  form, i+1, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d"))):
+                        # print('true')
                         self.__logger.info("Data for {}-{} already collected. Moving to next date...".format(current_time.strftime("%#d/%m/%#Y"), current_end_time.strftime("%#d/%m/%#Y")), extra={"markup": True})
                         current_time += chng_delta
                         i += 1
                 else:
                     try:
+                        print(geo, " Right Before")
                         self.__pytrend.build_payload(kw_list=[self.topic], geo=geo, 
                                                         timeframe='%s %s' % (current_time.strftime("%Y-%m-%d"), current_end_time.strftime("%Y-%m-%d"))) 
                         time.sleep(5)
                         df = self.__pytrend.interest_by_region(resolution=resolution, inc_geo_code=True, inc_low_vol=True)
                         df = df.rename(columns={self.topic:self.keyword})
                         i += 1
                     except ResponseError as e:
-                        #TODO: Throw error for status code 500
-                        #TODO: Save errors in a file
+
                         self.__logger.info("Please have patience as we reset rate limit ... ", extra={"markup": True})
                         time.sleep(5)
                         continue
                     except:
                         stats.stop() # Stop the animation
                         if not self.__in_notebook():
                             self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
@@ -297,14 +330,15 @@
 
             prev_window.iloc[:,1] = prev_window.iloc[:,1] * prev_window_multiplier
             next_window.iloc[:,1] = next_window.iloc[:,1] * next_window_multiplier
 
             prev_window = pd.concat([prev_window.iloc[:-1,:], next_window])
 
         prev_window.to_csv("{}/{}/concat_time_series/{}.csv".format(self.folder_name, self.data_format, reference_geo_code), index=False)
+        self.__logger.info("[bold green]Concatenation Complete! :) [/]", extra={"markup": True})
 
 
     def convert_cross_section(self, reference_geo_code: str="US", zero_replace: float=0.1):
         self.__logger.info("Rescaling cross section Data now", extra={"markup": True})
         
         self.__create_required_directory("{}/{}/converted".format(self.folder_name, self.data_format))
         self.__create_required_directory("{}/{}/converted/{}".format(self.folder_name, self.data_format, reference_geo_code))
@@ -316,22 +350,22 @@
                 record = row['date'].strftime('%Y%m%d')
                 time_ind = float(row[self.keyword])
 
                 snap_file = glob.glob("{}/{}/by_region/*{}*.csv".format(self.folder_name, self.data_format, record))[0]
                 fl_name = snap_file.split("\\")[-1]
                 col_name = fl_name.split('.')[0]
 
-                snap_df = pd.read_csv(snap_file)
+                snap_df = pd.read_csv(snap_file, keep_default_na=False)
                 snap_df[self.keyword].replace(0, zero_replace, inplace=True)
 
                 ref_value = float(snap_df.loc[snap_df['geoCode'].str.contains(reference_geo_code)][self.keyword])
         
                 conv_multiplier = float(time_ind/ref_value)
 
-                snap_df.iloc[:,2] = snap_df.iloc[:,2] * conv_multiplier
+                snap_df.iloc[:,2] = round(snap_df.iloc[:,2] * conv_multiplier, 2)
 
                 if ind==0:
                     conv = snap_df[['geoName', 'geoCode']]
 
                 kwarg = {col_name: list(snap_df[self.keyword])}
                 conv = conv.assign(**kwarg)
```

### Comparing `longitudinal_trends-0.1.6/longitudinal_trends.egg-info/PKG-INFO` & `longitudinal_trends-0.1.7/longitudinal_trends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longitudinal-trends
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
```

### Comparing `longitudinal_trends-0.1.6/pyproject.toml` & `longitudinal_trends-0.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]#, "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "longitudinal_trends"
-version='0.1.6'
+version='0.1.7'
 description="Generate long-term longitudinal Google Trends Data"
 urls = {homepage = "https://github.com/Mohammad-sakir/longitudinalTrends"}
 requires-python = ">=3.7"
 authors = [
     {name = "Mohammad Saleh Ahsan Sakir"},
     {name = "Taeyong Park"}, 
     {email="ahsansakir506@gmail.com"},
```

