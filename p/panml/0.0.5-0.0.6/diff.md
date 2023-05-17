# Comparing `tmp/panml-0.0.5.tar.gz` & `tmp/panml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.5.tar", last modified: Wed May 17 07:22:52 2023, max compression
+gzip compressed data, was "panml-0.0.6.tar", last modified: Wed May 17 07:39:53 2023, max compression
```

## Comparing `panml-0.0.5.tar` & `panml-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 07:22:52.848962 panml-0.0.5/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1501 2023-05-17 07:22:52.849086 panml-0.0.5/PKG-INFO
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 07:22:52.848912 panml-0.0.5/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.5/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    22590 2023-05-16 08:12:47.827759 panml-0.0.5/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     7024 2023-05-16 08:12:47.828416 panml-0.0.5/panml/search.py
--rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.5/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     3304 2023-05-17 07:22:12.706012 panml-0.0.5/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 07:39:53.900674 panml-0.0.6/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1501 2023-05-17 07:39:53.900816 panml-0.0.6/PKG-INFO
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 07:39:53.900610 panml-0.0.6/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.6/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    22590 2023-05-16 08:12:47.827759 panml-0.0.6/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     7024 2023-05-16 08:12:47.828416 panml-0.0.6/panml/search.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.6/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2404 2023-05-17 07:39:39.875818 panml-0.0.6/setup.py
```

### Comparing `panml-0.0.5/PKG-INFO` & `panml-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: panml
-Version: 0.0.5
+Version: 0.0.6
 Summary: PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: williamxn.z@gmail.com
 License: MIT
-Download-URL: https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.6.tar.gz
 Description: PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers.                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others.                       
         
         Quick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide                       
         
         Documentation/Wiki: https://github.com/Pan-ML/panml/wiki
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.5/panml/models.py` & `panml-0.0.6/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.5/panml/search.py` & `panml-0.0.6/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.5/setup.py` & `panml-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,35 @@
 
 from distutils.core import setup
 setup(
   name = 'panml', # package name     
   packages = ['panml'], # package name
-  version = '0.0.5', # version
+  version = '0.0.6', # version
   license = 'MIT', # license
   description = 'PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.', # short description about the package
   long_description = 'PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. \
                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others. \
                       \n\nQuick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide \
                       \n\nDocumentation/Wiki: https://github.com/Pan-ML/panml/wiki', # long description
   author = 'PanML team', # team name
   author_email = 'williamxn.z@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
-  download_url = 'https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.3.tar.gz', # set a release on GitHub (with release tag) -> Assets -> right click and copy the link
+  download_url = 'https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.6.tar.gz', # set a release on GitHub (with release tag) -> Assets -> right click and copy the link
   keywords = ['generative AI', 'generative model', 'machine learning', 'large language model', # keywords
               'LLM', 'prompt engineering', 'fine tuning', 'prompt tuning', 'retrieval augmentation', 
               'AI safety', 'AI alignment'], 
   install_requires=[  # dependencies
-        'aiohttp>=3.8.4',
-        'aiosignal>=1.3.1',
-        'async-timeout>=4.0.2',
-        'attrs>=23.1.0',
-        'certifi>=2023.5.7',
-        'charset-normalizer>=3.1.0',
-        'datasets>=2.12.0',
-        'dill>=0.3.6',
-        'filelock>=3.12.0',
-        'frozenlist>=1.3.3',
-        'fsspec>=2023.5.0',
         'huggingface-hub>=0.14.1',
-        'idna>=3.4',
-        'Jinja2>=3.1.2',
-        'MarkupSafe>=2.1.2',
-        'mpmath>=1.3.0',
-        'multidict>=6.0.4',
-        'multiprocess>=0.70.14',
-        'networkx>=3.1',
         'numpy>=1.24.3',
         'openai>=0.27.6',
-        'packaging>=23.1',
         'pandas>=2.0.1',
-        'pyarrow>=12.0.0',
-        'python-dateutil>=2.8.2',
-        'pytz>=2023.3',
-        'PyYAML>=6.0',
-        'regex>=2023.5.5',
-        'requests>=2.30.0',
-        'responses>=0.18.0',
-        'six>=1.16.0',
-        'sympy>=1.12',
         'tokenizers>=0.13.3',
         'torch>=2.0.1',
         'tqdm>=4.65.0',
         'transformers>=4.29.1',
-        'typing_extensions>=4.5.0',
-        'tzdata>=2023.3',
-        'urllib3>=2.0.2',
-        'xxhash>=3.2.0',
-        'yarl>=1.9.2',
         'faiss-cpu>=1.7.4',
         'faiss-gpu>=1.7.2',
         'sentence-transformers>=2.2.2',
       ],
   classifiers=[
     'Development Status :: 4 - Beta', # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of the package
     'Intended Audience :: Developers', # Define the audience type
```

