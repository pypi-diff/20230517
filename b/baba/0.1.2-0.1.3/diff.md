# Comparing `tmp/baba-0.1.2.tar.gz` & `tmp/baba-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baba-0.1.2.tar", last modified: Wed May 17 09:34:14 2023, max compression
+gzip compressed data, was "baba-0.1.3.tar", last modified: Wed May 17 09:36:32 2023, max compression
```

## Comparing `baba-0.1.2.tar` & `baba-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 09:34:14.967904 baba-0.1.2/
--rw-rw-rw-   0        0        0      165 2023-05-17 08:35:13.000000 baba-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1744 2023-05-17 09:34:14.965878 baba-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1330 2023-05-17 09:26:23.000000 baba-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 09:34:14.952392 baba-0.1.2/baba/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:52:03.000000 baba-0.1.2/baba/__init__.py
--rw-rw-rw-   0        0        0     2084 2023-05-17 08:20:22.000000 baba-0.1.2/baba/taskbase.py
--rw-rw-rw-   0        0        0      480 2023-05-17 08:36:00.000000 baba-0.1.2/baba/test.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:34:14.963883 baba-0.1.2/baba.egg-info/
--rw-rw-rw-   0        0        0     1744 2023-05-17 09:34:14.000000 baba-0.1.2/baba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-05-17 09:34:14.000000 baba-0.1.2/baba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 09:34:14.000000 baba-0.1.2/baba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-17 09:34:14.000000 baba-0.1.2/baba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 09:34:14.968870 baba-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      565 2023-05-17 09:33:47.000000 baba-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:36:32.811829 baba-0.1.3/
+-rw-rw-rw-   0        0        0      165 2023-05-17 08:35:13.000000 baba-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1744 2023-05-17 09:36:32.809835 baba-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1330 2023-05-17 09:26:23.000000 baba-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 09:36:32.797866 baba-0.1.3/baba/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:52:03.000000 baba-0.1.3/baba/__init__.py
+-rw-rw-rw-   0        0        0     2084 2023-05-17 08:20:22.000000 baba-0.1.3/baba/taskbase.py
+-rw-rw-rw-   0        0        0      480 2023-05-17 08:36:00.000000 baba-0.1.3/baba/test.py
+drwxrwxrwx   0        0        0        0 2023-05-17 09:36:32.807840 baba-0.1.3/baba.egg-info/
+-rw-rw-rw-   0        0        0     1744 2023-05-17 09:36:32.000000 baba-0.1.3/baba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-17 09:36:32.000000 baba-0.1.3/baba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 09:36:32.000000 baba-0.1.3/baba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-17 09:36:32.000000 baba-0.1.3/baba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 09:36:32.811829 baba-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      565 2023-05-17 09:36:27.000000 baba-0.1.3/setup.py
```

### Comparing `baba-0.1.2/PKG-INFO` & `baba-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baba
-Version: 0.1.2
+Version: 0.1.3
 Summary: 好爸爸系列，追求朴素而踏实的实践。继承好爸爸的思想，轻松实现自动埋点、统计、错误处理、状态控制、任务流转、单元测试等功能
 Home-page: https://pypi.org/project/baba/
 Author: jie.kim
 Author-email: ubbs@163.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `baba-0.1.2/README.md` & `baba-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `baba-0.1.2/baba/taskbase.py` & `baba-0.1.3/baba/taskbase.py`

 * *Files identical despite different names*

### Comparing `baba-0.1.2/baba.egg-info/PKG-INFO` & `baba-0.1.3/baba.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baba
-Version: 0.1.2
+Version: 0.1.3
 Summary: 好爸爸系列，追求朴素而踏实的实践。继承好爸爸的思想，轻松实现自动埋点、统计、错误处理、状态控制、任务流转、单元测试等功能
 Home-page: https://pypi.org/project/baba/
 Author: jie.kim
 Author-email: ubbs@163.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `baba-0.1.2/setup.py` & `baba-0.1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="baba",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     author="jie.kim",
     author_email="ubbs@163.com",
     license='MIT',
     description="好爸爸系列，追求朴素而踏实的实践。继承好爸爸的思想，轻松实现自动埋点、统计、错误处理、状态控制、任务流转、单元测试等功能",
     long_description=open('README.md',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
```

