# Comparing `tmp/rpycocotools-0.0.5.tar.gz` & `tmp/rpycocotools-0.0.6.tar.gz`

## Comparing `rpycocotools-0.0.5.tar` & `rpycocotools-0.0.6.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 rpycocotools-0.0.5/local_dependencies/cocotools/Cargo.toml
--rw-r--r--   0     1001      123       30 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/.gitignore
--rw-r--r--   0     1001      123    55307 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/Cargo.lock
--rw-r--r--   0     1001      123      980 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/README.md
--rw-r--r--   0     1001      123     1186 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/argparse.rs
--rw-r--r--   0     1001      123    18281 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/coco/object_detection.rs
--rw-r--r--   0     1001      123     7039 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/coco/pyo3.rs
--rw-r--r--   0     1001      123      181 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/coco.rs
--rw-r--r--   0     1001      123     3024 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/errors.rs
--rw-r--r--   0     1001      123     1901 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/lib.rs
--rw-r--r--   0     1001      123     1510 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/main.rs
--rw-r--r--   0     1001      123    23262 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/mask/conversions.rs
--rw-r--r--   0     1001      123     6222 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/mask/utils.rs
--rw-r--r--   0     1001      123      230 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/mask.rs
--rw-r--r--   0     1001      123      724 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/utils.rs
--rw-r--r--   0     1001      123     2296 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize/display.rs
--rw-r--r--   0     1001      123     6037 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize/draw.rs
--rw-r--r--   0     1001      123      141 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize.rs
--rw-r--r--   0     1001      123      610 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/local_dependencies/cocotools/tests/load_coco.rs
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 rpycocotools-0.0.5/Cargo.toml
--rw-r--r--   0     1001      123      173 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/.gitignore
--rw-r--r--   0     1001      123       58 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/.rustfmt.toml
--rw-r--r--   0     1001      123    45992 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/Cargo.lock
--rw-r--r--   0     1001      123     2127 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/README.md
--rw-r--r--   0     1001      123       10 2023-05-11 14:57:42.000000 rpycocotools-0.0.5/dist/rpycocotools-0.0.5.tar.gz
--rw-r--r--   0     1001      123      634 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/Makefile
--rw-r--r--   0     1001      123        0 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/_static/.gitkeep
--rw-r--r--   0     1001      123     1572 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/conf.py
--rw-r--r--   0     1001      123     9080 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/dataset.rst
--rw-r--r--   0     1001      123      623 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/examples.rst
--rw-r--r--   0     1001      123      731 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/index.rst
--rw-r--r--   0     1001      123      800 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/make.bat
--rw-r--r--   0     1001      123      101 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/quickstart.rst
--rw-r--r--   0     1001      123     2368 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/docs/segmentation_masks.rst
--rw-r--r--   0     1001      123     4114 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/pyproject.toml
--rw-r--r--   0     1001      123      157 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/python/rpycocotools/__init__.py
--rw-r--r--   0     1001      123     3402 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/python/rpycocotools/mask.py
--rw-r--r--   0     1001      123      872 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/README.md
--rw-r--r--   0     1001      123     4323 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-build.txt
--rw-r--r--   0     1001      123     6529 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-dev.txt
--rw-r--r--   0     1001      123    19383 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-doc.txt
--rw-r--r--   0     1001      123     7535 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-flake8.txt
--rw-r--r--   0     1001      123     4641 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements-test.txt
--rw-r--r--   0     1001      123     3142 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/requirements/requirements.txt
--rw-r--r--   0     1001      123     5136 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/coco.rs
--rw-r--r--   0     1001      123     1179 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/errors.rs
--rw-r--r--   0     1001      123     1433 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/lib.rs
--rw-r--r--   0     1001      123       31 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/main.rs
--rw-r--r--   0     1001      123     6476 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/src/mask.rs
--rw-r--r--   0     1001      123      205 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/tests/conftest.py
--rw-r--r--   0     1001      123     3062 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/tests/test_coco.py
--rw-r--r--   0     1001      123     5096 2023-05-11 14:56:12.000000 rpycocotools-0.0.5/tests/test_mask.py
--rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 rpycocotools-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 rpycocotools-0.0.6/local_dependencies/cocotools/Cargo.toml
+-rw-r--r--   0     1001      123       30 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/.gitignore
+-rw-r--r--   0     1001      123    55307 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/Cargo.lock
+-rw-r--r--   0     1001      123     1088 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/README.md
+-rw-r--r--   0     1001      123     1186 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/argparse.rs
+-rw-r--r--   0     1001      123    19128 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/coco/object_detection.rs
+-rw-r--r--   0     1001      123     8344 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/coco/pyo3.rs
+-rw-r--r--   0     1001      123      181 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/coco.rs
+-rw-r--r--   0     1001      123     3017 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/errors.rs
+-rw-r--r--   0     1001      123     1901 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/lib.rs
+-rw-r--r--   0     1001      123     1510 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/main.rs
+-rw-r--r--   0     1001      123    23262 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/mask/conversions.rs
+-rw-r--r--   0     1001      123     6222 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/mask/utils.rs
+-rw-r--r--   0     1001      123      230 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/mask.rs
+-rw-r--r--   0     1001      123      724 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/utils.rs
+-rw-r--r--   0     1001      123     2296 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize/display.rs
+-rw-r--r--   0     1001      123     6037 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize/draw.rs
+-rw-r--r--   0     1001      123      141 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize.rs
+-rw-r--r--   0     1001      123      610 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/local_dependencies/cocotools/tests/load_coco.rs
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 rpycocotools-0.0.6/Cargo.toml
+-rw-r--r--   0     1001      123      173 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/.gitignore
+-rw-r--r--   0     1001      123       58 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/.rustfmt.toml
+-rw-r--r--   0     1001      123    45992 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/Cargo.lock
+-rw-r--r--   0     1001      123     2289 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/README.md
+-rw-r--r--   0     1001      123       10 2023-05-17 13:28:34.000000 rpycocotools-0.0.6/dist/rpycocotools-0.0.6.tar.gz
+-rw-r--r--   0     1001      123      634 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/Makefile
+-rw-r--r--   0     1001      123        0 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/_static/.gitkeep
+-rw-r--r--   0     1001      123     1572 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/conf.py
+-rw-r--r--   0     1001      123     9389 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/dataset.rst
+-rw-r--r--   0     1001      123      623 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/examples.rst
+-rw-r--r--   0     1001      123      731 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/index.rst
+-rw-r--r--   0     1001      123      800 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/make.bat
+-rw-r--r--   0     1001      123      101 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/quickstart.rst
+-rw-r--r--   0     1001      123     2943 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/docs/segmentation_masks.rst
+-rw-r--r--   0     1001      123     4234 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/pyproject.toml
+-rw-r--r--   0     1001      123      171 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/python/rpycocotools/__init__.py
+-rw-r--r--   0     1001      123      266 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/python/rpycocotools/anns.py
+-rw-r--r--   0     1001      123     3402 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/python/rpycocotools/mask.py
+-rw-r--r--   0     1001      123      872 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/README.md
+-rw-r--r--   0     1001      123     4323 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-build.txt
+-rw-r--r--   0     1001      123     6529 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-dev.txt
+-rw-r--r--   0     1001      123    19383 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-doc.txt
+-rw-r--r--   0     1001      123     7535 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-flake8.txt
+-rw-r--r--   0     1001      123     4641 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements-test.txt
+-rw-r--r--   0     1001      123     3142 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/requirements/requirements.txt
+-rw-r--r--   0     1001      123     6021 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/coco.rs
+-rw-r--r--   0     1001      123     1179 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/errors.rs
+-rw-r--r--   0     1001      123     1524 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/lib.rs
+-rw-r--r--   0     1001      123       31 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/main.rs
+-rw-r--r--   0     1001      123     6476 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/src/mask.rs
+-rw-r--r--   0     1001      123      205 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/tests/conftest.py
+-rw-r--r--   0     1001      123     4055 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/tests/test_coco.py
+-rw-r--r--   0     1001      123     5096 2023-05-17 13:27:15.000000 rpycocotools-0.0.6/tests/test_mask.py
+-rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 rpycocotools-0.0.6/PKG-INFO
```

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/Cargo.toml` & `rpycocotools-0.0.6/local_dependencies/cocotools/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "cocotools"
-version = "0.0.5"
+version = "0.0.6"
 edition = "2021"
 rust-version = "1.64.0"
 description = "Package providing functionalities to work with COCO format datasets."
 readme = "README.md"
 categories = ["command-line-utilities"]
 authors = ["Hoel Bagard"]
 license = "MIT OR Apache-2.0"
@@ -18,21 +18,14 @@
 rand = "0.8.5"
 minifb = "0.23"
 anyhow = "1.0.69"
 thiserror = "1.0.38"
 ndarray = "0.15.6"
 pyo3 = { version = "0.18", features = ["extension-module"], optional = true}
 
-[dev-dependencies]
-rstest = "0.16.0"
-proptest = "1.1.0"
-rand = "0.8.5"
-# ndarray-rand = "0.14.0"
-criterion = {version = "0.4.0", features = ["html_reports"] }
-
 [features]
 default = []
 pyo3 = ["dep:pyo3"]
 
 [profile.dev]
 opt-level = 1
```

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/Cargo.lock` & `rpycocotools-0.0.6/local_dependencies/cocotools/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "cocotools"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
  "anyhow",
  "clap 4.1.8",
  "criterion",
  "image",
  "imageproc",
  "minifb",
```

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/README.md` & `rpycocotools-0.0.6/local_dependencies/cocotools/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Cocotools
+![cocotools ci](https://github.com/hoel-bagard/cocotools-rs/actions/workflows/ci-cocotools.yaml/badge.svg)
+
 The `cocotools` crate provides tools to load, manipulate, convert and visualize COCO format datasets.
 
 ## API Usage example
 ```
 use std::path::PathBuf;
 use cocotools::COCO;
```

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/argparse.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/argparse.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/coco/object_detection.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/coco/object_detection.rs`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 pub struct Dataset {
     pub images: Vec<Image>,
     pub annotations: Vec<Annotation>,
     pub categories: Vec<Category>,
 }
 
 /// Stores information relating to one image.
-#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
+#[cfg_attr(
+    feature = "pyo3",
+    pyclass(get_all, set_all, module = "rpycocotools.anns")
+)]
 #[derive(Clone, Debug, PartialEq, Eq, Deserialize, Serialize)]
 pub struct Image {
     pub id: u32,
     pub width: u32,
     pub height: u32,
     pub file_name: String,
     // "license": int,
@@ -37,15 +40,18 @@
 
 /// Object instance annotation for object detection.\
 ///
 /// Each object instance annotation contains a series of fields, including the category id and segmentation mask of the object.\
 /// In [the original COCO dataset](https://cocodataset.org/#home), the segmentation format depends on whether the instance represents a single object (`iscrowd=0` in which case polygons are used) or a collection of objects (`iscrowd=1` in which case RLE is used). Note that a single object (iscrowd=0) may require multiple polygons, for example if occluded.\
 /// Crowd annotations (`iscrowd=1`) are used to label large groups of objects (e.g. a crowd of people). In addition, an enclosing bounding box is provided for each object (box coordinates are measured from the top left image corner and are 0-indexed).\
 /// Finally, the categories field of the annotation structure stores the mapping of category id to category and supercategory names.
-#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
+#[cfg_attr(
+    feature = "pyo3",
+    pyclass(subclass, get_all, set_all, module = "rpycocotools.anns")
+)]
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 pub struct Annotation {
     pub id: u32,
     pub image_id: u32,
     pub category_id: u32,
     /// Segmentation in the annotation file can be a polygon, RLE or COCO RLE.\
     /// Examples of what each segmentation should look like in the JSON file:
@@ -58,14 +64,15 @@
     /// Example: "bbox": `[473.07, 395.93, 38.65, 28.67]`
     pub bbox: Bbox,
     /// Either 1 or 0
     pub iscrowd: u32,
 }
 
 // #[cfg_attr(feature = "pyo3", pyclass)]
+#[cfg_attr(feature = "pyo3", derive(FromPyObject))]
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 #[serde(untagged)]
 pub enum Segmentation {
     Rle(Rle),
     CocoRle(CocoRle),
     Polygons(Polygons),
     #[serde(skip)]
@@ -87,64 +94,76 @@
 /// assert_eq!(poly[0].len() % 2, 0);
 /// ```
 pub type Polygons = Vec<Vec<f64>>;
 
 /// Internal type used to represent polygons.
 ///
 /// It contains the width and height of the image for easier handling, notably when using traits.
-#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
+#[cfg_attr(
+    feature = "pyo3",
+    pyclass(get_all, set_all, module = "rpycocotools.anns")
+)]
 #[derive(Clone, Debug, Deserialize, Serialize)]
 pub struct PolygonsRS {
     /// Vector with two elements, the height and width of the image corresponding to the segmentation mask.
     pub size: Vec<u32>,
     /// See [`Polygons`].
     pub counts: Vec<Vec<f64>>,
 }
 
 /// Segmentation mask compressed as a [Run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding).
 #[cfg_attr(
     feature = "pyo3",
-    pyclass(get_all, name = "RLE", module = "rpycocotools.anns")
+    pyclass(get_all, set_all, name = "RLE", module = "rpycocotools.anns")
 )]
 #[derive(Clone, Debug, Eq, PartialEq, Deserialize, Serialize)]
 pub struct Rle {
     /// Vector with two elements, the height and width of the image corresponding to the segmentation mask.
     pub size: Vec<u32>,
     pub counts: Vec<u32>,
 }
 
 /// Segmentation mask compressed as a [Run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding) and then further compressed into a string.
 ///
 /// For the encoding process, see [here](https://github.com/cocodataset/cocoapi/blob/master/common/maskApi.c#L204).
 #[cfg_attr(
     feature = "pyo3",
-    pyclass(get_all, name = "COCO_RLE", module = "rpycocotools.anns")
+    pyclass(get_all, set_all, name = "COCO_RLE", module = "rpycocotools.anns")
 )]
 #[derive(Clone, Debug, Eq, PartialEq, Deserialize, Serialize)]
 pub struct CocoRle {
     /// Vector with two elements, the height and width of the image corresponding to the segmentation mask.
     pub size: Vec<u32>,
     pub counts: String,
 }
 
 /// Bounding box enclosing an object.
 #[cfg_attr(
     feature = "pyo3",
-    pyclass(sequence, get_all, name = "BBox", module = "rpycocotools.anns")
+    pyclass(
+        sequence,
+        get_all,
+        set_all,
+        name = "BBox",
+        module = "rpycocotools.anns"
+    )
 )]
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 pub struct Bbox {
     pub left: f64,
     pub top: f64,
     pub width: f64,
     pub height: f64,
 }
 
 /// Category of an annotation.
-#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
+#[cfg_attr(
+    feature = "pyo3",
+    pyclass(get_all, set_all, module = "rpycocotools.anns")
+)]
 #[derive(Clone, Debug, Eq, PartialEq, Deserialize, Serialize)]
 pub struct Category {
     pub id: u32,
     pub name: String,
     pub supercategory: String,
 }
 
@@ -172,15 +191,26 @@
     pub fn new<P: AsRef<Path>>(annotations_path: P, image_folder: P) -> Result<Self, LoadingError> {
         let annotations_path = annotations_path.as_ref().to_path_buf();
         let annotations_file_content = fs::read_to_string(&annotations_path)
             .map_err(|err| LoadingError::Read(err, annotations_path.clone()))?;
 
         let dataset: Dataset = serde_json::from_str(&annotations_file_content)
             .map_err(|err| LoadingError::Deserialize(err, annotations_path.clone()))?;
+        Self::from_dataset(dataset, image_folder)
+    }
 
+    /// Construct a hashmap COCO dataset from a "simple" dataset and the image folder.
+    ///
+    /// # Errors
+    ///
+    /// Will return `Err` if there is an annotation with an image id X, but no image entry has this id.
+    pub fn from_dataset<P: AsRef<Path>>(
+        dataset: Dataset,
+        image_folder: P,
+    ) -> Result<Self, LoadingError> {
         let cats = dataset
             .categories
             .into_iter()
             .map(|category| (category.id, category))
             .collect();
 
         let imgs: HashMap<u32, Image> = dataset
@@ -205,16 +235,15 @@
             // The polygon format from COCO is annoying to deal with as it does not contain the size of the image,
             // it is therefore transformed into a more complete format.
             if let Segmentation::Polygons(counts) = annotation.segmentation {
                 annotation.segmentation = Segmentation::PolygonsRS(PolygonsRS {
                     size: if let Some(img) = imgs.get(&img_id) {
                         vec![img.height, img.width]
                     } else {
-                        return Err(MissingIdError::Image(img_id))
-                            .map_err(|err| LoadingError::Parsing(err, annotations_path));
+                        return Err(MissingIdError::Image(img_id)).map_err(LoadingError::Parsing);
                     },
                     counts,
                 });
             };
 
             anns.insert(annotation.id, annotation);
             img_to_anns
@@ -338,14 +367,24 @@
     pub fn save_to<P: AsRef<Path>>(&self, output_path: P) -> Result<(), Box<dyn Error>> {
         let dataset = Dataset::from(self);
         let f = fs::File::create(output_path)?;
         serde_json::to_writer_pretty(&f, &dataset)?;
 
         Ok(())
     }
+
+    /// Return the dataset as a json string.
+    ///
+    /// # Errors
+    ///
+    /// Will return `Err` if the serialization fails.
+    pub fn json(&self) -> Result<String, serde_json::Error> {
+        let dataset = Dataset::from(self);
+        serde_json::to_string(&dataset)
+    }
 }
 
 impl From<&HashmapDataset> for Dataset {
     fn from(dataset: &HashmapDataset) -> Self {
         Self {
             images: dataset.get_imgs().into_iter().cloned().collect(),
             annotations: dataset.get_anns().into_iter().cloned().collect(),
```

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/coco/pyo3.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/coco/pyo3.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,63 @@
 use pyo3::class::basic::CompareOp;
 use pyo3::prelude::*;
 
 use crate::coco::object_detection::*;
 
 #[pymethods]
 impl Annotation {
+    #[new]
+    fn new(
+        id: u32,
+        image_id: u32,
+        category_id: u32,
+        segmentation: Segmentation,
+        area: f64,
+        bbox: Bbox,
+        iscrowd: u32,
+    ) -> Self {
+        Self {
+            id,
+            image_id,
+            category_id,
+            segmentation,
+            area,
+            bbox,
+            iscrowd,
+        }
+    }
+
     fn __repr__(&self) -> String {
         format!(
             "Annotation(id={}, image_id={}, category_id={}, segmentation={}, area={}, bbox={}, iscrowd={})",
             self.id, self.image_id, self.category_id, &self.segmentation.__repr__(), self.area, &self.bbox.__repr__(), self.iscrowd
         )
     }
+
+    fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
+        match op {
+            CompareOp::Eq => (self.id == other.id
+                && self.image_id == other.image_id
+                && self.category_id == other.category_id
+                && self.segmentation == other.segmentation
+                && self.area == other.area
+                && self.bbox == other.bbox
+                && self.iscrowd == other.iscrowd)
+                .into_py(py),
+            CompareOp::Ne => (self.id != other.id
+                || self.image_id != other.image_id
+                || self.category_id != other.category_id
+                || self.segmentation != other.segmentation
+                || self.area != other.area
+                || self.bbox != other.bbox
+                || self.iscrowd != other.iscrowd)
+                .into_py(py),
+            _ => py.NotImplemented(),
+        }
+    }
 }
 
 #[pymethods]
 impl Category {
     #[new]
     fn new(id: u32, name: String, supercategory: String) -> Self {
         Self {
```

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/errors.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/errors.rs`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 /// Error returned when a json annotations file cannot be loaded/parsed or when an image cannot be loaded.
 #[derive(Error)]
 pub enum LoadingError {
     #[error("Failed to read the annotation file {1:?}.")]
     Read(#[source] std::io::Error, PathBuf),
     #[error("Failed to deserialize the annotation file {1:?}.")]
     Deserialize(#[source] serde_json::Error, PathBuf),
-    #[error("Failed to parse the annotation file {1:?}. Found an annotation for an image id not in the dataset.")]
-    Parsing(#[source] MissingIdError, PathBuf),
+    #[error("Failed to parse the annotation file/dataset. Found an annotation for an image id not in the dataset.")]
+    Parsing(#[source] MissingIdError),
     #[error(transparent)]
     Image(#[from] anyhow::Error),
 }
 
 /// Error returned converting a segmentation mask to another format fails.
 #[allow(clippy::enum_variant_names)]
 #[derive(Debug, Error)]
```

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/lib.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/main.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/main.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/mask/conversions.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/mask/conversions.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/mask/utils.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/mask/utils.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/utils.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/utils.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize/display.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize/display.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/src/visualize/draw.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/src/visualize/draw.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/local_dependencies/cocotools/tests/load_coco.rs` & `rpycocotools-0.0.6/local_dependencies/cocotools/tests/load_coco.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/Cargo.lock` & `rpycocotools-0.0.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "cocotools"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
  "anyhow",
  "clap",
  "image",
  "imageproc",
  "minifb",
  "ndarray",
@@ -1245,15 +1245,15 @@
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "rpycocotools"
-version = "0.0.3"
+version = "0.0.6"
 dependencies = [
  "anyhow",
  "cocotools",
  "ndarray",
  "nshare",
  "numpy",
  "pyo3",
```

### Comparing `rpycocotools-0.0.5/docs/Makefile` & `rpycocotools-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/docs/conf.py` & `rpycocotools-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/docs/dataset.rst` & `rpycocotools-0.0.6/docs/dataset.rst`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,29 @@
 
     Draw the annotations on the image and returns it as a (RGB) numpy array.
 
     :param int img_id: The `id` of the `Image` whose annotations should be visualized.
     :param bool draw_bboxes: Whether to display bounding boxes or not (if `False`, only the masks will be drawn).
     :raises ValueError: If the image cannot be drawn (potentially due to it not being in the dataset) or cannot be displayed.
 
+    .. method:: json(self: Self) -> str: ...
+
+    Return the dataset as a json string.
+
+    :return: The dataset as a json string.
+    :rtype: str
+
+
+    .. method:: __len__(self: Self) -> int ...
+
+    Return number of images in the dataset.
+
+    :return: The number of images in the dataset.
+    :rtype: int
+
 .. class:: rpycocotools.anns.Annotation(id: int, image_id: int, category_id: int, segmentation: Polygons | PolygonsRS | RLE | COCO_RLE, area: float, bbox: BBox, iscrowd: int) -> None
 
     Create an annotation used for object detection tasks.
 
     Each object instance annotation contains a series of fields, including the category id and segmentation mask of the object.\
     In [the original COCO dataset](https://cocodataset.org/#home), the segmentation format depends on whether the instance represents a single object (`iscrowd=0` in which case polygons are used) or a collection of objects (`iscrowd=1` in which case RLE is used). Note that a single object (iscrowd=0) may require multiple polygons, for example if occluded.\
     Crowd annotations (`iscrowd=1`) are used to label large groups of objects (e.g. a crowd of people). In addition, an enclosing bounding box is provided for each object (box coordinates are measured from the top left image corner and are 0-indexed).\
```

### Comparing `rpycocotools-0.0.5/docs/examples.rst` & `rpycocotools-0.0.6/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/docs/index.rst` & `rpycocotools-0.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/docs/make.bat` & `rpycocotools-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/docs/segmentation_masks.rst` & `rpycocotools-0.0.6/docs/segmentation_masks.rst`

 * *Files 20% similar despite different names*

```diff
@@ -67,82 +67,118 @@
 00000420: 7669 6e67 2074 6f20 6c6f 6f6b 2075 7020  ving to look up 
 00000430: 6974 7320 7369 7a65 2e20 486f 7765 7665  its size. Howeve
 00000440: 7220 6974 2073 686f 756c 6420 6e6f 7420  r it should not 
 00000450: 6265 2077 7269 7474 656e 2074 6f20 6120  be written to a 
 00000460: 6a73 6f6e 2066 696c 6520 2861 7320 6974  json file (as it
 00000470: 2069 7320 6e6f 6e2d 7374 616e 6461 7264   is non-standard
 00000480: 292e 0a0a 4465 636f 6465 206d 6173 6b73  )...Decode masks
-00000490: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-000004a0: 2d0a 0a2e 2e20 6675 6e63 7469 6f6e 3a3a  -.... function::
-000004b0: 2072 7079 636f 636f 746f 6f6c 732e 6d61   rpycocotools.ma
-000004c0: 736b 2e64 6563 6f64 6528 656e 636f 6465  sk.decode(encode
-000004d0: 645f 6d61 736b 3a20 524c 4520 7c20 434f  d_mask: RLE | CO
-000004e0: 434f 5f52 4c45 207c 2050 6f6c 7967 6f6e  CO_RLE | Polygon
-000004f0: 7320 7c20 506f 6c79 676f 6e73 5253 2c20  s | PolygonsRS, 
-00000500: 7769 6474 683a 204e 6f6e 6520 7c20 696e  width: None | in
-00000510: 742c 2068 6569 6768 743a 204e 6f6e 6520  t, height: None 
-00000520: 7c20 696e 7429 202d 3e20 6e70 742e 4e44  | int) -> npt.ND
-00000530: 4172 7261 795b 6e70 2e75 696e 7438 5d0a  Array[np.uint8].
-00000540: 0a20 2044 6563 6f64 6520 6120 6d61 736b  .  Decode a mask
-00000550: 2074 6f20 6120 3a63 6c61 7373 3a60 6e75   to a :class:`nu
-00000560: 6d70 792e 6e64 6172 7261 7960 2e0a 0a20  mpy.ndarray`... 
-00000570: 203a 7061 7261 6d20 524c 4520 7c20 434f   :param RLE | CO
-00000580: 434f 5f52 4c45 207c 2050 6f6c 7967 6f6e  CO_RLE | Polygon
-00000590: 7320 7c20 506f 6c79 676f 6e73 5253 2065  s | PolygonsRS e
-000005a0: 6e63 6f64 6564 5f6d 6173 6b3a 2054 6865  ncoded_mask: The
-000005b0: 2065 6e63 6f64 6564 206d 6173 6b2e 0a20   encoded mask.. 
-000005c0: 203a 7061 7261 6d20 696e 7420 7769 6474   :param int widt
-000005d0: 683a 2055 7365 206f 6e6c 7920 7768 656e  h: Use only when
-000005e0: 2074 6865 206d 6173 6b20 6973 2061 203a   the mask is a :
-000005f0: 7079 3a63 6c61 7373 3a60 506f 6c79 676f  py:class:`Polygo
-00000600: 6e60 2e20 5468 6520 7769 6474 6820 6f66  n`. The width of
-00000610: 2074 6865 2069 6d61 6765 2063 6f72 7265   the image corre
-00000620: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
-00000630: 706f 6c79 676f 6e73 2e0a 2020 3a70 6172  polygons..  :par
-00000640: 616d 2069 6e74 2068 6569 6768 743a 2055  am int height: U
-00000650: 7365 206f 6e6c 7920 7768 656e 2074 6865  se only when the
-00000660: 206d 6173 6b20 6973 2061 203a 7079 3a63   mask is a :py:c
-00000670: 6c61 7373 3a60 506f 6c79 676f 6e60 2e20  lass:`Polygon`. 
-00000680: 5468 6520 6865 6967 6874 206f 6620 7468  The height of th
-00000690: 6520 696d 6167 6520 636f 7272 6573 706f  e image correspo
-000006a0: 6e64 696e 6720 746f 2074 6865 2070 6f6c  nding to the pol
-000006b0: 7967 6f6e 732e 0a20 203a 7261 6973 6520  ygons..  :raise 
-000006c0: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
-000006d0: 6865 206d 6173 6b20 636f 6e76 6572 7369  he mask conversi
-000006e0: 6f6e 2066 6169 6c65 642e 0a20 203a 7265  on failed..  :re
-000006f0: 7475 726e 3a20 5468 6520 6465 636f 6465  turn: The decode
-00000700: 6420 6d61 736b 2061 7320 6120 4e75 6d50  d mask as a NumP
-00000710: 7920 6172 7261 792e 0a20 203a 7274 7970  y array..  :rtyp
-00000720: 653a 2060 606e 7074 2e4e 4441 7272 6179  e: ``npt.NDArray
-00000730: 5b6e 702e 7569 6e74 385d 6060 0a0a 0a45  [np.uint8]``...E
-00000740: 6e63 6f64 6520 6d61 736b 730a 2d2d 2d2d  ncode masks.----
-00000750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e  ------------....
-00000760: 2066 756e 6374 696f 6e3a 3a20 7270 7963   function:: rpyc
-00000770: 6f63 6f74 6f6f 6c73 2e6d 6173 6b2e 656e  ocotools.mask.en
-00000780: 636f 6465 286d 6173 6b3a 206e 7074 2e4e  code(mask: npt.N
-00000790: 4441 7272 6179 5b6e 702e 7569 6e74 385d  DArray[np.uint8]
-000007a0: 2c20 7461 7267 6574 3a20 4c69 7465 7261  , target: Litera
-000007b0: 6c5b 2270 6f6c 7967 6f6e 7322 5d20 7c20  l["polygons"] | 
-000007c0: 4c69 7465 7261 6c5b 2272 6c65 225d 207c  Literal["rle"] |
-000007d0: 204c 6974 6572 616c 5b22 636f 636f 5f72   Literal["coco_r
-000007e0: 6c65 225d 207c 204c 6974 6572 616c 5b22  le"] | Literal["
-000007f0: 706f 6c79 676f 6e73 5f72 7322 5d29 202d  polygons_rs"]) -
-00000800: 3e20 506f 6c79 676f 6e73 207c 2052 4c45  > Polygons | RLE
-00000810: 207c 2043 4f43 4f5f 524c 4520 7c20 506f   | COCO_RLE | Po
-00000820: 6c79 676f 6e73 5253 3a0a 0a20 2045 6e63  lygonsRS:..  Enc
-00000830: 6f64 652f 636f 6d70 7265 7373 2061 203a  ode/compress a :
-00000840: 636c 6173 733a 606e 756d 7079 2e6e 6461  class:`numpy.nda
-00000850: 7272 6179 6020 6d61 736b 2074 6f20 7468  rray` mask to th
-00000860: 6520 6465 7369 7265 6420 666f 726d 6174  e desired format
-00000870: 2e0a 0a20 203a 7061 7261 6d20 6e70 742e  ...  :param npt.
-00000880: 4e44 4172 7261 795b 6e70 2e75 696e 7438  NDArray[np.uint8
-00000890: 5d20 656e 636f 6465 645f 6d61 736b 3a20  ] encoded_mask: 
-000008a0: 5468 6520 756e 636f 6d70 7265 7373 6564  The uncompressed
-000008b0: 206d 6173 6b2e 0a20 203a 7261 6973 6520   mask..  :raise 
-000008c0: 5661 6c75 6545 7272 6f72 3a20 4966 2074  ValueError: If t
-000008d0: 6865 206d 6173 6b20 636f 6e76 6572 7369  he mask conversi
-000008e0: 6f6e 2066 6169 6c65 642e 0a20 203a 7265  on failed..  :re
-000008f0: 7475 726e 3a20 5468 6520 636f 6d70 7265  turn: The compre
-00000900: 7373 6564 206d 6173 6b2e 0a20 203a 7274  ssed mask..  :rt
-00000910: 7970 653a 2060 6050 6f6c 7967 6f6e 7320  ype: ``Polygons 
-00000920: 7c20 524c 4520 7c20 434f 434f 5f52 4c45  | RLE | COCO_RLE
-00000930: 207c 2050 6f6c 7967 6f6e 7352 5360 600a   | PolygonsRS``.
+00000490: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e  .------------...
+000004a0: 2e20 6675 6e63 7469 6f6e 3a3a 2072 7079  . function:: rpy
+000004b0: 636f 636f 746f 6f6c 732e 6d61 736b 2e64  cocotools.mask.d
+000004c0: 6563 6f64 6528 656e 636f 6465 645f 6d61  ecode(encoded_ma
+000004d0: 736b 3a20 524c 4520 7c20 434f 434f 5f52  sk: RLE | COCO_R
+000004e0: 4c45 207c 2050 6f6c 7967 6f6e 7320 7c20  LE | Polygons | 
+000004f0: 506f 6c79 676f 6e73 5253 2c20 7769 6474  PolygonsRS, widt
+00000500: 683a 204e 6f6e 6520 7c20 696e 742c 2068  h: None | int, h
+00000510: 6569 6768 743a 204e 6f6e 6520 7c20 696e  eight: None | in
+00000520: 7429 202d 3e20 6e70 742e 4e44 4172 7261  t) -> npt.NDArra
+00000530: 795b 6e70 2e75 696e 7438 5d0a 0a20 2044  y[np.uint8]..  D
+00000540: 6563 6f64 6520 6120 6d61 736b 2074 6f20  ecode a mask to 
+00000550: 6120 3a63 6c61 7373 3a60 6e75 6d70 792e  a :class:`numpy.
+00000560: 6e64 6172 7261 7960 2e0a 0a20 203a 7061  ndarray`...  :pa
+00000570: 7261 6d20 524c 4520 7c20 434f 434f 5f52  ram RLE | COCO_R
+00000580: 4c45 207c 2050 6f6c 7967 6f6e 7320 7c20  LE | Polygons | 
+00000590: 506f 6c79 676f 6e73 5253 2065 6e63 6f64  PolygonsRS encod
+000005a0: 6564 5f6d 6173 6b3a 2054 6865 2065 6e63  ed_mask: The enc
+000005b0: 6f64 6564 206d 6173 6b2e 0a20 203a 7061  oded mask..  :pa
+000005c0: 7261 6d20 696e 7420 7769 6474 683a 2055  ram int width: U
+000005d0: 7365 206f 6e6c 7920 7768 656e 2074 6865  se only when the
+000005e0: 206d 6173 6b20 6973 2061 203a 7079 3a63   mask is a :py:c
+000005f0: 6c61 7373 3a60 506f 6c79 676f 6e60 2e20  lass:`Polygon`. 
+00000600: 5468 6520 7769 6474 6820 6f66 2074 6865  The width of the
+00000610: 2069 6d61 6765 2063 6f72 7265 7370 6f6e   image correspon
+00000620: 6469 6e67 2074 6f20 7468 6520 706f 6c79  ding to the poly
+00000630: 676f 6e73 2e0a 2020 3a70 6172 616d 2069  gons..  :param i
+00000640: 6e74 2068 6569 6768 743a 2055 7365 206f  nt height: Use o
+00000650: 6e6c 7920 7768 656e 2074 6865 206d 6173  nly when the mas
+00000660: 6b20 6973 2061 203a 7079 3a63 6c61 7373  k is a :py:class
+00000670: 3a60 506f 6c79 676f 6e60 2e20 5468 6520  :`Polygon`. The 
+00000680: 6865 6967 6874 206f 6620 7468 6520 696d  height of the im
+00000690: 6167 6520 636f 7272 6573 706f 6e64 696e  age correspondin
+000006a0: 6720 746f 2074 6865 2070 6f6c 7967 6f6e  g to the polygon
+000006b0: 732e 0a20 203a 7261 6973 6520 5661 6c75  s..  :raise Valu
+000006c0: 6545 7272 6f72 3a20 4966 2074 6865 206d  eError: If the m
+000006d0: 6173 6b20 636f 6e76 6572 7369 6f6e 2066  ask conversion f
+000006e0: 6169 6c65 642e 0a20 203a 7265 7475 726e  ailed..  :return
+000006f0: 3a20 5468 6520 6465 636f 6465 6420 6d61  : The decoded ma
+00000700: 736b 2061 7320 6120 4e75 6d50 7920 6172  sk as a NumPy ar
+00000710: 7261 792e 0a20 203a 7274 7970 653a 2060  ray..  :rtype: `
+00000720: 606e 7074 2e4e 4441 7272 6179 5b6e 702e  `npt.NDArray[np.
+00000730: 7569 6e74 385d 6060 0a0a 0a45 6e63 6f64  uint8]``...Encod
+00000740: 6520 6d61 736b 730a 2d2d 2d2d 2d2d 2d2d  e masks.--------
+00000750: 2d2d 2d2d 0a0a 2e2e 2066 756e 6374 696f  ----.... functio
+00000760: 6e3a 3a20 7270 7963 6f63 6f74 6f6f 6c73  n:: rpycocotools
+00000770: 2e6d 6173 6b2e 656e 636f 6465 286d 6173  .mask.encode(mas
+00000780: 6b3a 206e 7074 2e4e 4441 7272 6179 5b6e  k: npt.NDArray[n
+00000790: 702e 7569 6e74 385d 2c20 7461 7267 6574  p.uint8], target
+000007a0: 3a20 4c69 7465 7261 6c5b 2270 6f6c 7967  : Literal["polyg
+000007b0: 6f6e 7322 2c20 2272 6c65 222c 2022 636f  ons", "rle", "co
+000007c0: 636f 5f72 6c65 222c 2022 706f 6c79 676f  co_rle", "polygo
+000007d0: 6e73 5f72 7322 5d29 202d 3e20 506f 6c79  ns_rs"]) -> Poly
+000007e0: 676f 6e73 207c 2052 4c45 207c 2043 4f43  gons | RLE | COC
+000007f0: 4f5f 524c 4520 7c20 506f 6c79 676f 6e73  O_RLE | Polygons
+00000800: 5253 3a0a 0a20 2045 6e63 6f64 652f 636f  RS:..  Encode/co
+00000810: 6d70 7265 7373 2061 203a 636c 6173 733a  mpress a :class:
+00000820: 606e 756d 7079 2e6e 6461 7272 6179 6020  `numpy.ndarray` 
+00000830: 6d61 736b 2074 6f20 7468 6520 6465 7369  mask to the desi
+00000840: 7265 6420 666f 726d 6174 2e0a 0a20 203a  red format...  :
+00000850: 7061 7261 6d20 6e70 742e 4e44 4172 7261  param npt.NDArra
+00000860: 795b 6e70 2e75 696e 7438 5d20 6d61 736b  y[np.uint8] mask
+00000870: 3a20 5468 6520 756e 636f 6d70 7265 7373  : The uncompress
+00000880: 6564 206d 6173 6b2e 0a20 203a 7261 6973  ed mask..  :rais
+00000890: 6520 5661 6c75 6545 7272 6f72 3a20 4966  e ValueError: If
+000008a0: 2074 6865 206d 6173 6b20 636f 6e76 6572   the mask conver
+000008b0: 7369 6f6e 2066 6169 6c65 642e 0a20 203a  sion failed..  :
+000008c0: 7265 7475 726e 3a20 5468 6520 636f 6d70  return: The comp
+000008d0: 7265 7373 6564 206d 6173 6b2e 0a20 203a  ressed mask..  :
+000008e0: 7274 7970 653a 2060 6050 6f6c 7967 6f6e  rtype: ``Polygon
+000008f0: 7320 7c20 524c 4520 7c20 434f 434f 5f52  s | RLE | COCO_R
+00000900: 4c45 207c 2050 6f6c 7967 6f6e 7352 5360  LE | PolygonsRS`
+00000910: 600a 0a0a 5574 696c 730a 2d2d 2d2d 2d0a  `...Utils.-----.
+00000920: 0a2e 2e20 6675 6e63 7469 6f6e 3a3a 2072  ... function:: r
+00000930: 7079 636f 636f 746f 6f6c 732e 6d61 736b  pycocotools.mask
+00000940: 2e61 7265 6128 656e 636f 6465 645f 6d61  .area(encoded_ma
+00000950: 736b 3a20 524c 4520 7c20 434f 434f 5f52  sk: RLE | COCO_R
+00000960: 4c45 207c 2050 6f6c 7967 6f6e 7352 5320  LE | PolygonsRS 
+00000970: 7c20 506f 6c79 676f 6e73 2920 2d3e 2069  | Polygons) -> i
+00000980: 6e74 3a0a 0a20 2043 6f6d 7075 7465 2074  nt:..  Compute t
+00000990: 6865 2061 7265 6120 6f66 2074 6865 2067  he area of the g
+000009a0: 6976 656e 206d 6173 6b2e 0a0a 2020 3a70  iven mask...  :p
+000009b0: 6172 616d 2052 4c45 207c 2043 4f43 4f5f  aram RLE | COCO_
+000009c0: 524c 4520 7c20 506f 6c79 676f 6e73 5253  RLE | PolygonsRS
+000009d0: 207c 2050 6f6c 7967 6f6e 7320 656e 636f   | Polygons enco
+000009e0: 6465 645f 6d61 736b 3a20 5468 6520 6d61  ded_mask: The ma
+000009f0: 736b 2077 686f 7365 2061 7265 6120 7368  sk whose area sh
+00000a00: 6f75 6c64 2062 6520 636f 6d70 7574 6564  ould be computed
+00000a10: 2e0a 2020 3a72 6574 7572 6e3a 2054 6865  ..  :return: The
+00000a20: 2061 7265 610a 2020 3a72 7479 7065 3a20   area.  :rtype: 
+00000a30: 6060 696e 7460 600a 0a2e 2e20 6675 6e63  ``int``.... func
+00000a40: 7469 6f6e 3a3a 2072 7079 636f 636f 746f  tion:: rpycocoto
+00000a50: 6f6c 732e 6d61 736b 2e74 6f5f 6262 6f78  ols.mask.to_bbox
+00000a60: 2865 6e63 6f64 6564 5f6d 6173 6b3a 2052  (encoded_mask: R
+00000a70: 4c45 207c 2043 4f43 4f5f 524c 4520 7c20  LE | COCO_RLE | 
+00000a80: 506f 6c79 676f 6e73 5253 207c 2050 6f6c  PolygonsRS | Pol
+00000a90: 7967 6f6e 7329 202d 3e20 7270 7963 6f63  ygons) -> rpycoc
+00000aa0: 6f74 6f6f 6c73 2e61 6e6e 732e 4242 6f78  otools.anns.BBox
+00000ab0: 3a0a 0a20 2043 6f6d 7075 7465 2074 6865  :..  Compute the
+00000ac0: 2062 6f75 6e64 696e 6720 626f 7820 6f66   bounding box of
+00000ad0: 2074 6865 2067 6976 656e 206d 6173 6b2e   the given mask.
+00000ae0: 0a0a 2020 3a70 6172 616d 2052 4c45 207c  ..  :param RLE |
+00000af0: 2043 4f43 4f5f 524c 4520 7c20 506f 6c79   COCO_RLE | Poly
+00000b00: 676f 6e73 5253 207c 2050 6f6c 7967 6f6e  gonsRS | Polygon
+00000b10: 7320 656e 636f 6465 645f 6d61 736b 3a20  s encoded_mask: 
+00000b20: 5468 6520 6d61 736b 2077 686f 7365 2062  The mask whose b
+00000b30: 6f75 6e64 696e 6720 626f 7820 7368 6f75  ounding box shou
+00000b40: 6c64 2062 6520 636f 6d70 7574 6564 2e0a  ld be computed..
+00000b50: 2020 3a72 6574 7572 6e3a 2054 6865 2062    :return: The b
+00000b60: 6f75 6e64 696e 6720 626f 780a 2020 3a72  ounding box.  :r
+00000b70: 7479 7065 3a20 6060 4242 6f78 6060 0a    type: ``BBox``.
```

### Comparing `rpycocotools-0.0.5/pyproject.toml` & `rpycocotools-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "rpycocotools"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{name="Bagard Hoel"}]
 description = "Package providing utilities to load, manipulate, convert and visualize COCO format datasets."
 keywords = ["COCO", "COCO dataset"]
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -19,15 +19,15 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 license = {text="MIT"}
-dependencies = ["numpy", "rpycocotools-stubs==0.0.5"]
+dependencies = ["numpy>=1.21.0", "rpycocotools-stubs"]
 requires-python = ">=3.8"
 
 [project.urls]
 "Source Code" = "https://github.com/hoel-bagard/rust_coco_tools"
 
 [tool.maturin]
 sdist-include = ["LICENSE", "README.md"]
@@ -79,14 +79,15 @@
 max-args = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
+"python/rpycocotools/anns.py" = ["D101", "F403", "F405"]
 "tests/**/*.py" = ["D1", "INP001", "PLR2004", "S101"]
 
 [tool.pyright]
 include = ["tests"]
 ignore = ["python"]
 pythonVersion = "3.11"
 pythonPlatform = "Linux"
@@ -131,15 +132,16 @@
 inline-quotes = "double"
 # D1: Missing docstring
 # I100: Import statements are in the wrong order.
 # I201: Missing newline between import groups.
 # F401: imported but unused
 per-file-ignores = [
     "tests/*.py:D1,I201,I100",
-    "python/rpycocotools/__init__.py:F401"
+    "python/rpycocotools/__init__.py:F401,I100,NQA102",
+    "python/rpycocotools/anns.py:D101,F403,F405"
 ]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
     "import-error",
     "no-name-in-module",
```

### Comparing `rpycocotools-0.0.5/python/rpycocotools/mask.py` & `rpycocotools-0.0.6/python/rpycocotools/mask.py`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/requirements/README.md` & `rpycocotools-0.0.6/requirements/README.md`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/requirements/requirements-build.txt` & `rpycocotools-0.0.6/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/requirements/requirements-dev.txt` & `rpycocotools-0.0.6/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/requirements/requirements-doc.txt` & `rpycocotools-0.0.6/requirements/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/requirements/requirements-flake8.txt` & `rpycocotools-0.0.6/requirements/requirements-flake8.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/requirements/requirements-test.txt` & `rpycocotools-0.0.6/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/requirements/requirements.txt` & `rpycocotools-0.0.6/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/src/coco.rs` & `rpycocotools-0.0.6/src/coco.rs`

 * *Files 9% similar despite different names*

```diff
@@ -152,14 +152,42 @@
 
         let img = img
             .into_ndarray3()
             .permuted_axes([1, 2, 0])
             .into_pyarray(py);
         Ok(img)
     }
+
+    fn json(&self) -> PyResult<String> {
+        self.0
+            .json()
+            .map_err(|err| PyValueError::new_err(err.to_string()))
+    }
+}
+
+/// Construct a COCO dataset from its components and the image folder.
+///
+/// # Errors
+///
+/// Will return `Err` if there is an annotation with an image id X, but no image entry has this id.
+#[pyfunction]
+pub fn from_dataset(
+    images: Vec<object_detection::Image>,
+    annotations: Vec<object_detection::Annotation>,
+    categories: Vec<object_detection::Category>,
+    image_folder_path: &PyUnicode,
+) -> PyResult<PyCOCO> {
+    let image_folder_path = PathBuf::from(image_folder_path.to_str()?);
+    let dataset = object_detection::Dataset {
+        images,
+        annotations,
+        categories,
+    };
+    let dataset = COCO::from_dataset(dataset, image_folder_path).map_err(PyLoadingError::from)?;
+    Ok(PyCOCO(dataset))
 }
 
 #[pyclass(name = "Polygons", module = "rpycocotools.anns")]
 #[derive(Debug)]
 pub struct PyPolygons(pub cocotools::coco::object_detection::Polygons);
 
 #[pymethods]
```

### Comparing `rpycocotools-0.0.5/src/errors.rs` & `rpycocotools-0.0.6/src/errors.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/src/lib.rs` & `rpycocotools-0.0.6/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #![allow(clippy::redundant_pub_crate)]
 extern crate cocotools;
 use pyo3::types::PyDict;
-use pyo3::{prelude::*, wrap_pymodule};
+use pyo3::{prelude::*, wrap_pyfunction, wrap_pymodule};
 
 pub mod coco;
 pub mod errors;
 pub mod mask;
 
 #[pymodule]
 fn anns(_py: Python<'_>, module: &PyModule) -> PyResult<()> {
@@ -13,25 +13,26 @@
     module.add_class::<cocotools::coco::object_detection::Bbox>()?;
     module.add_class::<cocotools::coco::object_detection::Category>()?;
     module.add_class::<coco::PyPolygons>()?;
     module.add_class::<cocotools::coco::object_detection::PolygonsRS>()?;
     module.add_class::<cocotools::coco::object_detection::Rle>()?;
     module.add_class::<cocotools::coco::object_detection::CocoRle>()?;
     module.add_class::<cocotools::coco::object_detection::Image>()?;
+    module.add_function(wrap_pyfunction!(coco::from_dataset, module)?)?;
     Ok(())
 }
 
 #[pymodule]
 fn _rpycocotools(py: Python<'_>, module: &PyModule) -> PyResult<()> {
     module.add_class::<coco::PyCOCO>()?;
     module.add_wrapped(wrap_pymodule!(anns))?;
     module.add_wrapped(wrap_pymodule!(mask::py_mask))?;
 
     // Inserting to sys.modules allows importing submodules nicely from Python
     // e.g. from rpycocotools.mask import decode_rle
     let sys = PyModule::import(py, "sys")?;
     let sys_modules: &PyDict = sys.getattr("modules")?.downcast()?;
     sys_modules.set_item("_rpycocotools.mask", module.getattr("mask")?)?;
-    sys_modules.set_item("rpycocotools.anns", module.getattr("anns")?)?;
+    sys_modules.set_item("_rpycocotools.anns", module.getattr("anns")?)?;
 
     Ok(())
 }
```

### Comparing `rpycocotools-0.0.5/src/mask.rs` & `rpycocotools-0.0.6/src/mask.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/tests/test_mask.py` & `rpycocotools-0.0.6/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.5/PKG-INFO` & `rpycocotools-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: rpycocotools
-Version: 0.0.5
+Version: 0.0.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy
-Requires-Dist: rpycocotools-stubs ==0.0.5
+Requires-Dist: numpy >=1.21.0
+Requires-Dist: rpycocotools-stubs
 Requires-Dist: maturin ; extra == 'build'
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: hypothesis ; extra == 'test'
 Requires-Dist: pip-tools ; extra == 'dev'
 Requires-Dist: ruff ; extra == 'dev'
 Requires-Dist: pyright ; extra == 'dev'
 Requires-Dist: sphinx ; extra == 'doc'
@@ -47,25 +47,26 @@
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/hoel-bagard/rust_coco_tools
 
 # rpycocotools
 
-[![PyPI](https://img.shields.io/pypi/v/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
-[![PyPI - Implementation](https://img.shields.io/pypi/implementation/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
+[![PyPI](https://img.shields.io/pypi/v/rpycocotools?color=green&style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rpycocotools?style=flat-square)](https://pypistats.org/packages/rpycocotools)
 [![PyPI - License](https://img.shields.io/pypi/l/rpycocotools?style=flat)](https://opensource.org/licenses/MIT)
+![CI Python](https://github.com/hoel-bagard/cocotools-rs/actions/workflows/ci-python-rpycocotools.yaml/badge.svg)
+![CI Rust](https://github.com/hoel-bagard/cocotools-rs/actions/workflows/ci-rust-rpycocotools.yaml/badge.svg)
 
 The `rpycocotools` package provides tools to load, manipulate, convert and visualize COCO format datasets. The documentation is available [here](https://cocotools-rs.readthedocs.io/en/latest/index.html).
 
 ### Installation
 
-You can install the package through pip:
+The package is available on PyPI [here](https://pypi.org/project/rpycocotools/), and can installed with pip:
 ```
 pip install rpycocotools
 ```
 
 You can also git clone this repo and build it yourself with:
 ```
 pip install -r requirements/requirements-build.txt
@@ -86,15 +87,15 @@
   <img alt="rpycocotools_visu_example" src="https://user-images.githubusercontent.com/34478245/216580391-72226762-3fca-482b-a5ed-f93ed5a21931.png">
 </p>
 
 ```python
 import rpycocotools
 coco_dataset = rpycocotools.COCO("../data_samples/coco_25k/annotations.json", "../data_samples/coco_25k/images")
 anns = coco_dataset.get_img_anns(174482)
-mask = rpycocotools.mask.decode_poly_rs(anns[0].segmentation)
+mask = rpycocotools.mask.decode(anns[0].segmentation)
 ```
 The mask is a numpy array and can be visualized (for example with opencv):
 
 <p align="center">
   <img alt="bike_segmentation" src="https://user-images.githubusercontent.com/34478245/226691842-8a11cde1-905d-434e-b287-0c3c685e01d1.png">
 </p>
```

