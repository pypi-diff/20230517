# Comparing `tmp/sparclclient-1.2.0b4.dev0-py3-none-any.whl.zip` & `tmp/sparclclient-1.2.0b4.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 31659 bytes, number of entries: 20
+Zip file size: 31656 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx     8039 b- defN 23-Apr-30 18:22 sparcl/Results.py
--rw-rw-r--  2.0 unx     1035 b- defN 23-May-15 13:20 sparcl/__init__.py
+-rw-rw-r--  2.0 unx     1035 b- defN 23-May-17 15:29 sparcl/__init__.py
 -rw-rw-r--  2.0 unx      798 b- defN 23-Mar-15 14:12 sparcl/big_retrieve.py
 -rw-rw-r--  2.0 unx    29776 b- defN 23-May-15 13:11 sparcl/client.py
 -rw-rw-r--  2.0 unx      953 b- defN 23-Feb-08 18:38 sparcl/conf.py
 -rw-rw-r--  2.0 unx      887 b- defN 23-Mar-15 15:44 sparcl/dls_376.py
 -rw-rw-r--  2.0 unx     3813 b- defN 23-Apr-20 21:46 sparcl/exceptions.py
 -rw-rw-r--  2.0 unx     5002 b- defN 23-Mar-26 21:24 sparcl/fields.py
 -rw-rw-r--  2.0 unx     9254 b- defN 23-May-12 19:28 sparcl/gather_2d.py
 -rw-rw-r--  2.0 unx     1329 b- defN 23-Apr-30 15:12 sparcl/resample_spectra.py
 -rw-rw-r--  2.0 unx    13112 b- defN 23-Feb-08 18:38 sparcl/type_conversion.py
 -rw-rw-r--  2.0 unx     1867 b- defN 23-Feb-28 20:09 sparcl/unsupported.py
 -rw-rw-r--  2.0 unx     4682 b- defN 23-Mar-26 21:03 sparcl/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-08 18:38 sparcl/benchmarks/__init__.py
 -rw-rw-r--  2.0 unx     9667 b- defN 23-Feb-08 18:38 sparcl/benchmarks/benchmarks.py
--rw-rw-r--  2.0 unx     1576 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      872 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1601 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/RECORD
-20 files, 94362 bytes uncompressed, 29067 bytes compressed:  69.2%
+-rw-rw-r--  2.0 unx     1576 b- defN 23-May-17 15:30 sparclclient-1.2.0b4.dev1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      872 b- defN 23-May-17 15:30 sparclclient-1.2.0b4.dev1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-17 15:30 sparclclient-1.2.0b4.dev1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-17 15:30 sparclclient-1.2.0b4.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1601 b- defN 23-May-17 15:30 sparclclient-1.2.0b4.dev1.dist-info/RECORD
+20 files, 94362 bytes uncompressed, 29064 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: sparcl/benchmarks/__init__.py
 Comment: 
 
 Filename: sparcl/benchmarks/benchmarks.py
 Comment: 
 
-Filename: sparclclient-1.2.0b4.dev0.dist-info/LICENSE
+Filename: sparclclient-1.2.0b4.dev1.dist-info/LICENSE
 Comment: 
 
-Filename: sparclclient-1.2.0b4.dev0.dist-info/METADATA
+Filename: sparclclient-1.2.0b4.dev1.dist-info/METADATA
 Comment: 
 
-Filename: sparclclient-1.2.0b4.dev0.dist-info/WHEEL
+Filename: sparclclient-1.2.0b4.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: sparclclient-1.2.0b4.dev0.dist-info/top_level.txt
+Filename: sparclclient-1.2.0b4.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: sparclclient-1.2.0b4.dev0.dist-info/RECORD
+Filename: sparclclient-1.2.0b4.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparcl/__init__.py

```diff
@@ -27,8 +27,8 @@
 #__version__ = '1.0.0b1.dev7'
 #__version__ = '1.0.0b1.dev8'
 #__version__ = '1.0.0b1.dev9'
 #__version__ = '1.0.1b2.dev1'
 #__version__ = '1.1rc1'
 #__version__ = '1.1rc2'
 #__version__ = '1.1'
-__version__ = '1.2.0b4.dev0'
+__version__ = '1.2.0b4.dev1'
```

## Comparing `sparclclient-1.2.0b4.dev0.dist-info/LICENSE` & `sparclclient-1.2.0b4.dev1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparclclient-1.2.0b4.dev0.dist-info/METADATA` & `sparclclient-1.2.0b4.dev1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparclclient
-Version: 1.2.0b4.dev0
+Version: 1.2.0b4.dev1
 Summary: A client for getting spectra data from NOIRLab.
 Home-page: https://github.com/astro-datalab/sparclclient
 Author: NOIRLab DataLab
 Author-email: datalab-spectro@noirlab.edu
 Project-URL: Documentation, https://sparclclient.readthedocs.io/en/latest/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `sparclclient-1.2.0b4.dev0.dist-info/RECORD` & `sparclclient-1.2.0b4.dev1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 sparcl/Results.py,sha256=S4jQcXnw6qfdIEL-NEsCqMK6LolFaERGxjNWIvNhACM,8039
-sparcl/__init__.py,sha256=zTDqx1DZGxvXQ9ixlF3fwnBoK112erhc-7tJLpBwjdY,1035
+sparcl/__init__.py,sha256=8pb9RLVzuNau0xbGudM53BLKq2erRPV6ZIkavw12lkw,1035
 sparcl/big_retrieve.py,sha256=q0ScH87QqPL4bz4g0hB0AO3k4c_TiuQrWjBJHqHhE60,798
 sparcl/client.py,sha256=IEbXDqMsnMGcuhuSgvQNhVhwOdJgWFQDLcH68qp4dzE,29776
 sparcl/conf.py,sha256=O9l4-vpWBZK0QjhHxjskGO8kHPxBj7mkWlchd2rot1c,953
 sparcl/dls_376.py,sha256=WvZjuZFRU0jgH3ELRrMQdslkMWiF2wFQrSag0cYii-I,887
 sparcl/exceptions.py,sha256=q7ONsLsop9OQJJCD4SEzfdsojv0yo3WQT0SluaxGOQ0,3813
 sparcl/fields.py,sha256=7MpaJQr2d1GktS7aeM4010jyLqDdKQ7BZIF9hM0IjII,5002
 sparcl/gather_2d.py,sha256=ZRr41vNHV4tnf63-QuTu04SlWv6TOzK-CeHpbt9YwOY,9254
 sparcl/resample_spectra.py,sha256=2MO-sDCCFg2eNiK6jQs2EJRu4bNnXycGV8WaOydssG4,1329
 sparcl/type_conversion.py,sha256=RX7OD1iGuuUrf-yAd0ISdiqBq4CP7QlCw0vvkAdHdsQ,13112
 sparcl/unsupported.py,sha256=vkSaK3Ppcxx6mMsqBktUjI0uS7RwBJYH2BkBABsnyIM,1867
 sparcl/utils.py,sha256=YlLUP0j4thUyEwTJAaqJ7zzsvbCxPe5EYTn9kvWGfBY,4682
 sparcl/benchmarks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sparcl/benchmarks/benchmarks.py,sha256=FPZ2KExfVWHhGt3B4VyfgOhxxsemj7OeBWJO0dyDDC4,9667
-sparclclient-1.2.0b4.dev0.dist-info/LICENSE,sha256=y10EluGMCzGs9X4oYCYyix3l6u-lawB_vlGR8qe442Q,1576
-sparclclient-1.2.0b4.dev0.dist-info/METADATA,sha256=E9oVUvxzIgf8GLHD_0ET14UWRzmCcG2lR9u7p5iPvIg,872
-sparclclient-1.2.0b4.dev0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sparclclient-1.2.0b4.dev0.dist-info/top_level.txt,sha256=d5CZ3Duxq3MyQTB2ZqOrdtSBv4GdVceF-pOZFmsuHZY,7
-sparclclient-1.2.0b4.dev0.dist-info/RECORD,,
+sparclclient-1.2.0b4.dev1.dist-info/LICENSE,sha256=y10EluGMCzGs9X4oYCYyix3l6u-lawB_vlGR8qe442Q,1576
+sparclclient-1.2.0b4.dev1.dist-info/METADATA,sha256=QpqLubKFc30LpNbga7e7z22MlYhNeX2FfrkG-L9RuuQ,872
+sparclclient-1.2.0b4.dev1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sparclclient-1.2.0b4.dev1.dist-info/top_level.txt,sha256=d5CZ3Duxq3MyQTB2ZqOrdtSBv4GdVceF-pOZFmsuHZY,7
+sparclclient-1.2.0b4.dev1.dist-info/RECORD,,
```

