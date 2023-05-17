# Comparing `tmp/savant_rs-0.1.5.tar.gz` & `tmp/savant_rs-0.1.6.tar.gz`

## Comparing `savant_rs-0.1.5.tar` & `savant_rs-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,51 @@
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 savant_rs-0.1.5/Cargo.toml
--rw-r--r--   0     1001      123     1614 2023-05-16 08:23:57.000000 savant_rs-0.1.5/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      466 2023-05-16 08:23:57.000000 savant_rs-0.1.5/.gitignore
--rw-r--r--   0     1001      123    11357 2023-05-16 08:23:57.000000 savant_rs-0.1.5/LICENSE
--rw-r--r--   0     1001      123      514 2023-05-16 08:23:57.000000 savant_rs-0.1.5/README.md
--rw-r--r--   0     1001      123      769 2023-05-16 08:23:57.000000 savant_rs-0.1.5/benches/batch_snapshot.rs
--rw-r--r--   0     1001      123     1197 2023-05-16 08:23:57.000000 savant_rs-0.1.5/benches/message_save_load.rs
--rw-r--r--   0     1001      123       71 2023-05-16 08:23:57.000000 savant_rs-0.1.5/build.rs
--rw-r--r--   0     1001      123      459 2023-05-16 08:23:57.000000 savant_rs-0.1.5/pyproject.toml
--rw-r--r--   0     1001      123     2315 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/bbox/ops.py
--rw-r--r--   0     1001      123     2533 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/bbox/savant_scale.py
--rw-r--r--   0     1001      123      783 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/buf_copy.py
--rw-r--r--   0     1001      123     3741 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/frame_ops.py
--rw-r--r--   0     1001      123     1116 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/polygon_match.py
--rw-r--r--   0     1001      123      200 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_copy.py
--rw-r--r--   0     1001      123      184 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_proxy.py
--rw-r--r--   0     1001      123      407 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_pure.py
--rw-r--r--   0     1001      123      196 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_py.py
--rw-r--r--   0     1001      123      213 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_take.py
--rw-r--r--   0     1001      123      269 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/utils/fps_meter/rust_fps_meter.py
--rw-r--r--   0     1001      123     3515 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/utils/fps_meter/savant_fps_meter.py
--rw-r--r--   0     1001      123     3386 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/utils/symbol_mapper/rust_symbol_mapper.py
--rw-r--r--   0     1001      123     7226 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/utils/symbol_mapper/savant_symbol_mapper.py
--rw-r--r--   0     1001      123     1018 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/lib.rs
--rw-r--r--   0     1001      123    14160 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/attribute.rs
--rw-r--r--   0     1001      123    16607 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/bbox.rs
--rw-r--r--   0     1001      123     1141 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/eos.rs
--rw-r--r--   0     1001      123     2807 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/loader.rs
--rw-r--r--   0     1001      123     2141 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/saver.rs
--rw-r--r--   0     1001      123     1932 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/video/batch.rs
--rw-r--r--   0     1001      123    28830 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/video/frame.rs
--rw-r--r--   0     1001      123    14359 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/video/object.rs
--rw-r--r--   0     1001      123       46 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/video.rs
--rw-r--r--   0     1001      123     6710 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message.rs
--rw-r--r--   0     1001      123      853 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/point.rs
--rw-r--r--   0     1001      123    14179 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/polygonal_area.rs
--rw-r--r--   0     1001      123     2558 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/segment.rs
--rw-r--r--   0     1001      123       87 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/to_json_value.rs
--rw-r--r--   0     1001      123     1678 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives.rs
--rw-r--r--   0     1001      123     5863 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/test.rs
--rw-r--r--   0     1001      123     1071 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/test_rkyv_tuple.rs
--rw-r--r--   0     1001      123     2521 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/tests_pyo3_access.rs
--rw-r--r--   0     1001      123     5787 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/utils/bbox.rs
--rw-r--r--   0     1001      123     5961 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/utils/fps_meter.rs
--rw-r--r--   0     1001      123    21129 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/utils/symbol_mapper.rs
--rw-r--r--   0     1001      123     2772 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/utils.rs
--rw-r--r--   0     1001      123    37853 2023-05-16 08:25:19.000000 savant_rs-0.1.5/Cargo.lock
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 savant_rs-0.1.6/Cargo.toml
+-rw-r--r--   0     1001      123     1614 2023-05-17 07:14:32.000000 savant_rs-0.1.6/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      466 2023-05-17 07:14:32.000000 savant_rs-0.1.6/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-05-17 07:14:32.000000 savant_rs-0.1.6/LICENSE
+-rw-r--r--   0     1001      123      514 2023-05-17 07:14:32.000000 savant_rs-0.1.6/README.md
+-rw-r--r--   0     1001      123      769 2023-05-17 07:14:32.000000 savant_rs-0.1.6/benches/batch_snapshot.rs
+-rw-r--r--   0     1001      123     1197 2023-05-17 07:14:32.000000 savant_rs-0.1.6/benches/message_save_load.rs
+-rw-r--r--   0     1001      123       71 2023-05-17 07:14:32.000000 savant_rs-0.1.6/build.rs
+-rw-r--r--   0     1001      123      459 2023-05-17 07:14:32.000000 savant_rs-0.1.6/pyproject.toml
+-rw-r--r--   0     1001      123     2351 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/bbox/ops.py
+-rw-r--r--   0     1001      123     2533 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/bbox/savant_scale.py
+-rw-r--r--   0     1001      123      783 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/buf_copy.py
+-rw-r--r--   0     1001      123     3741 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/frame_ops.py
+-rw-r--r--   0     1001      123     1116 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/polygon_match.py
+-rw-r--r--   0     1001      123      200 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_copy.py
+-rw-r--r--   0     1001      123      184 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_proxy.py
+-rw-r--r--   0     1001      123      407 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_pure.py
+-rw-r--r--   0     1001      123      196 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_py.py
+-rw-r--r--   0     1001      123      213 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_take.py
+-rw-r--r--   0     1001      123      269 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/fps_meter/rust_fps_meter.py
+-rw-r--r--   0     1001      123     3515 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/fps_meter/savant_fps_meter.py
+-rw-r--r--   0     1001      123      627 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/numpy_ops.py
+-rw-r--r--   0     1001      123     3386 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/symbol_mapper/rust_symbol_mapper.py
+-rw-r--r--   0     1001      123     7226 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/symbol_mapper/savant_symbol_mapper.py
+-rw-r--r--   0     1001      123     1018 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/lib.rs
+-rw-r--r--   0     1001      123    14160 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/attribute.rs
+-rw-r--r--   0     1001      123    16607 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/bbox.rs
+-rw-r--r--   0     1001      123     1141 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/eos.rs
+-rw-r--r--   0     1001      123     2807 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/loader.rs
+-rw-r--r--   0     1001      123     2141 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/saver.rs
+-rw-r--r--   0     1001      123     1932 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/video/batch.rs
+-rw-r--r--   0     1001      123    28830 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/video/frame.rs
+-rw-r--r--   0     1001      123    14359 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/video/object.rs
+-rw-r--r--   0     1001      123       46 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/video.rs
+-rw-r--r--   0     1001      123     6710 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message.rs
+-rw-r--r--   0     1001      123      853 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/point.rs
+-rw-r--r--   0     1001      123    14179 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/polygonal_area.rs
+-rw-r--r--   0     1001      123     2558 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/segment.rs
+-rw-r--r--   0     1001      123       87 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/to_json_value.rs
+-rw-r--r--   0     1001      123     1678 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives.rs
+-rw-r--r--   0     1001      123     5863 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/test.rs
+-rw-r--r--   0     1001      123     1071 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/test_rkyv_tuple.rs
+-rw-r--r--   0     1001      123     2521 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/tests_pyo3_access.rs
+-rw-r--r--   0     1001      123     6745 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/bbox.rs
+-rw-r--r--   0     1001      123      713 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/conversions.rs
+-rw-r--r--   0     1001      123     5961 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/fps_meter.rs
+-rw-r--r--   0     1001      123     8546 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/numpy_utils.rs
+-rw-r--r--   0     1001      123    21129 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/symbol_mapper.rs
+-rw-r--r--   0     1001      123     2719 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils.rs
+-rw-r--r--   0     1001      123    38841 2023-05-17 07:15:53.000000 savant_rs-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.6/PKG-INFO
```

### Comparing `savant_rs-0.1.5/Cargo.toml` & `savant_rs-0.1.6/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "savant_rs"
-version = "0.1.5"
+version = "0.1.6"
 edition = "2021"
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Savant rust optimization library"
 homepage = "https://github.com/insight-platform/savant-rs"
 repository = "https://github.com/insight-platform/savant-rs"
 readme = "README.md"
 keywords = ["computer-vision", "video-processing"]
@@ -26,14 +26,16 @@
 rkyv = { version = "0.7", features = ["validation", "archive_le"] }
 numpy = {version = "0.18", features = ["nalgebra"]}
 pyo3-log = "0.8"
 derive_builder = "0.12"
 num_cpus = "1.15"
 hashbrown = "0.13"
 lazy_static = "1.4"
+nalgebra = "0.32"
+num-traits = "0.2"
 
 [dependencies.pyo3]
 version = "0.18"
 
 [dev-dependencies]
 serial_test = "2.0"
```

### Comparing `savant_rs-0.1.5/.github/workflows/CI.yml` & `savant_rs-0.1.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/LICENSE` & `savant_rs-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/README.md` & `savant_rs-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/benches/batch_snapshot.rs` & `savant_rs-0.1.6/benches/batch_snapshot.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/benches/message_save_load.rs` & `savant_rs-0.1.6/benches/message_save_load.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/python/primitives/bbox/ops.py` & `savant_rs-0.1.6/python/primitives/bbox/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,19 +73,18 @@
 # max_x is limited to 100, max_y is limited to 500
 box = box.as_graphical_wrapping_box(padding=5, border_width=2, max_x=100, max_y=500)
 print("Graphical wrapping box:", box)
 
 print(BBox.ltwh(0, 0, 100, 100))
 print(BBox.ltrb(0, 0, 100, 100))
 
-arr = bboxes_to_ndarray_float([BBox(50.0, 50.0, 30.0, 50.0), BBox(70.0, 70.0, 50.0, 50.0)], BBoxFormat.LeftTopRightBottom)
-print(arr)
+arr = bboxes_to_ndarray([BBox(50.0, 50.0, 30.0, 50.0), BBox(70.0, 70.0, 50.0, 50.0)], BBoxFormat.LeftTopRightBottom, 'float64')
+print("BBoxes to f64", arr)
 
-boxes = ndarray_float_to_bboxes(arr, BBoxFormat.LeftTopRightBottom)
+boxes = ndarray_to_bboxes(arr, BBoxFormat.LeftTopRightBottom)
 print(boxes)
 
+arr = bboxes_to_ndarray([BBox(50.0, 50.0, 30.0, 50.0), BBox(70.0, 70.0, 50.0, 50.0)], BBoxFormat.LeftTopRightBottom, 'float32')
+print("BBoxes to f32", arr)
 
-arr = bboxes_to_ndarray_int([BBox(50.0, 50.0, 30.0, 50.0), BBox(70.0, 70.0, 50.0, 50.0)], BBoxFormat.LeftTopRightBottom)
-print(arr)
-
-boxes = ndarray_int_to_bboxes(arr, BBoxFormat.LeftTopRightBottom)
-print(boxes)
+boxes = ndarray_to_bboxes(arr, BBoxFormat.LeftTopRightBottom)
+print(boxes)
```

### Comparing `savant_rs-0.1.5/python/primitives/bbox/savant_scale.py` & `savant_rs-0.1.6/python/primitives/bbox/savant_scale.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/python/primitives/buf_copy.py` & `savant_rs-0.1.6/python/primitives/buf_copy.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/python/primitives/frame_ops.py` & `savant_rs-0.1.6/python/primitives/frame_ops.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/python/primitives/polygon_match.py` & `savant_rs-0.1.6/python/primitives/polygon_match.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/python/utils/fps_meter/savant_fps_meter.py` & `savant_rs-0.1.6/python/utils/fps_meter/savant_fps_meter.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/python/utils/symbol_mapper/rust_symbol_mapper.py` & `savant_rs-0.1.6/python/utils/symbol_mapper/rust_symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/python/utils/symbol_mapper/savant_symbol_mapper.py` & `savant_rs-0.1.6/python/utils/symbol_mapper/savant_symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/lib.rs` & `savant_rs-0.1.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/attribute.rs` & `savant_rs-0.1.6/src/primitives/attribute.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/bbox.rs` & `savant_rs-0.1.6/src/primitives/bbox.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/message/eos.rs` & `savant_rs-0.1.6/src/primitives/message/eos.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/message/loader.rs` & `savant_rs-0.1.6/src/primitives/message/loader.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/message/saver.rs` & `savant_rs-0.1.6/src/primitives/message/saver.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/message/video/batch.rs` & `savant_rs-0.1.6/src/primitives/message/video/batch.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/message/video/frame.rs` & `savant_rs-0.1.6/src/primitives/message/video/frame.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/message/video/object.rs` & `savant_rs-0.1.6/src/primitives/message/video/object.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/message.rs` & `savant_rs-0.1.6/src/primitives/message.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/point.rs` & `savant_rs-0.1.6/src/primitives/point.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/polygonal_area.rs` & `savant_rs-0.1.6/src/primitives/polygonal_area.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives/segment.rs` & `savant_rs-0.1.6/src/primitives/segment.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/primitives.rs` & `savant_rs-0.1.6/src/primitives.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/test.rs` & `savant_rs-0.1.6/src/test.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/test_rkyv_tuple.rs` & `savant_rs-0.1.6/src/test_rkyv_tuple.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/tests_pyo3_access.rs` & `savant_rs-0.1.6/src/tests_pyo3_access.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/utils/fps_meter.rs` & `savant_rs-0.1.6/src/utils/fps_meter.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/utils/symbol_mapper.rs` & `savant_rs-0.1.6/src/utils/symbol_mapper.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.5/src/utils.rs` & `savant_rs-0.1.6/src/utils.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 pub mod bbox;
+pub mod conversions;
 pub mod fps_meter;
+pub mod numpy_utils;
 pub mod symbol_mapper;
 
 use pyo3::prelude::*;
 
 use crate::primitives::message::loader::load_message_py;
 use crate::primitives::message::saver::save_message_py;
 use crate::test::utils::gen_frame;
@@ -13,14 +15,15 @@
     build_model_object_key, clear_symbol_maps, dump_registry, get_model_id, get_model_name,
     get_object_id, get_object_ids, get_object_label, get_object_labels, is_model_registered,
     is_object_registered, parse_compound_key, register_model_objects, validate_base_key,
 };
 
 pub use bbox::*;
 pub use fps_meter::FpsMeter;
+pub use numpy_utils::*;
 
 #[pyfunction]
 #[inline]
 pub fn round_2_digits(v: f64) -> f64 {
     (v * 100.0).round() / 100.0
 }
 
@@ -30,24 +33,22 @@
     // ser deser
     m.add_function(wrap_pyfunction!(save_message_py, m)?)?;
     m.add_function(wrap_pyfunction!(load_message_py, m)?)?;
     // utility
     m.add_function(wrap_pyfunction!(round_2_digits, m)?)?;
 
     // bbox batch ops
-    m.add_function(wrap_pyfunction!(bboxes_to_ndarray_float, m)?)?;
-    m.add_function(wrap_pyfunction!(rotated_bboxes_to_ndarray_float, m)?)?;
-    m.add_function(wrap_pyfunction!(ndarray_float_to_bboxes, m)?)?;
-    m.add_function(wrap_pyfunction!(ndarray_float_to_bboxes, m)?)?;
-
-    // bbox batch ops
-    m.add_function(wrap_pyfunction!(bboxes_to_ndarray_int, m)?)?;
-    m.add_function(wrap_pyfunction!(rotated_bboxes_to_ndarray_int, m)?)?;
-    m.add_function(wrap_pyfunction!(ndarray_int_to_bboxes, m)?)?;
-    m.add_function(wrap_pyfunction!(ndarray_int_to_bboxes, m)?)?;
+    m.add_function(wrap_pyfunction!(rotated_bboxes_to_ndarray_py, m)?)?;
+    m.add_function(wrap_pyfunction!(bboxes_to_ndarray_py, m)?)?;
+    m.add_function(wrap_pyfunction!(ndarray_to_bboxes_py, m)?)?;
+    m.add_function(wrap_pyfunction!(ndarray_to_rotated_bboxes_py, m)?)?;
+
+    // numpy utils
+    m.add_function(wrap_pyfunction!(ndarray_to_matrix_py, m)?)?;
+    m.add_function(wrap_pyfunction!(matrix_to_ndarray_py, m)?)?;
 
     // model object registry
     m.add_function(wrap_pyfunction!(build_model_object_key, m)?)?;
     m.add_function(wrap_pyfunction!(clear_symbol_maps, m)?)?;
     m.add_function(wrap_pyfunction!(dump_registry, m)?)?;
     m.add_function(wrap_pyfunction!(get_model_id, m)?)?;
     m.add_function(wrap_pyfunction!(get_model_name, m)?)?;
@@ -61,10 +62,11 @@
     m.add_function(wrap_pyfunction!(register_model_objects, m)?)?;
     m.add_function(wrap_pyfunction!(validate_base_key, m)?)?;
 
     m.add_class::<FpsMeter>()?;
     m.add_class::<SymbolMapper>()?;
     m.add_class::<RegistrationPolicy>()?;
     m.add_class::<BBoxFormat>()?;
+    m.add_class::<Matrix>()?;
 
     Ok(())
 }
```

### Comparing `savant_rs-0.1.5/Cargo.lock` & `savant_rs-0.1.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "bytemuck"
+version = "1.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
+
+[[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "cc"
@@ -619,22 +625,35 @@
 [[package]]
 name = "nalgebra"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d68d47bba83f9e2006d117a9a33af1524e655516b8919caac694427a6fb1e511"
 dependencies = [
  "approx",
+ "matrixmultiply",
+ "nalgebra-macros",
  "num-complex",
  "num-rational",
  "num-traits",
  "simba",
  "typenum",
 ]
 
 [[package]]
+name = "nalgebra-macros"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d232c68884c0c99810a5a4d333ef7e47689cfd0edc85efc9e54e1e6bf5212766"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
  "matrixmultiply",
  "num-complex",
@@ -1011,24 +1030,35 @@
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
+name = "safe_arch"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
+dependencies = [
+ "bytemuck",
+]
+
+[[package]]
 name = "savant_rs"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "anyhow",
  "derive_builder",
  "env_logger",
  "geo",
  "hashbrown 0.13.2",
  "itertools",
  "lazy_static",
+ "nalgebra",
+ "num-traits",
  "num_cpus",
  "numpy",
  "pyo3",
  "pyo3-build-config",
  "pyo3-log",
  "rayon",
  "rkyv",
@@ -1117,14 +1147,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
 dependencies = [
  "approx",
  "num-complex",
  "num-traits",
  "paste",
+ "wide",
 ]
 
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
@@ -1276,14 +1307,24 @@
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "wide"
+version = "0.7.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b689b6c49d6549434bf944e6b0f39238cf63693cb7a147e9d887507fffa3b223"
+dependencies = [
+ "bytemuck",
+ "safe_arch",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
```

### Comparing `savant_rs-0.1.5/PKG-INFO` & `savant_rs-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savant_rs
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Savant rust optimization library
 Keywords: computer-vision,video-processing
 Home-Page: https://github.com/insight-platform/savant-rs
```

