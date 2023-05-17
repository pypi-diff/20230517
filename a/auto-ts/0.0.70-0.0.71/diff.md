# Comparing `tmp/auto_ts-0.0.70.tar.gz` & `tmp/auto_ts-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_ts-0.0.70.tar", last modified: Mon May  8 12:30:57 2023, max compression
+gzip compressed data, was "auto_ts-0.0.71.tar", last modified: Wed May 17 01:16:39 2023, max compression
```

## Comparing `auto_ts-0.0.70.tar` & `auto_ts-0.0.71.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.808270 auto_ts-0.0.70/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    15123 2023-05-08 12:30:57.808270 auto_ts-0.0.70/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    13237 2023-03-27 12:13:14.000000 auto_ts-0.0.70/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:56.890657 auto_ts-0.0.70/auto_ts/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    56587 2023-05-08 11:45:35.000000 auto_ts-0.0.70/auto_ts/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      370 2023-05-07 15:58:16.000000 auto_ts-0.0.70/auto_ts/__version__.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.153786 auto_ts-0.0.70/auto_ts/models/
--rwxrwxrwx   0 ram       (1000) ram       (1000)      229 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/__init__.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.432228 auto_ts-0.0.70/auto_ts/models/ar_based/
--rwxrwxrwx   0 ram       (1000) ram       (1000)      159 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11666 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_arima.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    16527 2023-05-08 11:46:10.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_arima_base.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     4148 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_autoarimax.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    18472 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_sarimax.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12940 2022-01-17 23:08:01.000000 auto_ts-0.0.70/auto_ts/models/ar_based/build_var.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     6502 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/ar_based/param_finder.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     3061 2022-08-16 11:58:44.000000 auto_ts-0.0.70/auto_ts/models/build_base.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    62805 2023-03-24 12:28:54.000000 auto_ts-0.0.70/auto_ts/models/build_ml.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    28736 2023-05-08 11:21:05.000000 auto_ts-0.0.70/auto_ts/models/build_prophet.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     5032 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/models/build_pyflux.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    30950 2022-01-30 16:58:11.000000 auto_ts-0.0.70/auto_ts/models/ml_models.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.587582 auto_ts-0.0.70/auto_ts/test/
--rwxrwxrwx   0 ram       (1000) ram       (1000)        0 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/test/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2921 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/test/test_auto_sarimax.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    79421 2023-02-22 13:28:30.000000 auto_ts-0.0.70/auto_ts/test/test_auto_ts.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12037 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/test/test_var.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.792641 auto_ts-0.0.70/auto_ts/utils/
--rwxrwxrwx   0 ram       (1000) ram       (1000)      710 2022-01-23 02:50:48.000000 auto_ts-0.0.70/auto_ts/utils/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      246 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/utils/colors.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    17493 2023-03-24 12:34:01.000000 auto_ts-0.0.70/auto_ts/utils/eda.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    25355 2023-05-07 16:15:31.000000 auto_ts-0.0.70/auto_ts/utils/etl.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1264 2021-08-27 20:33:30.000000 auto_ts-0.0.70/auto_ts/utils/logging.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     5020 2023-05-08 12:21:03.000000 auto_ts-0.0.70/auto_ts/utils/metrics.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11033 2022-01-22 20:15:38.000000 auto_ts-0.0.70/auto_ts/utils/my_encoders.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     9979 2021-12-07 01:54:05.000000 auto_ts-0.0.70/auto_ts/utils/val.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-08 12:30:57.006638 auto_ts-0.0.70/auto_ts.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    15123 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      975 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      181 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-05-08 12:30:56.000000 auto_ts-0.0.70/auto_ts.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-05-08 12:30:57.823891 auto_ts-0.0.70/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1072 2023-03-27 12:09:31.000000 auto_ts-0.0.70/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-17 01:16:39.839073 auto_ts-0.0.71/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14742 2023-05-17 01:16:39.823448 auto_ts-0.0.71/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12704 2023-05-17 01:09:28.000000 auto_ts-0.0.71/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-17 01:16:38.901570 auto_ts-0.0.71/auto_ts/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    56629 2023-05-17 01:00:44.000000 auto_ts-0.0.71/auto_ts/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      370 2023-05-16 11:30:38.000000 auto_ts-0.0.71/auto_ts/__version__.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-17 01:16:39.167198 auto_ts-0.0.71/auto_ts/models/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      229 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/models/__init__.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-17 01:16:39.417203 auto_ts-0.0.71/auto_ts/models/ar_based/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      159 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/models/ar_based/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11666 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/models/ar_based/build_arima.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    16527 2023-05-08 11:46:10.000000 auto_ts-0.0.71/auto_ts/models/ar_based/build_arima_base.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     4148 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/models/ar_based/build_autoarimax.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18472 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/models/ar_based/build_sarimax.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12940 2022-01-17 23:08:01.000000 auto_ts-0.0.71/auto_ts/models/ar_based/build_var.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     6502 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/models/ar_based/param_finder.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     3061 2022-08-16 11:58:44.000000 auto_ts-0.0.71/auto_ts/models/build_base.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    62805 2023-03-24 12:28:54.000000 auto_ts-0.0.71/auto_ts/models/build_ml.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    28736 2023-05-16 11:31:17.000000 auto_ts-0.0.71/auto_ts/models/build_prophet.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     5032 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/models/build_pyflux.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    30950 2022-01-30 16:58:11.000000 auto_ts-0.0.71/auto_ts/models/ml_models.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-17 01:16:39.542196 auto_ts-0.0.71/auto_ts/test/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        0 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/test/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     2921 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/test/test_auto_sarimax.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    79421 2023-02-22 13:28:30.000000 auto_ts-0.0.71/auto_ts/test/test_auto_ts.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12037 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/test/test_var.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-17 01:16:39.807821 auto_ts-0.0.71/auto_ts/utils/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      710 2022-01-23 02:50:48.000000 auto_ts-0.0.71/auto_ts/utils/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      246 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/utils/colors.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    17493 2023-03-24 12:34:01.000000 auto_ts-0.0.71/auto_ts/utils/eda.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    25355 2023-05-07 16:15:31.000000 auto_ts-0.0.71/auto_ts/utils/etl.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1264 2021-08-27 20:33:30.000000 auto_ts-0.0.71/auto_ts/utils/logging.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     5020 2023-05-08 12:21:03.000000 auto_ts-0.0.71/auto_ts/utils/metrics.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11033 2022-01-22 20:15:38.000000 auto_ts-0.0.71/auto_ts/utils/my_encoders.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     9979 2021-12-07 01:54:05.000000 auto_ts-0.0.71/auto_ts/utils/val.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-17 01:16:38.995323 auto_ts-0.0.71/auto_ts.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14742 2023-05-17 01:16:38.000000 auto_ts-0.0.71/auto_ts.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      975 2023-05-17 01:16:38.000000 auto_ts-0.0.71/auto_ts.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-05-17 01:16:38.000000 auto_ts-0.0.71/auto_ts.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      181 2023-05-17 01:16:38.000000 auto_ts-0.0.71/auto_ts.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-05-17 01:16:38.000000 auto_ts-0.0.71/auto_ts.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-05-17 01:16:39.839073 auto_ts-0.0.71/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1072 2023-05-17 00:29:01.000000 auto_ts-0.0.71/setup.py
```

### Comparing `auto_ts-0.0.70/PKG-INFO` & `auto_ts-0.0.71/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,82 +1,97 @@
 Metadata-Version: 2.1
 Name: auto_ts
-Version: 0.0.70
+Version: 0.0.71
 Summary: Automatically Build Multiple Time Series models fast - now with Facebook Prophet!
 Home-page: https://github.com/AutoViML/Auto_TS
 Author: Ram Seshadri
 License: Apache License 2.0
-Description: <!DOCTYPE html>
-        <html>
-        <head>
-        </head>
-        <body>
-        
-        ![auto-ts](logo.png)
-        
-        <h1 id="mar-update">March 2023 Update:</h1>
-        <p style="font-family:verdana">We have now upgraded FB Prophet to the latest version which is simply called prophet. <br>
-        If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise error!):
+Description: <h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
+        <p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.
+        
+        ![auto-ts](images/logo.png)
+        
+        `auto_timeseries` is a complex model building utility for time series data. Since it automates many
+        Tasks involved in a complex endeavor, it assumes many intelligent defaults. But you can change them.
+        Auto_Timeseries will rapidly build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet
+        and Scikit-Learn ML. It will automatically select the best model which gives best score specified.
+        
+        # Table of Contents
+        <ul>
+        <li><a href="#Latest">Latest updates</a></li>
+        <li><a href="#introduction">What is auto_ts</a></li>
+        <li><a href="#install">How to install auto_ts</a></li>
+        <li><a href="#usage">Usage</a></li>
+        <li><a href="#requirements">Requirements</a></li>
+        <li><a href="#tips">Tips</a></li>
+        <li><a href="#license">License</a></li>
+        <li><a href="#copyright">Copyright</a></li>
+        <li><a href="#disclaimer">Disclaimer</a></li>
+        </ul>
+        
+        ## Latest
+        To know about the latest updates and features added to Auto_TS please go to this [page](updates.md).
+        
+        <h2 id="introduction">Introduction</h2>
+        <p>Auto_TimeSeries enables you to build and select multiple time series models using techniques such as ARIMA, SARIMAX, VAR, decomposable (trend+seasonality+holidays) models, and ensemble machine learning models.</p>
+        <p>Auto_TimeSeries is an Automated ML library for time series data. Auto_TimeSeries was initially conceived and developed by <a href="https://www.linkedin.com/in/ram-seshadri-nyc-nj/">Ram Seshadri</a> and was significantly expanded in functionality and scope and upgraded to its present status by <a href="https://github.com/ngupta23">Nikhil Gupta</a>.</p>
+        <p>auto-ts.Auto_TimeSeries is the main function that you will call with your train data. You can then choose what kind of models you want: stats, ml or Prophet based model. You can also tell it to automatically select the best model based on the scoring parameter you want it to be based on. It will return the best model and a dictionary containing predictions for the number of forecast_periods you mentioned (default=2).
+        
+        ## Install
+        
+        ```
+        pip install auto-ts
+        ```
+        
+        Use `pip3 install auto-ts` if the above doesn’t work
+        
+        ```
+        pip install git+https://github.com/AutoViML/Auto_TS.git
+        ```
+        
+        ### Installing on Colab 
+        If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise you will get an error!):
         
         ```
         !pip install auto-ts --no-deps --ignore-installed
         !pip install 'fsspec>=0.3.3'
         !pip install statsmodels --upgrade
         !pip install pmdarima
         ```
         
-        <h1 id="aug-update">Aug 2022 Update:</h1>
-        <p style="font-family:verdana">You can now add FB Prophet arguments directly into Auto_TimeSeries using the kwargs argument. See example below:
-        
-        ![fb-prophet](add_fb_prophet.png)
+        ![auto_ts_colab](images/install_auto_ts.png)
         
-        <h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
-        <p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.</p>
-        <p>Auto_timeseries is a complex model building utility for time series data. Since it automates many
-        Tasks involved in a complex endeavor, it assumes many intelligent defaults. But you can change them.
-        Auto_Timeseries will rapidly build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet
-        and Scikit-Learn ML. It will automatically select the best model which gives best score specified.
-        </p>
-        <p>New version 0.0.35 onwards has major updates: You can now load your file into Dask dataframes. Just provide the name of your file and if it is too large to fit into a pandas dataframe, Auto_TS will automatically detect and load it into a Dask dataframe. </p>
-        <p>Also, new since version 0.0.25 is the syntax of Auto_TimeSerie: It is now more like scikit-learn (with fit and predict). You will have to initialize an object and then call fit with your data and then predict again with data. Hope this makes it easier to remember and use.</p>
-        <h2 id="introduction">Introduction</h2>
-        <p>Auto_TimeSeries enables you to build and select multiple time series models using techniques such as ARIMA, SARIMAX, VAR, decomposable (trend+seasonality+holidays) models, and ensemble machine learning models.</p>
-        <p>Auto_TimeSeries is an Automated ML library for time series data. Auto_TimeSeries was initially conceived and developed by <a href="https://www.linkedin.com/in/ram-seshadri-nyc-nj/">Ram Seshadri</a> and was significantly expanded in functionality and scope and upgraded to its present status by <a href="https://github.com/ngupta23">Nikhil Gupta</a>.</p>
-        <p>auto-ts.Auto_TimeSeries is the main function that you will call with your train data. You can then choose what kind of models you want: stats, ml or Prophet based model. You can also tell it to automatically select the best model based on the scoring parameter you want it to be based on. It will return the best model and a dictionary containing predictions for the number of forecast_periods you mentioned (default=2).</p>
-        <h2 id="installation-instructions">INSTALLATION INSTRUCTIONS</h2>
-        <ol>
-        <li>Use “pip install auto-ts”</li>
-        <li>Use “pip3 install auto-ts” if the above doesn’t work</li>
-        <li>pip install git+git://github.com/AutoViML/Auto_TS</li>
-        </ol>
-        <h4>Note for Windows Users</h4>
+        ### Installing on Windows
         <p>Windows users may experience difficulties with the Prophet and pystan dependency installations.  Because of this, we recommend installing Prophet using instructions from the <a hreff="https://facebook.github.io/prophet/docs/installation.html"> Prophet documentation page</a> prior to installing auto-ts.  For Anaconda users, this can be accomplished via:
         <ol>
         <li><p><code> conda install -c conda-forge prophet </code> </p></li>
         <li><p><code> pip install auto-ts </code> </p></li>
         </ol>
         
-        <h2 id="run">RUN</h2>
-        <p> First you need to import auto_timeseries from auto_ts library:<br>
-        <code>
+        <h2 id="usage">Usage</h2>
+        
+        ### First you need to import auto_timeseries from auto_ts library:<br>
+        
+        ```
         from auto_ts import auto_timeseries
-        </code>
-        </p>
-        <p>
-        Second, Initialize an auto_timeseries model object which will hold all your parameters:</p>
-        <p><code>
+        ```
+        
+        ### Second, Initialize an auto_timeseries model object which will hold all your parameters:</p>
+        
+        ```
         model = auto_timeseries(
                     score_type='rmse',
                     time_interval='Month',
                     non_seasonal_pdq=None, seasonality=False,
                     seasonal_period=12,
                     model_type=['Prophet'],
                     verbose=2)
-        </code></p>
-        Here are how the input parameters defined:<br>
+        ```
+        
+        #### Here are how the input parameters defined:<br>
         <ol>
         <li><b>score_type (default='rmse')</b>: The metric used for scoring the models. Type is string.
         Currently only the following two types are supported:
         (1) "rmse": Root Mean Squared Error (RMSE)
         (2) "normalized_rmse": Ratio of RMSE to the standard deviation of actuals</li>
         <li><b>time_interval (default is None)</b>: Used to indicate the frequency at which the data is collected.
         This is used for two purposes (1) in building the Prophet model and (2) used to impute the seasonal period for SARIMAX in case it is not provided by the user (None). Type is String.
@@ -127,71 +142,75 @@
         If a list is provided, then only those models will be built
         WARNING: "best" might take some time for large data sets. We recommend that you
         choose a small sample from your data set before attempting to run entire data.
         Type can be either: [string, list]
         </li>
         <li><b>verbose (default=0)</b>: Indicates the verbosity of printing (Default = 0). Type is integer.</li>
         </ol>
-        The next step after defining the model object is to fit it with some real data:
-        <p><code><br>
+        
+        ### The next step after defining the model object is to fit it with some real data:
+        
+        ```
         model.fit(
                     traindata=train_data,
                     ts_column=ts_column,
                     target=target,
                     cv=5,
                     sep=","
                 )
-        </code></p>
-        <br>Here are how the parameters defined:
+        ```
+        
+        Here are how the parameters defined:
         <ul>
         <li><b>traindata (required)</b>: It can be either a dataframe or a file. You must give the name of the file along with its data path in case if a file. It also accepts a pandas dataframe in case you already have a dataframe loaded in your notebook.</li>
         <li><b>ts_column (required)</b>: name of the datetime column in your dataset (it could be a name of column or index number in the columns index)</li>
         <li><b>target (required)</b>: name of the column you   are trying to predict. Target could also be the only column in your dataset</li>
         <li><b>cv (default=5)</b>: You can enter any integer for the number of folds you want in your cross validation data set.
         </li>
         <li><b>sep (default=",")</b>: Sep is the separator in your traindata file. If your separator is ",", "\t", ";", make sure you enter it here. If not, it is ignored.</li>
         </ul>
-        The next step after training the model object is to make some predictions with test data:<br>
-        <p><code><br>
+        
+        ### The next step after training the model object is to make some predictions with test data:<br>
+        
+        ```
         predictions = model.predict(
                     testdata = can be either a dataframe or an integer standing for the forecast_period,
                     model = 'best' or any other string that stands for the trained model
                 )  
-        </code></p>
+        ```
+        
         Here are how the parameters are defined. You can choose to send either testdata in the form of a dataframe or send in an integer to decide how many periods you want to forecast.  You need only
         <ul>
         <li><b>testdata (required)</b>: It can be either a dataframe containing test data or you can use an integer standing for the forecast_period (you want).</li>
         <li><b>model (optional, default = 'best')</b>: The name of the model you want to use among the many different models you have trained. Remember that the default is the best model. But you can choose any model that you want to forecast with. Type is String.</li>
         </ul>
+        
         <h2 id="requirements">Requirements</h2>
-        <p>dask</p>
-        <p>scikit-learn</p>
-        <p>Prophet</p>
-        <p>statsmodels</p>
-        <p>pmdarima</p>
-        <p>XGBoost</p>
-        <h1 id="license">License:</h1>
+        <p>dask, scikit-learn, prophet, statsmodels, pmdarima, XGBoost</p>
+        
+        <h2 id="license">License:</h2>
         <p>Apache License 2.0</p>
-        <h2 id="recommendations">Recommendations</h2>
+        
+        <h2 id="Tips">Tips</h2>
         <ul>
         <li>We recommend that you choose a small sample from your data set before attempting to run entire data. and the evaluation metric so it can select the best model. Currently models within “stats” are compared using AIC and BIC. However, models across different types are compared using RMSE. The results of models are shown using RMSE and Normalized RMSE (ratio of RMSE to the standard deviation of actuals).</li>
         <li>You must clean the data and not have any missing values. Make sure the target variable is numeric, otherwise, it won’t run. If there is more than one target variable in your data set, just specify only one for now, and if you know the time interval that is in your data, you can specify it. Otherwise it auto-ts will try to infer the time interval on its own.</li>
         <li>If you give Auto_Timeseries a different time interval than what the data has, it will automatically resample the data to the given time interval and use the mean of the target for the resampled period.</li>
         <li>Notice that except for filename and ts_column input arguments, which are required, all other arguments are optional.</li>
         <li>Note that optionally you can give a separator for the data in your file. Default is comma (",").</li>
         <li>“time_interval” options are any codes that you can find in this page below.
         <a href="https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#timeseries-offset-aliases">Pandas date-range frequency aliases</a>
         </li>
         <li>Optionally, you can give seasonal_period as any integer that measures the seasonality in the data. If not given, seasonal_period is assumed automatically as follows: Months = 12, Days = 30, Weeks = 52, Qtr = 4, Year = 1, Hours = 24, Minutes = 60 and Seconds = 60.</li>
         <li>If you want to give your own non-seasonal order, please input it as non_seasonal_pdq and for seasonal order, use seasonal_PDQ as the input. Use tuples. For example, seasonal_PDQ = (2,1,2) and non_seasonal_pdq = (0,0,3). It will accept only tuples. The default is None and Auto_Timeseries will automatically search for the best p,d,q (for Non Seasonal) and P, D, Q (for Seasonal) orders by searching for all parameters from 0 to 12 for each value of p,d,q and 0-3 for each P, Q and 0-1 for D.</li>
         </ul>
+        
         <h2 id="disclaimer">DISCLAIMER:</h2>
         <p>This is not an Officially supported Google project.</p>
+        
         <h2 id="copyright">Copyright</h2>
         <p>© Google</p>
-        </body>
-        </html>
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,73 +1,65 @@
-Metadata-Version: 2.1 Name: auto_ts Version: 0.0.70 Summary: Automatically
+Metadata-Version: 2.1 Name: auto_ts Version: 0.0.71 Summary: Automatically
 Build Multiple Time Series models fast - now with Facebook Prophet! Home-page:
 https://github.com/AutoViML/Auto_TS Author: Ram Seshadri License: Apache
 License 2.0 Description:
-![auto-ts](logo.png)
-****** March 2023 Update: ******
-We have now upgraded FB Prophet to the latest version which is simply called
-prophet.
-If you are using Colab or Kaggle kernel and want to install auto_ts, please use
-the following steps (otherwise error!): ``` !pip install auto-ts --no-deps --
-ignore-installed !pip install 'fsspec>=0.3.3' !pip install statsmodels --
-upgrade !pip install pmdarima ```
-****** Aug 2022 Update: ******
-You can now add FB Prophet arguments directly into Auto_TimeSeries using the
-kwargs argument. See example below: ![fb-prophet](add_fb_prophet.png)
 ****** Auto_TS: Auto_TimeSeries ******
 Automatically build multiple Time Series models using a Single Line of Code.
-Now updated with Dask.
-Auto_timeseries is a complex model building utility for time series data. Since
-it automates many Tasks involved in a complex endeavor, it assumes many
-intelligent defaults. But you can change them. Auto_Timeseries will rapidly
-build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet and
-Scikit-Learn ML. It will automatically select the best model which gives best
-score specified.
-New version 0.0.35 onwards has major updates: You can now load your file into
-Dask dataframes. Just provide the name of your file and if it is too large to
-fit into a pandas dataframe, Auto_TS will automatically detect and load it into
-a Dask dataframe.
-Also, new since version 0.0.25 is the syntax of Auto_TimeSerie: It is now more
-like scikit-learn (with fit and predict). You will have to initialize an object
-and then call fit with your data and then predict again with data. Hope this
-makes it easier to remember and use.
+Now updated with Dask. ![auto-ts](images/logo.png) `auto_timeseries` is a
+complex model building utility for time series data. Since it automates many
+Tasks involved in a complex endeavor, it assumes many intelligent defaults. But
+you can change them. Auto_Timeseries will rapidly build predictive models based
+on Statsmodels ARIMA, Seasonal ARIMA, Prophet and Scikit-Learn ML. It will
+automatically select the best model which gives best score specified. # Table
+of Contents
+    * Latest_updates
+    * What_is_auto_ts
+    * How_to_install_auto_ts
+    * Usage
+    * Requirements
+    * Tips
+    * License
+    * Copyright
+    * Disclaimer
+## Latest To know about the latest updates and features added to Auto_TS please
+go to this [page](updates.md).
 ***** Introduction *****
 Auto_TimeSeries enables you to build and select multiple time series models
 using techniques such as ARIMA, SARIMAX, VAR, decomposable
 (trend+seasonality+holidays) models, and ensemble machine learning models.
 Auto_TimeSeries is an Automated ML library for time series data.
 Auto_TimeSeries was initially conceived and developed by Ram_Seshadri and was
 significantly expanded in functionality and scope and upgraded to its present
 status by Nikhil_Gupta.
 auto-ts.Auto_TimeSeries is the main function that you will call with your train
 data. You can then choose what kind of models you want: stats, ml or Prophet
 based model. You can also tell it to automatically select the best model based
 on the scoring parameter you want it to be based on. It will return the best
 model and a dictionary containing predictions for the number of
-forecast_periods you mentioned (default=2).
-***** INSTALLATION INSTRUCTIONS *****
-   1. Use âpip install auto-tsâ
-   2. Use âpip3 install auto-tsâ if the above doesnât work
-   3. pip install git+git://github.com/AutoViML/Auto_TS
-*** Note for Windows Users ***
+forecast_periods you mentioned (default=2). ## Install ``` pip install auto-ts
+``` Use `pip3 install auto-ts` if the above doesnât work ``` pip install
+git+https://github.com/AutoViML/Auto_TS.git ``` ### Installing on Colab If you
+are using Colab or Kaggle kernel and want to install auto_ts, please use the
+following steps (otherwise you will get an error!): ``` !pip install auto-ts --
+no-deps --ignore-installed !pip install 'fsspec>=0.3.3' !pip install
+statsmodels --upgrade !pip install pmdarima ``` ![auto_ts_colab](images/
+install_auto_ts.png) ### Installing on Windows
 Windows users may experience difficulties with the Prophet and pystan
 dependency installations. Because of this, we recommend installing Prophet
 using instructions from the Prophet documentation page prior to installing
 auto-ts. For Anaconda users, this can be accomplished via:
    1. conda install -c conda-forge prophet
    2. pip install auto-ts
-***** RUN *****
-First you need to import auto_timeseries from auto_ts library:
-from auto_ts import auto_timeseries
-Second, Initialize an auto_timeseries model object which will hold all your
-parameters:
-model = auto_timeseries( score_type='rmse', time_interval='Month',
+***** Usage *****
+### First you need to import auto_timeseries from auto_ts library:
+``` from auto_ts import auto_timeseries ``` ### Second, Initialize an
+auto_timeseries model object which will hold all your parameters:
+``` model = auto_timeseries( score_type='rmse', time_interval='Month',
 non_seasonal_pdq=None, seasonality=False, seasonal_period=12, model_type=
-['Prophet'], verbose=2)
-Here are how the input parameters defined:
+['Prophet'], verbose=2) ``` #### Here are how the input parameters defined:
    1. score_type (default='rmse'): The metric used for scoring the models. Type
       is string. Currently only the following two types are supported: (1)
       "rmse": Root Mean Squared Error (RMSE) (2) "normalized_rmse": Ratio of
       RMSE to the standard deviation of actuals
    2. time_interval (default is None): Used to indicate the frequency at which
       the data is collected. This is used for two purposes (1) in building the
       Prophet model and (2) used to impute the seasonal period for SARIMAX in
@@ -123,58 +115,49 @@
       Random Forests provided explanatory vars are given 'best' will try to
       build all models and pick the best one If a list is provided, then only
       those models will be built WARNING: "best" might take some time for large
       data sets. We recommend that you choose a small sample from your data set
       before attempting to run entire data. Type can be either: [string, list]
    8. verbose (default=0): Indicates the verbosity of printing (Default = 0).
       Type is integer.
-The next step after defining the model object is to fit it with some real data:
-
-model.fit( traindata=train_data, ts_column=ts_column, target=target, cv=5,
-sep="," )
-
-Here are how the parameters defined:
+### The next step after defining the model object is to fit it with some real
+data: ``` model.fit( traindata=train_data, ts_column=ts_column, target=target,
+cv=5, sep="," ) ``` Here are how the parameters defined:
     * traindata (required): It can be either a dataframe or a file. You must
       give the name of the file along with its data path in case if a file. It
       also accepts a pandas dataframe in case you already have a dataframe
       loaded in your notebook.
     * ts_column (required): name of the datetime column in your dataset (it
       could be a name of column or index number in the columns index)
     * target (required): name of the column you are trying to predict. Target
       could also be the only column in your dataset
     * cv (default=5): You can enter any integer for the number of folds you
       want in your cross validation data set.
     * sep (default=","): Sep is the separator in your traindata file. If your
       separator is ",", "\t", ";", make sure you enter it here. If not, it is
       ignored.
-The next step after training the model object is to make some predictions with
-test data:
-
-predictions = model.predict( testdata = can be either a dataframe or an integer
-standing for the forecast_period, model = 'best' or any other string that
-stands for the trained model )
-Here are how the parameters are defined. You can choose to send either testdata
-in the form of a dataframe or send in an integer to decide how many periods you
-want to forecast. You need only
+### The next step after training the model object is to make some predictions
+with test data:
+``` predictions = model.predict( testdata = can be either a dataframe or an
+integer standing for the forecast_period, model = 'best' or any other string
+that stands for the trained model ) ``` Here are how the parameters are
+defined. You can choose to send either testdata in the form of a dataframe or
+send in an integer to decide how many periods you want to forecast. You need
+only
     * testdata (required): It can be either a dataframe containing test data or
       you can use an integer standing for the forecast_period (you want).
     * model (optional, default = 'best'): The name of the model you want to use
       among the many different models you have trained. Remember that the
       default is the best model. But you can choose any model that you want to
       forecast with. Type is String.
 ***** Requirements *****
-dask
-scikit-learn
-Prophet
-statsmodels
-pmdarima
-XGBoost
-****** License: ******
+dask, scikit-learn, prophet, statsmodels, pmdarima, XGBoost
+***** License: *****
 Apache License 2.0
-***** Recommendations *****
+***** Tips *****
     * We recommend that you choose a small sample from your data set before
       attempting to run entire data. and the evaluation metric so it can select
       the best model. Currently models within âstatsâ are compared using
       AIC and BIC. However, models across different types are compared using
       RMSE. The results of models are shown using RMSE and Normalized RMSE
       (ratio of RMSE to the standard deviation of actuals).
     * You must clean the data and not have any missing values. Make sure the
```

### Comparing `auto_ts-0.0.70/README.md` & `auto_ts-0.0.71/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,75 +1,90 @@
-<!DOCTYPE html>
-<html>
-<head>
-</head>
-<body>
-
-![auto-ts](logo.png)
-
-<h1 id="mar-update">March 2023 Update:</h1>
-<p style="font-family:verdana">We have now upgraded FB Prophet to the latest version which is simply called prophet. <br>
-If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise error!):
+<h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
+<p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.
+
+![auto-ts](images/logo.png)
+
+`auto_timeseries` is a complex model building utility for time series data. Since it automates many
+Tasks involved in a complex endeavor, it assumes many intelligent defaults. But you can change them.
+Auto_Timeseries will rapidly build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet
+and Scikit-Learn ML. It will automatically select the best model which gives best score specified.
+
+# Table of Contents
+<ul>
+<li><a href="#Latest">Latest updates</a></li>
+<li><a href="#introduction">What is auto_ts</a></li>
+<li><a href="#install">How to install auto_ts</a></li>
+<li><a href="#usage">Usage</a></li>
+<li><a href="#requirements">Requirements</a></li>
+<li><a href="#tips">Tips</a></li>
+<li><a href="#license">License</a></li>
+<li><a href="#copyright">Copyright</a></li>
+<li><a href="#disclaimer">Disclaimer</a></li>
+</ul>
+
+## Latest
+To know about the latest updates and features added to Auto_TS please go to this [page](updates.md).
+
+<h2 id="introduction">Introduction</h2>
+<p>Auto_TimeSeries enables you to build and select multiple time series models using techniques such as ARIMA, SARIMAX, VAR, decomposable (trend+seasonality+holidays) models, and ensemble machine learning models.</p>
+<p>Auto_TimeSeries is an Automated ML library for time series data. Auto_TimeSeries was initially conceived and developed by <a href="https://www.linkedin.com/in/ram-seshadri-nyc-nj/">Ram Seshadri</a> and was significantly expanded in functionality and scope and upgraded to its present status by <a href="https://github.com/ngupta23">Nikhil Gupta</a>.</p>
+<p>auto-ts.Auto_TimeSeries is the main function that you will call with your train data. You can then choose what kind of models you want: stats, ml or Prophet based model. You can also tell it to automatically select the best model based on the scoring parameter you want it to be based on. It will return the best model and a dictionary containing predictions for the number of forecast_periods you mentioned (default=2).
+
+## Install
+
+```
+pip install auto-ts
+```
+
+Use `pip3 install auto-ts` if the above doesn’t work
+
+```
+pip install git+https://github.com/AutoViML/Auto_TS.git
+```
+
+### Installing on Colab 
+If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise you will get an error!):
 
 ```
 !pip install auto-ts --no-deps --ignore-installed
 !pip install 'fsspec>=0.3.3'
 !pip install statsmodels --upgrade
 !pip install pmdarima
 ```
 
-<h1 id="aug-update">Aug 2022 Update:</h1>
-<p style="font-family:verdana">You can now add FB Prophet arguments directly into Auto_TimeSeries using the kwargs argument. See example below:
-
-![fb-prophet](add_fb_prophet.png)
+![auto_ts_colab](images/install_auto_ts.png)
 
-<h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
-<p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.</p>
-<p>Auto_timeseries is a complex model building utility for time series data. Since it automates many
-Tasks involved in a complex endeavor, it assumes many intelligent defaults. But you can change them.
-Auto_Timeseries will rapidly build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet
-and Scikit-Learn ML. It will automatically select the best model which gives best score specified.
-</p>
-<p>New version 0.0.35 onwards has major updates: You can now load your file into Dask dataframes. Just provide the name of your file and if it is too large to fit into a pandas dataframe, Auto_TS will automatically detect and load it into a Dask dataframe. </p>
-<p>Also, new since version 0.0.25 is the syntax of Auto_TimeSerie: It is now more like scikit-learn (with fit and predict). You will have to initialize an object and then call fit with your data and then predict again with data. Hope this makes it easier to remember and use.</p>
-<h2 id="introduction">Introduction</h2>
-<p>Auto_TimeSeries enables you to build and select multiple time series models using techniques such as ARIMA, SARIMAX, VAR, decomposable (trend+seasonality+holidays) models, and ensemble machine learning models.</p>
-<p>Auto_TimeSeries is an Automated ML library for time series data. Auto_TimeSeries was initially conceived and developed by <a href="https://www.linkedin.com/in/ram-seshadri-nyc-nj/">Ram Seshadri</a> and was significantly expanded in functionality and scope and upgraded to its present status by <a href="https://github.com/ngupta23">Nikhil Gupta</a>.</p>
-<p>auto-ts.Auto_TimeSeries is the main function that you will call with your train data. You can then choose what kind of models you want: stats, ml or Prophet based model. You can also tell it to automatically select the best model based on the scoring parameter you want it to be based on. It will return the best model and a dictionary containing predictions for the number of forecast_periods you mentioned (default=2).</p>
-<h2 id="installation-instructions">INSTALLATION INSTRUCTIONS</h2>
-<ol>
-<li>Use “pip install auto-ts”</li>
-<li>Use “pip3 install auto-ts” if the above doesn’t work</li>
-<li>pip install git+git://github.com/AutoViML/Auto_TS</li>
-</ol>
-<h4>Note for Windows Users</h4>
+### Installing on Windows
 <p>Windows users may experience difficulties with the Prophet and pystan dependency installations.  Because of this, we recommend installing Prophet using instructions from the <a hreff="https://facebook.github.io/prophet/docs/installation.html"> Prophet documentation page</a> prior to installing auto-ts.  For Anaconda users, this can be accomplished via:
 <ol>
 <li><p><code> conda install -c conda-forge prophet </code> </p></li>
 <li><p><code> pip install auto-ts </code> </p></li>
 </ol>
 
-<h2 id="run">RUN</h2>
-<p> First you need to import auto_timeseries from auto_ts library:<br>
-<code>
+<h2 id="usage">Usage</h2>
+
+### First you need to import auto_timeseries from auto_ts library:<br>
+
+```
 from auto_ts import auto_timeseries
-</code>
-</p>
-<p>
-Second, Initialize an auto_timeseries model object which will hold all your parameters:</p>
-<p><code>
+```
+
+### Second, Initialize an auto_timeseries model object which will hold all your parameters:</p>
+
+```
 model = auto_timeseries(
             score_type='rmse',
             time_interval='Month',
             non_seasonal_pdq=None, seasonality=False,
             seasonal_period=12,
             model_type=['Prophet'],
             verbose=2)
-</code></p>
-Here are how the input parameters defined:<br>
+```
+
+#### Here are how the input parameters defined:<br>
 <ol>
 <li><b>score_type (default='rmse')</b>: The metric used for scoring the models. Type is string.
 Currently only the following two types are supported:
 (1) "rmse": Root Mean Squared Error (RMSE)
 (2) "normalized_rmse": Ratio of RMSE to the standard deviation of actuals</li>
 <li><b>time_interval (default is None)</b>: Used to indicate the frequency at which the data is collected.
 This is used for two purposes (1) in building the Prophet model and (2) used to impute the seasonal period for SARIMAX in case it is not provided by the user (None). Type is String.
@@ -120,66 +135,70 @@
 If a list is provided, then only those models will be built
 WARNING: "best" might take some time for large data sets. We recommend that you
 choose a small sample from your data set before attempting to run entire data.
 Type can be either: [string, list]
 </li>
 <li><b>verbose (default=0)</b>: Indicates the verbosity of printing (Default = 0). Type is integer.</li>
 </ol>
-The next step after defining the model object is to fit it with some real data:
-<p><code><br>
+
+### The next step after defining the model object is to fit it with some real data:
+
+```
 model.fit(
             traindata=train_data,
             ts_column=ts_column,
             target=target,
             cv=5,
             sep=","
         )
-</code></p>
-<br>Here are how the parameters defined:
+```
+
+Here are how the parameters defined:
 <ul>
 <li><b>traindata (required)</b>: It can be either a dataframe or a file. You must give the name of the file along with its data path in case if a file. It also accepts a pandas dataframe in case you already have a dataframe loaded in your notebook.</li>
 <li><b>ts_column (required)</b>: name of the datetime column in your dataset (it could be a name of column or index number in the columns index)</li>
 <li><b>target (required)</b>: name of the column you   are trying to predict. Target could also be the only column in your dataset</li>
 <li><b>cv (default=5)</b>: You can enter any integer for the number of folds you want in your cross validation data set.
 </li>
 <li><b>sep (default=",")</b>: Sep is the separator in your traindata file. If your separator is ",", "\t", ";", make sure you enter it here. If not, it is ignored.</li>
 </ul>
-The next step after training the model object is to make some predictions with test data:<br>
-<p><code><br>
+
+### The next step after training the model object is to make some predictions with test data:<br>
+
+```
 predictions = model.predict(
             testdata = can be either a dataframe or an integer standing for the forecast_period,
             model = 'best' or any other string that stands for the trained model
         )  
-</code></p>
+```
+
 Here are how the parameters are defined. You can choose to send either testdata in the form of a dataframe or send in an integer to decide how many periods you want to forecast.  You need only
 <ul>
 <li><b>testdata (required)</b>: It can be either a dataframe containing test data or you can use an integer standing for the forecast_period (you want).</li>
 <li><b>model (optional, default = 'best')</b>: The name of the model you want to use among the many different models you have trained. Remember that the default is the best model. But you can choose any model that you want to forecast with. Type is String.</li>
 </ul>
+
 <h2 id="requirements">Requirements</h2>
-<p>dask</p>
-<p>scikit-learn</p>
-<p>Prophet</p>
-<p>statsmodels</p>
-<p>pmdarima</p>
-<p>XGBoost</p>
-<h1 id="license">License:</h1>
+<p>dask, scikit-learn, prophet, statsmodels, pmdarima, XGBoost</p>
+
+<h2 id="license">License:</h2>
 <p>Apache License 2.0</p>
-<h2 id="recommendations">Recommendations</h2>
+
+<h2 id="Tips">Tips</h2>
 <ul>
 <li>We recommend that you choose a small sample from your data set before attempting to run entire data. and the evaluation metric so it can select the best model. Currently models within “stats” are compared using AIC and BIC. However, models across different types are compared using RMSE. The results of models are shown using RMSE and Normalized RMSE (ratio of RMSE to the standard deviation of actuals).</li>
 <li>You must clean the data and not have any missing values. Make sure the target variable is numeric, otherwise, it won’t run. If there is more than one target variable in your data set, just specify only one for now, and if you know the time interval that is in your data, you can specify it. Otherwise it auto-ts will try to infer the time interval on its own.</li>
 <li>If you give Auto_Timeseries a different time interval than what the data has, it will automatically resample the data to the given time interval and use the mean of the target for the resampled period.</li>
 <li>Notice that except for filename and ts_column input arguments, which are required, all other arguments are optional.</li>
 <li>Note that optionally you can give a separator for the data in your file. Default is comma (",").</li>
 <li>“time_interval” options are any codes that you can find in this page below.
 <a href="https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#timeseries-offset-aliases">Pandas date-range frequency aliases</a>
 </li>
 <li>Optionally, you can give seasonal_period as any integer that measures the seasonality in the data. If not given, seasonal_period is assumed automatically as follows: Months = 12, Days = 30, Weeks = 52, Qtr = 4, Year = 1, Hours = 24, Minutes = 60 and Seconds = 60.</li>
 <li>If you want to give your own non-seasonal order, please input it as non_seasonal_pdq and for seasonal order, use seasonal_PDQ as the input. Use tuples. For example, seasonal_PDQ = (2,1,2) and non_seasonal_pdq = (0,0,3). It will accept only tuples. The default is None and Auto_Timeseries will automatically search for the best p,d,q (for Non Seasonal) and P, D, Q (for Seasonal) orders by searching for all parameters from 0 to 12 for each value of p,d,q and 0-3 for each P, Q and 0-1 for D.</li>
 </ul>
+
 <h2 id="disclaimer">DISCLAIMER:</h2>
 <p>This is not an Officially supported Google project.</p>
+
 <h2 id="copyright">Copyright</h2>
 <p>© Google</p>
-</body>
-</html>
```

#### html2text {}

```diff
@@ -1,69 +1,61 @@
-![auto-ts](logo.png)
-****** March 2023 Update: ******
-We have now upgraded FB Prophet to the latest version which is simply called
-prophet.
-If you are using Colab or Kaggle kernel and want to install auto_ts, please use
-the following steps (otherwise error!): ``` !pip install auto-ts --no-deps --
-ignore-installed !pip install 'fsspec>=0.3.3' !pip install statsmodels --
-upgrade !pip install pmdarima ```
-****** Aug 2022 Update: ******
-You can now add FB Prophet arguments directly into Auto_TimeSeries using the
-kwargs argument. See example below: ![fb-prophet](add_fb_prophet.png)
 ****** Auto_TS: Auto_TimeSeries ******
 Automatically build multiple Time Series models using a Single Line of Code.
-Now updated with Dask.
-Auto_timeseries is a complex model building utility for time series data. Since
-it automates many Tasks involved in a complex endeavor, it assumes many
-intelligent defaults. But you can change them. Auto_Timeseries will rapidly
-build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet and
-Scikit-Learn ML. It will automatically select the best model which gives best
-score specified.
-New version 0.0.35 onwards has major updates: You can now load your file into
-Dask dataframes. Just provide the name of your file and if it is too large to
-fit into a pandas dataframe, Auto_TS will automatically detect and load it into
-a Dask dataframe.
-Also, new since version 0.0.25 is the syntax of Auto_TimeSerie: It is now more
-like scikit-learn (with fit and predict). You will have to initialize an object
-and then call fit with your data and then predict again with data. Hope this
-makes it easier to remember and use.
+Now updated with Dask. ![auto-ts](images/logo.png) `auto_timeseries` is a
+complex model building utility for time series data. Since it automates many
+Tasks involved in a complex endeavor, it assumes many intelligent defaults. But
+you can change them. Auto_Timeseries will rapidly build predictive models based
+on Statsmodels ARIMA, Seasonal ARIMA, Prophet and Scikit-Learn ML. It will
+automatically select the best model which gives best score specified. # Table
+of Contents
+    * Latest_updates
+    * What_is_auto_ts
+    * How_to_install_auto_ts
+    * Usage
+    * Requirements
+    * Tips
+    * License
+    * Copyright
+    * Disclaimer
+## Latest To know about the latest updates and features added to Auto_TS please
+go to this [page](updates.md).
 ***** Introduction *****
 Auto_TimeSeries enables you to build and select multiple time series models
 using techniques such as ARIMA, SARIMAX, VAR, decomposable
 (trend+seasonality+holidays) models, and ensemble machine learning models.
 Auto_TimeSeries is an Automated ML library for time series data.
 Auto_TimeSeries was initially conceived and developed by Ram_Seshadri and was
 significantly expanded in functionality and scope and upgraded to its present
 status by Nikhil_Gupta.
 auto-ts.Auto_TimeSeries is the main function that you will call with your train
 data. You can then choose what kind of models you want: stats, ml or Prophet
 based model. You can also tell it to automatically select the best model based
 on the scoring parameter you want it to be based on. It will return the best
 model and a dictionary containing predictions for the number of
-forecast_periods you mentioned (default=2).
-***** INSTALLATION INSTRUCTIONS *****
-   1. Use âpip install auto-tsâ
-   2. Use âpip3 install auto-tsâ if the above doesnât work
-   3. pip install git+git://github.com/AutoViML/Auto_TS
-*** Note for Windows Users ***
+forecast_periods you mentioned (default=2). ## Install ``` pip install auto-ts
+``` Use `pip3 install auto-ts` if the above doesnât work ``` pip install
+git+https://github.com/AutoViML/Auto_TS.git ``` ### Installing on Colab If you
+are using Colab or Kaggle kernel and want to install auto_ts, please use the
+following steps (otherwise you will get an error!): ``` !pip install auto-ts --
+no-deps --ignore-installed !pip install 'fsspec>=0.3.3' !pip install
+statsmodels --upgrade !pip install pmdarima ``` ![auto_ts_colab](images/
+install_auto_ts.png) ### Installing on Windows
 Windows users may experience difficulties with the Prophet and pystan
 dependency installations. Because of this, we recommend installing Prophet
 using instructions from the Prophet documentation page prior to installing
 auto-ts. For Anaconda users, this can be accomplished via:
    1. conda install -c conda-forge prophet
    2. pip install auto-ts
-***** RUN *****
-First you need to import auto_timeseries from auto_ts library:
-from auto_ts import auto_timeseries
-Second, Initialize an auto_timeseries model object which will hold all your
-parameters:
-model = auto_timeseries( score_type='rmse', time_interval='Month',
+***** Usage *****
+### First you need to import auto_timeseries from auto_ts library:
+``` from auto_ts import auto_timeseries ``` ### Second, Initialize an
+auto_timeseries model object which will hold all your parameters:
+``` model = auto_timeseries( score_type='rmse', time_interval='Month',
 non_seasonal_pdq=None, seasonality=False, seasonal_period=12, model_type=
-['Prophet'], verbose=2)
-Here are how the input parameters defined:
+['Prophet'], verbose=2) ``` #### Here are how the input parameters defined:
    1. score_type (default='rmse'): The metric used for scoring the models. Type
       is string. Currently only the following two types are supported: (1)
       "rmse": Root Mean Squared Error (RMSE) (2) "normalized_rmse": Ratio of
       RMSE to the standard deviation of actuals
    2. time_interval (default is None): Used to indicate the frequency at which
       the data is collected. This is used for two purposes (1) in building the
       Prophet model and (2) used to impute the seasonal period for SARIMAX in
@@ -119,58 +111,49 @@
       Random Forests provided explanatory vars are given 'best' will try to
       build all models and pick the best one If a list is provided, then only
       those models will be built WARNING: "best" might take some time for large
       data sets. We recommend that you choose a small sample from your data set
       before attempting to run entire data. Type can be either: [string, list]
    8. verbose (default=0): Indicates the verbosity of printing (Default = 0).
       Type is integer.
-The next step after defining the model object is to fit it with some real data:
-
-model.fit( traindata=train_data, ts_column=ts_column, target=target, cv=5,
-sep="," )
-
-Here are how the parameters defined:
+### The next step after defining the model object is to fit it with some real
+data: ``` model.fit( traindata=train_data, ts_column=ts_column, target=target,
+cv=5, sep="," ) ``` Here are how the parameters defined:
     * traindata (required): It can be either a dataframe or a file. You must
       give the name of the file along with its data path in case if a file. It
       also accepts a pandas dataframe in case you already have a dataframe
       loaded in your notebook.
     * ts_column (required): name of the datetime column in your dataset (it
       could be a name of column or index number in the columns index)
     * target (required): name of the column you are trying to predict. Target
       could also be the only column in your dataset
     * cv (default=5): You can enter any integer for the number of folds you
       want in your cross validation data set.
     * sep (default=","): Sep is the separator in your traindata file. If your
       separator is ",", "\t", ";", make sure you enter it here. If not, it is
       ignored.
-The next step after training the model object is to make some predictions with
-test data:
-
-predictions = model.predict( testdata = can be either a dataframe or an integer
-standing for the forecast_period, model = 'best' or any other string that
-stands for the trained model )
-Here are how the parameters are defined. You can choose to send either testdata
-in the form of a dataframe or send in an integer to decide how many periods you
-want to forecast. You need only
+### The next step after training the model object is to make some predictions
+with test data:
+``` predictions = model.predict( testdata = can be either a dataframe or an
+integer standing for the forecast_period, model = 'best' or any other string
+that stands for the trained model ) ``` Here are how the parameters are
+defined. You can choose to send either testdata in the form of a dataframe or
+send in an integer to decide how many periods you want to forecast. You need
+only
     * testdata (required): It can be either a dataframe containing test data or
       you can use an integer standing for the forecast_period (you want).
     * model (optional, default = 'best'): The name of the model you want to use
       among the many different models you have trained. Remember that the
       default is the best model. But you can choose any model that you want to
       forecast with. Type is String.
 ***** Requirements *****
-dask
-scikit-learn
-Prophet
-statsmodels
-pmdarima
-XGBoost
-****** License: ******
+dask, scikit-learn, prophet, statsmodels, pmdarima, XGBoost
+***** License: *****
 Apache License 2.0
-***** Recommendations *****
+***** Tips *****
     * We recommend that you choose a small sample from your data set before
       attempting to run entire data. and the evaluation metric so it can select
       the best model. Currently models within âstatsâ are compared using
       AIC and BIC. However, models across different types are compared using
       RMSE. The results of models are shown using RMSE and Normalized RMSE
       (ratio of RMSE to the standard deviation of actuals).
     * You must clean the data and not have any missing values. Make sure the
```

### Comparing `auto_ts-0.0.70/auto_ts/__init__.py` & `auto_ts-0.0.71/auto_ts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,14 +566,15 @@
                     score_val = rmse_folds
                 else:
                     score_val = norm_rmse_folds
             except Exception as e:
                 print("Exception occurred while building Prophet model...")
                 print(e)
                 print('    FB Prophet may not be installed or Model is not running...')
+                forecast_df_folds = None
 
             self.ml_dict[name]['model'] = model
             self.ml_dict[name]['forecast'] = forecast_df_folds
             self.ml_dict[name][self.score_type] = score_val
             self.ml_dict[name]['model_build'] = model_build
 
         ### Once Prophet is finished, you can put the variable back ####
```

### Comparing `auto_ts-0.0.70/auto_ts/models/ar_based/build_arima.py` & `auto_ts-0.0.71/auto_ts/models/ar_based/build_arima.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/ar_based/build_arima_base.py` & `auto_ts-0.0.71/auto_ts/models/ar_based/build_arima_base.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/ar_based/build_autoarimax.py` & `auto_ts-0.0.71/auto_ts/models/ar_based/build_autoarimax.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/ar_based/build_sarimax.py` & `auto_ts-0.0.71/auto_ts/models/ar_based/build_sarimax.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/ar_based/build_var.py` & `auto_ts-0.0.71/auto_ts/models/ar_based/build_var.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/ar_based/param_finder.py` & `auto_ts-0.0.71/auto_ts/models/ar_based/param_finder.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/build_base.py` & `auto_ts-0.0.71/auto_ts/models/build_base.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/build_ml.py` & `auto_ts-0.0.71/auto_ts/models/build_ml.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/build_prophet.py` & `auto_ts-0.0.71/auto_ts/models/build_prophet.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             for key, value in zip(kwargs.keys(),kwargs.values()):
                 if key == 'seasonality_mode':
                     self.seasonality = True
                     key = value
                 else:
                     key = value
         else:
-            self.kwargs = {'iter':1e2}
+            self.kwargs = {'iter':100}
         print('kwargs for Prophet model: %s' %self.kwargs)
         
     def fit(self, ts_df: pd.DataFrame, target_col: str, cv: Optional[int], time_col: str):
         """
         Fits the model to the data
 
         :param ts_df The time series data to be used for fitting the model
@@ -253,15 +253,15 @@
 
                 model = Prophet(growth="linear")
 
                 ############################################
                 #### Fit the model with train_fold data ####
                 ############################################
 
-                kwargs = {'iter':1e2} ## this limits iterations and hence speeds up prophet
+                kwargs = {'iter':100} ## this limits iterations and hence speeds up prophet
                 model.fit(train_fold, **kwargs)
 
                 #################################################
                 #### Predict using model with test_fold data ####
                 #################################################
                 
                 future_period = model.make_future_dataframe(freq=time_int, periods=horizon)
@@ -565,15 +565,15 @@
         train_fold = train[start_p:end_p]
         start_s += i*period
         end_s += i*period
         test_fold = train[start_s: end_s]
         if len(test_fold) == 0:
             break
         model = Prophet(growth="linear")
-        kwargs = {'iter':1e2} ## this limits iterations and hence speeds up prophet
+        kwargs = {'iter':100} ## this limits iterations and hence speeds up prophet
         model.fit(train_fold, **kwargs)
         future_period = model.make_future_dataframe(freq="MS",periods=horizon)
         forecast_df = model.predict(future_period)
         y_pred = forecast_df.iloc[start_s:end_s]['yhat']
         if i == 0:
             y_preds = copy.deepcopy(y_pred)
         else:
```

### Comparing `auto_ts-0.0.70/auto_ts/models/build_pyflux.py` & `auto_ts-0.0.71/auto_ts/models/build_pyflux.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/models/ml_models.py` & `auto_ts-0.0.71/auto_ts/models/ml_models.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/test/test_auto_sarimax.py` & `auto_ts-0.0.71/auto_ts/test/test_auto_sarimax.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/test/test_auto_ts.py` & `auto_ts-0.0.71/auto_ts/test/test_auto_ts.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/test/test_var.py` & `auto_ts-0.0.71/auto_ts/test/test_var.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/utils/__init__.py` & `auto_ts-0.0.71/auto_ts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/utils/eda.py` & `auto_ts-0.0.71/auto_ts/utils/eda.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/utils/etl.py` & `auto_ts-0.0.71/auto_ts/utils/etl.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/utils/logging.py` & `auto_ts-0.0.71/auto_ts/utils/logging.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/utils/metrics.py` & `auto_ts-0.0.71/auto_ts/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/utils/my_encoders.py` & `auto_ts-0.0.71/auto_ts/utils/my_encoders.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts/utils/val.py` & `auto_ts-0.0.71/auto_ts/utils/val.py`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/auto_ts.egg-info/PKG-INFO` & `auto_ts-0.0.71/auto_ts.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,82 +1,97 @@
 Metadata-Version: 2.1
 Name: auto-ts
-Version: 0.0.70
+Version: 0.0.71
 Summary: Automatically Build Multiple Time Series models fast - now with Facebook Prophet!
 Home-page: https://github.com/AutoViML/Auto_TS
 Author: Ram Seshadri
 License: Apache License 2.0
-Description: <!DOCTYPE html>
-        <html>
-        <head>
-        </head>
-        <body>
-        
-        ![auto-ts](logo.png)
-        
-        <h1 id="mar-update">March 2023 Update:</h1>
-        <p style="font-family:verdana">We have now upgraded FB Prophet to the latest version which is simply called prophet. <br>
-        If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise error!):
+Description: <h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
+        <p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.
+        
+        ![auto-ts](images/logo.png)
+        
+        `auto_timeseries` is a complex model building utility for time series data. Since it automates many
+        Tasks involved in a complex endeavor, it assumes many intelligent defaults. But you can change them.
+        Auto_Timeseries will rapidly build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet
+        and Scikit-Learn ML. It will automatically select the best model which gives best score specified.
+        
+        # Table of Contents
+        <ul>
+        <li><a href="#Latest">Latest updates</a></li>
+        <li><a href="#introduction">What is auto_ts</a></li>
+        <li><a href="#install">How to install auto_ts</a></li>
+        <li><a href="#usage">Usage</a></li>
+        <li><a href="#requirements">Requirements</a></li>
+        <li><a href="#tips">Tips</a></li>
+        <li><a href="#license">License</a></li>
+        <li><a href="#copyright">Copyright</a></li>
+        <li><a href="#disclaimer">Disclaimer</a></li>
+        </ul>
+        
+        ## Latest
+        To know about the latest updates and features added to Auto_TS please go to this [page](updates.md).
+        
+        <h2 id="introduction">Introduction</h2>
+        <p>Auto_TimeSeries enables you to build and select multiple time series models using techniques such as ARIMA, SARIMAX, VAR, decomposable (trend+seasonality+holidays) models, and ensemble machine learning models.</p>
+        <p>Auto_TimeSeries is an Automated ML library for time series data. Auto_TimeSeries was initially conceived and developed by <a href="https://www.linkedin.com/in/ram-seshadri-nyc-nj/">Ram Seshadri</a> and was significantly expanded in functionality and scope and upgraded to its present status by <a href="https://github.com/ngupta23">Nikhil Gupta</a>.</p>
+        <p>auto-ts.Auto_TimeSeries is the main function that you will call with your train data. You can then choose what kind of models you want: stats, ml or Prophet based model. You can also tell it to automatically select the best model based on the scoring parameter you want it to be based on. It will return the best model and a dictionary containing predictions for the number of forecast_periods you mentioned (default=2).
+        
+        ## Install
+        
+        ```
+        pip install auto-ts
+        ```
+        
+        Use `pip3 install auto-ts` if the above doesn’t work
+        
+        ```
+        pip install git+https://github.com/AutoViML/Auto_TS.git
+        ```
+        
+        ### Installing on Colab 
+        If you are using Colab or Kaggle kernel and want to install auto_ts, please use the following steps (otherwise you will get an error!):
         
         ```
         !pip install auto-ts --no-deps --ignore-installed
         !pip install 'fsspec>=0.3.3'
         !pip install statsmodels --upgrade
         !pip install pmdarima
         ```
         
-        <h1 id="aug-update">Aug 2022 Update:</h1>
-        <p style="font-family:verdana">You can now add FB Prophet arguments directly into Auto_TimeSeries using the kwargs argument. See example below:
-        
-        ![fb-prophet](add_fb_prophet.png)
+        ![auto_ts_colab](images/install_auto_ts.png)
         
-        <h1 id="auto-ts">Auto_TS: Auto_TimeSeries</h1>
-        <p style="font-family:verdana">Automatically build multiple Time Series models using a Single Line of Code. Now updated with Dask.</p>
-        <p>Auto_timeseries is a complex model building utility for time series data. Since it automates many
-        Tasks involved in a complex endeavor, it assumes many intelligent defaults. But you can change them.
-        Auto_Timeseries will rapidly build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet
-        and Scikit-Learn ML. It will automatically select the best model which gives best score specified.
-        </p>
-        <p>New version 0.0.35 onwards has major updates: You can now load your file into Dask dataframes. Just provide the name of your file and if it is too large to fit into a pandas dataframe, Auto_TS will automatically detect and load it into a Dask dataframe. </p>
-        <p>Also, new since version 0.0.25 is the syntax of Auto_TimeSerie: It is now more like scikit-learn (with fit and predict). You will have to initialize an object and then call fit with your data and then predict again with data. Hope this makes it easier to remember and use.</p>
-        <h2 id="introduction">Introduction</h2>
-        <p>Auto_TimeSeries enables you to build and select multiple time series models using techniques such as ARIMA, SARIMAX, VAR, decomposable (trend+seasonality+holidays) models, and ensemble machine learning models.</p>
-        <p>Auto_TimeSeries is an Automated ML library for time series data. Auto_TimeSeries was initially conceived and developed by <a href="https://www.linkedin.com/in/ram-seshadri-nyc-nj/">Ram Seshadri</a> and was significantly expanded in functionality and scope and upgraded to its present status by <a href="https://github.com/ngupta23">Nikhil Gupta</a>.</p>
-        <p>auto-ts.Auto_TimeSeries is the main function that you will call with your train data. You can then choose what kind of models you want: stats, ml or Prophet based model. You can also tell it to automatically select the best model based on the scoring parameter you want it to be based on. It will return the best model and a dictionary containing predictions for the number of forecast_periods you mentioned (default=2).</p>
-        <h2 id="installation-instructions">INSTALLATION INSTRUCTIONS</h2>
-        <ol>
-        <li>Use “pip install auto-ts”</li>
-        <li>Use “pip3 install auto-ts” if the above doesn’t work</li>
-        <li>pip install git+git://github.com/AutoViML/Auto_TS</li>
-        </ol>
-        <h4>Note for Windows Users</h4>
+        ### Installing on Windows
         <p>Windows users may experience difficulties with the Prophet and pystan dependency installations.  Because of this, we recommend installing Prophet using instructions from the <a hreff="https://facebook.github.io/prophet/docs/installation.html"> Prophet documentation page</a> prior to installing auto-ts.  For Anaconda users, this can be accomplished via:
         <ol>
         <li><p><code> conda install -c conda-forge prophet </code> </p></li>
         <li><p><code> pip install auto-ts </code> </p></li>
         </ol>
         
-        <h2 id="run">RUN</h2>
-        <p> First you need to import auto_timeseries from auto_ts library:<br>
-        <code>
+        <h2 id="usage">Usage</h2>
+        
+        ### First you need to import auto_timeseries from auto_ts library:<br>
+        
+        ```
         from auto_ts import auto_timeseries
-        </code>
-        </p>
-        <p>
-        Second, Initialize an auto_timeseries model object which will hold all your parameters:</p>
-        <p><code>
+        ```
+        
+        ### Second, Initialize an auto_timeseries model object which will hold all your parameters:</p>
+        
+        ```
         model = auto_timeseries(
                     score_type='rmse',
                     time_interval='Month',
                     non_seasonal_pdq=None, seasonality=False,
                     seasonal_period=12,
                     model_type=['Prophet'],
                     verbose=2)
-        </code></p>
-        Here are how the input parameters defined:<br>
+        ```
+        
+        #### Here are how the input parameters defined:<br>
         <ol>
         <li><b>score_type (default='rmse')</b>: The metric used for scoring the models. Type is string.
         Currently only the following two types are supported:
         (1) "rmse": Root Mean Squared Error (RMSE)
         (2) "normalized_rmse": Ratio of RMSE to the standard deviation of actuals</li>
         <li><b>time_interval (default is None)</b>: Used to indicate the frequency at which the data is collected.
         This is used for two purposes (1) in building the Prophet model and (2) used to impute the seasonal period for SARIMAX in case it is not provided by the user (None). Type is String.
@@ -127,71 +142,75 @@
         If a list is provided, then only those models will be built
         WARNING: "best" might take some time for large data sets. We recommend that you
         choose a small sample from your data set before attempting to run entire data.
         Type can be either: [string, list]
         </li>
         <li><b>verbose (default=0)</b>: Indicates the verbosity of printing (Default = 0). Type is integer.</li>
         </ol>
-        The next step after defining the model object is to fit it with some real data:
-        <p><code><br>
+        
+        ### The next step after defining the model object is to fit it with some real data:
+        
+        ```
         model.fit(
                     traindata=train_data,
                     ts_column=ts_column,
                     target=target,
                     cv=5,
                     sep=","
                 )
-        </code></p>
-        <br>Here are how the parameters defined:
+        ```
+        
+        Here are how the parameters defined:
         <ul>
         <li><b>traindata (required)</b>: It can be either a dataframe or a file. You must give the name of the file along with its data path in case if a file. It also accepts a pandas dataframe in case you already have a dataframe loaded in your notebook.</li>
         <li><b>ts_column (required)</b>: name of the datetime column in your dataset (it could be a name of column or index number in the columns index)</li>
         <li><b>target (required)</b>: name of the column you   are trying to predict. Target could also be the only column in your dataset</li>
         <li><b>cv (default=5)</b>: You can enter any integer for the number of folds you want in your cross validation data set.
         </li>
         <li><b>sep (default=",")</b>: Sep is the separator in your traindata file. If your separator is ",", "\t", ";", make sure you enter it here. If not, it is ignored.</li>
         </ul>
-        The next step after training the model object is to make some predictions with test data:<br>
-        <p><code><br>
+        
+        ### The next step after training the model object is to make some predictions with test data:<br>
+        
+        ```
         predictions = model.predict(
                     testdata = can be either a dataframe or an integer standing for the forecast_period,
                     model = 'best' or any other string that stands for the trained model
                 )  
-        </code></p>
+        ```
+        
         Here are how the parameters are defined. You can choose to send either testdata in the form of a dataframe or send in an integer to decide how many periods you want to forecast.  You need only
         <ul>
         <li><b>testdata (required)</b>: It can be either a dataframe containing test data or you can use an integer standing for the forecast_period (you want).</li>
         <li><b>model (optional, default = 'best')</b>: The name of the model you want to use among the many different models you have trained. Remember that the default is the best model. But you can choose any model that you want to forecast with. Type is String.</li>
         </ul>
+        
         <h2 id="requirements">Requirements</h2>
-        <p>dask</p>
-        <p>scikit-learn</p>
-        <p>Prophet</p>
-        <p>statsmodels</p>
-        <p>pmdarima</p>
-        <p>XGBoost</p>
-        <h1 id="license">License:</h1>
+        <p>dask, scikit-learn, prophet, statsmodels, pmdarima, XGBoost</p>
+        
+        <h2 id="license">License:</h2>
         <p>Apache License 2.0</p>
-        <h2 id="recommendations">Recommendations</h2>
+        
+        <h2 id="Tips">Tips</h2>
         <ul>
         <li>We recommend that you choose a small sample from your data set before attempting to run entire data. and the evaluation metric so it can select the best model. Currently models within “stats” are compared using AIC and BIC. However, models across different types are compared using RMSE. The results of models are shown using RMSE and Normalized RMSE (ratio of RMSE to the standard deviation of actuals).</li>
         <li>You must clean the data and not have any missing values. Make sure the target variable is numeric, otherwise, it won’t run. If there is more than one target variable in your data set, just specify only one for now, and if you know the time interval that is in your data, you can specify it. Otherwise it auto-ts will try to infer the time interval on its own.</li>
         <li>If you give Auto_Timeseries a different time interval than what the data has, it will automatically resample the data to the given time interval and use the mean of the target for the resampled period.</li>
         <li>Notice that except for filename and ts_column input arguments, which are required, all other arguments are optional.</li>
         <li>Note that optionally you can give a separator for the data in your file. Default is comma (",").</li>
         <li>“time_interval” options are any codes that you can find in this page below.
         <a href="https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#timeseries-offset-aliases">Pandas date-range frequency aliases</a>
         </li>
         <li>Optionally, you can give seasonal_period as any integer that measures the seasonality in the data. If not given, seasonal_period is assumed automatically as follows: Months = 12, Days = 30, Weeks = 52, Qtr = 4, Year = 1, Hours = 24, Minutes = 60 and Seconds = 60.</li>
         <li>If you want to give your own non-seasonal order, please input it as non_seasonal_pdq and for seasonal order, use seasonal_PDQ as the input. Use tuples. For example, seasonal_PDQ = (2,1,2) and non_seasonal_pdq = (0,0,3). It will accept only tuples. The default is None and Auto_Timeseries will automatically search for the best p,d,q (for Non Seasonal) and P, D, Q (for Seasonal) orders by searching for all parameters from 0 to 12 for each value of p,d,q and 0-3 for each P, Q and 0-1 for D.</li>
         </ul>
+        
         <h2 id="disclaimer">DISCLAIMER:</h2>
         <p>This is not an Officially supported Google project.</p>
+        
         <h2 id="copyright">Copyright</h2>
         <p>© Google</p>
-        </body>
-        </html>
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,73 +1,65 @@
-Metadata-Version: 2.1 Name: auto-ts Version: 0.0.70 Summary: Automatically
+Metadata-Version: 2.1 Name: auto-ts Version: 0.0.71 Summary: Automatically
 Build Multiple Time Series models fast - now with Facebook Prophet! Home-page:
 https://github.com/AutoViML/Auto_TS Author: Ram Seshadri License: Apache
 License 2.0 Description:
-![auto-ts](logo.png)
-****** March 2023 Update: ******
-We have now upgraded FB Prophet to the latest version which is simply called
-prophet.
-If you are using Colab or Kaggle kernel and want to install auto_ts, please use
-the following steps (otherwise error!): ``` !pip install auto-ts --no-deps --
-ignore-installed !pip install 'fsspec>=0.3.3' !pip install statsmodels --
-upgrade !pip install pmdarima ```
-****** Aug 2022 Update: ******
-You can now add FB Prophet arguments directly into Auto_TimeSeries using the
-kwargs argument. See example below: ![fb-prophet](add_fb_prophet.png)
 ****** Auto_TS: Auto_TimeSeries ******
 Automatically build multiple Time Series models using a Single Line of Code.
-Now updated with Dask.
-Auto_timeseries is a complex model building utility for time series data. Since
-it automates many Tasks involved in a complex endeavor, it assumes many
-intelligent defaults. But you can change them. Auto_Timeseries will rapidly
-build predictive models based on Statsmodels ARIMA, Seasonal ARIMA, Prophet and
-Scikit-Learn ML. It will automatically select the best model which gives best
-score specified.
-New version 0.0.35 onwards has major updates: You can now load your file into
-Dask dataframes. Just provide the name of your file and if it is too large to
-fit into a pandas dataframe, Auto_TS will automatically detect and load it into
-a Dask dataframe.
-Also, new since version 0.0.25 is the syntax of Auto_TimeSerie: It is now more
-like scikit-learn (with fit and predict). You will have to initialize an object
-and then call fit with your data and then predict again with data. Hope this
-makes it easier to remember and use.
+Now updated with Dask. ![auto-ts](images/logo.png) `auto_timeseries` is a
+complex model building utility for time series data. Since it automates many
+Tasks involved in a complex endeavor, it assumes many intelligent defaults. But
+you can change them. Auto_Timeseries will rapidly build predictive models based
+on Statsmodels ARIMA, Seasonal ARIMA, Prophet and Scikit-Learn ML. It will
+automatically select the best model which gives best score specified. # Table
+of Contents
+    * Latest_updates
+    * What_is_auto_ts
+    * How_to_install_auto_ts
+    * Usage
+    * Requirements
+    * Tips
+    * License
+    * Copyright
+    * Disclaimer
+## Latest To know about the latest updates and features added to Auto_TS please
+go to this [page](updates.md).
 ***** Introduction *****
 Auto_TimeSeries enables you to build and select multiple time series models
 using techniques such as ARIMA, SARIMAX, VAR, decomposable
 (trend+seasonality+holidays) models, and ensemble machine learning models.
 Auto_TimeSeries is an Automated ML library for time series data.
 Auto_TimeSeries was initially conceived and developed by Ram_Seshadri and was
 significantly expanded in functionality and scope and upgraded to its present
 status by Nikhil_Gupta.
 auto-ts.Auto_TimeSeries is the main function that you will call with your train
 data. You can then choose what kind of models you want: stats, ml or Prophet
 based model. You can also tell it to automatically select the best model based
 on the scoring parameter you want it to be based on. It will return the best
 model and a dictionary containing predictions for the number of
-forecast_periods you mentioned (default=2).
-***** INSTALLATION INSTRUCTIONS *****
-   1. Use âpip install auto-tsâ
-   2. Use âpip3 install auto-tsâ if the above doesnât work
-   3. pip install git+git://github.com/AutoViML/Auto_TS
-*** Note for Windows Users ***
+forecast_periods you mentioned (default=2). ## Install ``` pip install auto-ts
+``` Use `pip3 install auto-ts` if the above doesnât work ``` pip install
+git+https://github.com/AutoViML/Auto_TS.git ``` ### Installing on Colab If you
+are using Colab or Kaggle kernel and want to install auto_ts, please use the
+following steps (otherwise you will get an error!): ``` !pip install auto-ts --
+no-deps --ignore-installed !pip install 'fsspec>=0.3.3' !pip install
+statsmodels --upgrade !pip install pmdarima ``` ![auto_ts_colab](images/
+install_auto_ts.png) ### Installing on Windows
 Windows users may experience difficulties with the Prophet and pystan
 dependency installations. Because of this, we recommend installing Prophet
 using instructions from the Prophet documentation page prior to installing
 auto-ts. For Anaconda users, this can be accomplished via:
    1. conda install -c conda-forge prophet
    2. pip install auto-ts
-***** RUN *****
-First you need to import auto_timeseries from auto_ts library:
-from auto_ts import auto_timeseries
-Second, Initialize an auto_timeseries model object which will hold all your
-parameters:
-model = auto_timeseries( score_type='rmse', time_interval='Month',
+***** Usage *****
+### First you need to import auto_timeseries from auto_ts library:
+``` from auto_ts import auto_timeseries ``` ### Second, Initialize an
+auto_timeseries model object which will hold all your parameters:
+``` model = auto_timeseries( score_type='rmse', time_interval='Month',
 non_seasonal_pdq=None, seasonality=False, seasonal_period=12, model_type=
-['Prophet'], verbose=2)
-Here are how the input parameters defined:
+['Prophet'], verbose=2) ``` #### Here are how the input parameters defined:
    1. score_type (default='rmse'): The metric used for scoring the models. Type
       is string. Currently only the following two types are supported: (1)
       "rmse": Root Mean Squared Error (RMSE) (2) "normalized_rmse": Ratio of
       RMSE to the standard deviation of actuals
    2. time_interval (default is None): Used to indicate the frequency at which
       the data is collected. This is used for two purposes (1) in building the
       Prophet model and (2) used to impute the seasonal period for SARIMAX in
@@ -123,58 +115,49 @@
       Random Forests provided explanatory vars are given 'best' will try to
       build all models and pick the best one If a list is provided, then only
       those models will be built WARNING: "best" might take some time for large
       data sets. We recommend that you choose a small sample from your data set
       before attempting to run entire data. Type can be either: [string, list]
    8. verbose (default=0): Indicates the verbosity of printing (Default = 0).
       Type is integer.
-The next step after defining the model object is to fit it with some real data:
-
-model.fit( traindata=train_data, ts_column=ts_column, target=target, cv=5,
-sep="," )
-
-Here are how the parameters defined:
+### The next step after defining the model object is to fit it with some real
+data: ``` model.fit( traindata=train_data, ts_column=ts_column, target=target,
+cv=5, sep="," ) ``` Here are how the parameters defined:
     * traindata (required): It can be either a dataframe or a file. You must
       give the name of the file along with its data path in case if a file. It
       also accepts a pandas dataframe in case you already have a dataframe
       loaded in your notebook.
     * ts_column (required): name of the datetime column in your dataset (it
       could be a name of column or index number in the columns index)
     * target (required): name of the column you are trying to predict. Target
       could also be the only column in your dataset
     * cv (default=5): You can enter any integer for the number of folds you
       want in your cross validation data set.
     * sep (default=","): Sep is the separator in your traindata file. If your
       separator is ",", "\t", ";", make sure you enter it here. If not, it is
       ignored.
-The next step after training the model object is to make some predictions with
-test data:
-
-predictions = model.predict( testdata = can be either a dataframe or an integer
-standing for the forecast_period, model = 'best' or any other string that
-stands for the trained model )
-Here are how the parameters are defined. You can choose to send either testdata
-in the form of a dataframe or send in an integer to decide how many periods you
-want to forecast. You need only
+### The next step after training the model object is to make some predictions
+with test data:
+``` predictions = model.predict( testdata = can be either a dataframe or an
+integer standing for the forecast_period, model = 'best' or any other string
+that stands for the trained model ) ``` Here are how the parameters are
+defined. You can choose to send either testdata in the form of a dataframe or
+send in an integer to decide how many periods you want to forecast. You need
+only
     * testdata (required): It can be either a dataframe containing test data or
       you can use an integer standing for the forecast_period (you want).
     * model (optional, default = 'best'): The name of the model you want to use
       among the many different models you have trained. Remember that the
       default is the best model. But you can choose any model that you want to
       forecast with. Type is String.
 ***** Requirements *****
-dask
-scikit-learn
-Prophet
-statsmodels
-pmdarima
-XGBoost
-****** License: ******
+dask, scikit-learn, prophet, statsmodels, pmdarima, XGBoost
+***** License: *****
 Apache License 2.0
-***** Recommendations *****
+***** Tips *****
     * We recommend that you choose a small sample from your data set before
       attempting to run entire data. and the evaluation metric so it can select
       the best model. Currently models within âstatsâ are compared using
       AIC and BIC. However, models across different types are compared using
       RMSE. The results of models are shown using RMSE and Normalized RMSE
       (ratio of RMSE to the standard deviation of actuals).
     * You must clean the data and not have any missing values. Make sure the
```

### Comparing `auto_ts-0.0.70/auto_ts.egg-info/SOURCES.txt` & `auto_ts-0.0.71/auto_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto_ts-0.0.70/setup.py` & `auto_ts-0.0.71/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="auto_ts",
-    version="0.0.70",
+    version="0.0.71",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Build Multiple Time Series models fast - now with Facebook Prophet!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/Auto_TS",
```

