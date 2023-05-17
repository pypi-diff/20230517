# Comparing `tmp/deep_copilot-0.0.4.tar.gz` & `tmp/deep_copilot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_copilot-0.0.4.tar", last modified: Wed May 17 08:17:42 2023, max compression
+gzip compressed data, was "deep_copilot-0.0.5.tar", last modified: Wed May 17 11:03:39 2023, max compression
```

## Comparing `deep_copilot-0.0.4.tar` & `deep_copilot-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:17:42.836412 deep_copilot-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-17 07:38:12.000000 deep_copilot-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11558 2023-05-17 07:38:12.000000 deep_copilot-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      116 2023-05-17 07:38:12.000000 deep_copilot-0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1909 2023-05-17 08:17:42.836412 deep_copilot-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-17 07:38:12.000000 deep_copilot-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:17:42.834412 deep_copilot-0.0.4/deep_copilot/
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 07:53:29.000000 deep_copilot-0.0.4/deep_copilot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:17:42.835412 deep_copilot-0.0.4/deep_copilot/mysql_tools/
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 08:03:31.000000 deep_copilot-0.0.4/deep_copilot/mysql_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12399 2023-05-17 08:10:27.000000 deep_copilot-0.0.4/deep_copilot/mysql_tools/mysql_copilot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 08:17:42.835412 deep_copilot-0.0.4/deep_copilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1909 2023-05-17 08:17:42.000000 deep_copilot-0.0.4/deep_copilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-17 08:17:42.000000 deep_copilot-0.0.4/deep_copilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 08:17:42.000000 deep_copilot-0.0.4/deep_copilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:55:17.000000 deep_copilot-0.0.4/deep_copilot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-17 08:17:42.000000 deep_copilot-0.0.4/deep_copilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 08:17:42.000000 deep_copilot-0.0.4/deep_copilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-17 08:17:37.000000 deep_copilot-0.0.4/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 08:17:42.836412 deep_copilot-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1972 2023-05-17 08:11:27.000000 deep_copilot-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.926931 deep_copilot-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-17 07:38:12.000000 deep_copilot-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-05-17 07:38:12.000000 deep_copilot-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      116 2023-05-17 07:38:12.000000 deep_copilot-0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-17 11:03:39.925931 deep_copilot-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-17 07:38:12.000000 deep_copilot-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.915931 deep_copilot-0.0.5/deep_copilot/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 07:53:29.000000 deep_copilot-0.0.5/deep_copilot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.917931 deep_copilot-0.0.5/deep_copilot/audio_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-10-11 01:39:00.000000 deep_copilot-0.0.5/deep_copilot/audio_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-05-17 09:05:05.000000 deep_copilot-0.0.5/deep_copilot/audio_tools/base_audio_tools.py
+-rw-r--r--   0 root         (0) root         (0)     8546 2022-10-11 06:47:07.000000 deep_copilot-0.0.5/deep_copilot/audio_tools/vad_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.918931 deep_copilot-0.0.5/deep_copilot/command_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-09-23 08:46:31.000000 deep_copilot-0.0.5/deep_copilot/command_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      303 2022-09-23 03:56:36.000000 deep_copilot-0.0.5/deep_copilot/command_tools/compat.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-05-17 09:18:16.000000 deep_copilot-0.0.5/deep_copilot/command_tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.918931 deep_copilot-0.0.5/deep_copilot/date_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-10-10 08:58:10.000000 deep_copilot-0.0.5/deep_copilot/date_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-05-17 09:05:05.000000 deep_copilot-0.0.5/deep_copilot/date_tools/datetimeutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.918931 deep_copilot-0.0.5/deep_copilot/excel_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-09-16 08:29:18.000000 deep_copilot-0.0.5/deep_copilot/excel_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2022-09-27 07:15:50.000000 deep_copilot-0.0.5/deep_copilot/excel_tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.919931 deep_copilot-0.0.5/deep_copilot/faiss_tools/
+-rw-r--r--   0 root         (0) root         (0)      136 2023-03-30 06:39:27.000000 deep_copilot-0.0.5/deep_copilot/faiss_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-01-03 13:34:50.000000 deep_copilot-0.0.5/deep_copilot/faiss_tools/faiss_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.919931 deep_copilot-0.0.5/deep_copilot/hanlp_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-11-03 11:34:56.000000 deep_copilot-0.0.5/deep_copilot/hanlp_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-05-17 08:59:59.000000 deep_copilot-0.0.5/deep_copilot/hanlp_tools/hanlp_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.920931 deep_copilot-0.0.5/deep_copilot/log_tools/
+-rw-r--r--   0 root         (0) root         (0)      128 2022-09-06 09:29:11.000000 deep_copilot-0.0.5/deep_copilot/log_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/log_tools/log_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.920931 deep_copilot-0.0.5/deep_copilot/misc_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-11-02 07:19:29.000000 deep_copilot-0.0.5/deep_copilot/misc_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5169 2023-02-13 06:44:39.000000 deep_copilot-0.0.5/deep_copilot/misc_tools/es_tools.py
+-rw-r--r--   0 root         (0) root         (0)     6659 2023-05-17 08:59:59.000000 deep_copilot-0.0.5/deep_copilot/misc_tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.921931 deep_copilot-0.0.5/deep_copilot/mysql_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-17 08:03:31.000000 deep_copilot-0.0.5/deep_copilot/mysql_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12529 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/mysql_tools/mysql_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.921931 deep_copilot-0.0.5/deep_copilot/path_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-11-18 08:11:56.000000 deep_copilot-0.0.5/deep_copilot/path_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3406 2022-11-18 08:17:40.000000 deep_copilot-0.0.5/deep_copilot/path_tools/path_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.922931 deep_copilot-0.0.5/deep_copilot/seed_tools/
+-rw-r--r--   0 root         (0) root         (0)      129 2022-09-07 03:30:37.000000 deep_copilot-0.0.5/deep_copilot/seed_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-05-17 08:59:59.000000 deep_copilot-0.0.5/deep_copilot/seed_tools/seed_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.922931 deep_copilot-0.0.5/deep_copilot/string_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-10-12 06:01:05.000000 deep_copilot-0.0.5/deep_copilot/string_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3530 2023-03-07 08:42:48.000000 deep_copilot-0.0.5/deep_copilot/string_tools/string_copilot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.924931 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-09-23 03:49:41.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/base_image_tools.py
+-rw-r--r--   0 root         (0) root         (0)     7517 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/base_video_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/ffmpeg_tools.py
+-rw-r--r--   0 root         (0) root         (0)     8461 2022-05-18 08:51:21.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/ffmpyutil.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/key_frame_extraction_tools.py
+-rw-r--r--   0 root         (0) root         (0)      690 2022-09-23 05:56:01.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/moviepy_tools.py
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-05-17 08:51:50.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/opencv_tools.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2022-05-26 07:58:31.000000 deep_copilot-0.0.5/deep_copilot/video_and_image_tools/sceneutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.925931 deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/
+-rw-r--r--   0 root         (0) root         (0)      134 2023-03-30 06:39:27.000000 deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-05-17 09:28:11.000000 deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/chatgpt_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-05-17 08:59:59.000000 deep_copilot-0.0.5/deep_copilot/zero_short_model_tools/t5_model_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 11:03:39.916931 deep_copilot-0.0.5/deep_copilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 07:55:17.000000 deep_copilot-0.0.5/deep_copilot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      289 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 11:03:39.000000 deep_copilot-0.0.5/deep_copilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-05-17 08:17:49.000000 deep_copilot-0.0.5/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 11:03:39.926931 deep_copilot-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-17 09:16:07.000000 deep_copilot-0.0.5/setup.py
```

### Comparing `deep_copilot-0.0.4/CONTRIBUTING.md` & `deep_copilot-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.4/LICENSE` & `deep_copilot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.4/PKG-INFO` & `deep_copilot-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_copilot
-Version: 0.0.4
+Version: 0.0.5
 Summary: gyw toolkits
 Home-page: https://github.com/612twilight/deep_copilot/tree/master/
 Author: gyw
 Author-email: 240590367@qqq.com
 License: Apache Software License 2.0
 Keywords: anything not for deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `deep_copilot-0.0.4/README.md` & `deep_copilot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deep_copilot-0.0.4/deep_copilot/mysql_tools/mysql_copilot.py` & `deep_copilot-0.0.5/deep_copilot/mysql_tools/mysql_copilot.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # @ description:
 
 import logging
 import re
 import pymysql
 import time
 from tqdm import tqdm
+from deep_copilot.log_tools.log_tool import logger
 
 try:
     from pymysql import escape_string
 except:
     from pymysql.converters import escape_string
 
 
@@ -49,15 +50,15 @@
                                        password=self.password, charset=self.charset,
                                        cursorclass=pymysql.cursors.DictCursor)
             self.con.autocommit(1)
             # 所有的查询，都在连接 con 的一个模块 cursor 上面运行的
             self.cur = self.con.cursor()
         except:
             logging.exception("")
-            print("DataBase connect error,please check the db config.")
+            logger.info("DataBase connect error,please check the db config.")
 
     def __del__(self):
         if self.con:
             self.con.close()
 
     def _conn(self):
         try:
@@ -86,23 +87,23 @@
                 time.sleep(stime)  # 连接不成功,休眠3秒钟,继续循环，知道成功或重试次数结束
 
     # 关闭数据库连接
     def close(self):
         if self.con:
             self.con.close()
         else:
-            print("DataBase doesn't connect,close connecting error;please check the db config.")
+            logger.info("DataBase doesn't connect,close connecting error;please check the db config.")
 
     # 创建数据库
     def createDataBase(self, DB_NAME):
         # 创建数据库
         self.cur.execute(
             'CREATE DATABASE IF NOT EXISTS %s DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci' % DB_NAME)
         self.con.select_db(DB_NAME)
-        print('creatDatabase:' + DB_NAME)
+        logger.info('creatDatabase:' + DB_NAME)
 
     # 选择数据库
     def selectDataBase(self, DB_NAME):
         self.con.select_db(DB_NAME)
 
     # 获取数据库版本号
     def get_version(self):
@@ -121,40 +122,40 @@
             args：
                 tablename  ：表名字
                 attrdict   ：属性键值对,{'book_name':'varchar(200) NOT NULL'...}
                 constraint ：主外键约束,PRIMARY KEY(`id`)
         """
         # 　判断表是否存在
         if self.isExistTable(tablename):
-            print("%s is exit" % tablename)
+            logger.info("%s is exit" % tablename)
             return
         sql = ''
         sql_mid = '`id` bigint(11) NOT NULL AUTO_INCREMENT,'
         for attr, value in attrdict.items():
             sql_mid = sql_mid + '`' + attr + '`' + ' ' + value + ','
         sql = sql + 'CREATE TABLE IF NOT EXISTS %s (' % tablename
         sql = sql + sql_mid
         sql = sql + constraint
         sql = sql + ') ENGINE=InnoDB DEFAULT CHARSET=utf8'
-        print('creatTable:' + sql)
+        logger.info('creatTable:' + sql)
         self.execute_commit(sql)
 
     def execute(self, sql=''):
         """执行sql语句，针对读操作返回结果集
             args：
                 sql  ：sql语句
         """
         try:
             self._re_conn()
             self.cur.execute(sql)
             records = self.cur.fetchall()
             return records
         except pymysql.Error as e:
             error = 'MySQL execute failed! ERROR (%s): %s' % (e.args[0], e.args[1])
-            print(error)
+            logger.info(error)
             raise e
 
     def execute_commit(self, sql=''):
         """
         执行数据库sql语句，针对更新,删除,事务等操作失败时回滚
         """
         try:
@@ -165,15 +166,15 @@
             # 最新插入行的主键id
             self.con.insert_id()
             self.con.commit()
             return row_id
         except pymysql.Error as e:
             self.con.rollback()
             error = 'MySQL execute failed! ERROR (%s): %s' % (e.args[0], e.args[1])
-            print("error:", error)
+            logger.info("error:", error)
             raise e
 
     def insert(self, tablename, params):
         """创建数据库表
             args：
                 tablename  ：表名字
                 key        ：属性键
@@ -217,17 +218,17 @@
         if fields == "*":
             sql = 'select * from %s where ' % tablename
         else:
             if isinstance(fields, list):
                 fields = ",".join(fields)
                 sql = 'select %s from %s where ' % (fields, tablename)
             else:
-                print("fields input error, please input list fields.")
+                logger.info("fields input error, please input list fields.")
         sql = sql + consql + order
-        print('select:' + sql)
+        logger.info('select:' + sql)
         return self.execute(sql)
 
     def batch_insert(self, table, attrs, values):
         """插入多条数据
             args：
                 tablename  ：表名字
                 attrs        ：属性键
@@ -239,24 +240,24 @@
                 mydb.insertMany(table, key, value)
         """
         values_sql = ['%s' for v in attrs]
         attrs_sql = '(' + ','.join(attrs) + ')'
         values_sql = ' values(' + ','.join(values_sql) + ')'
         sql = 'insert ignore into %s' % table
         sql = sql + attrs_sql + values_sql
-        print('insertMany:' + sql)
+        logger.info('insertMany:' + sql)
         self._re_conn()
         try:
             for i in tqdm(range(0, len(values), 20000)):
                 self.cur.executemany(sql, values[i:i + 20000])
                 self.con.commit()
         except pymysql.Error as e:
             self.con.rollback()
             error = 'insertMany executemany failed! ERROR (%s): %s' % (e.args[0], e.args[1])
-            print(error)
+            logger.info(error)
 
     def delete(self, tablename, cond_dict):
         """删除数据
             args：
                 tablename  ：表名字
                 cond_dict  ：删除条件字典
             example：
@@ -267,15 +268,15 @@
         if cond_dict != '':
             for k, v in cond_dict.items():
                 if isinstance(v, str):
                     v = "\'" + v + "\'"
                 consql = consql + tablename + "." + k + '=' + v + ' and '
         consql = consql + ' 1=1 '
         sql = "DELETE FROM %s where %s" % (tablename, consql)
-        print(sql)
+        logger.info(sql)
         return self.execute_commit(sql)
 
     def update(self, tablename, attrs_dict, cond_dict):
         """更新数据
             args：
                 tablename  ：表名字
                 attrs_dict  ：更新属性键值对字典
@@ -318,15 +319,15 @@
 
     def deleteTable(self, tablename):
         """清空数据库表
             args：
                 tablename  ：表名字
         """
         sql = "DELETE FROM %s" % tablename
-        print("sql=", sql)
+        logger.info("sql=", sql)
         self.execute_commit(sql)
 
     def isExistTable(self, tablename):
         """判断数据表是否存在
             args：
                 tablename  ：表名字
             Return:
```

### Comparing `deep_copilot-0.0.4/deep_copilot.egg-info/PKG-INFO` & `deep_copilot-0.0.5/deep_copilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-copilot
-Version: 0.0.4
+Version: 0.0.5
 Summary: gyw toolkits
 Home-page: https://github.com/612twilight/deep_copilot/tree/master/
 Author: gyw
 Author-email: 240590367@qqq.com
 License: Apache Software License 2.0
 Keywords: anything not for deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `deep_copilot-0.0.4/setup.py` & `deep_copilot-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
 import setuptools
-assert parse_version(setuptools.__version__)>=parse_version('36.2')
+
+assert parse_version(setuptools.__version__) >= parse_version('36.2')
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
 config.read('settings.ini')
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
 expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
 for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
-setup_cfg = {o:cfg[o] for o in cfg_keys}
+setup_cfg = {o: cfg[o] for o in cfg_keys}
 
 licenses = {
-    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'apache2': ('Apache Software License 2.0', 'OSI Approved :: Apache Software License'),
 }
-statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
-    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
+statuses = ['1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
+            '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive']
 py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8 3.9'.split()
 
-requirements = cfg.get('requirements','').split()
+requirements = []
+with open("requirements.txt", "r", encoding="utf8") as reader:
+    for line in reader:
+        requirements.append(line.strip())
 lic = licenses[cfg['license']]
 min_python = cfg['min_python']
 
 setuptools.setup(
-    name = cfg['lib_name'],
-    license = lic[0],
-    classifiers = [
-        'Development Status :: ' + statuses[int(cfg['status'])],
-        'Intended Audience :: ' + cfg['audience'].title(),
-        'License :: ' + lic[1],
-        'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]],
-    url = cfg['git_url'],
-    packages = setuptools.find_packages(),
-    include_package_data = True,
-    install_requires = requirements,
-    dependency_links = cfg.get('dep_links','').split(),
-    python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
-    long_description_content_type = 'text/markdown',
-    zip_safe = False,
-    entry_points = { 'console_scripts': cfg.get('console_scripts','').split() },
+    name=cfg['lib_name'],
+    license=lic[0],
+    classifiers=[
+                    'Development Status :: ' + statuses[int(cfg['status'])],
+                    'Intended Audience :: ' + cfg['audience'].title(),
+                    'License :: ' + lic[1],
+                    'Natural Language :: ' + cfg['language'].title(),
+                ] + ['Programming Language :: Python :: ' + o for o in py_versions[py_versions.index(min_python):]],
+    url=cfg['git_url'],
+    packages=setuptools.find_packages(),
+    include_package_data=True,
+    install_requires=requirements,
+    dependency_links=cfg.get('dep_links', '').split(),
+    python_requires='>=' + cfg['min_python'],
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    zip_safe=False,
+    entry_points={'console_scripts': cfg.get('console_scripts', '').split()},
     **setup_cfg)
-
```

