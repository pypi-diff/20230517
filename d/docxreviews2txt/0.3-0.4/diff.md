# Comparing `tmp/docxreviews2txt-0.3.tar.gz` & `tmp/docxreviews2txt-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docxreviews2txt-0.3.tar", last modified: Wed May 17 21:09:00 2023, max compression
+gzip compressed data, was "docxreviews2txt-0.4.tar", last modified: Wed May 17 20:58:18 2023, max compression
```

## Comparing `docxreviews2txt-0.3.tar` & `docxreviews2txt-0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/
--rw-r--r--   0 alan      (1000) alan      (1000)     1853 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/PKG-INFO
--rw-r--r--   0 alan      (1000) alan      (1000)     1220 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/README.md
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 21:09:00.391589 docxreviews2txt-0.3/docxreviews2txt/
--rw-r--r--   0 alan      (1000) alan      (1000)       75 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/docxreviews2txt/__init__.py
--rw-r--r--   0 alan      (1000) alan      (1000)     6272 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/docxreviews2txt/docxreviews2txt.py
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/docxreviews2txt.egg-info/
--rw-r--r--   0 alan      (1000) alan      (1000)     1853 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/PKG-INFO
--rw-r--r--   0 alan      (1000) alan      (1000)      299 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/SOURCES.txt
--rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/dependency_links.txt
--rw-r--r--   0 alan      (1000) alan      (1000)       28 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/requires.txt
--rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/top_level.txt
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/scripts/
--rw-r--r--   0 alan      (1000) alan      (1000)      133 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/scripts/docxreviews2txt
--rw-r--r--   0 alan      (1000) alan      (1000)       38 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/setup.cfg
--rw-r--r--   0 alan      (1000) alan      (1000)      997 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/setup.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 20:58:18.761583 docxreviews2txt-0.4/
+-rw-r--r--   0 alan      (1000) alan      (1000)     2980 2023-05-17 20:58:18.761583 docxreviews2txt-0.4/PKG-INFO
+-rw-r--r--   0 alan      (1000) alan      (1000)     2360 2023-05-17 19:12:28.000000 docxreviews2txt-0.4/README.md
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 20:58:18.761583 docxreviews2txt-0.4/docxreviews2txt/
+-rw-r--r--   0 alan      (1000) alan      (1000)       97 2023-05-17 19:11:15.000000 docxreviews2txt-0.4/docxreviews2txt/__init__.py
+-rw-r--r--   0 alan      (1000) alan      (1000)      961 2023-05-17 19:14:40.000000 docxreviews2txt-0.4/docxreviews2txt/__main__.py
+-rw-r--r--   0 alan      (1000) alan      (1000)     5145 2023-05-17 19:11:25.000000 docxreviews2txt-0.4/docxreviews2txt/docxreviews2txt.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 20:58:18.761583 docxreviews2txt-0.4/docxreviews2txt.egg-info/
+-rw-r--r--   0 alan      (1000) alan      (1000)     2980 2023-05-17 20:58:18.000000 docxreviews2txt-0.4/docxreviews2txt.egg-info/PKG-INFO
+-rw-r--r--   0 alan      (1000) alan      (1000)      375 2023-05-17 20:58:18.000000 docxreviews2txt-0.4/docxreviews2txt.egg-info/SOURCES.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-05-17 20:58:18.000000 docxreviews2txt-0.4/docxreviews2txt.egg-info/dependency_links.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)       67 2023-05-17 20:58:18.000000 docxreviews2txt-0.4/docxreviews2txt.egg-info/entry_points.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)       21 2023-05-17 20:58:18.000000 docxreviews2txt-0.4/docxreviews2txt.egg-info/requires.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)       16 2023-05-17 20:58:18.000000 docxreviews2txt-0.4/docxreviews2txt.egg-info/top_level.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)       38 2023-05-17 20:58:18.761583 docxreviews2txt-0.4/setup.cfg
+-rw-r--r--   0 alan      (1000) alan      (1000)     1116 2023-05-17 20:50:49.000000 docxreviews2txt-0.4/setup.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 20:58:18.761583 docxreviews2txt-0.4/tests/
+-rw-r--r--   0 alan      (1000) alan      (1000)     1774 2023-04-01 16:57:18.000000 docxreviews2txt-0.4/tests/test_docxreviews2txt.py
```

### Comparing `docxreviews2txt-0.3/PKG-INFO` & `docxreviews2txt-0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,74 @@
-Metadata-Version: 2.1
-Name: docxreviews2txt
-Version: 0.3
-Summary: Extract reviews changes and commentaries from a docx file as plan text.
-Home-page: http://github.com/alanlivio/docxreviews2txt
-Author: Alan Guedes
-Author-email: alanlivio@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >= 3.6
-Description-Content-Type: text/markdown
-
-# docxreviews2txt
-
-Extract reviews changes and comments from a docx file as plan text.
-
-## How to install? 
-
-```bash
-pip install docxreviews2txt
-```
-
-## How to use?
-
-```txt
-$ docxreviews2txt -h
-usage: docxreviews2txt [-h] [--save_txt | --save_p_xml] docx
-
-positional arguments:
-  docx          input docx
-
-options:
-  -h, --help    show this help message and exit
-  --save_txt    save review as txt
-  --save_p_xml  save extracted paragraphs xml for debugging
-```
-  
-Example:
-
-```txt
-$ docxreviews2txt tests/lorem_ipsum.docx
-# comments
-- This is a comment from docx
-# Typos and rewriting suggestions
-- sit amet, consectetur  -> sit amet, consectetur Lorem ipsum
-- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
-- sit amet, consectetur adipiscing elit, sed -> sit amet, consectetur adipiscings elit, sed
-- enim ad minim veniam, quis nostrud -> enim ad minim do veniam, quis nostrud
-- enim ad minim veniam -> enim ad minim Lorem veniam
-- veniam, quis nostrud -> veniam ipsum, quis nostrud
-- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
-```
-
-## References
-
-- https://github.com/ankushshah89/python-docx2txt
-
+# docxreviews2txt
+
+Command line tool to extract review changes and comments from a docx file as plain text.
+It is particullary usefull after do review changes in pdf files at docx editor (e.g., MS Word, gdocs).
+
+## How to install?
+
+```bash
+pip install docxreviews2txt
+```
+
+## How to use it?
+
+```txt
+usage: docxreviews2txt [-h] [--save_p_xml] [--version] docx
+
+Extract review changes and comments from a docx file as plain text.
+
+positional arguments:
+  docx          input docx
+
+optional arguments:
+  -h, --help    show this help message and exit
+  --save_p_xml  also save extracted Docx paragraphs as xml for debugging
+  --version     show version
+```
+
+Example:
+
+```txt
+$ docxreviews2txt tests/lorem_ipsum.docx
+txt reviews at file:///C:/Users/alan/src/docxreviews2txt/tests/lorem_ipsum_review.txt
+```
+
+```txt
+$ cat c:/Users/alan/src/docxreviews2txt/tests/lorem_ipsum_review.txt
+# comments
+- This is a comment from docx
+# Typos and rewriting suggestions
+- sit amet, consectetur  -> sit amet, consectetur Lorem ipsum
+- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
+- sit amet, consectetur adipiscing elit, sed -> sit amet, consectetur adipiscings elit, sed
+- enim ad minim veniam, quis nostrud -> enim ad minim do veniam, quis nostrud
+- enim ad minim veniam -> enim ad minim Lorem veniam
+- veniam, quis nostrud -> veniam ipsum, quis nostrud
+- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
+```
+
+## TODO
+
+- [ ] improve N words extractions for reviews changes and enable pass it as a param
+- [ ] organized extracted reviews by the input Docx headings
+- [ ] save txt as Docx to enable editing
+- [ ] support drag-and-drop GUI
+
+## Known issues
+
+The tool fails to capture changes in Docx files with text organized in tables (e.g., pdf2docx converts columns to tables).
+
+## ChangeLog
+
+- v0.4: add __main__.py, rm --save_xml_p_elems, -nwords
+- v0.3: add --version
+- v0.2: add python module and unittests
+- v0.1: one-script intial version
+
+
+## References
+
+This project takes inspiration from:
+
+- https://github.com/ankushshah89/python-docx2txt
+- https://stackoverflow.com/questions/47390928/extract-docx-comments
+- https://stackoverflow.com/questions/38247251/how-to-extract-text-inserted-with-track-changes-in-python-docx
```

### Comparing `docxreviews2txt-0.3/setup.py` & `docxreviews2txt-0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import setuptools
 
 with open('requirements.txt') as f:
-    required = f.read().splitlines()
+  required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
-    long_description = fh.read()
+  long_description = fh.read()
 
 setuptools.setup(
     name="docxreviews2txt",
-    version="0.3",
+    packages=['docxreviews2txt'],
+    version="0.4",
     author="Alan Guedes",
     license='MIT',
     url="http://github.com/alanlivio/docxreviews2txt",
     python_requires='>= 3.6',
     install_requires=required,
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Environment :: Console",
         "Operating System :: Microsoft :: Windows",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3", ],
+        "Programming Language :: Python :: 3",
+    ],
     author_email="alanlivio@gmail.com",
-    description="Extract reviews changes and commentaries from a docx file as plan text.",
-    scripts=['scripts/docxreviews2txt'],
-)
+    description=
+    "Command line tool to extract review changes and comments from a docx file as plain text.",
+    entry_points={"console_scripts": [
+        "docxreviews2txt = docxreviews2txt.__main__:main",
+    ]})
```

