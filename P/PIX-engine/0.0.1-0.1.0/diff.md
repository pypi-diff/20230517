# Comparing `tmp/pix_engine-0.0.1.tar.gz` & `tmp/pix_engine-0.1.0.tar.gz`

## Comparing `pix_engine-0.0.1.tar` & `pix_engine-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 pix_engine-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pix_engine-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pix_engine-0.0.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pix_engine-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pix_engine-0.0.1/pix/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pix_engine-0.0.1/pix/pix.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pix_engine-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pix_engine-0.0.1/LICENSE
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pix_engine-0.0.1/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pix_engine-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 pix_engine-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pix_engine-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 pix_engine-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pix_engine-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pix_engine-0.1.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pix_engine-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pix_engine-0.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pix_engine-0.1.0/pix/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pix_engine-0.1.0/pix/pix.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pix_engine-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pix_engine-0.1.0/LICENSE
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pix_engine-0.1.0/README.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pix_engine-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pix_engine-0.1.0/PKG-INFO
```

### Comparing `pix_engine-0.0.1/CODE_OF_CONDUCT.md` & `pix_engine-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pix_engine-0.0.1/.devcontainer/devcontainer.json` & `pix_engine-0.1.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pix_engine-0.0.1/pix/pix.py` & `pix_engine-0.1.0/pix/pix.py`

 * *Files identical despite different names*

### Comparing `pix_engine-0.0.1/.gitignore` & `pix_engine-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pix_engine-0.0.1/LICENSE` & `pix_engine-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_engine-0.0.1/pyproject.toml` & `pix_engine-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PIX-engine"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="TVRework", email="boxeigit@gmail.com" },
 ]
 description = "Terminal game engine that is community supported and open source"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pix_engine-0.0.1/PKG-INFO` & `pix_engine-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PIX-engine
-Version: 0.0.1
+Version: 0.1.0
 Summary: Terminal game engine that is community supported and open source
 Project-URL: Homepage, https://github.com/TVRework/PIX
 Project-URL: Bug Tracker, https://github.com/TVRework/PIX/issues
 Author-email: TVRework <boxeigit@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,11 +18,11 @@
 
 PIX is a **python terminal game engine** that is community supported and open source. Develop **games 🎮** _(and applications)_ with **ease.**
 
 ## Installation
 To install PIX, run the following command.
 
 ```
-pip install PIX
+pip install PIX-engine
 ```
 
 **Or,** clone this repoisitory to edit and contribute towards PIX's development and open source.
```

