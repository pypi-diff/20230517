# Comparing `tmp/TACTUS-live-1.1.0.tar.gz` & `tmp/tactus-live-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TACTUS-live-1.1.0.tar", last modified: Tue May 16 08:58:40 2023, max compression
+gzip compressed data, was "tactus-live-1.2.0.tar", last modified: Wed May 17 08:51:21 2023, max compression
```

## Comparing `TACTUS-live-1.1.0.tar` & `tactus-live-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:58:40.817401 TACTUS-live-1.1.0/
--rw-rw-rw-   0        0        0      715 2023-05-16 08:58:40.816415 TACTUS-live-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-05-15 16:33:04.000000 TACTUS-live-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 08:58:40.805415 TACTUS-live-1.1.0/TACTUS_live.egg-info/
--rw-rw-rw-   0        0        0      715 2023-05-16 08:58:40.000000 TACTUS-live-1.1.0/TACTUS_live.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-16 08:58:40.000000 TACTUS-live-1.1.0/TACTUS_live.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:58:40.000000 TACTUS-live-1.1.0/TACTUS_live.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-16 08:58:40.000000 TACTUS-live-1.1.0/TACTUS_live.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-16 08:58:40.000000 TACTUS-live-1.1.0/TACTUS_live.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      723 2023-05-16 08:56:54.000000 TACTUS-live-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 08:58:40.817401 TACTUS-live-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 08:58:40.810412 TACTUS-live-1.1.0/tactus_live/
--rw-rw-rw-   0        0        0        0 2023-05-15 16:31:30.000000 TACTUS-live-1.1.0/tactus_live/__init__.py
--rw-rw-rw-   0        0        0     4192 2023-05-16 08:53:16.000000 TACTUS-live-1.1.0/tactus_live/main.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:58:40.813408 TACTUS-live-1.1.0/tactus_live/utils/
--rw-rw-rw-   0        0        0     1838 2023-05-16 08:48:48.000000 TACTUS-live-1.1.0/tactus_live/utils/kafka_producer.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:51:21.488751 tactus-live-1.2.0/
+-rw-rw-rw-   0        0        0      715 2023-05-17 08:51:21.487746 tactus-live-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-05-15 16:33:04.000000 tactus-live-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 08:51:21.467749 tactus-live-1.2.0/TACTUS_live.egg-info/
+-rw-rw-rw-   0        0        0      715 2023-05-17 08:51:21.000000 tactus-live-1.2.0/TACTUS_live.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-05-17 08:51:21.000000 tactus-live-1.2.0/TACTUS_live.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 08:51:21.000000 tactus-live-1.2.0/TACTUS_live.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-17 08:51:21.000000 tactus-live-1.2.0/TACTUS_live.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-17 08:51:21.000000 tactus-live-1.2.0/TACTUS_live.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      723 2023-05-17 08:50:20.000000 tactus-live-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 08:51:21.488751 tactus-live-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 08:51:21.476746 tactus-live-1.2.0/tactus_live/
+-rw-rw-rw-   0        0        0        0 2023-05-15 16:31:30.000000 tactus-live-1.2.0/tactus_live/__init__.py
+-rw-rw-rw-   0        0        0     4302 2023-05-16 10:49:14.000000 tactus-live-1.2.0/tactus_live/main.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:51:21.485746 tactus-live-1.2.0/tactus_live/utils/
+-rw-rw-rw-   0        0        0     1838 2023-05-16 08:48:48.000000 tactus-live-1.2.0/tactus_live/utils/kafka_producer.py
```

### Comparing `TACTUS-live-1.1.0/PKG-INFO` & `tactus-live-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TACTUS-live
-Version: 1.1.0
+Name: tactus-live
+Version: 1.2.0
 Summary: Threatening activities classification toward users' security
 Project-URL: repository, https://github.com/Cranfield-GDP3/TACTUS-live
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `TACTUS-live-1.1.0/TACTUS_live.egg-info/PKG-INFO` & `tactus-live-1.2.0/TACTUS_live.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TACTUS-live
-Version: 1.1.0
+Name: tactus-live
+Version: 1.2.0
 Summary: Threatening activities classification toward users' security
 Project-URL: repository, https://github.com/Cranfield-GDP3/TACTUS-live
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `TACTUS-live-1.1.0/tactus_live/main.py` & `tactus-live-1.2.0/tactus_live/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 from tactus_model import FeatureTracker, Classifier, PredTracker
 from deep_sort_realtime.deepsort_tracker import DeepSort
 from deep_sort_realtime.deep_sort.track import Track
 
 from tactus_live.utils.kafka_producer import KafkaProducer
 
 
-def main(device: str = "cuda:0"):
+def main(device: str = "cuda:0", use_kafka_logger = False):
     deepsort_tracker = DeepSort(n_init=5, max_age=10, device=device)
     pose_model = PosePredictionYolov8(Path("data/raw/models"), "yolov8m-pose.pt", device)
 
     classifier = Classifier.load(Path("data/models/BEST_RUS.pickle"))
     feature_tracker = FeatureTracker(classifier.window_size, classifier.angle_to_compute)
     pred_tracker = PredTracker()
 
     cap = VideoCapture(r"C:\Users\marco\Downloads\img_7350 low bitrate.mp4",
                        target_fps=10,
                        tqdm_progressbar=tqdm.tqdm())
 
-    kafka_producer = KafkaProducer(stream_ip="1.1.1.1", topic_name="camera1/detections", sensor_id="camera1", client_id="x")
+    if use_kafka_logger:
+        kafka_producer = KafkaProducer(ip_adress="1.1.1.1", topic_name="camera1/detections", sensor_id="camera1", client_id="x")
 
     pr1 = Profile()
     pr1.enable()
     try:
         while (cap_frame := cap.read())[1] is not None:
             frame_id, frame = cap_frame
 
@@ -61,15 +62,16 @@
 
                         prediction = classifier.predict_label([features])[0]
 
                         if prediction != "neutral":
                             skeleton = feature_tracker.rolling_windows[track_id].skeleton
                             pred_tracker.add_pred(track_id, prediction, skeleton)
 
-                            kafka_producer.send_event("violence", "violence is happening on this camera")
+                            if use_kafka_logger:
+                                kafka_producer.send_event("violence", "violence is happening on this camera")
 
                 frame = plot_skeleton(frame, skeleton, track, feature_tracker, pred_tracker)
 
             save_dir = Path("data/visualisation")
             save_path = save_dir / (str(frame_id) + ".jpg")
             cv2.imwrite(str(save_path), frame)
```

### Comparing `TACTUS-live-1.1.0/tactus_live/utils/kafka_producer.py` & `tactus-live-1.2.0/tactus_live/utils/kafka_producer.py`

 * *Files identical despite different names*

