# Comparing `tmp/polyfactory-2.1.0.tar.gz` & `tmp/polyfactory-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.1.0.tar", max compression
+gzip compressed data, was "polyfactory-2.1.1.tar", max compression
```

## Comparing `polyfactory-2.1.0.tar` & `polyfactory-2.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1092 2023-05-06 15:37:10.553226 polyfactory-2.1.0/LICENSE
--rw-r--r--   0        0        0     9082 2023-05-06 15:37:10.553226 polyfactory-2.1.0/README.md
--rw-r--r--   0        0        0      425 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/__init__.py
--rw-r--r--   0        0        0      642 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    30193 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2757 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1603 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2193 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0     7389 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1471 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     2939 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3328 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/fields.py
--rw-r--r--   0        0        0     1191 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/py.typed
--rw-r--r--   0        0        0     2890 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3401 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     2812 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1838 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13431 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0     3845 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0     3633 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6030 2023-05-06 15:37:10.557226 polyfactory-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    11105 1970-01-01 00:00:00.000000 polyfactory-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-17 19:31:53.700877 polyfactory-2.1.1/LICENSE
+-rw-r--r--   0        0        0     9082 2023-05-17 19:31:53.700877 polyfactory-2.1.1/README.md
+-rw-r--r--   0        0        0      425 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    30193 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2757 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1603 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2193 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0     7552 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1471 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     2939 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3328 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/fields.py
+-rw-r--r--   0        0        0     1191 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/py.typed
+-rw-r--r--   0        0        0     2890 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3401 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     2807 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1838 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13431 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0     3845 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0     3635 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6185 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6030 2023-05-17 19:31:53.704877 polyfactory-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11105 1970-01-01 00:00:00.000000 polyfactory-2.1.1/PKG-INFO
```

### Comparing `polyfactory-2.1.0/LICENSE` & `polyfactory-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/README.md` & `polyfactory-2.1.1/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -102,17 +102,17 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
```

### Comparing `polyfactory-2.1.0/polyfactory/constants.py` & `polyfactory-2.1.1/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/decorators.py` & `polyfactory-2.1.1/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/exceptions.py` & `polyfactory-2.1.1/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/factories/base.py` & `polyfactory-2.1.1/polyfactory/factories/base.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.1.1/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.1.1/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.1.1/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.1.1/polyfactory/factories/pydantic_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,38 +64,45 @@
         if callable(model_field.default_factory):
             default_value = model_field.default_factory()
         else:
             default_value = model_field.default if model_field.default is not Undefined else Null
 
         name = model_field.alias if model_field.alias and use_alias else model_field.name
 
-        annotation = unwrap_new_type(
-            model_field.annotation if not isinstance(model_field.annotation, DeferredType) else model_field.outer_type_
+        outer_type = unwrap_new_type(model_field.outer_type_)
+        annotation = (
+            unwrap_new_type(model_field.annotation)
+            if not isinstance(model_field.annotation, DeferredType)
+            else outer_type
         )
 
         constraints = cast(
             "Constraints",
             {
                 "constant": bool(model_field.field_info.const) or None,
-                "ge": getattr(annotation, "ge", model_field.field_info.ge),
-                "gt": getattr(annotation, "gt", model_field.field_info.gt),
-                "le": getattr(annotation, "le", model_field.field_info.le),
-                "lt": getattr(annotation, "lt", model_field.field_info.lt),
-                "min_length": getattr(annotation, "min_length", model_field.field_info.min_length)
-                or getattr(annotation, "min_items", model_field.field_info.min_items),
-                "max_length": getattr(annotation, "max_length", model_field.field_info.max_length)
-                or getattr(annotation, "max_items", model_field.field_info.max_items),
-                "pattern": getattr(annotation, "regex", model_field.field_info.regex),
-                "unique_items": getattr(annotation, "unique_items", model_field.field_info.unique_items),
-                "decimal_places": getattr(annotation, "decimal_places", None),
-                "max_digits": getattr(annotation, "max_digits", None),
-                "multiple_of": getattr(annotation, "multiple_of", None),
-                "upper_case": getattr(annotation, "to_upper", None),
-                "lower_case": getattr(annotation, "to_lower", None),
-                "item_type": getattr(annotation, "item_type", None),
+                "ge": getattr(outer_type, "ge", model_field.field_info.ge),
+                "gt": getattr(outer_type, "gt", model_field.field_info.gt),
+                "le": getattr(outer_type, "le", model_field.field_info.le),
+                "lt": getattr(outer_type, "lt", model_field.field_info.lt),
+                "min_length": (
+                    getattr(outer_type, "min_length", model_field.field_info.min_length)
+                    or getattr(outer_type, "min_items", model_field.field_info.min_items)
+                ),
+                "max_length": (
+                    getattr(outer_type, "max_length", model_field.field_info.max_length)
+                    or getattr(outer_type, "max_items", model_field.field_info.max_items)
+                ),
+                "pattern": getattr(outer_type, "regex", model_field.field_info.regex),
+                "unique_items": getattr(outer_type, "unique_items", model_field.field_info.unique_items),
+                "decimal_places": getattr(outer_type, "decimal_places", None),
+                "max_digits": getattr(outer_type, "max_digits", None),
+                "multiple_of": getattr(outer_type, "multiple_of", None),
+                "upper_case": getattr(outer_type, "to_upper", None),
+                "lower_case": getattr(outer_type, "to_lower", None),
+                "item_type": getattr(outer_type, "item_type", None),
             },
         )
 
         children: list[FieldMeta] = []
         if model_field.key_field:
             children.append(PydanticFieldMeta.from_model_field(model_field.key_field, use_alias))
         if model_field.sub_fields:
```

### Comparing `polyfactory-2.1.0/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.1.1/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/field_meta.py` & `polyfactory-2.1.1/polyfactory/field_meta.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/fields.py` & `polyfactory-2.1.1/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/persistence.py` & `polyfactory-2.1.1/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/pytest_plugin.py` & `polyfactory-2.1.1/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/utils/helpers.py` & `polyfactory-2.1.1/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/utils/predicates.py` & `polyfactory-2.1.1/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/value_generators/complex_types.py` & `polyfactory-2.1.1/polyfactory/value_generators/complex_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,13 +60,13 @@
     """
     if origin := get_type_origin(unwrap_annotation(field_meta.annotation)):
         if issubclass(origin, Collection):
             return handle_collection_type(field_meta, origin, factory)
         return factory.get_mock_value(origin)
 
     if is_union(field_meta.annotation) and field_meta.children:
-        return handle_complex_type(factory.__random__.choice(field_meta.children), factory)
+        return factory.get_field_value(factory.__random__.choice(field_meta.children))
 
     if is_any(field_meta.annotation) or isinstance(field_meta.annotation, TypeVar):
         return create_random_string(factory.__random__, min_length=1, max_length=10)
 
     return factory.get_field_value(field_meta)
```

### Comparing `polyfactory-2.1.0/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.1.1/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.1.1/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.1.1/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.1.1/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/polyfactory/value_generators/primitives.py` & `polyfactory-2.1.1/polyfactory/value_generators/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     :param random: An instance of random.
     :param minimum: A minimum value
     :param maximum: A maximum value.
 
     :returns: A random integer.
     """
-    return int(create_random_float(random=random, minimum=minimum, maximum=maximum))
+    return round(create_random_float(random=random, minimum=minimum, maximum=maximum))
 
 
 def create_random_decimal(
     random: Random,
     minimum: Decimal | None = None,
     maximum: Decimal | None = None,
 ) -> Decimal:
```

### Comparing `polyfactory-2.1.0/polyfactory/value_generators/regex.py` & `polyfactory-2.1.1/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.0/pyproject.toml` & `polyfactory-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.1.0"
+version = "2.1.1"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
```

### Comparing `polyfactory-2.1.0/PKG-INFO` & `polyfactory-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.1.0
+Version: 2.1.1
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: dataclasses,factory,faker,mock,pydantic,pytest,litestar,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -149,17 +149,17 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
```

