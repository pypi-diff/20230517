# Comparing `tmp/bev-0.7.1.tar.gz` & `tmp/bev-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bev-0.7.1.tar", last modified: Wed May 10 13:20:05 2023, max compression
+gzip compressed data, was "bev-0.8.0.tar", last modified: Wed May 17 14:15:25 2023, max compression
```

## Comparing `bev-0.7.1.tar` & `bev-0.8.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.399525 bev-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-05-10 13:20:03.000000 bev-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 13:20:03.000000 bev-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-10 13:20:05.395525 bev-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-10 13:20:03.000000 bev-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.395525 bev-0.7.1/bev/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-10 13:20:03.000000 bev-0.7.1/bev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 13:20:03.000000 bev-0.7.1/bev/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.395525 bev-0.7.1/bev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/blame.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.395525 bev-0.7.1/bev/config/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-10 13:20:03.000000 bev-0.7.1/bev/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-10 13:20:03.000000 bev-0.7.1/bev/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-10 13:20:03.000000 bev-0.7.1/bev/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-10 13:20:03.000000 bev-0.7.1/bev/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-10 13:20:03.000000 bev-0.7.1/bev/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-10 13:20:03.000000 bev-0.7.1/bev/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-10 13:20:03.000000 bev-0.7.1/bev/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:03.000000 bev-0.7.1/bev/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-10 13:20:03.000000 bev-0.7.1/bev/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-10 13:20:03.000000 bev-0.7.1/bev/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-10 13:20:03.000000 bev-0.7.1/bev/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-10 13:20:03.000000 bev-0.7.1/bev/vc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-10 13:20:03.000000 bev-0.7.1/bev/wc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.395525 bev-0.7.1/bev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-10 13:20:03.000000 bev-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 13:20:03.000000 bev-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:20:05.399525 bev-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-10 13:20:03.000000 bev-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.972943 bev-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-05-17 14:15:21.000000 bev-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-17 14:15:21.000000 bev-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-17 14:15:25.972943 bev-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-17 14:15:21.000000 bev-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.968943 bev-0.8.0/bev/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-17 14:15:21.000000 bev-0.8.0/bev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 14:15:21.000000 bev-0.8.0/bev/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.972943 bev-0.8.0/bev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/blame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.972943 bev-0.8.0/bev/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-17 14:15:21.000000 bev-0.8.0/bev/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-17 14:15:21.000000 bev-0.8.0/bev/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-17 14:15:21.000000 bev-0.8.0/bev/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-17 14:15:21.000000 bev-0.8.0/bev/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-17 14:15:21.000000 bev-0.8.0/bev/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-17 14:15:21.000000 bev-0.8.0/bev/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-17 14:15:21.000000 bev-0.8.0/bev/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:21.000000 bev-0.8.0/bev/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-17 14:15:21.000000 bev-0.8.0/bev/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-17 14:15:21.000000 bev-0.8.0/bev/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-17 14:15:21.000000 bev-0.8.0/bev/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-17 14:15:21.000000 bev-0.8.0/bev/vc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-17 14:15:21.000000 bev-0.8.0/bev/wc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.968943 bev-0.8.0/bev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-17 14:15:21.000000 bev-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 14:15:21.000000 bev-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:15:25.972943 bev-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-17 14:15:21.000000 bev-0.8.0/setup.py
```

### Comparing `bev-0.7.1/LICENSE` & `bev-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/PKG-INFO` & `bev-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.7.1
+Version: 0.8.0
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
 License: MIT
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.7.1.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.8.0.tar.gz
 Keywords: data,version control
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bev-0.7.1/README.md` & `bev-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/add.py` & `bev-0.8.0/bev/cli/add.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/app.py` & `bev-0.8.0/bev/cli/app.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/blame.py` & `bev-0.8.0/bev/cli/blame.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/fetch.py` & `bev-0.8.0/bev/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/init.py` & `bev-0.8.0/bev/cli/init.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/pull.py` & `bev-0.8.0/bev/cli/pull.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/storage.py` & `bev-0.8.0/bev/cli/storage.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/update.py` & `bev-0.8.0/bev/cli/update.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/cli/utils.py` & `bev-0.8.0/bev/cli/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/config/base.py` & `bev-0.8.0/bev/config/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 
 class ConfigMeta(NoExtra):
     choose: str = None
     fallback: str = None
     order: str = None
     hash: Union[str, HashConfig] = None
     include: Sequence[Include] = ()
+    labels: Optional[Sequence[str]] = None
 
     _override = 'fallback', 'order', 'choose', 'hash'
 
     @validator('hash', pre=True)
     def normalize_hash(cls, v):
         if isinstance(v, str):
             v = {'name': v}
```

### Comparing `bev-0.7.1/bev/config/hostname.py` & `bev-0.8.0/bev/config/hostname.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/config/include.py` & `bev-0.8.0/bev/config/include.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/config/parse.py` & `bev-0.8.0/bev/config/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,21 +28,23 @@
     order_func: Callable[[Sequence[Location]], Sequence[Location]] = identity
     if meta.order is not None:
         path, attr = meta.order.rsplit('.', 1)
         order_func = getattr(importlib.import_module(path), attr)
 
     storage = HashKeyStorage(
         wrap_levels(config.local.storage, DiskDict, order_func),
-        remote=filter_remotes([remote.storage for remote in config.remotes])
+        remote=filter_remotes([remote.storage for remote in config.remotes]),
+        labels=meta.labels,
     )
     index = None
     if config.local.cache is not None:
         cache_storage = HashKeyStorage(
             wrap_levels(config.local.cache.storage, DiskDict, order_func),
-            remote=filter_remotes([remote.cache.storage for remote in config.remotes if remote.cache is not None])
+            remote=filter_remotes([remote.cache.storage for remote in config.remotes if remote.cache is not None]),
+            labels=meta.labels,
         )
         index = CacheStorageIndex(
             tuple(_filter_levels(config.local.cache.index)),
             filter_remotes([remote.cache.index for remote in config.remotes if remote.cache is not None]),
             cache_storage,
         )
     return storage, index
```

### Comparing `bev-0.7.1/bev/config/registry.py` & `bev-0.8.0/bev/config/registry.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/config/remote.py` & `bev-0.8.0/bev/config/remote.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/config/utils.py` & `bev-0.8.0/bev/config/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/hash.py` & `bev-0.8.0/bev/hash.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/interface.py` & `bev-0.8.0/bev/interface.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/ops.py` & `bev-0.8.0/bev/ops.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/shortcuts.py` & `bev-0.8.0/bev/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/testing.py` & `bev-0.8.0/bev/testing.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/utils.py` & `bev-0.8.0/bev/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/vc.py` & `bev-0.8.0/bev/vc.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev/wc.py` & `bev-0.8.0/bev/wc.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/bev.egg-info/PKG-INFO` & `bev-0.8.0/bev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.7.1
+Version: 0.8.0
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
 License: MIT
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.7.1.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.8.0.tar.gz
 Keywords: data,version control
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bev-0.7.1/bev.egg-info/SOURCES.txt` & `bev-0.8.0/bev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/pyproject.toml` & `bev-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bev-0.7.1/setup.py` & `bev-0.8.0/setup.py`

 * *Files identical despite different names*

