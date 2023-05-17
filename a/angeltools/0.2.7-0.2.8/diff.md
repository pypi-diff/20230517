# Comparing `tmp/angeltools-0.2.7.tar.gz` & `tmp/angeltools-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angeltools-0.2.7.tar", last modified: Mon May 15 09:06:42 2023, max compression
+gzip compressed data, was "angeltools-0.2.8.tar", last modified: Wed May 17 08:38:33 2023, max compression
```

## Comparing `angeltools-0.2.7.tar` & `angeltools-0.2.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.2.7/LICENSE
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-15 09:06:42.418693 angeltools-0.2.7/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.2.7/README.md
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools/
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools/Db/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.2.7/angeltools/Db/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3289 2022-04-21 02:57:31.000000 angeltools-0.2.7/angeltools/Db/redis_connector.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.2.7/angeltools/ImageTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.2.7/angeltools/MathTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.2.7/angeltools/Slavers.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    14085 2023-05-15 08:54:56.000000 angeltools-0.2.7/angeltools/StrTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.2.7/angeltools/TimeTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.2.7/angeltools/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.2.7/angeltools/commands.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools/fdfs/
--rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.2.7/angeltools/fdfs/__init__.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools/fdfs/fdfs_client/
--rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/connection.py
--rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/exceptions.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/fdfs_protol.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/fdfs_test.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/storage_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/tracker_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_client/utils.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.2.7/angeltools/fdfs/fdfs_operator.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-15 09:06:42.418693 angeltools-0.2.7/angeltools.egg-info/
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/SOURCES.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/dependency_links.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/entry_points.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.2.7/angeltools.egg-info/not-zip-safe
--rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/requires.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-05-15 09:06:42.000000 angeltools-0.2.7/angeltools.egg-info/top_level.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-05-15 09:06:42.418693 angeltools-0.2.7/setup.cfg
--rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-05-15 09:06:08.000000 angeltools-0.2.7/setup.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.271493 angeltools-0.2.8/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.2.8/LICENSE
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-17 08:38:33.271493 angeltools-0.2.8/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.2.8/README.md
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.267493 angeltools-0.2.8/angeltools/
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.267493 angeltools-0.2.8/angeltools/Db/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.2.8/angeltools/Db/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3289 2022-04-21 02:57:31.000000 angeltools-0.2.8/angeltools/Db/redis_connector.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.2.8/angeltools/ImageTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.2.8/angeltools/MathTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.2.8/angeltools/Slavers.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    15430 2023-05-17 08:36:58.000000 angeltools-0.2.8/angeltools/StrTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.2.8/angeltools/TimeTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.2.8/angeltools/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.2.8/angeltools/commands.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.271493 angeltools-0.2.8/angeltools/fdfs/
+-rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.2.8/angeltools/fdfs/__init__.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.271493 angeltools-0.2.8/angeltools/fdfs/fdfs_client/
+-rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/connection.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/exceptions.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/fdfs_protol.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/fdfs_test.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/storage_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/tracker_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_client/utils.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.2.8/angeltools/fdfs/fdfs_operator.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-17 08:38:33.267493 angeltools-0.2.8/angeltools.egg-info/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/entry_points.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.2.8/angeltools.egg-info/not-zip-safe
+-rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/requires.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-05-17 08:38:33.000000 angeltools-0.2.8/angeltools.egg-info/top_level.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-05-17 08:38:33.271493 angeltools-0.2.8/setup.cfg
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-05-17 08:38:28.000000 angeltools-0.2.8/setup.py
```

### Comparing `angeltools-0.2.7/LICENSE` & `angeltools-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/PKG-INFO` & `angeltools-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.2.7
+Version: 0.2.8
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.2.7/README.md` & `angeltools-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/Db/__init__.py` & `angeltools-0.2.8/angeltools/Db/__init__.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/Db/redis_connector.py` & `angeltools-0.2.8/angeltools/Db/redis_connector.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/ImageTool.py` & `angeltools-0.2.8/angeltools/ImageTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/MathTool.py` & `angeltools-0.2.8/angeltools/MathTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/Slavers.py` & `angeltools-0.2.8/angeltools/Slavers.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/StrTool.py` & `angeltools-0.2.8/angeltools/StrTool.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,28 @@
 import random
 import re
 import sys
 import time
 import uuid
 from pathlib import Path
 
+import urllib3
 
-def get_domain(url):
-    import urllib3
 
-    domain = urllib3.get_host(url)[1]
-    if domain.startswith('www.'):
-        domain = domain.lstrip('www.')
+def get_domain(url):
+    domain = ''
+    if url and url.strip():
+        domain = urllib3.get_host(url)[1]
+        if '.' in url:
+            second_domain = domain.split('.')[-2]
+            if second_domain in {"com", "net", "org", "gov"}:
+                dml = domain.split(".")[-3:]
+            else:
+                dml = domain.split(".")[-2:]
+            domain = '.'.join(dml)
     return domain
 
 
 def hash_str(data):
     md5 = hashlib.md5()
     md5.update(str(data).encode('utf-8'))
     return md5.hexdigest()
@@ -214,25 +221,30 @@
                 if p and p not in new_url:
                     new_url = p + sep + new_url
         else:
             new_url = sep.join(path_lis)
         return new_url
 
 
+file_lock_prefix = 'file_lock_'
+
+
 class FileLock:
     """
     使用文件操作实现的异步锁
 
     使用方式：
     with FileLock(lock_id='xxxx', timeout=xx.xx):
         do_the_jobs()
 
     """
-    def __init__(self, lock_id, timeout: float or int = None):
+    def __init__(self, lock_id=None, timeout: float or int = None):
         self.timeout = float(timeout) if timeout else 3600 * 24 * 30 * 12
+        self.__lock_dir()
+        self.__get_lock_prefix()
         self.__init_lock(lock_id)
         self.fps = self.fp.absolute()
         self.enter_with_acquire = False
 
     def __enter__(self):
         if not self.enter_with_acquire:
             self.__acquire_lock()
@@ -240,21 +252,40 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.__exit_lock()
 
     def __call__(self, *args, **kwargs):
         if 'timeout' in kwargs:
             self.timeout = kwargs['timeout']
 
-    def __init_lock(self, lock_id):
-        lock_id_hash = hash_str(str(lock_id))
+    def clear(self, lock_id=None):
+        if lock_id:
+            self.__init_lock(lock_id)
+            self.__exit_lock()
+        else:
+            for file in os.listdir(self.lock_dir):
+                if file.startswith(file_lock_prefix):
+                    try:
+                        os.remove(self.lock_dir / file)
+                    except:
+                        pass
 
+    def __lock_dir(self):
         if sys.platform == 'linux':
-            self.fp = Path(f'/tmp/{lock_id_hash}.lock')
+            self.lock_dir = Path(f'/tmp/')
         else:
-            self.fp = Path(__file__).parent / f'/{lock_id_hash}.lock'
+            self.lock_dir = Path(__file__).parent / 'FileLock'
+
+    def __get_lock_prefix(self):
+        self.fp_prefix = self.lock_dir / file_lock_prefix
+
+    def __init_lock(self, lock_id):
+        if not lock_id:
+            lock_id = gen_uid1()
+        lock_id_hash = hash_str(str(lock_id))
+        self.fp = Path(f'{str(self.fp_prefix.absolute())}{lock_id_hash}.lock')
 
     def __acquire_lock(self):
         expire_time = time.time() + self.timeout
         try:
             while self.__get_size() and time.time() - expire_time < 0:
                 self.__wait()
         except KeyboardInterrupt:
@@ -270,21 +301,28 @@
         except:pass
         num = int(num) if num else 0
         return num
 
     def __get_size(self):
         return 0 if not os.path.exists(self.fps) else os.path.getsize(self.fps)
 
+    def __write_num(self, num):
+        with open(self.fps, 'w+') as wf:
+            wf.write(str(num))
+            wf.flush()
+
     def __add_num(self):
-        self.fp.write_text("1" * (self.__get_size() + 1))
+        # self.fp.write_text("1" * (self.__get_size() + 1))
+        self.__write_num("1" * (self.__get_size() + 1))
 
     def __sub_num(self):
         num = self.__get_size()
         if num > 1:
-            self.fp.write_text("1" * (num - 1))
+            # self.fp.write_text("1" * (num - 1))
+            self.__write_num("1" * (num - 1))
         else:
             os.remove(self.fps)
 
     def __occupy(self):
         if not self.fp.exists():
             return False
         num = self.fp.read_text(encoding='utf-8')
@@ -295,15 +333,15 @@
     def __exit_lock(self):
         try:
             self.__sub_num()
         except:
             pass
 
     def __wait(self):
-        time.sleep(random.randint(1, 10)/10)
+        time.sleep(random.randint(1, 5)/10)
 
     def acquire(self, **kwargs):
         if 'timeout' in kwargs:
             self.timeout = kwargs['timeout']
         self.enter_with_acquire = True
         return self.__acquire_lock()
 
@@ -399,33 +437,38 @@
             wf.writelines(sorted_lines)
 
         print(f"data saved: {hgreen(self.save_path)}")
 
 
 if __name__ == '__main__':
     # with FileLock('test-lock', timeout=10) as lock:
-    #     print(lock.lock_time(format_time=True))
+    #     # print(lock.lock_time(format_time=True))
     #     for i in range(100):
     #         print(i)
     #         time.sleep(0.5)
-    #     print(lock.lock_time(format_time=True))
+    #     # print(lock.lock_time(format_time=True))
+
+    def do_job(job_name):
+        time.sleep(random.randint(1, 10) / 10)
+        with FileLock(f'test-lock', timeout=12):
+            for i in range(10):
+                print(f"{job_name}: {i}")
+                time.sleep(0.5)
+                # if i == 5:
+                #     raise ValueError("进程出错了")
+
+
+    # do_job("进程1")
+    from angeltools.Slavers import BigSlaves
+    BigSlaves(7).work(do_job, ["进程1", "进程2", "进程3"])
 
-    # from angeltools.Slavers import BigSlaves
-    #
-    # def do_job(job_name):
-    #     time.sleep(random.randint(1, 10) / 10)
-    #     with FileLock('test-lock', timeout=1000):
-    #         for i in range(20):
-    #             print(f"{job_name}: {i}")
-    #             time.sleep(0.5)
-    #
-    # BigSlaves(7).work(do_job, [x for x in "ABCDEFGHIJKLMN"])
+    # FileLock().clear(lock_id='test-lock')
 
     # uf = UrlFormat('http://www.baidu.com?page=1&user=me&name=%E5%BC%A0%E4%B8%89')
     # print(uf.split_url())
 
-    SortedWithFirstPinyin(
-        file_path='/home/ga/Guardian/For-Python/AngelTools/angeltools/testfiles/res.txt',
-        # save_path=save_path,
-        full_match=True,
-        reverse=False,
-    ).run()
+    # SortedWithFirstPinyin(
+    #     file_path='/home/ga/Guardian/For-Python/AngelTools/angeltools/testfiles/res.txt',
+    #     # save_path=save_path,
+    #     full_match=True,
+    #     reverse=False,
+    # ).run()
```

### Comparing `angeltools-0.2.7/angeltools/TimeTool.py` & `angeltools-0.2.8/angeltools/TimeTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/commands.py` & `angeltools-0.2.8/angeltools/commands.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/fdfs/fdfs_client/client.py` & `angeltools-0.2.8/angeltools/fdfs/fdfs_client/client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/fdfs/fdfs_client/connection.py` & `angeltools-0.2.8/angeltools/fdfs/fdfs_client/connection.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/fdfs/fdfs_client/fdfs_protol.py` & `angeltools-0.2.8/angeltools/fdfs/fdfs_client/fdfs_protol.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/fdfs/fdfs_client/fdfs_test.py` & `angeltools-0.2.8/angeltools/fdfs/fdfs_client/fdfs_test.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/fdfs/fdfs_client/storage_client.py` & `angeltools-0.2.8/angeltools/fdfs/fdfs_client/storage_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/fdfs/fdfs_client/tracker_client.py` & `angeltools-0.2.8/angeltools/fdfs/fdfs_client/tracker_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/fdfs/fdfs_client/utils.py` & `angeltools-0.2.8/angeltools/fdfs/fdfs_client/utils.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools/fdfs/fdfs_operator.py` & `angeltools-0.2.8/angeltools/fdfs/fdfs_operator.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/angeltools.egg-info/PKG-INFO` & `angeltools-0.2.8/angeltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.2.7
+Version: 0.2.8
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.2.7/angeltools.egg-info/SOURCES.txt` & `angeltools-0.2.8/angeltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.7/setup.py` & `angeltools-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 using_setuptools = True
 
 setup_args = {
     "name": "angeltools",
-    "version": "0.2.7",
+    "version": "0.2.8",
     "url": "https://github.com/ga1008/angeltools",
     "description": "personal python small tools collection",
     "long_description": long_description,
     "author": "Guardian",
     "author_email": "zhling2012@live.com",
     "maintainer": "Guardian",
     "maintainer_email": "zhling2012@live.com",
```

