# Comparing `tmp/BingImageCreator-0.1.5.tar.gz` & `tmp/BingImageCreator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.1.5.tar", last modified: Sat May  6 04:28:38 2023, max compression
+gzip compressed data, was "BingImageCreator-0.2.0.tar", last modified: Wed May 17 01:32:01 2023, max compression
```

## Comparing `BingImageCreator-0.1.5.tar` & `BingImageCreator-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:28:38.788215 BingImageCreator-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 04:28:38.000000 BingImageCreator-0.1.5/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/src/BingImageCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:28:38.792215 BingImageCreator-0.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-06 04:28:11.000000 BingImageCreator-0.1.5/test/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 01:32:01.098792 BingImageCreator-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/test/test_example.py
```

### Comparing `BingImageCreator-0.1.5/LICENSE` & `BingImageCreator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.1.5/PKG-INFO` & `BingImageCreator-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.1.5
+Version: 0.2.0
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.1.5/README.md` & `BingImageCreator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.1.5/setup.py` & `BingImageCreator-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.1.5",
+    version="0.2.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.1.5/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.2.0/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.1.5
+Version: 0.2.0
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.1.5/src/BingImageCreator.py` & `BingImageCreator-0.2.0/src/BingImageCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,20 @@
             prompt: str
         """
         if not self.quiet:
             print(sending_message)
         if self.debug_file:
             self.debug(sending_message)
         url_encoded_prompt = requests.utils.quote(prompt)
+        payload = f"q={url_encoded_prompt}&qs=ds"
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
-        response = self.session.post(url, allow_redirects=False)
+        response = self.session.post(
+            url, allow_redirects=False, data=payload, timeout=200
+        )
         # check for content waring message
         if "this prompt has been blocked" in response.text.lower():
             if self.debug_file:
                 self.debug(f"ERROR: {error_blocked_prompt}")
             raise Exception(
                 error_blocked_prompt,
             )
@@ -155,29 +158,31 @@
             if img in bad_images:
                 raise Exception("Bad images")
         # No images
         if not normal_image_links:
             raise Exception(error_no_images)
         return normal_image_links
 
-    def save_images(self, links: list, output_dir: str,file_name:str=None) -> None:
+    def save_images(self, links: list, output_dir: str, file_name: str = None) -> None:
         """
         Saves images to output directory
         """
         if self.debug_file:
             self.debug(download_message)
         if not self.quiet:
             print(download_message)
         with contextlib.suppress(FileExistsError):
             os.mkdir(output_dir)
         try:
-            fn=f'{file_name}_' if file_name else ''
+            fn = f"{file_name}_" if file_name else ""
             jpeg_index = 0
             for link in links:
-                while os.path.exists(os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")):
+                while os.path.exists(
+                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")
+                ):
                     jpeg_index += 1
                 with self.session.get(link, stream=True) as response:
                     # save response to file
                     response.raise_for_status()
                     with open(
                         os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"), "wb"
                     ) as output_file:
@@ -217,15 +222,18 @@
             prompt: str
         """
         if not self.quiet:
             print("Sending request...")
         url_encoded_prompt = requests.utils.quote(prompt)
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
-        async with self.session.post(url, allow_redirects=False) as response:
+        payload = f"q={url_encoded_prompt}&qs=ds"
+        async with self.session.post(
+            url, allow_redirects=False, data=payload
+        ) as response:
             content = await response.text()
             if "this prompt has been blocked" in content.lower():
                 raise Exception(
                     "Your prompt has been blocked by Bing. Try to change any bad words and try again.",
                 )
             if response.status != 302:
                 # if rt4 fails, try rt3
```

### Comparing `BingImageCreator-0.1.5/test/test_example.py` & `BingImageCreator-0.2.0/test/test_example.py`

 * *Files identical despite different names*

