# Comparing `tmp/nobubo-1.4.1.tar.gz` & `tmp/nobubo-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobubo-1.4.1.tar", last modified: Wed Oct 13 06:25:08 2021, max compression
+gzip compressed data, was "nobubo-1.5.0.tar", max compression
```

## Comparing `nobubo-1.4.1.tar` & `nobubo-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    34523 2019-09-06 15:24:29.018640 nobubo-1.4.1/LICENSE
--rw-r--r--   0        0        0     7093 2021-07-23 15:09:15.118002 nobubo-1.4.1/README.md
--rw-r--r--   0        0        0       17 2019-11-25 15:23:24.469112 nobubo-1.4.1/nobubo/.gitignore
--rw-r--r--   0        0        0        0 2020-10-05 08:52:36.733374 nobubo-1.4.1/nobubo/__init__.py
--rw-r--r--   0        0        0      307 2021-07-15 14:00:50.991304 nobubo-1.4.1/nobubo/__main__.py
--rw-r--r--   0        0        0     6531 2021-07-23 15:09:15.118002 nobubo-1.4.1/nobubo/assembly.py
--rw-r--r--   0        0        0     4589 2021-07-23 15:09:15.118002 nobubo-1.4.1/nobubo/cli.py
--rw-r--r--   0        0        0     9899 2021-07-23 15:09:15.118002 nobubo-1.4.1/nobubo/disassembly.py
--rw-r--r--   0        0        0      871 2021-01-20 12:20:25.252747 nobubo-1.4.1/nobubo/errors.py
--rw-r--r--   0        0        0     4145 2021-07-23 15:09:15.122002 nobubo-1.4.1/nobubo/init_nobubo.py
--rw-r--r--   0        0        0     2399 2021-10-13 06:21:10.684384 nobubo-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8086 2021-10-13 06:25:08.876684 nobubo-1.4.1/setup.py
--rw-r--r--   0        0        0     8000 2021-10-13 06:25:08.877166 nobubo-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2019-09-06 15:24:29.018640 nobubo-1.5.0/LICENSE
+-rw-r--r--   0        0        0     7513 2023-05-17 09:37:51.786894 nobubo-1.5.0/README.md
+-rw-r--r--   0        0        0     2679 2023-05-17 09:35:59.742351 nobubo-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       17 2023-05-17 09:35:59.742351 nobubo-1.5.0/src/nobubo/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-17 09:35:59.742351 nobubo-1.5.0/src/nobubo/__init__.py
+-rw-r--r--   0        0        0      307 2023-05-17 09:35:59.742351 nobubo-1.5.0/src/nobubo/__main__.py
+-rw-r--r--   0        0        0     6531 2023-05-17 09:35:59.742351 nobubo-1.5.0/src/nobubo/assembly.py
+-rw-r--r--   0        0        0     4589 2023-05-17 09:35:59.742351 nobubo-1.5.0/src/nobubo/cli.py
+-rw-r--r--   0        0        0     9871 2023-05-17 09:35:59.742351 nobubo-1.5.0/src/nobubo/disassembly.py
+-rw-r--r--   0        0        0      871 2023-05-17 09:35:59.742351 nobubo-1.5.0/src/nobubo/errors.py
+-rw-r--r--   0        0        0     4499 2023-05-17 09:35:59.742351 nobubo-1.5.0/src/nobubo/init_nobubo.py
+-rw-r--r--   0        0        0     8422 1970-01-01 00:00:00.000000 nobubo-1.5.0/PKG-INFO
```

### Comparing `nobubo-1.4.1/LICENSE` & `nobubo-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nobubo-1.4.1/README.md` & `nobubo-1.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # Nobubo
+
+Nobubo creates a collage from digital pattern pages and then chops it up into a 
+desired output layout. The collage is assembled according to one or several
+overview sheets. These overviews are usually provided along with the pattern
+pages in the same pdf or in the instructions pdf.
+<div align="center">
+<img src="img/nobubo-logo-dalle-nightcafe-small.png" alt="nobubo logo, nightcafe/dall-e2" width=50%/>
+</div>
+
+# About 
+
 Digital sewing patterns are very handy: No shipping costs and cheaper than physical patterns. There is one drawback: Many digital patterns are distributed in A4 size, and it is up to the sewist to assemble them.
 
-A jacket pattern has around 50 A4 pages that must be glued or taped together. This usually results in an apartment covered in A4 pages and a final collage in which printer irregularities lead to ill-matching pattern lines. Many indie pattern companies already sell their digital patterns as A4 and A0 in the same pattern purchase, but there are still other companies that only provide A4.
+A dress pattern has around 70 A4 pages that must be glued or taped together. This usually results in an apartment covered in A4 pages and a final collage in which small irregularities lead to ill-matching pattern lines. Many indie pattern companies already sell their digital patterns as A4 and A0 in the same pattern purchase, but there are still other companies that only provide A4.
 
 That's why I wrote nobubo: This tool assembles the pages of a digital pdf pattern and chops it into a desired output size, so that you can print it on any page size you want. 
 
-Nobubo has been developed and tested with several download patterns from Burda, Knipmode and other brands successfully. Even though nobubo has been developed with sewing patterns in mind, it is basically a fancy n-up tool for PDFs in general.
+Nobubo has been developed and tested with several download patterns from Burda, Knipmode and other brands successfully. Even though nobubo has been developed with sewing patterns in mind, it is basically a fancy n-up tool for pdfs in general.
 
 ## Prerequisites
 * A digital pattern where each page is made to be printed on A4 or US letter size. **If you haven't purchased a digital pattern, nobubo is useless**.
 * Each page is already cropped, so that only the bare pattern is visible (no white borders around the pattern). Nobubo is able to handle cropped pdfs, but you still have to do it yourself.
-* Usually, the assembled pattern pages form a huge rectangle. Some brands provide a handy overview how all the assembled pages are supposed to look like. Some brands, however, disregard this rectangle shape and the assembled pattern is of a weird "rectangle + n pages" shape. Nobubo can only handle rectangle shapes, so those leftover pages have to be print out and taped by hand.
-* Python >=3.8
+* Usually, the assembled pattern pages form a huge rectangle. Some brands provide a handy overview how all the assembled pages are supposed to look like. Some brands, however, disregard this rectangle shape and the assembled pattern is of a weird "rectangle + n pages" shape. Nobubo can only handle rectangle shapes, so those leftover pages have to be printed out and taped by hand.
+* Python >=3.10
 * `pdflatex` [must be installed](https://tex.stackexchange.com/questions/49569/where-to-download-pdflatex-exe)
 
 ## Installation
 
 ### Using pip
 
 1. [Create a virtual environment](https://docs.python-guide.org/dev/virtualenvs/#lower-level-virtualenv) 
@@ -102,14 +113,14 @@
 This prints only two pdfs (=2 overview sheets) which contain each a huge collage.
 
 ## Caveats
 * Please double-check and compare the overview sheet with the amount of pdf pages given (rows * columns = amount of pages needed).  If the result is wrong, check if you counted the rows and columns correctly or if a second overview sheet hides in later pages. Burda for example includes several overview sheets and their corresponding pages in one pdf.
 * Check if the pattern must be assembled from top left to bottom right (default) or bottom left to top right (use `--reverse` flag)
 * When you print the final pattern pages,  double-check and measure the control square. Don't forget to print 100% "as is", with any scaling or page fitting off.
 
-**I do not take any responsibility if nobubo leads to ill-matching garments or any other problems whatsoever. You use this tool at your own risk. If in doubt, make a backup of your original pattern pdf. Please have a look at the license if you want to improve the tool yourself.**
+**I do not take any responsibility if nobubo leads to ill-matching garments or any other problems whatsoever. You use this tool at your own risk. Always make a backup of your original pattern pdf. Please have a look at the license if you want to improve the tool yourself.**
 
 ## Thanks
 
 [The_Compiler](https://github.com/The-Compiler) for their invaluable feedback and encouragement.
 
-I was stuck on how to use pikepdf properly, [cfcurtis' sewingutils](https://github.com/cfcurtis/sewingutils) provided an answer.
+I was stuck on how to use pikepdf properly, [cfcurtis' pdfstitcher](https://github.com/cfcurtis/pdfstitcher) provided an answer.
```

### Comparing `nobubo-1.4.1/nobubo/assembly.py` & `nobubo-1.5.0/src/nobubo/assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021, Méline Sieber
+# Copyright 2023, Méline Sieber
 #
 # This file is part of Nobubo.
 #
 # Nobubo is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `nobubo-1.4.1/nobubo/cli.py` & `nobubo-1.5.0/src/nobubo/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021, Méline Sieber
+# Copyright 2023, Méline Sieber
 #
 # This file is part of Nobubo.
 #
 # Nobubo is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `nobubo-1.4.1/nobubo/disassembly.py` & `nobubo-1.5.0/src/nobubo/disassembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021, Méline Sieber
+# Copyright 2023, Méline Sieber
 #
 # This file is part of Nobubo.
 #
 # Nobubo is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -17,23 +17,22 @@
 
 """
 Contains functions for various output layouts.
 """
 import logging
 import math
 import pathlib
+from copy import copy
 from dataclasses import dataclass
 from typing import List, Tuple, Optional
 
 import pikepdf
 
-import nobubo.assembly
 from nobubo import errors
-from nobubo.assembly import Layout, PageSize
-
+from nobubo import assembly
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Point:
     """
@@ -56,15 +55,17 @@
 
 class NobuboOutput:
     """
     Holds all information of the output pdf and is responsible for creating
     the desired output pdf.
     """
 
-    def __init__(self, output_path: pathlib.Path, output_pagesize: Optional[PageSize]):
+    def __init__(
+        self, output_path: pathlib.Path, output_pagesize: Optional[assembly.PageSize]
+    ):
         """
         :param output_path: path where the output pdf should be saved.
         :param output_pagesize: The desired page size in user space units (can include
         user-defined print margin).
         """
         self.output_path = output_path
         self.output_pagesize = output_pagesize
@@ -75,15 +76,15 @@
             f"output_path: '{self.output_path}', "
             f"output_pagesize: '{self.output_pagesize}'>"
         )
 
     def create_output_files(
         self,
         temp_collage_paths: List[pathlib.Path],
-        input_properties: nobubo.assembly.NobuboInput,
+        input_properties: assembly.NobuboInput,
     ) -> None:
         for counter, collage_path in enumerate(temp_collage_paths):
             try:
                 collage = pikepdf.Pdf.open(collage_path)
             except OSError as e:
                 raise errors.UsageError(
                     "Could not open collage file for disassembly:" f"\n{e}."
@@ -122,16 +123,16 @@
                     f"An error occurred " f"while writing the collage:\n{e}"
                 )
             logger.info(f"Collage written to {new_outputpath}.")
 
     def _create_output_files(
         self,
         collage: pikepdf.Pdf,
-        input_pagesize: nobubo.assembly.PageSize,
-        current_layout: nobubo.assembly.Layout,
+        input_pagesize: assembly.PageSize,
+        current_layout: assembly.Layout,
     ) -> pikepdf.Pdf:
         """
         Chops up the collage that consists of all the pattern pages to individual pages
         of the desired output size.
         :param collage: One pdf page that contains all assembled pattern pages.
         :param input_pagesize: size of an input pdf page
         :param current_layout: the current layout of the input pdf
@@ -141,20 +142,21 @@
         assert self.output_pagesize is not None
         n_up_factor = self.nup_factors(input_pagesize, self.output_pagesize)
         # only two points are needed to be cropped,
         # lower left (x, y) and upper right (x, y)
         lowerleft_factor = Factor(x=0, y=0)
         upperright_factor = Factor(x=1, y=1)
 
-        output = pikepdf.Pdf.new()
-        output.copy_foreign(collage.Root)
-        # Root must be copied too, not only the page:
-        # thanks to https://github.com/cfcurtis/sewingutils
+        output = pikepdf.new()
+        # pdfstitcher made me aware of pikepdf and provided some hints
+        # on how to use it, thanks!
+        # https://github.com/cfcurtis/pdfstitcher
+
         for i in range(0, self.pages_needed(current_layout, n_up_factor)):
-            page = output.copy_foreign(collage.pages[0])
+            page = copy(collage.pages[0])
 
             lowerleft: Point = _calculate_lowerleft_point(
                 lowerleft_factor, n_up_factor, input_pagesize
             )
             upperright: Point = _calculate_upperright_point(
                 upperright_factor, n_up_factor, current_layout, input_pagesize
             )
@@ -168,27 +170,27 @@
             )
 
             page.CropBox = [lowerleft.x, lowerleft.y, upperright.x, upperright.y]
             output.pages.append(page)
 
         return output
 
-    def pages_needed(self, layout: Layout, n_up_factor: Factor) -> int:
+    def pages_needed(self, layout: assembly.Layout, n_up_factor: Factor) -> int:
         """
         Calculate the pages needed for the required output layout.
         :param layout: layout of the input pdf
         :param n_up_factor: how many pages of the input pdf fit on the desired layout
         :return:
         """
         x = layout.columns / n_up_factor.x
         y = layout.rows / n_up_factor.y
         return math.ceil(x) * math.ceil(y)
 
     def nup_factors(
-        self, input_pagesize: PageSize, output_pagesize: PageSize
+        self, input_pagesize: assembly.PageSize, output_pagesize: assembly.PageSize
     ) -> Factor:
         """
         Calculate the n-up factor for the output pdf, i.e. how many input pages
         fit on the desired output layout.
         :param input_pagesize: Size of a page of the input pdf in user space units
         :param output_pagesize: the output layout in user space units
         :return:
@@ -205,27 +207,27 @@
 
 
 def _calculate_colsrows_left(layout_element: int, factor: int, nup_factor: int) -> int:
     return layout_element - (factor * nup_factor)
 
 
 def _calculate_lowerleft_point(
-    lowerleft_factor: Factor, n_up_factor: Factor, pagesize: nobubo.assembly.PageSize
+    lowerleft_factor: Factor, n_up_factor: Factor, pagesize: assembly.PageSize
 ) -> Point:
     return Point(
         x=lowerleft_factor.x * n_up_factor.x * pagesize.width,
         y=lowerleft_factor.y * n_up_factor.y * pagesize.height,
     )
 
 
 def _calculate_upperright_point(
     upperright_factor: Factor,
     n_up_factor: Factor,
-    current_layout: nobubo.assembly.Layout,
-    pagesize: nobubo.assembly.PageSize,
+    current_layout: assembly.Layout,
+    pagesize: assembly.PageSize,
 ) -> Point:
     upperright = Point(x=0, y=0)
     # Manage ROWS: apply transformation to upper right, y-value
     rowsleft = _calculate_colsrows_left(
         current_layout.rows, upperright_factor.y, n_up_factor.y
     )
     if rowsleft < 0:  # end of pattern reached  (full amount of rows reached)
```

### Comparing `nobubo-1.4.1/nobubo/errors.py` & `nobubo-1.5.0/src/nobubo/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021, Méline Sieber
+# Copyright 2023, Méline Sieber
 #
 # This file is part of Nobubo.
 #
 # Nobubo is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `nobubo-1.4.1/nobubo/init_nobubo.py` & `nobubo-1.5.0/src/nobubo/init_nobubo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import pathlib
 import re
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 
 import pikepdf
 
 from nobubo import errors
 from nobubo.assembly import NobuboInput, PageSize, Layout
 from nobubo.disassembly import NobuboOutput
 
@@ -60,15 +60,17 @@
         if output_layout_cli
         else None,
     )
     logger.debug(f"Parsed output properties: {output_properties}")
     return output_properties
 
 
-def parse_output_layout(output_layout_cli: str, print_margin: int = None) -> PageSize:
+def parse_output_layout(
+    output_layout_cli: str, print_margin: Optional[int] = None
+) -> PageSize:
     print_size: List[int] = []
     if output_layout_cli == "a0":
         print_size = to_mm("841x1189")
     if output_layout_cli == "us":  # Arch E /Arch 6 size of 36 × 48 inches
         print_size = to_mm("914x1220")
     elif "x" in output_layout_cli:
         print_size = to_mm(output_layout_cli)
@@ -80,26 +82,31 @@
 
 
 def page_dimensions(page: pikepdf.Page) -> Tuple[float, float]:
     """
     Calculate the x, y value for the offset in default user space units
     as defined in the pdf standard.
     :param page: A PDF page.
-    :return: list with x, y value.
+    :return: tuple with x, y value.
     """
-    if not hasattr(page, "CropBox"):
-        # page is of type Object, and either MediaBox, CropBox or TrimBox
+    if not hasattr(page, "cropbox"):
+        # page is of type Object, and either mediabox, cropbox or trimbox
         # are all of type pikepdf.objects.Object
         # they exist (or not) depending on the pdf itself
-        box = page.MediaBox  # type: ignore
+        box: pikepdf.objects.Array = page.mediabox
     else:
-        box = page.CropBox  # type: ignore
-    return round(float(box[2]) - float(box[0]), 2), round(
-        float(box[3]) - float(box[1]), 2
-    )
+        box = page.cropbox
+    # pikepdf has some confusing types here
+    # type(box[2]) returns decimal.Decimal, but mypy/pikepdf insists it's of type Object
+    # the workaround is to convert it to a string,
+    # then to a float to calculate the offset
+    # since both Decimal and Object allow the stringification
+    width = float(str(box[2])) - float(str(box[0]))
+    height = float(str(box[3])) - float(str(box[1]))
+    return round(width, 2), round(height, 2)
 
 
 def to_mm(output_layout: str) -> List[int]:
     ol_in_mm = re.compile(r"\d+[x]\d+").findall(output_layout)[0].split("x")
     return [int(x) for x in ol_in_mm]
```

### Comparing `nobubo-1.4.1/pyproject.toml` & `nobubo-1.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 [tool.poetry]
 name = "nobubo"
-version = "1.4.1"
+version = "1.5.0"
 description = "Nobubo assembles a digital pdf sewing pattern and cuts it up into a desired output print size. A specialized n-up tool also suited for non-sewing purposes."
 authors = ["bytinbit"]
 license = "AGPL v3.0"
 readme = "README.md"
 homepage = "https://github.com/bytinbit/nobubo"
 repository = "https://github.com/bytinbit/nobubo"
 classifiers =  [
         "Topic :: Printing",
         "Topic :: Utilities",
         "Topic :: Multimedia :: Graphics :: Graphics Conversion",
         "License :: OSI Approved :: GNU Affero General Public License v3",
     ]
-
+packages = [
+	{ include = "nobubo", from = "src"},
+]
 
 [tool.poetry.scripts]
 nobubo = "nobubo.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-click = "^8.0.0"
-pikepdf = "^2.12.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.4"
-tox = "^3.23.1"
-mypy = "^0.910"
-pylint = "^2.8.2"
-flake8 = "^3.9.2"
+python = "^3.10"
+click = "^8.1.3"
+pikepdf = "^7.2.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+tox = "^4.5.1"
+mypy = "^1.3.0"
+pylint = "^2.17.4"
+flake8 = "^6.0.0"
+pdfminer-six = "^20221105"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
-python_version = 3.8
+python_version = "3.10"
 
 ### --strict
 warn_unused_configs = true
 disallow_any_generics = true
 disallow_subclassing_any = true
 # disallow_untyped_calls = true
 # disallow_untyped_defs = true  
@@ -58,52 +61,60 @@
 disallow_any_unimported = true
 
 ### Output
 show_error_codes = true
 show_error_context = true
 pretty = true
 
-[[tool.mypy.overrides]]
-module = "textract.*"
 ignore_missing_imports = true
 
+[tool.coverage.run]
+omit = [
+    "*/__init__.py",
+    "*/__main__.py",
+    ]
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
 envlist = py,mypy,linting
 testpaths = "tests"
 
 [testenv]
 description = Run pytest
 deps = 
     pytest
     pytest-cov
-    rich
-    textract
+    pdfminer-six
 commands = pytest {posargs}
 
 [testenv:mypy]
 description = Check typing with mypy
 deps = mypy
-       click
        pytest
-       rich
-       textract
+       pdfminer-six
 passenv = TERM
-commands = mypy {posargs} nobubo tests
+commands = mypy {posargs} src/nobubo tests
 
 [testenv:linting]
 description = Run flake8 for linting
 deps = flake8
-commands = flake8 --max-line-length 88 nobubo tests {posargs}
+commands = flake8 --max-line-length 88 src/nobubo tests {posargs}
+
+[testenv:coverage]
+description = Run pytest with coverage
+deps = pytest
+       pytest-cov
+       pdfminer-six
+commands = pytest tests --cov=nobubo --cov-report html -Werror
 
 [testenv:pikepdf-main]
 description = Run project tests against pikepdf-main branch
 deps = 
     git+https://github.com/pikepdf/pikepdf#master
     pytest
     pytest-cov
     rich
-    textract
+    pdfminer-six
 commands = pytest {posargs}
 """
```

### Comparing `nobubo-1.4.1/setup.py` & `nobubo-1.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,148 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nobubo
+Version: 1.5.0
+Summary: Nobubo assembles a digital pdf sewing pattern and cuts it up into a desired output print size. A specialized n-up tool also suited for non-sewing purposes.
+Home-page: https://github.com/bytinbit/nobubo
+License: AGPL v3.0
+Author: bytinbit
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
+Classifier: Topic :: Printing
+Classifier: Topic :: Utilities
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pikepdf (>=7.2.0,<8.0.0)
+Project-URL: Repository, https://github.com/bytinbit/nobubo
+Description-Content-Type: text/markdown
 
-packages = \
-['nobubo']
+# Nobubo
 
-package_data = \
-{'': ['*']}
+Nobubo creates a collage from digital pattern pages and then chops it up into a 
+desired output layout. The collage is assembled according to one or several
+overview sheets. These overviews are usually provided along with the pattern
+pages in the same pdf or in the instructions pdf.
+<div align="center">
+<img src="img/nobubo-logo-dalle-nightcafe-small.png" alt="nobubo logo, nightcafe/dall-e2" width=50%/>
+</div>
 
-install_requires = \
-['click>=8.0.0,<9.0.0', 'pikepdf>=2.12.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['nobubo = nobubo.cli:main']}
-
-setup_kwargs = {
-    'name': 'nobubo',
-    'version': '1.4.1',
-    'description': 'Nobubo assembles a digital pdf sewing pattern and cuts it up into a desired output print size. A specialized n-up tool also suited for non-sewing purposes.',
-    'long_description': '# Nobubo\nDigital sewing patterns are very handy: No shipping costs and cheaper than physical patterns. There is one drawback: Many digital patterns are distributed in A4 size, and it is up to the sewist to assemble them.\n\nA jacket pattern has around 50 A4 pages that must be glued or taped together. This usually results in an apartment covered in A4 pages and a final collage in which printer irregularities lead to ill-matching pattern lines. Many indie pattern companies already sell their digital patterns as A4 and A0 in the same pattern purchase, but there are still other companies that only provide A4.\n\nThat\'s why I wrote nobubo: This tool assembles the pages of a digital pdf pattern and chops it into a desired output size, so that you can print it on any page size you want. \n\nNobubo has been developed and tested with several download patterns from Burda, Knipmode and other brands successfully. Even though nobubo has been developed with sewing patterns in mind, it is basically a fancy n-up tool for PDFs in general.\n\n## Prerequisites\n* A digital pattern where each page is made to be printed on A4 or US letter size. **If you haven\'t purchased a digital pattern, nobubo is useless**.\n* Each page is already cropped, so that only the bare pattern is visible (no white borders around the pattern). Nobubo is able to handle cropped pdfs, but you still have to do it yourself.\n* Usually, the assembled pattern pages form a huge rectangle. Some brands provide a handy overview how all the assembled pages are supposed to look like. Some brands, however, disregard this rectangle shape and the assembled pattern is of a weird "rectangle + n pages" shape. Nobubo can only handle rectangle shapes, so those leftover pages have to be print out and taped by hand.\n* Python >=3.8\n* `pdflatex` [must be installed](https://tex.stackexchange.com/questions/49569/where-to-download-pdflatex-exe)\n\n## Installation\n\n### Using pip\n\n1. [Create a virtual environment](https://docs.python-guide.org/dev/virtualenvs/#lower-level-virtualenv) \n2. Activate it and install via pip:\n\n```bash\n$ pip install nobubo\n```\n\n### Using git\n\n1. Clone this repository.\n2. Change into the folder you just cloned, it\'s called `nobubo`.\n3. [Create a virtual environment](https://docs.python-guide.org/dev/virtualenvs/#lower-level-virtualenv) in the cloned repository and activate it.\n4. Stay in the folder and install nobubo locally via pip:\n\n```bash\n$ pip install .\n```\n\nCheck the installation with one of the mock patterns and run nobubo:\n\n```bash\n$ nobubo --il 2 8 4 --ol a0 tests/testdata/mockpattern_oneoverview_8x4.pdf sample.pdf\n```\n\n## Usage\n\nShow basic information:\n\n```bash\n$ nobubo --help\n```\n\nAvailable commands:\n\n```bash\n$ nobubo --il FIRSTPAGE COLUMNS ROWS --ol {a0|us|mmxmm} {--reverse} {--margin mm} INPUTPATH OUTPUTPATH\n```\n\nHave a look at the mock patterns in the test folder. Use them with with the above commands to see how nobubo works. \n\n### Example with one overview sheet, reverse assembly, A0 output\n\nThis example pattern has one overview sheet on page 1 with 6 columns and 5 rows (see also picture below) and is assembled from bottom left to top right:\n\n```bash\n$ nobubo --il 2 6 5 --ol a0 --reverse home/alice/patterns/jacket.pdf home/alice/patterns/jacket_a0.pdf\n```\n*  `--il ` (input layout) is required and followed by three numbers:\n  * `2`: The first pattern page of all the pages that form the huge rectangle displayed on the overview sheet.\n  * `6 5`: columns and rows you count on the overview sheet.\n* `--ol` (output layout) defines the size on which the pattern shall be printed. Currently supported:\n  * `a0`: Output size is A0.\n  * `us`: Output size is "copyshop size" of 36 x 48 inches, also called "[Arch E / Arch 6 ](https://en.wikipedia.org/wiki/Paper_size#Architectural_sizes)".\n  * `mmxmm`: use a custom output size in millimeters, e.g. `920x1187`.\n* if `--ol` is omitted, nobubo just prints a huge collage of all assembled pages without chopping them up into an output layout.\n* `--reverse`: as default, the pattern is assembled from top left to bottom right. Use the `--reverse` flag to assemble it from bottom left to top right, which is for example needed for Burda patterns.\n* `home/alice/patterns/jacket.pdf`: the path to the original pattern including filename.\n* `home/alice/patterns/jacket_a0.pdf`: the path where the collage should be saved, including filename.\n\nThe pdf has 6 columns and 5 rows, which means the final pdf collage will be four A0 pages to print, since 16 A4 pages fit on one A0 page. This is how the sample overview sheet might look like and how it will be split up:\n\n<img src="img/nobubo.png" alt="sample pattern" width=30%/>\n\nOf course, you can still choose to print pages 2-4 on A4 from your original pattern and just page 1 on A0.\n\n**The order of assembly differs between pattern companies. Burda assembles the pages from bottom left to top right, whereas others (Knipmode) assemble them from top left to bottom right. Please compare the order of the pdf pages in the pdf file itself to the overview to see in which way the pages are assembled. Rarely, some brands don\'t even provide an overview sheet (booh!), which means you have to figure it out yourself.**\n\n### Example with two overview sheets\n\n```bash\n$ nobubo --il 2 8 4 -il 35 7 3 --ol a0 home/alice/mypattern.pdf  home/alice/results/mypattern_a0.pdf\n```\n\nThe first overview sheet is on page 1 with 8 columns, 4 rows, which means the pattern pages start on page `2`: `--il 2 8 4`.  The second overview sheet is on page 34 with 7 columns, 3 rows, the pattern pages start on page `35`: `--il 35 7 3`. The assembly is from top left to bottom right, the output to be printed on A0.\n\n### Example with a collage output\n\n``` bash\n$ nobubo --il 2 8 4 --il 35 7 3 home/alice/mypattern.pdf  home/alice/results/mypattern_a0.pdf\n```\n\nThis prints only two pdfs (=2 overview sheets) which contain each a huge collage.\n\n## Caveats\n* Please double-check and compare the overview sheet with the amount of pdf pages given (rows * columns = amount of pages needed).  If the result is wrong, check if you counted the rows and columns correctly or if a second overview sheet hides in later pages. Burda for example includes several overview sheets and their corresponding pages in one pdf.\n* Check if the pattern must be assembled from top left to bottom right (default) or bottom left to top right (use `--reverse` flag)\n* When you print the final pattern pages,  double-check and measure the control square. Don\'t forget to print 100% "as is", with any scaling or page fitting off.\n\n**I do not take any responsibility if nobubo leads to ill-matching garments or any other problems whatsoever. You use this tool at your own risk. If in doubt, make a backup of your original pattern pdf. Please have a look at the license if you want to improve the tool yourself.**\n\n## Thanks\n\n[The_Compiler](https://github.com/The-Compiler) for their invaluable feedback and encouragement.\n\nI was stuck on how to use pikepdf properly, [cfcurtis\' sewingutils](https://github.com/cfcurtis/sewingutils) provided an answer.\n',
-    'author': 'bytinbit',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/bytinbit/nobubo',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+# About 
 
+Digital sewing patterns are very handy: No shipping costs and cheaper than physical patterns. There is one drawback: Many digital patterns are distributed in A4 size, and it is up to the sewist to assemble them.
+
+A dress pattern has around 70 A4 pages that must be glued or taped together. This usually results in an apartment covered in A4 pages and a final collage in which small irregularities lead to ill-matching pattern lines. Many indie pattern companies already sell their digital patterns as A4 and A0 in the same pattern purchase, but there are still other companies that only provide A4.
+
+That's why I wrote nobubo: This tool assembles the pages of a digital pdf pattern and chops it into a desired output size, so that you can print it on any page size you want. 
+
+Nobubo has been developed and tested with several download patterns from Burda, Knipmode and other brands successfully. Even though nobubo has been developed with sewing patterns in mind, it is basically a fancy n-up tool for pdfs in general.
+
+## Prerequisites
+* A digital pattern where each page is made to be printed on A4 or US letter size. **If you haven't purchased a digital pattern, nobubo is useless**.
+* Each page is already cropped, so that only the bare pattern is visible (no white borders around the pattern). Nobubo is able to handle cropped pdfs, but you still have to do it yourself.
+* Usually, the assembled pattern pages form a huge rectangle. Some brands provide a handy overview how all the assembled pages are supposed to look like. Some brands, however, disregard this rectangle shape and the assembled pattern is of a weird "rectangle + n pages" shape. Nobubo can only handle rectangle shapes, so those leftover pages have to be printed out and taped by hand.
+* Python >=3.10
+* `pdflatex` [must be installed](https://tex.stackexchange.com/questions/49569/where-to-download-pdflatex-exe)
+
+## Installation
+
+### Using pip
+
+1. [Create a virtual environment](https://docs.python-guide.org/dev/virtualenvs/#lower-level-virtualenv) 
+2. Activate it and install via pip:
+
+```bash
+$ pip install nobubo
+```
+
+### Using git
+
+1. Clone this repository.
+2. Change into the folder you just cloned, it's called `nobubo`.
+3. [Create a virtual environment](https://docs.python-guide.org/dev/virtualenvs/#lower-level-virtualenv) in the cloned repository and activate it.
+4. Stay in the folder and install nobubo locally via pip:
+
+```bash
+$ pip install .
+```
+
+Check the installation with one of the mock patterns and run nobubo:
+
+```bash
+$ nobubo --il 2 8 4 --ol a0 tests/testdata/mockpattern_oneoverview_8x4.pdf sample.pdf
+```
+
+## Usage
+
+Show basic information:
+
+```bash
+$ nobubo --help
+```
+
+Available commands:
+
+```bash
+$ nobubo --il FIRSTPAGE COLUMNS ROWS --ol {a0|us|mmxmm} {--reverse} {--margin mm} INPUTPATH OUTPUTPATH
+```
+
+Have a look at the mock patterns in the test folder. Use them with with the above commands to see how nobubo works. 
+
+### Example with one overview sheet, reverse assembly, A0 output
+
+This example pattern has one overview sheet on page 1 with 6 columns and 5 rows (see also picture below) and is assembled from bottom left to top right:
+
+```bash
+$ nobubo --il 2 6 5 --ol a0 --reverse home/alice/patterns/jacket.pdf home/alice/patterns/jacket_a0.pdf
+```
+*  `--il ` (input layout) is required and followed by three numbers:
+  * `2`: The first pattern page of all the pages that form the huge rectangle displayed on the overview sheet.
+  * `6 5`: columns and rows you count on the overview sheet.
+* `--ol` (output layout) defines the size on which the pattern shall be printed. Currently supported:
+  * `a0`: Output size is A0.
+  * `us`: Output size is "copyshop size" of 36 x 48 inches, also called "[Arch E / Arch 6 ](https://en.wikipedia.org/wiki/Paper_size#Architectural_sizes)".
+  * `mmxmm`: use a custom output size in millimeters, e.g. `920x1187`.
+* if `--ol` is omitted, nobubo just prints a huge collage of all assembled pages without chopping them up into an output layout.
+* `--reverse`: as default, the pattern is assembled from top left to bottom right. Use the `--reverse` flag to assemble it from bottom left to top right, which is for example needed for Burda patterns.
+* `home/alice/patterns/jacket.pdf`: the path to the original pattern including filename.
+* `home/alice/patterns/jacket_a0.pdf`: the path where the collage should be saved, including filename.
+
+The pdf has 6 columns and 5 rows, which means the final pdf collage will be four A0 pages to print, since 16 A4 pages fit on one A0 page. This is how the sample overview sheet might look like and how it will be split up:
+
+<img src="img/nobubo.png" alt="sample pattern" width=30%/>
+
+Of course, you can still choose to print pages 2-4 on A4 from your original pattern and just page 1 on A0.
+
+**The order of assembly differs between pattern companies. Burda assembles the pages from bottom left to top right, whereas others (Knipmode) assemble them from top left to bottom right. Please compare the order of the pdf pages in the pdf file itself to the overview to see in which way the pages are assembled. Rarely, some brands don't even provide an overview sheet (booh!), which means you have to figure it out yourself.**
+
+### Example with two overview sheets
+
+```bash
+$ nobubo --il 2 8 4 -il 35 7 3 --ol a0 home/alice/mypattern.pdf  home/alice/results/mypattern_a0.pdf
+```
+
+The first overview sheet is on page 1 with 8 columns, 4 rows, which means the pattern pages start on page `2`: `--il 2 8 4`.  The second overview sheet is on page 34 with 7 columns, 3 rows, the pattern pages start on page `35`: `--il 35 7 3`. The assembly is from top left to bottom right, the output to be printed on A0.
+
+### Example with a collage output
+
+``` bash
+$ nobubo --il 2 8 4 --il 35 7 3 home/alice/mypattern.pdf  home/alice/results/mypattern_a0.pdf
+```
+
+This prints only two pdfs (=2 overview sheets) which contain each a huge collage.
+
+## Caveats
+* Please double-check and compare the overview sheet with the amount of pdf pages given (rows * columns = amount of pages needed).  If the result is wrong, check if you counted the rows and columns correctly or if a second overview sheet hides in later pages. Burda for example includes several overview sheets and their corresponding pages in one pdf.
+* Check if the pattern must be assembled from top left to bottom right (default) or bottom left to top right (use `--reverse` flag)
+* When you print the final pattern pages,  double-check and measure the control square. Don't forget to print 100% "as is", with any scaling or page fitting off.
+
+**I do not take any responsibility if nobubo leads to ill-matching garments or any other problems whatsoever. You use this tool at your own risk. Always make a backup of your original pattern pdf. Please have a look at the license if you want to improve the tool yourself.**
+
+## Thanks
+
+[The_Compiler](https://github.com/The-Compiler) for their invaluable feedback and encouragement.
+
+I was stuck on how to use pikepdf properly, [cfcurtis' pdfstitcher](https://github.com/cfcurtis/pdfstitcher) provided an answer.
 
-setup(**setup_kwargs)
```

