# Comparing `tmp/scrapy_processors-1.0.1.tar.gz` & `tmp/scrapy_processors-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_processors-1.0.1.tar", max compression
+gzip compressed data, was "scrapy_processors-1.1.0.tar", max compression
```

## Comparing `scrapy_processors-1.0.1.tar` & `scrapy_processors-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_processors-1.0.1/LICENSE
--rw-r--r--   0        0        0     6039 2023-05-16 13:20:04.801881 scrapy_processors-1.0.1/README.md
--rw-r--r--   0        0        0      752 2023-05-16 14:57:05.176941 scrapy_processors-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-16 13:15:28.932402 scrapy_processors-1.0.1/scrapy_processors/__init__.py
--rw-r--r--   0        0        0     5431 2023-05-16 15:14:20.997819 scrapy_processors-1.0.1/scrapy_processors/processors.py
--rw-r--r--   0        0        0     6922 1970-01-01 00:00:00.000000 scrapy_processors-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-16 13:45:56.239068 scrapy_processors-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6604 2023-05-17 14:50:33.362775 scrapy_processors-1.1.0/README.md
+-rw-r--r--   0        0        0      793 2023-05-17 14:25:20.631596 scrapy_processors-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-16 13:15:28.932402 scrapy_processors-1.1.0/scrapy_processors/__init__.py
+-rw-r--r--   0        0        0     7178 2023-05-17 14:06:02.392719 scrapy_processors-1.1.0/scrapy_processors/processors.py
+-rw-r--r--   0        0        0     7537 1970-01-01 00:00:00.000000 scrapy_processors-1.1.0/PKG-INFO
```

### Comparing `scrapy_processors-1.0.1/LICENSE` & `scrapy_processors-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_processors-1.0.1/README.md` & `scrapy_processors-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 
 # Scrapy Processors
 
+![License](https://img.shields.io/badge/license-MIT-blue.svg)
+[![Python Versions](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+<!-- [![codecov](https://codecov.io/gh/nicholas-mischke/scrapy-processors/branch/master/graph/badge.svg)](https://codecov.io/gh/nicholas-mischke/scrapy-processors) -->
+
+
 Scrapy Processors is a collection of Processor classes meant to extend the collection provided in the [itemloaders](https://pypi.org/project/itemloaders/) package, commonly used with the [scrapy](https://pypi.org/project/Scrapy/) webscraping framework.
 
 
 https://docs.scrapy.org/en/latest/topics/loaders.html
 
 ## Repositories
-[PyPi]("https://pypi.org/scrapy-processors/")
+[PyPI](https://pypi.org/project/scrapy-processors/)
 
-[GitHub]("https://github.com/nicholas-mischke/scrapy-processors")
+[GitHub](https://github.com/nicholas-mischke/scrapy-processors)
 
 ## Installation
 
 To install Scrapy Processors, simply use pip:
 
 ```
 $ pip install scrapy-processors
 ```
 
 ## Usage
 
 Here is an overview of the processors available in the package:
 
-- `MapCompose`: A processor that allows for the sequential application of multiple callables to a list of values. 
+- `MapCompose`: A processor that allows you to specify a list of callables that will be applied sequentially to a value, or to each value in a list of values. 
     It supports functions (regular functions, lambda or methods), objects with a `__call__` method or classes that once initialized return an object with a `__call__` method.
-    This class inherits from itemloaders.processors.MapCompose and overrides its constructor.
+    This class inherits from itemloaders.processors.MapCompose and overrides its constructor and defines `__add__`.
 - `Processor`: A base class for creating custom processors. Subclasses of `Processor` should implement the `process_value` method.
 - `EnsureEncoding`: A processor that converts a string to a specified encoding, defaults to utf-8 & ignores errors.
 - `NormalizeWhitespace`: A processor that normalizes whitespace in a string by 
-    removing zero-width spaces, replacing multiple whitespaces with a single whitespace, removeing leading whitespace in front of punctuation and finally removing leading/trailing whitespaces. 
+    removing zero-width spaces, replacing multiple whitespaces with a single whitespace, removing leading whitespace in front of punctuation and finally removing leading/trailing whitespaces. 
     default punctuation=(',', '.', '!', '?', ';', ':')
 - `PriceParser`: A processor that converts a string representing a price to a `Price` object using the `price_parser` library.
 - `RemoveHTMLTags`: A processor that removes HTML tags from a string using the `BeautifulSoup` library.
 - `Demojize`: A processor that replaces Unicode emojis in a string with emoji shortcodes using the `emoji` library.
 - `RemoveEmojis`: A processor that removes emojis from a string using the `emoji` library.
-- `StringToDateTime`: A processor that converts a string representing a date and time to a `datetime` object. default format='%Y-%m-%d, %H:%M:%S'
-- `StringToDate`: A processor that converts a string representing a date to a `date` object. default format='%Y-%m-%d'
-- `StringToTime`: A processor that converts a string representing a time to a `time` object. default format='%H:%M:%S'
+- `StripQuotes`: A processor that removes any number of leading/trailing quotes or tick marks from a string.
+- `StringToDateTime`: A processor that converts a string representing a date and time to a `datetime.datetime` object. default format='%Y-%m-%d, %H:%M:%S'
+- `StringToDate`: A processor that converts a string representing a date to a `datetime.date` object. default format='%Y-%m-%d'
+- `StringToTime`: A processor that converts a string representing a time to a `datetime.time` object. default format='%H:%M:%S'
 - `TakeAll`: A processor that returns all values passed to it. This is a renaming of the built-in `Identity` processor.
 - `TakeAllTruthy`: A processor that returns all truthy values passed to it. It also accepts a default value to return if no values are truthy.
 
 
 
 ```python
 # example.py
@@ -92,37 +98,37 @@
 
 To contribute to this project, please follow these steps:
 
 1. Fork the repository by clicking on the "Fork" button at the top of the repository page. This will create a copy of the repository in your GitHub account.
 2. Clone the forked repository to your local machine using Git:
 
     ```
-    $ git clone https://github.com/your-username/repository.git
+    $ git clone https://github.com/your-username/scrapy-processors.git
     ```
 
 3. Create a new branch for your changes:
 
     ```
-    $ git checkout -b feature/new-feature
+    $ git checkout -b feature
     ```
 
 4. Make your desired changes to the codebase.
 5. Commit your changes with descriptive commit messages:
 
     ```
     $ git commit -m "Add new feature"
     ```
 
 6. Push your changes to your forked repository:
 
     ```
-    $ git push origin feature/new-feature
+    $ git push origin feature
     ```
 
-7. Open a pull request (PR) from your forked repository to the original repository's `main` branch.
+7. Open a pull request (PR) from your forked repository to the original repository's `master` branch.
 8. Provide a clear and descriptive title for your PR and explain the changes you have made.
 9. Wait for the project maintainers to review your PR. You may need to make additional changes based on their feedback.
 10. Once your PR is approved, it will be merged into the main codebase. Congratulations on your contribution!
 
 If you have any questions or need further assistance, feel free to open an issue or reach out to the project maintainers.
 
 Happy contributing!
```

### Comparing `scrapy_processors-1.0.1/pyproject.toml` & `scrapy_processors-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 
 [tool.poetry]
 name = "scrapy-processors"
-version = "1.0.1"
+version = "1.1.0"
 description = "Provides processors for the itemloaders package, commonly used with scrapy."
 authors = ["Nicholas Mischke <nmischkework@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "scrapy_processors"}]
 repository = "https://github.com/nicholas-mischke/scrapy-processors"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.7"
 itemloaders = "1.1.0"
 emoji = "2.2.0"
 price-parser = "0.3.4"
 beautifulsoup4 = "4.12.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "4.0.0"
+tox = "4.5.1"
+coverage = "7.2.5"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 sources = [
-    {name = "pypi scrapy-processors", url = "https://pypi.org/scrapy-processors/"},
+    {name = "pypi scrapy-processors", url = "https://pypi.org/project/scrapy-processors/"},
 ]
```

### Comparing `scrapy_processors-1.0.1/scrapy_processors/processors.py` & `scrapy_processors-1.1.0/scrapy_processors/processors.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,14 +34,46 @@
                 functions.append(callable)
             elif isclass(callable):
                 functions.append(callable().__call__)
             elif hasattr(callable, '__call__'):
                 functions.append(callable.__call__)
         self.functions = tuple(functions)
 
+    def __add__(self, other):
+        # Must be of of type MapCompose or subclass
+        if not isinstance(other, MapCompose):
+            raise TypeError(
+                f"Unsupported operand type for +: 'MapCompose' and '{type(other).__name__}'"
+            )
+
+        # default_loader_context must have same key:value pairs
+        # if the keys are present in both
+        shared_keys = set(self.default_loader_context.keys()) & set(
+            other.default_loader_context.keys())
+
+        error_msg = ''
+        for key in shared_keys:
+            if self.default_loader_context[key] != other.default_loader_context[key]:
+                error_msg += f"Key: {key}, self[{key}]: {self.default_loader_context[key]}, other[{key}]: {other.default_loader_context[key]}\n"
+        if error_msg:
+            error_msg = (
+                "Cannot add MapCompose objects with mismatched "
+                "key, value pairs in their default_loader_context\n"
+            ) + error_msg
+            raise ValueError(error_msg.strip())
+
+        # Combine default_loader_contexts
+        default_loader_context = self.default_loader_context.copy()
+        default_loader_context.update(other.default_loader_context)
+
+        # Combine functions
+        functions = self.functions + other.functions
+
+        return MapCompose(*functions, **default_loader_context)
+
 
 class Processor:
 
     def process_value(self, value):
         raise NotImplementedError()
 
     def __call__(self, values):
@@ -138,14 +170,26 @@
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def process_value(self, value):
         return emoji.replace_emoji(value, **self.kwargs)
 
 
+class StripQuotes(Processor):
+    """
+    Given a string, return a string striped of any number of quotes/tick marks.
+    Assumes utf8, utf16, ascii or latin-1 encoding.
+    """
+
+    pattern = r'^[`ˋ‘’“”\'"\u0060\u02CB\x91\x92\x93\x94]+|[`ˋ‘’“”\'"\u0060\u02CB\x91\x92\x93\x94]+$'
+
+    def process_value(self, value):
+        return re.sub(self.pattern, '', value)
+    
+
 class StringToDateTime(Processor):
     """
     Given a string representing a date and time, return a datetime object.
     """
 
     def __init__(self, format='%Y-%m-%d, %H:%M:%S'):
         self.format = format
```

### Comparing `scrapy_processors-1.0.1/PKG-INFO` & `scrapy_processors-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 Metadata-Version: 2.1
 Name: scrapy-processors
-Version: 1.0.1
+Version: 1.1.0
 Summary: Provides processors for the itemloaders package, commonly used with scrapy.
 Home-page: https://github.com/nicholas-mischke/scrapy-processors
 License: MIT
 Author: Nicholas Mischke
 Author-email: nmischkework@proton.me
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (==4.12.2)
 Requires-Dist: emoji (==2.2.0)
 Requires-Dist: itemloaders (==1.1.0)
 Requires-Dist: price-parser (==0.3.4)
 Project-URL: Repository, https://github.com/nicholas-mischke/scrapy-processors
 Description-Content-Type: text/markdown
 
 
 # Scrapy Processors
 
+![License](https://img.shields.io/badge/license-MIT-blue.svg)
+[![Python Versions](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+<!-- [![codecov](https://codecov.io/gh/nicholas-mischke/scrapy-processors/branch/master/graph/badge.svg)](https://codecov.io/gh/nicholas-mischke/scrapy-processors) -->
+
+
 Scrapy Processors is a collection of Processor classes meant to extend the collection provided in the [itemloaders](https://pypi.org/project/itemloaders/) package, commonly used with the [scrapy](https://pypi.org/project/Scrapy/) webscraping framework.
 
 
 https://docs.scrapy.org/en/latest/topics/loaders.html
 
 ## Repositories
-[PyPi]("https://pypi.org/scrapy-processors/")
+[PyPI](https://pypi.org/project/scrapy-processors/)
 
-[GitHub]("https://github.com/nicholas-mischke/scrapy-processors")
+[GitHub](https://github.com/nicholas-mischke/scrapy-processors)
 
 ## Installation
 
 To install Scrapy Processors, simply use pip:
 
 ```
 $ pip install scrapy-processors
 ```
 
 ## Usage
 
 Here is an overview of the processors available in the package:
 
-- `MapCompose`: A processor that allows for the sequential application of multiple callables to a list of values. 
+- `MapCompose`: A processor that allows you to specify a list of callables that will be applied sequentially to a value, or to each value in a list of values. 
     It supports functions (regular functions, lambda or methods), objects with a `__call__` method or classes that once initialized return an object with a `__call__` method.
-    This class inherits from itemloaders.processors.MapCompose and overrides its constructor.
+    This class inherits from itemloaders.processors.MapCompose and overrides its constructor and defines `__add__`.
 - `Processor`: A base class for creating custom processors. Subclasses of `Processor` should implement the `process_value` method.
 - `EnsureEncoding`: A processor that converts a string to a specified encoding, defaults to utf-8 & ignores errors.
 - `NormalizeWhitespace`: A processor that normalizes whitespace in a string by 
-    removing zero-width spaces, replacing multiple whitespaces with a single whitespace, removeing leading whitespace in front of punctuation and finally removing leading/trailing whitespaces. 
+    removing zero-width spaces, replacing multiple whitespaces with a single whitespace, removing leading whitespace in front of punctuation and finally removing leading/trailing whitespaces. 
     default punctuation=(',', '.', '!', '?', ';', ':')
 - `PriceParser`: A processor that converts a string representing a price to a `Price` object using the `price_parser` library.
 - `RemoveHTMLTags`: A processor that removes HTML tags from a string using the `BeautifulSoup` library.
 - `Demojize`: A processor that replaces Unicode emojis in a string with emoji shortcodes using the `emoji` library.
 - `RemoveEmojis`: A processor that removes emojis from a string using the `emoji` library.
-- `StringToDateTime`: A processor that converts a string representing a date and time to a `datetime` object. default format='%Y-%m-%d, %H:%M:%S'
-- `StringToDate`: A processor that converts a string representing a date to a `date` object. default format='%Y-%m-%d'
-- `StringToTime`: A processor that converts a string representing a time to a `time` object. default format='%H:%M:%S'
+- `StripQuotes`: A processor that removes any number of leading/trailing quotes or tick marks from a string.
+- `StringToDateTime`: A processor that converts a string representing a date and time to a `datetime.datetime` object. default format='%Y-%m-%d, %H:%M:%S'
+- `StringToDate`: A processor that converts a string representing a date to a `datetime.date` object. default format='%Y-%m-%d'
+- `StringToTime`: A processor that converts a string representing a time to a `datetime.time` object. default format='%H:%M:%S'
 - `TakeAll`: A processor that returns all values passed to it. This is a renaming of the built-in `Identity` processor.
 - `TakeAllTruthy`: A processor that returns all truthy values passed to it. It also accepts a default value to return if no values are truthy.
 
 
 
 ```python
 # example.py
@@ -114,37 +121,37 @@
 
 To contribute to this project, please follow these steps:
 
 1. Fork the repository by clicking on the "Fork" button at the top of the repository page. This will create a copy of the repository in your GitHub account.
 2. Clone the forked repository to your local machine using Git:
 
     ```
-    $ git clone https://github.com/your-username/repository.git
+    $ git clone https://github.com/your-username/scrapy-processors.git
     ```
 
 3. Create a new branch for your changes:
 
     ```
-    $ git checkout -b feature/new-feature
+    $ git checkout -b feature
     ```
 
 4. Make your desired changes to the codebase.
 5. Commit your changes with descriptive commit messages:
 
     ```
     $ git commit -m "Add new feature"
     ```
 
 6. Push your changes to your forked repository:
 
     ```
-    $ git push origin feature/new-feature
+    $ git push origin feature
     ```
 
-7. Open a pull request (PR) from your forked repository to the original repository's `main` branch.
+7. Open a pull request (PR) from your forked repository to the original repository's `master` branch.
 8. Provide a clear and descriptive title for your PR and explain the changes you have made.
 9. Wait for the project maintainers to review your PR. You may need to make additional changes based on their feedback.
 10. Once your PR is approved, it will be merged into the main codebase. Congratulations on your contribution!
 
 If you have any questions or need further assistance, feel free to open an issue or reach out to the project maintainers.
 
 Happy contributing!
```

