# Comparing `tmp/halig-0.3.1.tar.gz` & `tmp/halig-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halig-0.3.1.tar", last modified: Sat May 13 09:13:51 2023, max compression
+gzip compressed data, was "halig-0.3.2.tar", last modified: Wed May 17 17:01:10 2023, max compression
```

## Comparing `halig-0.3.1.tar` & `halig-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0    34670 2023-04-12 19:46:50.194310 halig-0.3.1/LICENSE
--rw-r--r--   0        0        0     1633 2023-05-13 08:52:41.111337 halig-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.3.1/halig/__init__.py
--rw-r--r--   0        0        0       22 2023-05-13 09:12:06.193606 halig-0.3.1/halig/__version__.py
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.3.1/halig/commands/__init__.py
--rw-r--r--   0        0        0      292 2023-04-12 19:47:22.382591 halig-0.3.1/halig/commands/base.py
--rw-r--r--   0        0        0     2781 2023-05-09 06:48:39.717700 halig-0.3.1/halig/commands/edit.py
--rw-r--r--   0        0        0     1076 2023-04-12 19:47:22.382591 halig-0.3.1/halig/commands/notebooks.py
--rw-r--r--   0        0        0     1199 2023-04-12 19:47:22.382591 halig-0.3.1/halig/commands/show.py
--rw-r--r--   0        0        0     1418 2023-05-09 18:17:46.623174 halig-0.3.1/halig/encryption.py
--rw-r--r--   0        0        0     1354 2023-05-08 19:32:21.621775 halig-0.3.1/halig/literals.py
--rw-r--r--   0        0        0     2868 2023-05-08 20:59:47.779605 halig-0.3.1/halig/main.py
--rw-r--r--   0        0        0     3448 2023-05-13 09:05:36.698098 halig-0.3.1/halig/settings.py
--rw-r--r--   0        0        0      733 2023-05-08 21:12:42.122646 halig-0.3.1/halig/utils.py
--rw-r--r--   0        0        0     2728 2023-05-13 09:13:51.309472 halig-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 19:46:50.202310 halig-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 19:47:22.382591 halig-0.3.1/tests/commands/__init__.py
--rw-r--r--   0        0        0     1645 2023-04-24 10:55:32.886664 halig-0.3.1/tests/commands/conftest.py
--rw-r--r--   0        0        0     1168 2023-05-09 17:58:32.738050 halig-0.3.1/tests/commands/test_edit.py
--rw-r--r--   0        0        0     1563 2023-04-24 10:55:32.886664 halig-0.3.1/tests/commands/test_notebooks.py
--rw-r--r--   0        0        0     1141 2023-04-24 10:55:32.886664 halig-0.3.1/tests/commands/test_show.py
--rw-r--r--   0        0        0     2820 2023-04-12 19:47:22.382591 halig-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     2276 2023-05-09 06:28:25.521779 halig-0.3.1/tests/test_encryption.py
--rw-r--r--   0        0        0     1320 2023-05-13 09:11:29.085662 halig-0.3.1/tests/test_settings.py
--rw-r--r--   0        0        0     1482 2023-04-24 10:55:32.886664 halig-0.3.1/tests/test_utils.py
--rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 halig-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34670 2023-04-12 19:46:50.194310 halig-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1633 2023-05-13 08:52:41.111337 halig-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.3.2/halig/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-17 17:00:35.079571 halig-0.3.2/halig/__version__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.3.2/halig/commands/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-12 19:47:22.382591 halig-0.3.2/halig/commands/base.py
+-rw-r--r--   0        0        0     2781 2023-05-09 06:48:39.717700 halig-0.3.2/halig/commands/edit.py
+-rw-r--r--   0        0        0     1397 2023-05-17 09:18:35.363381 halig-0.3.2/halig/commands/import_unencrypted.py
+-rw-r--r--   0        0        0     1076 2023-04-12 19:47:22.382591 halig-0.3.2/halig/commands/notebooks.py
+-rw-r--r--   0        0        0     1199 2023-04-12 19:47:22.382591 halig-0.3.2/halig/commands/show.py
+-rw-r--r--   0        0        0     1418 2023-05-09 18:17:46.623174 halig-0.3.2/halig/encryption.py
+-rw-r--r--   0        0        0     1573 2023-05-13 10:06:04.121116 halig-0.3.2/halig/literals.py
+-rw-r--r--   0        0        0     3757 2023-05-14 19:00:10.001739 halig-0.3.2/halig/main.py
+-rw-r--r--   0        0        0     3420 2023-05-13 10:13:03.572546 halig-0.3.2/halig/settings.py
+-rw-r--r--   0        0        0      733 2023-05-08 21:12:42.122646 halig-0.3.2/halig/utils.py
+-rw-r--r--   0        0        0     2717 2023-05-17 17:01:10.991488 halig-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.202310 halig-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:47:22.382591 halig-0.3.2/tests/commands/__init__.py
+-rw-r--r--   0        0        0     2279 2023-05-14 18:42:09.595033 halig-0.3.2/tests/commands/conftest.py
+-rw-r--r--   0        0        0     1168 2023-05-09 17:58:32.738050 halig-0.3.2/tests/commands/test_edit.py
+-rw-r--r--   0        0        0     1423 2023-05-17 16:53:27.712608 halig-0.3.2/tests/commands/test_import.py
+-rw-r--r--   0        0        0     1563 2023-04-24 10:55:32.886664 halig-0.3.2/tests/commands/test_notebooks.py
+-rw-r--r--   0        0        0     1141 2023-04-24 10:55:32.886664 halig-0.3.2/tests/commands/test_show.py
+-rw-r--r--   0        0        0     2820 2023-04-12 19:47:22.382591 halig-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     2276 2023-05-09 06:28:25.521779 halig-0.3.2/tests/test_encryption.py
+-rw-r--r--   0        0        0     1320 2023-05-13 09:11:29.085662 halig-0.3.2/tests/test_settings.py
+-rw-r--r--   0        0        0     1482 2023-04-24 10:55:32.886664 halig-0.3.2/tests/test_utils.py
+-rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 halig-0.3.2/PKG-INFO
```

### Comparing `halig-0.3.1/LICENSE` & `halig-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/README.md` & `halig-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/halig/commands/edit.py` & `halig-0.3.2/halig/commands/edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/halig/commands/notebooks.py` & `halig-0.3.2/halig/commands/notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/halig/commands/show.py` & `halig-0.3.2/halig/commands/show.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/halig/encryption.py` & `halig-0.3.2/halig/encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/halig/literals.py` & `halig-0.3.2/halig/literals.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # COMMANDS
 COMMANDS_NOTEBOOKS_HELP = "List all notebooks and notes, tree-style"
 COMMANDS_EDIT_HELP = "Edit or add a note into a notebook"
 COMMANDS_SHOW_HELP = "Show a note's contents"
 COMMANDS_VERSION = "Show halig's version"
+COMMANDS_IMPORT_HELP = "Encrypt existing unencrypted files"
 
 # OPTIONS
 OPTION_CONFIG_HELP = "Configuration file. Must be YAML and schema compatible"
 OPTION_LEVEL_HELP = (
     "Tree max recursion level; negative numbers indicate a value of infinity"
 )
-
+OPTION_UNLINK_HELP = """Setting this will remove the original markdown files;
+only the newly encrypted .age files will be preserved. Backup your data first
+"""
 # ARGUMENTS
 ARGUMENT_EDIT_NOTE_HELP = """A valid, settings-relative path.
 Be aware that valid can also mean implicit notes, that is, pointing to a
 current-day note just by its notebook name. For example, if today is
 2023-04-04 and you have a notebook containing a 2023-04-04.age note,
 simply pointing to the notebook's name, e.g. `halig edit notebook` will
 edit the 2023-04-04.age note. Also keep in mind that the note may or may
```

### Comparing `halig-0.3.1/halig/settings.py` & `halig-0.3.2/halig/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,17 +77,15 @@
     class Config:
         env_prefix = "halig_"
 
 
 @lru_cache
 def load_from_file(file_path: Path | None = None) -> Settings:
     if file_path is None:
-        halig_config_home = Path(
-            platformdirs.user_config_dir("halig", ensure_exists=True),
-        )
+        halig_config_home = platformdirs.user_config_path("halig", ensure_exists=True)
         file_path = halig_config_home / "halig.yml"
         file_path.touch(exist_ok=True)
     elif not file_path.exists():
         err = f"File {file_path} does not exist"
         raise FileNotFoundError(err)
 
     with file_path.open("r") as f:
```

### Comparing `halig-0.3.1/halig/utils.py` & `halig-0.3.2/halig/utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/pyproject.toml` & `halig-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Terminals",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-version = "0.3.1"
+version = "0.3.2"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "https://git.roboces.dev/catalin/halig"
 Repository = "https://git.roboces.dev/catalin/halig"
@@ -98,15 +98,14 @@
     "W",
     "C90",
     "I",
     "N",
     "UP",
     "S",
     "BLE",
-    "FBT",
     "B",
     "A",
     "COM",
     "C4",
     "DTZ",
     "T10",
     "EM",
```

### Comparing `halig-0.3.1/tests/commands/conftest.py` & `halig-0.3.2/tests/commands/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,32 @@
     dailies.mkdir()
 
     dt = pendulum.now()
     for day_offset in range(10):
         dt = dt.subtract(days=day_offset)
         (dailies / f"{dt.date()}.age").touch()
 
+@pytest.fixture()
+def unencrypted_notes(notebooks_path):
+    unencrypted_root_path = notebooks_path / "unencrypted"
+    unencrypted_root_path.mkdir()
+    for i in range(5):
+        note = unencrypted_root_path / f"note_{i}.md"
+        note.touch()
+        subnote_path = unencrypted_root_path / f"inner_{i}"
+        subnote_path.mkdir()
+        for j in range(2):
+            subnote = subnote_path / f"note_{i}_{j}.md"
+            subnote.touch()
+            with subnote.open("w") as f:
+                f.write(f"subnote {i} {j}")
+        with note.open("w") as f:
+            f.write(f"note {i}")
+    return unencrypted_root_path
+
 
 @pytest.fixture
 def notebooks_command(settings: Settings):
     return NotebooksCommand(max_depth=float("inf"), settings=settings)
 
 
 @pytest.fixture()
```

### Comparing `halig-0.3.1/tests/commands/test_edit.py` & `halig-0.3.2/tests/commands/test_edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/tests/commands/test_notebooks.py` & `halig-0.3.2/tests/commands/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/tests/commands/test_show.py` & `halig-0.3.2/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/tests/conftest.py` & `halig-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/tests/test_encryption.py` & `halig-0.3.2/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/tests/test_settings.py` & `halig-0.3.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/tests/test_utils.py` & `halig-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.3.1/PKG-INFO` & `halig-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halig
-Version: 0.3.1
+Version: 0.3.2
 Summary: age-encrypted, file-based, note-taking CLI app
 Keywords: cli notes age rage encryption notebook
 Author-Email: cătălin <185504a9@duck.com>
 License: GPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

