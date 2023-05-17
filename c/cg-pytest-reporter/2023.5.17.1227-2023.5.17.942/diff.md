# Comparing `tmp/cg_pytest_reporter-2023.5.17.1227.tar.gz` & `tmp/cg_pytest_reporter-2023.5.17.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_pytest_reporter-2023.5.17.1227.tar", max compression
+gzip compressed data, was "cg_pytest_reporter-2023.5.17.942.tar", max compression
```

## Comparing `cg_pytest_reporter-2023.5.17.1227.tar` & `cg_pytest_reporter-2023.5.17.942.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       21 2023-05-17 12:27:21.699639 cg_pytest_reporter-2023.5.17.1227/README.md
--rw-r--r--   0        0        0      422 2023-05-17 12:27:21.699639 cg_pytest_reporter-2023.5.17.1227/cg_pytest_reporter/__init__.py
--rw-r--r--   0        0        0    17704 2023-05-17 12:27:21.699639 cg_pytest_reporter-2023.5.17.1227/cg_pytest_reporter/plugin.py
--rw-r--r--   0        0        0     1809 2023-05-17 12:27:43.636021 cg_pytest_reporter-2023.5.17.1227/pyproject.toml
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.17.1227/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/README.md
+-rw-r--r--   0        0        0      422 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/__init__.py
+-rw-r--r--   0        0        0    17620 2023-05-17 09:42:07.964449 cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/plugin.py
+-rw-r--r--   0        0        0     1810 2023-05-17 09:42:33.186790 cg_pytest_reporter-2023.5.17.942/pyproject.toml
+-rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.17.942/PKG-INFO
```

### Comparing `cg_pytest_reporter-2023.5.17.1227/cg_pytest_reporter/plugin.py` & `cg_pytest_reporter-2023.5.17.942/cg_pytest_reporter/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,26 +102,26 @@
 
 @dataclasses.dataclass
 class CgMarks:
     """Marks set on each test case by the `cg-pytest-reporter` plugin used when
     generating the report.
     """
     #: The name of the test suite.
-    suite_name: t.Optional[str]
+    suite_name: str | None
     #: The weight of the test suite.
-    suite_weight: t.Union[int, float, None]
+    suite_weight: int | float | None
 
     #: The name of the test case.
-    name: t.Optional[str]
+    name: str | None
     #: The description of the test case.
-    description: t.Optional[str]
+    description: str | None
     #: The weight of the test case.
-    weight: t.Union[int, float, None]
+    weight: int | float | None
     #: The reason the test failed.
-    reason: t.Optional[str]
+    reason: str | None
     #: The stdout produced while running the test.
     hide_stdout: bool
     #: The stderr produced while running the test.
     hide_stderr: bool
 
     @classmethod
     def from_item(cls, item: pytest.Item) -> 'CgMarks':
@@ -148,47 +148,47 @@
         )
 
     @classmethod
     def _get_suite_mark_value(
         cls,
         item: pytest.Item,
         name: str,
-    ) -> t.Optional[object]:
+    ) -> object | None:
         # It is not possible to add marks on the module level because you cannot
         # call a decorator on a module. So on the module level we allow a custom
         # name and weight by setting the `__cg_suite_{name,weight}__` variables
         # at the top level of the module.
         if isinstance(item.parent, pytest.Module):
             # Pytest offers no way to get the module object from a `Module` node.
             # pylint: disable=protected-access
             return getattr(item.parent._obj, f'__{name}__', None)
         else:
             return cls._get_mark_value(item.parent, name)
 
     @classmethod
     def _get_mark_value(
         cls,
-        item: t.Optional[_pytest.nodes.Node],
+        item: _pytest.nodes.Node | None,
         name: str,
-    ) -> t.Optional[object]:
+    ) -> object | None:
         if item is None:
             return None
-        mark: t.Optional[pytest.Mark] = item.get_closest_marker(name)
+        mark: pytest.Mark | None = item.get_closest_marker(name)
         if mark is None or not mark.args:
             return None
         return mark.args[0]
 
     @staticmethod
-    def _as_str(obj: object) -> t.Optional[str]:
+    def _as_str(obj: object) -> str | None:
         if isinstance(obj, str):
             return obj
         return None
 
     @staticmethod
-    def _as_num(obj: object) -> t.Union[float, int, None]:
+    def _as_num(obj: object) -> float | int | None:
         if isinstance(obj, (int, float)):
             return obj
         return None
 
 
 class CGPytestReporterPlugin:
     """Implementation of the reporter plugin.
@@ -358,17 +358,16 @@
         that the smaller one of stdout and stderr is included, and finally the
         other one as well.
         """
         def jsonlen(obj: object) -> int:
             return len(json_dumps(obj))
 
         def field_length(
-            dct: t.Mapping[str, object],
-            field: str,
-        ) -> t.Optional[int]:
+            dct: t.Mapping[str, object], field: str
+        ) -> int | None:
             val = dct.get(field)
             if val is None:
                 return None
 
             length = len(f'"{field}":')
             if isinstance(val, str):
                 # Add 2 for the quotes.
```

### Comparing `cg_pytest_reporter-2023.5.17.1227/pyproject.toml` & `cg_pytest_reporter-2023.5.17.942/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "cg-pytest-reporter"
-version = "2023.05.17.1227"
+version = "2023.05.17.0942"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{include = "cg_pytest_reporter"}]
 
 [tool.poetry.plugins.pytest11]
 cg_pytest_reporter = "cg_pytest_reporter.plugin"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pytest = ">=7.0.0"
+python = "^3.10"
+pytest = ">=7.3.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 pylint = "^2.17.4"
 yapf = "^0.33.0"
 isort = "^5.12.0"
```

