# Comparing `tmp/gptsubtitler-0.0.1.tar.gz` & `tmp/gptsubtitler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptsubtitler-0.0.1.tar", last modified: Wed May 17 08:23:57 2023, max compression
+gzip compressed data, was "gptsubtitler-0.0.2.tar", last modified: Wed May 17 08:26:25 2023, max compression
```

## Comparing `gptsubtitler-0.0.1.tar` & `gptsubtitler-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 08:23:57.921925 gptsubtitler-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      384 2023-05-17 08:23:57.921925 gptsubtitler-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2333 2023-05-17 07:35:00.000000 gptsubtitler-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 08:23:57.901872 gptsubtitler-0.0.1/gptsubtitler/
--rw-rw-rw-   0        0        0       36 2023-05-17 08:04:46.000000 gptsubtitler-0.0.1/gptsubtitler/__init__.py
--rw-rw-rw-   0        0        0     5496 2023-05-17 07:50:23.000000 gptsubtitler-0.0.1/gptsubtitler/transcriber.py
--rw-rw-rw-   0        0        0     4030 2023-05-17 07:39:13.000000 gptsubtitler-0.0.1/gptsubtitler/translator.py
--rw-rw-rw-   0        0        0     1360 2023-05-17 07:38:36.000000 gptsubtitler-0.0.1/gptsubtitler/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:23:57.920926 gptsubtitler-0.0.1/gptsubtitler.egg-info/
--rw-rw-rw-   0        0        0      384 2023-05-17 08:23:57.000000 gptsubtitler-0.0.1/gptsubtitler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-05-17 08:23:57.000000 gptsubtitler-0.0.1/gptsubtitler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 08:23:57.000000 gptsubtitler-0.0.1/gptsubtitler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-17 08:23:57.000000 gptsubtitler-0.0.1/gptsubtitler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 08:23:57.000000 gptsubtitler-0.0.1/gptsubtitler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 08:23:57.921925 gptsubtitler-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-05-17 08:23:37.000000 gptsubtitler-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:26:25.860806 gptsubtitler-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-17 07:34:14.000000 gptsubtitler-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2760 2023-05-17 08:26:25.860806 gptsubtitler-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2333 2023-05-17 07:35:00.000000 gptsubtitler-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 08:26:25.844881 gptsubtitler-0.0.2/gptsubtitler/
+-rw-rw-rw-   0        0        0       36 2023-05-17 08:04:46.000000 gptsubtitler-0.0.2/gptsubtitler/__init__.py
+-rw-rw-rw-   0        0        0     5496 2023-05-17 07:50:23.000000 gptsubtitler-0.0.2/gptsubtitler/transcriber.py
+-rw-rw-rw-   0        0        0     4030 2023-05-17 07:39:13.000000 gptsubtitler-0.0.2/gptsubtitler/translator.py
+-rw-rw-rw-   0        0        0     1360 2023-05-17 07:38:36.000000 gptsubtitler-0.0.2/gptsubtitler/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:26:25.859806 gptsubtitler-0.0.2/gptsubtitler.egg-info/
+-rw-rw-rw-   0        0        0     2760 2023-05-17 08:26:25.000000 gptsubtitler-0.0.2/gptsubtitler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-05-17 08:26:25.000000 gptsubtitler-0.0.2/gptsubtitler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 08:26:25.000000 gptsubtitler-0.0.2/gptsubtitler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-17 08:26:25.000000 gptsubtitler-0.0.2/gptsubtitler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 08:26:25.000000 gptsubtitler-0.0.2/gptsubtitler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 08:26:25.860806 gptsubtitler-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      684 2023-05-17 08:26:23.000000 gptsubtitler-0.0.2/setup.py
```

### Comparing `gptsubtitler-0.0.1/LICENSE` & `gptsubtitler-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.1/README.md` & `gptsubtitler-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.1/gptsubtitler/transcriber.py` & `gptsubtitler-0.0.2/gptsubtitler/transcriber.py`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.1/gptsubtitler/translator.py` & `gptsubtitler-0.0.2/gptsubtitler/translator.py`

 * *Files identical despite different names*

### Comparing `gptsubtitler-0.0.1/gptsubtitler/video_utils.py` & `gptsubtitler-0.0.2/gptsubtitler/video_utils.py`

 * *Files identical despite different names*

