# Comparing `tmp/redis_simple_orm-2.0.0.tar.gz` & `tmp/redis_simple_orm-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_simple_orm-2.0.0.tar", last modified: Mon May 15 17:11:00 2023, max compression
+gzip compressed data, was "redis_simple_orm-2.0.1.tar", last modified: Wed May 17 09:06:11 2023, max compression
```

## Comparing `redis_simple_orm-2.0.0.tar` & `redis_simple_orm-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.763039 redis_simple_orm-2.0.0/RSO/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.763039 redis_simple_orm-2.0.0/RSO/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/asyncio/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/asyncio/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/RSO/txredisapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/txredisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/txredisapi/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/txredisapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.532223 redis_simple_orm-2.0.1/RSO/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/RSO/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/asyncio/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/asyncio/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/RSO/txredisapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/txredisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/txredisapi/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/RSO/txredisapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 09:06:11.000000 redis_simple_orm-2.0.1/redis_simple_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:06:11.536223 redis_simple_orm-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-17 09:05:57.000000 redis_simple_orm-2.0.1/tests/test_model.py
```

### Comparing `redis_simple_orm-2.0.0/LICENSE` & `redis_simple_orm-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.0/PKG-INFO` & `redis_simple_orm-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis_simple_orm
-Version: 2.0.0
+Version: 2.0.1
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-2.0.0/README.md` & `redis_simple_orm-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.0/RSO/asyncio/index.py` & `redis_simple_orm-2.0.1/RSO/asyncio/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.0/RSO/base.py` & `redis_simple_orm-2.0.1/RSO/base.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.0/RSO/index.py` & `redis_simple_orm-2.0.1/RSO/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.0/RSO/model.py` & `redis_simple_orm-2.0.1/RSO/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import List, Optional, Union
 
 from redis.client import Pipeline, Redis
 
 from RSO.base import BaseModel
 
 
 class Model(BaseModel):
@@ -21,24 +21,49 @@
                 continue
             index_class.save(pipe, self)
 
         if not isinstance(redis, Pipeline):
             pipe.execute()
 
     @classmethod
-    def search(cls, redis: Redis, value):
+    def search(cls, redis: Redis, value) -> Optional['Model']:
         redis_key = cls.redis_key_from_value(value)
         if bool(redis.exists(redis_key)):
             fields = cls.get_fields()
             redis_data = redis.hmget(redis_key, fields)
             dict_data = cls.from_redis(dict(zip(fields, redis_data)))
             return cls(**dict_data)
         else:
             return None
 
+    @classmethod
+    def all(cls, redis: Redis) -> List['Model']:
+        redis_key = cls.redis_key_from_value('*')
+        members = redis.keys(redis_key)
+        indexes = []
+        for index_class in cls.__indexes__:
+            indexes.append(
+                f'::{index_class.__index_name__}::{index_class.__key__}'
+            )
+        with redis.pipeline(transaction=True) as pipe:
+            for member in members:
+                is_index = False
+                for index in indexes:
+                    if index in member:
+                        is_index = True
+                        break
+                if not is_index:
+                    pipe.hgetall(member)
+            result_data = pipe.execute()
+
+        result = []
+        for data in result_data:
+            result.append(cls(**data))
+        return result
+
     def delete(self, redis: Union[Pipeline, Redis]):
         if isinstance(redis, Pipeline):
             pipe = redis
         else:
             pipe = redis.pipeline()
 
         for index_class in self.__indexes__:
```

### Comparing `redis_simple_orm-2.0.0/RSO/txredisapi/index.py` & `redis_simple_orm-2.0.1/RSO/txredisapi/index.py`

 * *Files 7% similar despite different names*

```diff
@@ -149,31 +149,31 @@
     @classmethod
     @inlineCallbacks
     def save(
         cls, redis: Union[BaseRedisProtocol, ConnectionHandler], model_obj: T
     ):
         if isinstance(redis, BaseRedisProtocol):
             redis.sadd(
-                cls.redis_key(model_obj),
-                cls.model_key_value(model_obj)
+                key=cls.redis_key(model_obj),
+                members=cls.model_key_value(model_obj)
             )
             returnValue(None)
         else:
             yield redis.sadd(
-                cls.redis_key(model_obj),
+                key=cls.redis_key(model_obj),
                 members=cls.model_key_value(model_obj)
             )
 
     @classmethod
     @inlineCallbacks
     def remove(
         cls, redis: Union[BaseRedisProtocol, ConnectionHandler], model_obj: T
     ):
         yield redis.srem(
-            cls.redis_key(model_obj),
+            key=cls.redis_key(model_obj),
             members=cls.model_key_value(model_obj)
         )
 
     @classmethod
     @inlineCallbacks
     def get_members(
         cls, redis: ConnectionHandler, index_value: Any
```

### Comparing `redis_simple_orm-2.0.0/redis_simple_orm.egg-info/PKG-INFO` & `redis_simple_orm-2.0.1/redis_simple_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-simple-orm
-Version: 2.0.0
+Version: 2.0.1
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-2.0.0/setup.py` & `redis_simple_orm-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.0/tests/test_example.py` & `redis_simple_orm-2.0.1/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.0/tests/test_index.py` & `redis_simple_orm-2.0.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-2.0.0/tests/test_model.py` & `redis_simple_orm-2.0.1/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .models.redispy import (
     UserModel,
     SingleIndexUsername,
     SingleIndexEmail,
     SetIndexGroupID,
     NoPrefixUserModel
 )
+from .data import USERS
 
 
 class TestModelCreate:
     def test_redis_key(self):
         # With prefix
         user = UserModel(
             user_id=1, username='test', email='test@create.success',
@@ -80,14 +81,26 @@
 
         assert UserModel.search(sync_redis, user.user_id) \
                is not None
 
     def test_not_found(self, sync_redis):
         assert UserModel.search(sync_redis, 1) is None
 
+    def test_get_all_success(self, sync_redis):
+        users = UserModel.all(sync_redis)
+        assert len(users) == 0
+
+        for data in USERS:
+            user = UserModel(**data)
+            user.save(sync_redis)
+
+        users = UserModel.all(sync_redis)
+        assert len(users) == len(USERS)
+        assert isinstance(users[0], UserModel)
+
 
 class TestModelDelete:
     def test_success(self, sync_redis):
         user = UserModel(
             user_id=1,
             username='test_create_success',
             email='test@create.success',
```

