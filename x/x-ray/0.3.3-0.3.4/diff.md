# Comparing `tmp/x-ray-0.3.3.tar.gz` & `tmp/x_ray-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-ray-0.3.3.tar", max compression
+gzip compressed data, was "x_ray-0.3.4.tar", max compression
```

## Comparing `x-ray-0.3.3.tar` & `x_ray-0.3.4.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1326 2021-11-24 20:50:56.173469 x-ray-0.3.3/LICENSE
--rw-r--r--   0        0        0     5660 2021-11-24 20:50:56.173469 x-ray-0.3.3/README.md
--rw-r--r--   0        0        0     1846 2021-11-24 20:50:56.177470 x-ray-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1557 2021-11-24 20:50:56.209474 x-ray-0.3.3/xray/__init__.py
--rw-r--r--   0        0        0      159 2021-11-24 20:50:56.209474 x-ray-0.3.3/xray/__main__.py
--rw-r--r--   0        0        0      445 2021-11-24 20:50:56.209474 x-ray-0.3.3/xray/custom_types.py
--rw-r--r--   0        0        0    11584 2021-11-24 20:50:56.209474 x-ray-0.3.3/xray/pdf_utils.py
--rw-r--r--   0        0        0        0 2021-11-24 20:50:56.209474 x-ray-0.3.3/xray/py.typed
--rw-r--r--   0        0        0     1998 2021-11-24 20:50:56.209474 x-ray-0.3.3/xray/text_utils.py
--rw-r--r--   0        0        0     6739 2021-11-24 20:51:31.247809 x-ray-0.3.3/setup.py
--rw-r--r--   0        0        0     7138 2021-11-24 20:51:31.248498 x-ray-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1326 2023-05-17 16:36:50.020941 x_ray-0.3.4/LICENSE
+-rw-r--r--   0        0        0     5864 2023-05-17 16:36:50.020941 x_ray-0.3.4/README.md
+-rw-r--r--   0        0        0     2153 2023-05-17 16:36:50.020941 x_ray-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1557 2023-05-17 16:36:50.056942 x_ray-0.3.4/xray/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-17 16:36:50.056942 x_ray-0.3.4/xray/__main__.py
+-rw-r--r--   0        0        0      445 2023-05-17 16:36:50.056942 x_ray-0.3.4/xray/custom_types.py
+-rw-r--r--   0        0        0    11584 2023-05-17 16:36:50.056942 x_ray-0.3.4/xray/pdf_utils.py
+-rw-r--r--   0        0        0        0 2023-05-17 16:36:50.056942 x_ray-0.3.4/xray/py.typed
+-rw-r--r--   0        0        0     1998 2023-05-17 16:36:50.056942 x_ray-0.3.4/xray/text_utils.py
+-rw-r--r--   0        0        0     7820 1970-01-01 00:00:00.000000 x_ray-0.3.4/PKG-INFO
```

### Comparing `x-ray-0.3.3/LICENSE` & `x_ray-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `x-ray-0.3.3/README.md` & `x_ray-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,23 +53,23 @@
       ],
       "text": "The Ring travels by way of Cirith Ungol"
     }
   ]
 }
 ```
 
-Or if you have hte file on a server somewhere, give it a URL. If it starts
+Or if you have the file on a server somewhere, give it a URL. If it starts
 with `https://`, it will be interpreted as a PDF to download:
 
 ```bash
 % xray https://free.law/pdf/congressional-testimony-michael-lissner-free-law-project-hearing-on-ethics-and-transparency-2021-10-26.pdf
 {}
 ```
 
-A fun trick you can now do is to make a file with one URL per line, call it `urls.txt`. Then you can run this to check each URL:
+A fun trick you can do is to make a file with one URL per line, call it `urls.txt`. Then you can run this to check each URL:
 
 ```bash
 xargs -n 1 xray  < urls.txt
 ```
 
 However you run `xray` on the command line, you'll get JSON as output. When you have that, you can use it with tools like [`jq`][jq]. The format is as follows:
 
@@ -81,15 +81,15 @@
  - The second key is `text`. This is the text under the bad rectangle.
 
 Simple enough.
 
 You can also use it as a Python module, if you prefer the long-form:
 
 ```
-% pathon -m xray some-file.pdf
+% python -m xray some-file.pdf
 ```
 
 But that's not as easy to remember.
 
 If you want a bit more, you can, of course, use `xray` in Python:
 
 ```python
@@ -140,29 +140,36 @@
 
 You can read the source to see how it works, but the general idea is to:
 
 1. Find rectangles in a PDF.
 
 2. Find letters in the same location
 
-3. Render the rectangle
+3. Render the rectangle as an image
 
-4. Inspect the rectangle to see if it's all one color
+4. Inspect the rectangle to see if it's all one color. If it is, then that's a
+   bad redaction. If not, then we assume you can see a mix of text and
+   drawings, indicating a redaction that's OK.
+
+The PDF format is a big and complicated one, so it's difficult to do all this perfectly. We do our best, but there's always more to do to make it better. [Donations][d] and sponsored work help.
+
+[d]: https://free.law/donate/
 
-The PDF format is a big and complicated one, so it's difficult to do all this l and perfectly. We do our best, but there's always more to do to make it better. Donations and sponsored work help.
 
 ## Contributions
 
 Please see the issues list on Github for things we need, or start a conversation if you have questions. Before you do your first contribution, we'll need a signed contributor license agreement. See the template in the repo.
 
 
 ## Deployment
 
 Releases happen automatically via Github Actions. To trigger an automated build:
 
+0. Update CHANGES.md
+
 1. Update the version in pyproject.toml
 
 2. Tag the commit with something like "v0.0.0".
 
 
 If you wish to create a new version manually, the process is:
```

### Comparing `x-ray-0.3.3/pyproject.toml` & `x_ray-0.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -20,38 +20,43 @@
 license = "BSD-2-Clause"
 maintainers = ["Free Law Project <info@free.law>"]
 name = "x-ray"
 packages = [
     {include = "xray"}
 ]
 readme = "README.md"
-repository = "https://github.com/freelawproject/pdf-redaction-detector"
-version = "0.3.3"
+homepage = "https://free.law/projects/x-ray"
+repository = "https://github.com/freelawproject/x-ray"
+documentation = "https://github.com/freelawproject/x-ray/blob/main/README.md"
+version = "0.3.4"
 
 [tool.poetry.scripts]
 xray = "xray.__init__:cli"
 
 [tool.poetry.urls]
 "Organisation Homepage" = "https://free.law/"
+"Change Log" = "https://github.com/freelawproject/x-ray/blob/main/CHANGES.md"
+Issues = "https://github.com/freelawproject/x-ray/issues"
+Funding = "https://www.courtlistener.com/donate/?referrer=pypi-xray"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-PyMuPDF = "1.19.2"
+PyMuPDF = "1.22.2"
 requests = "^2.26.0"
 types-requests = "^2.26.0"
 
 [tool.poetry.dev-dependencies]
-black = "^21.11b1"
-isort = "^5.10.0"
+black = "^23.1"
+isort = "^5.12.0"
 mypy = "^0.910"
 pylint = "^2.7.1"
-wheel = "^0.35.1"
+wheel = "^0.38.2"
 flynt = "^0.69"
-pre-commit = "^2.15.0"
-ipython = "^7.29.0"
+pre-commit = "^3.2.2"
+ipython = "^8.12.0"
 
 [tool.black]
 include = '''.*\.pyi?$'''
 line-length = 79
 
 [tool.isort]
 force_grid_wrap = 0
```

### Comparing `x-ray-0.3.3/xray/__init__.py` & `x_ray-0.3.4/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `x-ray-0.3.3/xray/pdf_utils.py` & `x_ray-0.3.4/xray/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `x-ray-0.3.3/xray/text_utils.py` & `x_ray-0.3.4/xray/text_utils.py`

 * *Files identical despite different names*

### Comparing `x-ray-0.3.3/PKG-INFO` & `x_ray-0.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: x-ray
-Version: 0.3.3
+Version: 0.3.4
 Summary: A library and microservice to find bad redactions in PDFs
-Home-page: https://github.com/freelawproject/pdf-redaction-detector
+Home-page: https://free.law/projects/x-ray
 License: BSD-2-Clause
 Keywords: legal,courts,redactions
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: PyMuPDF (==1.19.2)
+Requires-Dist: PyMuPDF (==1.22.2)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: types-requests (>=2.26.0,<3.0.0)
+Project-URL: Change Log, https://github.com/freelawproject/x-ray/blob/main/CHANGES.md
+Project-URL: Documentation, https://github.com/freelawproject/x-ray/blob/main/README.md
+Project-URL: Funding, https://www.courtlistener.com/donate/?referrer=pypi-xray
+Project-URL: Issues, https://github.com/freelawproject/x-ray/issues
 Project-URL: Organisation Homepage, https://free.law/
-Project-URL: Repository, https://github.com/freelawproject/pdf-redaction-detector
+Project-URL: Repository, https://github.com/freelawproject/x-ray
 Description-Content-Type: text/markdown
 
 ![Image of REDACTED STAMP](https://raw.githubusercontent.com/freelawproject/x-ray/main/redacted.png)
 
 x-ray is a Python library for finding bad redactions in PDF documents.
 
 ## Why?
@@ -87,23 +95,23 @@
       ],
       "text": "The Ring travels by way of Cirith Ungol"
     }
   ]
 }
 ```
 
-Or if you have hte file on a server somewhere, give it a URL. If it starts
+Or if you have the file on a server somewhere, give it a URL. If it starts
 with `https://`, it will be interpreted as a PDF to download:
 
 ```bash
 % xray https://free.law/pdf/congressional-testimony-michael-lissner-free-law-project-hearing-on-ethics-and-transparency-2021-10-26.pdf
 {}
 ```
 
-A fun trick you can now do is to make a file with one URL per line, call it `urls.txt`. Then you can run this to check each URL:
+A fun trick you can do is to make a file with one URL per line, call it `urls.txt`. Then you can run this to check each URL:
 
 ```bash
 xargs -n 1 xray  < urls.txt
 ```
 
 However you run `xray` on the command line, you'll get JSON as output. When you have that, you can use it with tools like [`jq`][jq]. The format is as follows:
 
@@ -115,15 +123,15 @@
  - The second key is `text`. This is the text under the bad rectangle.
 
 Simple enough.
 
 You can also use it as a Python module, if you prefer the long-form:
 
 ```
-% pathon -m xray some-file.pdf
+% python -m xray some-file.pdf
 ```
 
 But that's not as easy to remember.
 
 If you want a bit more, you can, of course, use `xray` in Python:
 
 ```python
@@ -174,29 +182,36 @@
 
 You can read the source to see how it works, but the general idea is to:
 
 1. Find rectangles in a PDF.
 
 2. Find letters in the same location
 
-3. Render the rectangle
+3. Render the rectangle as an image
 
-4. Inspect the rectangle to see if it's all one color
+4. Inspect the rectangle to see if it's all one color. If it is, then that's a
+   bad redaction. If not, then we assume you can see a mix of text and
+   drawings, indicating a redaction that's OK.
+
+The PDF format is a big and complicated one, so it's difficult to do all this perfectly. We do our best, but there's always more to do to make it better. [Donations][d] and sponsored work help.
+
+[d]: https://free.law/donate/
 
-The PDF format is a big and complicated one, so it's difficult to do all this l and perfectly. We do our best, but there's always more to do to make it better. Donations and sponsored work help.
 
 ## Contributions
 
 Please see the issues list on Github for things we need, or start a conversation if you have questions. Before you do your first contribution, we'll need a signed contributor license agreement. See the template in the repo.
 
 
 ## Deployment
 
 Releases happen automatically via Github Actions. To trigger an automated build:
 
+0. Update CHANGES.md
+
 1. Update the version in pyproject.toml
 
 2. Tag the commit with something like "v0.0.0".
 
 
 If you wish to create a new version manually, the process is:
```

