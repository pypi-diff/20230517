# Comparing `tmp/hoyo-daily-logins-helper-2.4.0.tar.gz` & `tmp/hoyo-daily-logins-helper-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.4.0.tar", last modified: Wed May 17 03:01:32 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.4.1.tar", last modified: Wed May 17 03:13:18 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.4.0.tar` & `hoyo-daily-logins-helper-2.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.784653 hoyo-daily-logins-helper-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 03:01:32.000000 hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:01:32.788653 hoyo-daily-logins-helper-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:01:12.000000 hoyo-daily-logins-helper-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:13:18.655162 hoyo-daily-logins-helper-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:13:18.651162 hoyo-daily-logins-helper-2.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:13:18.655162 hoyo-daily-logins-helper-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-17 03:13:18.655162 hoyo-daily-logins-helper-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:13:18.655162 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 03:13:18.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:13:18.655162 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-17 03:13:18.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-17 03:13:18.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:13:18.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 03:13:18.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 03:13:18.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 03:13:18.000000 hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:13:18.655162 hoyo-daily-logins-helper-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:12:57.000000 hoyo-daily-logins-helper-2.4.1/setup.py
```

### Comparing `hoyo-daily-logins-helper-2.4.0/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.4.1/.github/workflows/deploy.yml`

 * *Files 23% similar despite different names*

```diff
@@ -27,16 +27,16 @@
       - uses: docker/build-push-action@v4
         with:
           context: .
           platforms: >-
             linux/amd64,
             linux/arm64
           push: true
-          tags: ${{ steps.meta.outputs.tags }}
-          labels: ${{ steps.meta.outputs.labels }}
+          tags: ${{ env.DOCKER_METADATA_OUTPUT_TAGS }}
+          labels: ${{ env.DOCKER_METADATA_OUTPUT_LABELS }}
 
   deploy-pypi:
     runs-on: ubuntu-latest
     permissions:
       id-token: write
     environment:
       name: pypi
```

### Comparing `hoyo-daily-logins-helper-2.4.0/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/.gitignore` & `hoyo-daily-logins-helper-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/LICENSE` & `hoyo-daily-logins-helper-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/PKG-INFO` & `hoyo-daily-logins-helper-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.4.0
+Version: 2.4.1
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.4.0/README.md` & `hoyo-daily-logins-helper-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/hoyo-daily-logins-helper.toml.template` & `hoyo-daily-logins-helper-2.4.1/hoyo-daily-logins-helper.toml.template`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/games.py` & `hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/games.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/http.py` & `hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/main.py` & `hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/main.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/notifications.py` & `hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/notifications.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper/scheduler.py` & `hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper/scheduler.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.4.0
+Version: 2.4.1
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.4.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.4.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/pyproject.toml` & `hoyo-daily-logins-helper-2.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.0/requirements.txt` & `hoyo-daily-logins-helper-2.4.1/requirements.txt`

 * *Files identical despite different names*

