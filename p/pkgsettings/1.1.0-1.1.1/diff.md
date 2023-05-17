# Comparing `tmp/pkgsettings-1.1.0.tar.gz` & `tmp/pkgsettings-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgsettings-1.1.0.tar", last modified: Mon May 15 14:34:42 2023, max compression
+gzip compressed data, was "pkgsettings-1.1.1.tar", last modified: Wed May 17 21:03:24 2023, max compression
```

## Comparing `pkgsettings-1.1.0.tar` & `pkgsettings-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.726378 pkgsettings-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.726378 pkgsettings-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/_static/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     9870 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/pkgsettings/
--rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/pkgsettings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4363 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/pkgsettings/pkgsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/pkgsettings/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/pkgsettings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 14:34:42.000000 pkgsettings-1.1.0/pkgsettings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-15 14:34:42.730378 pkgsettings-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 14:34:30.000000 pkgsettings-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:24.266123 pkgsettings-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:24.262123 pkgsettings-1.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:24.262123 pkgsettings-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-17 21:03:24.266123 pkgsettings-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:24.262123 pkgsettings-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:24.262123 pkgsettings-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/docs/_static/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9870 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:24.262123 pkgsettings-1.1.1/pkgsettings/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/pkgsettings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5085 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/pkgsettings/pkgsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/pkgsettings/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:03:24.266123 pkgsettings-1.1.1/pkgsettings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-17 21:03:24.000000 pkgsettings-1.1.1/pkgsettings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-17 21:03:24.000000 pkgsettings-1.1.1/pkgsettings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:03:24.000000 pkgsettings-1.1.1/pkgsettings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:03:24.000000 pkgsettings-1.1.1/pkgsettings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 21:03:24.000000 pkgsettings-1.1.1/pkgsettings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 21:03:24.000000 pkgsettings-1.1.1/pkgsettings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-17 21:03:24.266123 pkgsettings-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-17 21:03:13.000000 pkgsettings-1.1.1/tox.ini
```

### Comparing `pkgsettings-1.1.0/.editorconfig` & `pkgsettings-1.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/.gitchangelog.rc` & `pkgsettings-1.1.1/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/.github/workflows/publish.yml` & `pkgsettings-1.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/.github/workflows/tests.yml` & `pkgsettings-1.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/.gitignore` & `pkgsettings-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/Changelog.md` & `pkgsettings-1.1.1/Changelog.md`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/LICENSE` & `pkgsettings-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/Makefile` & `pkgsettings-1.1.1/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 
 .PHONY: lint/isort
 lint/isort: venv
 	venv/bin/isort --diff --check $(SRC)
 
 .PHONY: lint/mypy
 lint/mypy: venv
-	venv/bin/mypy $(SRC)
+	venv/bin/mypy --python-version 3.7 -p pkgsettings -p tests
+	venv/bin/mypy --python-version 3.8 -p pkgsettings -p tests
+	venv/bin/mypy --python-version 3.9 -p pkgsettings -p tests
+	venv/bin/mypy --python-version 3.10 -p pkgsettings -p tests
+	venv/bin/mypy --python-version 3.11 -p pkgsettings -p tests
 
 .PHONY: format
 format: format/isort format/black
 
 .PHONY: format/isort
 format/isort: venv
 	venv/bin/isort $(SRC)
```

### Comparing `pkgsettings-1.1.0/PKG-INFO` & `pkgsettings-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgsettings
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package to ease the configuration of packages
 Home-page: https://github.com/kpn/py-pkgsettings
 Author: KPN DE Platform
 Author-email: de-platform@kpn.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pkgsettings-1.1.0/README.md` & `pkgsettings-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/docs/Makefile` & `pkgsettings-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/docs/conf.py` & `pkgsettings-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/docs/make.bat` & `pkgsettings-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pkgsettings-1.1.0/pkgsettings/pkgsettings.py` & `pkgsettings-1.1.1/pkgsettings/pkgsettings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 from __future__ import annotations
 
 import functools
+import sys
 import warnings
-from typing import Any, Callable, Dict, Generator, Optional, TypeVar, overload
+from collections.abc import Generator
+from types import TracebackType
+from typing import Any, Callable, cast, overload
 
-from typing_extensions import Self
+from typing_extensions import Literal, ParamSpec, Self, TypeVar
 
-_F = TypeVar("_F", bound=Callable[..., Any])
+if sys.version_info < (3, 9):
+    from typing import ContextManager as AbstractContextManager
+else:
+    from contextlib import AbstractContextManager
+
+
+P = ParamSpec("P")
+T = TypeVar("T")
 
 
 class DuplicateConfigureWarning(UserWarning):
     pass
 
 
 class SimpleSettings:
     """
     A single layer of settings.
 
     Layers get stacked on each other in `Settings`, so allowing to override specific options.
     """
 
-    def as_dict(self) -> Dict[str, Any]:
+    def as_dict(self) -> dict[str, Any]:
         return self.__dict__
 
 
-class Settings:
+class Settings(AbstractContextManager["Settings"]):
     def __init__(self) -> None:
         self._chain = [SimpleSettings()]
-        self._override_settings: Dict[str, Any] = {}
+        self._override_settings: dict[str, Any] = {}
 
     def __getattr__(self, attr: str) -> Any:
         for item in self._chain:
             try:
                 return getattr(item, attr)
             except AttributeError:
                 pass
         raise AttributeError(attr)
 
-    def as_dict(self) -> Dict[str, Any]:
+    def as_dict(self) -> dict[str, Any]:
         result = {}
         for item in reversed(self._chain):
             result.update(item.as_dict())
         return result
 
     def children(self) -> Generator[SimpleSettings, None, None]:
         """
@@ -51,16 +61,15 @@
 
         :return: generator of settings objects.
         """
         for child in self._chain:
             yield child
             children = getattr(child, "children", None)
             if callable(children):
-                for settings in children():
-                    yield settings
+                yield from children()
 
     def _has_duplicates(self) -> bool:
         """
         Check if there are duplicates in the chained settings objects.
 
         :return: True if there are duplicate, False otherwise.
         """
@@ -69,15 +78,15 @@
             if settings in children:
                 return True
 
             children.add(settings)
 
         return False
 
-    def configure(self, obj: Optional[Any] = None, **kwargs) -> None:
+    def configure(self, obj: Any = None, **kwargs: Any) -> None:
         """
         Settings that will be used by the time_execution decorator
 
         Args:
             obj: class or object with the settings as attributes
         """
         if not obj:
@@ -94,64 +103,73 @@
         if self._has_duplicates():
             warnings.warn("One setting was added multiple times, maybe a loop?", DuplicateConfigureWarning)
 
     def __enter__(self) -> Self:
         self._override_enable()
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback) -> None:
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
+    ) -> None:
         self._override_disable()
 
     @overload
-    def __call__(self, func: _F) -> _F:
+    def __call__(self, func: Callable[P, T]) -> Callable[P, T]:
         ...
 
     @overload
-    def __call__(self, **override_settings: Any) -> Self:
+    def __call__(self, func: Literal[None] = None, **override_settings: Any) -> Self:
         ...
 
-    def __call__(self, func=None, **override_settings: Any):
+    def __call__(self, func: Callable[P, T] | None = None, **override_settings: Any) -> Self | Callable[P, T]:
         """
         Override settings for a decorated function.
 
         Example:
              >>> settings = Settings()
              >>>
              >>> @settings(option=42)
              >>> def foo():
              >>>     assert settings.option == 42
         """
 
-        if func:
+        if func is not None:
 
             @functools.wraps(func)
-            def inner(*args, **kwargs):
+            def inner(*args: P.args, **kwargs: P.kwargs) -> T:
                 with self:
-                    return func(*args, **kwargs)
+                    # Cast is necessary since otherwise mypy thinks
+                    # that the inner function is Optional[Callable]
+                    # type. See related bug
+                    # https://github.com/python/mypy/issues/15251
+                    return cast(Callable[P, T], func)(*args, **kwargs)
 
             return inner
 
         elif override_settings:
             self._override_settings = override_settings
-            return self
+        return self
 
     def _override_enable(self) -> None:
         obj = SimpleSettings()
         for key, new_value in self._override_settings.items():
             setattr(obj, key, new_value)
 
         self._chain.insert(0, obj)
 
     def _override_disable(self) -> None:
         self._chain.pop(0)
         self._override_settings = {}
 
 
 class PrefixedSettings:
-    def __init__(self, settings: Any, prefix: Optional[str] = None) -> None:
+    def __init__(self, settings: Any, prefix: str | None = None) -> None:
         self.settings = settings
         self.prefix = prefix
 
     def __getattr__(self, attr: str) -> Any:
         if self.prefix:
             attr = self.prefix + attr
         return getattr(self.settings, attr)
```

### Comparing `pkgsettings-1.1.0/pkgsettings.egg-info/PKG-INFO` & `pkgsettings-1.1.1/pkgsettings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgsettings
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package to ease the configuration of packages
 Home-page: https://github.com/kpn/py-pkgsettings
 Author: KPN DE Platform
 Author-email: de-platform@kpn.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pkgsettings-1.1.0/pyproject.toml` & `pkgsettings-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 [tool.setuptools_scm]
 
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm[toml]>=3.4"]
 
 [tool.mypy]
 check_untyped_defs = true
+strict = true
```

### Comparing `pkgsettings-1.1.0/setup.py` & `pkgsettings-1.1.1/setup.py`

 * *Files identical despite different names*

