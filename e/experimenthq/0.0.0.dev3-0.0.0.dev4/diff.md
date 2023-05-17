# Comparing `tmp/experimenthq-0.0.0.dev3.tar.gz` & `tmp/experimenthq-0.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimenthq-0.0.0.dev3.tar", last modified: Sun May 14 20:27:11 2023, max compression
+gzip compressed data, was "experimenthq-0.0.0.dev4.tar", last modified: Wed May 17 00:15:12 2023, max compression
```

## Comparing `experimenthq-0.0.0.dev3.tar` & `experimenthq-0.0.0.dev4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:27:11.906046 experimenthq-0.0.0.dev3/
--rw-r--r--   0 ramonabendias   (501) staff       (20)     1071 2023-04-28 20:27:57.000000 experimenthq-0.0.0.dev3/LICENSE
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3991 2023-05-14 20:27:11.906144 experimenthq-0.0.0.dev3/PKG-INFO
--rw-r--r--   0 ramonabendias   (501) staff       (20)     2383 2023-05-14 20:21:42.000000 experimenthq-0.0.0.dev3/README.md
--rw-r--r--   0 ramonabendias   (501) staff       (20)      983 2023-05-14 20:27:11.906506 experimenthq-0.0.0.dev3/setup.cfg
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3501 2023-05-14 19:42:35.000000 experimenthq-0.0.0.dev3/setup.py
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:27:11.902568 experimenthq-0.0.0.dev3/src/
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:27:11.904640 experimenthq-0.0.0.dev3/src/experimenthq/
--rw-r--r--   0 ramonabendias   (501) staff       (20)      148 2023-05-14 19:40:55.000000 experimenthq-0.0.0.dev3/src/experimenthq/__init__.py
--rw-r--r--   0 ramonabendias   (501) staff       (20)      129 2023-05-14 20:26:56.000000 experimenthq-0.0.0.dev3/src/experimenthq/_about.py
--rw-r--r--   0 ramonabendias   (501) staff       (20)     2192 2023-05-10 21:14:32.000000 experimenthq-0.0.0.dev3/src/experimenthq/experiment.py
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-14 20:27:11.905908 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3991 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/PKG-INFO
--rw-r--r--   0 ramonabendias   (501) staff       (20)      361 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/SOURCES.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/dependency_links.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-06 11:57:37.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/not-zip-safe
--rw-r--r--   0 ramonabendias   (501) staff       (20)      126 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/requires.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)       13 2023-05-14 20:27:11.000000 experimenthq-0.0.0.dev3/src/experimenthq.egg-info/top_level.txt
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.937007 experimenthq-0.0.0.dev4/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     1071 2023-04-28 20:27:57.000000 experimenthq-0.0.0.dev4/LICENSE
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3608 2023-05-17 00:15:12.937173 experimenthq-0.0.0.dev4/PKG-INFO
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     2383 2023-05-14 20:21:42.000000 experimenthq-0.0.0.dev4/README.md
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      983 2023-05-17 00:15:12.937657 experimenthq-0.0.0.dev4/setup.cfg
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3265 2023-05-17 00:15:07.000000 experimenthq-0.0.0.dev4/setup.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.933200 experimenthq-0.0.0.dev4/src/
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.934887 experimenthq-0.0.0.dev4/src/experimenthq/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      148 2023-05-14 19:40:55.000000 experimenthq-0.0.0.dev4/src/experimenthq/__init__.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      129 2023-05-17 00:14:26.000000 experimenthq-0.0.0.dev4/src/experimenthq/_about.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     2832 2023-05-17 00:13:36.000000 experimenthq-0.0.0.dev4/src/experimenthq/experiment.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.936358 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3608 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/PKG-INFO
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      386 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/SOURCES.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/dependency_links.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-06 11:57:37.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/not-zip-safe
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      126 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/requires.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)       13 2023-05-17 00:15:12.000000 experimenthq-0.0.0.dev4/src/experimenthq.egg-info/top_level.txt
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 00:15:12.936660 experimenthq-0.0.0.dev4/tests/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)       36 2023-05-15 17:54:05.000000 experimenthq-0.0.0.dev4/tests/test_experiment.py
```

### Comparing `experimenthq-0.0.0.dev3/LICENSE` & `experimenthq-0.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev3/PKG-INFO` & `experimenthq-0.0.0.dev4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: experimenthq
-Version: 0.0.0.dev3
+Version: 0.0.0.dev4
 Summary: A Python package for tracking experiments in Notion
-Home-page: https://github.com/EperimentHQ/experiment-hq
 Author: 
 Author-email: 
 License: MIT
-Project-URL: Changelog, https://github.com/EperimentHQ/experiment-hq/releases
-Project-URL: Issue Tracker, https://github.com/EperimentHQ/experiment-hq/issues
-Project-URL: Documentation, https://github.com/EperimentHQ/experiment-hq#documentation
-Project-URL: Source, https://github.com/EperimentHQ/experiment-hq
-Project-URL: Website, https://ml-notion-tracking-ui-vs3h.vercel.app/
+Project-URL: Website, https://www.experiment-hq.com/
 Keywords: notion,tracking,ml,machine learning,experiment,experimentation,experiment tracking,python,sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `experimenthq-0.0.0.dev3/README.md` & `experimenthq-0.0.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev3/setup.cfg` & `experimenthq-0.0.0.dev4/setup.cfg`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev3/setup.py` & `experimenthq-0.0.0.dev4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 
 from setuptools import find_packages, setup  # type: ignore
 
 # TODO: Update the package meta-data
 NAME = "experimenthq"
 MAIN_PACKAGE = "experimenthq"
 DESCRIPTION = "A Python package for tracking experiments in Notion"
-URL = "https://github.com/EperimentHQ/experiment-hq"
 EMAIL = ""
 AUTHOR = ""
 LICENSE = "MIT"
 REQUIRES_PYTHON = ">=3.7"
 VERSION = None  # Only set version if you like to overwrite the version in _about.py
-WEBSITE = "https://ml-notion-tracking-ui-vs3h.vercel.app/"
+WEBSITE = "https://www.experiment-hq.com/"
 
 
 PWD = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
@@ -38,15 +37,14 @@
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
-    url=URL,
     license=LICENSE,
     packages=find_packages(where="src", exclude=("tests", "test", "examples", "docs")),
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
     zip_safe=False,
     install_requires=["requests", "types-requests"],
     extras_require={
@@ -85,18 +83,14 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Utilities",
     ],
     project_urls={
-        "Changelog": URL + "/releases",
-        "Issue Tracker": URL + "/issues",
-        "Documentation": URL + "#documentation",
-        "Source": URL,
         "Website": WEBSITE,
     },
     # entry_points={"console_scripts": [f"{NAME}={MAIN_PACKAGE}._cli:cli"]},
     keywords=[
         "notion",
         "tracking",
         "ml",
```

### Comparing `experimenthq-0.0.0.dev3/src/experimenthq.egg-info/PKG-INFO` & `experimenthq-0.0.0.dev4/src/experimenthq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: experimenthq
-Version: 0.0.0.dev3
+Version: 0.0.0.dev4
 Summary: A Python package for tracking experiments in Notion
-Home-page: https://github.com/EperimentHQ/experiment-hq
 Author: 
 Author-email: 
 License: MIT
-Project-URL: Changelog, https://github.com/EperimentHQ/experiment-hq/releases
-Project-URL: Issue Tracker, https://github.com/EperimentHQ/experiment-hq/issues
-Project-URL: Documentation, https://github.com/EperimentHQ/experiment-hq#documentation
-Project-URL: Source, https://github.com/EperimentHQ/experiment-hq
-Project-URL: Website, https://ml-notion-tracking-ui-vs3h.vercel.app/
+Project-URL: Website, https://www.experiment-hq.com/
 Keywords: notion,tracking,ml,machine learning,experiment,experimentation,experiment tracking,python,sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

