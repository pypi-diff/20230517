# Comparing `tmp/versions-1.3.0.tar.gz` & `tmp/versions-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versions-1.3.0.tar", max compression
+gzip compressed data, was "versions-1.4.0.tar", max compression
```

## Comparing `versions-1.3.0.tar` & `versions-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
--rw-r--r--   0        0        0     1092 2022-10-24 18:56:28.997090 versions-1.3.0/LICENSE
--rw-r--r--   0        0        0     4634 2022-10-24 18:56:28.997090 versions-1.3.0/README.md
--rw-r--r--   0        0        0     3000 2022-10-24 18:56:28.997090 versions-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2986 2022-10-24 18:56:28.997090 versions-1.3.0/versions/__init__.py
--rw-r--r--   0        0        0     2609 2022-10-24 18:56:28.997090 versions-1.3.0/versions/constants.py
--rw-r--r--   0        0        0     4663 2022-10-24 18:56:28.997090 versions-1.3.0/versions/converters.py
--rw-r--r--   0        0        0      519 2022-10-24 18:56:28.997090 versions-1.3.0/versions/errors.py
--rw-r--r--   0        0        0     1880 2022-10-24 18:56:28.997090 versions-1.3.0/versions/functions.py
--rw-r--r--   0        0        0     1032 2022-10-24 18:56:28.997090 versions-1.3.0/versions/meta.py
--rw-r--r--   0        0        0    24008 2022-10-24 18:56:28.997090 versions-1.3.0/versions/operators.py
--rw-r--r--   0        0        0     8238 2022-10-24 18:56:28.997090 versions-1.3.0/versions/parsers.py
--rw-r--r--   0        0        0     7821 2022-10-24 18:56:28.997090 versions-1.3.0/versions/patterns.py
--rw-r--r--   0        0        0     2602 2022-10-24 18:56:28.997090 versions-1.3.0/versions/phases.py
--rw-r--r--   0        0        0        0 2022-10-24 18:56:28.997090 versions-1.3.0/versions/py.typed
--rw-r--r--   0        0        0      450 2022-10-24 18:56:28.997090 versions-1.3.0/versions/representation.py
--rw-r--r--   0        0        0    21791 2022-10-24 18:56:28.997090 versions-1.3.0/versions/segments.py
--rw-r--r--   0        0        0      693 2022-10-24 18:56:29.001090 versions-1.3.0/versions/specification.py
--rw-r--r--   0        0        0     7519 2022-10-24 18:56:29.001090 versions-1.3.0/versions/specifiers.py
--rw-r--r--   0        0        0     3594 2022-10-24 18:56:29.001090 versions-1.3.0/versions/string.py
--rw-r--r--   0        0        0     6324 2022-10-24 18:56:29.001090 versions-1.3.0/versions/types.py
--rw-r--r--   0        0        0      956 2022-10-24 18:56:29.001090 versions-1.3.0/versions/typing.py
--rw-r--r--   0        0        0     1352 2022-10-24 18:56:29.001090 versions-1.3.0/versions/utils.py
--rw-r--r--   0        0        0    25266 2022-10-24 18:56:29.001090 versions-1.3.0/versions/version.py
--rw-r--r--   0        0        0    40407 2022-10-24 18:56:29.001090 versions-1.3.0/versions/version_sets.py
--rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 versions-1.3.0/setup.py
--rw-r--r--   0        0        0     5837 1970-01-01 00:00:00.000000 versions-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-17 21:34:32.173164 versions-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5452 2023-05-17 21:34:32.173164 versions-1.4.0/README.md
+-rw-r--r--   0        0        0     3445 2023-05-17 21:34:32.173164 versions-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3488 2023-05-17 21:34:32.173164 versions-1.4.0/versions/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-17 21:34:32.173164 versions-1.4.0/versions/__main__.py
+-rw-r--r--   0        0        0     2715 2023-05-17 21:34:32.173164 versions-1.4.0/versions/constants.py
+-rw-r--r--   0        0        0      607 2023-05-17 21:34:32.173164 versions-1.4.0/versions/converters.py
+-rw-r--r--   0        0        0     3473 2023-05-17 21:34:32.173164 versions-1.4.0/versions/converters_modern.py
+-rw-r--r--   0        0        0     3466 2023-05-17 21:34:32.173164 versions-1.4.0/versions/converters_normal.py
+-rw-r--r--   0        0        0     2267 2023-05-17 21:34:32.173164 versions-1.4.0/versions/converters_utils.py
+-rw-r--r--   0        0        0      520 2023-05-17 21:34:32.173164 versions-1.4.0/versions/errors.py
+-rw-r--r--   0        0        0     1934 2023-05-17 21:34:32.173164 versions-1.4.0/versions/functions.py
+-rw-r--r--   0        0        0      709 2023-05-17 21:34:32.173164 versions-1.4.0/versions/main.py
+-rw-r--r--   0        0        0     1032 2023-05-17 21:34:32.173164 versions-1.4.0/versions/meta.py
+-rw-r--r--   0        0        0    28284 2023-05-17 21:34:32.173164 versions-1.4.0/versions/operators.py
+-rw-r--r--   0        0        0     7989 2023-05-17 21:34:32.173164 versions-1.4.0/versions/parsers.py
+-rw-r--r--   0        0        0     7816 2023-05-17 21:34:32.173164 versions-1.4.0/versions/patterns.py
+-rw-r--r--   0        0        0     2602 2023-05-17 21:34:32.173164 versions-1.4.0/versions/phases.py
+-rw-r--r--   0        0        0        0 2023-05-17 21:34:32.173164 versions-1.4.0/versions/py.typed
+-rw-r--r--   0        0        0      429 2023-05-17 21:34:32.173164 versions-1.4.0/versions/representation.py
+-rw-r--r--   0        0        0    21915 2023-05-17 21:34:32.173164 versions-1.4.0/versions/segments.py
+-rw-r--r--   0        0        0     1008 2023-05-17 21:34:32.173164 versions-1.4.0/versions/specification.py
+-rw-r--r--   0        0        0     7561 2023-05-17 21:34:32.173164 versions-1.4.0/versions/specifiers.py
+-rw-r--r--   0        0        0     3656 2023-05-17 21:34:32.173164 versions-1.4.0/versions/string.py
+-rw-r--r--   0        0        0     3076 2023-05-17 21:34:32.173164 versions-1.4.0/versions/types.py
+-rw-r--r--   0        0        0      704 2023-05-17 21:34:32.177164 versions-1.4.0/versions/typing.py
+-rw-r--r--   0        0        0     1288 2023-05-17 21:34:32.177164 versions-1.4.0/versions/utils.py
+-rw-r--r--   0        0        0    27967 2023-05-17 21:34:32.177164 versions-1.4.0/versions/version.py
+-rw-r--r--   0        0        0    40693 2023-05-17 21:34:32.177164 versions-1.4.0/versions/version_sets.py
+-rw-r--r--   0        0        0     2655 2023-05-17 21:34:32.177164 versions-1.4.0/versions/versioned.py
+-rw-r--r--   0        0        0     6788 1970-01-01 00:00:00.000000 versions-1.4.0/PKG-INFO
```

### Comparing `versions-1.3.0/LICENSE` & `versions-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `versions-1.3.0/README.md` & `versions-1.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add versions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-versions = "^1.3.0"
+versions = "^1.4.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.versions]
 git = "https://github.com/nekitdev/versions.git"
@@ -108,32 +108,57 @@
 True
 ```
 
 ### Specification
 
 `versions` also supports specifying version requirements and matching version against them.
 
-Since versions support total ordering, they can be checked using version sets
+Since versions support total ordering, they can be checked using *version sets*
 (via [`parse_version_set`][versions.functions.parse_version_set]):
 
 ```python
 >>> from versions import parse_version, parse_version_set
 >>> version_set = parse_version_set("^1.0.0")
 >>> version_set
 <VersionRange (>= 1.0.0, < 2.0.0)>
 >>> version = parse_version("1.3.0")
->>> version
-<Version (1.3.0)>
 >>> version.matches(version_set)
 True
 >>> another = parse_version("2.2.0")
 >>> another.matches(version_set)
 False
 ```
 
+Alternatively, one can use *specifiers*, which are similar to version sets, except they retain
+the structure of specifications given (via [`parse_specifier`][versions.functions.parse_specifier]):
+
+```python
+>>> from versions import parse_specifier, parse_version
+>>> specifier = parse_specifier("^1.0.0")
+>>> specifier
+<SpecifierOne (^1.0.0)>
+>>> version = parse_version("1.3.0")
+>>> version.matches(specifier)
+True
+>>> another = parse_version("2.2.0")
+>>> another.matches(specifier)
+False
+```
+
+## Versioned
+
+`versions` allows users to access versions of items that have the `__version__` attribute:
+
+```python
+>>> from versions import get_version
+>>> import versions
+>>> get_version(versions)
+<Version (1.4.0)>
+```
+
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
 
 If you need support with the library, you can send an [email][Email]
@@ -179,9 +204,10 @@
 [Downloads Badge]: https://img.shields.io/pypi/dm/versions
 
 [Documentation Badge]: https://github.com/nekitdev/versions/workflows/docs/badge.svg
 [Check Badge]: https://github.com/nekitdev/versions/workflows/check/badge.svg
 [Test Badge]: https://github.com/nekitdev/versions/workflows/test/badge.svg
 [Coverage Badge]: https://codecov.io/gh/nekitdev/versions/branch/main/graph/badge.svg
 
+[versions.functions.parse_specifier]: https://nekitdev.github.io/versions/reference/functions#versions.functions.parse_specifier
 [versions.functions.parse_version]: https://nekitdev.github.io/versions/reference/functions#versions.functions.parse_version
 [versions.functions.parse_version_set]: https://nekitdev.github.io/versions/reference/functions#versions.functions.parse_version_set
```

### Comparing `versions-1.3.0/pyproject.toml` & `versions-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "versions"
-version = "1.3.0"
+version = "1.4.0"
 description = "Parsing, inspecting and specifying versions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/versions"
@@ -28,77 +28,98 @@
 
 [[tool.poetry.packages]]
 include = "versions"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
-attrs = ">= 22.1.0"
-typing-extensions = ">= 4.3.0"
+attrs = ">= 23.1.0"
+typing-extensions = ">= 4.5.0"
+
+click = ">= 8.1.3"
+
+orderings = ">= 1.1.0"
+solus = ">= 1.1.0"
+entrypoint = ">= 1.4.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.8.0"
+black = "23.3.0"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.10.1"
-python = "^3.7"
+version = "5.12.0"
+python = ">= 3.8"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "0.971"
+mypy = "1.3.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
 
-hypothesis = "6.54.6"
+hypothesis = "6.75.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.1"
-mkdocs-material = "8.5.3"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.13"
 
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
+ignore = [
+    "E402",  # module level import not at top of file (circular import fixes)
+]
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--cov versions"
 testpaths = ["tests"]
 
 [tool.coverage.run]
 source = ["versions"]
+omit = ["versions/main.py", "versions/__main__.py"]
 
 [tool.coverage.report]
 ignore_errors = true
 exclude_lines = [
     "pragma: never",
     "pragma: no cover",
     "if TYPE_CHECKING",
     "@overload",
     "@abstractmethod",
     "raise NotImplementedError",
     "raise AssertionError",
+    "raise InternalError",
     "def __repr__",
 ]
 
 [tool.coverage.html]
 directory = "coverage"
 
 [tool.mypy]
@@ -124,15 +145,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "versions"
-version = "1.3.0"
+version = "1.4.0"
 url = "https://github.com/nekitdev/versions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
@@ -141,9 +162,9 @@
 bullet = "-"
 wrap = true
 wrap_size = 100
 
 display = ["feature", "change", "fix", "security", "deprecation", "removal", "internal"]
 
 [build-system]
-requires = ["poetry-core >= 1.3.2"]
+requires = ["poetry-core >= 1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `versions-1.3.0/versions/__init__.py` & `versions-1.4.0/versions/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Parsing, inspecting and specifying versions.
 
 ## Example
 
 ```python
->>> from versions import parse_version, parse_version_set
+>>> from versions import parse_specifier, parse_version, parse_version_set
 >>> version = parse_version("1.0.0")
 >>> version
 <Version (1.0.0)>
+>>> specifier = parse_specifier("^1.0.0")
+>>> specifier
+<SpecifierOne (^1.0.0)>
+>>> assert version.matches(specifier)
 >>> version_set = parse_version_set("^1.0.0")
 >>> version_set
 <VersionRange (>= 1.0.0, < 2.0.0)>
 >>> assert version.matches(version_set)
 ```
 """
 
@@ -32,42 +36,53 @@
 from versions.errors import ParseError, ParseSpecificationError, ParseVersionError
 from versions.functions import parse_specifier, parse_version, parse_version_set
 from versions.meta import python_version_info, version_info
 from versions.operators import Operator, OperatorType
 from versions.segments import DevTag, Epoch, Local, PostTag, PreTag, Release, Tag
 from versions.specification import Specification
 from versions.specifiers import (
+    ALWAYS,
+    NEVER,
     Specifier,
     SpecifierAll,
+    SpecifierAlways,
     SpecifierAny,
-    SpecifierFalse,
-    SpecifierSingle,
-    SpecifierTrue,
+    SpecifierNever,
+    SpecifierOne,
     is_specifier,
     is_specifier_all,
+    is_specifier_always,
     is_specifier_any,
-    is_specifier_false,
-    is_specifier_single,
-    is_specifier_true,
+    is_specifier_never,
+    is_specifier_one,
 )
 from versions.version import Version
 from versions.version_sets import (
+    EMPTY_SET,
+    UNIVERSAL_SET,
     VersionEmpty,
     VersionItem,
     VersionPoint,
     VersionRange,
     VersionSet,
     VersionUnion,
     is_version_empty,
     is_version_item,
     is_version_point,
     is_version_range,
     is_version_set,
     is_version_union,
 )
+from versions.versioned import (
+    Versioned,
+    get_version,
+    get_version_unchecked,
+    has_version,
+    is_versioned,
+)
 
 __all__ = (
     # versions
     "Version",
     # segments
     "Epoch",
     "Release",
@@ -78,28 +93,32 @@
     "Local",
     # operators
     "Operator",
     "OperatorType",
     # specification
     "Specification",
     # specifiers
+    "NEVER",
+    "ALWAYS",
     "Specifier",
-    "SpecifierFalse",
-    "SpecifierTrue",
-    "SpecifierSingle",
+    "SpecifierNever",
+    "SpecifierAlways",
+    "SpecifierOne",
     "SpecifierAll",
     "SpecifierAny",
     # specifiers type guards
     "is_specifier",
-    "is_specifier_false",
-    "is_specifier_true",
-    "is_specifier_single",
+    "is_specifier_never",
+    "is_specifier_always",
+    "is_specifier_one",
     "is_specifier_all",
     "is_specifier_any",
     # version sets
+    "EMPTY_SET",
+    "UNIVERSAL_SET",
     "VersionEmpty",
     "VersionPoint",
     "VersionRange",
     "VersionUnion",
     "VersionItem",
     "VersionSet",
     # version sets type guards
@@ -122,8 +141,14 @@
     # functions
     "parse_specifier",
     "parse_version",
     "parse_version_set",
     # meta
     "version_info",
     "python_version_info",
+    # versioned
+    "Versioned",
+    "is_versioned",
+    "has_version",
+    "get_version",
+    "get_version_unchecked",
 )
```

### Comparing `versions-1.3.0/versions/constants.py` & `versions-1.4.0/versions/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from versions.utils import unary_tuple
+
 __all__ = (
     # release constants
     "ALPHA",
     "A_LITERAL",
     "BETA",
     "B_LITERAL",
     "CANDIDATE",
@@ -72,42 +74,42 @@
 
 # candidate release
 CANDIDATE = "candidate"
 C_LITERAL = "c"
 
 RC = "rc"  # preferred
 
-# preview release
+# preview (post) release
 PREVIEW = "preview"
 PRE = "pre"
 
 # post release
 POST = "post"
 
-# revision release
+# revision (post) release
 REV = "rev"
 R_LITERAL = "r"
 
 # development release
 DEV = "dev"
 
-# phases
+# phases (in order of precedence, used in patterns)
 PRE_PHASES = (ALPHA, BETA, A_LITERAL, B_LITERAL, C_LITERAL, RC, PREVIEW, PRE)
 POST_PHASES = (POST, REV, R_LITERAL)
-DEV_PHASES = (DEV,)
+DEV_PHASES = unary_tuple(DEV)
 
 # empty and space strings
 EMPTY = str()
 SPACE = " "
 
 # zero string
 ZERO = "0"
 
 # empty and universe
-EMPTY_VERSION = "∅"
+EMPTY_VERSION = ZERO
 UNIVERSE_VERSION = "*"
 
 # some punctuation
 COMMA = ","
 DASH = "-"
 DOT = "."
 EXCLAMATION = "!"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `versions-1.3.0/versions/errors.py` & `versions-1.4.0/versions/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 
 class ParseVersionError(ParseError):
     """Parsing a version has failed."""
 
 
 class InternalError(RuntimeError):
-    """An internal error has occured."""
+    """An internal error has occurred."""
```

### Comparing `versions-1.3.0/versions/functions.py` & `versions-1.4.0/versions/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Type, TypeVar, overload
 
 from versions.parsers import SpecifierParser, VersionParser, VersionSetParser
+from versions.utils import cache
 from versions.version import Version
 
 if TYPE_CHECKING:
     from versions.specifiers import Specifier
     from versions.version_sets import VersionSet
 
 __all__ = ("parse_version", "parse_specifier", "parse_version_set")
@@ -20,40 +21,43 @@
 
 
 @overload
 def parse_version(string: str, version_type: Type[V]) -> V:
     ...
 
 
+@cache
 def parse_version(string: str, version_type: Type[Version] = Version) -> Version:
     """Parses a `string` into a version of `version_type`.
 
     Arguments:
         string: The string to parse.
         version_type: The version type to use in conversion.
 
     Returns:
         The newly parsed [`Version`][versions.version.Version].
     """
     return VersionParser(version_type).parse(string)
 
 
+@cache
 def parse_specifier(string: str, version_type: Type[Version] = Version) -> Specifier:
     """Parses a `string` into a version specifier with versions of `version_type`.
 
     Arguments:
         string: The string to parse.
         version_type: The version type to use in conversion.
 
     Returns:
         The newly parsed [`Specifier`][versions.specifiers.Specifier].
     """
     return SpecifierParser(VersionParser(version_type)).parse(string)
 
 
+@cache
 def parse_version_set(string: str, version_type: Type[Version] = Version) -> VersionSet:
     """Parses a `string` into a version set with versions of `version_type`.
 
     Arguments:
         string: The string to parse.
         version_type: The version type to use in conversion.
```

### Comparing `versions-1.3.0/versions/meta.py` & `versions-1.4.0/versions/meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 
 if python_phase == FINAL:  # pragma: no cover
     python_version_info = Version.from_parts(python_major, python_minor, python_micro)
     """The python version represented as a [`Version`][versions.version.Version]."""
 
 else:  # pragma: no cover
     python_version_info = Version.from_parts(
-        python_major, python_minor, python_micro, pre=PreTag(python_phase, python_value).normalize()
-    )
+        python_major, python_minor, python_micro, pre=PreTag(python_phase, python_value)
+    ).normalize()
     """The python version represented as a [`Version`][versions.version.Version]."""
```

### Comparing `versions-1.3.0/versions/operators.py` & `versions-1.4.0/versions/operators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Mapping, Optional, Tuple, TypeVar, Union
+from string import digits
+from typing import TYPE_CHECKING, Any, Mapping, Optional, Tuple, Type, TypeVar, Union
 
 from attrs import frozen
 
 from versions.constants import (
     CARET,
-    DOT,
     DOUBLE_EQUAL,
     EQUAL,
     GREATER,
     GREATER_OR_EQUAL,
     LESS,
     LESS_OR_EQUAL,
     NOT_EQUAL,
@@ -20,15 +20,15 @@
     TILDE_EQUAL,
     WILDCARD_DOUBLE_EQUAL,
     WILDCARD_EQUAL,
     WILDCARD_NOT_EQUAL,
 )
 from versions.errors import InternalError
 from versions.representation import Representation
-from versions.string import ToString, concat_dot_args, concat_empty_args, concat_space_args
+from versions.string import ToString, concat_empty_args, concat_space_args
 from versions.typing import Binary, Unary, is_same_type
 
 if TYPE_CHECKING:
     from versions.version import Version
     from versions.version_sets import VersionSet
 
     Matches = Binary[Version, Version, bool]
@@ -47,47 +47,45 @@
     "matches_not_equal",
     "matches_less",
     "matches_less_or_equal",
     "matches_greater",
     "matches_greater_or_equal",
     "matches_wildcard_equal",
     "matches_wildcard_not_equal",
-    # translating versions to constraints
+    # translating versions to version sets
     "translate_caret",
     "translate_tilde",
     "translate_tilde_equal",
     "translate_equal",
     "translate_not_equal",
     "translate_less",
     "translate_less_or_equal",
     "translate_greater",
     "translate_greater_or_equal",
     "translate_wildcard_equal",
     "translate_wildcard_not_equal",
-    # get next breaking versions of different types
+    # fetching next breaking versions of different types
     "next_caret_breaking",
     "next_tilde_breaking",
     "next_tilde_equal_breaking",
     "next_wildcard_breaking",
+    # partial matches
+    "partial_matches",
     # operators
     "Operator",
     "OperatorType",
-    # types that represent functions and their signatures
-    "Matches",
-    "PartialMatches",
-    "Translate",
 )
 
 V = TypeVar("V", bound="Version")
 
 
 def next_caret_breaking(version: V) -> V:
     """Returns the next breaking version according to the *caret* (`^`) strategy.
 
-    This function is slightly convoluted due to handling `0.x.y` versions.
+    This function is slightly convoluted due to handling `0.x.y` and `0.0.z` versions.
 
     See [`next_breaking`][versions.version.Version.next_breaking] for more information.
 
     Example:
         ```python
         >>> from versions import next_caret_breaking, parse_version
         >>> version = parse_version("1.0.0")
@@ -230,17 +228,15 @@
 
         index -= 1
 
     return version.next_at(index)  # this will take care of unstable releases
 
 
 def wildcard_string(string: str, wildcard: str = STAR) -> str:
-    string, _dot, _last = string.rpartition(DOT)
-
-    return concat_dot_args(string, wildcard)
+    return concat_empty_args(string.rstrip(digits), wildcard)
 
 
 def wildcard_type(string: str, wildcard: str = STAR) -> str:
     return string.strip(wildcard)
 
 
 def partial_matches(matches: Matches, against: Version) -> PartialMatches:
@@ -304,15 +300,15 @@
     Returns:
         Whether the `version` matches `against`.
     """
     return against <= version < next_tilde_breaking(against)
 
 
 def matches_equal(version: Version, against: Version) -> bool:
-    """Checks if the `version` matches the *equal* (`==`) specification.
+    """Checks if the `version` matches the *equal* (`=`) specification.
 
     This is equivalent to:
 
     ```python
     version == against
     ```
 
@@ -419,15 +415,15 @@
     Returns:
         Whether the `version` matches `against`.
     """
     return version >= against
 
 
 def matches_wildcard_equal(version: Version, against: Version) -> bool:
-    """Checks if the `version` matches the *wildcard-equal* (`== *`) specification.
+    """Checks if the `version` matches the *wildcard-equal* (`=*`) specification.
 
     This is equivalent to:
 
     ```python
     wildcard = next_wildcard_breaking(against)
 
     wildcard is None or against <= version < wildcard
@@ -445,15 +441,15 @@
     if wildcard is None:
         return True
 
     return against <= version < wildcard
 
 
 def matches_wildcard_not_equal(version: Version, against: Version) -> bool:
-    """Checks if the `version` matches the *wildcard-not-equal* (`!= *`) specification.
+    """Checks if the `version` matches the *wildcard-not-equal* (`!=*`) specification.
 
     This is equivalent to:
 
     ```python
     wildcard = next_wildcard_breaking(against)
 
     wildcard is not None and (version < against or version >= wildcard)
@@ -523,17 +519,17 @@
         max=next_tilde_breaking(version),
         include_min=True,
         include_max=False,
     )
 
 
 def translate_equal(version: Version) -> VersionPoint:
-    """Translates the `version` into a version set according to the *equal* (`==`) strategy.
+    """Translates the `version` into a version set according to the *equal* (`=`) strategy.
 
-    This function returns the `[version, version]` range (aka `version` point).
+    This function returns the `[version, version]` range (aka single `version`, `{version}`).
 
     Arguments:
         version: The version to translate.
 
     Returns:
         The version set representing the *equal* specification.
     """
@@ -617,15 +613,15 @@
         The version set representing the *greater-or-equal* specification.
     """
     return VersionRange(min=version, include_min=True)
 
 
 def translate_wildcard_equal(version: Version) -> VersionRange:
     """Translates the `version` into a version set according to
-    the *wildcard-equal* (`== *`) strategy.
+    the *wildcard-equal* (`==*`) strategy.
 
     This function returns the `[version, next_wildcard_version(version))` range in most cases,
     except for when the version is `*`; then the `(ε, ω)` range is returned.
 
     Arguments:
         version: The version to translate.
 
@@ -641,15 +637,15 @@
 
 
 UNEXPECTED_WILDCARD_EQUAL_COMPLEMENT = "unexpected wildcard-equal complement"
 
 
 def translate_wildcard_not_equal(version: Version) -> Union[VersionEmpty, VersionUnion]:
     """Translates the `version` into a version set according to
-    the *wildcard-not-equal* (`!= *`) strategy.
+    the *wildcard-not-equal* (`!=*`) strategy.
 
     This function returns the `(ε, version) | (next_wildcard_breaking(version), ω)` union
     in most cases, except for when the version is `*`; then the `{}` empty set is returned.
 
     Arguments:
         version: The version to translate.
 
@@ -693,54 +689,97 @@
     WILDCARD_DOUBLE_EQUAL = WILDCARD_DOUBLE_EQUAL
     """The wildcard binary `==*` operator."""
     WILDCARD_EQUAL = WILDCARD_EQUAL
     """The wildcard binary `=*` operator."""
     WILDCARD_NOT_EQUAL = WILDCARD_NOT_EQUAL
     """The wildcard binary `!=*` operator."""
 
+    def is_tilde_equal(self) -> bool:
+        return self is type(self).TILDE_EQUAL
+
+    def is_double_equal(self) -> bool:
+        return self is type(self).DOUBLE_EQUAL
+
+    def is_not_equal(self) -> bool:
+        return self is type(self).NOT_EQUAL
+
+    def is_less(self) -> bool:
+        return self is type(self).LESS
+
+    def is_less_or_equal(self) -> bool:
+        return self is type(self).LESS_OR_EQUAL
+
+    def is_greater(self) -> bool:
+        return self is type(self).GREATER
+
+    def is_greater_or_equal(self) -> bool:
+        return self is type(self).GREATER_OR_EQUAL
+
+    def is_caret(self) -> bool:
+        return self is type(self).CARET
+
+    def is_equal(self) -> bool:
+        return self is type(self).EQUAL
+
+    def is_tilde(self) -> bool:
+        return self is type(self).TILDE
+
+    def is_wildcard_double_equal(self) -> bool:
+        return self is type(self).WILDCARD_DOUBLE_EQUAL
+
+    def is_wildcard_equal(self) -> bool:
+        return self is type(self).WILDCARD_EQUAL
+
+    def is_wildcard_not_equal(self) -> bool:
+        return self is type(self).WILDCARD_NOT_EQUAL
+
     def is_wildcard(self) -> bool:
         """Checks if an operator is *wildcard*.
 
         Returns:
             Whether the operator is *wildcard*.
         """
         return self in WILDCARD
 
-    def is_equals(self) -> bool:
-        """Checks if an operator is *equals*.
-
-        Returns:
-            Whether the operator is *equals*.
-        """
+    def in_equals(self) -> bool:
         return self in EQUALS
 
+    def in_wildcard_equals(self) -> bool:
+        return self in WILDCARD_EQUALS
+
     def is_unary(self) -> bool:
         """Checks if an operator is *unary*.
 
         Returns:
             Whether the operator is *unary*.
         """
         return self in UNARY
 
     def __eq__(self, other: Any) -> bool:
         if is_same_type(other, self):
-            return (self.is_equals() and other.is_equals()) or super().__eq__(other)
+            return (
+                (self.in_equals() and other.in_equals())
+                or (self.in_wildcard_equals() and other.in_wildcard_equals())
+                or super().__eq__(other)
+            )
 
-        return NotImplemented
+        return NotImplemented  # pragma: no cover  # not tested
 
     def __hash__(self) -> int:
         return super().__hash__()  # type: ignore
 
     @property
     def string(self) -> str:
         return wildcard_type(self.value)
 
 
 EQUALS = {OperatorType.DOUBLE_EQUAL, OperatorType.EQUAL}
 
+WILDCARD_EQUALS = {OperatorType.WILDCARD_DOUBLE_EQUAL, OperatorType.WILDCARD_EQUAL}
+
 UNARY = {OperatorType.CARET, OperatorType.TILDE}
 
 WILDCARD = {
     OperatorType.WILDCARD_DOUBLE_EQUAL,
     OperatorType.WILDCARD_EQUAL,
     OperatorType.WILDCARD_NOT_EQUAL,
 }
@@ -757,25 +796,73 @@
     OperatorType.EQUAL: (matches_equal, translate_equal),
     OperatorType.TILDE: (matches_tilde, translate_tilde),
     OperatorType.WILDCARD_DOUBLE_EQUAL: (matches_wildcard_equal, translate_wildcard_equal),
     OperatorType.WILDCARD_EQUAL: (matches_wildcard_equal, translate_wildcard_equal),
     OperatorType.WILDCARD_NOT_EQUAL: (matches_wildcard_not_equal, translate_wildcard_not_equal),
 }
 
+O = TypeVar("O", bound="Operator")
+
 
 @frozen(repr=False)
 class Operator(Representation, ToString):
     """Represents operators."""
 
     type: OperatorType
     """The operator type."""
 
     version: Version
     """The operator version."""
 
+    def validate(self) -> None:
+        if self.type.is_tilde_equal():
+            if not self.version.last_index:
+                raise ValueError(CAN_NOT_USE_TILDE_EQUAL)
+
+    __attrs_post_init__ = validate
+
+    def is_tilde_equal(self) -> bool:
+        return self.type.is_tilde_equal()
+
+    def is_double_equal(self) -> bool:
+        return self.type.is_double_equal()
+
+    def is_not_equal(self) -> bool:
+        return self.type.is_not_equal()
+
+    def is_less(self) -> bool:
+        return self.type.is_less()
+
+    def is_less_or_equal(self) -> bool:
+        return self.type.is_less_or_equal()
+
+    def is_greater(self) -> bool:
+        return self.type.is_greater()
+
+    def is_greater_or_equal(self) -> bool:
+        return self.type.is_greater_or_equal()
+
+    def is_caret(self) -> bool:
+        return self.type.is_caret()
+
+    def is_equal(self) -> bool:
+        return self.type.is_equal()
+
+    def is_tilde(self) -> bool:
+        return self.type.is_tilde()
+
+    def is_wildcard_double_equal(self) -> bool:
+        return self.type.is_wildcard_double_equal()
+
+    def is_wildcard_equal(self) -> bool:
+        return self.type.is_wildcard_equal()
+
+    def is_wildcard_not_equal(self) -> bool:
+        return self.type.is_wildcard_not_equal()
+
     def is_unary(self) -> bool:
         """Checks if an operator is *unary*.
 
         Returns:
             Whether the operator is *unary*.
         """
         return self.type.is_unary()
@@ -784,14 +871,66 @@
         """Checks if an operator is *wildcard*.
 
         Returns:
             Whether the operator is *wildcard*.
         """
         return self.type.is_wildcard()
 
+    @classmethod
+    def tilde_equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.TILDE_EQUAL, version)
+
+    @classmethod
+    def double_equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.DOUBLE_EQUAL, version)
+
+    @classmethod
+    def not_equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.NOT_EQUAL, version)
+
+    @classmethod
+    def less(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.LESS, version)
+
+    @classmethod
+    def less_or_equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.LESS_OR_EQUAL, version)
+
+    @classmethod
+    def greater(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.GREATER, version)
+
+    @classmethod
+    def greater_or_equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.GREATER_OR_EQUAL, version)
+
+    @classmethod
+    def caret(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.CARET, version)
+
+    @classmethod
+    def equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.EQUAL, version)
+
+    @classmethod
+    def tilde(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.TILDE, version)
+
+    @classmethod
+    def wildcard_double_equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.WILDCARD_DOUBLE_EQUAL, version)
+
+    @classmethod
+    def wildcard_equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.WILDCARD_EQUAL, version)
+
+    @classmethod
+    def wildcard_not_equal(cls: Type[O], version: Version) -> O:
+        return cls(OperatorType.WILDCARD_NOT_EQUAL, version)
+
     @property
     def matches_and_translate(self) -> Tuple[Matches, Translate]:
         return OPERATOR[self.type]
 
     @property
     def matches(self) -> Matches:
         """The `matches` function representing the operator."""
@@ -804,15 +943,17 @@
         """The `translate` function representing the operator."""
         _matches, translate = self.matches_and_translate
 
         return translate
 
     @property
     def partial_matches(self) -> PartialMatches:
-        """The partial `matches` function with `self.version` as the `against` version."""
+        """The partial `matches` function with
+        [`self.version`][versions.operators.Operator.version] as the `against` version.
+        """
         return partial_matches(self.matches, self.version)
 
     def to_string(self) -> str:
         """Converts an [`Operator`][versions.operators.Operator] to its string representation.
 
         Returns:
             The operator string.
@@ -824,15 +965,16 @@
 
         if self.is_unary():
             return concat_empty_args(self.type.string, string)
 
         return concat_space_args(self.type.string, string)
 
     def to_short_string(self) -> str:
-        """Converts an [`Operator`][versions.operators.Operator] to its *short* string representation.
+        """Converts an [`Operator`][versions.operators.Operator]
+        to its *short* string representation.
 
         Returns:
             The *short* operator string.
         """
         string = self.version.to_short_string()
 
         if self.is_wildcard():
```

### Comparing `versions-1.3.0/versions/parsers.py` & `versions-1.4.0/versions/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
-from abc import abstractmethod
+from abc import abstractmethod as required
 from typing import TYPE_CHECKING, Generic, Optional, Pattern, Type, TypeVar
 
 from attrs import frozen
+from named import get_name
 from typing_extensions import Protocol, runtime_checkable
 
-from versions.constants import STAR, ZERO
+from versions.constants import STAR, X_LITERAL, ZERO
 from versions.converters import specifier_to_version_set
 from versions.errors import InternalError, ParseSpecificationError, ParseTagError, ParseVersionError
 from versions.operators import OperatorType
 from versions.patterns import (
     CARET_SPECIFICATION,
     DEV,
     EPOCH,
@@ -26,24 +27,16 @@
     TAG,
     TILDE_SPECIFICATION,
     VALUE,
     VERSION,
     VERSION_NAME,
     WILDCARD_SPECIFICATION,
 )
-from versions.specifiers import (
-    Specifier,
-    SpecifierAll,
-    SpecifierAny,
-    SpecifierFalse,
-    SpecifierSingle,
-    SpecifierTrue,
-)
+from versions.specifiers import Specifier, SpecifierAll, SpecifierAny, SpecifierOne
 from versions.string import clear_whitespace, split_comma, split_pipes
-from versions.typing import get_name
 from versions.version_sets import VersionSet
 
 if TYPE_CHECKING:
     from versions.segments import Tag
     from versions.version import Version
 
 __all__ = ("Parser", "SpecifierParser", "TagParser", "VersionParser", "VersionSetParser")
@@ -54,15 +47,15 @@
 R = TypeVar("R", covariant=True)
 
 CAN_NOT_PARSE = "can not parse `{}` to `{}`"
 
 
 @runtime_checkable
 class Parser(Protocol[R]):
-    @abstractmethod
+    @required
     def parse(self, string: str) -> R:
         raise NotImplementedError
 
 
 PHASE_IS_NONE = "the tag was matched but the `phase` is `None`"
 
 
@@ -71,20 +64,20 @@
     tag_type: Type[T]
 
     def parse(self, string: str) -> T:
         tag_type = self.tag_type
 
         match = TAG.fullmatch(string)
 
-        if match is None:  # pragma: no cover
+        if match is None:  # pragma: no cover  # not tested
             raise ParseTagError(CAN_NOT_PARSE.format(string, get_name(tag_type)))
 
         phase = match.group(PHASE)
 
-        if phase is None:  # pragma: no cover
+        if phase is None:
             raise InternalError(PHASE_IS_NONE)
 
         value_string = match.group(VALUE)
 
         if value_string is None:
             return tag_type(phase)
 
@@ -124,18 +117,20 @@
     @staticmethod
     def parse_local_optional(string: Optional[str]) -> Optional[Local]:
         return None if string is None else Local.parse(string)
 
     def parse(self, string: str) -> V:
         match = VERSION.fullmatch(string)
 
+        version_type = self.version_type
+
         if match is None:
-            raise ParseVersionError(CAN_NOT_PARSE.format(string, get_name(self.version_type)))
+            raise ParseVersionError(CAN_NOT_PARSE.format(string, get_name(version_type)))
 
-        return self.version_type(
+        return version_type(
             epoch=self.parse_epoch_optional(match.group(EPOCH)),
             release=self.parse_release_optional(match.group(RELEASE)),
             pre=self.parse_pre_optional(match.group(PRE)),
             post=(
                 self.parse_post_implicit_optional(match.group(POST_IMPLICIT))
                 or self.parse_post_optional(match.group(POST))
             ),
@@ -191,27 +186,27 @@
         match = pattern.fullmatch(string)
 
         if match is None:
             return None
 
         operator_string = match.group(OPERATOR_NAME)
 
-        if operator_string is None:  # pragma: no cover
+        if operator_string is None:
             raise InternalError(OPERATOR_IS_NONE)
 
         operator_type = OperatorType(operator_string)
 
         version_string = match.group(VERSION_NAME)
 
-        if version_string is None:  # pragma: no cover
+        if version_string is None:
             raise InternalError(VERSION_IS_NONE)
 
         version = self.version_parser.parse(version_string)
 
-        return SpecifierSingle(operator_type, version)
+        return SpecifierOne(operator_type, version)
 
     def try_parse_equal(self, string: str) -> Optional[Specifier]:
         match = EQUAL_SPECIFICATION.fullmatch(string)
 
         if match is None:
             return None
 
@@ -221,20 +216,20 @@
             operator_type = OperatorType.EQUAL
 
         else:
             operator_type = OperatorType(operator_string)
 
         version_string = match.group(VERSION_NAME)
 
-        if version_string is None:  # pragma: no cover
+        if version_string is None:
             raise InternalError(VERSION_IS_NONE)
 
         version = self.version_parser.parse(version_string)
 
-        return SpecifierSingle(operator_type, version)
+        return SpecifierOne(operator_type, version)
 
     def try_parse_wildcard(self, string: str) -> Optional[Specifier]:
         match = WILDCARD_SPECIFICATION.fullmatch(string)
 
         if match is None:
             return None
 
@@ -244,26 +239,22 @@
             operator_type = OperatorType.WILDCARD_EQUAL
 
         else:
             operator_type = OperatorType(operator_string + STAR)
 
         version_string = match.group(VERSION_NAME)
 
-        if version_string is None:  # pragma: no cover
+        if version_string is None:
             raise InternalError(VERSION_IS_NONE)
 
-        if version_string == STAR:
-            if operator_type == OperatorType.WILDCARD_NOT_EQUAL:
-                return SpecifierFalse()
-
-            return SpecifierTrue()
-
-        version = self.version_parser.parse(version_string.replace(STAR, ZERO))
+        version = self.version_parser.parse(
+            version_string.replace(X_LITERAL, STAR).replace(STAR, ZERO)
+        )
 
-        return SpecifierSingle(operator_type, version)
+        return SpecifierOne(operator_type, version)
 
 
 @frozen()
 class VersionSetParser(Generic[V], Parser[VersionSet]):
     specifier_parser: SpecifierParser[V]
 
     def parse(self, string: str) -> VersionSet:
```

### Comparing `versions-1.3.0/versions/patterns.py` & `versions-1.4.0/versions/patterns.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 # CONSTANTS
 
 ALPHA_DIGIT = r"[a-z0-9]"
 ALPHA = r"[a-z]"
 DIGIT = r"[0-9]"
 
-SEPARATOR = SET(COMBINE_ITERABLE(map(ESCAPE, SEPARATORS)))
+SEPARATOR = SET(ESCAPE(COMBINE_ITERABLE(SEPARATORS)))
 
 FLAGS = re.IGNORECASE | re.VERBOSE
 
 # VERSION PARTS
 
 EPOCH = "epoch"
```

### Comparing `versions-1.3.0/versions/phases.py` & `versions-1.4.0/versions/phases.py`

 * *Files identical despite different names*

### Comparing `versions-1.3.0/versions/segments.py` & `versions-1.4.0/versions/segments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import ClassVar, Iterable, Optional, Set, Tuple, Type, TypeVar, Union
 
 from attrs import Attribute, evolve, field, frozen
+from named import get_type_name
 
 from versions.constants import EMPTY
 from versions.parsers import TagParser
 from versions.phases import (
     PHASE_ALL_DEFAULT,
     PHASE_ALL_SET,
     PHASE_DEV_DEFAULT,
@@ -18,27 +19,25 @@
     PHASE_TO_NEXT,
     PHASE_TO_NORMAL,
     PHASE_TO_SHORT,
     SHORT_TO_PHASE,
 )
 from versions.representation import Representation
 from versions.string import (
-    FromString,
-    ToString,
-    case_fold,
+    String,
     check_int,
     concat_dot,
     concat_dot_args,
     concat_empty_args,
     split_dot,
     split_separators,
 )
 from versions.types import NegativeInfinity, negative_infinity
-from versions.typing import DynamicTuple, get_name, is_int
-from versions.utils import count_leading_zeros, evolve_in_place, fix_to_length
+from versions.typing import DynamicTuple, is_int
+from versions.utils import count_leading_zeros, fix_to_length
 
 __all__ = (
     # default values
     "DEFAULT_PARTS",
     "DEFAULT_VALUE",
     "DEFAULT_PADDING",
     # useful release indexes
@@ -59,15 +58,15 @@
     "Extra",
     "Parts",
     "LocalPart",
     "LocalParts",
     "local_part",
 )
 
-Parts = DynamicTuple[int]
+Parts = DynamicTuple[int]  # technically parts are never empty
 Extra = DynamicTuple[int]
 
 DEFAULT_PARTS = (0, 0, 0)  # makes sense as the default for semantic versions
 """The default parts of the [`Release`][versions.segments.Release]."""
 
 DEFAULT_VALUE = 0
 """The default value to use."""
@@ -82,15 +81,15 @@
 
 PATCH = MICRO  # alias
 
 E = TypeVar("E", bound="Epoch")
 
 
 @frozen(repr=False, eq=True, order=True)
-class Epoch(Representation, FromString, ToString):
+class Epoch(Representation, String):
     """Represents the *epoch* segment of the version (`e!`)."""
 
     value: int = field(default=DEFAULT_VALUE)
     """The value of the epoch."""
 
     def __bool__(self) -> bool:
         return bool(self.value)
@@ -123,44 +122,48 @@
         """Converts an [`Epoch`][versions.segments.Epoch] to its string representation.
 
         Returns:
             The epoch string.
         """
         return str(self.value)
 
+    def set_value(self: E, value: int) -> E:
+        return evolve(self, value=value)
+
+    def next_value(self: E) -> E:
+        return self.set_value(self.value + 1)
+
 
 EMPTY_RELEASE = "release can not be empty"
 
 R = TypeVar("R", bound="Release")
 
 
 @frozen(repr=False, eq=True, order=True)
-class Release(Representation, FromString, ToString):
+class Release(Representation, String):
     """Represents the *release* segment of the version (`x.y.z`)."""
 
     parts: Parts = field(default=DEFAULT_PARTS, eq=False, order=False)
     """The parts of the release."""
 
     compare_parts: Parts = field(repr=False, init=False, eq=True, order=True, hash=False)
 
     @parts.validator
     def check_parts(self, attribute: Attribute[Parts], value: Parts) -> None:
         if not value:
             raise ValueError(EMPTY_RELEASE)
 
-    def __attrs_post_init__(self) -> None:
-        evolve_in_place(self, compare_parts=self.compute_compare_parts())
-
-    def compute_compare_parts(self) -> Parts:
+    @compare_parts.default
+    def default_compare_parts(self) -> Parts:
         parts = self.parts
 
         index = count_leading_zeros(reversed(parts))
 
         if index == self.precision:
-            index -= 1
+            index -= 1  # preserve single zero if the version fully consists of zeros
 
         return self.slice_parts(-index) if index else parts
 
     @classmethod
     def create(cls: Type[R], parts: Parts = DEFAULT_PARTS) -> R:
         """Creates a [`Release`][versions.segments.Release] from `parts`.
 
@@ -200,14 +203,17 @@
         """Converts a [`Release`][versions.segments.Release] to its parts.
 
         Returns:
             The parts of the release.
         """
         return self.parts
 
+    def set_parts(self: R, *parts: int) -> R:
+        return evolve(self, parts=parts)
+
     @property
     def precision(self) -> int:
         """The count of the release parts."""
         return len(self.parts)
 
     @property
     def last_index(self) -> int:
@@ -494,19 +500,19 @@
             padding: The padding to use.
 
         Returns:
             The padded release.
         """
         return self.pad_to(self.precision + 1, padding)
 
-    def slice(self: R, stop: int) -> R:
-        return self.create(self.slice_parts(stop))
+    def slice(self: R, index: int) -> R:
+        return self.create(self.slice_parts(index))
 
-    def slice_parts(self, stop: int) -> Parts:
-        return self.parts[:stop]
+    def slice_parts(self, index: int) -> Parts:
+        return self.parts[:index]
 
     @classmethod
     def from_string(cls: Type[R], string: str) -> R:
         """Parses a [`Release`][versions.segments.Release] from `string`.
 
         Arguments:
             string: The string to parse.
@@ -527,50 +533,39 @@
 
 PHASE_NOT_ALLOWED = "phase `{}` is not allowed in `{}`"
 CAN_NOT_PARSE = "can not parse `{}` to `{}`"
 
 T = TypeVar("T", bound="Tag")
 
 
+def convert_phase(phase: str) -> str:
+    return SHORT_TO_PHASE.get(phase, phase)
+
+
 @frozen(repr=False, eq=True, order=True)
-class Tag(Representation, FromString, ToString):
+class Tag(Representation, String):
     """Represents various version *tags* (`tag.n`)."""
 
     DEFAULT_PHASE: ClassVar[str] = PHASE_ALL_DEFAULT
     PHASE_SET: ClassVar[Set[str]] = PHASE_ALL_SET
 
-    phase: str = field(converter=case_fold)  # type: ignore
+    phase: str = field(converter=convert_phase)
     """The phase of the release tag."""
 
     value: int = field(default=DEFAULT_VALUE)
     """The value of the release tag."""
 
     @phase.default
     def default_phase(self) -> str:
         return self.DEFAULT_PHASE
 
     @phase.validator
     def check_phase(self, attribute: Attribute[str], value: str) -> None:
         if value not in self.PHASE_SET:
-            raise ValueError(PHASE_NOT_ALLOWED.format(value, get_name(type(self))))
-
-    def __attrs_post_init__(self) -> None:
-        evolve_in_place(self, phase=self.expand(self.phase))
-
-    @staticmethod
-    def expand(phase: str) -> str:
-        return SHORT_TO_PHASE.get(phase, phase)
-
-    @staticmethod
-    def reduce(phase: str) -> str:
-        return PHASE_TO_SHORT.get(phase, phase)
-
-    @staticmethod
-    def normalize_phase(phase: str) -> str:
-        return PHASE_TO_NORMAL.get(phase, phase)
+            raise ValueError(PHASE_NOT_ALLOWED.format(value, get_type_name(self)))
 
     @classmethod
     def create(cls: Type[T], phase: Optional[str] = None, value: int = DEFAULT_VALUE) -> T:
         """Creates a [`Tag`][versions.segments.Tag] from `phase` and `value`.
 
         Arguments:
             phase: The phase of the tag.
@@ -594,37 +589,47 @@
         Returns:
             The newly created [`Tag`][versions.segments.Tag].
         """
         return cls(cls.DEFAULT_PHASE, value)
 
     @property
     def short(self) -> str:
-        """The *short* phase of the release."""
-        return self.reduce(self.phase)
+        """The *short* phase of the tag."""
+        phase = self.phase
+
+        return PHASE_TO_SHORT.get(phase, phase)
 
     @property
     def normal(self) -> str:
-        """The *normalized* phase of the release."""
-        return self.normalize_phase(self.phase)
+        """The *normalized* phase of the tag."""
+        phase = self.phase
+
+        return PHASE_TO_NORMAL.get(phase, phase)
 
     def normalize(self: T) -> T:
         """Normalizes the version tag.
 
         Returns:
             The normalized tag.
         """
-        return evolve(self, phase=self.normal)
+        return self.set_phase(self.normal)
+
+    def set_phase(self: T, phase: str) -> T:
+        return evolve(self, phase=phase)
+
+    def set_value(self: T, value: int) -> T:
+        return evolve(self, value=value)
 
     def next(self: T) -> T:
-        """Bumps the version tag.
+        """Bumps the version tag value.
 
         Returns:
             The next version tag.
         """
-        return evolve(self, value=self.value + 1)
+        return self.set_value(self.value + 1)
 
     def next_phase(self: T) -> Optional[T]:
         """Bumps the version tag phase, if possible.
 
         Returns:
             The next version tag, if present.
         """
@@ -682,15 +687,15 @@
     """Represents the *dev-release* tag of the version (`dev.n`)."""
 
     DEFAULT_PHASE = PHASE_DEV_DEFAULT
     PHASE_SET = PHASE_DEV_SET
 
 
 LocalPart = Union[int, str]
-LocalParts = DynamicTuple[LocalPart]
+LocalParts = DynamicTuple[LocalPart]  # technically local parts are never empty
 
 CompareLocalIntPart = Tuple[int, str]
 CompareLocalStringPart = Tuple[NegativeInfinity, str]
 
 CompareLocalPart = Union[CompareLocalIntPart, CompareLocalStringPart]
 CompareLocalParts = DynamicTuple[CompareLocalPart]
 
@@ -700,31 +705,31 @@
 
 
 def local_part(string: str) -> LocalPart:
     return int(string) if check_int(string) else string
 
 
 @frozen(repr=False, eq=True, order=True)
-class Local(Representation, FromString, ToString):
-    """Represents the *local* segment of the version (`+abcdefg.n`)"""
+class Local(Representation, String):
+    """Represents the *local* segment of the version (`+abcdef.n`)"""
 
     parts: LocalParts = field(eq=False, order=False)
     """The local segment parts."""
 
-    compare_parts: CompareLocalParts = field(repr=False, init=False, eq=True, order=True, hash=False)
+    compare_parts: CompareLocalParts = field(
+        repr=False, init=False, eq=True, order=True, hash=False
+    )
 
     @parts.validator
     def check_parts(self, attribute: Attribute[LocalParts], value: LocalParts) -> None:
         if not value:
             raise ValueError(EMPTY_LOCAL)
 
-    def __attrs_post_init__(self) -> None:
-        evolve_in_place(self, compare_parts=self.compute_compare_parts())
-
-    def compute_compare_parts(self) -> CompareLocalParts:
+    @compare_parts.default
+    def default_compare_parts(self) -> CompareLocalParts:
         empty = EMPTY
 
         return tuple(
             (part, empty) if is_int(part) else (negative_infinity, part)  # type: ignore
             for part in self.parts
         )
 
@@ -768,14 +773,17 @@
         """Converts a [`Local`][versions.segments.Local] segment to its parts.
 
         Returns:
             The parts of the local segment.
         """
         return self.parts
 
+    def set_parts(self: L, *parts: LocalPart) -> L:
+        return evolve(self, parts=parts)
+
     @classmethod
     def from_string(cls: Type[L], string: str) -> L:
         """Parses a [`Local`][versions.segments.Local] segment from `string`.
 
         Arguments:
             string: The string to parse.
```

### Comparing `versions-1.3.0/versions/specifiers.py` & `versions-1.4.0/versions/specifiers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from builtins import isinstance as is_instance
 from typing import TYPE_CHECKING, Any, ClassVar, Iterable
 
 from attrs import Attribute, field, frozen
 from typing_extensions import Literal, TypeGuard
 
 from versions.constants import EMPTY_VERSION, UNIVERSE_VERSION
 from versions.operators import Operator
@@ -14,67 +13,75 @@
     ToString,
     concat_comma,
     concat_comma_space,
     concat_pipes,
     concat_pipes_spaced,
     create_wrap_around,
 )
-from versions.typing import DynamicTuple
+from versions.typing import DynamicTuple, is_instance
 from versions.utils import contains_only_item, first
 
 if TYPE_CHECKING:
     from versions.version import Version
 
 __all__ = (
+    "NEVER",
+    "ALWAYS",
     "Specifier",
-    "SpecifierFalse",
-    "SpecifierTrue",
-    "SpecifierSingle",
+    "SpecifierNever",
+    "SpecifierAlways",
+    "SpecifierOne",
     "SpecifierAny",
     "SpecifierAll",
     "is_specifier",
-    "is_specifier_false",
-    "is_specifier_true",
-    "is_specifier_single",
+    "is_specifier_never",
+    "is_specifier_always",
+    "is_specifier_one",
     "is_specifier_any",
     "is_specifier_all",
 )
 
 
 class Specifier(Representation, ToString, Specification):
     """Represents all possible specifiers."""
 
 
 Specifiers = DynamicTuple[Specifier]
 
 
 @frozen(repr=False)
-class SpecifierFalse(Specifier):
+class SpecifierNever(Specifier):
     """Represents specifiers that do not accept any versions."""
 
     def accepts(self, version: Version) -> Literal[False]:
         return False
 
     def to_string(self) -> str:
         return EMPTY_VERSION
 
 
+NEVER = SpecifierNever()
+
+
 @frozen(repr=False)
-class SpecifierTrue(Specifier):
+class SpecifierAlways(Specifier):
     """Represents specifiers that accept all versions."""
 
     def accepts(self, version: Version) -> Literal[True]:
         return True
 
     def to_string(self) -> str:
         return UNIVERSE_VERSION
 
 
+ALWAYS = SpecifierAlways()
+
+
 @frozen(repr=False)
-class SpecifierSingle(Operator, Specifier):
+class SpecifierOne(Operator, Specifier):
     """Represents specifiers that accept versions according to the
     [`Operator`][versions.operators.Operator] type.
     """
 
     def accepts(self, version: Version) -> bool:
         return self.partial_matches(version)
 
@@ -104,15 +111,15 @@
     @specifiers.validator
     def check_specifiers(self, attribute: Attribute[Specifiers], specifiers: Specifiers) -> None:
         check_specifiers(specifiers)
 
     @classmethod
     def of_specifiers(cls, specifiers: Specifiers) -> Specifier:
         if not specifiers:
-            return SpecifierTrue()
+            return SpecifierNever()
 
         if contains_only_item(specifiers):
             return first(specifiers)
 
         return cls(specifiers)
 
     @classmethod
@@ -150,15 +157,15 @@
     @specifiers.validator
     def check_specifiers(self, attribute: Attribute[Specifiers], specifiers: Specifiers) -> None:
         check_specifiers(specifiers)
 
     @classmethod
     def of_specifiers(cls, specifiers: Specifiers) -> Specifier:
         if not specifiers:
-            return SpecifierTrue()
+            return SpecifierAlways()
 
         if contains_only_item(specifiers):
             return first(specifiers)
 
         return cls(specifiers)
 
     @classmethod
@@ -191,54 +198,54 @@
 
     Returns:
         Whether the `item` provided is an instance of [`Specifier`][versions.specifiers.Specifier].
     """
     return is_instance(item, Specifier)
 
 
-def is_specifier_false(item: Any) -> TypeGuard[SpecifierFalse]:
+def is_specifier_never(item: Any) -> TypeGuard[SpecifierNever]:
     """Checks if an `item` is an instance of
-    [`SpecifierFalse`][versions.specifiers.SpecifierFalse].
+    [`SpecifierNever`][versions.specifiers.SpecifierNever].
 
     Arguments:
         item: The item to check.
 
     Returns:
         Whether the `item` provided is an instance of
-            [`SpecifierFalse`][versions.specifiers.SpecifierFalse].
+            [`SpecifierNever`][versions.specifiers.SpecifierNever].
     """
-    return is_instance(item, SpecifierFalse)
+    return is_instance(item, SpecifierNever)
 
 
-def is_specifier_true(item: Any) -> TypeGuard[SpecifierTrue]:
+def is_specifier_always(item: Any) -> TypeGuard[SpecifierAlways]:
     """Checks if an `item` is an instance of
-    [`SpecifierTrue`][versions.specifiers.SpecifierTrue].
+    [`SpecifierAlways`][versions.specifiers.SpecifierAlways].
 
     Arguments:
         item: The item to check.
 
     Returns:
         Whether the `item` provided is an instance of
-            [`SpecifierTrue`][versions.specifiers.SpecifierTrue].
+            [`SpecifierAlways`][versions.specifiers.SpecifierAlways].
     """
-    return is_instance(item, SpecifierTrue)
+    return is_instance(item, SpecifierAlways)
 
 
-def is_specifier_single(item: Any) -> TypeGuard[SpecifierSingle]:
+def is_specifier_one(item: Any) -> TypeGuard[SpecifierOne]:
     """Checks if an `item` is an instance of
-    [`SpecifierSingle`][versions.specifiers.SpecifierSingle].
+    [`SpecifierOne`][versions.specifiers.SpecifierOne].
 
     Arguments:
         item: The item to check.
 
     Returns:
         Whether the `item` provided is an instance of
-            [`SpecifierSingle`][versions.specifiers.SpecifierSingle].
+            [`SpecifierOne`][versions.specifiers.SpecifierOne].
     """
-    return is_instance(item, SpecifierSingle)
+    return is_instance(item, SpecifierOne)
 
 
 def is_specifier_any(item: Any) -> TypeGuard[SpecifierAny]:
     """Checks if an `item` is an instance of
     [`SpecifierAny`][versions.specifiers.SpecifierAny].
 
     Arguments:
```

### Comparing `versions-1.3.0/versions/string.py` & `versions-1.4.0/versions/string.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import abstractmethod
+from abc import abstractmethod as required
 from typing import Iterable, List, Type, TypeVar
 
 from typing_extensions import Protocol, runtime_checkable
 
 from versions.constants import (
     BRACKETS,
     COMMA,
@@ -19,16 +19,15 @@
 )
 from versions.typing import Unary
 
 __all__ = (
     # simple from_string() and to_string() protocols
     "FromString",
     "ToString",
-    # case folding
-    "case_fold",
+    "String",
     # checks
     "check_int",
     # clearing whitespace
     "clear_whitespace",
     # various concatenation
     "concat_comma",
     "concat_comma_space",
@@ -53,43 +52,46 @@
     "split_comma",
     "split_dot",
     "split_pipes",
     # split function
     "Split",
 )
 
-F = TypeVar("F", bound="FromString")
+T = TypeVar("T", bound="FromString")
 
 
 @runtime_checkable
 class FromString(Protocol):
     @classmethod
-    @abstractmethod
-    def from_string(cls: Type[F], string: str) -> F:
+    @required
+    def from_string(cls: Type[T], string: str) -> T:
         raise NotImplementedError
 
     @classmethod
-    def parse(cls: Type[F], string: str) -> F:
+    def parse(cls: Type[T], string: str) -> T:
         return cls.from_string(string)
 
 
 @runtime_checkable
 class ToString(Protocol):
-    @abstractmethod
+    @required
     def to_string(self) -> str:
         raise NotImplementedError
 
     def to_short_string(self) -> str:
         return self.to_string()
 
     def __str__(self) -> str:
         return self.to_string()
 
 
-case_fold = str.casefold
+@runtime_checkable
+class String(FromString, ToString, Protocol):
+    pass
+
 
 check_int = str.isdigit
 
 
 def concat_empty_args(*args: str) -> str:
     return concat_empty(args)
 
@@ -127,15 +129,15 @@
 EXPECTED_PAIR = "expected a pair of characters"
 
 
 def create_wrap_around(string: str, wrap: Iterable[str] = BRACKETS) -> str:
     try:
         left, right = wrap
 
-    except (ValueError, TypeError):
+    except (ValueError, TypeError):  # pragma: no cover  # not tested
         raise ValueError(EXPECTED_PAIR) from None
 
     return left + string + right
 
 
 create_translation = str.maketrans
 dict_from_keys = dict.fromkeys
```

### Comparing `versions-1.3.0/versions/utils.py` & `versions-1.4.0/versions/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+from functools import lru_cache
 from itertools import chain
 from itertools import islice as iter_slice
 from itertools import repeat
-from typing import Any, Iterable, Iterator, MutableSequence, Optional, Sequence, Sized, TypeVar
+from typing import Iterable, Iterator, MutableSequence, Optional, Sequence, Sized, Tuple, TypeVar
 
 __all__ = (
+    "cache",
+    "flatten",
     "first",
     "last",
     "set_last",
     "next_or_none",
     "contains_only_item",
-    "evolve_in_place",
     "fix_to_length",
     "count_leading_zeros",
 )
 
-A = TypeVar("A")
-T = TypeVar("T")
+cache = lru_cache(None)
 
-set_attribute_directly = object.__setattr__
+flatten = chain.from_iterable
 
+A = TypeVar("A")
+T = TypeVar("T")
 
 FIRST = 0
 LAST = ~0
 
 
 def first(sequence: Sequence[T]) -> T:
     return sequence[FIRST]
@@ -40,28 +43,25 @@
     return next(iterator, None)
 
 
 def contains_only_item(sized: Sized) -> bool:
     return len(sized) == 1
 
 
-def evolve_in_place(instance: A, **changes: Any) -> A:
-    for name, value in changes.items():
-        set_attribute_directly(instance, name, value)
-
-    return instance
-
-
 def fix_to_length(length: int, padding: T, iterable: Iterable[T]) -> Iterator[T]:
     return iter_slice(chain(iterable, repeat(padding)), length)
 
 
 def count_leading_zeros(iterable: Iterable[int]) -> int:
     count = 0
 
     for item in iterable:
         if item:
             break
 
         count += 1
 
     return count
+
+
+def unary_tuple(item: T) -> Tuple[T]:
+    return (item,)
```

### Comparing `versions-1.3.0/versions/version.py` & `versions-1.4.0/versions/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Any, Iterator, Optional, Tuple, Type, TypeVar, Union
+from typing import Iterator, Optional, Tuple, Type, TypeVar, Union
 
 from attrs import evolve, field, frozen
 
 from versions.constants import DASH, DOT, EXCLAMATION, PLUS
 from versions.parsers import VersionParser
 from versions.representation import Representation
 from versions.segments import (
     DEFAULT_PADDING,
     DEFAULT_VALUE,
     DevTag,
     Epoch,
     Extra,
     Local,
+    LocalPart,
     PostTag,
     PreTag,
     Release,
 )
 from versions.specification import Specification
-from versions.string import FromString, ToString, concat_empty
+from versions.string import String, concat_empty
 from versions.types import AnyInfinity, Infinity, NegativeInfinity, infinity, negative_infinity
-from versions.utils import evolve_in_place
 
 __all__ = ("CompareKey", "Version")
 
 CompareEpoch = Epoch
 CompareRelease = Release
 ComparePreTag = Union[PreTag, AnyInfinity]
 ComparePostTag = Union[PostTag, NegativeInfinity]
@@ -40,15 +40,15 @@
 ]
 
 V = TypeVar("V", bound="Version")
 W = TypeVar("W", bound="Version")
 
 
 @frozen(repr=False, eq=True, order=True)
-class Version(Representation, FromString, ToString):
+class Version(Representation, String):
     """Represents versions."""
 
     epoch: Epoch = field(factory=Epoch, eq=False, order=False)
     """The *epoch* segment of the version."""
 
     release: Release = field(factory=Release, eq=False, order=False)
     """The *release* segment of the version."""
@@ -63,16 +63,33 @@
     """The *dev-release* tag of the version."""
 
     local: Optional[Local] = field(default=None, eq=False, order=False)
     """The *local* segment of the version."""
 
     compare_key: CompareKey = field(repr=False, init=False, eq=True, order=True, hash=False)
 
-    def __attrs_post_init__(self) -> None:
-        evolve_in_place(self, compare_key=self.compute_compare_key())
+    @compare_key.default
+    def default_compare_key(self) -> CompareKey:
+        compare_epoch = self.epoch
+        compare_release = self.release
+
+        compare_pre, compare_post, compare_dev = self.compute_compare_tags(
+            self.pre, self.post, self.dev
+        )
+
+        compare_local = self.compute_compare_local(self.local)
+
+        return (
+            compare_epoch,
+            compare_release,
+            compare_pre,
+            compare_post,
+            compare_dev,
+            compare_local,
+        )
 
     @staticmethod
     def compute_compare_tags(
         pre: Optional[PreTag], post: Optional[PostTag], dev: Optional[DevTag]
     ) -> Tuple[ComparePreTag, ComparePostTag, CompareDevTag]:
         compare_pre: ComparePreTag
         compare_post: ComparePostTag
@@ -93,33 +110,14 @@
 
         return (compare_pre, compare_post, compare_dev)
 
     @staticmethod
     def compute_compare_local(local: Optional[Local]) -> CompareLocal:
         return negative_infinity if local is None else local
 
-    def compute_compare_key(self) -> CompareKey:
-        compare_epoch = self.epoch
-        compare_release = self.release
-
-        compare_pre, compare_post, compare_dev = self.compute_compare_tags(
-            self.pre, self.post, self.dev
-        )
-
-        compare_local = self.compute_compare_local(self.local)
-
-        return (
-            compare_epoch,
-            compare_release,
-            compare_pre,
-            compare_post,
-            compare_dev,
-            compare_local,
-        )
-
     @classmethod
     def from_string(cls: Type[V], string: str) -> V:
         """Parses a [`Version`][versions.version.Version] from `string`.
 
         Arguments:
             string: The string to parse.
 
@@ -205,14 +203,33 @@
         """Converts a [`Version`][versions.version.Version] to its *short* string representation.
 
         Returns:
             The *short* version string.
         """
         return concat_empty(self.to_short_string_iterator())
 
+    def to_pep440_string(self) -> str:
+        """Converts a [`Version`][versions.version.Version] to its
+        [*PEP 440*](https://peps.python.org/pep-0440) representation.
+
+        ```python
+        version.to_pep440_string()
+        ```
+
+        Is equivalent to the following:
+
+        ```python
+        version.normalize().to_short_string()
+        ```
+
+        Returns:
+            The [*PEP 440*](https://peps.python.org/pep-0440) version string.
+        """
+        return self.normalize().to_short_string()
+
     @property
     def precision(self) -> int:
         """The precision of the [`Release`][versions.segments.Release]."""
         return self.release.precision
 
     @property
     def last_index(self) -> int:
@@ -286,88 +303,106 @@
     def to_semantic(self: V) -> V:
         """Converts the [`Release`][versions.segments.Release]
         to match the [`semver`](https://semver.org/) schema.
 
         Returns:
             The converted version.
         """
-        return self.update(release=self.release.to_semantic())
+        return evolve(self, release=self.release.to_semantic())
+
+    def set_epoch(self: V, epoch: Epoch) -> V:
+        return evolve(self, epoch=epoch)
+
+    def set_epoch_value(self: V, value: int) -> V:
+        return self.set_epoch(self.epoch.set_value(value))
+
+    def set_release(self: V, release: Release) -> V:
+        return evolve(self, release=release)
+
+    def set_release_parts(self: V, *parts: int) -> V:
+        return self.set_release(self.release.set_parts(*parts))
+
+    def slice(self: V, index: int) -> V:
+        return self.set_release(self.release.slice(index))
 
     def set_major(self: V, value: int) -> V:
         """Sets the *major* part of the [`Release`][versions.segments.Release] to the `value`.
 
         Arguments:
             value: The value to set the *major* part to.
 
         Returns:
             The updated version.
         """
-        return self.update(release=self.release.set_major(value))
+        return self.set_release(self.release.set_major(value))
 
     def set_minor(self: V, value: int) -> V:
         """Sets the *minor* part of the [`Release`][versions.segments.Release] to the `value`.
 
         Arguments:
             value: The value to set the *minor* part to.
 
         Returns:
             The updated version.
         """
-        return self.update(release=self.release.set_minor(value))
+        return self.set_release(self.release.set_minor(value))
 
     def set_micro(self: V, value: int) -> V:
         """Sets the *micro* part of the [`Release`][versions.segments.Release] to the `value`.
 
         Arguments:
             value: The value to set the *micro* part to.
 
         Returns:
             The updated version.
         """
-        return self.update(release=self.release.set_micro(value))
+        return self.set_release(self.release.set_micro(value))
 
     def set_patch(self: V, value: int) -> V:
         """Sets the *patch* part of the [`Release`][versions.segments.Release] to the `value`.
 
         This is equivalent to [`set_micro`][versions.version.Version.set_micro].
 
         Arguments:
             value: The value to set the *patch* part to.
 
         Returns:
             The updated version.
         """
-        return self.update(release=self.release.set_patch(value))
+        return self.set_release(self.release.set_patch(value))
 
     def set_at(self: V, index: int, value: int) -> V:
         """Sets the [`Release`][versions.segments.Release] part at the `index` to the `value`.
 
         Arguments:
             index: The index to set the `value` at.
             value: The value to set the part to.
 
         Returns:
             The updated version.
         """
-        return self.update(release=self.release.set_at(index, value))
+        return self.set_release(self.release.set_at(index, value))
 
     def set_at_unchecked(self: V, index: int, value: int) -> V:
         """Sets the [`Release`][versions.segments.Release] part at the `index` to the `value`.
 
         Arguments:
             index: The index to set the `value` at.
             value: The value to set the part to.
 
         Raises:
             IndexError: The index is *out-of-bounds*.
 
         Returns:
             The updated version.
         """
-        return self.update(release=self.release.set_at_unchecked(index, value))
+        return self.set_release(self.release.set_at_unchecked(index, value))
+
+    def next_epoch(self: V) -> V:
+        return self.set_epoch(self.epoch.next_value())
 
     def next_major(self: V) -> V:
         """Bumps the *major* part of the [`Release`][versions.segments.Release]
         if the version is stable, otherwise converts the version to be stable.
 
         Returns:
             The bumped version.
@@ -496,38 +531,38 @@
         Arguments:
             length: The length to pad the release to.
             padding: The padding to use.
 
         Returns:
             The padded version.
         """
-        return evolve(self, release=self.release.pad_to(length, padding))
+        return self.set_release(self.release.pad_to(length, padding))
 
     def pad_to_index(self: V, index: int, padding: int = DEFAULT_PADDING) -> V:
         """Pads the [`Release`][versions.segments.Release] to the `index` with `padding`.
 
         Arguments:
             index: The index to pad the release to.
             padding: The padding to use.
 
         Returns:
             The padded version.
         """
-        return evolve(self, release=self.release.pad_to_index(index, padding))
+        return self.set_release(self.release.pad_to_index(index, padding))
 
     def pad_to_next(self: V, padding: int = DEFAULT_PADDING) -> V:
         """Pads the [`Release`][versions.segments.Release] to the next index.
 
         Arguments:
             padding: The padding to use.
 
         Returns:
             The padded version.
         """
-        return evolve(self, release=self.release.pad_to_next(padding))
+        return self.set_release(self.release.pad_to_next(padding))
 
     def is_pre_release(self) -> bool:
         """Checks if the version is *pre-release*.
 
         Returns:
             Whether the version is *pre-release*.
         """
@@ -604,15 +639,15 @@
 
         else:
             pre = pre.next_phase()
 
             if pre is None:
                 return None
 
-        return self.create(self.epoch, self.release, pre)
+        return self.without_tags_and_local().with_pre(pre)
 
     def next_post(self: V) -> V:
         """Bumps the [`PostTag`][versions.segments.PostTag] if it is present,
         otherwise adds one to the version.
 
         Returns:
             The bumped version.
@@ -621,15 +656,15 @@
 
         if post is None:
             post = PostTag()
 
         else:
             post = post.next()
 
-        return self.create(self.epoch, self.release, self.pre, post, self.dev)
+        return self.with_post(post).without_dev_and_local()
 
     def next_dev(self: V) -> V:
         """Bumps the [`DevTag`][versions.segments.DevTag] if it is present,
         otherwise adds one to the version.
 
         Returns:
             The bumped version.
@@ -638,102 +673,145 @@
 
         if dev is None:
             dev = DevTag()
 
         else:
             dev = dev.next()
 
-        return self.create(self.epoch, self.release, self.pre, self.post, dev)
+        return self.with_dev(dev).without_local()
+
+    def set_pre(self: V, pre: Optional[PreTag]) -> V:
+        return evolve(self, pre=pre)
+
+    def set_post(self: V, post: Optional[PostTag]) -> V:
+        return evolve(self, post=post)
+
+    def set_dev(self: V, dev: Optional[DevTag]) -> V:
+        return evolve(self, dev=dev)
+
+    def set_tags(
+        self: V, pre: Optional[PreTag], post: Optional[PostTag], dev: Optional[DevTag]
+    ) -> V:
+        return evolve(self, pre=pre, post=post, dev=dev)
+
+    def set_local(self: V, local: Optional[Local]) -> V:
+        return evolve(self, local=local)
+
+    def set_local_parts(self: V, *parts: LocalPart) -> V:
+        local = self.local
+
+        local = Local.from_parts(*parts) if local is None else local.set_parts(*parts)
+
+        return self.set_local(local)
+
+    def set_dev_and_local(self: V, dev: Optional[DevTag], local: Optional[Local]) -> V:
+        return evolve(self, dev=dev, local=local)
+
+    def set_tags_and_local(
+        self: V,
+        pre: Optional[PreTag],
+        post: Optional[PostTag],
+        dev: Optional[DevTag],
+        local: Optional[Local],
+    ) -> V:
+        return evolve(self, pre=pre, post=post, dev=dev, local=local)
 
     def with_pre(self: V, pre: PreTag) -> V:
         """Updates a version to include [`PreTag`][versions.segments.PreTag].
 
         Arguments:
             pre: The *pre-release* tag to include.
 
         Returns:
             The updated version.
         """
-        return self.update(pre=pre)
+        return self.set_pre(pre)
 
     def with_post(self: V, post: PostTag) -> V:
         """Updates a version to include [`PostTag`][versions.segments.PostTag].
 
         Arguments:
             post: The *post-release* tag to include.
 
         Returns:
             The updated version.
         """
-        return self.update(post=post)
+        return self.set_post(post)
 
     def with_dev(self: V, dev: DevTag) -> V:
         """Updates a version to include [`DevTag`][versions.segments.DevTag].
 
         Arguments:
             dev: The *dev-release* tag to include.
 
         Returns:
             The updated version.
         """
-        return self.update(dev=dev)
+        return self.set_dev(dev)
+
+    def with_tags(self: V, pre: PreTag, post: PostTag, dev: DevTag) -> V:
+        return self.set_tags(pre, post, dev)
 
     def with_local(self: V, local: Local) -> V:
         """Updates a version to include [`Local`][versions.segments.Local].
 
         Arguments:
             local: The *local* segment to include.
 
         Returns:
             The updated version.
         """
-        return self.update(local=local)
+        return self.set_local(local)
+
+    def with_dev_and_local(self: V, dev: DevTag, local: Local) -> V:
+        return self.set_dev_and_local(dev, local)
+
+    def with_tags_and_local(self: V, pre: PreTag, post: PostTag, dev: DevTag, local: Local) -> V:
+        return self.set_tags_and_local(pre, post, dev, local)
 
     def without_pre(self: V) -> V:
         """Updates a version, removing any [`PreTag`][versions.segments.PreTag] from it.
 
         Returns:
             The updated version.
         """
-        return self.update(pre=None)
+        return self.set_pre(None)
 
     def without_post(self: V) -> V:
         """Updates a version, removing any [`PostTag`][versions.segments.PostTag] from it.
 
         Returns:
             The updated version.
         """
-        return self.update(post=None)
+        return self.set_post(None)
 
     def without_dev(self: V) -> V:
         """Updates a version, removing any [`DevTag`][versions.segments.DevTag] from it.
 
         Returns:
             The updated version.
         """
-        return self.update(dev=None)
+        return self.set_dev(None)
+
+    def without_tags(self: V) -> V:
+        return self.set_tags(None, None, None)
 
     def without_local(self: V) -> V:
         """Updates a version, removing any [`Local`][versions.segments.Local] segment from it.
 
         Returns:
             The updated version.
         """
-        return self.update(local=None)
-
-    def update(self: V, **changes: Any) -> V:
-        """Updates a version with `changes`.
+        return self.set_local(None)
 
-        Arguments:
-            **changes: The changes to apply.
+    def without_dev_and_local(self: V) -> V:
+        return self.set_dev_and_local(None, None)
 
-        Returns:
-            The updated version.
-        """
-        return evolve(self, **changes)
+    def without_tags_and_local(self: V) -> V:
+        return self.set_tags_and_local(None, None, None, None)
 
     def weaken(self, other: W) -> W:
         """Weakens the `other` version for further comparison.
 
         Arguments:
             other: The version to weaken.
 
@@ -750,20 +828,28 @@
 
     def to_stable(self: V) -> V:
         """Forces a version to be stable.
 
         Returns:
             The stable version.
         """
-        return self if self.is_stable() else self.create(self.epoch, self.release)
+        return self if self.is_stable() else self.to_stable_unchecked()
+
+    def to_stable_unchecked(self: V) -> V:
+        """Forces a version to be stable, without checking whether it is already stable.
+
+        Returns:
+            The stable version.
+        """
+        return self.without_tags_and_local()
 
     def next_breaking(self: V) -> V:
         """Returns the next breaking version.
 
-        This function is slightly convoluted due to how `0.x.y` versions are handled:
+        This function is slightly convoluted due to how `0.x.y` and `0.0.z` versions are handled:
 
         | version | next breaking |
         |---------|---------------|
         | `1.2.3` | `2.0.0`       |
         | `1.2.0` | `2.0.0`       |
         | `1.0.0` | `2.0.0`       |
         | `0.2.3` | `0.3.0`       |
@@ -806,15 +892,15 @@
             post = post.normalize()
 
         dev = self.dev
 
         if dev is not None:
             dev = dev.normalize()
 
-        return self.update(pre=pre, post=post, dev=dev)
+        return self.set_tags(pre, post, dev)
 
     @classmethod
     def create(
         cls: Type[V],
         epoch: Optional[Epoch] = None,
         release: Optional[Release] = None,
         pre: Optional[PreTag] = None,
```

### Comparing `versions-1.3.0/versions/version_sets.py` & `versions-1.4.0/versions/version_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 from __future__ import annotations
 
-from abc import abstractmethod
-from builtins import isinstance as is_instance
-from itertools import chain
-from typing import TYPE_CHECKING, Any, Iterable, Iterator, List, Optional, Tuple, TypeVar, Union
+from abc import abstractmethod as required
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 from attrs import Attribute, define, evolve, field, frozen
+from orderings import Ordering
 from typing_extensions import Literal, Protocol, TypeGuard, runtime_checkable
 
 from versions.constants import EMPTY_VERSION, UNIVERSE_VERSION
 from versions.errors import InternalError
 from versions.operators import Operator, OperatorType
 from versions.representation import Representation
 from versions.specification import Specification
 from versions.string import (
     ToString,
     concat_comma,
     concat_comma_space,
     concat_pipes,
     concat_pipes_spaced,
 )
-from versions.types import Infinity, NegativeInfinity, Ordering, infinity, negative_infinity
-from versions.typing import DynamicTuple
-from versions.utils import contains_only_item, evolve_in_place, first, last, next_or_none, set_last
+from versions.types import Infinity, NegativeInfinity, infinity, negative_infinity
+from versions.typing import DynamicTuple, is_instance
+from versions.utils import contains_only_item, first, flatten, last, next_or_none, set_last
 
 if TYPE_CHECKING:
     from versions.version import Version
 
 __all__ = (
     "VersionEmpty",
     "VersionPoint",
@@ -38,58 +48,54 @@
     "is_version_point",
     "is_version_range",
     "is_version_union",
     "is_version_item",
     "is_version_set",
 )
 
-flatten = chain.from_iterable
-
-T = TypeVar("T")
-
 
 @runtime_checkable
 class VersionSetProtocol(Specification, Protocol):
-    @abstractmethod
+    @required
     def is_empty(self) -> bool:
         """Checks if the set is *empty*.
 
         Returns:
             Whether the set is *empty*.
         """
         raise NotImplementedError
 
-    @abstractmethod
-    def is_universe(self) -> bool:
+    @required
+    def is_universal(self) -> bool:
         """Checks if the set is the *universal*.
 
         Returns:
             Whether the set is *universal*.
         """
         raise NotImplementedError
 
-    @abstractmethod
+    @required
     def includes(self, version_set: VersionSet) -> bool:
         """Checks if the set includes `version_set`.
 
         Returns:
             Whether the set includes `version_set`.
         """
         raise NotImplementedError
 
-    @abstractmethod
+    @required
     def intersects(self, version_set: VersionSet) -> bool:
         """Checks if the set intersects `version_set`.
 
         Returns:
             Whether the set intersects `version_set`.
         """
         raise NotImplementedError
 
-    @abstractmethod
+    @required
     def contains(self, version: Version) -> bool:
         """Checks if the set contains some `version`.
 
         Returns:
             Whether the `version` is contained within the set.
         """
         raise NotImplementedError
@@ -102,42 +108,42 @@
         [`self.contains(version)`][versions.version_sets.VersionSetProtocol.contains].
 
         Returns:
             Whether the `version` is accepted by the set.
         """
         return self.contains(version)
 
-    @abstractmethod
+    @required
     def intersection(self, version_set: VersionSet) -> VersionSet:
         """Computes the *intersection* of `self` and `version_set`.
 
         Returns:
             The set representing the *intersection* of `self` and `version_set`.
         """
         raise NotImplementedError
 
-    @abstractmethod
+    @required
     def union(self, version_set: VersionSet) -> VersionSet:
         """Computes the *union* of `self` and `version_set`.
 
         Returns:
             The set representing the *union* of `self` and `version_set`.
         """
         raise NotImplementedError
 
-    @abstractmethod
+    @required
     def difference(self, version_set: VersionSet) -> VersionSet:
         """Computes the *difference* of `self` and `version_set`.
 
         Returns:
             The set representing the *difference* of `self` and `version_set`.
         """
         raise NotImplementedError
 
-    @abstractmethod
+    @required
     def complement(self) -> VersionSet:
         """Computes the *complement* of `self`.
 
         Returns:
             The set representing the *complement* of `self`.
         """
         raise NotImplementedError
@@ -327,20 +333,20 @@
 
 E = TypeVar("E", bound="VersionEmpty")
 S = TypeVar("S", bound="VersionSet")
 
 
 @frozen(repr=False, order=False)
 class VersionEmpty(Representation, ToString, VersionSetProtocol):
-    """Represents empty version sets (`{}`)."""
+    """Represents empty version sets (`0`)."""
 
     def is_empty(self) -> Literal[True]:
         return True
 
-    def is_universe(self) -> Literal[False]:
+    def is_universal(self) -> Literal[False]:
         return False
 
     def includes(self, version_set: VersionSet) -> bool:
         return version_set.is_empty()
 
     def intersects(self, version_set: VersionSet) -> Literal[False]:
         return False
@@ -357,30 +363,52 @@
     def difference(self: E, version_set: VersionSet) -> E:
         return self
 
     def symmetric_difference(self, version_set: S) -> S:
         return version_set
 
     def complement(self) -> VersionRange:
-        return VersionRange()
+        return UNIVERSAL_SET
 
     def to_string(self) -> str:
         return EMPTY_VERSION
 
 
-def is_version_range_protocol(item: Any) -> TypeGuard[VersionRangeProtocol]:
-    return is_instance(item, VersionRangeProtocol)
+EMPTY_SET = VersionEmpty()
+
+MIN_MAX_CONSTRAINT = "version ranges expect `min <= max`, got `min > max`"
+RANGE_NOT_POINT = "version range is not a point"
+UNEXPECTED_VERSION_SET = "unexpected version set provided: {}"
+CAN_NOT_INCLUDE_INFINITY = "ranges can not contain infinities"
+
 
+def unexpected_version_set(item: Any) -> TypeError:
+    return TypeError(UNEXPECTED_VERSION_SET.format(item))
 
-@runtime_checkable
-class VersionRangeProtocol(Protocol):
-    min: Optional[Version]
-    max: Optional[Version]
-    include_min: bool
-    include_max: bool
+
+@frozen(repr=False, eq=False, order=False)
+class VersionRange(Representation, ToString, VersionSetProtocol):
+    """Represents version ranges (`(v, w)`, `(v, w]`, `[v, w)` and `[v, w]`)."""
+
+    min: Optional[Version] = None
+    max: Optional[Version] = None
+    include_min: bool = False
+    include_max: bool = False
+
+    def __attrs_post_init__(self) -> None:
+        if self.min is None and self.include_min:
+            raise ValueError(CAN_NOT_INCLUDE_INFINITY)
+
+        if self.max is None and self.include_max:
+            raise ValueError(CAN_NOT_INCLUDE_INFINITY)
+
+        if self.comparable_min > self.comparable_max:
+            raise ValueError(MIN_MAX_CONSTRAINT)
+
+    # range stuff
 
     @property
     def parameters(self) -> Tuple[Optional[Version], Optional[Version], bool, bool]:
         return (self.min, self.max, self.include_min, self.include_max)
 
     @property
     def exclude_min(self) -> bool:
@@ -437,90 +465,93 @@
 
     def is_right_bounded(self) -> bool:
         return self.max is not None
 
     def is_empty_or_point(self) -> bool:
         return self.comparable_min == self.comparable_max
 
-    def is_lower(self, other: VersionRangeProtocol) -> bool:
+    def is_lower(self, other: VersionRange) -> bool:
         self_comparable_min = self.comparable_min
         other_comparable_min = other.comparable_min
 
         if self_comparable_min < other_comparable_min:
             return True
 
         if self_comparable_min > other_comparable_min:
             return False
 
         return self.include_min and other.exclude_min
 
-    def is_higher(self, other: VersionRangeProtocol) -> bool:
+    def is_higher(self, other: VersionRange) -> bool:
         self_comparable_max = self.comparable_max
         other_comparable_max = other.comparable_max
 
         if self_comparable_max < other_comparable_max:
             return False
 
         if self_comparable_max > other_comparable_max:
             return True
 
         return self.include_max and other.exclude_max
 
-    def is_strictly_lower(self, other: VersionRangeProtocol) -> bool:
+    def is_strictly_lower(self, other: VersionRange) -> bool:
         self_comparable_max = self.comparable_max
         other_comparable_min = other.comparable_min
 
         if self_comparable_max < other_comparable_min:
             return True
 
         if self_comparable_max > other_comparable_min:
             return False
 
         return self.exclude_max or other.exclude_min
 
-    def is_strictly_higher(self, other: VersionRangeProtocol) -> bool:
+    def is_strictly_higher(self, other: VersionRange) -> bool:
         self_comparable_min = self.comparable_min
         other_comparable_max = other.comparable_max
 
         if self_comparable_min > other_comparable_max:
             return True
 
         if self_comparable_min < other_comparable_max:
             return False
 
         return self.exclude_min or other.exclude_max
 
-    def is_left_adjacent(self, other: VersionRangeProtocol) -> bool:
-        return (self.max == other.min) and (self.include_max != other.include_min)
+    def is_left_adjacent(self, other: VersionRange) -> bool:
+        return (self.max == other.min) and (self.include_max is other.exclude_min)
 
-    def is_right_adjacent(self, other: VersionRangeProtocol) -> bool:
-        return (self.min == other.max) and (self.include_min != other.include_max)
+    def is_right_adjacent(self, other: VersionRange) -> bool:
+        return (self.min == other.max) and (self.include_min is other.exclude_max)
 
-    def is_adjacent(self, other: VersionRangeProtocol) -> bool:
+    def is_adjacent(self, other: VersionRange) -> bool:
         return self.is_left_adjacent(other) or self.is_right_adjacent(other)
 
+    def __hash__(self) -> int:
+        return hash(self.parameters)
+
     def __eq__(self, other: Any) -> bool:
-        return is_version_range_protocol(other) and self.parameters == other.parameters
+        return is_version_range(other) and self.parameters == other.parameters
 
     def __ne__(self, other: Any) -> bool:
         return not self.__eq__(other)
 
-    def __lt__(self, other: VersionRangeProtocol) -> bool:
+    def __lt__(self, other: VersionRange) -> bool:
         return self.compare(other).is_less()
 
-    def __le__(self, other: VersionRangeProtocol) -> bool:
+    def __le__(self, other: VersionRange) -> bool:
         return self.compare(other).is_less_or_equal()
 
-    def __gt__(self, other: VersionRangeProtocol) -> bool:
+    def __gt__(self, other: VersionRange) -> bool:
         return self.compare(other).is_greater()
 
-    def __ge__(self, other: VersionRangeProtocol) -> bool:
+    def __ge__(self, other: VersionRange) -> bool:
         return self.compare(other).is_greater_or_equal()
 
-    def compare(self, other: VersionRangeProtocol) -> Ordering:
+    def compare(self, other: VersionRange) -> Ordering:
         self_comparable_min = self.comparable_min
         other_comparable_min = other.comparable_min
 
         if self_comparable_min > other_comparable_min:
             return Ordering.GREATER
 
         if self_comparable_min < other_comparable_min:
@@ -543,59 +574,40 @@
         include_max = self.include_max
 
         if include_max == other.exclude_max:
             return Ordering.GREATER if include_max else Ordering.LESS
 
         return Ordering.EQUAL
 
-
-MIN_MAX_CONSTRAINT = "version ranges expect min <= max, got min > max"
-RANGE_NOT_POINT = "version range is not a point"
-UNEXPECTED_VERSION_SET = "unexpected version set provided: {}"
-
-
-@frozen(repr=False, eq=False, order=False)
-class VersionRange(Representation, ToString, VersionRangeProtocol, VersionSetProtocol):
-    """Represents version ranges (`(x, y)`, `(x, y]`, `[x, y)` and `[x, y]`)."""
-
-    min: Optional[Version] = None
-    max: Optional[Version] = None
-    include_min: bool = False
-    include_max: bool = False
-
-    def __attrs_post_init__(self) -> None:
-        if self.min is None:
-            evolve_in_place(self, include_min=False)
-
-        if self.max is None:
-            evolve_in_place(self, include_max=False)
-
-        if self.comparable_min > self.comparable_max:
-            raise ValueError(MIN_MAX_CONSTRAINT)
+    # protocol implementation
 
     def is_empty(self) -> bool:
         return self.is_empty_or_point() and not self.is_closed()
 
     def is_point(self) -> bool:
         return self.is_empty_or_point() and self.is_closed()
 
-    def is_universe(self) -> bool:
+    def is_universal(self) -> bool:
         return self.is_unbounded()
 
     @property
     def version(self) -> Version:
+        if self.is_point():
+            return self.version_unchecked
+
+        raise ValueError(RANGE_NOT_POINT)
+
+    @property
+    def version_unchecked(self) -> Version:
         version = self.min or self.max
 
-        if version is None:
+        if version is None:  # we can not violate the type system
             raise ValueError(RANGE_NOT_POINT)
 
-        if self.is_point():
-            return version
-
-        raise ValueError(RANGE_NOT_POINT)
+        return version
 
     def contains(self, version: Version) -> bool:
         comparable_min = self.comparable_min
         comparable_max = self.comparable_max
 
         if version < comparable_min:
             return False
@@ -622,52 +634,52 @@
 
         if is_version_range(version_set):
             return not version_set.is_lower(self) and not version_set.is_higher(self)
 
         if is_version_union(version_set):
             return all(self.includes(item) for item in version_set.items)
 
-        raise TypeError(UNEXPECTED_VERSION_SET.format(repr(version_set)))
+        raise unexpected_version_set(version_set)
 
     def intersects(self, version_set: VersionSet) -> bool:
         if is_version_empty(version_set):
             return False
 
         if is_version_point(version_set):
             return self.contains(version_set.version)
 
         if is_version_range(version_set):
             return self.intersects_range(version_set)
 
         if is_version_union(version_set):
             return any(self.intersects(item) for item in version_set.items)
 
-        raise TypeError(UNEXPECTED_VERSION_SET.format(repr(version_set)))
+        raise unexpected_version_set(version_set)
 
     def intersects_range(self, range: VersionRange) -> bool:
         return not range.is_strictly_lower(self) and not range.is_strictly_higher(self)
 
     def intersection(self, version_set: VersionSet) -> VersionSet:
         if is_version_empty(version_set):
-            return VersionEmpty()
+            return EMPTY_SET
 
         if is_version_point(version_set):
             return version_set.intersection(self)
 
         if is_version_range(version_set):
             if self.is_lower(version_set):
                 if self.is_strictly_lower(version_set):
-                    return VersionEmpty()
+                    return EMPTY_SET
 
                 intersection_min = version_set.min
                 intersection_include_min = version_set.include_min
 
             else:
                 if self.is_strictly_higher(version_set):
-                    return VersionEmpty()
+                    return EMPTY_SET
 
                 intersection_min = self.min
                 intersection_include_min = self.include_min
 
             if self.is_higher(version_set):
                 intersection_max = version_set.max
                 intersection_include_max = version_set.include_max
@@ -688,15 +700,15 @@
                 return VersionPoint(intersection.version)
 
             return intersection
 
         if is_version_union(version_set):
             return version_set.intersection(self)
 
-        raise TypeError(UNEXPECTED_VERSION_SET.format(repr(version_set)))
+        raise unexpected_version_set(version_set)
 
     def union(self, version_set: VersionSet) -> VersionSet:
         if is_version_empty(version_set):
             return self
 
         if is_version_point(version_set):
             version = version_set.version
@@ -738,15 +750,15 @@
                 union_include_min,
                 union_include_max,
             )
 
         if is_version_union(version_set):
             return version_set.union(self)
 
-        raise TypeError(UNEXPECTED_VERSION_SET.format(repr(version_set)))
+        raise unexpected_version_set(version_set)
 
     def difference(self, version_set: VersionSet) -> VersionSet:
         if is_version_empty(version_set):
             return self
 
         if is_version_point(version_set):
             version = version_set.version
@@ -794,28 +806,28 @@
             elif self.max == version_set.max:
                 after = VersionPoint(self.max)  # type: ignore
 
             else:
                 after = evolve(self, min=version_set.max, include_min=version_set.exclude_max)
 
             if before is None and after is None:
-                return VersionEmpty()
+                return EMPTY_SET
 
             if before is None:
                 return after  # type: ignore
 
             if after is None:
                 return before  # type: ignore
 
             return VersionUnion.of(before, after)
 
         if is_version_union(version_set):
             return VersionUnion.of_iterable(self.difference_iterator(version_set))
 
-        raise TypeError(UNEXPECTED_VERSION_SET.format(repr(version_set)))
+        raise unexpected_version_set(version_set)
 
     def difference_iterator(self, version_union: VersionUnion) -> Iterator[VersionItem]:
         current: VersionItem = self
 
         for item in version_union.items:
             if item.is_strictly_lower(current):
                 continue
@@ -832,110 +844,113 @@
 
             if is_version_item(difference):
                 current = difference
 
         yield current
 
     def complement(self) -> VersionSet:
-        return VersionRange().difference(self)
+        return UNIVERSAL_SET.difference(self)
 
     def to_string_iterator(self) -> Iterator[str]:
         if self.is_empty():
             yield EMPTY_VERSION
             return
 
         if self.is_point():
             yield self.version.to_string()
             return
 
-        if self.is_universe():
+        if self.is_universal():
             yield UNIVERSE_VERSION
             return
 
         min = self.min
 
-        if min:
-            min_type = OperatorType.GREATER_OR_EQUAL if self.include_min else OperatorType.GREATER
-            min_operator = Operator(min_type, min)
+        if min is not None:
+            min_operator = (
+                Operator.greater_or_equal(min) if self.include_min else Operator.greater(min)
+            )
 
             yield min_operator.to_string()
 
         max = self.max
 
-        if max:
-            max_type = OperatorType.LESS_OR_EQUAL if self.include_max else OperatorType.LESS
-            max_operator = Operator(max_type, max)
+        if max is not None:
+            max_operator = Operator.less_or_equal(max) if self.include_max else Operator.less(max)
 
             yield max_operator.to_string()
 
     def to_short_string_iterator(self) -> Iterator[str]:
         if self.is_empty():
             yield EMPTY_VERSION
             return
 
         if self.is_point():
             yield self.version.to_short_string()
             return
 
-        if self.is_universe():
+        if self.is_universal():
             yield UNIVERSE_VERSION
             return
 
         min = self.min
 
-        if min:
-            min_type = OperatorType.GREATER_OR_EQUAL if self.include_min else OperatorType.GREATER
-            min_operator = Operator(min_type, min)
+        if min is not None:
+            min_operator = (
+                Operator.greater_or_equal(min) if self.include_min else Operator.greater(min)
+            )
 
             yield min_operator.to_short_string()
 
         max = self.max
 
-        if max:
-            max_type = OperatorType.LESS_OR_EQUAL if self.include_max else OperatorType.LESS
-            max_operator = Operator(max_type, max)
+        if max is not None:
+            max_operator = Operator.less_or_equal(max) if self.include_max else Operator.less(max)
 
             yield max_operator.to_short_string()
 
     def to_string(self) -> str:
         return concat_comma_space(self.to_string_iterator())
 
     def to_short_string(self) -> str:
         return concat_comma(self.to_short_string_iterator())
 
 
+UNIVERSAL_SET = VersionRange()
+
+
 @frozen(repr=False, eq=False, order=False)
-class VersionPoint(Representation, ToString, VersionRangeProtocol, VersionSetProtocol):
-    """Represents version points (`[v, v]` aka `{v}`)."""
+class VersionPoint(VersionRange):
+    """Represents version points (`[v, v]` ranges, also known as singleton sets `{v}`)."""
 
-    version: Version
+    version: Version = field()
 
-    @property
-    def min(self) -> Optional[Version]:  # type: ignore
-        return self.version
+    # initialize range fields accordingly
 
-    @property
-    def max(self) -> Optional[Version]:  # type: ignore
-        return self.version
+    min: Version = field(init=False)
+    max: Version = field(init=False)
 
-    @property
-    def include_min(self) -> bool:  # type: ignore
-        return True
+    include_min: Literal[True] = field(default=True, init=False)
+    include_max: Literal[True] = field(default=True, init=False)
 
-    @property
-    def include_max(self) -> bool:  # type: ignore
-        return True
+    @min.default
+    def default_min(self) -> Version:
+        return self.version
+
+    @max.default
+    def default_max(self) -> Version:
+        return self.version
 
     def is_empty(self) -> bool:
         return False
 
     def is_point(self) -> bool:
         return True
 
-    def is_universe(self) -> bool:
+    def is_universal(self) -> bool:
         return False
 
     def contains(self, version: Version) -> bool:
         # version = self.version.weaken(version)
         return self.version == version
 
     accepts = contains
@@ -945,15 +960,15 @@
             is_version_point(version_set) and self.contains(version_set.version)
         )
 
     def intersects(self, version_set: VersionSet) -> bool:
         return version_set.contains(self.version)
 
     def intersection(self, version_set: VersionSet) -> VersionSet:
-        return self if version_set.contains(self.version) else VersionEmpty()
+        return self if version_set.contains(self.version) else EMPTY_SET
 
     def union(self, version_set: VersionSet) -> VersionSet:
         if is_version_empty(version_set):
             return self
 
         if is_version_point(version_set):
             if self.contains(version_set.version):
@@ -963,21 +978,21 @@
 
         if version_set.contains(self.version):
             return version_set
 
         if is_version_range(version_set) or is_version_union(version_set):
             return VersionUnion.of(self, version_set)
 
-        raise TypeError(UNEXPECTED_VERSION_SET.format(repr(version_set)))
+        raise unexpected_version_set(version_set)
 
     def difference(self, version_set: VersionSet) -> VersionSet:
-        return VersionEmpty() if version_set.contains(self.version) else self
+        return EMPTY_SET if version_set.contains(self.version) else self
 
     def complement(self) -> VersionSet:
-        return VersionRange().difference(self)
+        return UNIVERSAL_SET.difference(self)
 
     def to_string(self) -> str:
         return self.version.to_string()
 
     def to_short_string(self) -> str:
         return self.version.to_short_string()
 
@@ -992,85 +1007,99 @@
 
     if contains_only_item(items):
         raise ValueError(ONE_ITEM)
 
 
 UNEXPECTED_UNION = "the union of adjacent or intersecting ranges must be a range"
 
+U = TypeVar("U", bound="VersionUnion")
+
 
 @frozen(repr=False, order=False)
 class VersionUnion(Representation, ToString, Specification):
     """Represents version unions."""
 
     items: VersionItems = field()
 
     @items.validator
     def check_items(self, attribute: Attribute[VersionItems], items: VersionItems) -> None:
         check_items(items)
 
     @classmethod
-    def extract(cls, version_set: VersionSet) -> Iterator[VersionItem]:
+    def of_unchecked(cls: Type[U], *items: VersionItem) -> U:
+        return cls(items)
+
+    @classmethod
+    def of_iterable_unchecked(cls: Type[U], items: Iterable[VersionItem]) -> U:
+        return cls(tuple(items))
+
+    @staticmethod
+    def extract(version_set: VersionSet) -> Iterator[VersionItem]:
         if is_version_union(version_set):
             yield from version_set.items
 
         if is_version_item(version_set):
             yield version_set
 
     @classmethod
-    def of(cls, *version_sets: VersionSet) -> VersionSet:
-        return cls.of_iterable(version_sets)
-
-    @classmethod
-    def of_iterable(cls, iterable: Iterable[VersionSet]) -> VersionSet:
+    def merge(cls, iterable: Iterable[VersionSet]) -> VersionSet:
         extracted = list(flatten(map(cls.extract, iterable)))
 
         if not extracted:
-            return VersionEmpty()
+            return EMPTY_SET
 
-        if any(item.is_universe() for item in extracted):
-            return VersionRange()
+        if any(item.is_universal() for item in extracted):
+            return UNIVERSAL_SET
 
-        extracted.sort()
+        extracted.sort()  # since ranges and points are ordered
 
         merged: List[VersionItem] = []
 
         for item in extracted:
-            if not merged:
+            if not merged:  # nothing to merge yet
                 merged.append(item)
 
             else:
                 last_item = last(merged)
 
                 if last_item.intersects(item) or last_item.is_adjacent(item):
                     result = last_item.union(item)
 
                     if is_version_item(result):
                         set_last(merged, result)
 
-                    else:  # pragma: no cover
+                    else:
                         raise InternalError(UNEXPECTED_UNION)
 
                 else:
                     merged.append(item)
 
         if contains_only_item(merged):
             return first(merged)
 
-        return cls(tuple(merged))
+        return cls.of_iterable_unchecked(merged)
+
+    @classmethod
+    def of(cls, *version_sets: VersionSet) -> VersionSet:
+        return cls.of_iterable(version_sets)
+
+    @classmethod
+    def of_iterable(cls, version_sets: Iterable[VersionSet]) -> VersionSet:
+        return cls.merge(version_sets)
 
     @property
     def exclude_version(self) -> Optional[Version]:
         complement = self.complement()
 
         return complement.version if is_version_point(complement) else None
 
     def is_empty(self) -> bool:
         return False
 
-    def is_universe(self) -> bool:
+    def is_universal(self) -> bool:
         return False
 
     def contains(self, version: Version) -> bool:
         return any(item.contains(version) for item in self.items)
 
     accepts = contains
 
@@ -1135,15 +1164,15 @@
         return self.of(self, version_set)
 
     def difference(self, version_set: VersionSet) -> VersionSet:
         items_difference = ItemsDifference(iter(self.items), self.extract(version_set))
         return self.of_iterable(items_difference.compute())
 
     def complement(self) -> VersionSet:
-        return VersionRange().difference(self)
+        return UNIVERSAL_SET.difference(self)
 
     def to_string(self) -> str:
         exclude_version = self.exclude_version
 
         if exclude_version:
             operator = Operator(OperatorType.NOT_EQUAL, exclude_version)
```

### Comparing `versions-1.3.0/PKG-INFO` & `versions-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versions
-Version: 1.3.0
+Version: 1.4.0
 Summary: Parsing, inspecting and specifying versions.
 Home-page: https://github.com/nekitdev/versions
 License: MIT
 Keywords: python,semver,version
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,16 +15,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: attrs (>=22.1.0)
-Requires-Dist: typing-extensions (>=4.3.0)
+Requires-Dist: attrs (>=23.1.0)
+Requires-Dist: click (>=8.1.3)
+Requires-Dist: entrypoint (>=1.4.0)
+Requires-Dist: orderings (>=1.1.0)
+Requires-Dist: solus (>=1.1.0)
+Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/versions
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/versions/issues
 Project-URL: Repository, https://github.com/nekitdev/versions
 Description-Content-Type: text/markdown
 
@@ -70,15 +74,15 @@
 $ poetry add versions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-versions = "^1.3.0"
+versions = "^1.4.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.versions]
 git = "https://github.com/nekitdev/versions.git"
@@ -138,32 +142,57 @@
 True
 ```
 
 ### Specification
 
 `versions` also supports specifying version requirements and matching version against them.
 
-Since versions support total ordering, they can be checked using version sets
+Since versions support total ordering, they can be checked using *version sets*
 (via [`parse_version_set`][versions.functions.parse_version_set]):
 
 ```python
 >>> from versions import parse_version, parse_version_set
 >>> version_set = parse_version_set("^1.0.0")
 >>> version_set
 <VersionRange (>= 1.0.0, < 2.0.0)>
 >>> version = parse_version("1.3.0")
->>> version
-<Version (1.3.0)>
 >>> version.matches(version_set)
 True
 >>> another = parse_version("2.2.0")
 >>> another.matches(version_set)
 False
 ```
 
+Alternatively, one can use *specifiers*, which are similar to version sets, except they retain
+the structure of specifications given (via [`parse_specifier`][versions.functions.parse_specifier]):
+
+```python
+>>> from versions import parse_specifier, parse_version
+>>> specifier = parse_specifier("^1.0.0")
+>>> specifier
+<SpecifierOne (^1.0.0)>
+>>> version = parse_version("1.3.0")
+>>> version.matches(specifier)
+True
+>>> another = parse_version("2.2.0")
+>>> another.matches(specifier)
+False
+```
+
+## Versioned
+
+`versions` allows users to access versions of items that have the `__version__` attribute:
+
+```python
+>>> from versions import get_version
+>>> import versions
+>>> get_version(versions)
+<Version (1.4.0)>
+```
+
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
 
 If you need support with the library, you can send an [email][Email]
@@ -209,10 +238,11 @@
 [Downloads Badge]: https://img.shields.io/pypi/dm/versions
 
 [Documentation Badge]: https://github.com/nekitdev/versions/workflows/docs/badge.svg
 [Check Badge]: https://github.com/nekitdev/versions/workflows/check/badge.svg
 [Test Badge]: https://github.com/nekitdev/versions/workflows/test/badge.svg
 [Coverage Badge]: https://codecov.io/gh/nekitdev/versions/branch/main/graph/badge.svg
 
+[versions.functions.parse_specifier]: https://nekitdev.github.io/versions/reference/functions#versions.functions.parse_specifier
 [versions.functions.parse_version]: https://nekitdev.github.io/versions/reference/functions#versions.functions.parse_version
 [versions.functions.parse_version_set]: https://nekitdev.github.io/versions/reference/functions#versions.functions.parse_version_set
```

