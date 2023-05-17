# Comparing `tmp/pygris-0.1.4.tar.gz` & `tmp/pygris-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygris-0.1.4.tar", last modified: Wed May  3 14:35:19 2023, max compression
+gzip compressed data, was "pygris-0.1.5.tar", last modified: Wed May 17 17:50:52 2023, max compression
```

## Comparing `pygris-0.1.4.tar` & `pygris-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-03 14:35:19.573255 pygris-0.1.4/
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     1050 2022-10-05 14:20:47.000000 pygris-0.1.4/LICENSE
--rw-rw-r--   0 kyle      (1001) kyle      (1001)       55 2022-11-25 16:28:53.000000 pygris-0.1.4/MANIFEST.in
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     2137 2023-05-03 14:35:19.573255 pygris-0.1.4/PKG-INFO
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     1543 2022-11-25 15:22:17.000000 pygris-0.1.4/README.md
-drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-03 14:35:19.573255 pygris-0.1.4/pygris/
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      229 2023-04-06 13:28:03.000000 pygris-0.1.4/pygris/__init__.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    10047 2023-05-03 14:21:45.000000 pygris-0.1.4/pygris/data.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    37601 2022-11-20 21:03:28.000000 pygris-0.1.4/pygris/enumeration_units.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    11872 2022-11-21 12:13:43.000000 pygris-0.1.4/pygris/geocode.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     5448 2022-12-31 13:21:40.000000 pygris-0.1.4/pygris/helpers.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      180 2022-10-19 14:24:10.000000 pygris-0.1.4/pygris/internal_data.py
-drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-03 14:35:19.573255 pygris-0.1.4/pygris/internals/
--rw-rw-r--   0 kyle      (1001) kyle      (1001)        0 2022-10-13 19:22:43.000000 pygris-0.1.4/pygris/internals/__init__.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)   111585 2022-07-29 23:53:00.000000 pygris-0.1.4/pygris/internals/fips_codes.csv
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    12451 2022-11-20 21:07:11.000000 pygris-0.1.4/pygris/legislative.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    10168 2022-11-20 21:06:27.000000 pygris-0.1.4/pygris/metro_areas.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     3955 2022-10-20 20:36:10.000000 pygris-0.1.4/pygris/national.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    12253 2022-11-20 21:04:25.000000 pygris-0.1.4/pygris/native.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    12451 2022-11-20 21:05:17.000000 pygris-0.1.4/pygris/transportation.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)    13836 2023-05-01 18:04:49.000000 pygris-0.1.4/pygris/utils.py
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     7163 2022-11-20 21:05:52.000000 pygris-0.1.4/pygris/water.py
-drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-03 14:35:19.573255 pygris-0.1.4/pygris.egg-info/
--rw-rw-r--   0 kyle      (1001) kyle      (1001)     2137 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/PKG-INFO
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      530 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/SOURCES.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)        1 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/dependency_links.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      110 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/requires.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)       28 2023-05-03 14:35:19.000000 pygris-0.1.4/pygris.egg-info/top_level.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)      953 2023-04-06 13:32:23.000000 pygris-0.1.4/pyproject.toml
--rw-rw-r--   0 kyle      (1001) kyle      (1001)       68 2022-11-21 15:16:13.000000 pygris-0.1.4/requirements.txt
--rw-rw-r--   0 kyle      (1001) kyle      (1001)       38 2023-05-03 14:35:19.573255 pygris-0.1.4/setup.cfg
+drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-17 17:50:52.249755 pygris-0.1.5/
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     1050 2022-10-05 14:20:47.000000 pygris-0.1.5/LICENSE
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)       55 2022-11-25 16:28:53.000000 pygris-0.1.5/MANIFEST.in
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     2137 2023-05-17 17:50:52.249755 pygris-0.1.5/PKG-INFO
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     1543 2022-11-25 15:22:17.000000 pygris-0.1.5/README.md
+drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-17 17:50:52.249755 pygris-0.1.5/pygris/
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      229 2023-05-10 15:14:36.000000 pygris-0.1.5/pygris/__init__.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    16070 2023-05-16 13:41:11.000000 pygris-0.1.5/pygris/data.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    37836 2023-05-16 13:38:12.000000 pygris-0.1.5/pygris/enumeration_units.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    11872 2022-11-21 12:13:43.000000 pygris-0.1.5/pygris/geocode.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      737 2023-05-14 20:53:12.000000 pygris-0.1.5/pygris/geometry.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     5455 2023-05-09 17:41:50.000000 pygris-0.1.5/pygris/helpers.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      180 2022-10-19 14:24:10.000000 pygris-0.1.5/pygris/internal_data.py
+drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-17 17:50:52.249755 pygris-0.1.5/pygris/internals/
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)        0 2022-10-13 19:22:43.000000 pygris-0.1.5/pygris/internals/__init__.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)   111585 2022-07-29 23:53:00.000000 pygris-0.1.5/pygris/internals/fips_codes.csv
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    12451 2022-11-20 21:07:11.000000 pygris-0.1.5/pygris/legislative.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    10168 2022-11-20 21:06:27.000000 pygris-0.1.5/pygris/metro_areas.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     3955 2022-10-20 20:36:10.000000 pygris-0.1.5/pygris/national.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    12253 2022-11-20 21:04:25.000000 pygris-0.1.5/pygris/native.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    12451 2022-11-20 21:05:17.000000 pygris-0.1.5/pygris/transportation.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)    13836 2023-05-01 18:04:49.000000 pygris-0.1.5/pygris/utils.py
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     7163 2022-11-20 21:05:52.000000 pygris-0.1.5/pygris/water.py
+drwxrwxr-x   0 kyle      (1001) kyle      (1001)        0 2023-05-17 17:50:52.249755 pygris-0.1.5/pygris.egg-info/
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)     2137 2023-05-17 17:50:52.000000 pygris-0.1.5/pygris.egg-info/PKG-INFO
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      549 2023-05-17 17:50:52.000000 pygris-0.1.5/pygris.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)        1 2023-05-17 17:50:52.000000 pygris-0.1.5/pygris.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      110 2023-05-17 17:50:52.000000 pygris-0.1.5/pygris.egg-info/requires.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)       28 2023-05-17 17:50:52.000000 pygris-0.1.5/pygris.egg-info/top_level.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)      953 2023-05-10 15:14:25.000000 pygris-0.1.5/pyproject.toml
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)       68 2022-11-21 15:16:13.000000 pygris-0.1.5/requirements.txt
+-rw-rw-r--   0 kyle      (1001) kyle      (1001)       38 2023-05-17 17:50:52.249755 pygris-0.1.5/setup.cfg
```

### Comparing `pygris-0.1.4/LICENSE` & `pygris-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/PKG-INFO` & `pygris-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygris
-Version: 0.1.4
+Version: 0.1.5
 Summary: Download and use US Census Bureau TIGER/Line Shapefiles and other data resources in Python
 Author-email: Kyle Walker <kyle@walker-data.com>
 License: MIT
 Project-URL: Homepage, https://github.com/walkerke/pygris
 Project-URL: Bug Tracker, https://github.com/walkerke/pygris/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygris-0.1.4/README.md` & `pygris-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris/data.py` & `pygris-0.1.5/pygris/geocode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,252 +1,323 @@
 import requests
 import pandas as pd
-import appdirs
-import os
-from pygris.enumeration_units import states, counties, tracts, block_groups, blocks
+import json
+import geopandas as gp
+import numpy as np
+from io import StringIO
+import csv
 
-def get_census(dataset, variables, year = None, params = {}, 
-               return_geoid = False, guess_dtypes = False):
-    """
-    Make a request to a US Census Bureau API endpoint
 
-    Parameters
-    --------------
-    dataset : str
-        The dataset name; browse https://api.census.gov/data.html for options.
-        The name will be the componet of the API URL that follows "data/" or 
-        the year.  For example, 1-year ACS data will be "acs/acs1". 
-    variables : str or list
-        A string (or list of strings) representing the variables requested from the 
-        API. Datasets have 'variables.html' pages that can be viewed to find 
-        variable IDs, e.g. "https://api.census.gov/data/2017/acs/acs1/variables.html". 
-    year : int
-        The year of the dataset, e.g. 2021. Not all datasets use a year, so leave 
-        blank if so (such as the timeseries APIs). 
-    params : dict
-        A dict of parameters to send with your API request.  This will 
-        vary based on the API you are using. You don't need to include
-        variables in the request, but other optional parameters 
-        will be included here. 
-    return_geoid : bool
-        If True, `get_census()` will attempt to assemble a GEOID column 
-        from contextual information in the dataset that is suitable for 
-        merging to Census shapes acquired with pygris.  This won't make sense
-        / won't work for all datasets, so use this option with caution. 
-        Defaults to False. 
-    guess_dtypes : bool
-        The Census APIs return all columns as strings, but many data 
-        columns should be treated as numbers.  If True, `get_census()` 
-        will scan the columns and try to guess which columns should be
-        converted to numeric and do so. Users may want to leave this
-        option False (the default) and convert columns on a 
-        case-by-case basis.  
+def _parse_geographies(response_obj, geography, keep_geo_cols, type):
+    # Walk through the response object 
+    # first, grab appropriate geography data
+    if type == "geocode":
+        geo_data = pd.json_normalize(response_obj['result'], ['addressMatches', 'geographies', geography])
 
-    Returns
-    -------------
-    A Pandas DataFrame of data from the requested US Census dataset.
+        if not keep_geo_cols:
+            geo_data = geo_data.filter(['GEOID'])
 
-    Notes
-    -------------
-    This function is a low-level interface to the Census APIs provided for convenience. For a full-featured, Pythonic
-    interface to the US Census Bureau APIs, I would recommend using the cenpy package (https://cenpy-devs.github.io/cenpy/index.html)
+        # Next, get the coordinates
+        coords = pd.json_normalize(response_obj['result'], 'addressMatches').filter(['coordinates.x', 'coordinates.y'])
 
-    `get_census()` is inspired by Hannah Recht's work on the censusapi R package (https://www.hrecht.com/censusapi/).  
+        coords.columns = ['longitude', 'latitude']
+
+        # Combine the two frames
+        out = coords.join(geo_data)
+
+        return out
+
+    else:
+        geo_data = pd.json_normalize(response_obj['result'], ['geographies', geography])
 
+        if not keep_geo_cols:
+            geo_data = geo_data.filter(['GEOID'])
+        
+        return geo_data
+    
+
+def geocode(address = None, street = None, city = None, state = None, zip = None,
+            benchmark = "Public_AR_Current",  
+            vintage = "Census2020_Current", as_gdf = False,
+            geography = "Census Blocks", limit = 1, 
+            keep_geo_cols = False, return_dict = False):
     """
+    Use the Census geocoder to return XY coordinates and Census geography for an input address in the
+    United States.
 
-    endpoint = "https://api.census.gov/data"
+    Parameters
+    ---------------
+    address : str
+        A single-line address to be geocoded, e.g. "1600 Pennsylvania Ave, Washington DC 20500"
+    street : str
+        The street address component, e.g. "1600 Pennsylvania Ave", if breaking out the address into 
+        multiple arguments.
+    city : str
+        The city address component, e.g. "Washington"
+    state : str
+        The state address component, e.g. "DC"
+    zip : str
+        The zip code address component, e.g. "20500"
+    benchmark : str
+        The geocoding benchmark to use. Defaults to "Public_AR_Current"; other options are 
+        outlined at https://geocoding.geo.census.gov/geocoder/benchmarks. 
+    vintage : str
+        The geocoding vintage to use. Defaults to "Census2020_Current" to return 2020 Census
+        geographies. Vintages available for a given benchmark can be looked up at 
+        https://geocoding.geo.census.gov/geocoder/vintages?benchmark={benchmark_id}, 
+        where benchmark_id is replaced with the benchmark ID.  
+    as_gdf : bool
+        If False (the default), returns a regular Pandas DataFrame of results. 
+        If True, converts the DataFrame into a GeoDataFrame of points.
+    geography : str
+        The Census geography to return; defaults to 'Census Blocks'. 
+    limit : int
+        How many records to return (as the geocoder can sometimes return multiple
+        matches). Defaults to 1.
+    keep_geo_cols : bool
+        The Census geocoder can return a wide range of contextual information about
+        a location with its response. If True, return all of these columns 
+        (default False)
+    return_dict : bool
+        Advanced users may want to keep the general structure of the Census 
+        geocoder response as a dict without having pygris parse the response. 
+        If so, use True (default False).
+    
+    Returns
+    ---------------
+    A DataFrame (or GeoDataFrame) representing the geocoded address.
 
-    if type(variables) is not list:
-        variables = [variables]
 
-    joined_vars = ",".join(variables)
+    Notes
+    ---------------
+    See https://geocoding.geo.census.gov/geocoder/Geocoding_Services_API.html for more information.
 
-    params.update({'get': joined_vars})
+    """
 
-    if year is None:
-        base = f"{endpoint}/{dataset}"
+    if address is not None:
+        url = "https://geocoding.geo.census.gov/geocoder/geographies/onelineaddress"
+    elif street is not None:
+        url = "https://geocoding.geo.census.gov/geocoder/geographies/address"
     else:
-        base = f"{endpoint}/{year}/{dataset}"
+        raise ValueError("Either a single-line address or street must be specified.")
 
-    req = requests.get(url = base, params = params)
+    req = requests.get(url = url, 
+                       params = {"address": address,
+                        "street": street,
+                        "city": city,
+                        "state": state,
+                        "zip": zip,
+                        "benchmark": benchmark,
+                        "vintage": vintage,
+                        "format": "json"})
 
     if req.status_code != 200:
-        raise SyntaxError(f"Request failed. The Census Bureau error message is {req.text}")
+        raise SyntaxError(f"Your request failed. The error message is {req.text}")
+    
+    r = json.loads(req.text)
+
+    if return_dict:
+        return r
+    else:
+        output = _parse_geographies(response_obj = r, geography = geography, keep_geo_cols = keep_geo_cols,
+                                    type = "geocode")
+
+        if address is not None:
+            output['address'] = address
+        elif street is not None:
+            output['street'] = street
+            output['city'] = city
+            output['state'] = state
+            output['zip'] = zip
 
+        output = output.iloc[0:limit]
+
+    if as_gdf:
+        output = gp.GeoDataFrame(data = output, crs = 4326, geometry = gp.points_from_xy(x = output.longitude, y = output.latitude))
     
-    out = pd.read_json(req.text)
+    return output
 
-    out.columns = out.iloc[0]
-    out = out[1:]
 
-    if return_geoid:
-        # find the columns that are not in variables
-        my_cols = list(out.columns)
+def geolookup(longitude, latitude,
+            benchmark = "Public_AR_Current",  
+            vintage = "Census2020_Current",
+            geography = "Census Blocks", limit = 1, 
+            keep_geo_cols = False, return_dict = False): 
 
-        # if 'state' is not in the list of columns, don't assemble the GEOID; too much 
-        # ambiguity among possible combinations across the various endpoints
-        if "state" not in my_cols:
-            raise ValueError("`return_geoid` is not supported for this geography hierarchy.")
+    """
+    Use the Census GeoLookup service to return Census geography for an XY coordinate
+    pair in the United States.
 
-        # Identify the position of the state column in my_cols, and 
-        # extract all the columns that follow it
-        state_ix = my_cols.index("state")
+    Parameters
+    ---------------
+    longitude : float
+        The X (longitude) coordinate of your requested location.
+    latitude : float
+        The Y (latitude) coordinate of your requested location.
+    benchmark : str
+        The geocoding benchmark to use. Defaults to "Public_AR_Current"; other options are 
+        outlined at https://geocoding.geo.census.gov/geocoder/benchmarks. 
+    vintage : str
+        The geocoding vintage to use. Defaults to "Census2020_Current" to return 2020 Census
+        geographies. Vintages available for a given benchmark can be looked up at 
+        https://geocoding.geo.census.gov/geocoder/vintages?benchmark={benchmark_id}, 
+        where benchmark_id is replaced with the benchmark ID.  
+    geography : str
+        The Census geography to return; defaults to 'Census Blocks'. 
+    limit : int
+        How many records to return (as the geocoder can sometimes return multiple
+        matches). Defaults to 1.
+    keep_geo_cols : bool
+        The Census geocoder can return a wide range of contextual information about
+        a location with its response. If True, return all of these columns 
+        (default False)
+    return_dict : bool
+        Advanced users may want to keep the general structure of the Census 
+        geocoder response as a dict without having pygris parse the response. 
+        If so, use True (default False).
+    
+    Returns
+    ---------------
+    A DataFrame representing the location with contextual information from the Census Bureau.
+
+
+    Notes
+    ---------------
+    See https://geocoding.geo.census.gov/geocoder/Geocoding_Services_API.html for more information.
+
+    """
 
-        geoid_cols = my_cols[state_ix:]
-       
-        # Assemble the GEOID column, then remove its constituent parts
-        out['GEOID'] = out[geoid_cols].agg("".join, axis = 1)
+    url = "https://geocoding.geo.census.gov/geocoder/geographies/coordinates"
 
-        out = out.drop(geoid_cols, axis = 1)
+    req = requests.get(url = url, 
+                       params = {"x": longitude,
+                        "y": latitude,
+                        "benchmark": benchmark,
+                        "vintage": vintage,
+                        "format": "json"})
+    
+    if req.status_code != 200:
+        raise SyntaxError(f"Your request failed. The error message is {req.text}")
     
-    if guess_dtypes:
-        num_list = []
-        # Iterate through the columns in variables and try to guess if they should be converted
-        for v in variables:
-            check = pd.to_numeric(out[v], errors = "coerce")
-            # If the columns aren't fully null, convert to numeric, taking care of any oddities
-            if not pd.isnull(check.unique())[0]:
-                out[v] = check
-                num_list.append(v)
+    r = json.loads(req.text)
 
-        # If we are guessing numerics, we should convert NAs (negatives below -1 million)
-        # to NaN. Users who want to keep the codes should keep as object and handle
-        # themselves.
-        out[num_list] = out[num_list].where(out[num_list] > -999999)
+    if return_dict:
+        return r
+    else:
+        output = _parse_geographies(response_obj = r, geography = geography, keep_geo_cols = keep_geo_cols,
+                                    type = "geolookup")
 
-    return out
+        output['longitude'] = longitude
+        output['latitude'] = latitude
 
+        output = output.iloc[0:limit]
 
-def get_lodes(state, year, version = "LODES8", lodes_type = "od", part = "main", 
-              job_type = "JT00", segment = "S000", agg_level = "block", cache = False):
+        return output
+
+def batch_geocode(df, address, city = None, state = None, zip = None,
+                  id_column = None, benchmark = "Public_AR_Current",
+                  vintage = "Census2020_Current", as_gdf = False):
 
     """
-    Get synthetic block-level data on workplace, residence, and origin-destination flows characteristics from the 
-    LEHD Origin-Destination Employment Statistics (LODES) dataset
+    Use the Census batch geocoder to geocode a DataFrame of addresses in the Unied States.
 
     Parameters
-    --------------
+    ---------------
+    df : pandas.DataFrame
+        A Pandas DataFrame containing addresses to be geocoded.  Address components should be 
+        split across columns, meaning that separate columns are required for street address,
+        city, state, and zip code.  
+    street : str
+        The name of the street address column, e.g. "address"
+    city : str
+        The name of the city column, e.g. "city"
     state : str
-        The state postal code of your requested data. Please note that not all states are available 
-        in all years.
-    year : int
-        The year of your requested data. LODES data go back to 2002, but not all datasets are available 
-        for all years / for all states.  
-    version : str
-        The LODES version to use.  Version 8 (the default, use "LODES8") is enumerated at 2020 Census blocks.
-        "LODES7" is enumerated at 2010 Census blocks, but ends in 2019; "LODES5" is enumerated at 2000 Census
-        blocks, but ends in 2009.  
-    lodes_type : str
-        One of "od" (the default) for origin-destination flows, "wac" for workplace area characteristics, 
-        or "rac" for residence area characteristics.  
-    part : str
-        Only relevant for the "od" file.  "main" gives information on within-state residence to workplace flows.
-        "aux" gives information for residence to workplace flows from outside a given state.
-    job_type : str
-        The available job type breakdown; defaults to "JT00" for all jobs. Please review the LODES technical
-        documentation for a description of other options.
-    segment : str
-        The workforce segment, relevant when lodes_type is "wac" or "rac". Defaults to "S000" for total jobs;
-        review the LODES technical documentation for a description of other options.
-    agg_level : str
-        The level at which to aggregate the data.  Defaults to the Census block; other options include 
-        "state", "county", "tract", and "block group".  
-    cache : bool
-        If True, downloads the requested LODES data to a cache directory on your computer and reads from
-        that directory if the file exists. Defaults to False, which will download the data by default. 
-
+        The name of the state column, e.g. "state"
+    zip : str
+        The name of the zip code column, e.g. "zip"
+    benchmark : str
+        The geocoding benchmark to use. Defaults to "Public_AR_Current"; other options are 
+        outlined at https://geocoding.geo.census.gov/geocoder/benchmarks. 
+    vintage : str
+        The geocoding vintage to use. Defaults to "Census2020_Current" to return 2020 Census
+        geographies. Vintages available for a given benchmark can be looked up at 
+        https://geocoding.geo.census.gov/geocoder/vintages?benchmark={benchmark_id}, 
+        where benchmark_id is replaced with the benchmark ID.  
+    as_gdf : bool
+        If False (the default), returns a regular Pandas DataFrame of results. 
+        If True, converts the DataFrame into a GeoDataFrame of points.
+    
     Returns
     ---------------
-    A Pandas DataFrame of LODES data.
+    A DataFrame (or GeoDataFrame) representing the geocoded addresses.
 
 
     Notes
     ---------------
-    Please review the LODES technical documentation at https://lehd.ces.census.gov/data/lodes/LODES7/LODESTechDoc7.5.pdf for 
-    more information.
-
-    `get_lodes()` is inspired by the lehdr R package (https://github.com/jamgreen/lehdr) by 
-    Jamaal Green, Dillon Mahmoudi, and Liming Wang.
+    See https://geocoding.geo.census.gov/geocoder/Geocoding_Services_API.html for more information.
 
-
-    
     """
 
-    if lodes_type not in ['od', 'wac', 'rac']:
-        raise ValueError("lodes_type must be one of 'od', 'rac', or 'wac'.")
+    # Check to make sure the dataset doesn't exceed 10k rows
+    if df.shape[0] > 10000:
+        raise ValueError("The row limit for the Census batch geocoder is 10,000. Consider splitting your request into multiple requests and retry.")
     
-    state = state.lower()
+    # Prep the df object for sending to the geocoder
+    if id_column is None:
+        request_df = pd.DataFrame(
+            {"Unique ID": range(0, df.shape[0]),
+             "Street address": df[address]}
+        )
+    else:
+        request_df = pd.DataFrame(
+            {"Unique ID": df[id_column],
+             "Street address": df[address]}
+        )    
 
-    if lodes_type == "od":
-        url = f"https://lehd.ces.census.gov/data/lodes/{version}/{state}/od/{state}_od_{part}_{job_type}_{year}.csv.gz"
+    if city is None:
+        request_df["City"] = np.nan
     else:
-        url = f"https://lehd.ces.census.gov/data/lodes/{version}/{state}/{lodes_type}/{state}_{lodes_type}_{segment}_{job_type}_{year}.csv.gz"
+        request_df["City"] = df[city]
     
-    if not cache:
-        lodes_data = pd.read_csv(url)
-        
+    if state is None:
+        request_df["State"] = np.nan
+    else:
+        request_df["State"] = df[state]
+    
+    if zip is None:
+        request_df["ZIP"] = np.nan
     else:
-        cache_dir = appdirs.user_cache_dir("pygris")
+        request_df["ZIP"] = df[zip]
 
-        if not os.path.isdir(cache_dir):
-            os.mkdir(cache_dir) 
+    # Store the df as a CSV
+    request_csv = request_df.to_csv(index = False, header = False)
 
-        basename = os.path.basename(url)
+    # Formulate the request
+    req = requests.post(
+        url = "https://geocoding.geo.census.gov/geocoder/geographies/addressbatch",
+        files = {"addressFile": ('request.csv', request_csv)},
+        data = {
+            "benchmark": benchmark,
+            "vintage": vintage
+        }
+    )
 
-        out_file = os.path.join(cache_dir, basename)
-        
-        # If the file doesn't exist, you'll need to download it
-        # and write it to the cache directory
-        if not os.path.isfile(out_file):
-            req = requests.get(url = url)
+    if req.status_code != 200:
+        raise SyntaxError(f"Your request failed. The error message is {req.text}")
 
-            with open(out_file, 'wb') as fd:
-                fd.write(req.content)
-        
-        # Now, read in the file from the cache directory
-        lodes_data = pd.read_csv(out_file)
+    output = pd.read_csv(StringIO(req.text), sep = ",", header = None, quoting = csv.QUOTE_ALL)
 
-    # Drop the 'createdate' column
-    lodes_data = lodes_data.drop('createdate', axis = 1)
+    # name the columns appropriately
+    output.columns = ['id', 'address', 'status', 'match_quality', 'matched_address', 'coordinates', 'tiger_line_id', 'tiger_side', 
+                      'state', 'county', 'tract', 'block']
 
-    if lodes_type == "od":
-        lodes_data['w_geocode'] = lodes_data['w_geocode'].astype(str).str.zfill(15)
-        lodes_data['h_geocode'] = lodes_data['h_geocode'].astype(str).str.zfill(15)
-    elif lodes_type == "rac":
-        lodes_data['h_geocode'] = lodes_data['h_geocode'].astype(str).str.zfill(15)
-    else:
-        lodes_data['w_geocode'] = lodes_data['w_geocode'].astype(str).str.zfill(15)
-
-    # Handle aggregation logic
-    if agg_level != "block":
-        if agg_level == "state":
-            end = 2
-        elif agg_level == "county":
-            end = 5
-        elif agg_level == "tract":
-            end = 11
-        elif agg_level == "block group":
-            end = 12
-        else: 
-            raise ValueError("Invalid agg_level; choose one of 'state', 'county', 'tract', or 'block group'.")
-        
-        if lodes_type == "wac":
-            lodes_data['w_geocode'] = lodes_data['w_geocode'].str.slice(stop = end)
+    # split longitude/latitude
+    output = output.join(output['coordinates'].str.split(',', expand = True).rename(columns = {0: 'longitude', 1: 'latitude'})).drop('coordinates', axis = 1)
 
-            lodes_data = lodes_data.groupby('w_geocode').agg("sum")
-        elif lodes_type == "rac":
-            lodes_data['h_geocode'] = lodes_data['h_geocode'].str.slice(stop = end)
+    if as_gdf:
+        output = gp.GeoDataFrame(data = output, crs = 4326, geometry = gp.points_from_xy(x = output.longitude, y = output.latitude))
 
-            lodes_data = lodes_data.groupby('h_geocode').agg("sum")
-        elif lodes_type == "od":
-            lodes_data['h_geocode'] = lodes_data['h_geocode'].str.slice(stop = end)
-            lodes_data['w_geocode'] = lodes_data['w_geocode'].str.slice(stop = end)
+    return output
 
-            lodes_data = lodes_data.groupby(['h_geocode', 'w_geocode']).agg("sum")  
 
-        return lodes_data.reset_index()          
     
 
-
-
-
```

### Comparing `pygris-0.1.4/pygris/enumeration_units.py` & `pygris-0.1.5/pygris/enumeration_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,15 +479,22 @@
         print(f"Using the default year of {year}")
     
     if state is None:
         if year == 2019 and cb:
             state = "us"
             print("Retrieving PUMAs for the entire United States")
         else:
-            raise ValueError("A year must be specified for this year/dataset combination.")
+            fips = fips_codes()
+
+            print("Retrieving PUMAs by state and combining the result")
+            all_states = [code for code in fips['state_code'].unique().tolist() if code <= "56"]
+
+            all_pumas = pd.concat([pumas(x, year = year, cache = cache) for x in all_states])
+
+            return all_pumas
     else:
         state = validate_state(state)
     
 
     if year > 2021:
         suf = "20"
     else:
```

### Comparing `pygris-0.1.4/pygris/helpers.py` & `pygris-0.1.5/pygris/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,8 +157,11 @@
             if not quiet:
                 print(f"Using FIPS code '{cty_code}' for input '{county}'")
 
             return cty_code
         else:
             msg = f"Your string matches {' and '.join(possible_counties)}. Please refine your selection."
 
-            raise ValueError(msg)
+            raise ValueError(msg)   
+
+
+
```

### Comparing `pygris-0.1.4/pygris/internals/fips_codes.csv` & `pygris-0.1.5/pygris/internals/fips_codes.csv`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris/legislative.py` & `pygris-0.1.5/pygris/legislative.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris/metro_areas.py` & `pygris-0.1.5/pygris/metro_areas.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris/national.py` & `pygris-0.1.5/pygris/national.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris/native.py` & `pygris-0.1.5/pygris/native.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris/transportation.py` & `pygris-0.1.5/pygris/transportation.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris/utils.py` & `pygris-0.1.5/pygris/utils.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris/water.py` & `pygris-0.1.5/pygris/water.py`

 * *Files identical despite different names*

### Comparing `pygris-0.1.4/pygris.egg-info/PKG-INFO` & `pygris-0.1.5/pygris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygris
-Version: 0.1.4
+Version: 0.1.5
 Summary: Download and use US Census Bureau TIGER/Line Shapefiles and other data resources in Python
 Author-email: Kyle Walker <kyle@walker-data.com>
 License: MIT
 Project-URL: Homepage, https://github.com/walkerke/pygris
 Project-URL: Bug Tracker, https://github.com/walkerke/pygris/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygris-0.1.4/pygris.egg-info/SOURCES.txt` & `pygris-0.1.5/pygris.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 requirements.txt
 pygris/__init__.py
 pygris/data.py
 pygris/enumeration_units.py
 pygris/geocode.py
+pygris/geometry.py
 pygris/helpers.py
 pygris/internal_data.py
 pygris/legislative.py
 pygris/metro_areas.py
 pygris/national.py
 pygris/native.py
 pygris/transportation.py
```

### Comparing `pygris-0.1.4/pyproject.toml` & `pygris-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygris"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Kyle Walker", email="kyle@walker-data.com" },
 ]
 license = {text = "MIT"}
 description = "Download and use US Census Bureau TIGER/Line Shapefiles and other data resources in Python"
 readme = "README.md"
 requires-python = ">=3.7"
```

