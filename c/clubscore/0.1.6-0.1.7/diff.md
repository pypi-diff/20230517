# Comparing `tmp/clubscore-0.1.6.tar.gz` & `tmp/clubscore-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clubscore-0.1.6.tar", last modified: Tue May 16 22:13:58 2023, max compression
+gzip compressed data, was "dist/clubscore-0.1.7.tar", last modified: Tue May 16 22:28:21 2023, max compression
```

## Comparing `clubscore-0.1.6.tar` & `clubscore-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:13:58.000000 clubscore-0.1.6/
--rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.6/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-16 22:13:58.000000 clubscore-0.1.6/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.6/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:13:58.000000 clubscore-0.1.6/clubscore/
--rw-r--r--   0 dave       (501) staff       (20)      752 2023-05-09 16:58:15.000000 clubscore-0.1.6/clubscore/API.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.6/clubscore/__init__.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:13:58.000000 clubscore-0.1.6/clubscore/objects/
--rw-r--r--   0 dave       (501) staff       (20)     5233 2023-05-16 22:07:16.000000 clubscore-0.1.6/clubscore/objects/CONTAINER.py
--rw-r--r--   0 dave       (501) staff       (20)     2408 2023-05-16 22:07:16.000000 clubscore-0.1.6/clubscore/objects/IMG.py
--rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.6/clubscore/objects/RECTANGLE.py
--rw-r--r--   0 dave       (501) staff       (20)     3945 2023-05-16 22:08:47.000000 clubscore-0.1.6/clubscore/objects/TEXT.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.6/clubscore/objects/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     3983 2023-05-16 22:12:51.000000 clubscore-0.1.6/clubscore/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:13:58.000000 clubscore-0.1.6/clubscore.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-16 22:13:58.000000 clubscore-0.1.6/clubscore.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      435 2023-05-16 22:13:58.000000 clubscore-0.1.6/clubscore.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-16 22:13:58.000000 clubscore-0.1.6/clubscore.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-16 22:13:58.000000 clubscore-0.1.6/clubscore.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-16 22:13:58.000000 clubscore-0.1.6/clubscore.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-16 22:13:58.000000 clubscore-0.1.6/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-16 22:13:57.000000 clubscore-0.1.6/setup.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:13:58.000000 clubscore-0.1.6/tests/
--rw-r--r--   0 dave       (501) staff       (20)     1961 2023-05-11 23:19:07.000000 clubscore-0.1.6/tests/test_templates.py
--rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.1.6/tests/test_utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:28:21.000000 clubscore-0.1.7/
+-rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.7/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-16 22:28:21.000000 clubscore-0.1.7/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.7/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:28:21.000000 clubscore-0.1.7/clubscore/
+-rw-r--r--   0 dave       (501) staff       (20)      752 2023-05-09 16:58:15.000000 clubscore-0.1.7/clubscore/API.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.7/clubscore/__init__.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:28:21.000000 clubscore-0.1.7/clubscore/objects/
+-rw-r--r--   0 dave       (501) staff       (20)     5233 2023-05-16 22:07:16.000000 clubscore-0.1.7/clubscore/objects/CONTAINER.py
+-rw-r--r--   0 dave       (501) staff       (20)     2408 2023-05-16 22:07:16.000000 clubscore-0.1.7/clubscore/objects/IMG.py
+-rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.7/clubscore/objects/RECTANGLE.py
+-rw-r--r--   0 dave       (501) staff       (20)     3966 2023-05-16 22:26:38.000000 clubscore-0.1.7/clubscore/objects/TEXT.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.7/clubscore/objects/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     4027 2023-05-16 22:26:38.000000 clubscore-0.1.7/clubscore/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:28:21.000000 clubscore-0.1.7/clubscore.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-16 22:28:21.000000 clubscore-0.1.7/clubscore.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      435 2023-05-16 22:28:21.000000 clubscore-0.1.7/clubscore.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-16 22:28:21.000000 clubscore-0.1.7/clubscore.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-16 22:28:21.000000 clubscore-0.1.7/clubscore.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-16 22:28:21.000000 clubscore-0.1.7/clubscore.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-16 22:28:21.000000 clubscore-0.1.7/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-16 22:27:53.000000 clubscore-0.1.7/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 22:28:21.000000 clubscore-0.1.7/tests/
+-rw-r--r--   0 dave       (501) staff       (20)     1961 2023-05-11 23:19:07.000000 clubscore-0.1.7/tests/test_templates.py
+-rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.1.7/tests/test_utils.py
```

### Comparing `clubscore-0.1.6/LICENSE` & `clubscore-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.6/PKG-INFO` & `clubscore-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.1.6/clubscore/API.py` & `clubscore-0.1.7/clubscore/API.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.6/clubscore/objects/CONTAINER.py` & `clubscore-0.1.7/clubscore/objects/CONTAINER.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.6/clubscore/objects/IMG.py` & `clubscore-0.1.7/clubscore/objects/IMG.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.6/clubscore/objects/RECTANGLE.py` & `clubscore-0.1.7/clubscore/objects/RECTANGLE.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.6/clubscore/objects/TEXT.py` & `clubscore-0.1.7/clubscore/objects/TEXT.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         if "testo" in dict:
             if "*" in dict["testo"]:
 
                 testo = lines.pop(0).strip()
 
                 if "match_word" in dict:
                     print(dict["match_word"])
-                    testo = u.matchWord(testo, u.getTeams(dict["match_word"]))
+                    testo = u.matchWord(testo, u.getTeamsFromTXT(dict["match_word"]))
 
                 if "upper" in dict and "True" in dict["upper"]:
                     testo = testo.upper()
 
                 dict["testo"] = dict["testo"].replace("*", testo)
 
             final_text = dict["testo"]
@@ -87,16 +87,17 @@
         elif "concatenation" in dict:
 
             for i in range(len(lines)):
                 repl = "{%s}" % str(i)
                 if repl in dict["concatenation"]:
                     testo = lines[i].strip()
 
-                    if "match_word" in dict and "True" in dict["match_word"]:
-                        testo = u.matchWord(testo, u.getTeams("graphics/teams/squadre.txt"))
+                    if "match_word" in dict:
+                        print(dict["match_word"])
+                        testo = u.matchWord(testo, u.getTeamsFromTXT(dict["match_word"]))
 
                     if "upper" in dict and "True" in dict["upper"]:
                         testo = testo.upper()
 
                     dict["concatenation"] = dict["concatenation"].replace(repl, testo)
```

### Comparing `clubscore-0.1.6/clubscore/utils.py` & `clubscore-0.1.7/clubscore/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,25 +98,28 @@
 
 """
 Recupera la lista delle squadre di cui si hanno le grafiche
 """
 
 
 def getTeams(path):
+    return list(map(lambda elem: elem.replace('.png', ''), os.listdir(path)))
+
+def getTeamsFromTXT(path):
     if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
         path = "../" + path
 
+    print(path)
+
     if ".txt" in path:
         f = open(path)
         f = f.readlines()
         f = [s.strip() for s in f]
         print(f)
         return f
-    return list(map(lambda elem: elem.replace('.png', ''), os.listdir(path)))
-
 
 
 def getTemplateText(template,s):
     if 'ENV' in os.environ and os.environ['ENV'] == 'testing':
         template = "../" + template
 
     tree = ET.parse(template)
```

### Comparing `clubscore-0.1.6/clubscore.egg-info/PKG-INFO` & `clubscore-0.1.7/clubscore.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.1.6/setup.py` & `clubscore-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clubscore',
-    version='0.1.6',
+    version='0.1.7',
     author='Davide Gimondo',
     author_email='davegimo@gmail.com',
     description='A package for creating customizable templates in XML',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clubscore',
     packages=find_packages(),
```

### Comparing `clubscore-0.1.6/tests/test_templates.py` & `clubscore-0.1.7/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.6/tests/test_utils.py` & `clubscore-0.1.7/tests/test_utils.py`

 * *Files identical despite different names*

