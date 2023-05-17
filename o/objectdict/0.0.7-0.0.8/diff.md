# Comparing `tmp/objectdict-0.0.7.tar.gz` & `tmp/objectdict-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/objectdict-0.0.7.tar", last modified: Thu Mar 11 03:46:39 2021, max compression
+gzip compressed data, was "objectdict-0.0.8.tar", last modified: Wed May 17 02:41:55 2023, max compression
```

## Comparing `objectdict-0.0.7.tar` & `objectdict-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xzr        (501) staff       (20)        0 2021-03-11 03:46:39.000000 objectdict-0.0.7/
--rw-r--r--   0 xzr        (501) staff       (20)      435 2021-03-11 03:46:39.000000 objectdict-0.0.7/PKG-INFO
--rw-r--r--   0 xzr        (501) staff       (20)        0 2020-11-24 03:15:34.000000 objectdict-0.0.7/requirements.txt
--rw-r--r--   0 xzr        (501) staff       (20)        0 2021-01-13 04:41:40.000000 objectdict-0.0.7/README.md
-drwxr-xr-x   0 xzr        (501) staff       (20)        0 2021-03-11 03:46:39.000000 objectdict-0.0.7/objectdict.egg-info/
--rw-r--r--   0 xzr        (501) staff       (20)      435 2021-03-11 03:46:38.000000 objectdict-0.0.7/objectdict.egg-info/PKG-INFO
--rw-r--r--   0 xzr        (501) staff       (20)      185 2021-03-11 03:46:38.000000 objectdict-0.0.7/objectdict.egg-info/SOURCES.txt
--rw-r--r--   0 xzr        (501) staff       (20)       11 2021-03-11 03:46:38.000000 objectdict-0.0.7/objectdict.egg-info/top_level.txt
--rw-r--r--   0 xzr        (501) staff       (20)        1 2021-03-11 03:46:38.000000 objectdict-0.0.7/objectdict.egg-info/dependency_links.txt
--rw-r--r--   0 xzr        (501) staff       (20)     1672 2021-03-11 03:44:14.000000 objectdict-0.0.7/setup.py
--rw-r--r--   0 xzr        (501) staff       (20)      893 2021-03-11 03:44:10.000000 objectdict-0.0.7/objectdict.py
--rw-r--r--   0 xzr        (501) staff       (20)       38 2021-03-11 03:46:39.000000 objectdict-0.0.7/setup.cfg
+drwxr-xr-x   0 xiezhaorong   (501) staff       (20)        0 2023-05-17 02:41:55.648321 objectdict-0.0.8/
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)     1319 2023-05-17 02:41:55.648196 objectdict-0.0.8/PKG-INFO
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)      902 2023-05-17 02:29:00.000000 objectdict-0.0.8/README.md
+drwxr-xr-x   0 xiezhaorong   (501) staff       (20)        0 2023-05-17 02:41:55.648038 objectdict-0.0.8/objectdict.egg-info/
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)     1319 2023-05-17 02:41:55.000000 objectdict-0.0.8/objectdict.egg-info/PKG-INFO
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)      185 2023-05-17 02:41:55.000000 objectdict-0.0.8/objectdict.egg-info/SOURCES.txt
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)        1 2023-05-17 02:41:55.000000 objectdict-0.0.8/objectdict.egg-info/dependency_links.txt
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)       11 2023-05-17 02:41:55.000000 objectdict-0.0.8/objectdict.egg-info/top_level.txt
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)      996 2023-05-17 02:26:59.000000 objectdict-0.0.8/objectdict.py
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)        0 2023-05-17 02:09:10.000000 objectdict-0.0.8/requirements.txt
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)       38 2023-05-17 02:41:55.648356 objectdict-0.0.8/setup.cfg
+-rw-r--r--   0 xiezhaorong   (501) staff       (20)     2225 2023-05-17 02:41:40.000000 objectdict-0.0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `objectdict-0.0.7/setup.py` & `objectdict-0.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,37 @@
 # -*- coding: utf-8 -*-
 # https://blog.konghy.cn/2018/04/29/setup-dot-py/
+import shutil
+
 import setuptools
+import sys
+import os
+
+if sys.argv[-1] == 'publish':
+    if os.system("pip freeze | grep twine"):
+        print("twine not installed.\nUse `pip install twine`.\nExiting.")
+        sys.exit()
+    os.system("python setup.py sdist bdist_wheel")
+    if os.system("twine check dist/*"):
+        print("twine check failed. Packages might be outdated.")
+        print("Try using `pip install -U twine wheel`.\nExiting.")
+        sys.exit()
+    os.system("twine upload dist/*")
+    shutil.rmtree('dist')
+    shutil.rmtree('build')
+
+    sys.exit()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 install_requires = [l.strip() for l in open('./requirements.txt').readlines() if l.strip()]
 setuptools.setup(
         name="objectdict",  # 包的分发名称，使用字母、数字、_、-
-        version="0.0.7",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+        version="0.0.8",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
         author="xzregg",  # 作者名字
         author_email="xzregg@gmail.com",  # 作者邮箱
         description="objectdict",  # 包的简介描述
         long_description=long_description,  # 包的详细介绍(一般通过加载README.md)
         long_description_content_type="text/markdown",  # 和上条命令配合使用，声明加载的是markdown文件
         url="https://github.com/xzregg/pyobjectdict",  # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
         py_modules=['objectdict'],
```

