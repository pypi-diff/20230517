# Comparing `tmp/jupyterhub-backendspawner-0.2.6.tar.gz` & `tmp/jupyterhub-backendspawner-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.2.6.tar", last modified: Mon May 15 15:13:23 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.3.0.tar", last modified: Wed May 17 13:03:16 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.2.6.tar` & `jupyterhub-backendspawner-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 15:13:23.600605 jupyterhub-backendspawner-0.2.6/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.6/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-15 15:13:23.600605 jupyterhub-backendspawner-0.2.6/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 15:13:23.600605 jupyterhub-backendspawner-0.2.6/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.6/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.2.6/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17351 2023-05-15 14:54:00.000000 jupyterhub-backendspawner-0.2.6/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10710 2023-05-15 15:01:05.000000 jupyterhub-backendspawner-0.2.6/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 15:13:23.600605 jupyterhub-backendspawner-0.2.6/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-15 15:13:23.000000 jupyterhub-backendspawner-0.2.6/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-15 15:13:23.000000 jupyterhub-backendspawner-0.2.6/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-15 15:13:23.000000 jupyterhub-backendspawner-0.2.6/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-15 15:13:23.000000 jupyterhub-backendspawner-0.2.6/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-15 15:13:23.000000 jupyterhub-backendspawner-0.2.6/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-15 15:13:23.600605 jupyterhub-backendspawner-0.2.6/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-15 15:11:39.000000 jupyterhub-backendspawner-0.2.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.3.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.3.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.3.0/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.3.0/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17351 2023-05-15 14:54:00.000000 jupyterhub-backendspawner-0.3.0/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10231 2023-05-17 12:59:06.000000 jupyterhub-backendspawner-0.3.0/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-17 12:59:38.000000 jupyterhub-backendspawner-0.3.0/setup.py
```

### Comparing `jupyterhub-backendspawner-0.2.6/LICENSE` & `jupyterhub-backendspawner-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.6/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.3.0/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.6/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.3.0/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.6/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.3.0/backendspawner/eventspawner.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,25 +120,14 @@
         pattern = re.compile(
             r"([0-9]+(_[0-9]+)+).*[0-9]{2}:[0-9]{2}:[0-9]{2}(\\.[0-9]{1,3})?"
         )
         message = event["html_message"]
         match = re.search(pattern, message)
         return match.group()
 
-    def get_ready_event(self):
-        event = super().get_ready_event()
-        ready_msg = f"Service {self.name} started."
-        now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
-        url = url_path_join(self.user.url, self.name, "/")
-        event[
-            "html_message"
-        ] = f'<details><summary>{now}: {ready_msg}</summary>You will be redirected to <a href="{url}">{url}</a></details>'
-        self.latest_events.append(event)
-        return event
-
     cancelling_event = Union(
         [Dict(), Callable()],
         default_value={
             "failed": False,
             "ready": False,
             "progress": 99,
             "message": "",
```

### Comparing `jupyterhub-backendspawner-0.2.6/setup.py` & `jupyterhub-backendspawner-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.2.6",
+    version="0.3.0",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

