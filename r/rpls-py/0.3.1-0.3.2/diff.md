# Comparing `tmp/rpls_py-0.3.1.tar.gz` & `tmp/rpls_py-0.3.2.tar.gz`

## Comparing `rpls_py-0.3.1.tar` & `rpls_py-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 rpls_py-0.3.1/Cargo.toml
--rw-rw-r--   0     1000     1000     2905 2023-04-17 22:53:47.000000 rpls_py-0.3.1/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      327 2023-04-17 19:52:01.000000 rpls_py-0.3.1/.gitignore
--rw-rw-r--   0     1000     1000        9 2023-04-17 18:22:01.000000 rpls_py-0.3.1/README.md
--rw-rw-r--   0     1000     1000      562 2023-05-12 21:28:21.000000 rpls_py-0.3.1/pyproject.toml
--rw-rw-r--   0     1000     1000      125 2023-04-17 19:51:20.000000 rpls_py-0.3.1/requirements.txt
--rw-rw-r--   0     1000     1000     1453 2023-04-19 19:55:06.000000 rpls_py-0.3.1/src/lib.rs
--rw-rw-r--   0     1000     1000    38462 2023-05-12 21:27:48.000000 rpls_py-0.3.1/Cargo.lock
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 rpls_py-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 rpls_py-0.3.2/Cargo.toml
+-rw-rw-r--   0     1000     1000     2908 2023-05-17 20:48:26.000000 rpls_py-0.3.2/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      327 2023-04-17 19:52:01.000000 rpls_py-0.3.2/.gitignore
+-rw-rw-r--   0     1000     1000      114 2023-05-17 20:48:26.000000 rpls_py-0.3.2/README.md
+-rw-rw-r--   0     1000     1000      562 2023-05-12 21:28:21.000000 rpls_py-0.3.2/pyproject.toml
+-rw-rw-r--   0     1000     1000      125 2023-04-17 19:51:20.000000 rpls_py-0.3.2/requirements.txt
+-rw-rw-r--   0     1000     1000     1453 2023-04-19 19:55:06.000000 rpls_py-0.3.2/src/lib.rs
+-rw-rw-r--   0     1000     1000    38462 2023-05-17 20:45:22.000000 rpls_py-0.3.2/Cargo.lock
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 rpls_py-0.3.2/PKG-INFO
```

### Comparing `rpls_py-0.3.1/.github/workflows/CI.yml` & `rpls_py-0.3.2/.github/workflows/CI.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
     steps:
       - uses: actions/checkout@v3
       - name: Install fontconfig
-        run: sudo apt install libfontconfig1-dev libfontconfig
+        run: sudo apt install -y libfontconfig1-dev libfontconfig
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
```

### Comparing `rpls_py-0.3.1/pyproject.toml` & `rpls_py-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpls_py-0.3.1/src/lib.rs` & `rpls_py-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpls_py-0.3.1/Cargo.lock` & `rpls_py-0.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -959,15 +959,15 @@
  "geo",
  "geo-types",
  "plotters",
 ]
 
 [[package]]
 name = "rpls-py"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "pyo3",
  "rpls",
 ]
 
 [[package]]
 name = "rstar"
```

