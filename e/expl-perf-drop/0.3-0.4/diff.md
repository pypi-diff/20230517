# Comparing `tmp/expl_perf_drop-0.3.tar.gz` & `tmp/expl_perf_drop-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expl_perf_drop-0.3.tar", last modified: Wed May 17 08:24:44 2023, max compression
+gzip compressed data, was "expl_perf_drop-0.4.tar", last modified: Wed May 17 08:25:44 2023, max compression
```

## Comparing `expl_perf_drop-0.3.tar` & `expl_perf_drop-0.4.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxrwx---   0 hrzhang  (62021) hrzhang  (62021)        0 2023-05-17 08:24:44.000000 expl_perf_drop-0.3/
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     1069 2023-05-17 06:53:39.000000 expl_perf_drop-0.3/LICENSE
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      312 2023-05-17 08:24:44.000000 expl_perf_drop-0.3/PKG-INFO
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     2507 2023-05-17 08:20:13.000000 expl_perf_drop-0.3/README.md
-drwxrwx---   0 hrzhang  (62021) hrzhang  (62021)        0 2023-05-17 08:24:44.000000 expl_perf_drop-0.3/expl_perf_drop/
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     7968 2023-03-19 06:29:42.000000 expl_perf_drop-0.3/expl_perf_drop/KLIEP.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     3664 2023-05-17 06:54:28.000000 expl_perf_drop-0.3/expl_perf_drop/SHAPExplainer.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     8566 2023-05-17 07:37:53.000000 expl_perf_drop-0.3/expl_perf_drop/experiments.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     7907 2023-05-17 07:20:22.000000 expl_perf_drop-0.3/expl_perf_drop/explain.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     4568 2023-05-17 06:54:28.000000 expl_perf_drop-0.3/expl_perf_drop/explain_janzing.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)    15251 2023-05-17 07:10:17.000000 expl_perf_drop-0.3/expl_perf_drop/explainers.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     1784 2022-09-18 08:49:15.000000 expl_perf_drop-0.3/expl_perf_drop/launchers.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     2597 2023-05-16 03:40:09.000000 expl_perf_drop-0.3/expl_perf_drop/metrics.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     9883 2023-05-17 06:54:27.000000 expl_perf_drop-0.3/expl_perf_drop/models.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)    25183 2022-09-18 08:49:15.000000 expl_perf_drop-0.3/expl_perf_drop/shapley.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     7116 2023-05-17 06:54:27.000000 expl_perf_drop-0.3/expl_perf_drop/sweep.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     3428 2023-05-17 07:20:06.000000 expl_perf_drop-0.3/expl_perf_drop/train_model.py
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     8529 2023-01-21 23:15:12.000000 expl_perf_drop-0.3/expl_perf_drop/utils.py
-drwxrwx---   0 hrzhang  (62021) hrzhang  (62021)        0 2023-05-17 08:24:44.000000 expl_perf_drop-0.3/expl_perf_drop.egg-info/
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      312 2023-05-17 08:24:43.000000 expl_perf_drop-0.3/expl_perf_drop.egg-info/PKG-INFO
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      573 2023-05-17 08:24:43.000000 expl_perf_drop-0.3/expl_perf_drop.egg-info/SOURCES.txt
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)        1 2023-05-17 08:24:43.000000 expl_perf_drop-0.3/expl_perf_drop.egg-info/dependency_links.txt
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      111 2023-05-17 08:24:43.000000 expl_perf_drop-0.3/expl_perf_drop.egg-info/requires.txt
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)        1 2023-05-17 08:24:43.000000 expl_perf_drop-0.3/expl_perf_drop.egg-info/top_level.txt
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)       38 2023-05-17 08:24:44.000000 expl_perf_drop-0.3/setup.cfg
--rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      612 2023-05-17 08:24:04.000000 expl_perf_drop-0.3/setup.py
+drwxrwx---   0 hrzhang  (62021) hrzhang  (62021)        0 2023-05-17 08:25:44.000000 expl_perf_drop-0.4/
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     1069 2023-05-17 06:53:39.000000 expl_perf_drop-0.4/LICENSE
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      312 2023-05-17 08:25:44.000000 expl_perf_drop-0.4/PKG-INFO
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     2507 2023-05-17 08:20:13.000000 expl_perf_drop-0.4/README.md
+drwxrwx---   0 hrzhang  (62021) hrzhang  (62021)        0 2023-05-17 08:25:44.000000 expl_perf_drop-0.4/expl_perf_drop/
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     7968 2023-03-19 06:29:42.000000 expl_perf_drop-0.4/expl_perf_drop/KLIEP.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     3664 2023-05-17 06:54:28.000000 expl_perf_drop-0.4/expl_perf_drop/SHAPExplainer.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)        0 2023-05-17 08:25:35.000000 expl_perf_drop-0.4/expl_perf_drop/__init__.py
+drwxrwx---   0 hrzhang  (62021) hrzhang  (62021)        0 2023-05-17 08:25:44.000000 expl_perf_drop-0.4/expl_perf_drop/data/
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      594 2023-05-17 07:19:52.000000 expl_perf_drop-0.4/expl_perf_drop/data/__init__.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     4240 2023-05-17 07:21:30.000000 expl_perf_drop-0.4/expl_perf_drop/data/camelyon.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     4204 2023-05-17 06:54:28.000000 expl_perf_drop-0.4/expl_perf_drop/data/celebA.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     3420 2023-05-17 06:54:28.000000 expl_perf_drop-0.4/expl_perf_drop/data/cmnist.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     3901 2023-05-17 06:54:28.000000 expl_perf_drop-0.4/expl_perf_drop/data/eicu.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     2768 2023-05-17 06:54:28.000000 expl_perf_drop-0.4/expl_perf_drop/data/synthetic.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     8566 2023-05-17 07:37:53.000000 expl_perf_drop-0.4/expl_perf_drop/experiments.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     7907 2023-05-17 07:20:22.000000 expl_perf_drop-0.4/expl_perf_drop/explain.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     4568 2023-05-17 06:54:28.000000 expl_perf_drop-0.4/expl_perf_drop/explain_janzing.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)    15251 2023-05-17 07:10:17.000000 expl_perf_drop-0.4/expl_perf_drop/explainers.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     1784 2022-09-18 08:49:15.000000 expl_perf_drop-0.4/expl_perf_drop/launchers.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     2597 2023-05-16 03:40:09.000000 expl_perf_drop-0.4/expl_perf_drop/metrics.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     9883 2023-05-17 06:54:27.000000 expl_perf_drop-0.4/expl_perf_drop/models.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)    25183 2022-09-18 08:49:15.000000 expl_perf_drop-0.4/expl_perf_drop/shapley.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     7116 2023-05-17 06:54:27.000000 expl_perf_drop-0.4/expl_perf_drop/sweep.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     3428 2023-05-17 07:20:06.000000 expl_perf_drop-0.4/expl_perf_drop/train_model.py
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)     8529 2023-01-21 23:15:12.000000 expl_perf_drop-0.4/expl_perf_drop/utils.py
+drwxrwx---   0 hrzhang  (62021) hrzhang  (62021)        0 2023-05-17 08:25:44.000000 expl_perf_drop-0.4/expl_perf_drop.egg-info/
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      312 2023-05-17 08:25:43.000000 expl_perf_drop-0.4/expl_perf_drop.egg-info/PKG-INFO
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      785 2023-05-17 08:25:43.000000 expl_perf_drop-0.4/expl_perf_drop.egg-info/SOURCES.txt
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)        1 2023-05-17 08:25:43.000000 expl_perf_drop-0.4/expl_perf_drop.egg-info/dependency_links.txt
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      111 2023-05-17 08:25:43.000000 expl_perf_drop-0.4/expl_perf_drop.egg-info/requires.txt
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)       15 2023-05-17 08:25:43.000000 expl_perf_drop-0.4/expl_perf_drop.egg-info/top_level.txt
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)       38 2023-05-17 08:25:44.000000 expl_perf_drop-0.4/setup.cfg
+-rw-rw----   0 hrzhang  (62021) hrzhang  (62021)      612 2023-05-17 08:25:38.000000 expl_perf_drop-0.4/setup.py
```

### Comparing `expl_perf_drop-0.3/LICENSE` & `expl_perf_drop-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/README.md` & `expl_perf_drop-0.4/README.md`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/KLIEP.py` & `expl_perf_drop-0.4/expl_perf_drop/KLIEP.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/SHAPExplainer.py` & `expl_perf_drop-0.4/expl_perf_drop/SHAPExplainer.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/experiments.py` & `expl_perf_drop-0.4/expl_perf_drop/experiments.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/explain.py` & `expl_perf_drop-0.4/expl_perf_drop/explain.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/explain_janzing.py` & `expl_perf_drop-0.4/expl_perf_drop/explain_janzing.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/explainers.py` & `expl_perf_drop-0.4/expl_perf_drop/explainers.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/launchers.py` & `expl_perf_drop-0.4/expl_perf_drop/launchers.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/metrics.py` & `expl_perf_drop-0.4/expl_perf_drop/metrics.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/models.py` & `expl_perf_drop-0.4/expl_perf_drop/models.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/shapley.py` & `expl_perf_drop-0.4/expl_perf_drop/shapley.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/sweep.py` & `expl_perf_drop-0.4/expl_perf_drop/sweep.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/train_model.py` & `expl_perf_drop-0.4/expl_perf_drop/train_model.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop/utils.py` & `expl_perf_drop-0.4/expl_perf_drop/utils.py`

 * *Files identical despite different names*

### Comparing `expl_perf_drop-0.3/expl_perf_drop.egg-info/SOURCES.txt` & `expl_perf_drop-0.4/expl_perf_drop.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 expl_perf_drop/KLIEP.py
 expl_perf_drop/SHAPExplainer.py
+expl_perf_drop/__init__.py
 expl_perf_drop/experiments.py
 expl_perf_drop/explain.py
 expl_perf_drop/explain_janzing.py
 expl_perf_drop/explainers.py
 expl_perf_drop/launchers.py
 expl_perf_drop/metrics.py
 expl_perf_drop/models.py
@@ -14,8 +15,14 @@
 expl_perf_drop/sweep.py
 expl_perf_drop/train_model.py
 expl_perf_drop/utils.py
 expl_perf_drop.egg-info/PKG-INFO
 expl_perf_drop.egg-info/SOURCES.txt
 expl_perf_drop.egg-info/dependency_links.txt
 expl_perf_drop.egg-info/requires.txt
-expl_perf_drop.egg-info/top_level.txt
+expl_perf_drop.egg-info/top_level.txt
+expl_perf_drop/data/__init__.py
+expl_perf_drop/data/camelyon.py
+expl_perf_drop/data/celebA.py
+expl_perf_drop/data/cmnist.py
+expl_perf_drop/data/eicu.py
+expl_perf_drop/data/synthetic.py
```

### Comparing `expl_perf_drop-0.3/setup.py` & `expl_perf_drop-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 setup(name='expl_perf_drop',
-      version='0.3',
+      version='0.4',
       description='Attributing performance drops to distribution shifts',
       url='https://github.com/MLforHealth/expl_perf_drop',
       author='Haoran Zhang',
       author_email='haoranz@mit.edu',
       license='BSD',
       packages=find_packages(),
       python_requires='>=3.7',
```

