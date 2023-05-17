# Comparing `tmp/XmindExcelTestcases-0.0.8.tar.gz` & `tmp/XmindExcelTestcases-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XmindExcelTestcases-0.0.8.tar", last modified: Mon Sep 27 10:57:36 2021, max compression
+gzip compressed data, was "XmindExcelTestcases-0.0.9.tar", last modified: Wed May 17 02:42:03 2023, max compression
```

## Comparing `XmindExcelTestcases-0.0.8.tar` & `XmindExcelTestcases-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xue        (501) staff       (20)        0 2021-09-27 10:57:36.087425 XmindExcelTestcases-0.0.8/
--rw-r--r--   0 xue        (501) staff       (20)        0 2021-05-21 08:37:16.000000 XmindExcelTestcases-0.0.8/LICENSE
--rw-r--r--   0 xue        (501) staff       (20)      604 2021-09-27 10:57:36.087205 XmindExcelTestcases-0.0.8/PKG-INFO
--rw-r--r--   0 xue        (501) staff       (20)      171 2021-05-21 08:37:16.000000 XmindExcelTestcases-0.0.8/README.md
-drwxr-xr-x   0 xue        (501) staff       (20)        0 2021-09-27 10:57:36.085666 XmindExcelTestcases-0.0.8/XmindExcelTestcases/
--rw-r--r--   0 xue        (501) staff       (20)       21 2021-09-26 12:12:41.000000 XmindExcelTestcases-0.0.8/XmindExcelTestcases/__init__.py
--rw-r--r--   0 xue        (501) staff       (20)      385 2021-09-27 04:36:33.000000 XmindExcelTestcases-0.0.8/XmindExcelTestcases/__main__.py
--rw-r--r--   0 xue        (501) staff       (20)    15068 2021-09-27 10:55:45.000000 XmindExcelTestcases-0.0.8/XmindExcelTestcases/convert_xmind_to_excel.py
-drwxr-xr-x   0 xue        (501) staff       (20)        0 2021-09-27 10:57:36.086896 XmindExcelTestcases-0.0.8/XmindExcelTestcases.egg-info/
--rw-r--r--   0 xue        (501) staff       (20)      604 2021-09-27 10:57:35.000000 XmindExcelTestcases-0.0.8/XmindExcelTestcases.egg-info/PKG-INFO
--rw-r--r--   0 xue        (501) staff       (20)      354 2021-09-27 10:57:35.000000 XmindExcelTestcases-0.0.8/XmindExcelTestcases.egg-info/SOURCES.txt
--rw-r--r--   0 xue        (501) staff       (20)        1 2021-09-27 10:57:35.000000 XmindExcelTestcases-0.0.8/XmindExcelTestcases.egg-info/dependency_links.txt
--rw-r--r--   0 xue        (501) staff       (20)       75 2021-09-27 10:57:35.000000 XmindExcelTestcases-0.0.8/XmindExcelTestcases.egg-info/entry_points.txt
--rw-r--r--   0 xue        (501) staff       (20)       20 2021-09-27 10:57:35.000000 XmindExcelTestcases-0.0.8/XmindExcelTestcases.egg-info/top_level.txt
--rw-r--r--   0 xue        (501) staff       (20)       38 2021-09-27 10:57:36.087500 XmindExcelTestcases-0.0.8/setup.cfg
--rw-r--r--   0 xue        (501) staff       (20)      949 2021-09-27 10:57:32.000000 XmindExcelTestcases-0.0.8/setup.py
+drwxr-xr-x   0 xue        (501) staff       (20)        0 2023-05-17 02:42:03.717731 XmindExcelTestcases-0.0.9/
+-rw-r--r--   0 xue        (501) staff       (20)        0 2021-05-21 08:37:16.000000 XmindExcelTestcases-0.0.9/LICENSE
+-rw-r--r--   0 xue        (501) staff       (20)      604 2023-05-17 02:42:03.717525 XmindExcelTestcases-0.0.9/PKG-INFO
+-rw-r--r--   0 xue        (501) staff       (20)      171 2021-05-21 08:37:16.000000 XmindExcelTestcases-0.0.9/README.md
+drwxr-xr-x   0 xue        (501) staff       (20)        0 2023-05-17 02:42:03.716022 XmindExcelTestcases-0.0.9/XmindExcelTestcases/
+-rw-r--r--   0 xue        (501) staff       (20)       21 2021-09-26 12:12:41.000000 XmindExcelTestcases-0.0.9/XmindExcelTestcases/__init__.py
+-rw-r--r--   0 xue        (501) staff       (20)      385 2021-09-27 04:36:33.000000 XmindExcelTestcases-0.0.9/XmindExcelTestcases/__main__.py
+-rw-r--r--   0 xue        (501) staff       (20)    15232 2023-05-17 02:07:14.000000 XmindExcelTestcases-0.0.9/XmindExcelTestcases/convert_xmind_to_excel.py
+drwxr-xr-x   0 xue        (501) staff       (20)        0 2023-05-17 02:42:03.717230 XmindExcelTestcases-0.0.9/XmindExcelTestcases.egg-info/
+-rw-r--r--   0 xue        (501) staff       (20)      604 2023-05-17 02:42:03.000000 XmindExcelTestcases-0.0.9/XmindExcelTestcases.egg-info/PKG-INFO
+-rw-r--r--   0 xue        (501) staff       (20)      354 2023-05-17 02:42:03.000000 XmindExcelTestcases-0.0.9/XmindExcelTestcases.egg-info/SOURCES.txt
+-rw-r--r--   0 xue        (501) staff       (20)        1 2023-05-17 02:42:03.000000 XmindExcelTestcases-0.0.9/XmindExcelTestcases.egg-info/dependency_links.txt
+-rw-r--r--   0 xue        (501) staff       (20)       75 2023-05-17 02:42:03.000000 XmindExcelTestcases-0.0.9/XmindExcelTestcases.egg-info/entry_points.txt
+-rw-r--r--   0 xue        (501) staff       (20)       20 2023-05-17 02:42:03.000000 XmindExcelTestcases-0.0.9/XmindExcelTestcases.egg-info/top_level.txt
+-rw-r--r--   0 xue        (501) staff       (20)       38 2023-05-17 02:42:03.717809 XmindExcelTestcases-0.0.9/setup.cfg
+-rw-r--r--   0 xue        (501) staff       (20)      949 2023-05-17 02:34:37.000000 XmindExcelTestcases-0.0.9/setup.py
```

### Comparing `XmindExcelTestcases-0.0.8/PKG-INFO` & `XmindExcelTestcases-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XmindExcelTestcases
-Version: 0.0.8
+Version: 0.0.9
 Summary: xmind脑图转换为Excel格式的测试用例
 Home-page: UNKNOWN
 Author: kaven.xue
 Author-email: 454086662@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `XmindExcelTestcases-0.0.8/XmindExcelTestcases/convert_xmind_to_excel.py` & `XmindExcelTestcases-0.0.9/XmindExcelTestcases/convert_xmind_to_excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,34 +16,34 @@
         self.case_pre_condition = '前置条件'
         self.case_steps = '用例步骤'
         self.result = '预期结果'
         self.case_type = '用例类型'
         self.case_state = '用例状态'
         self.case_level = '用例等级'
         self.case_founder = '创建人'
-        #self.case_isauto = '是否实现自动化'
-        #self.case_isput = '是否上架'
-        #self.autocase_type = '自动化测试类型'
-        #self.autocase_platform = '自动化测试平台'
+        # self.case_isauto = '是否实现自动化'
+        # self.case_isput = '是否上架'
+        # self.autocase_type = '自动化测试类型'
+        # self.autocase_platform = '自动化测试平台'
 
         self.markdown_dict[self.feature_layer] = []
         self.markdown_dict[self.case_feature_id] = []
         self.markdown_dict[self.case_title] = []
         self.markdown_dict[self.case_description] = []
         self.markdown_dict[self.case_pre_condition] = []
         self.markdown_dict[self.case_steps] = []
         self.markdown_dict[self.result] = []
         self.markdown_dict[self.case_type] = []
         self.markdown_dict[self.case_state] = []
         self.markdown_dict[self.case_level] = []
         self.markdown_dict[self.case_founder] = []
-        #self.markdown_dict[self.case_isauto] = []
-        #self.markdown_dict[self.case_isput] = []
-        #self.markdown_dict[self.autocase_type] = []
-        #self.markdown_dict[self.autocase_platform] = []
+        # self.markdown_dict[self.case_isauto] = []
+        # self.markdown_dict[self.case_isput] = []
+        # self.markdown_dict[self.autocase_type] = []
+        # self.markdown_dict[self.autocase_platform] = []
 
         self.index = 0
         self.ignore_layer_number = 1
 
     def convert(self, xmind_path, excel_path, ignore_layer_number='1'):
         if os.path.isfile(xmind_path):
             # 如果传递单个xmind文件，则直接转换
@@ -86,18 +86,20 @@
             worksheet.set_column('A:Z', None, fmt)
             worksheet.set_row(0, None, fmt)
             for col_num, value in enumerate(df.columns.values):
                 worksheet.write(0, col_num, value, fmt)
 
             for idx, col in enumerate(df):
                 series = df[col]
-                max_len = max(series.astype(str).map(len).max(),len(str(series.name)))+4
-                worksheet.set_column(idx,idx ,max_len)
-
-            writer.save()
+                max_len = max(series.astype(str).map(len).max(), len(str(series.name))) + 4
+                worksheet.set_column(idx, idx, max_len)
+            try:
+                writer.save()
+            except:
+                writer.close()
 
     # 将单个xmind转换为单个excel文件
     def convert_single_file(self, xmind_path, excel_path, ignore_layer_number):
         try:
             self.ignore_layer_number = int(ignore_layer_number)
             self.parseXmindToDict(xmind_path)
             df = pd.DataFrame(self.markdown_dict)
@@ -110,56 +112,58 @@
             worksheet.set_column('A:Z', None, fmt)
             worksheet.set_row(0, None, fmt)
             for col_num, value in enumerate(df.columns.values):
                 worksheet.write(0, col_num, value, fmt)
 
             for idx, col in enumerate(df):
                 series = df[col]
-                max_len = max(series.astype(str).map(len).max(),len(str(series.name)))+4
+                max_len = max(series.astype(str).map(len).max(), len(str(series.name))) + 4
                 worksheet.set_column(idx, idx, max_len)
 
-            writer.save()
+            try:
+                writer.save()
+            except:
+                writer.close()
 
         finally:
             self.markdown_dict = dict()
             self.feature_layer = '用例目录'
             self.case_feature_id = '需求ID'
             self.case_title = '用例名称'
             self.case_description = '用例描述'
             self.case_pre_condition = '前置条件'
             self.case_steps = '用例步骤'
             self.result = '预期结果'
             self.case_type = '用例类型'
             self.case_state = '用例状态'
             self.case_level = '用例等级'
             self.case_founder = '创建人'
-            #self.case_isauto = '是否实现自动化'
-            #self.case_isput = '是否上架'
-            #self.autocase_type = '自动化测试类型'
-            #self.autocase_platform = '自动化测试平台'
+            # self.case_isauto = '是否实现自动化'
+            # self.case_isput = '是否上架'
+            # self.autocase_type = '自动化测试类型'
+            # self.autocase_platform = '自动化测试平台'
 
             self.markdown_dict[self.feature_layer] = []
             self.markdown_dict[self.case_feature_id] = []
             self.markdown_dict[self.case_title] = []
             self.markdown_dict[self.case_description] = []
             self.markdown_dict[self.case_pre_condition] = []
             self.markdown_dict[self.case_steps] = []
             self.markdown_dict[self.result] = []
             self.markdown_dict[self.case_type] = []
             self.markdown_dict[self.case_state] = []
             self.markdown_dict[self.case_level] = []
             self.markdown_dict[self.case_founder] = []
-            #self.markdown_dict[self.case_isauto] = []
-            #self.markdown_dict[self.case_isput] = []
-            #self.markdown_dict[self.autocase_type] = []
-            #self.markdown_dict[self.autocase_platform] = []
+            # self.markdown_dict[self.case_isauto] = []
+            # self.markdown_dict[self.case_isput] = []
+            # self.markdown_dict[self.autocase_type] = []
+            # self.markdown_dict[self.autocase_platform] = []
             self.index = 0
             self.ignore_layer_number = 0
 
-
     def parseXmindToDict(self, xmind_file_path):
         content_dict = xmind_to_dict(xmind_file_path)
         object = content_dict[0]['topic']
         content_array = []
         for i in range(100):
             content_array.append(i)
         self.analyze(content_array, object)
@@ -175,15 +179,15 @@
         self.index = self.index - 1
 
     def generate(self, content_array):
         title = ''
 
         flag_dict = {self.feature_layer: False, self.case_feature_id: False, self.case_description: False,
                      self.case_pre_condition: False, self.case_steps: False, self.result: False,
-                     self.case_level: False, self.case_founder: False }
+                     self.case_level: False, self.case_founder: False}
 
         for i in range(self.index + 1):
             content = content_array[i]
             content = content.replace('\b', '')
             if self.check_in_column(content):
                 # 如果content以 "列名："的样式开开头，则进入对应的列名解析
                 column_name, column_value = self.analyse_column(content)
```

### Comparing `XmindExcelTestcases-0.0.8/XmindExcelTestcases.egg-info/PKG-INFO` & `XmindExcelTestcases-0.0.9/XmindExcelTestcases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XmindExcelTestcases
-Version: 0.0.8
+Version: 0.0.9
 Summary: xmind脑图转换为Excel格式的测试用例
 Home-page: UNKNOWN
 Author: kaven.xue
 Author-email: 454086662@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `XmindExcelTestcases-0.0.8/setup.py` & `XmindExcelTestcases-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # 读取项目的readme介绍
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="XmindExcelTestcases",# 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.8",
+    version="0.0.9",
     author="kaven.xue", # 项目作者
     author_email="454086662@qq.com",
     description="xmind脑图转换为Excel格式的测试用例", # 项目的一句话描述
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",# 项目地址
     packages=setuptools.find_packages(),
```

