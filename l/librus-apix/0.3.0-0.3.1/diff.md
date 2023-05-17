# Comparing `tmp/librus_apix-0.3.0.tar.gz` & `tmp/librus_apix-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.3.0.tar", last modified: Fri Apr 21 20:44:00 2023, max compression
+gzip compressed data, was "librus_apix-0.3.1.tar", last modified: Wed May 17 16:21:17 2023, max compression
```

## Comparing `librus_apix-0.3.0.tar` & `librus_apix-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-21 20:44:00.805606 librus_apix-0.3.0/
--rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-04-21 20:43:44.000000 librus_apix-0.3.0/LICENSE
--rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-04-21 20:43:44.000000 librus_apix-0.3.0/LICENSE.orig
--rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-21 20:44:00.805606 librus_apix-0.3.0/PKG-INFO
--rw-r--r--   0 poro      (1000) poro      (1000)     2430 2023-04-21 20:43:44.000000 librus_apix-0.3.0/README.md
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-21 20:44:00.805606 librus_apix-0.3.0/librus_apix/
--rw-r--r--   0 poro      (1000) poro      (1000)      346 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/__init__.py
--rw-r--r--   0 poro      (1000) poro      (1000)     1156 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/announcements.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2810 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/attendance.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2810 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/completed_lessons.py
--rw-r--r--   0 poro      (1000) poro      (1000)      210 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/exceptions.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2367 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/get_token.py
--rw-r--r--   0 poro      (1000) poro      (1000)     4693 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/grades.py
--rw-r--r--   0 poro      (1000) poro      (1000)      287 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/helpers.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2175 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/homework.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2616 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/messages.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3053 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/schedule.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3098 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/timetable.py
--rw-r--r--   0 poro      (1000) poro      (1000)      480 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/urls.py
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-21 20:44:00.805606 librus_apix-0.3.0/librus_apix.egg-info/
--rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 poro      (1000) poro      (1000)      563 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 poro      (1000) poro      (1000)        1 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       18 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/requires.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       12 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       89 2023-04-21 20:43:44.000000 librus_apix-0.3.0/pyproject.toml
--rw-r--r--   0 poro      (1000) poro      (1000)      589 2023-04-21 20:44:00.808940 librus_apix-0.3.0/setup.cfg
--rw-r--r--   0 poro      (1000) poro      (1000)       37 2023-04-21 20:43:44.000000 librus_apix-0.3.0/setup.py
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-05-17 16:21:17.619382 librus_apix-0.3.1/
+-rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-05-17 16:21:03.000000 librus_apix-0.3.1/LICENSE
+-rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-05-17 16:21:03.000000 librus_apix-0.3.1/LICENSE.orig
+-rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-05-17 16:21:17.622714 librus_apix-0.3.1/PKG-INFO
+-rw-r--r--   0 poro      (1000) poro      (1000)     2430 2023-05-17 16:21:03.000000 librus_apix-0.3.1/README.md
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-05-17 16:21:17.619382 librus_apix-0.3.1/librus_apix/
+-rw-r--r--   0 poro      (1000) poro      (1000)      346 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/__init__.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     1156 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/announcements.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2810 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/attendance.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2810 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/completed_lessons.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      210 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/exceptions.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2367 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/get_token.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     4693 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/grades.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      287 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/helpers.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2175 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/homework.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2616 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/messages.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3053 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/schedule.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3098 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/timetable.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      480 2023-05-17 16:21:03.000000 librus_apix-0.3.1/librus_apix/urls.py
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-05-17 16:21:17.619382 librus_apix-0.3.1/librus_apix.egg-info/
+-rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-05-17 16:21:17.000000 librus_apix-0.3.1/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 poro      (1000) poro      (1000)      563 2023-05-17 16:21:17.000000 librus_apix-0.3.1/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)        1 2023-05-17 16:21:17.000000 librus_apix-0.3.1/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       18 2023-05-17 16:21:17.000000 librus_apix-0.3.1/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       12 2023-05-17 16:21:17.000000 librus_apix-0.3.1/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       89 2023-05-17 16:21:03.000000 librus_apix-0.3.1/pyproject.toml
+-rw-r--r--   0 poro      (1000) poro      (1000)      589 2023-05-17 16:21:17.622714 librus_apix-0.3.1/setup.cfg
+-rw-r--r--   0 poro      (1000) poro      (1000)       37 2023-05-17 16:21:03.000000 librus_apix-0.3.1/setup.py
```

### Comparing `librus_apix-0.3.0/LICENSE` & `librus_apix-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/LICENSE.orig` & `librus_apix-0.3.1/LICENSE.orig`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/README.md` & `librus_apix-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix/announcements.py` & `librus_apix-0.3.1/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix/attendance.py` & `librus_apix-0.3.1/librus_apix/attendance.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,18 @@
     )
     table = soup.find("table", attrs={"class": "center big decorated"})
     if table is None:
         raise ParseError("Error parsing attendance.")
     days = table.find_all("tr", attrs={"class": ["line0", "line1"]})
     current = ""
     att = [[], []]
-    semester = 1
+    semester = 2
     for day in days:
         if current == day.attrs["class"]:
-            semester = 2
+            semester = 1
         current = day.attrs["class"]
         date = day.find("td", attrs={"class": None})
         attendance = day.find_all("td", attrs={"class": "center"})
         for attend in attendance:
             at = attend.find_all("a")
             for single in at:
                 if not single:
```

### Comparing `librus_apix-0.3.0/librus_apix/completed_lessons.py` & `librus_apix-0.3.1/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix/get_token.py` & `librus_apix-0.3.1/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix/grades.py` & `librus_apix-0.3.1/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix/homework.py` & `librus_apix-0.3.1/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix/messages.py` & `librus_apix-0.3.1/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix/schedule.py` & `librus_apix-0.3.1/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix/timetable.py` & `librus_apix-0.3.1/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.3.1/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.3.0/setup.cfg` & `librus_apix-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.3.0
+version = 0.3.1
 license = MIT
 description = Web Scraper for Librus Synergia
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers = 
 	License :: OSI Approved :: MIT License
```

