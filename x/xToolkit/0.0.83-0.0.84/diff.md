# Comparing `tmp/xToolkit-0.0.83.tar.gz` & `tmp/xToolkit-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xToolkit-0.0.83.tar", last modified: Mon Mar 20 06:43:27 2023, max compression
+gzip compressed data, was "dist\xToolkit-0.0.84.tar", last modified: Wed May 17 07:42:36 2023, max compression
```

## Comparing `xToolkit-0.0.83.tar` & `xToolkit-0.0.84.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.993680 xToolkit-0.0.83/
--rw-rw-rw-   0        0        0    25508 2023-03-20 06:43:27.993680 xToolkit-0.0.83/PKG-INFO
--rw-rw-rw-   0        0        0    25218 2023-03-20 06:37:50.000000 xToolkit-0.0.83/README.md
--rw-rw-rw-   0        0        0       42 2023-03-20 06:43:27.993680 xToolkit-0.0.83/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-03-20 06:42:21.000000 xToolkit-0.0.83/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.880632 xToolkit-0.0.83/xToolkit/
--rw-rw-rw-   0        0        0      558 2022-07-06 09:57:21.000000 xToolkit-0.0.83/xToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.893319 xToolkit-0.0.83/xToolkit/xdatetime/
--rw-rw-rw-   0        0        0      313 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xdatetime/__init__.py
--rw-rw-rw-   0        0        0     3289 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xdatetime/api.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.907562 xToolkit-0.0.83/xToolkit/xdatetime/xdatetime/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xdatetime/xdatetime/__init__.py
--rw-rw-rw-   0        0        0    13012 2022-07-06 08:51:30.000000 xToolkit-0.0.83/xToolkit/xdatetime/xdatetime/xdatetime.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.911342 xToolkit-0.0.83/xToolkit/xfile/
--rw-rw-rw-   0        0        0      320 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xfile/__init__.py
--rw-rw-rw-   0        0        0      976 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xfile/api.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.914524 xToolkit-0.0.83/xToolkit/xfile/dispose/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xfile/dispose/__init__.py
--rw-rw-rw-   0        0        0     4771 2022-07-06 09:15:56.000000 xToolkit-0.0.83/xToolkit/xfile/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.928081 xToolkit-0.0.83/xToolkit/xhotchpotch/
--rw-rw-rw-   0        0        0      356 2022-07-06 09:43:23.000000 xToolkit-0.0.83/xToolkit/xhotchpotch/__init__.py
--rw-rw-rw-   0        0        0      907 2022-07-07 01:20:46.000000 xToolkit-0.0.83/xToolkit/xhotchpotch/api.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.938403 xToolkit-0.0.83/xToolkit/xhotchpotch/dispose/
--rw-rw-rw-   0        0        0        0 2022-07-06 09:19:47.000000 xToolkit-0.0.83/xToolkit/xhotchpotch/dispose/__init__.py
--rw-rw-rw-   0        0        0     1773 2022-07-07 01:20:46.000000 xToolkit-0.0.83/xToolkit/xhotchpotch/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.953222 xToolkit-0.0.83/xToolkit/xlist/
--rw-rw-rw-   0        0        0      329 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xlist/__init__.py
--rw-rw-rw-   0        0        0      903 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xlist/api.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.956220 xToolkit-0.0.83/xToolkit/xlist/dispose/
--rw-rw-rw-   0        0        0      268 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xlist/dispose/__init__.py
--rw-rw-rw-   0        0        0     1636 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xlist/dispose/dispose.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.966421 xToolkit-0.0.83/xToolkit/xstring/
--rw-rw-rw-   0        0        0      338 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xstring/__init__.py
--rw-rw-rw-   0        0        0     1818 2022-08-10 07:14:52.000000 xToolkit-0.0.83/xToolkit/xstring/api.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.975048 xToolkit-0.0.83/xToolkit/xstring/check/
--rw-rw-rw-   0        0        0      255 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xstring/check/__init__.py
--rw-rw-rw-   0        0        0    11609 2023-03-20 06:16:13.000000 xToolkit-0.0.83/xToolkit/xstring/check/check.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.978047 xToolkit-0.0.83/xToolkit/xstring/dispose/
--rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xstring/dispose/__init__.py
--rw-rw-rw-   0        0        0     5693 2022-07-06 08:41:33.000000 xToolkit-0.0.83/xToolkit/xstring/dispose/dispose.py
--rw-rw-rw-   0        0        0     3648 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xstring/xstring.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.981305 xToolkit-0.0.83/xToolkit/xthreading/
--rw-rw-rw-   0        0        0      293 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xthreading/__init__.py
--rw-rw-rw-   0        0        0     1727 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xthreading/xthread.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.992044 xToolkit-0.0.83/xToolkit/xtoolkit/
--rw-rw-rw-   0        0        0      254 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xtoolkit/__init__.py
--rw-rw-rw-   0        0        0     3108 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xtoolkit/judgement.py
--rw-rw-rw-   0        0        0      441 2022-07-06 07:25:01.000000 xToolkit-0.0.83/xToolkit/xtoolkit/xtoolkit.py
-drwxrwxrwx   0        0        0        0 2023-03-20 06:43:27.889919 xToolkit-0.0.83/xToolkit.egg-info/
--rw-rw-rw-   0        0        0    25508 2023-03-20 06:43:27.000000 xToolkit-0.0.83/xToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-03-20 06:43:27.000000 xToolkit-0.0.83/xToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 06:43:27.000000 xToolkit-0.0.83/xToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-03-20 06:43:27.000000 xToolkit-0.0.83/xToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-20 06:43:27.000000 xToolkit-0.0.83/xToolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.797854 xToolkit-0.0.84/
+-rw-rw-rw-   0        0        0    25597 2023-05-17 07:42:36.797854 xToolkit-0.0.84/PKG-INFO
+-rw-rw-rw-   0        0        0    25307 2023-05-17 07:34:59.000000 xToolkit-0.0.84/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:42:36.797854 xToolkit-0.0.84/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-05-17 07:37:10.000000 xToolkit-0.0.84/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.694696 xToolkit-0.0.84/xToolkit/
+-rw-rw-rw-   0        0        0      558 2022-07-06 09:57:21.000000 xToolkit-0.0.84/xToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.705722 xToolkit-0.0.84/xToolkit/xdatetime/
+-rw-rw-rw-   0        0        0      313 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xdatetime/__init__.py
+-rw-rw-rw-   0        0        0     3289 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xdatetime/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.727514 xToolkit-0.0.84/xToolkit/xdatetime/xdatetime/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xdatetime/xdatetime/__init__.py
+-rw-rw-rw-   0        0        0    13012 2022-07-06 08:51:30.000000 xToolkit-0.0.84/xToolkit/xdatetime/xdatetime/xdatetime.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.731945 xToolkit-0.0.84/xToolkit/xfile/
+-rw-rw-rw-   0        0        0      320 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xfile/__init__.py
+-rw-rw-rw-   0        0        0      976 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xfile/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.734944 xToolkit-0.0.84/xToolkit/xfile/dispose/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xfile/dispose/__init__.py
+-rw-rw-rw-   0        0        0     4771 2022-07-06 09:15:56.000000 xToolkit-0.0.84/xToolkit/xfile/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.748558 xToolkit-0.0.84/xToolkit/xhotchpotch/
+-rw-rw-rw-   0        0        0      356 2022-07-06 09:43:23.000000 xToolkit-0.0.84/xToolkit/xhotchpotch/__init__.py
+-rw-rw-rw-   0        0        0      907 2022-07-07 01:20:46.000000 xToolkit-0.0.84/xToolkit/xhotchpotch/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.759631 xToolkit-0.0.84/xToolkit/xhotchpotch/dispose/
+-rw-rw-rw-   0        0        0        0 2022-07-06 09:19:47.000000 xToolkit-0.0.84/xToolkit/xhotchpotch/dispose/__init__.py
+-rw-rw-rw-   0        0        0     1773 2022-07-07 01:20:46.000000 xToolkit-0.0.84/xToolkit/xhotchpotch/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.766071 xToolkit-0.0.84/xToolkit/xlist/
+-rw-rw-rw-   0        0        0      329 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xlist/__init__.py
+-rw-rw-rw-   0        0        0      903 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xlist/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.769071 xToolkit-0.0.84/xToolkit/xlist/dispose/
+-rw-rw-rw-   0        0        0      268 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xlist/dispose/__init__.py
+-rw-rw-rw-   0        0        0     1636 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xlist/dispose/dispose.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.773073 xToolkit-0.0.84/xToolkit/xstring/
+-rw-rw-rw-   0        0        0      338 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xstring/__init__.py
+-rw-rw-rw-   0        0        0     1818 2023-05-17 07:33:53.000000 xToolkit-0.0.84/xToolkit/xstring/api.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.780142 xToolkit-0.0.84/xToolkit/xstring/check/
+-rw-rw-rw-   0        0        0      255 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xstring/check/__init__.py
+-rw-rw-rw-   0        0        0    12135 2023-05-17 07:33:53.000000 xToolkit-0.0.84/xToolkit/xstring/check/check.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.783151 xToolkit-0.0.84/xToolkit/xstring/dispose/
+-rw-rw-rw-   0        0        0      260 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xstring/dispose/__init__.py
+-rw-rw-rw-   0        0        0     5693 2022-07-06 08:41:33.000000 xToolkit-0.0.84/xToolkit/xstring/dispose/dispose.py
+-rw-rw-rw-   0        0        0     3648 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xstring/xstring.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.786109 xToolkit-0.0.84/xToolkit/xthreading/
+-rw-rw-rw-   0        0        0      293 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xthreading/__init__.py
+-rw-rw-rw-   0        0        0     1727 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xthreading/xthread.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.796186 xToolkit-0.0.84/xToolkit/xtoolkit/
+-rw-rw-rw-   0        0        0      254 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xtoolkit/__init__.py
+-rw-rw-rw-   0        0        0     3108 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xtoolkit/judgement.py
+-rw-rw-rw-   0        0        0      441 2022-07-06 07:25:01.000000 xToolkit-0.0.84/xToolkit/xtoolkit/xtoolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:42:36.702724 xToolkit-0.0.84/xToolkit.egg-info/
+-rw-rw-rw-   0        0        0    25597 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 07:42:36.000000 xToolkit-0.0.84/xToolkit.egg-info/top_level.txt
```

### Comparing `xToolkit-0.0.83/PKG-INFO` & `xToolkit-0.0.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xToolkit
-Version: 0.0.83
+Version: 0.0.84
 Summary: UNKNOWN
 Home-page: https://github.com/xionglihong/xToolkit
 Author: xionglihong
 Author-email: xionglihong@163.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -908,11 +908,15 @@
 
 - 正则校验模块改为match
 
 2022年08月24日 V0.0.83
 
 - 复合参数校验添加ip地址校验
 
+2022年05月17日 V0.0.84
+
+- 复合参数校验添加自定义正则表达式校验
+
 开发计划：
 
 - 无
```

### Comparing `xToolkit-0.0.83/README.md` & `xToolkit-0.0.84/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -897,10 +897,14 @@
 
 - 正则校验模块改为match
 
 2022年08月24日 V0.0.83
 
 - 复合参数校验添加ip地址校验
 
+2022年05月17日 V0.0.84
+
+- 复合参数校验添加自定义正则表达式校验
+
 开发计划：
 
 - 无
```

### Comparing `xToolkit-0.0.83/setup.py` & `xToolkit-0.0.84/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.83'
+VERSION = '0.0.84'
 
 # 导入信息说明文档
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name='xToolkit',
```

### Comparing `xToolkit-0.0.83/xToolkit/__init__.py` & `xToolkit-0.0.84/xToolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xdatetime/api.py` & `xToolkit-0.0.84/xToolkit/xdatetime/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xdatetime/xdatetime/xdatetime.py` & `xToolkit-0.0.84/xToolkit/xdatetime/xdatetime/xdatetime.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xfile/api.py` & `xToolkit-0.0.84/xToolkit/xfile/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xfile/dispose/dispose.py` & `xToolkit-0.0.84/xToolkit/xfile/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xhotchpotch/api.py` & `xToolkit-0.0.84/xToolkit/xhotchpotch/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xhotchpotch/dispose/dispose.py` & `xToolkit-0.0.84/xToolkit/xhotchpotch/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xlist/api.py` & `xToolkit-0.0.84/xToolkit/xlist/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xlist/dispose/dispose.py` & `xToolkit-0.0.84/xToolkit/xlist/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xstring/api.py` & `xToolkit-0.0.84/xToolkit/xstring/api.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xstring/check/check.py` & `xToolkit-0.0.84/xToolkit/xstring/check/check.py`

 * *Files 3% similar despite different names*

```diff
@@ -261,47 +261,58 @@
         # 任意
         elif rule == "casual":
             return True
         else:
             return False
 
     # 校验逻辑
-    def regular_logic(self, rule, choices):
+    def regular_logic(self, rule, **kwargs):
         """
         校验逻辑
         """
+        choices, regular = kwargs["choices"], kwargs["regular"]
+
         tem_list = ["is_json", "is_json_list", "is_casual_list"]
         tem_list += self.rule_list_list
-        if self.regular(rule, choices=choices) is not False:
-            if rule in tem_list:
-                return json.loads(self.parameter)
-            elif rule == "is_int":
-                return int(self.parameter)
-            else:
+
+        # 如果用户自定义正则表达式，就用用户自定义的正则表达式
+        if regular:
+            if re.match(regular, str(self.parameter)):
                 return self.parameter
+            else:
+                return False
         else:
-            return False
+            if self.regular(rule, choices=choices) is not False:
+                if rule in tem_list:
+                    return json.loads(self.parameter)
+                elif rule == "is_int":
+                    return int(self.parameter)
+                else:
+                    return self.parameter
+            else:
+                return False
 
     def introduction(self, **kwargs):
         """
         is_blank 如果为True代表如果用户传值，就进行校验，如果传空，值就为空
         """
         rule = kwargs["rule"] if kwargs.get("rule") else None
         is_blank = kwargs["is_blank"] if kwargs.get("is_blank") else False
         choices = kwargs["choices"] if kwargs.get("choices") else None
         max_length = kwargs["max_length"] if kwargs.get("max_length") else None  # 最大字符串长度
+        regular = kwargs["regular"] if kwargs.get("regular") else None  # 自定义正则表达式
 
         result = False
         # 如果长度超出最大长度
         if max_length:
             if len(self.parameter) > max_length:
                 return result
 
         if is_blank is True:
             if self.parameter:
-                result = self.regular_logic(rule, choices)
+                result = self.regular_logic(rule, choices=choices, regular=regular)
             else:
                 result = self.parameter
         else:
-            result = self.regular_logic(rule, choices)
+            result = self.regular_logic(rule, choices=choices, regular=regular)
 
         return result
```

### Comparing `xToolkit-0.0.83/xToolkit/xstring/dispose/dispose.py` & `xToolkit-0.0.84/xToolkit/xstring/dispose/dispose.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xstring/xstring.py` & `xToolkit-0.0.84/xToolkit/xstring/xstring.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xthreading/xthread.py` & `xToolkit-0.0.84/xToolkit/xthreading/xthread.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit/xtoolkit/judgement.py` & `xToolkit-0.0.84/xToolkit/xtoolkit/judgement.py`

 * *Files identical despite different names*

### Comparing `xToolkit-0.0.83/xToolkit.egg-info/PKG-INFO` & `xToolkit-0.0.84/xToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xToolkit
-Version: 0.0.83
+Version: 0.0.84
 Summary: UNKNOWN
 Home-page: https://github.com/xionglihong/xToolkit
 Author: xionglihong
 Author-email: xionglihong@163.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -908,11 +908,15 @@
 
 - 正则校验模块改为match
 
 2022年08月24日 V0.0.83
 
 - 复合参数校验添加ip地址校验
 
+2022年05月17日 V0.0.84
+
+- 复合参数校验添加自定义正则表达式校验
+
 开发计划：
 
 - 无
```

### Comparing `xToolkit-0.0.83/xToolkit.egg-info/SOURCES.txt` & `xToolkit-0.0.84/xToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

