# Comparing `tmp/rpycocotools_stubs-0.0.5.tar.gz` & `tmp/rpycocotools_stubs-0.0.6.tar.gz`

## Comparing `rpycocotools_stubs-0.0.5.tar` & `rpycocotools_stubs-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/requirements/README.md
--rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/requirements/requirements-build.txt
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/requirements/requirements.txt
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/src/rpycocotools-stubs/__init__.pyi
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/src/rpycocotools-stubs/anns.pyi
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/src/rpycocotools-stubs/mask.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/src/rpycocotools-stubs/py.typed
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/LICENSE
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/README.md
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/requirements/README.md
+-rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/requirements/requirements-build.txt
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/requirements/requirements-flake8.txt
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/requirements/requirements.txt
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/src/rpycocotools-stubs/__init__.pyi
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/src/rpycocotools-stubs/anns.pyi
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/src/rpycocotools-stubs/mask.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/src/rpycocotools-stubs/py.typed
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/LICENSE
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/README.md
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.6/PKG-INFO
```

### Comparing `rpycocotools_stubs-0.0.5/requirements/requirements-build.txt` & `rpycocotools_stubs-0.0.6/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools_stubs-0.0.5/requirements/requirements-dev.txt` & `rpycocotools_stubs-0.0.6/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools_stubs-0.0.5/requirements/requirements.txt` & `rpycocotools_stubs-0.0.6/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools_stubs-0.0.5/src/rpycocotools-stubs/mask.pyi` & `rpycocotools_stubs-0.0.6/src/rpycocotools-stubs/mask.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 @overload
 def encode(mask: npt.NDArray[np.uint8],
            target: Literal["polygons"],
            ) -> Polygons:
     ...
 
 def encode(mask: npt.NDArray[np.uint8],
-           target: Literal["polygons"] | Literal["rle"] | Literal["coco_rle"] | Literal["polygons_rs"],
+           target: Literal["polygons", "rle", "coco_rle", "polygons_rs"],
            ) -> Polygons | RLE | COCO_RLE | PolygonsRS:
     """Encode/compress a mask into the desired format.
 
     Args:
         mask: The mask to encode, it should be a 2 dimensional array.
         target: The desired format for the encoded mask.
```

### Comparing `rpycocotools_stubs-0.0.5/LICENSE` & `rpycocotools_stubs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rpycocotools_stubs-0.0.5/pyproject.toml` & `rpycocotools_stubs-0.0.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -25,20 +25,35 @@
 dependencies = ["typing_extensions>=4.0", "numpy>=1.21.0"]
 requires-python = ">=3.8"
 packages = [
     { "include" = "rpycocotools-stubs"}
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/hoel-bagard/rpycocotools-stubs"
-"Bug Tracker" = "https://github.com/hoel-bagard/rpycocotools-stubs/issues"
+"Homepage" = "https://github.com/hoel-bagard/cocotools-rs/tree/master/rpycocotools-stubs"
+"Bug Tracker" = "https://github.com/hoel-bagard/cocotools-rs/issues"
 
 [project.optional-dependencies]
-dev = ["pre-commit", "pip-tools", "ruff", "pyright"]
+dev = ["pip-tools", "ruff", "pyright"]
 build = ["hatch"]
+flake8 = [
+    "flake8>=5.0.4,<6.0",
+    "flake8-bugbear>=23.3.12,<24.0",
+    "flake8-builtins>=2.1.0,<3.0",
+    "flake8-comprehensions>=3.12.0,<4.0",
+    "flake8-docstrings>=1.7.0,<2.0",
+    "flake8-quotes>=3.3.2,<4",
+    "pep8-naming>=0.13.3",
+    "flake8-import-order>=0.18.2",
+    "flake8-noqa>=1.3.1,<2",
+    "flake8-broken-line>=0.6.0",
+    "flake8-commas>=2.1.0,<3.0",
+    "flake8-pyi>=23.5.0",
+    "Flake8-pyproject>=1.2.3,<2"
+]
 
 [tool.hatch.version]
 path = "src/rpycocotools-stubs/__init__.pyi"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
@@ -53,34 +68,34 @@
 
 [tool.hatch.envs.pypi.scripts]
 # hatch run pypi:publish_test
 publish_test = "hatch build --clean && hatch publish -r test"
 publish = "hatch build --clean && hatch publish"
 
 [tool.ruff]
-select = ["A", "B", "C4", "D", "E", "F", "N", "I", "Q", "UP", "ANN", "S", "BLE", "COM", "DTZ", "PIE", "PT", "RSE", "SIM","PTH", "PL", "TRY", "NPY", "RUF"]
-# D407: Missing dashed underline after section ("Args", "Returns", etc...)
-ignore = ["A002", "A003", "D1", "D204", "D203", "D213", "D401", "D407", "S101", "PLR2004"]
+select = ["ALL"]
+# A002/A003 Argument/Class attribute `id` is shadowing a python builtin
+# D1: Missing docstring
+# FBT001: Boolean positional arg in function definition
+# PYI021: Docstrings should not be included in stubs
+ignore = ["A002", "A003", "D1", "FBT001", "PYI021"]
 line-length = 120
 
 [tool.ruff.isort]
 order-by-type = false
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.pylint]
 max-args = 10
 
-[tool.ruff.per-file-ignores]
-"__init__.py" = ["F401"]
-
 [tool.pyright]
 include = ["src/rpycocotools-stubs"]
 pythonVersion = "3.11"
 pythonPlatform = "Linux"
 
 strictListInference = true
 strictDictionaryInference = true
@@ -108,7 +123,23 @@
 reportUnnecessaryCast = "warning"
 reportUnnecessaryComparison = "warning"
 reportImplicitStringConcatenation = false
 reportUnusedCallResult = false
 reportUnusedExpression = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
 reportMatchNotExhaustive = "warning"
+
+[tool.flake8]
+application_import_names = "rpycocotools"
+exclude = ["env", "venv", "docs"]
+max-line-length = 120
+docstring-convention = "google"
+import-order-style = "smarkets"
+inline-quotes = "double"
+# A002/A003 Argument/Class attribute `id` is shadowing a python builtin
+# D1: Missing docstring
+# E301/E302: expected 1/2 blank lines, found 0/1
+# E305: expected 2 blank lines after class or function definition, found 1
+# E704: multiple statements on one line (def)
+# Y021: Docstrings should not be included in stubs
+# Y048: Function body should contain exactly one statement  -> This doesn't allow for docstrings
+ignore = ["A002", "A003", "D1", "E301", "E302", "E305", "E704", "NQA103", "Y021", "Y048"]
```

