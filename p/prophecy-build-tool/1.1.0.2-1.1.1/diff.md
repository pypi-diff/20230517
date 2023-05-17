# Comparing `tmp/prophecy-build-tool-1.1.0.2.tar.gz` & `tmp/prophecy-build-tool-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-build-tool-1.1.0.2.tar", last modified: Tue May 16 17:14:23 2023, max compression
+gzip compressed data, was "/home/runner/work/prophecy-build-tool/prophecy-build-tool/dist/.tmp-3as3mteb/prophecy-build-tool-1.1.1.tar", last modified: Wed May 17 09:23:57 2023, max compression
```

## Comparing `prophecy-build-tool-1.1.0.2.tar` & `prophecy-build-tool-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-05-16 17:14:23.760160 prophecy-build-tool-1.1.0.2/
--rw-r--r--   0 kiran      (501) staff       (20)    11357 2022-08-09 06:53:00.000000 prophecy-build-tool-1.1.0.2/LICENSE
--rw-r--r--   0 kiran      (501) staff       (20)     5941 2023-05-16 17:14:23.760244 prophecy-build-tool-1.1.0.2/PKG-INFO
--rw-r--r--   0 kiran      (501) staff       (20)     5318 2023-05-16 14:38:45.000000 prophecy-build-tool-1.1.0.2/README.md
--rw-r--r--   0 kiran      (501) staff       (20)      419 2023-05-16 14:38:45.000000 prophecy-build-tool-1.1.0.2/pyproject.toml
--rw-r--r--   0 kiran      (501) staff       (20)      239 2023-05-16 17:14:23.760534 prophecy-build-tool-1.1.0.2/setup.cfg
--rw-r--r--   0 kiran      (501) staff       (20)     1182 2023-05-16 17:14:09.000000 prophecy-build-tool-1.1.0.2/setup.py
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-05-16 17:14:23.757021 prophecy-build-tool-1.1.0.2/src/
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-05-16 17:14:23.758720 prophecy-build-tool-1.1.0.2/src/pbt/
--rw-r--r--   0 kiran      (501) staff       (20)     2654 2023-05-16 14:38:45.000000 prophecy-build-tool-1.1.0.2/src/pbt/__init__.py
--rw-r--r--   0 kiran      (501) staff       (20)     1941 2023-05-16 14:38:45.000000 prophecy-build-tool-1.1.0.2/src/pbt/process.py
--rw-r--r--   0 kiran      (501) staff       (20)    37577 2023-05-16 17:14:09.000000 prophecy-build-tool-1.1.0.2/src/pbt/prophecy_build_tool.py
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-05-16 17:14:23.759626 prophecy-build-tool-1.1.0.2/src/prophecy_build_tool.egg-info/
--rw-r--r--   0 kiran      (501) staff       (20)     5941 2023-05-16 17:14:23.000000 prophecy-build-tool-1.1.0.2/src/prophecy_build_tool.egg-info/PKG-INFO
--rw-r--r--   0 kiran      (501) staff       (20)      444 2023-05-16 17:14:23.000000 prophecy-build-tool-1.1.0.2/src/prophecy_build_tool.egg-info/SOURCES.txt
--rw-r--r--   0 kiran      (501) staff       (20)        1 2023-05-16 17:14:23.000000 prophecy-build-tool-1.1.0.2/src/prophecy_build_tool.egg-info/dependency_links.txt
--rw-r--r--   0 kiran      (501) staff       (20)       33 2023-05-16 17:14:23.000000 prophecy-build-tool-1.1.0.2/src/prophecy_build_tool.egg-info/entry_points.txt
--rw-r--r--   0 kiran      (501) staff       (20)       77 2023-05-16 17:14:23.000000 prophecy-build-tool-1.1.0.2/src/prophecy_build_tool.egg-info/requires.txt
--rw-r--r--   0 kiran      (501) staff       (20)        4 2023-05-16 17:14:23.000000 prophecy-build-tool-1.1.0.2/src/prophecy_build_tool.egg-info/top_level.txt
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-05-16 17:14:23.760050 prophecy-build-tool-1.1.0.2/test/
--rw-r--r--   0 kiran      (501) staff       (20)     2186 2023-05-16 14:38:45.000000 prophecy-build-tool-1.1.0.2/test/test_build.py
--rw-r--r--   0 kiran      (501) staff       (20)     9225 2023-05-16 17:14:09.000000 prophecy-build-tool-1.1.0.2/test/test_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/pbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/src/pbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/src/pbt/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37709 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/src/pbt/prophecy_build_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:23:57.000000 prophecy-build-tool-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-17 09:19:34.000000 prophecy-build-tool-1.1.1/test/test_deploy.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `prophecy-build-tool-1.1.0.2/LICENSE` & `prophecy-build-tool-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.2/PKG-INFO` & `prophecy-build-tool-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.0.2
+Version: 1.1.1
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.0.2/README.md` & `prophecy-build-tool-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.2/setup.py` & `prophecy-build-tool-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool",
-    version="1.1.0.2",
+    version="1.1.1",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
     "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
@@ -26,14 +26,15 @@
     install_requires=[
         "requests>=2.28.0",
         "PyYAML>=6.0",
         "databricks_cli>=0.17.7",
         "rich>=12.5.1",
         "wheel",
         "build",
+        "pyspark==3.3.0"
     ],
     python_requires=">=3.7",
     entry_points="""
         [console_scripts]
         pbt=pbt:main
     """,
 )
```

### Comparing `prophecy-build-tool-1.1.0.2/src/pbt/__init__.py` & `prophecy-build-tool-1.1.1/src/pbt/__init__.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.2/src/pbt/process.py` & `prophecy-build-tool-1.1.1/src/pbt/process.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.2/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-1.1.1/src/pbt/prophecy_build_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,21 +233,21 @@
         else:
             return overall_build_status, self.pipelines_build_path
 
     def deploy(self, fabric_ids: str = "", skip_builds: bool = False, job_ids=None):
         # not allowed to pass job_id and fabric_ids filter together ( as only job_id support incremental build and
         # deploy), fabric_ids filter builds all pipelines by default and then deploy after filtering
         if job_ids and fabric_ids:
-            print(f"[ERROR]: Can't combine filters, Please pass either --fabric_ids or --job_ids")
+            print("[ERROR]: Can't combine filters, Please pass either --fabric_ids or --job_ids")
             raise Exception()
 
         if job_ids and skip_builds:
             print(
-                f"[ERROR]: Can't skip builds for job_id filter,\nas it only builds depending pipelines ,\nPlease "
-                f"pass either --skip-builds or --job_id filter"
+                "[ERROR]: Can't skip builds for job_id filter,\nas it only builds depending pipelines ,\nPlease "
+                "pass either --skip-builds or --job_id filter"
             )
             raise Exception()
 
         fabric_ids = list(i.strip() for i in fabric_ids.split(r",")) if fabric_ids else list()
         job_ids = list(i.strip() for i in job_ids.split(r",")) if job_ids else list()
 
         if not fabric_ids and not job_ids:
@@ -381,15 +381,18 @@
                                 )
                                 for project in self.dependent_projects.values():
                                     if (
                                         pipeline_id in project.pipelines
                                         and self.project_language == project.project_language
                                     ):
                                         print("    Building dependent project's pipeline:")
-                                        (dependent_build_status, dependent_build_paths,) = project.build(
+                                        (
+                                            dependent_build_status,
+                                            dependent_build_paths,
+                                        ) = project.build(
                                             {
                                                 k: v
                                                 for (k, v) in project.pipelines.items()
                                                 if pipeline_id in project.pipelines
                                             },
                                             False,
                                         )
@@ -792,16 +795,15 @@
 
     @classmethod
     def _error(cls, message: str):
         print("[bold red]ERROR[/bold red]:", message)
         sys.exit(1)
 
     def _setJarsNeededForUT(self, build_jars):
-        import random
-
-        uniqueKey = random.random()
-        jars_unique_key: str = f"driver_library_path_{uniqueKey}"
+        # import random
+        # uniqueKey = random.random()
+        # jars_unique_key: str = f"driver_library_path_{uniqueKey}"
         os.environ["SPARK_JARS_CONFIG"] = build_jars if build_jars else ""
         # return jars_unique_key
 
     def removeJarsKeyFromEnv(self):
         del os.environ["SPARK_JARS_CONFIG"]
```

### Comparing `prophecy-build-tool-1.1.0.2/src/prophecy_build_tool.egg-info/PKG-INFO` & `prophecy-build-tool-1.1.1/src/prophecy_build_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.0.2
+Version: 1.1.1
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.0.2/test/test_build.py` & `prophecy-build-tool-1.1.1/test/test_build.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.2/test/test_deploy.py` & `prophecy-build-tool-1.1.1/test/test_deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,23 +29,28 @@
     result = runner.invoke(deploy, ["--path", PROJECT_PATH_NEW, "--release-version", "1.0", "--project-id", "1"])
     assert "Found 2 jobs: AutomatedPBT-truescala, AutomatedPBTNo-truescala" in result.output
     assert "Found 2 pipelines: AutomatedPBT-truescala (scala), AutomatedPBTNo-truescala \n(scala)" in result.output
     assert "Building pipeline pipelines/AutomatedPBT-truescala" in result.output
     assert "Building pipeline pipelines/AutomatedPBTNo-truescala" in result.output
     assert "Deploying job jobs/AutomatedPBT-truescala" in result.output
     assert "Deploying job jobs/AutomatedPBTNo-truescala" in result.output
-    assert (
-        "Uploading AutomatedPBT-truescala-1.0.jar to \ndbfs:/FileStore/prophecy/artifacts/prophecy/uitesting/1/1.0/pipeline/AutomatedPB\nT-truescala.jar"
-        in result.output
-    )
-    assert (
-        "Uploading AutomatedPBTNo-truescala-1.0.jar to \ndbfs:/FileStore/prophecy/artifacts/prophecy/uitesting/1/1.0/pipeline/AutomatedPB\nTNo-truescala.jar"
-        in result.output
-    )
-    assert "[DONE]: Deployment completed successfully!" in result.output
+
+    # If running with Databricks creds on GitHub Actions
+    if os.environ["DATABRICKS_HOST"] != "test":
+        assert (
+            "Uploading AutomatedPBT-truescala-1.0.jar to "
+            "\ndbfs:/FileStore/prophecy/artifacts/prophecy/uitesting/1/1.0/pipeline/AutomatedPB\nT-truescala.jar"
+            in result.output
+        )
+        assert (
+            "Uploading AutomatedPBTNo-truescala-1.0.jar to "
+            "\ndbfs:/FileStore/prophecy/artifacts/prophecy/uitesting/1/1.0/pipeline/AutomatedPB\nTNo-truescala.jar"
+            in result.output
+        )
+        assert "[DONE]: Deployment completed successfully!" in result.output
 
 
 def test_deploy_path_default_skip_builds():
     runner = CliRunner()
     result = runner.invoke(deploy, ["--path", PROJECT_PATH, "--skip-builds"])
     assert "Found 2 jobs: test-job1234, job-another" in result.output
     assert "[SKIP]: Skipping builds for all pipelines as '--skip-builds' flag is passed." in result.output
```

