# Comparing `tmp/pip-setting-0.0.9.tar.gz` & `tmp/pip-setting-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-setting-0.0.9.tar", last modified: Thu Jun  3 04:40:51 2021, max compression
+gzip compressed data, was "pip-setting-1.0.0.tar", last modified: Wed May 17 13:25:07 2023, max compression
```

## Comparing `pip-setting-0.0.9.tar` & `pip-setting-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-06-03 04:40:51.855239 pip-setting-0.0.9/
--rw-rw-rw-   0        0        0     1165 2021-06-03 04:40:51.854241 pip-setting-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      503 2021-06-03 04:27:08.000000 pip-setting-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2021-06-03 04:40:51.843270 pip-setting-0.0.9/pip_setting/
--rw-rw-rw-   0        0        0     1540 2021-06-03 04:39:25.000000 pip-setting-0.0.9/pip_setting/__init__.py
--rw-rw-rw-   0        0        0      633 2021-06-03 04:39:25.000000 pip-setting-0.0.9/pip_setting/mirrors.json
-drwxrwxrwx   0        0        0        0 2021-06-03 04:40:51.853244 pip-setting-0.0.9/pip_setting.egg-info/
--rw-rw-rw-   0        0        0     1165 2021-06-03 04:40:51.000000 pip-setting-0.0.9/pip_setting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2021-06-03 04:40:51.000000 pip-setting-0.0.9/pip_setting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-03 04:40:51.000000 pip-setting-0.0.9/pip_setting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2021-06-03 04:40:51.000000 pip-setting-0.0.9/pip_setting.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2021-06-03 04:40:51.000000 pip-setting-0.0.9/pip_setting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-06-03 04:40:51.855239 pip-setting-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      926 2021-06-03 04:39:25.000000 pip-setting-0.0.9/setup.py
+drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2023-05-17 13:25:07.046181 pip-setting-1.0.0/
+-rw-r--r--   0 qiujiajin   (501) staff       (20)     1061 2023-05-17 13:21:18.000000 pip-setting-1.0.0/LICENSE
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      810 2023-05-17 13:25:07.045975 pip-setting-1.0.0/PKG-INFO
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      399 2023-05-17 13:23:12.000000 pip-setting-1.0.0/README.md
+drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2023-05-17 13:25:07.044472 pip-setting-1.0.0/pip_setting/
+-rw-r--r--   0 qiujiajin   (501) staff       (20)     1540 2023-05-17 13:21:18.000000 pip-setting-1.0.0/pip_setting/__init__.py
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      775 2023-05-17 13:21:18.000000 pip-setting-1.0.0/pip_setting/mirrors.json
+drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2023-05-17 13:25:07.045570 pip-setting-1.0.0/pip_setting.egg-info/
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      810 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/PKG-INFO
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      253 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/SOURCES.txt
+-rw-r--r--   0 qiujiajin   (501) staff       (20)        1 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/dependency_links.txt
+-rw-r--r--   0 qiujiajin   (501) staff       (20)       78 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/entry_points.txt
+-rw-r--r--   0 qiujiajin   (501) staff       (20)       12 2023-05-17 13:25:07.000000 pip-setting-1.0.0/pip_setting.egg-info/top_level.txt
+-rw-r--r--   0 qiujiajin   (501) staff       (20)       38 2023-05-17 13:25:07.046276 pip-setting-1.0.0/setup.cfg
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      926 2023-05-17 13:23:26.000000 pip-setting-1.0.0/setup.py
```

### Comparing `pip-setting-0.0.9/pip_setting/__init__.py` & `pip-setting-1.0.0/pip_setting/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-setting-0.0.9/pip_setting/mirrors.json` & `pip-setting-1.0.0/pip_setting/mirrors.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'上海交大'": "OrderedDict([('global', 'index-url = https://mirror.sjtu.edu.cn/pypi/web/simple'), "*

 * *           "('install', 'trusted-host=mirror.sjtu.edu.cn')])"}*

```diff
@@ -1,8 +1,12 @@
 {
+    "\u4e0a\u6d77\u4ea4\u5927": {
+        "global": "index-url = https://mirror.sjtu.edu.cn/pypi/web/simple",
+        "install": "trusted-host=mirror.sjtu.edu.cn"
+    },
     "\u6e05\u534e": {
         "global": "index-url = https://pypi.tuna.tsinghua.edu.cn/simple",
         "install": "trusted-host=pypi.tuna.tsinghua.edu.cn"
     },
     "\u817e\u8baf\u4e91": {
         "global": "index-url = https://mirrors.cloud.tencent.com/pypi/simple",
         "install": "trusted-host=mirrors.cloud.tencent.com"
```

### Comparing `pip-setting-0.0.9/setup.py` & `pip-setting-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.core import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pip-setting',
-    version='0.0.9',
+    version='1.0.0',
     author='丘家劲',
     author_email='609799548@qq.com',
     description='快速设置pip镜像源的工具',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/13528080556/pip_setting',
```

