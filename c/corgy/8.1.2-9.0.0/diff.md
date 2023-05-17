# Comparing `tmp/corgy-8.1.2.tar.gz` & `tmp/corgy-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-8.1.2.tar", max compression
+gzip compressed data, was "corgy-9.0.0.tar", max compression
```

## Comparing `corgy-8.1.2.tar` & `corgy-9.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    30621 2023-05-16 00:52:41.060122 corgy-8.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-05-16 00:52:41.060122 corgy-8.1.2/LICENSE
--rw-r--r--   0        0        0     4196 2023-05-16 00:52:41.060122 corgy-8.1.2/README.md
--rw-r--r--   0        0        0      468 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_annotations.py
--rw-r--r--   0        0        0    49762 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_corgy.py
--rw-r--r--   0        0        0     3202 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_corgychecker.py
--rw-r--r--   0        0        0     6237 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_corgyparser.py
--rw-r--r--   0        0        0    36993 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_helpfmt.py
--rw-r--r--   0        0        0    18742 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-05-16 00:53:17.388231 corgy-8.1.2/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_expand.py
--rw-r--r--   0        0        0     3413 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_subclass.py
--rw-r--r--   0        0        0    35296 2023-05-16 00:52:41.064122 corgy-8.1.2/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-05-16 00:52:41.064122 corgy-8.1.2/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-05-16 00:52:41.064122 corgy-8.1.2/docs/index.md
--rw-r--r--   0        0        0     2679 2023-05-16 00:53:17.384231 corgy-8.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/__init__.py
--rw-r--r--   0        0        0    90410 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_corgy.py
--rw-r--r--   0        0        0     4240 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_corgychecker.py
--rw-r--r--   0        0        0    16681 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_corgyparser.py
--rw-r--r--   0        0        0      800 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_doctests.py
--rw-r--r--   0        0        0    47095 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-8.1.2/PKG-INFO
+-rw-r--r--   0        0        0    31468 2023-05-17 09:39:56.515288 corgy-9.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-05-17 09:39:56.515288 corgy-9.0.0/LICENSE
+-rw-r--r--   0        0        0     4196 2023-05-17 09:39:56.515288 corgy-9.0.0/README.md
+-rw-r--r--   0        0        0      468 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_annotations.py
+-rw-r--r--   0        0        0    49963 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_corgy.py
+-rw-r--r--   0        0        0     3202 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_corgychecker.py
+-rw-r--r--   0        0        0     6237 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    36993 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    18742 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-05-17 09:40:32.351710 corgy-9.0.0/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3750 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-05-17 09:39:56.515288 corgy-9.0.0/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    35396 2023-05-17 09:39:56.515288 corgy-9.0.0/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-05-17 09:39:56.515288 corgy-9.0.0/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-05-17 09:39:56.515288 corgy-9.0.0/docs/index.md
+-rw-r--r--   0        0        0     2679 2023-05-17 09:40:32.351710 corgy-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    90889 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_corgy.py
+-rw-r--r--   0        0        0     4240 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_corgychecker.py
+-rw-r--r--   0        0        0    16681 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      800 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_doctests.py
+-rw-r--r--   0        0        0    47095 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-05-17 09:39:56.519288 corgy-9.0.0/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-9.0.0/PKG-INFO
```

### Comparing `corgy-8.1.2/CHANGELOG.md` & `corgy-9.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [9.0.0](https://github.com/jayanthkoushik/corgy/compare/v8.1.2...v9.0.0) (2023-05-17)
+
+
+### ⚠ BREAKING CHANGES
+
+* `Corgy.add_args_to_parser` no longer uses `store_`
+actions for types with a single choice defined using `__choices__`. Only
+`Literal` types receive this special treatment.
+
+### Features
+
+* in `Corgy.add_args_to_parser`, restrict handling of single choice attrs to `Literal` types ([5d1bfcc](https://github.com/jayanthkoushik/corgy/commit/5d1bfcce520efa2f97ddface800c67745449eb6d))
+* raise informative error if `types.InitArgs` cannot be used ([61e79c3](https://github.com/jayanthkoushik/corgy/commit/61e79c39ca6ff9fd7ec7fac21e6698928bdbccd2))
+
+
+### Bug Fixes
+
+* make arguments without defaults be required in `types.InitArgs` ([5cb533b](https://github.com/jayanthkoushik/corgy/commit/5cb533b5da87f921aba1973d4deab1266e14f48b))
+
 ### [8.1.2](https://github.com/jayanthkoushik/corgy/compare/v8.1.1...v8.1.2) (2023-05-16)
 
 
 ### Bug Fixes
 
 * inherit `corgy_` parameters for `Corgy` sub-classes ([9e87e4d](https://github.com/jayanthkoushik/corgy/commit/9e87e4d5fb0a58c63d0c2e7cd4aaff33ecf47aef))
```

### Comparing `corgy-8.1.2/LICENSE` & `corgy-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/README.md` & `corgy-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/_actions.py` & `corgy-9.0.0/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/_corgy.py` & `corgy-9.0.0/corgy/_corgy.py`

 * *Files 1% similar despite different names*

```diff
@@ -656,14 +656,17 @@
             >>> parser.parse_args(["--x"])  # Note that `y` and `z` are absent
             Namespace(x=True)
             >>> parser.parse_args(["--y"])
             Namespace(y=False)
             >>> parser.parse_args(["--z"])
             Namespace(z=42)
 
+        Note: This special case only applies to `Literal` types, and not types which
+        define `__choices__`.
+
         *Corgy*
         Attributes which are themselves `Corgy` types are treated as argument groups.
         Group arguments are added to the command line parser with the group attribute
         name prefixed. Note that groups will ignore any custom flags when computing the
         prefix; elements within the group will use custom flags, but because they are
         prefixed with `--`, they will not be positional.
 
@@ -821,15 +824,16 @@
                             f"`{var_name}` has unsupported type `{var_base_type}`: only"
                             f" single-type collections are supported"
                         )
                     var_nargs = len(var_base_type.__args__)
                 var_base_type = var_base_type.__args__[0]
 
             # Check if the variable has choices.
-            if is_literal_type(var_base_type):
+            _is_literal_type = is_literal_type(var_base_type)
+            if _is_literal_type:
                 # Determine if the first choice has `__bases__`, in which case
                 # the first base class is the type for the argument.
                 try:
                     c0_type = var_base_type.__args__[0].__bases__[0]
                 except AttributeError:
                     c0_type = type(var_base_type.__args__[0])
                     f_check_type: Callable[[Any, Any], bool] = isinstance
@@ -857,14 +861,15 @@
 
             # Convert single choice attributes to `store_*` actions.
             if (
                 var_choices is not None
                 and len(var_choices) == 1
                 and var_nargs is None
                 and var_action is None
+                and _is_literal_type
             ):
                 _choice = var_choices[0]
                 if _choice is True:
                     var_action = _StoreTrueAction
                     var_const = None
                 elif _choice is False:
                     var_action = _StoreFalseAction
```

### Comparing `corgy-8.1.2/corgy/_corgychecker.py` & `corgy-9.0.0/corgy/_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/_corgyparser.py` & `corgy-9.0.0/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/_helpfmt.py` & `corgy-9.0.0/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/_meta.py` & `corgy-9.0.0/corgy/_meta.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/types/__init__.py` & `corgy-9.0.0/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/types/_expand.py` & `corgy-9.0.0/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/types/_initargs.py` & `corgy-9.0.0/corgy/types/_initargs.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from corgy import Corgy
 
 __all__ = ("InitArgs",)
 _T = TypeVar("_T")
 
 
-class InitArgs(Corgy, Generic[_T]):
+class InitArgs(Corgy, Generic[_T], corgy_required_by_default=True):
     """Corgy wrapper around arguments of a class's `__init__`.
 
     Example::
 
         >>> import argparse
         >>> from argparse import ArgumentParser
         >>> from typing import Sequence
@@ -35,16 +35,16 @@
         ...     formatter_class=CorgyHelpFormatter,
         ...     add_help=False,
         ...     usage=argparse.SUPPRESS,
         ... )
         >>> FooInitArgs.add_args_to_parser(parser)
         >>> parser.print_help()
         options:
-          --a int        (optional)
-          --b [str ...]  (optional)
+          --a int        (required)
+          --b [str ...]  (required)
           --c float      (default: 0.0)
 
         >>> args = parser.parse_args(["--a", "1", "--b", "one", "two"])
         >>> foo = Foo(args.a, args.b, args.c)
 
     This is a generic class, and on using the `InitArgs[Cls]` syntax, a concrete
     `Corgy` class is created, which has attributes corresponding to the arguments of
@@ -57,14 +57,20 @@
     they are not associated with an argument name. `TypeError` is raised if either of
     these conditions is not met.
     """
 
     __slots__ = ()
 
     def __class_getitem__(cls, item: Type[_T]) -> Type[InitArgs[_T]]:
+        try:
+            is_generic = issubclass(item, Generic)  # type: ignore
+        except TypeError as e:
+            raise TypeError(f"could not perform class test on `{item}`: {e}") from None
+        if is_generic:
+            raise TypeError(f"{cls.__name__} cannot be used with generic classes")
         item_sig = inspect.signature(item)
         item_annotations, item_defaults = {}, {}
         for param_name, param in item_sig.parameters.items():
             if param.annotation is inspect.Parameter.empty:
                 raise TypeError(
                     f"`{item}` is missing annotation for parameter `{param_name}`"
                 )
```

### Comparing `corgy-8.1.2/corgy/types/_inputfile.py` & `corgy-9.0.0/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/types/_keyvaluepairs.py` & `corgy-9.0.0/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/types/_outputfile.py` & `corgy-9.0.0/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/corgy/types/_subclass.py` & `corgy-9.0.0/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/docs/corgy.md` & `corgy-9.0.0/docs/corgy.md`

 * *Files 0% similar despite different names*

```diff
@@ -694,14 +694,17 @@
 Namespace(x=True)
 >>> parser.parse_args(["--y"])
 Namespace(y=False)
 >>> parser.parse_args(["--z"])
 Namespace(z=42)
 ```
 
+Note: This special case only applies to `Literal` types, and not types which
+define `__choices__`.
+
 *Corgy*
 Attributes which are themselves `Corgy` types are treated as argument groups.
 Group arguments are added to the command line parser with the group attribute
 name prefixed. Note that groups will ignore any custom flags when computing the
 prefix; elements within the group will use custom flags, but because they are
 prefixed with `--`, they will not be positional.
```

### Comparing `corgy-8.1.2/docs/corgy.types.md` & `corgy-9.0.0/docs/corgy.types.md`

 * *Files 1% similar despite different names*

```diff
@@ -348,16 +348,16 @@
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
 ...     usage=argparse.SUPPRESS,
 ... )
 >>> FooInitArgs.add_args_to_parser(parser)
 >>> parser.print_help()
 options:
-  --a int        (optional)
-  --b [str ...]  (optional)
+  --a int        (required)
+  --b [str ...]  (required)
   --c float      (default: 0.0)
 
 >>> args = parser.parse_args(["--a", "1", "--b", "one", "two"])
 >>> foo = Foo(args.a, args.b, args.c)
 ```
 
 This is a generic class, and on using the `InitArgs[Cls]` syntax, a concrete
```

### Comparing `corgy-8.1.2/pyproject.toml` & `corgy-9.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "8.1.2"  # managed by `poetry-dynamic-versioning`
+version = "9.0.0"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
```

### Comparing `corgy-8.1.2/tests/test_corgy.py` & `corgy-9.0.0/tests/test_corgy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1800,17 +1800,22 @@
             with self.subTest(type=type_):
 
                 class C(Corgy):
                     x: type_
 
                 self.setUp()
                 C.add_args_to_parser(self.parser)
-                self.parser.add_argument.assert_called_once_with(
-                    "--x", action=_StoreConstAction, const=42, required=True
-                )
+                if type_ is A:
+                    self.parser.add_argument.assert_called_once_with(
+                        "--x", type=A, choices=(42,), required=True
+                    )
+                else:
+                    self.parser.add_argument.assert_called_once_with(
+                        "--x", action=_StoreConstAction, const=42, required=True
+                    )
 
     def test_add_args_uses_store_true_false_action_for_true_false_literal(self):
         for val in (True, False):
 
             class A:
                 __choices__ = (val,)
 
@@ -1818,19 +1823,24 @@
                 with self.subTest(val=val, type=type_):
 
                     class C(Corgy):
                         x: type_
 
                     self.setUp()
                     C.add_args_to_parser(self.parser)
-                    self.parser.add_argument.assert_called_once_with(
-                        "--x",
-                        action=(_StoreTrueAction if val else _StoreFalseAction),
-                        required=True,
-                    )
+                    if type_ is A:
+                        self.parser.add_argument.assert_called_once_with(
+                            "--x", type=A, choices=(val,), required=True
+                        )
+                    else:
+                        self.parser.add_argument.assert_called_once_with(
+                            "--x",
+                            action=(_StoreTrueAction if val else _StoreFalseAction),
+                            required=True,
+                        )
 
     def test_add_args_handles_user_defined_class_as_type(self):
         class T:
             ...
 
         class C(Corgy):
             x: T
```

### Comparing `corgy-8.1.2/tests/test_corgychecker.py` & `corgy-9.0.0/tests/test_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/test_corgyparser.py` & `corgy-9.0.0/tests/test_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/test_doctests.py` & `corgy-9.0.0/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/test_helpfmt.py` & `corgy-9.0.0/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/types/_specialtmps.py` & `corgy-9.0.0/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/types/_test_file.py` & `corgy-9.0.0/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/types/test_initargs.py` & `corgy-9.0.0/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/types/test_inputfiles.py` & `corgy-9.0.0/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/types/test_keyvaluepairs.py` & `corgy-9.0.0/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/types/test_outputfiles.py` & `corgy-9.0.0/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/tests/types/test_subclass.py` & `corgy-9.0.0/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.2/PKG-INFO` & `corgy-9.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 8.1.2
+Version: 9.0.0
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
```

