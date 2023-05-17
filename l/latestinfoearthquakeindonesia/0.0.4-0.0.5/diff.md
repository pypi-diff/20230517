# Comparing `tmp/latestinfoearthquakeindonesia-0.0.4.tar.gz` & `tmp/latestinfoearthquakeindonesia-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latestinfoearthquakeindonesia-0.0.4.tar", last modified: Mon May 15 12:39:09 2023, max compression
+gzip compressed data, was "latestinfoearthquakeindonesia-0.0.5.tar", last modified: Wed May 17 12:00:22 2023, max compression
```

## Comparing `latestinfoearthquakeindonesia-0.0.4.tar` & `latestinfoearthquakeindonesia-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 12:39:09.626260 latestinfoearthquakeindonesia-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-05-10 11:57:41.000000 latestinfoearthquakeindonesia-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1215 2023-05-15 12:39:09.624255 latestinfoearthquakeindonesia-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      571 2023-05-15 12:36:14.000000 latestinfoearthquakeindonesia-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 12:39:09.567176 latestinfoearthquakeindonesia-0.0.4/gempaterkini/
--rw-rw-rw-   0        0        0     2521 2023-05-12 12:16:43.000000 latestinfoearthquakeindonesia-0.0.4/gempaterkini/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:39:09.619248 latestinfoearthquakeindonesia-0.0.4/latestinfoearthquakeindonesia.egg-info/
--rw-rw-rw-   0        0        0     1215 2023-05-15 12:39:09.000000 latestinfoearthquakeindonesia-0.0.4/latestinfoearthquakeindonesia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-05-15 12:39:09.000000 latestinfoearthquakeindonesia-0.0.4/latestinfoearthquakeindonesia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 12:39:09.000000 latestinfoearthquakeindonesia-0.0.4/latestinfoearthquakeindonesia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-15 12:39:09.000000 latestinfoearthquakeindonesia-0.0.4/latestinfoearthquakeindonesia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 12:39:09.627260 latestinfoearthquakeindonesia-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-05-15 12:36:30.000000 latestinfoearthquakeindonesia-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 12:00:22.521739 latestinfoearthquakeindonesia-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-10 11:57:41.000000 latestinfoearthquakeindonesia-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1215 2023-05-17 12:00:22.506112 latestinfoearthquakeindonesia-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2023-05-15 12:36:14.000000 latestinfoearthquakeindonesia-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 12:00:22.412360 latestinfoearthquakeindonesia-0.0.5/gempaterkini/
+-rw-rw-rw-   0        0        0     2647 2023-05-17 11:39:39.000000 latestinfoearthquakeindonesia-0.0.5/gempaterkini/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 12:00:22.506112 latestinfoearthquakeindonesia-0.0.5/latestinfoearthquakeindonesia.egg-info/
+-rw-rw-rw-   0        0        0     1215 2023-05-17 12:00:22.000000 latestinfoearthquakeindonesia-0.0.5/latestinfoearthquakeindonesia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-17 12:00:22.000000 latestinfoearthquakeindonesia-0.0.5/latestinfoearthquakeindonesia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 12:00:22.000000 latestinfoearthquakeindonesia-0.0.5/latestinfoearthquakeindonesia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 12:00:22.000000 latestinfoearthquakeindonesia-0.0.5/latestinfoearthquakeindonesia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 12:00:22.521739 latestinfoearthquakeindonesia-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-05-17 11:54:57.000000 latestinfoearthquakeindonesia-0.0.5/setup.py
```

### Comparing `latestinfoearthquakeindonesia-0.0.4/LICENSE` & `latestinfoearthquakeindonesia-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `latestinfoearthquakeindonesia-0.0.4/PKG-INFO` & `latestinfoearthquakeindonesia-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latestinfoearthquakeindonesia
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package will get the latest earthquake from BMKG | Meteorological, Climatological, and Geophysical Agency.
 Home-page: https://github.com/TOSS-ID/latest-indonesia-earthquake
 Author: Hendra Go
 Author-email: hendrago91@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `latestinfoearthquakeindonesia-0.0.4/README.md` & `latestinfoearthquakeindonesia-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `latestinfoearthquakeindonesia-0.0.4/gempaterkini/__init__.py` & `latestinfoearthquakeindonesia-0.0.5/gempaterkini/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import requests
 from bs4 import BeautifulSoup
 
+description = 'To get the latest Earthquake in Indonesia information from bmkg.go.id'
+
 
 def ekstraksi_data():
     """
     Tanggal: 04 Mei 2023
     Waktu: 21:22:03 WIB
     Magnitudo: 3.6
     Kedalaman: 10 km
@@ -45,16 +47,16 @@
                 bt = koordinat[1]
             elif i == 4:
                 lokasi = res.text
             elif i == 5:
                 dirasakan = res.text
             i = i + 1
 
-    #soup = BeautifulSoup(content)
-    #print(soup.prettify())
+#soup = BeautifulSoup(content)
+#print(soup.prettify())
 
         hasil = dict()
         hasil['tanggal'] = tanggal
         hasil['waktu'] = waktu
         hasil['magnitudo'] = magnitudo
         hasil['kedalaman'] = kedalaman
         hasil['koordinat'] = {'ls': ls, 'bt': bt}
@@ -75,11 +77,12 @@
     print(f"Magnitudo {result['magnitudo']}")
     print(f"Kedalaman {result['kedalaman']}")
     print(f"Lokasi {result['lokasi']}")
     print(f"Koordinat: LS={result['koordinat']['ls']}, BT={result['koordinat']['bt']}")
     print(f"Dirasakan {result['dirasakan']}")
 
 if __name__ == '__main__':
+    print('Deskripsi Package', description)
     result = ekstraksi_data()
     tampilkan_data(result)
 
 # print('ini adalah package gempaterkini')
```

### Comparing `latestinfoearthquakeindonesia-0.0.4/latestinfoearthquakeindonesia.egg-info/PKG-INFO` & `latestinfoearthquakeindonesia-0.0.5/latestinfoearthquakeindonesia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latestinfoearthquakeindonesia
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package will get the latest earthquake from BMKG | Meteorological, Climatological, and Geophysical Agency.
 Home-page: https://github.com/TOSS-ID/latest-indonesia-earthquake
 Author: Hendra Go
 Author-email: hendrago91@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `latestinfoearthquakeindonesia-0.0.4/setup.py` & `latestinfoearthquakeindonesia-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="latestinfoearthquakeindonesia",
-    version="0.0.4",
+    version="0.0.5",
     author="Hendra Go",
     author_email="hendrago91@gmail.com",
     description="This package will get the latest earthquake from BMKG | Meteorological, Climatological, and "
                 "Geophysical Agency.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TOSS-ID/latest-indonesia-earthquake",
```

