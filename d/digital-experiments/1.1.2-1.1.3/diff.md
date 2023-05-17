# Comparing `tmp/digital-experiments-1.1.2.tar.gz` & `tmp/digital-experiments-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-experiments-1.1.2.tar", last modified: Wed May 10 08:36:11 2023, max compression
+gzip compressed data, was "digital-experiments-1.1.3.tar", last modified: Wed May 17 15:51:06 2023, max compression
```

## Comparing `digital-experiments-1.1.2.tar` & `digital-experiments-1.1.3.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:36:11.902091 digital-experiments-1.1.2/
--rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.1.2/LICENSE
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-10 08:36:11.901941 digital-experiments-1.1.2/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/README.md
--rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-10 08:35:31.000000 digital-experiments-1.1.2/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-05-10 08:36:11.902142 digital-experiments-1.1.2/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:36:11.896913 digital-experiments-1.1.2/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:36:11.899256 digital-experiments-1.1.2/src/digital_experiments/
--rw-r--r--   0 john       (504) staff       (20)      139 2023-05-10 08:35:31.000000 digital-experiments-1.1.2/src/digital_experiments/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     7031 2023-05-10 08:34:42.000000 digital-experiments-1.1.2/src/digital_experiments/backends.py
--rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/src/digital_experiments/control_center.py
--rw-r--r--   0 john       (504) staff       (20)     3651 2023-05-09 14:17:13.000000 digital-experiments-1.1.2/src/digital_experiments/experiment.py
--rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/src/digital_experiments/inspection.py
--rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/src/digital_experiments/metadata.py
--rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.1.2/src/digital_experiments/minimize.py
--rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/src/digital_experiments/observation.py
--rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.1.2/src/digital_experiments/pretty.py
--rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.1.2/src/digital_experiments/querying.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:36:11.900384 digital-experiments-1.1.2/src/digital_experiments/search/
--rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/src/digital_experiments/search/skopt_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/src/digital_experiments/search/space.py
--rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.1.2/src/digital_experiments/search/suggest.py
--rw-r--r--   0 john       (504) staff       (20)     3837 2023-05-10 08:20:22.000000 digital-experiments-1.1.2/src/digital_experiments/util.py
--rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/src/digital_experiments/version_control.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:36:11.899969 digital-experiments-1.1.2/src/digital_experiments.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-10 08:36:11.000000 digital-experiments-1.1.2/src/digital_experiments.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1070 2023-05-10 08:36:11.000000 digital-experiments-1.1.2/src/digital_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-05-10 08:36:11.000000 digital-experiments-1.1.2/src/digital_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      160 2023-05-10 08:36:11.000000 digital-experiments-1.1.2/src/digital_experiments.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       32 2023-05-10 08:36:11.000000 digital-experiments-1.1.2/src/digital_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:36:11.901736 digital-experiments-1.1.2/tests/
--rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.1.2/tests/test_backends.py
--rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/tests/test_control_center.py
--rw-r--r--   0 john       (504) staff       (20)     1179 2023-05-09 14:17:13.000000 digital-experiments-1.1.2/tests/test_experiment.py
--rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/tests/test_metadata.py
--rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/tests/test_minimize.py
--rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.1.2/tests/test_pretty.py
--rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.1.2/tests/test_querying.py
--rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.1.2/tests/test_space.py
--rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.1.2/tests/test_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     2309 2023-05-10 08:20:22.000000 digital-experiments-1.1.2/tests/test_util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.194426 digital-experiments-1.1.3/
+-rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.1.3/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 15:51:06.194268 digital-experiments-1.1.3/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-17 15:50:59.000000 digital-experiments-1.1.3/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-05-17 15:51:06.194471 digital-experiments-1.1.3/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.188239 digital-experiments-1.1.3/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.190868 digital-experiments-1.1.3/src/digital_experiments/
+-rw-r--r--   0 john       (504) staff       (20)      138 2023-05-17 15:50:59.000000 digital-experiments-1.1.3/src/digital_experiments/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     6877 2023-05-17 15:48:49.000000 digital-experiments-1.1.3/src/digital_experiments/backends.py
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/src/digital_experiments/control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     4377 2023-05-17 15:50:20.000000 digital-experiments-1.1.3/src/digital_experiments/experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/inspection.py
+-rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.1.3/src/digital_experiments/minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/observation.py
+-rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.1.3/src/digital_experiments/pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.1.3/src/digital_experiments/querying.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.191942 digital-experiments-1.1.3/src/digital_experiments/search/
+-rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/search/skopt_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/search/space.py
+-rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.1.3/src/digital_experiments/search/suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     1682 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/src/digital_experiments/timing.py
+-rw-r--r--   0 john       (504) staff       (20)     5211 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/src/digital_experiments/util.py
+-rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/src/digital_experiments/version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.191577 digital-experiments-1.1.3/src/digital_experiments.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1147 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      160 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       20 2023-05-17 15:51:06.000000 digital-experiments-1.1.3/src/digital_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-17 15:51:06.193940 digital-experiments-1.1.3/tests/
+-rw-r--r--   0 john       (504) staff       (20)     2083 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_backends.py
+-rw-r--r--   0 john       (504) staff       (20)      844 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/tests/test_control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     2099 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      391 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_inspection.py
+-rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/tests/test_minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      309 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_observation.py
+-rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.1.3/tests/test_pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.1.3/tests/test_querying.py
+-rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.1.3/tests/test_space.py
+-rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.1.3/tests/test_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)      682 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/tests/test_timing.py
+-rw-r--r--   0 john       (504) staff       (20)     2820 2023-05-17 15:42:42.000000 digital-experiments-1.1.3/tests/test_util.py
+-rw-r--r--   0 john       (504) staff       (20)     2397 2023-05-17 11:01:07.000000 digital-experiments-1.1.3/tests/test_version_control.py
```

### Comparing `digital-experiments-1.1.2/LICENSE` & `digital-experiments-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/PKG-INFO` & `digital-experiments-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.1.2
+Version: 1.1.3
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.1.2/README.md` & `digital-experiments-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/pyproject.toml` & `digital-experiments-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digital-experiments"
-version = "1.1.2"
+version = "1.1.3"
 description = "Keep track of digital experiments."
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
     "pytest-cov",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/digital-experiments"
 
 [tool.bumpver]
-current_version = "1.1.2"
+current_version = "1.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digital-experiments-1.1.2/src/digital_experiments/backends.py` & `digital-experiments-1.1.3/src/digital_experiments/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import contextlib
 import pickle
 import shutil
 from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass
 from functools import partial
 from pathlib import Path
 from typing import Dict, List
 
 import pandas as pd
 import yaml
 
-from .control_center import Run
 from .observation import Observation
 from .util import dict_equality, exclusive_file_access, flatten, generate_id, unflatten
 
 __BACKENDS: Dict[str, "Backend"] = {}
 
 
 def register_backend(name: str, cls: "Backend"):
@@ -83,22 +81,20 @@
         self.home = home
 
     @abstractmethod
     def save(self, obs: Observation):
         """
         save an observation object to the backend
         """
-        pass
 
     @abstractmethod
     def all_observations(self) -> List[Observation]:
         """
         load all observations from the backend
         """
-        pass
 
     @classmethod
     def create_new(cls, location: Path, code: str):
         """
         Create a new backend at the given location.
         """
         assert not location.exists(), f"{location} already exists"
@@ -106,41 +102,47 @@
 
         # label this directory as a digital experiment
         # and store various required metadata
         HomeLabel.create_new(location, cls.name, code)
 
         return cls(location)
 
-    @contextlib.contextmanager
     def unique_run(self):
+        """
+        Create a new unique run.
+        """
+
         id = generate_id()
         directory = self.home / Files.RUNS / id
         directory.mkdir(parents=True, exist_ok=False)
 
-        run = Run(id, directory)
+        return id, directory
 
-        yield run  # experiments happen while this is yielded
+    def clean_up(self, id):
+        """
+        clean up after the run with the given id has finished
+        """
 
-        if not any(run.directory.iterdir()):
-            shutil.rmtree(run.directory)
+        directory = self.home / Files.RUNS / id
+        if not any(directory.iterdir()):
+            shutil.rmtree(directory)
 
     @staticmethod
     def from_existing(home: Path):
         """
         Load an existing backend from the given location.
         """
 
         label = HomeLabel.from_existing(home)
         return backend_from_type(label.backend_name)(home)
 
-    def _observation_for_(self, config):
-        for obs in self.all_observations():
-            if dict_equality(obs.config, config):
-                return obs
-        return None
+    def _observations_for_(self, config):
+        return [
+            obs for obs in self.all_observations() if dict_equality(obs.config, config)
+        ]
 
 
 @this_is_a_backend("yaml")
 class YAMLBackend(Backend):
     @property
     def yaml_file(self):
         return self.home / "observations.yaml"
@@ -150,21 +152,15 @@
         with exclusive_file_access(self.yaml_file, "a") as f:
             yaml.dump([obs], f, indent=2)
 
     def all_observations(self) -> List[Observation]:
         if not self.yaml_file.exists():
             return []
         with exclusive_file_access(self.yaml_file) as f:
-            return yaml.load(f, Loader=ObservationLoader)
-
-
-class ObservationLoader(yaml.Loader):
-    def construct_observation(self, node):
-        data = self.construct_mapping(node)
-        return Observation(**data)
+            return yaml.load(f, Loader=yaml.Loader)
 
 
 @this_is_a_backend("csv")
 class CSVBackend(Backend):
     SEPARATOR = "|"
 
     @property
```

### Comparing `digital-experiments-1.1.2/src/digital_experiments/experiment.py` & `digital-experiments-1.1.3/src/digital_experiments/experiment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 from functools import partial
 from pathlib import Path
-from typing import Union
+from typing import Dict, Union
 
-from . import control_center as GLOBAL
-from . import querying
+from . import control_center as ControlCenter
+from . import querying, timing
 from .inspection import code_for, complete_config
-from .metadata import record_metadata
 from .observation import Observation
 from .pretty import pretty_instance
 from .version_control import get_or_create_backend_for
 
 
 def experiment(
     experiment_fn=None,
     *,
     backend: str = "yaml",
     root: str = None,
     absolute_root: Union[str, Path] = None,
     verbose: bool = False,
-    cache: bool = True,
+    cache: bool = False,
 ):
     """
     decorator to record an experiment
     """
     if experiment_fn is None:
-        return partial(
-            experiment,
-            backend=backend,
-            root=root,
-            absolute_root=absolute_root,
-            verbose=verbose,
-            cache=cache,
-        )
+        kwargs = locals()
+        kwargs.pop("experiment_fn")
+        return partial(experiment, **kwargs)
 
     # get the directory of the file where the experiment is defined
     # and where <root> should be relative to
     expmt_file = Path(experiment_fn.__code__.co_filename).parent
     if "ipykernel" in str(expmt_file):
         expmt_file = Path(".")
 
@@ -61,47 +55,71 @@
     ):
         self._experiment = experiment
         self._backend = get_or_create_backend_for(root, code_for(experiment), backend)
         self.verbose = verbose
         self.cache = cache
 
     def run(self, args: list, kwargs: dict):
-        if not GLOBAL.should_record():
-            return self._experiment(*args, **kwargs)
+        """
+        run the experiment with the given arguments and save the result
+        """
 
         config = complete_config(self._experiment, args, kwargs)
 
-        previous_observation = self._backend._observation_for_(config)
-        if self.cache and previous_observation is not None:
+        # check if we've run this experiment before
+        previous_observations = self._backend._observations_for_(config)
+        if self.cache and len(previous_observations) > 0:
+            previous_observation = previous_observations[0]
             return previous_observation.result
 
-        with self._backend.unique_run() as run, GLOBAL.recording_run(run):
-            id = run.id
-            if self.verbose:
-                print(
-                    f"digital-experiments: Running experiment {id} with config: {config}"
-                )
-            metadata, result = record_metadata(self._experiment, args, kwargs)
-            if self.verbose:
-                print(
-                    f"digital-experiments: Finished experiment {id} with result: {result}"
-                )
+        # if we're not recording, just run the experiment
+        if not ControlCenter.should_record():
+            return self._experiment(*args, **kwargs)
+
+        # otherwise, run the experiment and record the result
+        id, directory = self._backend.unique_run()
+        ControlCenter.start_run(id, directory)
+        self._log(f"Running experiment {id} with config: {config}")
+        timing.mark("start")
+        result = self._experiment(*args, **kwargs)
+        timing.mark("end")
+        self._log(f"Finished experiment {id} with result: {result}")
+        finished_run = ControlCenter.end_run()
+        self._backend.clean_up(id)
 
-        observation = Observation(id, config, result, metadata)
+        observation = Observation(id, config, result, finished_run.metadata)
         self._backend.save(observation)
 
         return result
 
     def __call__(self, *args, **kwargs):
         return self.run(args, kwargs)
 
+    def _log(self, msg):
+        if self.verbose:
+            print(f"digital-experiments: {self._experiment.__name__}: {msg}")
+
     @property
     def observations(self):
         return self._backend.all_observations()
 
+    def observation_for(self, config: Dict):
+        """
+        return the observation for the given config
+        """
+        observations = self._backend._observations_for_(config)
+        if len(observations) == 0:
+            return None
+
+        if len(observations) > 1:
+            raise Exception(
+                f"Found multiple observations for config {config}: {observations}"
+            )
+        return observations[0]
+
     def to_dataframe(
         self,
         include_metadata=False,
         include_id=True,
         config=None,
         metadata=None,
         result=None,
```

### Comparing `digital-experiments-1.1.2/src/digital_experiments/minimize.py` & `digital-experiments-1.1.3/src/digital_experiments/minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/src/digital_experiments/observation.py` & `digital-experiments-1.1.3/src/digital_experiments/observation.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/src/digital_experiments/pretty.py` & `digital-experiments-1.1.3/src/digital_experiments/pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/src/digital_experiments/querying.py` & `digital-experiments-1.1.3/src/digital_experiments/querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/src/digital_experiments/search/skopt_suggest.py` & `digital-experiments-1.1.3/src/digital_experiments/search/skopt_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/src/digital_experiments/search/space.py` & `digital-experiments-1.1.3/src/digital_experiments/search/space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/src/digital_experiments/search/suggest.py` & `digital-experiments-1.1.3/src/digital_experiments/search/suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/src/digital_experiments/version_control.py` & `digital-experiments-1.1.3/src/digital_experiments/version_control.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/src/digital_experiments.egg-info/PKG-INFO` & `digital-experiments-1.1.3/src/digital_experiments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.1.2
+Version: 1.1.3
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.1.2/src/digital_experiments.egg-info/SOURCES.txt` & `digital-experiments-1.1.3/src/digital_experiments.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 README.md
 pyproject.toml
 src/digital_experiments/__init__.py
 src/digital_experiments/backends.py
 src/digital_experiments/control_center.py
 src/digital_experiments/experiment.py
 src/digital_experiments/inspection.py
-src/digital_experiments/metadata.py
 src/digital_experiments/minimize.py
 src/digital_experiments/observation.py
 src/digital_experiments/pretty.py
 src/digital_experiments/querying.py
+src/digital_experiments/timing.py
 src/digital_experiments/util.py
 src/digital_experiments/version_control.py
 src/digital_experiments.egg-info/PKG-INFO
 src/digital_experiments.egg-info/SOURCES.txt
 src/digital_experiments.egg-info/dependency_links.txt
 src/digital_experiments.egg-info/requires.txt
 src/digital_experiments.egg-info/top_level.txt
 src/digital_experiments/search/skopt_suggest.py
 src/digital_experiments/search/space.py
 src/digital_experiments/search/suggest.py
 tests/test_backends.py
 tests/test_control_center.py
 tests/test_experiment.py
-tests/test_metadata.py
+tests/test_inspection.py
 tests/test_minimize.py
+tests/test_observation.py
 tests/test_pretty.py
 tests/test_querying.py
 tests/test_space.py
 tests/test_suggest.py
-tests/test_util.py
+tests/test_timing.py
+tests/test_util.py
+tests/test_version_control.py
```

### Comparing `digital-experiments-1.1.2/tests/test_backends.py` & `digital-experiments-1.1.3/tests/test_backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+from digital_experiments import experiment
 from digital_experiments.backends import (
     Backend,
     available_backends,
     backend_from_type,
     this_is_a_backend,
 )
 from digital_experiments.observation import Observation
@@ -70,15 +71,23 @@
     """
 
     klass = backend_from_type(backend)
     assert klass.name == backend
 
     home = tmp_path / backend
     home.mkdir()
-    backend = klass(home)
-    backend.save(Observation(id="1", config={"a": 1, "b": 2}, result=1))
+    backend_instance = klass(home)
+    backend_instance.save(Observation(id="1", config={"a": 1, "b": 2}, result=1))
 
-    observations = backend.all_observations()
+    observations = backend_instance.all_observations()
     assert len(observations) == 1
     assert observations[0].id == "1"
     assert observations[0].config == {"a": 1, "b": 2}
     assert observations[0].result == 1
+
+    @experiment(backend=backend, absolute_root=tmp_path)
+    def add(a, b):
+        return a + b
+
+    add(1, 2)
+
+    assert len(add.observations) == 1
```

### Comparing `digital-experiments-1.1.2/tests/test_experiment.py` & `digital-experiments-1.1.3/tests/test_experiment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import shutil
 from pathlib import Path
 
+import pytest
+
+from digital_experiments.backends import available_backends
 from digital_experiments.experiment import experiment
 
 
 def test_absolute_path(tmp_path):
     if tmp_path.exists():
         shutil.rmtree(tmp_path)
 
@@ -53,7 +56,42 @@
 
     ret = add(1, 2)
     assert calls == 1
     assert ret == 3
 
     add(1, 3)
     assert calls == 2
+
+
+def test_verbose(capsys, tmp_path):
+    @experiment(verbose=True, absolute_root=tmp_path)
+    def add(a, b):
+        return a + b
+
+    add(1, 2)
+    captured = capsys.readouterr()
+
+    assert "Running experiment" in captured.out
+    assert "Finished experiment" in captured.out
+
+
+def test_repr(tmp_path):
+    @experiment(absolute_root=tmp_path)
+    def add(a, b):
+        return a + b
+
+    add(1, 2)
+    add(2, 3)
+    assert repr(add) == "Experiment(add, observations=2)"
+
+
+@pytest.mark.parametrize("backend", available_backends())
+def test_backends(backend, tmp_path):
+    @experiment(backend=backend, absolute_root=tmp_path)
+    def add(a, b):
+        return a + b
+
+    add(1, 2)
+    assert len(add.observations) == 1
+    observation = add.observations[0]
+    assert observation.config == {"a": 1, "b": 2}
+    assert observation.result == 3
```

### Comparing `digital-experiments-1.1.2/tests/test_minimize.py` & `digital-experiments-1.1.3/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/tests/test_pretty.py` & `digital-experiments-1.1.3/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/tests/test_querying.py` & `digital-experiments-1.1.3/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/tests/test_space.py` & `digital-experiments-1.1.3/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/tests/test_suggest.py` & `digital-experiments-1.1.3/tests/test_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.2/tests/test_util.py` & `digital-experiments-1.1.3/tests/test_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from digital_experiments.util import (
     dict_equality,
     flatten,
     generate_id,
     get_passed_kwargs,
     get_passed_kwargs_for,
     intersect,
+    merge_dicts,
     unflatten,
     union,
 )
 
 nested = {"a": 1, "b": {"c": 2, "d": {"f": "hi"}}}
 flat = {"a": 1, "b_c": 2, "b_d_f": "hi"}
 
@@ -76,7 +77,26 @@
 
     # get_passed_kwargs_for should return a dict of the correct types
     # by inferring them either from
     #  - the defaults in a signature
     #  - type hints
     kwargs = get_passed_kwargs_for(test_experiment)
     assert kwargs == {"a": 1, "b": False, "c": "hello"}
+
+
+def test_merge_dicts():
+    d1 = {"a": {"b": 1, "c": 2}, "d": 3}
+    d2 = {"a": {"e": 5}, "f": 6}
+
+    # ensure correct nested merge
+    assert merge_dicts(d1, d2) == {"a": {"b": 1, "c": 2, "e": 5}, "d": 3, "f": 6}
+
+    bad_d2 = {"a": 1}
+    with pytest.raises(ValueError):
+        merge_dicts(d1, bad_d2)
+
+    bad_d2 = {"d": 4}
+    with pytest.raises(ValueError):
+        merge_dicts(d1, bad_d2)
+
+    good_d2 = {"d": 3}
+    assert merge_dicts(d1, good_d2) == {"a": {"b": 1, "c": 2}, "d": 3}
```

