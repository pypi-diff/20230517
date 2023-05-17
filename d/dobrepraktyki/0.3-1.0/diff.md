# Comparing `tmp/dobrepraktyki-0.3.tar.gz` & `tmp/dobrepraktyki-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dobrepraktyki-0.3.tar", last modified: Tue May 16 15:48:13 2023, max compression
+gzip compressed data, was "dobrepraktyki-1.0.tar", last modified: Wed May 17 06:58:40 2023, max compression
```

## Comparing `dobrepraktyki-0.3.tar` & `dobrepraktyki-1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 15:48:13.550419 dobrepraktyki-0.3/
--rw-rw-rw-   0        0        0      208 2023-05-16 15:48:13.549416 dobrepraktyki-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6337 2023-05-15 17:07:40.000000 dobrepraktyki-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 15:48:13.512117 dobrepraktyki-0.3/Songs/
--rw-rw-rw-   0        0        0        0 2023-05-16 08:16:56.000000 dobrepraktyki-0.3/Songs/__init__.py
--rw-rw-rw-   0        0        0      660 2023-05-16 08:16:56.000000 dobrepraktyki-0.3/Songs/shazam.py
-drwxrwxrwx   0        0        0        0 2023-05-16 15:48:13.519794 dobrepraktyki-0.3/Weather/
--rw-rw-rw-   0        0        0        0 2023-05-16 08:16:56.000000 dobrepraktyki-0.3/Weather/__init__.py
--rw-rw-rw-   0        0        0     1469 2023-05-16 08:16:56.000000 dobrepraktyki-0.3/Weather/weatherapi.py
--rw-rw-rw-   0        0        0      925 2023-05-16 08:16:56.000000 dobrepraktyki-0.3/Weather/weatherbit.py
-drwxrwxrwx   0        0        0        0 2023-05-16 15:48:13.546460 dobrepraktyki-0.3/dobrepraktyki.egg-info/
--rw-rw-rw-   0        0        0      208 2023-05-16 15:48:13.000000 dobrepraktyki-0.3/dobrepraktyki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-16 15:48:13.000000 dobrepraktyki-0.3/dobrepraktyki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 15:48:13.000000 dobrepraktyki-0.3/dobrepraktyki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 15:48:13.000000 dobrepraktyki-0.3/dobrepraktyki.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-16 15:48:13.000000 dobrepraktyki-0.3/dobrepraktyki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 15:48:13.551416 dobrepraktyki-0.3/setup.cfg
--rw-rw-rw-   0        0        0      255 2023-05-16 15:37:21.000000 dobrepraktyki-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:58:40.082949 dobrepraktyki-1.0/
+-rw-rw-rw-   0        0        0      208 2023-05-17 06:58:40.082949 dobrepraktyki-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6337 2023-05-15 17:07:40.000000 dobrepraktyki-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 06:58:40.036082 dobrepraktyki-1.0/Songs/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:16:56.000000 dobrepraktyki-1.0/Songs/__init__.py
+-rw-rw-rw-   0        0        0      660 2023-05-16 08:16:56.000000 dobrepraktyki-1.0/Songs/shazam.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:58:40.051656 dobrepraktyki-1.0/Weather/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:16:56.000000 dobrepraktyki-1.0/Weather/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-05-17 06:58:14.000000 dobrepraktyki-1.0/Weather/weatherapi.py
+-rw-rw-rw-   0        0        0     1008 2023-05-17 06:58:14.000000 dobrepraktyki-1.0/Weather/weatherbit.py
+drwxrwxrwx   0        0        0        0 2023-05-17 06:58:40.067323 dobrepraktyki-1.0/dobrepraktyki.egg-info/
+-rw-rw-rw-   0        0        0      208 2023-05-17 06:58:39.000000 dobrepraktyki-1.0/dobrepraktyki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-17 06:58:39.000000 dobrepraktyki-1.0/dobrepraktyki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 06:58:39.000000 dobrepraktyki-1.0/dobrepraktyki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 06:58:39.000000 dobrepraktyki-1.0/dobrepraktyki.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-17 06:58:39.000000 dobrepraktyki-1.0/dobrepraktyki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 06:58:40.082949 dobrepraktyki-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      255 2023-05-17 06:58:26.000000 dobrepraktyki-1.0/setup.py
```

### Comparing `dobrepraktyki-0.3/README.md` & `dobrepraktyki-1.0/README.md`

 * *Files identical despite different names*

### Comparing `dobrepraktyki-0.3/Songs/shazam.py` & `dobrepraktyki-1.0/Songs/shazam.py`

 * *Files identical despite different names*

### Comparing `dobrepraktyki-0.3/Weather/weatherapi.py` & `dobrepraktyki-1.0/Weather/weatherapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,13 +27,15 @@
             data = response.json()
 
             for forecast in data["forecast"]["forecastday"]:
                 date = forecast["date"]
                 max_temp = forecast["day"]["maxtemp_c"]
                 min_temp = forecast["day"]["mintemp_c"]
                 condition = forecast["day"]["condition"]["text"]
+                uv = forecast["day"]["uv"]
 
                 tmp.update({date: {"max_temp": max_temp,
                                    "min_temp": min_temp,
-                                   "condition": condition}})
+                                   "condition": condition,
+                                   "uv": uv}})
             return tmp
         return None
```

### Comparing `dobrepraktyki-0.3/Weather/weatherbit.py` & `dobrepraktyki-1.0/Weather/weatherbit.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,13 +16,15 @@
             data = response.json()
 
             for forecast in data["data"]:
                 date = forecast["valid_date"]
                 max_temp = forecast["max_temp"]
                 min_temp = forecast["min_temp"]
                 condition = forecast["weather"]["description"]
+                uv = forecast["uv"]
 
                 tmp.update({date: {"max_temp": max_temp,
                                    "min_temp": min_temp,
-                                   "condition": condition}})
+                                   "condition": condition,
+                                   "uv": uv}})
             return tmp
         return None
```

