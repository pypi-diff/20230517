# Comparing `tmp/imaginepy-1.0.5.tar.gz` & `tmp/imaginepy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaginepy-1.0.5.tar", last modified: Wed May 17 16:48:07 2023, max compression
+gzip compressed data, was "imaginepy-1.0.7.tar", last modified: Wed May 17 20:39:56 2023, max compression
```

## Comparing `imaginepy-1.0.5.tar` & `imaginepy-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:48:07.370766 imaginepy-1.0.5/
--rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     4054 2023-05-17 16:48:07.370267 imaginepy-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3355 2023-05-14 18:30:19.000000 imaginepy-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 16:48:07.351766 imaginepy-1.0.5/imaginepy/
--rw-rw-rw-   0        0        0    25557 2023-05-17 16:43:19.000000 imaginepy-1.0.5/imaginepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:48:07.369266 imaginepy-1.0.5/imaginepy.egg-info/
--rw-rw-rw-   0        0        0     4054 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-17 16:48:07.000000 imaginepy-1.0.5/imaginepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 16:48:07.370766 imaginepy-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1045 2023-05-17 16:44:25.000000 imaginepy-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:39:56.353000 imaginepy-1.0.7/
+-rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4026 2023-05-17 20:39:56.352501 imaginepy-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3355 2023-05-14 18:30:19.000000 imaginepy-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 20:39:56.334000 imaginepy-1.0.7/imaginepy/
+-rw-rw-rw-   0        0        0    25623 2023-05-17 20:37:40.000000 imaginepy-1.0.7/imaginepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:39:56.351001 imaginepy-1.0.7/imaginepy.egg-info/
+-rw-rw-rw-   0        0        0     4026 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 20:39:56.353000 imaginepy-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-05-17 20:36:32.000000 imaginepy-1.0.7/setup.py
```

### Comparing `imaginepy-1.0.5/LICENSE` & `imaginepy-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `imaginepy-1.0.5/PKG-INFO` & `imaginepy-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: imaginepy
-Version: 1.0.5
+Version: 1.0.7
 Summary: Python library to create Art with AI.
-Home-page: https://github.com/ItsCEED/ImaginePY-Midjourney-Free-Alternative
+Home-page: https://github.com/ItsCEED/imaginepy
 Author: CEED
 Author-email: 
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `imaginepy-1.0.5/README.md` & `imaginepy-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `imaginepy-1.0.5/imaginepy/__init__.py` & `imaginepy-1.0.7/imaginepy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
         return self._request(
             method="POST",
             url=f"{self.api}/variate",
             data=multi,
             headers=headers
         ).content
 
-    def sdprem(self, prompt: str, negative: str = None, priority: str = None, high_res_results: str = None, style: Style = Style.IMAGINE_V1, seed: str = None, ratio: Ratio = Ratio.RATIO_1X1, cfg: float = 9.5) -> bytes:
+    def sdprem(self, prompt: str, negative: str = None, priority: str = None, steps: str = None, high_res_results: str = None, style: Style = Style.IMAGINE_V1, seed: str = None, ratio: Ratio = Ratio.RATIO_1X1, cfg: float = 9.5) -> bytes:
         """Generates AI Art."""
         try:
             validated_cfg = validate_cfg(cfg)
         except Exception as e:
             print(f"An error occurred while validating cfg: {e}")
             return None
 
@@ -256,17 +256,18 @@
                     "model_version": self.version,
                     "prompt": prompt + (style.value[3] or ""),
                     "negative_prompt": negative or "",
                     "style_id": style.value[0],
                     "width": ratio.value[0],
                     "height": ratio.value[1],
                     "seed": seed or "",
+                    "steps": steps or "30",
                     "cfg": validated_cfg,
-                    "priority": priority or "",
-                    "high_res_results": high_res_results or ""
+                    "priority": priority or "0",
+                    "high_res_results": high_res_results or "0"
                 }
             ).content
         except Exception as e:
             print(f"An error occurred while making the request: {e}")
             return None
 
     def upscale(self, image: bytes) -> bytes:
@@ -356,8 +357,8 @@
             method="POST",
             url=f"{self.api}/controlnet",
             data=multi,
             headers=headers
         ).content
 
 
-__version__ = "1.0.5"
+__version__ = "1.0.7"
```

### Comparing `imaginepy-1.0.5/imaginepy.egg-info/PKG-INFO` & `imaginepy-1.0.7/imaginepy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: imaginepy
-Version: 1.0.5
+Version: 1.0.7
 Summary: Python library to create Art with AI.
-Home-page: https://github.com/ItsCEED/ImaginePY-Midjourney-Free-Alternative
+Home-page: https://github.com/ItsCEED/imaginepy
 Author: CEED
 Author-email: 
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `imaginepy-1.0.5/setup.py` & `imaginepy-1.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='imaginepy',
-    version='1.0.5',
+    version='1.0.7',
     author='CEED',
     author_email='',
     description='Python library to create Art with AI.',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/ItsCEED/ImaginePY-Midjourney-Free-Alternative',
+    url='https://github.com/ItsCEED/imaginepy',
     packages=find_packages(),
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
```

