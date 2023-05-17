# Comparing `tmp/wordcab-0.6.4.tar.gz` & `tmp/wordcab-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordcab-0.6.4.tar", max compression
+gzip compressed data, was "wordcab-0.6.5.tar", max compression
```

## Comparing `wordcab-0.6.4.tar` & `wordcab-0.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11361 2023-03-24 19:34:11.017753 wordcab-0.6.4/LICENSE
--rw-r--r--   0        0        0     5068 2023-03-24 19:34:11.017753 wordcab-0.6.4/README.md
--rw-r--r--   0        0        0     2081 2023-03-24 19:34:23.734017 wordcab-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     1260 2023-03-24 19:34:23.734017 wordcab-0.6.4/src/wordcab/__init__.py
--rw-r--r--   0        0        0     1159 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/__main__.py
--rw-r--r--   0        0        0    15203 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/api.py
--rw-r--r--   0        0        0    22551 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/client.py
--rw-r--r--   0        0        0     2574 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/config.py
--rw-r--r--   0        0        0     1570 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/core_objects/__init__.py
--rw-r--r--   0        0        0     3768 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/core_objects/job.py
--rw-r--r--   0        0        0    20882 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/core_objects/source.py
--rw-r--r--   0        0        0     2198 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/core_objects/stats.py
--rw-r--r--   0        0        0     6816 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/core_objects/summary.py
--rw-r--r--   0        0        0     2473 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/core_objects/transcript.py
--rw-r--r--   0        0        0     2990 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/core_objects/utils.py
--rw-r--r--   0        0        0     3863 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/login.py
--rw-r--r--   0        0        0        0 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/py.typed
--rw-r--r--   0        0        0     6165 2023-03-24 19:34:11.021753 wordcab-0.6.4/src/wordcab/utils.py
--rw-r--r--   0        0        0     6005 1970-01-01 00:00:00.000000 wordcab-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11361 2023-05-17 07:44:06.279698 wordcab-0.6.5/LICENSE
+-rw-r--r--   0        0        0     5070 2023-05-17 07:44:06.279698 wordcab-0.6.5/README.md
+-rw-r--r--   0        0        0     2081 2023-05-17 07:44:23.375701 wordcab-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1260 2023-05-17 07:44:23.375701 wordcab-0.6.5/src/wordcab/__init__.py
+-rw-r--r--   0        0        0     1159 2023-05-17 07:44:06.279698 wordcab-0.6.5/src/wordcab/__main__.py
+-rw-r--r--   0        0        0    15203 2023-05-17 07:44:06.279698 wordcab-0.6.5/src/wordcab/api.py
+-rw-r--r--   0        0        0    22551 2023-05-17 07:44:06.279698 wordcab-0.6.5/src/wordcab/client.py
+-rw-r--r--   0        0        0     2574 2023-05-17 07:44:06.279698 wordcab-0.6.5/src/wordcab/config.py
+-rw-r--r--   0        0        0     1570 2023-05-17 07:44:06.279698 wordcab-0.6.5/src/wordcab/core_objects/__init__.py
+-rw-r--r--   0        0        0     3839 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/core_objects/job.py
+-rw-r--r--   0        0        0    20882 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/core_objects/source.py
+-rw-r--r--   0        0        0     2198 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/core_objects/stats.py
+-rw-r--r--   0        0        0     6816 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/core_objects/summary.py
+-rw-r--r--   0        0        0     2473 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/core_objects/transcript.py
+-rw-r--r--   0        0        0     2990 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/core_objects/utils.py
+-rw-r--r--   0        0        0     3863 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/login.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/py.typed
+-rw-r--r--   0        0        0     6165 2023-05-17 07:44:06.283697 wordcab-0.6.5/src/wordcab/utils.py
+-rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 wordcab-0.6.5/PKG-INFO
```

### Comparing `wordcab-0.6.4/LICENSE` & `wordcab-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/README.md` & `wordcab-0.6.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 # Get the summary id
 summary_id = job.summary_details["summary_id"]
 # Retrieve the summary
 summary = retrieve_summary(summary_id=summary_id)
 
 # Get the summary as a human-readable string
-print(summary.get_formatted_summary())
+print(summary.get_formatted_summaries())
 
 # Save the json object to a file
 with open("wordcab_summary.json", "w") as f:
 	f.write(summary)
 ```
 
 # Documentation
```

#### html2text {}

```diff
@@ -38,15 +38,15 @@
 start_summary( source_object=source, display_name="sample_txt",
 summary_type="narrative", summary_lens=[1, 3], tags=["sample", "text"], ) #
 Wait for the job completion while True: job = retrieve_job
 (job_name=job.job_name) if job.job_status == "SummaryComplete": break else:
 time.sleep(3) # Get the summary id summary_id = job.summary_details
 ["summary_id"] # Retrieve the summary summary = retrieve_summary
 (summary_id=summary_id) # Get the summary as a human-readable string print
-(summary.get_formatted_summary()) # Save the json object to a file with open
+(summary.get_formatted_summaries()) # Save the json object to a file with open
 ("wordcab_summary.json", "w") as f: f.write(summary) ``` # Documentation Please
 see the [Documentation](https://wordcab-python.readthedocs.io/) for more
 details. # Contributing Contributions are very welcome. ð To learn more, see
 the [Contributor Guide]. # License - Distributed under the terms of the [!
 [Apache 2.0 License Badge](https://img.shields.io/badge/License-Apache%202.0-
 blue.svg)](https://opensource.org/licenses/Apache-2.0) - _Wordcab Python SDK_
 is free and open source software. # Issues If you encounter any problems,
```

### Comparing `wordcab-0.6.4/pyproject.toml` & `wordcab-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordcab"
-version = "0.6.4"
+version = "0.6.5"
 description = "Wordcab Python SDK"
 authors = ["Wordcab <info@wordcab.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Wordcab/wordcab-python"
 repository = "https://github.com/Wordcab/wordcab-python"
 documentation = "https://wordcab-python.readthedocs.io"
```

### Comparing `wordcab-0.6.4/src/wordcab/__init__.py` & `wordcab-0.6.5/src/wordcab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     "retrieve_job",
     "retrieve_summary",
     "retrieve_transcript",
     "start_extract",
     "start_summary",
 ]
 
-__version__ = "0.6.4"
+__version__ = "0.6.5"
```

### Comparing `wordcab-0.6.4/src/wordcab/__main__.py` & `wordcab-0.6.5/src/wordcab/__main__.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/api.py` & `wordcab-0.6.5/src/wordcab/api.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/client.py` & `wordcab-0.6.5/src/wordcab/client.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/config.py` & `wordcab-0.6.5/src/wordcab/config.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/core_objects/__init__.py` & `wordcab-0.6.5/src/wordcab/core_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/core_objects/job.py` & `wordcab-0.6.5/src/wordcab/core_objects/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     metadata: Optional[Dict[str, str]] = field(default=None)
     settings: Optional[JobSettings] = field(default=None)
     source_lang: Optional[str] = field(default=None)
     target_lang: Optional[str] = field(default=None)
     tags: Optional[List[str]] = field(default=None)
     time_started: Optional[str] = field(default=None)
     time_completed: Optional[str] = field(default=None)
+    transcript_details: Optional[Dict[str, str]] = field(default=None)
     transcript_id: Optional[str] = field(default=None)
 
     def __post_init__(self) -> None:
         """Post-init method."""
         logger.info(f"Job {self.job_name} created.")
         if self.source not in SOURCE_OBJECT_MAPPING.keys():
             raise ValueError(
```

### Comparing `wordcab-0.6.4/src/wordcab/core_objects/source.py` & `wordcab-0.6.5/src/wordcab/core_objects/source.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/core_objects/stats.py` & `wordcab-0.6.5/src/wordcab/core_objects/stats.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/core_objects/summary.py` & `wordcab-0.6.5/src/wordcab/core_objects/summary.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/core_objects/transcript.py` & `wordcab-0.6.5/src/wordcab/core_objects/transcript.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/core_objects/utils.py` & `wordcab-0.6.5/src/wordcab/core_objects/utils.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/login.py` & `wordcab-0.6.5/src/wordcab/login.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/src/wordcab/utils.py` & `wordcab-0.6.5/src/wordcab/utils.py`

 * *Files identical despite different names*

### Comparing `wordcab-0.6.4/PKG-INFO` & `wordcab-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordcab
-Version: 0.6.4
+Version: 0.6.5
 Summary: Wordcab Python SDK
 Home-page: https://github.com/Wordcab/wordcab-python
 License: Apache-2.0
 Author: Wordcab
 Author-email: info@wordcab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -123,15 +123,15 @@
 
 # Get the summary id
 summary_id = job.summary_details["summary_id"]
 # Retrieve the summary
 summary = retrieve_summary(summary_id=summary_id)
 
 # Get the summary as a human-readable string
-print(summary.get_formatted_summary())
+print(summary.get_formatted_summaries())
 
 # Save the json object to a file
 with open("wordcab_summary.json", "w") as f:
 	f.write(summary)
 ```
 
 # Documentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wordcab Version: 0.6.4 Summary: Wordcab Python SDK
+Metadata-Version: 2.1 Name: wordcab Version: 0.6.5 Summary: Wordcab Python SDK
 Home-page: https://github.com/Wordcab/wordcab-python License: Apache-2.0
 Author: Wordcab Author-email: info@wordcab.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
@@ -51,15 +51,15 @@
 start_summary( source_object=source, display_name="sample_txt",
 summary_type="narrative", summary_lens=[1, 3], tags=["sample", "text"], ) #
 Wait for the job completion while True: job = retrieve_job
 (job_name=job.job_name) if job.job_status == "SummaryComplete": break else:
 time.sleep(3) # Get the summary id summary_id = job.summary_details
 ["summary_id"] # Retrieve the summary summary = retrieve_summary
 (summary_id=summary_id) # Get the summary as a human-readable string print
-(summary.get_formatted_summary()) # Save the json object to a file with open
+(summary.get_formatted_summaries()) # Save the json object to a file with open
 ("wordcab_summary.json", "w") as f: f.write(summary) ``` # Documentation Please
 see the [Documentation](https://wordcab-python.readthedocs.io/) for more
 details. # Contributing Contributions are very welcome. ð To learn more, see
 the [Contributor Guide]. # License - Distributed under the terms of the [!
 [Apache 2.0 License Badge](https://img.shields.io/badge/License-Apache%202.0-
 blue.svg)](https://opensource.org/licenses/Apache-2.0) - _Wordcab Python SDK_
 is free and open source software. # Issues If you encounter any problems,
```

