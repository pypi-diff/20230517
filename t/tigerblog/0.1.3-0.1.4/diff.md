# Comparing `tmp/tigerblog-0.1.3.tar.gz` & `tmp/tigerblog-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigerblog-0.1.3.tar", last modified: Sat May 13 20:49:38 2023, max compression
+gzip compressed data, was "tigerblog-0.1.4.tar", last modified: Wed May 17 08:15:50 2023, max compression
```

## Comparing `tigerblog-0.1.3.tar` & `tigerblog-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,37 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-13 20:49:38.393877 tigerblog-0.1.3/
--rw-r--r--   0 user      (1000) user      (1000)    11358 2023-05-13 19:28:39.000000 tigerblog-0.1.3/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)      842 2023-05-13 20:49:38.393877 tigerblog-0.1.3/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      358 2023-05-13 19:37:09.000000 tigerblog-0.1.3/README.md
--rw-r--r--   0 user      (1000) user      (1000)      344 2023-05-13 20:49:38.393877 tigerblog-0.1.3/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      994 2023-05-13 20:49:25.000000 tigerblog-0.1.3/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-13 20:49:38.392877 tigerblog-0.1.3/tigerblog/
--rw-r--r--   0 user      (1000) user      (1000)      163 2023-05-13 19:36:22.000000 tigerblog-0.1.3/tigerblog/config.json
--rwxr-xr-x   0 user      (1000) user      (1000)    11633 2023-05-13 20:41:31.000000 tigerblog-0.1.3/tigerblog/tigerblog.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-13 20:49:38.393877 tigerblog-0.1.3/tigerblog.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      842 2023-05-13 20:49:38.000000 tigerblog-0.1.3/tigerblog.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      313 2023-05-13 20:49:38.000000 tigerblog-0.1.3/tigerblog.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-13 20:49:38.000000 tigerblog-0.1.3/tigerblog.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       54 2023-05-13 20:49:38.000000 tigerblog-0.1.3/tigerblog.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)      108 2023-05-13 20:49:38.000000 tigerblog-0.1.3/tigerblog.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       10 2023-05-13 20:49:38.000000 tigerblog-0.1.3/tigerblog.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-13 20:05:19.000000 tigerblog-0.1.3/tigerblog.egg-info/zip-safe
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 08:15:50.138986 tigerblog-0.1.4/
+-rw-r--r--   0 user      (1000) user      (1000)    11358 2023-05-13 19:28:39.000000 tigerblog-0.1.4/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)       36 2023-05-17 08:15:37.000000 tigerblog-0.1.4/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)      842 2023-05-17 08:15:50.138986 tigerblog-0.1.4/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      358 2023-05-13 19:37:09.000000 tigerblog-0.1.4/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      344 2023-05-17 08:15:50.138986 tigerblog-0.1.4/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1035 2023-05-17 08:15:37.000000 tigerblog-0.1.4/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 08:15:50.121986 tigerblog-0.1.4/tigerblog/
+-rw-r--r--   0 user      (1000) user      (1000)      162 2023-05-17 08:15:37.000000 tigerblog-0.1.4/tigerblog/config.json
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 08:15:50.111986 tigerblog-0.1.4/tigerblog/themes/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 08:15:50.125986 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/
+-rw-r--r--   0 user      (1000) user      (1000)     1651 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/contact.html
+-rw-r--r--   0 user      (1000) user      (1000)      372 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/listing.html
+-rw-r--r--   0 user      (1000) user      (1000)      555 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/macros.html
+-rw-r--r--   0 user      (1000) user      (1000)     3370 2023-05-13 21:02:45.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/master.html
+-rw-r--r--   0 user      (1000) user      (1000)       94 2023-05-13 19:52:56.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/navlinks.html
+-rw-r--r--   0 user      (1000) user      (1000)     6386 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/post.html
+-rw-r--r--   0 user      (1000) user      (1000)      211 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/sidebar.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 08:15:50.111986 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 08:15:50.128986 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/css/
+-rw-r--r--   0 user      (1000) user      (1000)     3527 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/css/single-blog.css
+-rw-r--r--   0 user      (1000) user      (1000)     6888 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/css/style.css
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 08:15:50.137986 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/images/
+-rw-r--r--   0 user      (1000) user      (1000)    45454 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/images/aside-logo.svg
+-rw-r--r--   0 user      (1000) user      (1000)     1150 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/images/favicon.ico
+-rw-r--r--   0 user      (1000) user      (1000)    30029 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/images/logo-white.png
+-rw-r--r--   0 user      (1000) user      (1000)   268427 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/images/logo.jpg
+-rw-r--r--   0 user      (1000) user      (1000)    45423 2023-05-13 19:28:39.000000 tigerblog-0.1.4/tigerblog/themes/beautiful-tiger/static/images/nav-logo.svg
+-rwxr-xr-x   0 user      (1000) user      (1000)    11603 2023-05-17 08:15:37.000000 tigerblog-0.1.4/tigerblog/tigerblog.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-17 08:15:50.122986 tigerblog-0.1.4/tigerblog.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      842 2023-05-17 08:15:50.000000 tigerblog-0.1.4/tigerblog.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1056 2023-05-17 08:15:50.000000 tigerblog-0.1.4/tigerblog.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-17 08:15:50.000000 tigerblog-0.1.4/tigerblog.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       54 2023-05-17 08:15:50.000000 tigerblog-0.1.4/tigerblog.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      108 2023-05-17 08:15:50.000000 tigerblog-0.1.4/tigerblog.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2023-05-17 08:15:50.000000 tigerblog-0.1.4/tigerblog.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-13 20:05:19.000000 tigerblog-0.1.4/tigerblog.egg-info/zip-safe
```

### Comparing `tigerblog-0.1.3/LICENSE.txt` & `tigerblog-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tigerblog-0.1.3/PKG-INFO` & `tigerblog-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigerblog
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simplest Blog Engine for Developers
 Home-page: https://github.com/tigerteamx/tigerblog
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: blog,productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tigerblog-0.1.3/setup.py` & `tigerblog-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 
 setuptools.setup(
     name="tigerblog",
     packages=["tigerblog"],
     package_dir={"tigerblog": "tigerblog"},
     package_data={
-        'tigerblog': ['config.json', "themes/*"]
+        'tigerblog': ['config.json', 'themes/*'],
+        'tigerblog.themes.abc': ["**"],
     },
-    version="0.1.3",
+    version="0.1.4",
     author="Martin F",
     author_email="pypi.org@tigerteamx.com",
     description="Simplest Blog Engine for Developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tigerteamx/tigerblog",
     install_requires=[],  # Used for dependencies
```

### Comparing `tigerblog-0.1.3/tigerblog/tigerblog.py` & `tigerblog-0.1.4/tigerblog/tigerblog.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 continue
 
             page_data = read_page(fn)
             tags = []
             for tag in page_data['tags']:
                 tags.append(Tag(
                     title=tag,
-                    slug=f'/tags/{slugify(tag)}',
+                    slug=f'tags/{slugify(tag)}',
                     url=f"{self.config['host']}/tags/{slugify(tag)}/"),
                 )
 
             path = fn[len(self.config['content_path']):]
 
             if path.endswith("index.md"):
                 # if path is of format /my-blog-post/index.md
@@ -316,15 +316,15 @@
     )
 
     for tag in blog.tags:
         blog.write_listing(
             f"{blog.config['tmp']}/{tag.slug}/index.html",
             blog.get_pages_with_tag(tag),
             tag,
-            f'{blog.config["host"]}/{tag.slug}/',
+            tag.url,
         )
     blog.copy_files()
 
     if Path(f'{blog.config["theme"]}/static').is_dir():
         shutil.copytree(f'{blog.config["theme"]}/static', f"{blog.config['tmp']}/static")
 
     if Path('static').is_dir():
```

### Comparing `tigerblog-0.1.3/tigerblog.egg-info/PKG-INFO` & `tigerblog-0.1.4/tigerblog.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigerblog
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simplest Blog Engine for Developers
 Home-page: https://github.com/tigerteamx/tigerblog
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: blog,productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

