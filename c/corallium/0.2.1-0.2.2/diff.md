# Comparing `tmp/corallium-0.2.1.tar.gz` & `tmp/corallium-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corallium-0.2.1.tar", max compression
+gzip compressed data, was "corallium-0.2.2.tar", max compression
```

## Comparing `corallium-0.2.1.tar` & `corallium-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-04-08 17:23:14.679517 corallium-0.2.1/LICENSE
--rw-r--r--   0        0        0      505 2023-04-22 15:34:34.274654 corallium-0.2.1/corallium/__init__.py
--rw-r--r--   0        0        0     8688 2023-04-22 15:33:16.021263 corallium-0.2.1/corallium/file_helpers.py
--rw-r--r--   0        0        0     3671 2023-02-25 15:48:42.282044 corallium-0.2.1/corallium/log.py
--rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-0.2.1/corallium/loggers/__init__.py
--rw-r--r--   0        0        0      526 2023-04-22 04:53:47.931473 corallium-0.2.1/corallium/loggers/plain_printer.py
--rw-r--r--   0        0        0     2109 2023-04-08 00:00:16.873929 corallium-0.2.1/corallium/loggers/rich_printer.py
--rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-0.2.1/corallium/loggers/structlog_logger/__init__.py
--rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-0.2.1/corallium/loggers/structlog_logger/_structlog_logger.py
--rw-r--r--   0        0        0     2122 2023-02-25 16:07:54.214330 corallium-0.2.1/corallium/loggers/styles.py
--rw-r--r--   0        0        0     4486 2023-04-22 05:00:46.991583 corallium-0.2.1/corallium/pretty_process.py
--rw-r--r--   0        0        0     2493 2023-04-22 07:02:25.379564 corallium-0.2.1/corallium/shell.py
--rw-r--r--   0        0        0      192 2023-02-22 03:38:37.960591 corallium-0.2.1/corallium/tomllib.py
--rw-r--r--   0        0        0     2833 2023-04-22 15:34:38.535754 corallium-0.2.1/docs/README.md
--rw-r--r--   0        0        0     1586 2023-04-22 15:34:34.284201 corallium-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 corallium-0.2.1/setup.py
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 corallium-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-08 17:23:14.679517 corallium-0.2.2/LICENSE
+-rw-r--r--   0        0        0      505 2023-05-17 00:04:47.972377 corallium-0.2.2/corallium/__init__.py
+-rw-r--r--   0        0        0     8688 2023-04-22 15:33:16.021263 corallium-0.2.2/corallium/file_helpers.py
+-rw-r--r--   0        0        0     3671 2023-02-25 15:48:42.282044 corallium-0.2.2/corallium/log.py
+-rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-0.2.2/corallium/loggers/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-22 04:53:47.931473 corallium-0.2.2/corallium/loggers/plain_printer.py
+-rw-r--r--   0        0        0     2106 2023-05-16 23:56:42.625392 corallium-0.2.2/corallium/loggers/rich_printer.py
+-rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-0.2.2/corallium/loggers/structlog_logger/__init__.py
+-rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-0.2.2/corallium/loggers/structlog_logger/_structlog_logger.py
+-rw-r--r--   0        0        0     2122 2023-02-25 16:07:54.214330 corallium-0.2.2/corallium/loggers/styles.py
+-rw-r--r--   0        0        0     4486 2023-04-22 05:00:46.991583 corallium-0.2.2/corallium/pretty_process.py
+-rw-r--r--   0        0        0     2493 2023-04-22 07:02:25.379564 corallium-0.2.2/corallium/shell.py
+-rw-r--r--   0        0        0      192 2023-02-22 03:38:37.960591 corallium-0.2.2/corallium/tomllib.py
+-rw-r--r--   0        0        0     2833 2023-05-17 00:04:53.524551 corallium-0.2.2/docs/README.md
+-rw-r--r--   0        0        0     1586 2023-05-17 00:04:47.987207 corallium-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 corallium-0.2.2/setup.py
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 corallium-0.2.2/PKG-INFO
```

### Comparing `corallium-0.2.1/LICENSE` & `corallium-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/corallium/file_helpers.py` & `corallium-0.2.2/corallium/file_helpers.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/corallium/log.py` & `corallium-0.2.2/corallium/log.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/corallium/loggers/plain_printer.py` & `corallium-0.2.2/corallium/loggers/plain_printer.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/corallium/loggers/rich_printer.py` & `corallium-0.2.2/corallium/loggers/rich_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     full_lines = []
     for key in _keys_on_own_line or []:
         if line := kwargs.pop(key, None):
             full_lines.append((key, line))
     for key, value in kwargs.items():
         text.append(f' {key}=', style=_styles.key)
-        text.append(f'{str(value)}', style=_styles.value)
+        text.append(f'{value!s}', style=_styles.value)
     _console.print(text)
     for key, line in full_lines:
         new_text = Text()
         new_text.append(f' ∟ {key}', style=_styles.key)
         new_text.append(f': {line}', style=_styles.value_own_line)
         _console.print(new_text)
```

### Comparing `corallium-0.2.1/corallium/loggers/structlog_logger/_structlog_logger.py` & `corallium-0.2.2/corallium/loggers/structlog_logger/_structlog_logger.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/corallium/loggers/styles.py` & `corallium-0.2.2/corallium/loggers/styles.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/corallium/pretty_process.py` & `corallium-0.2.2/corallium/pretty_process.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/corallium/shell.py` & `corallium-0.2.2/corallium/shell.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/docs/README.md` & `corallium-0.2.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `corallium-0.2.1/pyproject.toml` & `corallium-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "0.2.1"
+version = "0.2.2"
 version_files = ["corallium/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -22,25 +22,25 @@
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "corallium"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/corallium"
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 beartype = ">=0.12.0"
 pydantic = ">=1.10.4"
 rich = ">=12.6.0"
 tomli = {markers = "python_version < '3.11'", version = ">=2.0.1"}
 
 [tool.poetry.group.dev.dependencies]
-calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=1.2.1"}
+calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=1.2.4"}
 pytest-structlog = ">=0.6" # Provides pytest fixture 'log'
 pytest-subprocess = ">=1.4.1"
 structlog = ">=22.3.0"
 types-pyyaml = ">=6.0.12.8"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kyleking/corallium/issues"
```

### Comparing `corallium-0.2.1/setup.py` & `corallium-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['beartype>=0.12.0', 'pydantic>=1.10.4', 'rich>=12.6.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1']}
 
 setup_kwargs = {
     'name': 'corallium',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Shared functionality for calcipy-ecosystem',
     'long_description': '# corallium\n\nShared functionality for the calcipy-ecosystem.\n\n## Installation\n\n1. `poetry add corallium`\n\n1. Take advantage of the logger or other common functionality\n\n    ```sh\n    form corallium.log import logger\n\n    logger.info(\'Hello!\')\n    ```\n\n## Usage\n\n<!-- < TODO: Show an example (screenshots, terminal recording, etc.) >\n\n- **log**: TBD\n- **pretty_process**: TBD\n- **shell**: TBD\n- **file_helpers**: TBD\n- **tomllib**: This is a lightweight wrapper to backport `tomli` in place of `tomllib` until we can use Python >3.11. Use with `from corallium.tomllib import tomllib`\n- **dot_dict**: has one function `ddict`, which is a light-weight wrapper around whatever is the most [maintained dotted-dictionary package in Python](https://pypi.org/search/?q=dot+accessible+dictionary&o=). Dotted dictionaries can sometimes improve code readability, but they aren\'t a one-size fits all solution. Sometimes `attr.s` or `dataclass` are more appropriate.\n    - The benefit of this wrapper is a stable interface that can be replaced with better internal implementations, such [Bunch](https://pypi.org/project/bunch/), [Chunk](https://pypi.org/project/chunk/), [Munch](https://pypi.org/project/munch/), [flexible-dotdict](https://pypi.org/project/flexible-dotdict/), [classy-json](https://pypi.org/project/classy-json/), and now [Python-Box](https://pypi.org/project/python-box/)\n -->\n\nFor more example code, see the [scripts] directory or the [tests].\n\n## Project Status\n\nSee the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].\n\n## Contributing\n\nWe welcome pull requests! For your pull request to be accepted smoothly, we suggest that you first open a GitHub issue to discuss your idea. For resources on getting started with the code base, see the below documentation:\n\n- [DEVELOPER_GUIDE]\n- [STYLE_GUIDE]\n\n## Code of Conduct\n\nWe follow the [Contributor Covenant Code of Conduct][contributor-covenant].\n\n### Open Source Status\n\nWe try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/corallium)\n\n## Responsible Disclosure\n\nIf you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).\n\n## License\n\n[LICENSE]\n\n[changelog]: https://corallium.kyleking.me/docs/CHANGELOG\n[code_tag_summary]: https://corallium.kyleking.me/docs/CODE_TAG_SUMMARY\n[contributor-covenant]: https://www.contributor-covenant.org\n[developer_guide]: https://corallium.kyleking.me/docs/DEVELOPER_GUIDE\n[license]: https://github.com/kyleking/corallium/blob/main/LICENSE\n[scripts]: https://github.com/kyleking/corallium/blob/main/scripts\n[style_guide]: https://corallium.kyleking.me/docs/STYLE_GUIDE\n[tests]: https://github.com/kyleking/corallium/blob/main/tests\n',
     'author': 'Kyle King',
     'author_email': 'dev.act.kyle@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyleking/corallium',
```

### Comparing `corallium-0.2.1/PKG-INFO` & `corallium-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corallium
-Version: 0.2.1
+Version: 0.2.2
 Summary: Shared functionality for calcipy-ecosystem
 Home-page: https://github.com/kyleking/corallium
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

