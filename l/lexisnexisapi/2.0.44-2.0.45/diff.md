# Comparing `tmp/lexisnexisapi-2.0.44.tar.gz` & `tmp/lexisnexisapi-2.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexisnexisapi-2.0.44.tar", last modified: Fri Feb 24 21:22:27 2023, max compression
+gzip compressed data, was "lexisnexisapi-2.0.45.tar", last modified: Wed May 17 16:37:36 2023, max compression
```

## Comparing `lexisnexisapi-2.0.44.tar` & `lexisnexisapi-2.0.45.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 21:22:27.274279 lexisnexisapi-2.0.44/
--rw-rw-rw-   0        0        0      466 2022-12-20 12:40:20.000000 lexisnexisapi-2.0.44/LICENSE.txt
--rw-rw-rw-   0        0        0     1904 2023-02-24 21:22:27.272277 lexisnexisapi-2.0.44/PKG-INFO
--rw-rw-rw-   0        0        0     1382 2023-02-08 14:35:01.000000 lexisnexisapi-2.0.44/README.md
--rw-rw-rw-   0        0        0      588 2023-02-24 20:42:01.000000 lexisnexisapi-2.0.44/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-24 21:22:27.275279 lexisnexisapi-2.0.44/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-02-24 20:42:14.000000 lexisnexisapi-2.0.44/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-24 21:22:27.218278 lexisnexisapi-2.0.44/src/
-drwxrwxrwx   0        0        0        0 2023-02-24 21:22:27.250278 lexisnexisapi-2.0.44/src/lexisnexisapi/
--rw-rw-rw-   0        0        0        0 2023-01-28 19:22:50.000000 lexisnexisapi-2.0.44/src/lexisnexisapi/__init__.py
--rw-rw-rw-   0        0        0     1863 2023-02-02 17:25:44.000000 lexisnexisapi-2.0.44/src/lexisnexisapi/credentials.py
--rw-rw-rw-   0        0        0    10114 2023-02-24 19:32:29.000000 lexisnexisapi-2.0.44/src/lexisnexisapi/metabase.py
-drwxrwxrwx   0        0        0        0 2023-02-24 21:22:27.268278 lexisnexisapi-2.0.44/src/lexisnexisapi.egg-info/
--rw-rw-rw-   0        0        0     1904 2023-02-24 21:22:27.000000 lexisnexisapi-2.0.44/src/lexisnexisapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-02-24 21:22:27.000000 lexisnexisapi-2.0.44/src/lexisnexisapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 21:22:27.000000 lexisnexisapi-2.0.44/src/lexisnexisapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-02-24 21:22:27.000000 lexisnexisapi-2.0.44/src/lexisnexisapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 16:37:36.346732 lexisnexisapi-2.0.45/
+-rw-rw-rw-   0        0        0      466 2022-12-20 12:40:20.000000 lexisnexisapi-2.0.45/LICENSE.txt
+-rw-rw-rw-   0        0        0     1904 2023-05-17 16:37:36.344732 lexisnexisapi-2.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0     1382 2023-02-08 14:35:01.000000 lexisnexisapi-2.0.45/README.md
+-rw-rw-rw-   0        0        0      588 2023-05-17 16:36:30.000000 lexisnexisapi-2.0.45/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 16:37:36.346732 lexisnexisapi-2.0.45/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-05-17 16:36:08.000000 lexisnexisapi-2.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:37:36.295730 lexisnexisapi-2.0.45/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 16:37:36.331730 lexisnexisapi-2.0.45/src/lexisnexisapi/
+-rw-rw-rw-   0        0        0        0 2023-01-28 19:22:50.000000 lexisnexisapi-2.0.45/src/lexisnexisapi/__init__.py
+-rw-rw-rw-   0        0        0     1863 2023-02-02 17:25:44.000000 lexisnexisapi-2.0.45/src/lexisnexisapi/credentials.py
+-rw-rw-rw-   0        0        0     9947 2023-05-17 16:34:24.000000 lexisnexisapi-2.0.45/src/lexisnexisapi/metabase.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:37:36.341734 lexisnexisapi-2.0.45/src/lexisnexisapi.egg-info/
+-rw-rw-rw-   0        0        0     1904 2023-05-17 16:37:36.000000 lexisnexisapi-2.0.45/src/lexisnexisapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-17 16:37:36.000000 lexisnexisapi-2.0.45/src/lexisnexisapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 16:37:36.000000 lexisnexisapi-2.0.45/src/lexisnexisapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-17 16:37:36.000000 lexisnexisapi-2.0.45/src/lexisnexisapi.egg-info/top_level.txt
```

### Comparing `lexisnexisapi-2.0.44/PKG-INFO` & `lexisnexisapi-2.0.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexisnexisapi
-Version: 2.0.44
+Version: 2.0.45
 Summary: A small example package
 Home-page: 
 Author: Robert Cuffney
 Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
 License: MIT
 Keywords: example project
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lexisnexisapi-2.0.44/README.md` & `lexisnexisapi-2.0.45/README.md`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-2.0.44/pyproject.toml` & `lexisnexisapi-2.0.45/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexisnexisapi"
-version = "2.0.44"
+version = "2.0.45"
 authors = [{ name = "Robert Cuffney", email = "robert.cuffney@lexisnexis.com" },
 		   { name = "Ozgur Aycan", email = "ozgur.aycan@lexisnexis.co.uk" }
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lexisnexisapi-2.0.44/src/lexisnexisapi/credentials.py` & `lexisnexisapi-2.0.45/src/lexisnexisapi/credentials.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-2.0.44/src/lexisnexisapi/metabase.py` & `lexisnexisapi-2.0.45/src/lexisnexisapi/metabase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import requests
 import json
 import pandas as pd
 from datetime import datetime
 from lexisnexisapi import credentials as cred
 import time
+import ast
+
 
 __version__ = '0.1'
 __author__ = "Robert Cuffney & Ozgur Aycan, CS Integration Consultants @ LexisNexis"
 
 #Constants are usually defined on a module level and written in all capital letters with underscores separating words. 
 #Examples include MAX_OVERFLOW and TOTAL.
 
@@ -32,17 +34,14 @@
             print(data['totalResults'])
         else:
             data = http_request(self.parameters)
         if type(data)==dict:
             self.__dict__.update(data)
         else:
             print("Something went wrong, No data was returned")
-        #print(f'Class instance of "{self.__class__.__name__}" has been created!')
-        #%notify -m "http request complete"
-        #self.__dict__.update(r)
     def set_parameters(self,p):
         if 'key' not in p:
             p['key']= cred.get_Key("Metabase_Search_Key")
         if 'limit' not in p:
             p['limit']='1000'
         p['format']='json'
         if p['key']=='':
@@ -51,15 +50,15 @@
             to save a key:
             use metabase.set_mb_search_key("your key here")
             to send a key:
             include key parameter in your metabase.Search parameters (e.g. metabase.Search(key="your key here", query="your query")
             '''
             print(msg)
         return p
-    def get_dataframe(self,*args):
+    def articles_dataframe(self,*args):
         '''
         returns a data frame of the articles
         optional parameter fields, is a list of desired fields to return
         '''
         df = pd.DataFrame()
         for a in self.articles:
             df = df.append(a, ignore_index=True)
@@ -73,15 +72,15 @@
         creates a json file
         '''
         if self.totalResults != 0:
             with open(file, "w") as my_file:
                 my_file.write(json.dumps(self.articles, indent=4))
                 print(f'{len(self.articles)} article(s) successfully written to a file:{file}')
         else:
-            print("no articles to write!") 
+            print("no articles to write to file!") 
 
 #### Below Functions, within this class, used only for FullDataSet
     def get_fulldataset(self):
         self.parameters.pop('sequence_id',"")                 #get rid of 'sequence_id' if it's there
         #self.parameters['limit']='1000'                       #This will set the limit to the maximum allowed per their key  
         t_lst =[]                                             #this will be the list of all articles
         x=1                                                   #this will represent the number of articles left
@@ -170,15 +169,15 @@
     r = requests.get(rateCheckUrl)
     if r.status_code == 200:
         data = r.json()
     return data['rateLimits']
         
 def set_mb_search_key(v):
     cred.set_Key(Metabase_Search_Key=v)
-def get_mb_search_key(): 
+def mb_search_key(): 
     '''
     Uses mycred.json file to determine Metabase Search Key
     '''
     myMBkey = cred.get_Key('Metabase_Search_Key')
     return myMBkey
 def get_time():
     '''
@@ -195,34 +194,34 @@
     def __init__(self, myArticle):
         '''
         Takes each key from the article dictionary and sets it as an attribute of the class
         '''
         self.__dict__.update(myArticle)
 
     
-def get_df(obj,*args):
+def indexTerms(obj,*args):
     '''
     returns a dataframe of index terms
     accepts either an instance of Search, or an instance of Article.
     if Search is sent, df return is an aggregate count of the terms
     if Article is sent, df return is a dataframe of all index terms
     '''
     if isinstance(obj, Search):
         if obj.articles:
             df=  pd.concat(
                 [
                     pd.DataFrame.from_dict(article["indexTerms"], orient="columns")
                     for article in obj.articles
                 ]
             )
-            df["domains"] =df["domains"].astype(str)
-            df = df[['name','domains']].value_counts().reset_index(name='count')
-            df['domains'] = df['domains'].str.strip("]['").str.split(', ')
-            #df = df.sort_values('count', ascending=False)
-            #return df
+            df['count'] = df.groupby(['name'])['domains'].transform('count')
+            df= df.drop(columns=['score','code'])
+            df = df.dropna()
+            df = df.drop_duplicates(['name'])
+            df = df.sort_values('count', ascending=False)
         else:
             print("no indexTerms to show!")
     if isinstance(obj, Article):
         indexterms_lst = obj.indexTerms
         for x in indexterms_lst:
             if not 'domains' in x:
                 x.remove(x)
```

### Comparing `lexisnexisapi-2.0.44/src/lexisnexisapi.egg-info/PKG-INFO` & `lexisnexisapi-2.0.45/src/lexisnexisapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexisnexisapi
-Version: 2.0.44
+Version: 2.0.45
 Summary: A small example package
 Home-page: 
 Author: Robert Cuffney
 Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
 License: MIT
 Keywords: example project
 Classifier: Programming Language :: Python :: 3
```

