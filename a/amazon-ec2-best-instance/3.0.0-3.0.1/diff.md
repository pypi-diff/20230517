# Comparing `tmp/amazon-ec2-best-instance-3.0.0.tar.gz` & `tmp/amazon-ec2-best-instance-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/alexey/PycharmProjects/kankou-aliaksei/amazon-ec2-best-instance/dist/.tmp-9cuibstj/amazon-ec2-best-instance-3.0.0.tar", last modified: Wed May 17 10:57:13 2023, max compression
+gzip compressed data, was "/Users/alexey/PycharmProjects/kankou-aliaksei/amazon-ec2-best-instance/dist/.tmp-jnvwgw7_/amazon-ec2-best-instance-3.0.1.tar", last modified: Wed May 17 11:43:02 2023, max compression
```

## Comparing `amazon-ec2-best-instance-3.0.0.tar` & `amazon-ec2-best-instance-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/
--rw-r--r--   0 alexey     (501) staff       (20)     7355 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)     6791 2023-05-17 10:53:19.000000 amazon-ec2-best-instance-3.0.0/README.md
--rw-r--r--   0 alexey     (501) staff       (20)        0 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/pyproject.toml
--rw-r--r--   0 alexey     (501) staff       (20)      812 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)      214 2023-05-13 18:54:46.000000 amazon-ec2-best-instance-3.0.0/setup.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/
--rw-r--r--   0 alexey     (501) staff       (20)     1677 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/SpotUtils.py
--rw-r--r--   0 alexey     (501) staff       (20)       67 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/__init__.py
--rw-r--r--   0 alexey     (501) staff       (20)    22676 2023-05-17 08:51:37.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     7355 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      809 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)       58 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       25 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/top_level.txt
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 10:57:13.000000 amazon-ec2-best-instance-3.0.0/test/
--rw-r--r--   0 alexey     (501) staff       (20)      914 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test.py
--rw-r--r--   0 alexey     (501) staff       (20)     1822 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test1.py
--rw-r--r--   0 alexey     (501) staff       (20)      870 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test10.py
--rw-r--r--   0 alexey     (501) staff       (20)     1008 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test11.py
--rw-r--r--   0 alexey     (501) staff       (20)     1250 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test2.py
--rw-r--r--   0 alexey     (501) staff       (20)      242 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test3.py
--rw-r--r--   0 alexey     (501) staff       (20)     1257 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test4.py
--rw-r--r--   0 alexey     (501) staff       (20)     1397 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test5.py
--rw-r--r--   0 alexey     (501) staff       (20)      804 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test6.py
--rw-r--r--   0 alexey     (501) staff       (20)     1720 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test7.py
--rw-r--r--   0 alexey     (501) staff       (20)     1154 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test8.py
--rw-r--r--   0 alexey     (501) staff       (20)      517 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test9.py
--rw-r--r--   0 alexey     (501) staff       (20)     1086 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test_azs.py
--rw-r--r--   0 alexey     (501) staff       (20)     1996 2023-05-13 17:39:20.000000 amazon-ec2-best-instance-3.0.0/test/test_cache.py
--rw-r--r--   0 alexey     (501) staff       (20)     1869 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_2.py
--rw-r--r--   0 alexey     (501) staff       (20)      938 2023-05-13 17:42:39.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_3.py
--rw-r--r--   0 alexey     (501) staff       (20)     1040 2023-05-13 17:54:23.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_4.py
--rw-r--r--   0 alexey     (501) staff       (20)     1028 2023-05-13 17:55:02.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_5.py
--rw-r--r--   0 alexey     (501) staff       (20)      638 2023-05-13 18:06:28.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_6.py
--rw-r--r--   0 alexey     (501) staff       (20)      599 2023-05-13 18:07:20.000000 amazon-ec2-best-instance-3.0.0/test/test_cache_7.py
--rw-r--r--   0 alexey     (501) staff       (20)     2138 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.0/test/test_clients.py
--rw-r--r--   0 alexey     (501) staff       (20)     2145 2023-05-14 14:57:55.000000 amazon-ec2-best-instance-3.0.0/test/test_fast.py
--rw-r--r--   0 alexey     (501) staff       (20)     2191 2023-05-17 08:52:19.000000 amazon-ec2-best-instance-3.0.0/test/test_gpu.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/
+-rw-r--r--   0 alexey     (501) staff       (20)     7355 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)     6791 2023-05-17 10:53:19.000000 amazon-ec2-best-instance-3.0.1/README.md
+-rw-r--r--   0 alexey     (501) staff       (20)        0 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/pyproject.toml
+-rw-r--r--   0 alexey     (501) staff       (20)      812 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)      214 2023-05-13 18:54:46.000000 amazon-ec2-best-instance-3.0.1/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/
+-rw-r--r--   0 alexey     (501) staff       (20)     1677 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/SpotUtils.py
+-rw-r--r--   0 alexey     (501) staff       (20)       67 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/__init__.py
+-rw-r--r--   0 alexey     (501) staff       (20)    22672 2023-05-17 11:42:14.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     7355 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      809 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       58 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       25 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/top_level.txt
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-17 11:43:02.000000 amazon-ec2-best-instance-3.0.1/test/
+-rw-r--r--   0 alexey     (501) staff       (20)      914 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1822 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test1.py
+-rw-r--r--   0 alexey     (501) staff       (20)      870 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test10.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1008 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test11.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1250 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test2.py
+-rw-r--r--   0 alexey     (501) staff       (20)      242 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test3.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1257 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test4.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1397 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test5.py
+-rw-r--r--   0 alexey     (501) staff       (20)      804 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test6.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1720 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test7.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1154 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test8.py
+-rw-r--r--   0 alexey     (501) staff       (20)      517 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test9.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1086 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test_azs.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1996 2023-05-13 17:39:20.000000 amazon-ec2-best-instance-3.0.1/test/test_cache.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1869 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_2.py
+-rw-r--r--   0 alexey     (501) staff       (20)      938 2023-05-13 17:42:39.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_3.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1040 2023-05-13 17:54:23.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_4.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1028 2023-05-13 17:55:02.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_5.py
+-rw-r--r--   0 alexey     (501) staff       (20)      638 2023-05-13 18:06:28.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_6.py
+-rw-r--r--   0 alexey     (501) staff       (20)      599 2023-05-13 18:07:20.000000 amazon-ec2-best-instance-3.0.1/test/test_cache_7.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2138 2023-05-13 17:32:45.000000 amazon-ec2-best-instance-3.0.1/test/test_clients.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2145 2023-05-14 14:57:55.000000 amazon-ec2-best-instance-3.0.1/test/test_fast.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2186 2023-05-17 11:36:07.000000 amazon-ec2-best-instance-3.0.1/test/test_gpu.py
```

### Comparing `amazon-ec2-best-instance-3.0.0/PKG-INFO` & `amazon-ec2-best-instance-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-ec2-best-instance
-Version: 3.0.0
+Version: 3.0.1
 Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
 Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `amazon-ec2-best-instance-3.0.0/README.md` & `amazon-ec2-best-instance-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/setup.cfg` & `amazon-ec2-best-instance-3.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amazon-ec2-best-instance
-version = 3.0.0
+version = 3.0.1
 author = Aliaksei Kankou
 author_email = aliaksei.kankou@gmail.com
 description = Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 project_urls =
```

### Comparing `amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/SpotUtils.py` & `amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/SpotUtils.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance/main.py` & `amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,17 +503,17 @@
         list_set = set(list1)
         unique_list = (list(list_set))
         return unique_list
 
     @staticmethod
     def __get_pool() -> Any:
         if os.environ.get('AWS_LAMBDA_FUNCTION_NAME') is None:
-            return ThreadPool()
+            return ThreadPool
         else:
-            return LambdaThreadPool()
+            return LambdaThreadPool
 
     @staticmethod
     def __get_client(options: Dict[str, Any], service: str, region: str) -> Any:
         if options.get('clients') is not None and options['clients'].get(service) is not None:
             return options['clients'][service]
         else:
             return boto3.session.Session().client(service, region_name=region)
```

### Comparing `amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/PKG-INFO` & `amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-ec2-best-instance
-Version: 3.0.0
+Version: 3.0.1
 Summary: Amazon EC2 Best Instance (amazon-ec2-best-instance) allows you to choose the most optimal and cheap EC2 instance type for on-demand and spot and with a less reclaimed rate for a spot instance.
 Home-page: https://github.com/kankou-aliaksei/amazon-ec2-best-instance
 Author: Aliaksei Kankou
 Author-email: aliaksei.kankou@gmail.com
 Project-URL: Bug Tracker, https://github.com/kankou-aliaksei/amazon-ec2-best-instance/issues
 Requires-Python: >3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `amazon-ec2-best-instance-3.0.0/src/amazon_ec2_best_instance.egg-info/SOURCES.txt` & `amazon-ec2-best-instance-3.0.1/src/amazon_ec2_best_instance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test.py` & `amazon-ec2-best-instance-3.0.1/test/test.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test1.py` & `amazon-ec2-best-instance-3.0.1/test/test1.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test10.py` & `amazon-ec2-best-instance-3.0.1/test/test10.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test11.py` & `amazon-ec2-best-instance-3.0.1/test/test11.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test2.py` & `amazon-ec2-best-instance-3.0.1/test/test2.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test4.py` & `amazon-ec2-best-instance-3.0.1/test/test4.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test5.py` & `amazon-ec2-best-instance-3.0.1/test/test5.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test6.py` & `amazon-ec2-best-instance-3.0.1/test/test6.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test7.py` & `amazon-ec2-best-instance-3.0.1/test/test7.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test8.py` & `amazon-ec2-best-instance-3.0.1/test/test8.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test9.py` & `amazon-ec2-best-instance-3.0.1/test/test9.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_azs.py` & `amazon-ec2-best-instance-3.0.1/test/test_azs.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_cache.py` & `amazon-ec2-best-instance-3.0.1/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_cache_2.py` & `amazon-ec2-best-instance-3.0.1/test/test_cache_2.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_cache_3.py` & `amazon-ec2-best-instance-3.0.1/test/test_cache_3.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_cache_4.py` & `amazon-ec2-best-instance-3.0.1/test/test_cache_4.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_cache_5.py` & `amazon-ec2-best-instance-3.0.1/test/test_cache_5.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_cache_6.py` & `amazon-ec2-best-instance-3.0.1/test/test_cache_6.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_cache_7.py` & `amazon-ec2-best-instance-3.0.1/test/test_cache_7.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_clients.py` & `amazon-ec2-best-instance-3.0.1/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_fast.py` & `amazon-ec2-best-instance-3.0.1/test/test_fast.py`

 * *Files identical despite different names*

### Comparing `amazon-ec2-best-instance-3.0.0/test/test_gpu.py` & `amazon-ec2-best-instance-3.0.1/test/test_gpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 response = ec2_best_instance.get_best_instance_types({
     # Required.
     'vcpu': 1,
     # Required.
     'memory_gb': 2,
     # Optional. Default: 'on-demand'. Values: 'spot'|'on-demand'
-    'usage_class': 'on-demand',
+    'usage_class': 'spot',
     # Optional.
     #'burstable': False,
     # Optional. Default: 'x86_64'. Values: 'i386'|'x86_64'|'arm64'|'x86_64_mac'
     #'architecture': 'x86_64_mac',
     # Optional. Default: ['Linux/UNIX'].
     # Values: Linux/UNIX | Red Hat Enterprise Linux | SUSE Linux | Windows | Linux/UNIX (Amazon VPC) | 
         # Red Hat Enterprise Linux (Amazon VPC) | SUSE Linux (Amazon VPC) | Windows (Amazon VPC)
```

