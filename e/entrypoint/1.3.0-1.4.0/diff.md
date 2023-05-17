# Comparing `tmp/entrypoint-1.3.0.tar.gz` & `tmp/entrypoint-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entrypoint-1.3.0.tar", max compression
+gzip compressed data, was "entrypoint-1.4.0.tar", max compression
```

## Comparing `entrypoint-1.3.0.tar` & `entrypoint-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1092 2022-07-05 21:54:31.769498 entrypoint-1.3.0/LICENSE
--rw-r--r--   0        0        0     4670 2022-07-05 21:54:31.769498 entrypoint-1.3.0/README.md
--rw-r--r--   0        0        0      605 2022-07-05 21:54:31.769498 entrypoint-1.3.0/entrypoint/__init__.py
--rw-r--r--   0        0        0     1850 2022-07-05 21:54:31.769498 entrypoint-1.3.0/entrypoint/core.py
--rw-r--r--   0        0        0        0 2022-07-05 21:54:31.769498 entrypoint-1.3.0/entrypoint/py.typed
--rw-r--r--   0        0        0     2961 2022-07-05 21:54:31.773498 entrypoint-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5419 1970-01-01 00:00:00.000000 entrypoint-1.3.0/setup.py
--rw-r--r--   0        0        0     5751 1970-01-01 00:00:00.000000 entrypoint-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-17 20:29:36.586464 entrypoint-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4864 2023-05-17 20:29:36.586464 entrypoint-1.4.0/README.md
+-rw-r--r--   0        0        0      619 2023-05-17 20:29:36.586464 entrypoint-1.4.0/entrypoint/__init__.py
+-rw-r--r--   0        0        0     1818 2023-05-17 20:29:36.586464 entrypoint-1.4.0/entrypoint/core.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:29:36.586464 entrypoint-1.4.0/entrypoint/py.typed
+-rw-r--r--   0        0        0     3202 2023-05-17 20:29:36.586464 entrypoint-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6028 1970-01-01 00:00:00.000000 entrypoint-1.4.0/PKG-INFO
```

### Comparing `entrypoint-1.3.0/LICENSE` & `entrypoint-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `entrypoint-1.3.0/README.md` & `entrypoint-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 $ poetry add entrypoint
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-entrypoint = "^1.3.0"
+entrypoint = "^1.4.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.entrypoint]
 git = "https://github.com/nekitdev/entrypoint.git"
@@ -124,29 +124,34 @@
 ```python
 from entrypoint import is_main
 
 if is_main(__name__):
     print("Hello, world!")
 ```
 
+### Return
+
+`entrypoint` expects `main` functions to not return anything. Even though this is *not* checked
+at *runtime*, returning from `main` will cause *type-checkers* to *error*!
+
 ### Async
 
 `entrypoint` does not provide any specific functionality to run async functions.
 
 Instead, you can specify, for example, a `main` function that runs its `async_main` counterpart:
 
 ```python
-import asyncio
+from async_extensions import run
 
 async def async_main() -> None:
     print("Hello, world!")
 
 @entrypoint(__name__)
 def main() -> None:
-    asyncio.run(async_main())
+    run(async_main())
 ```
 
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
```

### Comparing `entrypoint-1.3.0/entrypoint/core.py` & `entrypoint-1.4.0/entrypoint/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-from typing import Any, Callable, Type, TypeVar, overload
+from typing import Callable, Type, TypeVar, overload
 
-__all__ = ("MAIN", "EntryPoint", "entrypoint", "is_main")
+from attrs import frozen
 
-R = TypeVar("R")
+__all__ = ("MAIN", "Main", "EntryPoint", "entrypoint", "is_main")
 
-Main = Callable[[], R]
+Main = Callable[[], None]
+"""The `main` function that does not return anything."""
 
-# XXX: change to M[R] if/when HKTs get added?
-M = TypeVar("M", bound=Main[Any])
+M = TypeVar("M", bound=Main)
 
 MAIN = "__main__"
+"""The `__main__` name constant."""
 
 
 def is_main(name: str) -> bool:
-    """Checks if `name` equals `__main__`.
+    """Checks if the `name` is equal to `__main__`.
 
     Arguments:
         name: The name to check.
 
     Returns:
         Whether the `name` is equal to `__main__`.
     """
     return name == MAIN
 
 
+@frozen()
 class EntryPoint:
-    """Handlers for [`@entrypoint`][entrypoint.core.entrypoint] decorators."""
+    """Represents handlers for [`@entrypoint`][entrypoint.core.entrypoint] decorators."""
 
-    def __init__(self, name: str) -> None:
-        self._name = name
-
-    @property
-    def name(self) -> str:
-        return self._name
+    name: str
 
     def call(self, main: M) -> M:
         if is_main(self.name):
             main()
 
         return main
 
@@ -53,30 +50,28 @@
 
 
 @overload
 def entrypoint(name: str, entrypoint_type: Type[EP]) -> EP:
     ...
 
 
-def entrypoint(
-    name: str, entrypoint_type: Type[EntryPoint] = EntryPoint
-) -> EntryPoint:
+def entrypoint(name: str, entrypoint_type: Type[EntryPoint] = EntryPoint) -> EntryPoint:
     """Defines decorated functions as entry points.
 
     Calls the wrapped function if the module gets run directly.
 
     Instead of applying dark magic, this function expects
     callers to pass the `__name__` variable as an argument,
     and merely checks it against `__main__` when needed.
 
     `entrypoint_type(name)` is created under the hood, and is
     then used to handle calls.
 
     Args:
-        name: The `__name__` of the module
-        entrypoint_type: An [`EntryPoint`][entrypoint.core.EntryPoint]
+        name: The `__name__` of the module.
+        entrypoint_type: The [`EntryPoint`][entrypoint.core.EntryPoint]
             type that is used to handle calls.
 
     Returns:
-        An [`EntryPoint`][entrypoint.core.EntryPoint] instance.
+        The created [`EntryPoint`][entrypoint.core.EntryPoint] instance.
     """
     return entrypoint_type(name)
```

### Comparing `entrypoint-1.3.0/pyproject.toml` & `entrypoint-1.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entrypoint"
-version = "1.3.0"
+version = "1.4.0"
 description = "Decorated functions as entry points."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/entrypoint"
@@ -27,53 +27,65 @@
 Issues = "https://github.com/nekitdev/entrypoint/issues"
 
 [[tool.poetry.packages]]
 include = "entrypoint"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
+attrs = ">= 23.1.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.6.0"
+black = "23.3.0"
+flake8-pyproject = "1.2.3"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.10.1"
-python = "^3.7"
+version = "5.12.0"
+python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "0.961"
+mypy = "1.3.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.1.2"
-pytest-cov = "3.0.0"
-typing-extensions = "4.2.0"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
+typing-extensions = "4.5.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.0"
-mkdocs-material = "8.3.8"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.12"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.19.0"
+version = "0.21.2"
 extras = ["python"]
 
+[tool.poetry.group.dev.dependencies]
+changelogging = "1.2.0"
+
 [tool.black]
 line_length = 100
 
+[tool.flake8]
+max_line_length = 100
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--cov entrypoint"
 testpaths = ["tests"]
@@ -118,28 +130,28 @@
 
 warn_no_return = true
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
-[tool.changelog]
+[tool.changelogging]
 name = "entrypoint"
-version = "1.3.0"
+version = "1.4.0"
 url = "https://github.com/nekitdev/entrypoint"
 directory = "changes"
 output = "CHANGELOG.md"
 
-start_string = "<!-- changelog: start -->"
+start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
 issue_format = "[#{issue}]({url}/pull/{issue})"
 
 bullet = "-"
 wrap = true
 wrap_size = 100
 
 display = ["feature", "change", "fix", "security", "deprecation", "removal", "internal"]
 
 [build-system]
-requires = ["poetry-core >= 1.1.0b2"]
+requires = ["poetry-core >= 1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `entrypoint-1.3.0/setup.py` & `entrypoint-1.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,234 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: entrypoint
+Version: 1.4.0
+Summary: Decorated functions as entry points.
+Home-page: https://github.com/nekitdev/entrypoint
+License: MIT
+Keywords: python,entrypoint,entry
+Author: nekitdev
+Requires-Python: >=3.7
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: attrs (>=23.1.0)
+Project-URL: Documentation, https://nekitdev.github.io/entrypoint
+Project-URL: Discord, https://nekit.dev/discord
+Project-URL: Funding, https://patreon.com/nekitdev
+Project-URL: Issues, https://github.com/nekitdev/entrypoint/issues
+Project-URL: Repository, https://github.com/nekitdev/entrypoint
+Description-Content-Type: text/markdown
 
-packages = \
-['entrypoint']
+# `entrypoint`
 
-package_data = \
-{'': ['*']}
+[![License][License Badge]][License]
+[![Version][Version Badge]][Package]
+[![Downloads][Downloads Badge]][Package]
+[![Discord][Discord Badge]][Discord]
 
-setup_kwargs = {
-    'name': 'entrypoint',
-    'version': '1.3.0',
-    'description': 'Decorated functions as entry points.',
-    'long_description': '# `entrypoint`\n\n[![License][License Badge]][License]\n[![Version][Version Badge]][Package]\n[![Downloads][Downloads Badge]][Package]\n[![Discord][Discord Badge]][Discord]\n\n[![Documentation][Documentation Badge]][Documentation]\n[![Check][Check Badge]][Actions]\n[![Test][Test Badge]][Actions]\n[![Coverage][Coverage Badge]][Coverage]\n\n> *Decorated functions as entry points.*\n\nIn python, an *entry point* can be thought of as an explicit function\nthat gets called when the script is run directly from the console.\n\nDefining an entry point requires some boilerplate code, which is\nabstracted away by this library.\n\n## Installing\n\n**Python 3.7 or above is required.**\n\n### pip\n\nInstalling the library with `pip` is quite simple:\n\n```console\n$ pip install entrypoint\n```\n\nAlternatively, the library can be installed from source:\n\n```console\n$ git clone https://github.com/nekitdev/entrypoint.git\n$ cd entrypoint\n$ python -m pip install .\n```\n\n### poetry\n\nYou can add `entrypoint` as a dependency with the following command:\n\n```console\n$ poetry add entrypoint\n```\n\nOr by directly specifying it in the configuration like so:\n\n```toml\n[tool.poetry.dependencies]\nentrypoint = "^1.3.0"\n```\n\nAlternatively, you can add it directly from the source:\n\n```toml\n[tool.poetry.dependencies.entrypoint]\ngit = "https://github.com/nekitdev/entrypoint.git"\n```\n\n## Examples\n\n### Decorated\n\nDeclare the `main` function as an *entry point*:\n\n```python\nfrom entrypoint import entrypoint\n\n@entrypoint(__name__)\ndef main() -> None:\n    print("Hello, world!")\n```\n\nRun the script directly from the console:\n\n```console\n$ python file.py\nHello, world!\n```\n\nWhen importing the module, `main` does not get called:\n\n```python\n>>> import file\n>>> # no output\n```\n\n### Note\n\nNote that `main` gets called **immediately, before any code below can be executed**.\n\n```python\n@entrypoint(__name__)\ndef main() -> None:\n    print("-> in main")\n\nprint("<- outside")\n```\n\n```console\n$ python note.py\n-> in main\n<- outside\n```\n\n### Direct\n\nIt is possible to run `main` directly:\n\n```python\nentrypoint(__name__).call(main)\n```\n\nThis method allows to take control over where and when the function gets called.\n\n### Check\n\n`entrypoint` also provides `is_main` function that resembles\nthe common (and de-facto standard) way of implementing *entry points*:\n\n```python\nfrom entrypoint import is_main\n\nif is_main(__name__):\n    print("Hello, world!")\n```\n\n### Async\n\n`entrypoint` does not provide any specific functionality to run async functions.\n\nInstead, you can specify, for example, a `main` function that runs its `async_main` counterpart:\n\n```python\nimport asyncio\n\nasync def async_main() -> None:\n    print("Hello, world!")\n\n@entrypoint(__name__)\ndef main() -> None:\n    asyncio.run(async_main())\n```\n\n## Documentation\n\nYou can find the documentation [here][Documentation].\n\n## Support\n\nIf you need support with the library, you can send an [email][Email]\nor refer to the official [Discord server][Discord].\n\n## Changelog\n\nYou can find the changelog [here][Changelog].\n\n## Security Policy\n\nYou can find the Security Policy of `entrypoint` [here][Security].\n\n## Contributing\n\nIf you are interested in contributing to `entrypoint`, make sure to take a look at the\n[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].\n\n## License\n\n`entrypoint` is licensed under the MIT License terms. See [License][License] for details.\n\n[Email]: mailto:support@nekit.dev\n\n[Discord]: https://nekit.dev/discord\n\n[Actions]: https://github.com/nekitdev/entrypoint/actions\n\n[Changelog]: https://github.com/nekitdev/entrypoint/blob/main/CHANGELOG.md\n[Code of Conduct]: https://github.com/nekitdev/entrypoint/blob/main/CODE_OF_CONDUCT.md\n[Contributing Guide]: https://github.com/nekitdev/entrypoint/blob/main/CONTRIBUTING.md\n[Security]: https://github.com/nekitdev/entrypoint/blob/main/SECURITY.md\n\n[License]: https://github.com/nekitdev/entrypoint/blob/main/LICENSE\n\n[Package]: https://pypi.org/project/entrypoint\n[Coverage]: https://codecov.io/gh/nekitdev/entrypoint\n[Documentation]: https://nekitdev.github.io/entrypoint\n\n[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2\n[License Badge]: https://img.shields.io/pypi/l/entrypoint\n[Version Badge]: https://img.shields.io/pypi/v/entrypoint\n[Downloads Badge]: https://img.shields.io/pypi/dm/entrypoint\n\n[Documentation Badge]: https://github.com/nekitdev/entrypoint/workflows/docs/badge.svg\n[Check Badge]: https://github.com/nekitdev/entrypoint/workflows/check/badge.svg\n[Test Badge]: https://github.com/nekitdev/entrypoint/workflows/test/badge.svg\n[Coverage Badge]: https://codecov.io/gh/nekitdev/entrypoint/branch/main/graph/badge.svg\n',
-    'author': 'nekitdev',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nekitdev/entrypoint',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7',
-}
+[![Documentation][Documentation Badge]][Documentation]
+[![Check][Check Badge]][Actions]
+[![Test][Test Badge]][Actions]
+[![Coverage][Coverage Badge]][Coverage]
 
+> *Decorated functions as entry points.*
+
+In python, an *entry point* can be thought of as an explicit function
+that gets called when the script is run directly from the console.
+
+Defining an entry point requires some boilerplate code, which is
+abstracted away by this library.
+
+## Installing
+
+**Python 3.7 or above is required.**
+
+### pip
+
+Installing the library with `pip` is quite simple:
+
+```console
+$ pip install entrypoint
+```
+
+Alternatively, the library can be installed from source:
+
+```console
+$ git clone https://github.com/nekitdev/entrypoint.git
+$ cd entrypoint
+$ python -m pip install .
+```
+
+### poetry
+
+You can add `entrypoint` as a dependency with the following command:
+
+```console
+$ poetry add entrypoint
+```
+
+Or by directly specifying it in the configuration like so:
+
+```toml
+[tool.poetry.dependencies]
+entrypoint = "^1.4.0"
+```
+
+Alternatively, you can add it directly from the source:
+
+```toml
+[tool.poetry.dependencies.entrypoint]
+git = "https://github.com/nekitdev/entrypoint.git"
+```
+
+## Examples
+
+### Decorated
+
+Declare the `main` function as an *entry point*:
+
+```python
+from entrypoint import entrypoint
+
+@entrypoint(__name__)
+def main() -> None:
+    print("Hello, world!")
+```
+
+Run the script directly from the console:
+
+```console
+$ python file.py
+Hello, world!
+```
+
+When importing the module, `main` does not get called:
+
+```python
+>>> import file
+>>> # no output
+```
+
+### Note
+
+Note that `main` gets called **immediately, before any code below can be executed**.
+
+```python
+@entrypoint(__name__)
+def main() -> None:
+    print("-> in main")
+
+print("<- outside")
+```
+
+```console
+$ python note.py
+-> in main
+<- outside
+```
+
+### Direct
+
+It is possible to run `main` directly:
+
+```python
+entrypoint(__name__).call(main)
+```
+
+This method allows to take control over where and when the function gets called.
+
+### Check
+
+`entrypoint` also provides `is_main` function that resembles
+the common (and de-facto standard) way of implementing *entry points*:
+
+```python
+from entrypoint import is_main
+
+if is_main(__name__):
+    print("Hello, world!")
+```
+
+### Return
+
+`entrypoint` expects `main` functions to not return anything. Even though this is *not* checked
+at *runtime*, returning from `main` will cause *type-checkers* to *error*!
+
+### Async
+
+`entrypoint` does not provide any specific functionality to run async functions.
+
+Instead, you can specify, for example, a `main` function that runs its `async_main` counterpart:
+
+```python
+from async_extensions import run
+
+async def async_main() -> None:
+    print("Hello, world!")
+
+@entrypoint(__name__)
+def main() -> None:
+    run(async_main())
+```
+
+## Documentation
+
+You can find the documentation [here][Documentation].
+
+## Support
+
+If you need support with the library, you can send an [email][Email]
+or refer to the official [Discord server][Discord].
+
+## Changelog
+
+You can find the changelog [here][Changelog].
+
+## Security Policy
+
+You can find the Security Policy of `entrypoint` [here][Security].
+
+## Contributing
+
+If you are interested in contributing to `entrypoint`, make sure to take a look at the
+[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].
+
+## License
+
+`entrypoint` is licensed under the MIT License terms. See [License][License] for details.
+
+[Email]: mailto:support@nekit.dev
+
+[Discord]: https://nekit.dev/discord
+
+[Actions]: https://github.com/nekitdev/entrypoint/actions
+
+[Changelog]: https://github.com/nekitdev/entrypoint/blob/main/CHANGELOG.md
+[Code of Conduct]: https://github.com/nekitdev/entrypoint/blob/main/CODE_OF_CONDUCT.md
+[Contributing Guide]: https://github.com/nekitdev/entrypoint/blob/main/CONTRIBUTING.md
+[Security]: https://github.com/nekitdev/entrypoint/blob/main/SECURITY.md
+
+[License]: https://github.com/nekitdev/entrypoint/blob/main/LICENSE
+
+[Package]: https://pypi.org/project/entrypoint
+[Coverage]: https://codecov.io/gh/nekitdev/entrypoint
+[Documentation]: https://nekitdev.github.io/entrypoint
+
+[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2
+[License Badge]: https://img.shields.io/pypi/l/entrypoint
+[Version Badge]: https://img.shields.io/pypi/v/entrypoint
+[Downloads Badge]: https://img.shields.io/pypi/dm/entrypoint
+
+[Documentation Badge]: https://github.com/nekitdev/entrypoint/workflows/docs/badge.svg
+[Check Badge]: https://github.com/nekitdev/entrypoint/workflows/check/badge.svg
+[Test Badge]: https://github.com/nekitdev/entrypoint/workflows/test/badge.svg
+[Coverage Badge]: https://codecov.io/gh/nekitdev/entrypoint/branch/main/graph/badge.svg
 
-setup(**setup_kwargs)
```

