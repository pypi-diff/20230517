# Comparing `tmp/ever_playground-0.4.1.tar.gz` & `tmp/ever_playground-0.4.2.tar.gz`

## Comparing `ever_playground-0.4.1.tar` & `ever_playground-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 ever_playground-0.4.1/Cargo.toml
--rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.4.1/.gitignore
--rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.4.1/.vscode/settings.json
--rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.4.1/README.md
--rw-rw-r--   0     1000     1000     2459 2023-05-15 16:42:04.000000 ever_playground-0.4.1/ever_playground/__init__.py
--rw-rw-r--   0     1000     1000     4627 2023-05-17 11:29:17.000000 ever_playground-0.4.1/ever_playground/ever_playground.pyi
--rw-rw-r--   0     1000     1000     4363 2023-05-16 17:02:44.000000 ever_playground-0.4.1/examples.py
--rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.4.1/pyproject.toml
--rw-rw-r--   0     1000     1000    14446 2023-05-17 11:29:09.000000 ever_playground-0.4.1/src/lib.rs
--rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.4.1/src/tests.rs
--rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.4.1/src/utils.rs
--rw-rw-r--   0     1000     1000    24701 2023-05-17 11:42:29.000000 ever_playground-0.4.1/Cargo.lock
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 ever_playground-0.4.2/Cargo.toml
+-rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.4.2/.gitignore
+-rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.4.2/.vscode/settings.json
+-rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.4.2/README.md
+-rw-rw-r--   0     1000     1000     2484 2023-05-17 14:29:51.000000 ever_playground-0.4.2/ever_playground/__init__.py
+-rw-rw-r--   0     1000     1000     4627 2023-05-17 11:29:17.000000 ever_playground-0.4.2/ever_playground/ever_playground.pyi
+-rw-rw-r--   0     1000     1000     4363 2023-05-16 17:02:44.000000 ever_playground-0.4.2/examples.py
+-rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.4.2/pyproject.toml
+-rw-rw-r--   0     1000     1000    14446 2023-05-17 11:29:09.000000 ever_playground-0.4.2/src/lib.rs
+-rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.4.2/src/tests.rs
+-rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.4.2/src/utils.rs
+-rw-rw-r--   0     1000     1000    24701 2023-05-17 14:31:56.000000 ever_playground-0.4.2/Cargo.lock
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.4.2/PKG-INFO
```

### Comparing `ever_playground-0.4.1/Cargo.toml` & `ever_playground-0.4.2/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ever-playground"
-version = "0.4.1"
+version = "0.4.2"
 edition = "2021"
 
 [lib]
 name = "ever_playground"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `ever_playground-0.4.1/README.md` & `ever_playground-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.1/ever_playground/__init__.py` & `ever_playground-0.4.2/ever_playground/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+from typing import Tuple
 
 from .ever_playground import Cell, Builder, Slice, Dictionary, assemble, runvm
 
 __all__ = [
     "Cell",
     "Builder",
     "Slice",
@@ -27,15 +28,15 @@
     CellUnderflow = 9
     DictionaryError = 10
     UnknownError = 11
     FatalError = 12
     OutOfGas = 13
     IllegalInstruction = 14
 
-def parse_smc_addr(addr_string: str) -> tuple[int, int]:
+def parse_smc_addr(addr_string: str) -> Tuple[int, int]:
     addr_pair = addr_string.split(":")
     assert(len(addr_pair) == 2)
     wc = int(addr_pair[0])
     addr = int(addr_pair[1], 16)
     return wc, addr
 
 class StateInit:
```

### Comparing `ever_playground-0.4.1/ever_playground/ever_playground.pyi` & `ever_playground-0.4.2/ever_playground/ever_playground.pyi`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.1/examples.py` & `ever_playground-0.4.2/examples.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.1/pyproject.toml` & `ever_playground-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.1/src/lib.rs` & `ever_playground-0.4.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.1/src/tests.rs` & `ever_playground-0.4.2/src/tests.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.1/src/utils.rs` & `ever_playground-0.4.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.4.1/Cargo.lock` & `ever_playground-0.4.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
  "serde",
  "sha2 0.9.9",
  "zeroize",
 ]
 
 [[package]]
 name = "ever-playground"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "num-bigint",
  "pyo3",
  "ton_block",
  "ton_labs_assembler",
  "ton_types",
  "ton_vm",
```

### Comparing `ever_playground-0.4.1/PKG-INFO` & `ever_playground-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ever-playground
-Version: 0.4.1
+Version: 0.4.2
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ever-playground
 
 A tool alternative to Fift: play with Cells, Slices, Builders, and Dictionaries — native types of TVM; assemble and run TVM code.
```

