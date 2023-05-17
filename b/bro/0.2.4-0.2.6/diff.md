# Comparing `tmp/bro-0.2.4.tar.gz` & `tmp/bro-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bro-0.2.4.tar", last modified: Fri Apr  7 13:13:49 2023, max compression
+gzip compressed data, was "bro-0.2.6.tar", last modified: Wed May 17 13:38:17 2023, max compression
```

## Comparing `bro-0.2.4.tar` & `bro-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:13:49.220624 bro-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-07 13:13:25.000000 bro-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-07 13:13:49.220624 bro-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-07 13:13:25.000000 bro-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:13:49.220624 bro-0.2.4/bro/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-07 13:13:25.000000 bro-0.2.4/bro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-07 13:13:25.000000 bro-0.2.4/bro/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-07 13:13:25.000000 bro-0.2.4/bro/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-07 13:13:25.000000 bro-0.2.4/bro/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-07 13:13:25.000000 bro-0.2.4/bro/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:13:49.220624 bro-0.2.4/bro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-07 13:13:49.000000 bro-0.2.4/bro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 13:13:49.000000 bro-0.2.4/bro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 13:13:49.000000 bro-0.2.4/bro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-07 13:13:49.000000 bro-0.2.4/bro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 13:13:49.000000 bro-0.2.4/bro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:13:49.220624 bro-0.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 13:13:25.000000 bro-0.2.4/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-07 13:13:25.000000 bro-0.2.4/examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-07 13:13:25.000000 bro-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 13:13:49.220624 bro-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-07 13:13:25.000000 bro-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:13:49.220624 bro-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-07 13:13:25.000000 bro-0.2.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-07 13:13:25.000000 bro-0.2.4/tests/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:38:17.930089 bro-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 13:37:57.000000 bro-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-17 13:38:17.930089 bro-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-17 13:37:57.000000 bro-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:38:17.930089 bro-0.2.6/bro/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-17 13:37:57.000000 bro-0.2.6/bro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 13:37:57.000000 bro-0.2.6/bro/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-05-17 13:37:57.000000 bro-0.2.6/bro/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-17 13:37:57.000000 bro-0.2.6/bro/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-17 13:37:57.000000 bro-0.2.6/bro/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:38:17.930089 bro-0.2.6/bro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-17 13:38:17.000000 bro-0.2.6/bro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-17 13:38:17.000000 bro-0.2.6/bro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:38:17.000000 bro-0.2.6/bro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 13:38:17.000000 bro-0.2.6/bro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 13:38:17.000000 bro-0.2.6/bro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:38:17.930089 bro-0.2.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:37:57.000000 bro-0.2.6/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-17 13:37:57.000000 bro-0.2.6/examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-17 13:37:57.000000 bro-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:38:17.930089 bro-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 13:37:57.000000 bro-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:38:17.930089 bro-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-17 13:37:57.000000 bro-0.2.6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-17 13:37:57.000000 bro-0.2.6/tests/test_objects.py
```

### Comparing `bro-0.2.4/LICENSE.txt` & `bro-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bro-0.2.4/PKG-INFO` & `bro-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: bro
-Version: 0.2.4
+Version: 0.2.6
 Summary: Open source python library for accessing BRO API
-Home-page: https://github.com/viktor-platform/bro
 Author: VIKTOR
 Author-email: support@viktor.ai
 License: see LICENSE.txt
+Project-URL: Source code, https://github.com/viktor-platform/bro
 Project-URL: Example VIKTOR application, https://demo.viktor.ai/public/bro-app
 Project-URL: Source code VIKTOR application, https://github.com/viktor-platform/bro-app
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: Free To Use But Restricted
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-![](https://img.shields.io/badge/release-v0.2.4-green)
+![](https://img.shields.io/badge/release-v0.2.6-green)
 
 # BRO
 This package can access the REST API from the [BRO](https://www.broloket.nl/ondergrondgegevens). Currently, this package provides
 functionality to request CPTs from the BRO when you provide a region of interest. The format is based on the REST API of the BRO, which is described [here](https://publiek.broservices.nl/sr/cpt/v1/swagger-ui/#/default/) for CPTs.
 
 Current options include retrieval of the following objects: 
 1. CPTs (format: bytes, dict)
@@ -89,9 +89,9 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 ```
 
 ## Publish
 - update changelog with version number
-- update bro/__version__.py
+- update `bro/__version__.py`
 - tag with version number
```

### Comparing `bro-0.2.4/bro/api.py` & `bro-0.2.6/bro/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         self.cpt_standard: Optional[str] = (
             parsed_dispatch_document["cptStandard"]["value"] if parsed_dispatch_document.get("cptStandard") else None
         )
         self.offset: Optional[float] = (
             float(parsed_dispatch_document["offset"]["value"]) if parsed_dispatch_document.get("offset") else None
         )
         self.quality_class: Optional[str] = (
-            parsed_dispatch_document["qualityClass"] if parsed_dispatch_document.get("offset") else None
+            parsed_dispatch_document["qualityClass"]["value"] if parsed_dispatch_document.get("qualityClass") else None
         )
         self.research_report_date: Optional[str] = (
             parsed_dispatch_document["researchReportDate"]["brocom:date"]
             if parsed_dispatch_document.get("researchReportDate")
             else None
         )
         self.start_time: Optional[str] = parsed_dispatch_document.get("startTime")
```

### Comparing `bro-0.2.4/bro/helper_functions.py` & `bro-0.2.6/bro/helper_functions.py`

 * *Files identical despite different names*

### Comparing `bro-0.2.4/bro/objects.py` & `bro-0.2.6/bro/objects.py`

 * *Files identical despite different names*

### Comparing `bro-0.2.4/bro.egg-info/PKG-INFO` & `bro-0.2.6/bro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: bro
-Version: 0.2.4
+Version: 0.2.6
 Summary: Open source python library for accessing BRO API
-Home-page: https://github.com/viktor-platform/bro
 Author: VIKTOR
 Author-email: support@viktor.ai
 License: see LICENSE.txt
+Project-URL: Source code, https://github.com/viktor-platform/bro
 Project-URL: Example VIKTOR application, https://demo.viktor.ai/public/bro-app
 Project-URL: Source code VIKTOR application, https://github.com/viktor-platform/bro-app
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: Free To Use But Restricted
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-![](https://img.shields.io/badge/release-v0.2.4-green)
+![](https://img.shields.io/badge/release-v0.2.6-green)
 
 # BRO
 This package can access the REST API from the [BRO](https://www.broloket.nl/ondergrondgegevens). Currently, this package provides
 functionality to request CPTs from the BRO when you provide a region of interest. The format is based on the REST API of the BRO, which is described [here](https://publiek.broservices.nl/sr/cpt/v1/swagger-ui/#/default/) for CPTs.
 
 Current options include retrieval of the following objects: 
 1. CPTs (format: bytes, dict)
@@ -89,9 +89,9 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 ```
 
 ## Publish
 - update changelog with version number
-- update bro/__version__.py
+- update `bro/__version__.py`
 - tag with version number
```

### Comparing `bro-0.2.4/examples/examples.py` & `bro-0.2.6/examples/examples.py`

 * *Files identical despite different names*

### Comparing `bro-0.2.4/pyproject.toml` & `bro-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bro-0.2.4/setup.py` & `bro-0.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,48 +3,46 @@
 from setuptools import find_packages
 from setuptools import setup
 
 about = {}
 with open(Path(__file__).parent / "bro" / "__version__.py", "r") as f:
     exec(f.read(), about)
 
-license_content = (Path(__file__).parent / "LICENSE.txt").read_text()
 long_description = (Path(__file__).parent / "README.md").read_text()
 long_description = long_description.replace("X.Y.Z", about["__version__"])
-long_description = long_description.replace("LICENSE-PLACEHOLDER", license_content)
 
 setup(
     name="bro",
     version=about["__version__"],
     description="Open source python library for accessing BRO API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/viktor-platform/bro",
     author="VIKTOR",
     author_email="support@viktor.ai",
     license="see LICENSE.txt",
     license_files=("LICENSE.txt",),
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "xmltodict==0.13.0",
         "requests==2.28.2",
         "lxml==4.9.2",
         "pyproj==3.4.1",
     ],
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
-        "License :: Free To Use But Restricted",
+        "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     test_suite="tests",
     project_urls={
+        "Source code": "https://github.com/viktor-platform/bro",
         "Example VIKTOR application": "https://demo.viktor.ai/public/bro-app",
         "Source code VIKTOR application": "https://github.com/viktor-platform/bro-app",
     },
 )
```

### Comparing `bro-0.2.4/tests/test_api.py` & `bro-0.2.6/tests/test_api.py`

 * *Files identical despite different names*

