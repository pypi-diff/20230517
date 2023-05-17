# Comparing `tmp/skyndo-0.7.8.tar.gz` & `tmp/skyndo-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyndo-0.7.8.tar", last modified: Tue May 16 08:31:40 2023, max compression
+gzip compressed data, was "skyndo-0.7.9.tar", last modified: Wed May 17 03:48:26 2023, max compression
```

## Comparing `skyndo-0.7.8.tar` & `skyndo-0.7.9.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:31:40.288885 skyndo-0.7.8/
--rw-rw-rw-   0        0        0      378 2023-05-16 08:31:40.287888 skyndo-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-16 08:31:40.288885 skyndo-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0      606 2023-05-16 08:30:42.000000 skyndo-0.7.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:31:39.837093 skyndo-0.7.8/skyndo/
--rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7.8/skyndo/_init_.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:31:39.918875 skyndo-0.7.8/skyndo/data/
--rw-rw-rw-   0        0        0 25199035 2023-03-31 16:13:20.000000 skyndo-0.7.8/skyndo/data/model.pkl
--rw-rw-rw-   0        0        0     2175 2023-05-16 04:33:41.000000 skyndo-0.7.8/skyndo/predict.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:31:39.917878 skyndo-0.7.8/skyndo.egg-info/
--rw-rw-rw-   0        0        0      378 2023-05-16 08:31:39.000000 skyndo-0.7.8/skyndo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-16 08:31:39.000000 skyndo-0.7.8/skyndo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:31:39.000000 skyndo-0.7.8/skyndo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-16 08:31:39.000000 skyndo-0.7.8/skyndo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 08:31:39.000000 skyndo-0.7.8/skyndo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 03:48:26.707384 skyndo-0.7.9/
+-rw-rw-rw-   0        0        0      378 2023-05-17 03:48:26.706357 skyndo-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-17 03:48:26.707384 skyndo-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-05-16 10:58:17.000000 skyndo-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:48:26.627069 skyndo-0.7.9/skyndo/
+-rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7.9/skyndo/_init_.py
+-rw-rw-rw-   0        0        0     2657 2023-05-16 10:55:27.000000 skyndo-0.7.9/skyndo/predict.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:48:26.704364 skyndo-0.7.9/skyndo.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-05-17 03:48:26.000000 skyndo-0.7.9/skyndo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-17 03:48:26.000000 skyndo-0.7.9/skyndo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 03:48:26.000000 skyndo-0.7.9/skyndo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-17 03:48:26.000000 skyndo-0.7.9/skyndo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 03:48:26.000000 skyndo-0.7.9/skyndo.egg-info/top_level.txt
```

### Comparing `skyndo-0.7.8/skyndo/predict.py` & `skyndo-0.7.9/skyndo/predict.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,29 @@
-import pickle
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 
+df_zc_r = pd.read_csv('https://raw.githubusercontent.com/NishanD21/Astronomical-Objects-Classification/main/Datasets/sgq_classification_zc_r.csv')
+
+x = df_zc_r.drop("class",axis='columns')
+y = df_zc_r["class"]
+
+from sklearn.model_selection import train_test_split
+x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.1,random_state=42, stratify=y)
+
+from sklearn.ensemble import RandomForestClassifier
+
+# initializing model
+model_rf = RandomForestClassifier(n_estimators=100, random_state=42)
+model_rf.fit(x_train,y_train)
 
 def predictor(alpha, delta, u, g, i, r, z, redshift): # To predict the class of the astronomical objet for given features.
     # Load the trained model
-    with open('model.pkl', 'rb') as f:
-        model = pickle.load(f)
+    model = model_rf
     
     # Make the prediction
     x = np.array([[alpha, delta, u, g, i, r, z, redshift]])
     prediction = model.predict(x)[0]
     
     # Map the predicted value to the desired class
     if prediction == 0:
```

