# Comparing `tmp/bimcvcovid19i-0.0.7.tar.gz` & `tmp/bimcvcovid19i-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimcvcovid19i-0.0.7.tar", last modified: Wed May 10 22:27:43 2023, max compression
+gzip compressed data, was "bimcvcovid19i-0.1.0.tar", last modified: Wed May 17 12:10:11 2023, max compression
```

## Comparing `bimcvcovid19i-0.0.7.tar` & `bimcvcovid19i-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1088 2022-10-18 07:33:34.000000 bimcvcovid19i-0.0.7/LICENSE
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      169 2022-10-18 07:33:57.000000 bimcvcovid19i-0.0.7/MANIFEST.in
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/PKG-INFO
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      675 2023-05-10 22:10:21.000000 bimcvcovid19i-0.0.7/README.md
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/bimcvcovid19i/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 11:36:01.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/__init__.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/__init__.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       22 2023-05-10 22:26:40.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/__version__.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/__version__.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      884 2023-05-10 21:16:06.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/assets.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      285 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/assets.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)    17304 2023-05-10 21:41:37.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/data.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2058 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/data.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2022-10-18 16:36:33.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/interface.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/interface.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4886 2022-12-03 14:07:39.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/postprocessing.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1333 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/postprocessing.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      225 2022-10-18 07:10:47.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/py.typed
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6745 2023-05-10 22:04:37.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/tools.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1261 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/tools.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6995 2023-05-10 22:05:50.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/typing.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2438 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/typing.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     3802 2023-05-08 09:47:17.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/webdav.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      501 2023-05-10 22:27:42.000000 bimcvcovid19i-0.0.7/bimcvcovid19i/webdav.pyi
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/PKG-INFO
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      769 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/SOURCES.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/dependency_links.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-18 07:36:29.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/not-zip-safe
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/requires.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       14 2023-05-10 22:27:43.000000 bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/top_level.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2022-12-02 14:19:33.000000 bimcvcovid19i-0.0.7/requirements.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       38 2023-05-10 22:27:43.767092 bimcvcovid19i-0.0.7/setup.cfg
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1325 2022-10-18 09:08:11.000000 bimcvcovid19i-0.0.7/setup.py
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1088 2022-10-18 07:33:34.000000 bimcvcovid19i-0.1.0/LICENSE
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      169 2022-10-18 07:33:57.000000 bimcvcovid19i-0.1.0/MANIFEST.in
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/PKG-INFO
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      675 2023-05-10 22:10:21.000000 bimcvcovid19i-0.1.0/README.md
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/bimcvcovid19i/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 11:36:01.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/__init__.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/__init__.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       22 2023-05-17 12:09:46.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/__version__.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/__version__.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      884 2023-05-10 21:16:06.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/assets.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      285 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/assets.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)    17902 2023-05-12 13:02:59.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/data.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2058 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/data.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4918 2023-05-17 12:08:44.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/interface.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1660 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/interface.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4886 2022-12-03 14:07:39.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/postprocessing.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1333 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/postprocessing.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      225 2022-10-18 07:10:47.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/py.typed
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6745 2023-05-10 22:04:37.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/tools.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1261 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/tools.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6995 2023-05-10 22:05:50.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/typing.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2438 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/typing.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     3802 2023-05-08 09:47:17.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/webdav.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      501 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/webdav.pyi
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/PKG-INFO
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      769 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/SOURCES.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/dependency_links.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-18 07:36:29.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/not-zip-safe
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/requires.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       14 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/top_level.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2022-12-02 14:19:33.000000 bimcvcovid19i-0.1.0/requirements.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       38 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/setup.cfg
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1325 2022-10-18 09:08:11.000000 bimcvcovid19i-0.1.0/setup.py
```

### Comparing `bimcvcovid19i-0.0.7/LICENSE` & `bimcvcovid19i-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/PKG-INFO` & `bimcvcovid19i-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimcvcovid19i
-Version: 0.0.7
+Version: 0.1.0
 Summary: Interface for working with BIMCV COVID 19 dataset
 Home-page: https://github.com/rilshok/BIMCV-COVID-19-interface
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bimcvcovid19i-0.0.7/README.md` & `bimcvcovid19i-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/assets.py` & `bimcvcovid19i-0.1.0/bimcvcovid19i/assets.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/data.py` & `bimcvcovid19i-0.1.0/bimcvcovid19i/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,66 +71,76 @@
     def sessions_iter(self) -> tp.Iterator[Path]:
         """Unpacks the next session into a temporary folder and returns the path to it"""
         part_paths = sorted(list(self.original.glob("*part*.tar.gz")))
         with TemporaryDirectory() as temp_root:
             temp_root_ = Path(temp_root)
             for part_path in part_paths:
                 logging.info("Start processing tar file: %s", part_path.name)
-                with tarfile.open(part_path) as part_file:
-                    members = part_file.getmembers()
-
-                    # extracting root paths for sessions inside an archive
-                    sessions_root_paths = {}
-                    for member in members:
-                        member_path = member.name
-                        member_path_split = member_path.split("/")
-                        if not member_path_split[-1].startswith("ses-"):
-                            continue
-                        if not member_path_split[-2].startswith("sub-"):
-                            continue
-                        session_id = member_path_split[-1]
-                        assert member.isdir()
-                        sessions_root_paths[session_id] = member_path
-
-                    # extract paths to each file inside an archive.
-                    # distribution of paths by sessions
-
-                    sessions_element_paths: tp.Dict[str, tp.List[str]] = {
-                        uid: [] for uid in sessions_root_paths
-                    }
-
-                    for member in members:
-                        if not member.isfile():
-                            continue
-                        member_path = member.name
+                try:
+                    with tarfile.open(part_path) as part_file:
+                        members = part_file.getmembers()
 
-                        for uid, sessions_root in sessions_root_paths.items():
-                            if member_path.startswith(sessions_root):
-                                sessions_element_paths[uid].append(member_path)
-                                break
-                        else:
-                            raise AssertionError
-
-                    for session_id, part_file_paths in sessions_element_paths.items():
-                        logging.info("Extracting session %s files", session_id)
-                        session_root = temp_root_ / session_id
-                        session_root.mkdir()
-                        part_file_session_root = Path(sessions_root_paths[session_id])
-                        for path in part_file_paths:
-                            file_path = session_root / Path(path).relative_to(
-                                part_file_session_root
+                        # extracting root paths for sessions inside an archive
+                        sessions_root_paths = {}
+                        for member in members:
+                            member_path = member.name
+                            member_path_split = member_path.split("/")
+                            if not member_path_split[-1].startswith("ses-"):
+                                continue
+                            if not member_path_split[-2].startswith("sub-"):
+                                continue
+                            session_id = member_path_split[-1]
+                            assert member.isdir()
+                            sessions_root_paths[session_id] = member_path
+
+                        # extract paths to each file inside an archive.
+                        # distribution of paths by sessions
+
+                        sessions_element_paths: tp.Dict[str, tp.List[str]] = {
+                            uid: [] for uid in sessions_root_paths
+                        }
+
+                        for member in members:
+                            if not member.isfile():
+                                continue
+                            member_path = member.name
+
+                            for uid, sessions_root in sessions_root_paths.items():
+                                if member_path.startswith(sessions_root):
+                                    sessions_element_paths[uid].append(member_path)
+                                    break
+                            else:
+                                msg = f"{member.name=} not found in sessions_root_paths"
+                                msg += f"patrt file = {part_path}"
+                                print(msg)
+
+                        for (
+                            session_id,
+                            part_file_paths,
+                        ) in sessions_element_paths.items():
+                            logging.info("Extracting session %s files", session_id)
+                            session_root = temp_root_ / session_id
+                            session_root.mkdir()
+                            part_file_session_root = Path(
+                                sessions_root_paths[session_id]
                             )
-                            file_path.parent.mkdir(parents=True, exist_ok=True)
-
-                            with open(file_path, "wb") as file:
-                                data = part_file.extractfile(path)
-                                assert data is not None
-                                file.write(data.read())
-                        yield session_root
-                        shutil.rmtree(session_root)
+                            for path in part_file_paths:
+                                file_path = session_root / Path(path).relative_to(
+                                    part_file_session_root
+                                )
+                                file_path.parent.mkdir(parents=True, exist_ok=True)
+
+                                with open(file_path, "wb") as file:
+                                    data = part_file.extractfile(path)
+                                    assert data is not None
+                                    file.write(data.read())
+                            yield session_root
+                            shutil.rmtree(session_root)
+                except Exception as exc:
+                    print(exc.__class__, exc)
 
     def series_iter(self) -> tp.Iterator[Series]:
         session_dirs = self.sessions_iter()
         for session_root in session_dirs:
             for series_raw_path in _group_series_files_by_name(session_root):
                 logging.info("Series %s reading", series_raw_path.uid)
                 try:
@@ -400,20 +410,23 @@
 
     subjects_tarfile_name = "covid19_posi_metadata.tar.gz"
     subjects_tarfile_subpath = "covid19_posi/participants.tsv"
 
     sessions_tarfile_name = "covid19_posi_sessions_tsv.tar.gz"
 
     tests_tarfile_name = "covid19_posi_derivative.tar.gz"
-    tests_tarfile_subpath = "covid19_posi/derivatives/EHR/SIL_REG_COVID_POSI_iter123.txt"
+    tests_tarfile_subpath = (
+        "covid19_posi/derivatives/EHR/SIL_REG_COVID_POSI_iter123.txt"
+    )
     # TODO: covid19_posi/derivatives/EHR/ contains other *.csv files
 
     labels_tarfile_name = "covid19_posi_derivative.tar.gz"
     labels_tarfile_subpath = "covid19_posi/derivatives/labels/Labels_covid_123.tsv"
 
+
 class BIMCVCOVID19negativeData_12(BIMCVCOVID19Data):
     webdav_hostname = "https://b2drop.bsc.es/public.php/webdav"
     webdav_login = "BIMCV-COVID19-cIter_1_2-Negative"
     webdav_password = "maybeempty"
 
     subjects_tarfile_name = "covid19_neg_metadata.tar.gz"
     subjects_tarfile_subpath = "covid19_neg/participants.tsv"
```

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/data.pyi` & `bimcvcovid19i-0.1.0/bimcvcovid19i/data.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/postprocessing.py` & `bimcvcovid19i-0.1.0/bimcvcovid19i/postprocessing.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/postprocessing.pyi` & `bimcvcovid19i-0.1.0/bimcvcovid19i/postprocessing.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/tools.py` & `bimcvcovid19i-0.1.0/bimcvcovid19i/tools.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/tools.pyi` & `bimcvcovid19i-0.1.0/bimcvcovid19i/tools.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/typing.py` & `bimcvcovid19i-0.1.0/bimcvcovid19i/typing.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/typing.pyi` & `bimcvcovid19i-0.1.0/bimcvcovid19i/typing.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i/webdav.py` & `bimcvcovid19i-0.1.0/bimcvcovid19i/webdav.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/PKG-INFO` & `bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimcvcovid19i
-Version: 0.0.7
+Version: 0.1.0
 Summary: Interface for working with BIMCV COVID 19 dataset
 Home-page: https://github.com/rilshok/BIMCV-COVID-19-interface
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bimcvcovid19i-0.0.7/bimcvcovid19i.egg-info/SOURCES.txt` & `bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.7/setup.py` & `bimcvcovid19i-0.1.0/setup.py`

 * *Files identical despite different names*

