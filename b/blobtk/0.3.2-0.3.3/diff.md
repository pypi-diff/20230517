# Comparing `tmp/blobtk-0.3.2.tar.gz` & `tmp/blobtk-0.3.3.tar.gz`

## Comparing `blobtk-0.3.2.tar` & `blobtk-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 blobtk-0.3.2/Cargo.toml
--rw-r--r--   0      501       20    59960 2023-05-16 08:39:04.000000 blobtk-0.3.2/Cargo.lock
--rw-r--r--   0      501       20      313 2023-05-16 08:39:04.000000 blobtk-0.3.2/pyproject.toml
--rw-r--r--   0      501       20     9018 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/bam.rs
--rw-r--r--   0      501       20    18205 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/blobdir.rs
--rw-r--r--   0      501       20     8832 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/cli.rs
--rw-r--r--   0      501       20      553 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/depth.rs
--rw-r--r--   0      501       20     1855 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/fasta.rs
--rw-r--r--   0      501       20     6177 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/fastq.rs
--rw-r--r--   0      501       20     1440 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/filter.rs
--rw-r--r--   0      501       20     2738 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/io.rs
--rw-r--r--   0      501       20      788 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/lib.rs
--rw-r--r--   0      501       20      659 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/main.rs
--rw-r--r--   0      501       20     4150 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/axis.rs
--rw-r--r--   0      501       20    22218 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/blob.rs
--rw-r--r--   0      501       20     5567 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/category.rs
--rw-r--r--   0      501       20     5730 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/chart.rs
--rw-r--r--   0      501       20    38034 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/component.rs
--rw-r--r--   0      501       20     5835 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/cumulative.rs
--rw-r--r--   0      501       20     4398 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/data.rs
--rw-r--r--   0      501       20    29932 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/snail.rs
--rw-r--r--   0      501       20     1020 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/style.rs
--rw-r--r--   0      501       20    11606 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot.rs
--rw-r--r--   0      501       20     3172 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/python/depth.rs
--rw-r--r--   0      501       20     3518 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/python/filter.rs
--rw-r--r--   0      501       20     1879 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/python/utils.rs
--rw-r--r--   0      501       20      491 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/python.rs
--rw-r--r--   0      501       20     4497 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/taxonomy.rs
--rw-r--r--   0      501       20     8053 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/utils.rs
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 blobtk-0.3.3/Cargo.toml
+-rw-r--r--   0      501       20    59960 2023-05-17 09:24:31.000000 blobtk-0.3.3/Cargo.lock
+-rw-r--r--   0      501       20      313 2023-05-17 09:24:31.000000 blobtk-0.3.3/pyproject.toml
+-rw-r--r--   0      501       20     9018 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/bam.rs
+-rw-r--r--   0      501       20    18356 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/blobdir.rs
+-rw-r--r--   0      501       20     8832 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/cli.rs
+-rw-r--r--   0      501       20      553 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/depth.rs
+-rw-r--r--   0      501       20     1855 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/fasta.rs
+-rw-r--r--   0      501       20     6177 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/fastq.rs
+-rw-r--r--   0      501       20     1440 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/filter.rs
+-rw-r--r--   0      501       20     2738 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/io.rs
+-rw-r--r--   0      501       20      788 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/lib.rs
+-rw-r--r--   0      501       20      659 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/main.rs
+-rw-r--r--   0      501       20     4150 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/axis.rs
+-rw-r--r--   0      501       20    22218 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/blob.rs
+-rw-r--r--   0      501       20     5567 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/category.rs
+-rw-r--r--   0      501       20     5730 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/chart.rs
+-rw-r--r--   0      501       20    38034 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/component.rs
+-rw-r--r--   0      501       20     5835 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/cumulative.rs
+-rw-r--r--   0      501       20     4398 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/data.rs
+-rw-r--r--   0      501       20    29932 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/snail.rs
+-rw-r--r--   0      501       20     1020 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/style.rs
+-rw-r--r--   0      501       20    11606 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot.rs
+-rw-r--r--   0      501       20     3172 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/python/depth.rs
+-rw-r--r--   0      501       20     3518 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/python/filter.rs
+-rw-r--r--   0      501       20     1879 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/python/utils.rs
+-rw-r--r--   0      501       20      491 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/python.rs
+-rw-r--r--   0      501       20     4497 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/taxonomy.rs
+-rw-r--r--   0      501       20     8053 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/utils.rs
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.3/PKG-INFO
```

### Comparing `blobtk-0.3.2/Cargo.toml` & `blobtk-0.3.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "blobtk"
-version = "0.3.2"
+version = "0.3.3"
 edition = "2021"
 authors = [
     "Rich Challis <rc28@sanger.ac.uk>",
 ]
 license = "MIT"
 description = "Core utilities for BlobToolKit."
 homepage = "https://github.com/blobtoolkit/blobtk"
```

### Comparing `blobtk-0.3.2/Cargo.lock` & `blobtk-0.3.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blobtk"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "atty",
  "clap",
  "clap-num",
  "colorous",
  "coord_transforms",
  "flate2",
```

### Comparing `blobtk-0.3.2/src/bam.rs` & `blobtk-0.3.3/src/bam.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/blobdir.rs` & `blobtk-0.3.3/src/blobdir.rs`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 #[derive(Serialize, Deserialize, Debug)]
 pub struct AssemblyMeta {
     #[serde(default = "default_accession")]
     pub accession: String,
     #[serde(default = "default_level")]
     pub level: String,
-    pub prefix: String,
+    pub prefix: Option<String>,
     pub alias: Option<String>,
     pub bioproject: Option<String>,
     pub biosample: Option<String>,
     pub file: Option<PathBuf>,
     #[serde(rename = "scaffold-count")]
     pub scaffold_count: Option<usize>,
     pub span: Option<usize>,
@@ -88,22 +88,30 @@
     pub class: Option<String>,
     pub family: Option<String>,
     pub genus: Option<String>,
     pub kingdom: Option<String>,
     pub order: Option<String>,
     pub phylum: Option<String>,
     pub superkingdom: Option<String>,
-    #[serde(deserialize_with = "deserialize_string_from_number")]
+    #[serde(
+        default = "default_taxid",
+        deserialize_with = "deserialize_string_from_number"
+    )]
     pub taxid: String,
 }
 
+fn default_taxid() -> String {
+    "0".to_string()
+}
+
 #[derive(Serialize, Deserialize, Debug)]
 pub struct Meta {
     pub id: String,
     pub name: String,
+    #[serde(default = "default_level")]
     pub record_type: String,
     pub records: usize,
     #[serde(default = "default_revision")]
     pub revision: u8,
     #[serde(default = "default_version")]
     pub version: u8,
     pub assembly: AssemblyMeta,
```

### Comparing `blobtk-0.3.2/src/cli.rs` & `blobtk-0.3.3/src/cli.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/depth.rs` & `blobtk-0.3.3/src/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/fasta.rs` & `blobtk-0.3.3/src/fasta.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/fastq.rs` & `blobtk-0.3.3/src/fastq.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/filter.rs` & `blobtk-0.3.3/src/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/io.rs` & `blobtk-0.3.3/src/io.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/lib.rs` & `blobtk-0.3.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/main.rs` & `blobtk-0.3.3/src/main.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/axis.rs` & `blobtk-0.3.3/src/plot/axis.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/blob.rs` & `blobtk-0.3.3/src/plot/blob.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/category.rs` & `blobtk-0.3.3/src/plot/category.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/chart.rs` & `blobtk-0.3.3/src/plot/chart.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/component.rs` & `blobtk-0.3.3/src/plot/component.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/cumulative.rs` & `blobtk-0.3.3/src/plot/cumulative.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/data.rs` & `blobtk-0.3.3/src/plot/data.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/snail.rs` & `blobtk-0.3.3/src/plot/snail.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot/style.rs` & `blobtk-0.3.3/src/plot/style.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/plot.rs` & `blobtk-0.3.3/src/plot.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/python/depth.rs` & `blobtk-0.3.3/src/python/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/python/filter.rs` & `blobtk-0.3.3/src/python/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/python/utils.rs` & `blobtk-0.3.3/src/python/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/taxonomy.rs` & `blobtk-0.3.3/src/taxonomy.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/src/utils.rs` & `blobtk-0.3.3/src/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.2/PKG-INFO` & `blobtk-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtk
-Version: 0.3.2
+Version: 0.3.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Core utilities for BlobToolKit.
 Keywords: bioinformatics,blobtoolkit,genome,genomics
 Home-Page: https://github.com/blobtoolkit/blobtk
 Author: Rich Challis <rc28@sanger.ac.uk>
```

