# Comparing `tmp/savant_rs-0.1.6.tar.gz` & `tmp/savant_rs-0.1.7.tar.gz`

## Comparing `savant_rs-0.1.6.tar` & `savant_rs-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 savant_rs-0.1.6/Cargo.toml
--rw-r--r--   0     1001      123     1614 2023-05-17 07:14:32.000000 savant_rs-0.1.6/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      466 2023-05-17 07:14:32.000000 savant_rs-0.1.6/.gitignore
--rw-r--r--   0     1001      123    11357 2023-05-17 07:14:32.000000 savant_rs-0.1.6/LICENSE
--rw-r--r--   0     1001      123      514 2023-05-17 07:14:32.000000 savant_rs-0.1.6/README.md
--rw-r--r--   0     1001      123      769 2023-05-17 07:14:32.000000 savant_rs-0.1.6/benches/batch_snapshot.rs
--rw-r--r--   0     1001      123     1197 2023-05-17 07:14:32.000000 savant_rs-0.1.6/benches/message_save_load.rs
--rw-r--r--   0     1001      123       71 2023-05-17 07:14:32.000000 savant_rs-0.1.6/build.rs
--rw-r--r--   0     1001      123      459 2023-05-17 07:14:32.000000 savant_rs-0.1.6/pyproject.toml
--rw-r--r--   0     1001      123     2351 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/bbox/ops.py
--rw-r--r--   0     1001      123     2533 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/bbox/savant_scale.py
--rw-r--r--   0     1001      123      783 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/buf_copy.py
--rw-r--r--   0     1001      123     3741 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/frame_ops.py
--rw-r--r--   0     1001      123     1116 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/primitives/polygon_match.py
--rw-r--r--   0     1001      123      200 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_copy.py
--rw-r--r--   0     1001      123      184 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_proxy.py
--rw-r--r--   0     1001      123      407 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_pure.py
--rw-r--r--   0     1001      123      196 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_py.py
--rw-r--r--   0     1001      123      213 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/test_pyo3_access/get_take.py
--rw-r--r--   0     1001      123      269 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/fps_meter/rust_fps_meter.py
--rw-r--r--   0     1001      123     3515 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/fps_meter/savant_fps_meter.py
--rw-r--r--   0     1001      123      627 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/numpy_ops.py
--rw-r--r--   0     1001      123     3386 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/symbol_mapper/rust_symbol_mapper.py
--rw-r--r--   0     1001      123     7226 2023-05-17 07:14:32.000000 savant_rs-0.1.6/python/utils/symbol_mapper/savant_symbol_mapper.py
--rw-r--r--   0     1001      123     1018 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/lib.rs
--rw-r--r--   0     1001      123    14160 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/attribute.rs
--rw-r--r--   0     1001      123    16607 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/bbox.rs
--rw-r--r--   0     1001      123     1141 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/eos.rs
--rw-r--r--   0     1001      123     2807 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/loader.rs
--rw-r--r--   0     1001      123     2141 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/saver.rs
--rw-r--r--   0     1001      123     1932 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/video/batch.rs
--rw-r--r--   0     1001      123    28830 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/video/frame.rs
--rw-r--r--   0     1001      123    14359 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/video/object.rs
--rw-r--r--   0     1001      123       46 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message/video.rs
--rw-r--r--   0     1001      123     6710 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/message.rs
--rw-r--r--   0     1001      123      853 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/point.rs
--rw-r--r--   0     1001      123    14179 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/polygonal_area.rs
--rw-r--r--   0     1001      123     2558 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/segment.rs
--rw-r--r--   0     1001      123       87 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives/to_json_value.rs
--rw-r--r--   0     1001      123     1678 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/primitives.rs
--rw-r--r--   0     1001      123     5863 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/test.rs
--rw-r--r--   0     1001      123     1071 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/test_rkyv_tuple.rs
--rw-r--r--   0     1001      123     2521 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/tests_pyo3_access.rs
--rw-r--r--   0     1001      123     6745 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/bbox.rs
--rw-r--r--   0     1001      123      713 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/conversions.rs
--rw-r--r--   0     1001      123     5961 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/fps_meter.rs
--rw-r--r--   0     1001      123     8546 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/numpy_utils.rs
--rw-r--r--   0     1001      123    21129 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils/symbol_mapper.rs
--rw-r--r--   0     1001      123     2719 2023-05-17 07:14:32.000000 savant_rs-0.1.6/src/utils.rs
--rw-r--r--   0     1001      123    38841 2023-05-17 07:15:53.000000 savant_rs-0.1.6/Cargo.lock
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 savant_rs-0.1.7/Cargo.toml
+-rw-r--r--   0     1001      123     1614 2023-05-17 10:52:40.000000 savant_rs-0.1.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      466 2023-05-17 10:52:40.000000 savant_rs-0.1.7/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-05-17 10:52:40.000000 savant_rs-0.1.7/LICENSE
+-rw-r--r--   0     1001      123      514 2023-05-17 10:52:40.000000 savant_rs-0.1.7/README.md
+-rw-r--r--   0     1001      123      769 2023-05-17 10:52:40.000000 savant_rs-0.1.7/benches/batch_snapshot.rs
+-rw-r--r--   0     1001      123     1197 2023-05-17 10:52:40.000000 savant_rs-0.1.7/benches/message_save_load.rs
+-rw-r--r--   0     1001      123       71 2023-05-17 10:52:40.000000 savant_rs-0.1.7/build.rs
+-rw-r--r--   0     1001      123      459 2023-05-17 10:52:40.000000 savant_rs-0.1.7/pyproject.toml
+-rw-r--r--   0     1001      123     2351 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/bbox/ops.py
+-rw-r--r--   0     1001      123     2531 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/bbox/savant_scale.py
+-rw-r--r--   0     1001      123      783 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/buf_copy.py
+-rw-r--r--   0     1001      123     3785 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/frame_ops.py
+-rw-r--r--   0     1001      123     1116 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/polygon_match.py
+-rw-r--r--   0     1001      123      200 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_copy.py
+-rw-r--r--   0     1001      123      184 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_proxy.py
+-rw-r--r--   0     1001      123      407 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_pure.py
+-rw-r--r--   0     1001      123      196 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_py.py
+-rw-r--r--   0     1001      123      213 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_take.py
+-rw-r--r--   0     1001      123      269 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/fps_meter/rust_fps_meter.py
+-rw-r--r--   0     1001      123     3515 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/fps_meter/savant_fps_meter.py
+-rw-r--r--   0     1001      123      627 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/numpy_ops.py
+-rw-r--r--   0     1001      123     3387 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/symbol_mapper/rust_symbol_mapper.py
+-rw-r--r--   0     1001      123     7231 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/symbol_mapper/savant_symbol_mapper.py
+-rw-r--r--   0     1001      123      997 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/lib.rs
+-rw-r--r--   0     1001      123    14160 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/attribute.rs
+-rw-r--r--   0     1001      123    16607 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/bbox.rs
+-rw-r--r--   0     1001      123     1141 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/eos.rs
+-rw-r--r--   0     1001      123     2807 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/loader.rs
+-rw-r--r--   0     1001      123     2135 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/saver.rs
+-rw-r--r--   0     1001      123     1932 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/video/batch.rs
+-rw-r--r--   0     1001      123    28830 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/video/frame.rs
+-rw-r--r--   0     1001      123    14359 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/video/object.rs
+-rw-r--r--   0     1001      123       46 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/video.rs
+-rw-r--r--   0     1001      123     6736 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message.rs
+-rw-r--r--   0     1001      123      853 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/point.rs
+-rw-r--r--   0     1001      123    14179 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/polygonal_area.rs
+-rw-r--r--   0     1001      123     2558 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/segment.rs
+-rw-r--r--   0     1001      123       87 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/to_json_value.rs
+-rw-r--r--   0     1001      123     1678 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives.rs
+-rw-r--r--   0     1001      123     5863 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/test.rs
+-rw-r--r--   0     1001      123     2521 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/tests_pyo3_access.rs
+-rw-r--r--   0     1001      123     6745 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/bbox.rs
+-rw-r--r--   0     1001      123      713 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/conversions.rs
+-rw-r--r--   0     1001      123     5961 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/fps_meter.rs
+-rw-r--r--   0     1001      123     8546 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/numpy_utils.rs
+-rw-r--r--   0     1001      123    21129 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/symbol_mapper.rs
+-rw-r--r--   0     1001      123     2719 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils.rs
+-rw-r--r--   0     1001      123    38841 2023-05-17 10:54:16.000000 savant_rs-0.1.7/Cargo.lock
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.7/PKG-INFO
```

### Comparing `savant_rs-0.1.6/Cargo.toml` & `savant_rs-0.1.7/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "savant_rs"
-version = "0.1.6"
+version = "0.1.7"
 edition = "2021"
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Savant rust optimization library"
 homepage = "https://github.com/insight-platform/savant-rs"
 repository = "https://github.com/insight-platform/savant-rs"
 readme = "README.md"
 keywords = ["computer-vision", "video-processing"]
```

### Comparing `savant_rs-0.1.6/.github/workflows/CI.yml` & `savant_rs-0.1.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/LICENSE` & `savant_rs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/README.md` & `savant_rs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/benches/batch_snapshot.rs` & `savant_rs-0.1.7/benches/batch_snapshot.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/benches/message_save_load.rs` & `savant_rs-0.1.7/benches/message_save_load.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/python/primitives/bbox/ops.py` & `savant_rs-0.1.7/python/primitives/bbox/ops.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/python/primitives/bbox/savant_scale.py` & `savant_rs-0.1.7/python/primitives/bbox/savant_scale.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 
 
 from timeit import default_timer as timer
 
 bbox = [0, 0, 100, 100, 0]
 
 t = timer()
-for _ in range(100):
+for _ in range(10000):
     res = scale_rbbox(np.array([bbox]), 2, 3)
 
 print(f"Time to scale (python): {timer() - t}")
 
-bbox = BBox(0, 0, 100, 100, None)
+bbox = BBox(0, 0, 100, 100)
 
 t = timer()
-for _ in range(100):
+for _ in range(10000):
     res = bbox.scale(2, 3)
 
 print(f"Time to scale (rust): {timer() - t}")
```

### Comparing `savant_rs-0.1.6/python/primitives/buf_copy.py` & `savant_rs-0.1.7/python/primitives/buf_copy.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/python/primitives/frame_ops.py` & `savant_rs-0.1.7/python/primitives/frame_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     Value.float(1.0, confidence=0.5),
     Value.string("hello", confidence=0.5),
     Value.boolean(True, confidence=0.5),
     Value.strings(["hello", "world"], confidence=0.5),
     Value.integers([1, 2, 3], confidence=0.5),
     Value.floats([1.0, 2.0, 3.0], confidence=0.5),
     Value.booleans([True, False, True], confidence=0.5),
-    Value.bbox(BBox(0.1, 0.2, 0.3, 0.4), confidence=0.5),
-    Value.bboxes([BBox(0.1, 0.2, 0.3, 0.4), BBox(0.1, 0.2, 0.3, 0.4)], confidence=0.5),
+    Value.bbox(BBox(0.1, 0.2, 0.3, 0.4).as_rbbox(), confidence=0.5),
+    Value.bboxes([BBox(0.1, 0.2, 0.3, 0.4).as_rbbox(), BBox(0.1, 0.2, 0.3, 0.4).as_rbbox()], confidence=0.5),
     Value.point(Point(0.1, 0.2), confidence=0.5),
     Value.points([Point(0.1, 0.2), Point(0.1, 0.2)], confidence=0.5),
     Value.polygon(PolygonalArea([Point(-1, 1), Point(1, 1), Point(1, -1), Point(-1, -1)], ["up", None, "down", None]), confidence=0.5),
     Value.polygons([
         PolygonalArea([Point(-1, 1), Point(1, 1), Point(1, -1), Point(-1, -1)], ["up", None, "down", None]),
         PolygonalArea([Point(-1, 1), Point(1, 1), Point(1, -1), Point(-1, -1)], ["up", None, "down", None])], confidence=0.5),
 ]))
@@ -84,15 +84,15 @@
 deleted = frame.delete_attribute(creator="some", name="attr")
 print(deleted)
 
 frame.add_object(Object(
     id=1,
     creator="some",
     label="person",
-    bbox=BBox(0.1, 0.2, 0.3, 0.4),
+    bbox=BBox(0.1, 0.2, 0.3, 0.4).as_rbbox(),
     confidence=0.5,
     attributes={},
     parent=ParentObject(id=2, creator="some", label="car"),
     track_id=None,
 ))
 
 o = frame.access_objects_by_id([1])
```

### Comparing `savant_rs-0.1.6/python/primitives/polygon_match.py` & `savant_rs-0.1.7/python/primitives/polygon_match.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/python/utils/fps_meter/savant_fps_meter.py` & `savant_rs-0.1.7/python/utils/fps_meter/savant_fps_meter.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/python/utils/numpy_ops.py` & `savant_rs-0.1.7/python/utils/numpy_ops.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/python/utils/symbol_mapper/rust_symbol_mapper.py` & `savant_rs-0.1.7/python/utils/symbol_mapper/rust_symbol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 print(f"Time to get in individually (total: {total}, idle: {total - single_total_time}): {num}, cnt: {cntr}, time spent in counter {cntr / 10_000_000 * mil_count}")
 
 
 def batched_count():
     total_time = timer()
     random_model = choice(models)
     random_objects = [f"object_{choice(range(1000))}_{random_model}" for _ in range(100)]
-    num = 100000
+    num = 100_000
     for _ in range(num):
         get_object_ids(model_name=random_model, object_labels=random_objects)
     return num, timer() - total_time
 
 
 num, single_total_time = batched_count()
```

### Comparing `savant_rs-0.1.6/python/utils/symbol_mapper/savant_symbol_mapper.py` & `savant_rs-0.1.7/python/utils/symbol_mapper/savant_symbol_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     def threaded_count():
         global cntr, exit_flag
         while not exit_flag:
             cntr += plus_one()
 
     t = timer()
     cnt = 0
-    while cnt < 1000_000:
+    while cnt < 10_000_000:
         cnt += plus_one()
 
     mil_count = timer() - t
     print(f"Time to count to million: {mil_count}")
 
     res = 0
     for m in models:
@@ -192,15 +192,15 @@
         res += timer() - t
 
     print(f"Time to register: {res}")
 
     def simple_count():
         res = 0
         total_time = timer()
-        for _ in range(1000_000):
+        for _ in range(10_000_000):
             random_model = choice(models)
             random_object = f"object_{choice(range(1000))}_{random_model}"
             t = timer()
             m = registry.get_model_uid(random_model)
             m, o = registry.get_model_object_ids(model_name=random_model, object_label=random_object)
             res += timer() - t
         return res, timer() - total_time
@@ -209,8 +209,8 @@
     cntr = 0
     exit_flag = False
     t = threading.Thread(target=threaded_count)
     t.start()
     res, total_time = simple_count()
     exit_flag = True
     t.join()
-    print(f"Time to get in individually ({total_time}): {res}, cnt: {cntr}, time spent in counter {cntr / 1_000_000 * mil_count}")
+    print(f"Time to get in individually ({total_time}): {res}, cnt: {cntr}, time spent in counter {cntr / 10_000_000 * mil_count}")
```

### Comparing `savant_rs-0.1.6/src/lib.rs` & `savant_rs-0.1.7/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 pub mod primitives;
 pub mod test;
-mod test_rkyv_tuple;
 pub mod tests_pyo3_access;
 pub mod utils;
 
 use crate::tests_pyo3_access::{
     CopyWrapper, Internal, InternalMtx, InternalNoClone, ProxyWrapper, TakeWrapper, Wrapper,
 };
```

### Comparing `savant_rs-0.1.6/src/primitives/attribute.rs` & `savant_rs-0.1.7/src/primitives/attribute.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/bbox.rs` & `savant_rs-0.1.7/src/primitives/bbox.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/message/eos.rs` & `savant_rs-0.1.7/src/primitives/message/eos.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/message/loader.rs` & `savant_rs-0.1.7/src/primitives/message/loader.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/message/saver.rs` & `savant_rs-0.1.7/src/primitives/message/saver.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 #[pyfunction]
 #[pyo3(name = "save_message")]
 pub fn save_message_py(frame: Message) -> Vec<u8> {
     Python::with_gil(|py| py.allow_threads(|| save_message(frame)))
 }
 
-pub fn save_message(frame: Message) -> Vec<u8> {
-    match frame.frame {
+pub fn save_message(m: Message) -> Vec<u8> {
+    match m.payload {
         NativeMessage::EndOfStream(s) => {
             let mut buf = Vec::with_capacity(32);
             buf.extend_from_slice(
                 rkyv::to_bytes::<_, 32>(&s)
                     .expect("Failed to serialize EndOfStream")
                     .as_ref(),
             );
```

### Comparing `savant_rs-0.1.6/src/primitives/message/video/batch.rs` & `savant_rs-0.1.7/src/primitives/message/video/batch.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/message/video/frame.rs` & `savant_rs-0.1.7/src/primitives/message/video/frame.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/message/video/object.rs` & `savant_rs-0.1.7/src/primitives/message/video/object.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/message.rs` & `savant_rs-0.1.7/src/primitives/message.rs`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         }
     }
 }
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct Message {
-    frame: NativeMessage,
+    payload: NativeMessage,
 }
 
 #[pymethods]
 impl Message {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
@@ -67,86 +67,86 @@
     fn __str__(&self) -> String {
         self.__repr__()
     }
 
     #[staticmethod]
     pub fn unknown(s: String) -> Self {
         Self {
-            frame: NativeMessage::Unknown(s),
+            payload: NativeMessage::Unknown(s),
         }
     }
 
     #[staticmethod]
     pub fn video_frame(frame: VideoFrame) -> Self {
         Self {
-            frame: NativeMessage::VideoFrame(frame),
+            payload: NativeMessage::VideoFrame(frame),
         }
     }
 
     #[staticmethod]
     pub fn video_frame_batch(batch: VideoFrameBatch) -> Self {
         Self {
-            frame: NativeMessage::VideoFrameBatch(batch),
+            payload: NativeMessage::VideoFrameBatch(batch),
         }
     }
 
     #[staticmethod]
     pub fn end_of_stream(eos: EndOfStream) -> Self {
         Self {
-            frame: NativeMessage::EndOfStream(eos),
+            payload: NativeMessage::EndOfStream(eos),
         }
     }
 
     #[getter]
     pub fn is_unknown(&self) -> bool {
-        matches!(self.frame, NativeMessage::Unknown(_))
+        matches!(self.payload, NativeMessage::Unknown(_))
     }
 
     #[getter]
     pub fn is_end_of_stream(&self) -> bool {
-        matches!(self.frame, NativeMessage::EndOfStream(_))
+        matches!(self.payload, NativeMessage::EndOfStream(_))
     }
 
     #[getter]
     pub fn is_video_frame(&self) -> bool {
-        matches!(self.frame, NativeMessage::VideoFrame(_))
+        matches!(self.payload, NativeMessage::VideoFrame(_))
     }
 
     #[getter]
     pub fn is_video_frame_batch(&self) -> bool {
-        matches!(self.frame, NativeMessage::VideoFrameBatch(_))
+        matches!(self.payload, NativeMessage::VideoFrameBatch(_))
     }
 
     #[getter]
     pub fn as_unknown(&self) -> Option<String> {
-        match &self.frame {
+        match &self.payload {
             NativeMessage::Unknown(s) => Some(s.clone()),
             _ => None,
         }
     }
 
     #[getter]
     pub fn as_end_of_stream(&self) -> Option<EndOfStream> {
-        match &self.frame {
+        match &self.payload {
             NativeMessage::EndOfStream(eos) => Some(eos.clone()),
             _ => None,
         }
     }
 
     #[getter]
     pub fn as_video_frame(&self) -> Option<VideoFrame> {
-        match &self.frame {
+        match &self.payload {
             NativeMessage::VideoFrame(frame) => Some(frame.clone()),
             _ => None,
         }
     }
 
     #[getter]
     pub fn as_video_frame_batch(&self) -> Option<VideoFrameBatch> {
-        match &self.frame {
+        match &self.payload {
             NativeMessage::VideoFrameBatch(batch) => Some(batch.clone()),
             _ => None,
         }
     }
 }
 
 #[cfg(test)]
```

### Comparing `savant_rs-0.1.6/src/primitives/point.rs` & `savant_rs-0.1.7/src/primitives/point.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/polygonal_area.rs` & `savant_rs-0.1.7/src/primitives/polygonal_area.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives/segment.rs` & `savant_rs-0.1.7/src/primitives/segment.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/primitives.rs` & `savant_rs-0.1.7/src/primitives.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/test.rs` & `savant_rs-0.1.7/src/test.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/tests_pyo3_access.rs` & `savant_rs-0.1.7/src/tests_pyo3_access.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/utils/bbox.rs` & `savant_rs-0.1.7/src/utils/bbox.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/utils/conversions.rs` & `savant_rs-0.1.7/src/utils/conversions.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/utils/fps_meter.rs` & `savant_rs-0.1.7/src/utils/fps_meter.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/utils/numpy_utils.rs` & `savant_rs-0.1.7/src/utils/numpy_utils.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/utils/symbol_mapper.rs` & `savant_rs-0.1.7/src/utils/symbol_mapper.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/src/utils.rs` & `savant_rs-0.1.7/src/utils.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.6/Cargo.lock` & `savant_rs-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1040,15 +1040,15 @@
 checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "savant_rs"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "anyhow",
  "derive_builder",
  "env_logger",
  "geo",
  "hashbrown 0.13.2",
  "itertools",
```

### Comparing `savant_rs-0.1.6/PKG-INFO` & `savant_rs-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savant_rs
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Savant rust optimization library
 Keywords: computer-vision,video-processing
 Home-Page: https://github.com/insight-platform/savant-rs
```

