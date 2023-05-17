# Comparing `tmp/baba-0.1.5.tar.gz` & `tmp/baba-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baba-0.1.5.tar", last modified: Wed May 17 09:47:11 2023, max compression
+gzip compressed data, was "baba-0.1.6.tar", last modified: Wed May 17 10:24:09 2023, max compression
```

## Comparing `baba-0.1.5.tar` & `baba-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 09:47:11.018145 baba-0.1.5/
--rw-rw-rw-   0        0        0      165 2023-05-17 08:35:13.000000 baba-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1744 2023-05-17 09:47:11.016142 baba-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1330 2023-05-17 09:26:23.000000 baba-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 09:47:11.004176 baba-0.1.5/baba/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:52:03.000000 baba-0.1.5/baba/__init__.py
--rw-rw-rw-   0        0        0     2084 2023-05-17 08:20:22.000000 baba-0.1.5/baba/taskbase.py
--rw-rw-rw-   0        0        0      480 2023-05-17 08:36:00.000000 baba-0.1.5/baba/test.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:47:11.013126 baba-0.1.5/baba.egg-info/
--rw-rw-rw-   0        0        0     1744 2023-05-17 09:47:10.000000 baba-0.1.5/baba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-05-17 09:47:10.000000 baba-0.1.5/baba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 09:47:10.000000 baba-0.1.5/baba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-17 09:47:10.000000 baba-0.1.5/baba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 09:47:11.018145 baba-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      565 2023-05-17 09:46:59.000000 baba-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:24:09.685630 baba-0.1.6/
+-rw-rw-rw-   0        0        0      165 2023-05-17 08:35:13.000000 baba-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1771 2023-05-17 10:24:09.683627 baba-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1330 2023-05-17 09:26:23.000000 baba-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 10:24:09.671659 baba-0.1.6/baba/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:52:03.000000 baba-0.1.6/baba/__init__.py
+-rw-rw-rw-   0        0        0     2084 2023-05-17 08:20:22.000000 baba-0.1.6/baba/taskbase.py
+-rw-rw-rw-   0        0        0      480 2023-05-17 08:36:00.000000 baba-0.1.6/baba/test.py
+drwxrwxrwx   0        0        0        0 2023-05-17 10:24:09.680633 baba-0.1.6/baba.egg-info/
+-rw-rw-rw-   0        0        0     1771 2023-05-17 10:24:09.000000 baba-0.1.6/baba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-17 10:24:09.000000 baba-0.1.6/baba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 10:24:09.000000 baba-0.1.6/baba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-17 10:24:09.000000 baba-0.1.6/baba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 10:24:09.685630 baba-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-05-17 10:23:19.000000 baba-0.1.6/setup.py
```

### Comparing `baba-0.1.5/PKG-INFO` & `baba-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: baba
-Version: 0.1.5
-Summary: 好爸爸系列，追求朴素而踏实的实践。继承好爸爸的思想，轻松实现自动埋点、统计、错误处理、状态控制、任务流转、单元测试等功能
+Version: 0.1.6
+Summary: 好爸爸的每个类都是被用来继承的。作为顶层设计，它为通用行为实现了最基础的标准实践。比如自动埋点、性能分析、任务流转、异常处理、单元测试等。
 Home-page: https://pypi.org/project/baba/
 Author: jie.kim
 Author-email: ubbs@163.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `baba-0.1.5/README.md` & `baba-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `baba-0.1.5/baba/taskbase.py` & `baba-0.1.6/baba/taskbase.py`

 * *Files identical despite different names*

### Comparing `baba-0.1.5/baba.egg-info/PKG-INFO` & `baba-0.1.6/baba.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: baba
-Version: 0.1.5
-Summary: 好爸爸系列，追求朴素而踏实的实践。继承好爸爸的思想，轻松实现自动埋点、统计、错误处理、状态控制、任务流转、单元测试等功能
+Version: 0.1.6
+Summary: 好爸爸的每个类都是被用来继承的。作为顶层设计，它为通用行为实现了最基础的标准实践。比如自动埋点、性能分析、任务流转、异常处理、单元测试等。
 Home-page: https://pypi.org/project/baba/
 Author: jie.kim
 Author-email: ubbs@163.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

