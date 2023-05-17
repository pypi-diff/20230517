# Comparing `tmp/bitbucket-pipeline-runner-0.3.6.tar.gz` & `tmp/bitbucket_pipeline_runner-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbucket-pipeline-runner-0.3.6.tar", max compression
+gzip compressed data, was "bitbucket_pipeline_runner-0.3.7.tar", max compression
```

## Comparing `bitbucket-pipeline-runner-0.3.6.tar` & `bitbucket_pipeline_runner-0.3.7.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1070 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/LICENSE
--rw-r--r--   0        0        0     1046 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/README.md
--rw-r--r--   0        0        0       29 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/__init__.py
--rw-r--r--   0        0        0       61 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/__main__.py
--rw-r--r--   0        0        0     2943 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/artifacts.py
--rw-r--r--   0        0        0     7623 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/cache.py
--rw-r--r--   0        0        0     4679 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/cli.py
--rw-r--r--   0        0        0     3190 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/config.py
--rw-r--r--   0        0        0    14529 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/container.py
--rw-r--r--   0        0        0     5501 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/context.py
--rw-r--r--   0        0        0    12858 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/models.py
--rw-r--r--   0        0        0      519 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/parse.py
--rw-r--r--   0        0        0     4138 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/repository.py
--rw-r--r--   0        0        0    14367 2022-02-23 21:37:38.262372 bitbucket-pipeline-runner-0.3.6/pipeline_runner/runner.py
--rw-r--r--   0        0        0     8784 2022-02-23 21:37:38.266373 bitbucket-pipeline-runner-0.3.6/pipeline_runner/service.py
--rw-r--r--   0        0        0        0 2022-02-23 21:37:38.266373 bitbucket-pipeline-runner-0.3.6/pipeline_runner/static/__init__.py
--rwxr-xr-x   0        0        0     1521 2022-02-23 21:37:38.266373 bitbucket-pipeline-runner-0.3.6/pipeline_runner/static/dind
--rwxr-xr-x   0        0        0      304 2022-02-23 21:37:38.266373 bitbucket-pipeline-runner-0.3.6/pipeline_runner/static/runit.sh
--rw-r--r--   0        0        0     3389 2022-02-23 21:37:38.266373 bitbucket-pipeline-runner-0.3.6/pipeline_runner/utils.py
--rw-r--r--   0        0        0     1353 2022-02-23 21:37:38.266373 bitbucket-pipeline-runner-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2285 2022-02-23 21:37:52.744713 bitbucket-pipeline-runner-0.3.6/setup.py
--rw-r--r--   0        0        0     2311 2022-02-23 21:37:52.745085 bitbucket-pipeline-runner-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-17 21:36:28.964914 bitbucket_pipeline_runner-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1046 2023-05-17 21:36:28.964914 bitbucket_pipeline_runner-0.3.7/README.md
+-rw-r--r--   0        0        0       29 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/__main__.py
+-rw-r--r--   0        0        0     2943 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/artifacts.py
+-rw-r--r--   0        0        0     7691 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/cache.py
+-rw-r--r--   0        0        0     4725 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/cli.py
+-rw-r--r--   0        0        0     3190 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/config.py
+-rw-r--r--   0        0        0    14535 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/container.py
+-rw-r--r--   0        0        0     5501 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/context.py
+-rw-r--r--   0        0        0    12858 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/models.py
+-rw-r--r--   0        0        0      352 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/parse.py
+-rw-r--r--   0        0        0     4144 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/repository.py
+-rw-r--r--   0        0        0    14318 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/runner.py
+-rw-r--r--   0        0        0     8847 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/service.py
+-rw-r--r--   0        0        0        0 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/static/__init__.py
+-rwxr-xr-x   0        0        0     1521 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/static/dind
+-rwxr-xr-x   0        0        0      304 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/static/runit.sh
+-rw-r--r--   0        0        0     3388 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pipeline_runner/utils.py
+-rw-r--r--   0        0        0     2233 2023-05-17 21:36:28.968914 bitbucket_pipeline_runner-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.3.7/PKG-INFO
```

### Comparing `bitbucket-pipeline-runner-0.3.6/LICENSE` & `bitbucket_pipeline_runner-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbucket-pipeline-runner-0.3.6/README.md` & `bitbucket_pipeline_runner-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/artifacts.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/artifacts.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/cache.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,26 +171,26 @@
 
         logger.info("Cache '%s': Downloading", self._cache_name)
 
         t = ts()
 
         with NamedTemporaryFile(dir=self._cache_directory, delete=False) as f:
             try:
-                logger.debug(f"Downloading cache folder '{src}' to '{f.name}'")
+                logger.debug("Downloading cache folder '%s' to '%s'", src, f.name)
                 data, _ = self._container.get_archive(src)
                 size = 0
                 for chunk in data:
                     size += len(chunk)
                     f.write(chunk)
-            except Exception as e:
-                logger.error(f"Error getting cache from container: {self._cache_name}: {e}")
+            except Exception as e:  # noqa: BLE001: Do not catch blind exception: `Exception`
+                logger.error("Error getting cache from container: %s: %s", self._cache_name, e)
                 os.unlink(f.name)
                 return
             else:
-                logger.debug(f"Moving temp cache archive {f.name} to {dst}")
+                logger.debug("Moving temp cache archive %s to %s", f.name, dst)
                 os.rename(f.name, dst)
 
         t = ts() - t
 
         logger.info("Cache '%s': Downloaded %s in %.3fs", self._cache_name, utils.get_human_readable_size(size), t)
```

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/cli.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,18 +171,21 @@
     print(parsed.json(indent=2))
 
 
 @main.command()
 @click.argument("action", type=click.Choice(["clear", "list"]))
 def cache(action):
     cache_dir = utils.get_cache_directory()
+    if not os.path.isdir(cache_dir):
+        return
+
     projects = sorted(os.listdir(cache_dir))
     if action == "list":
         print("Caches:")
-        print("\n".join(map(lambda i: f"\t{i}", projects)))
+        print("\n".join(f"\t{p}" for p in projects))
     elif action == "clear":
         for p in projects:
             shutil.rmtree(os.path.join(cache_dir, p))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/config.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/config.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/container.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self._name = name
         self._image = image
         self._network_name = network_name
         self._repository_path = repository_path
         self._data_volume_name = data_volume_name
         self._environment = env_vars
         self._logger = output_logger
-        self._mem_limit = mem_limit * 2 ** 20  # MiB to B
+        self._mem_limit = mem_limit * 2**20  # MiB to B
         self._ssh_private_key = ssh_private_key
 
         self._client = docker.from_env()
         self._container = None
 
     def start(self):
         self._start_container()
@@ -274,15 +274,15 @@
             raise Exception(f"Error getting command exit code: {output.decode()}")
 
         str_code = output.decode().strip()
 
         try:
             exit_code = int(str_code)
         except ValueError:
-            raise Exception(f"Invalid exit code: {str_code}")
+            raise Exception(f"Invalid exit code: {str_code}") from None
         else:
             return exit_code
 
     def _add_traces_to_script(self):
         script_lines = map(self._add_trace_to_script_line, self._script)
 
         return '\nprintf "\\n"\n'.join(line for line in script_lines if line)
@@ -329,15 +329,15 @@
             ]
         )
 
     def _upload_to_container(self, scripts: Iterable[Tuple[str, str]]):
         tar_data = io.BytesIO()
 
         with tarfile.open(fileobj=tar_data, mode="w|") as tar:
-            for (name, script) in scripts:
+            for name, script in scripts:
                 ti = tarfile.TarInfo(name)
                 script_data = script.encode()
                 ti.size = len(script_data)
                 ti.mode = 0o644
 
                 tar.addfile(ti, io.BytesIO(script_data))
```

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/context.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/context.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/models.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/models.py`

 * *Files identical despite different names*

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/repository.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         return [
             git_clone_cmd,
             "git reset --hard $BITBUCKET_COMMIT",
             "git config user.name bitbucket-pipelines",
             "git config user.email commits-noreply@bitbucket.org",
             "git config push.default current",
-            # "git config http.${BITBUCKET_GIT_HTTP_ORIGIN}.proxy http://localhost:29418/",
+            # TODO: "git config http.${BITBUCKET_GIT_HTTP_ORIGIN}.proxy http://localhost:29418/",
             f"git remote set-url origin {origin}",
             "git reflog expire --expire=all --all",
             "echo '.bitbucket/pipelines/generated' >> .git/info/exclude",
         ]
 
     @staticmethod
     def _get_origin() -> str:
```

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/runner.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
 
         self._container_name = self._ctx.slug
         self._data_volume_name = f"{self._container_name}-data"
         self._output_logger = utils.get_output_logger(
             self._ctx.pipeline_ctx.get_log_directory(), f"{self._container_name}"
         )
 
-    def run(self) -> Optional[int]:
+    # TODO: Decomplexify
+    def run(self) -> Optional[int]:  # noqa: C901: Too complex (11)
         if not self._should_run():
             logger.info("Skipping step: %s", self._step.name)
             return
 
         logger.info("Running step: %s", self._step.name)
         logger.debug("Step ID: %s", self._ctx.step_uuid)
 
@@ -223,19 +224,15 @@
         if self._ctx.pipeline_ctx.default_image:
             return self._ctx.pipeline_ctx.default_image
 
         return Image(name=config.default_image)
 
     def _create_network(self) -> Network:
         name = f"{self._ctx.pipeline_ctx.project_metadata.slug}-network"
-        network = self._docker_client.networks.create(
-            name,
-            driver="bridge",
-            # options={"com.docker.network.bridge.enable_icc": 'true'}
-        )
+        network = self._docker_client.networks.create(name, driver="bridge")
 
         return network
 
     def _get_step_env_vars(self) -> Dict[str, str]:
         env_vars = self._get_bitbucket_env_vars()
 
         if "docker" in self._step.services:
```

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/service.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-import importlib.resources
 import logging
+from importlib.resources import as_file, files
 from typing import Dict, List
 
 import docker
 from docker import DockerClient
 from docker.models.containers import Container
 from docker.models.volumes import Volume
 from slugify import slugify
 from tenacity import retry, retry_if_exception_type, stop_after_delay, wait_fixed
 
-from . import static
+import pipeline_runner
+
 from .config import config
 from .container import ContainerScriptRunner, pull_image
 from .models import Service
 
 logger = logging.getLogger(__name__)
 
 
-class ServiceNotReadyException(Exception):
+class ServiceNotReadyError(Exception):
     pass
 
 
-class ServiceUnhealthyException(Exception):
+class ServiceUnhealthyError(Exception):
     pass
 
 
 class ServicesManager:
     def __init__(
         self,
         service_names: List[str],
@@ -156,15 +157,15 @@
         logger.info("Removing service: %s", self._service_name)
 
         self._teardown()
 
         self._container.remove(v=True, force=True)
 
     def _get_mem_limit(self) -> int:
-        return self._service.memory * 2 ** 20
+        return self._service.memory * 2**20
 
     def _teardown(self):
         pass
 
 
 class DockerServiceRunner(ServiceRunner):
     def _start_container(self) -> Container:
@@ -187,31 +188,33 @@
                 "start_period": 30_000_000_000,
                 "timeout": 1_000_000_000,
             },
         )
 
         return container
 
-    @retry(wait=wait_fixed(1), stop=stop_after_delay(30), retry=retry_if_exception_type(ServiceNotReadyException))
+    @retry(wait=wait_fixed(1), stop=stop_after_delay(30), retry=retry_if_exception_type(ServiceNotReadyError))
     def _ensure_container_ready(self, container: Container):
         # Refresh container to ensure we have its health status
         container = self._client.containers.get(container.name)
         health = container.attrs["State"]["Health"]["Status"]
         if health == "healthy":
             return
         elif health == "unhealthy":
-            raise ServiceUnhealthyException()
+            raise ServiceUnhealthyError()
         else:
-            raise ServiceNotReadyException()
+            raise ServiceNotReadyError()
 
     def _get_volumes(self) -> Dict[str, Dict[str, str]]:
-        with importlib.resources.path(static, "dind") as p:
+        static_files = files(pipeline_runner).joinpath("static")
+
+        with as_file(static_files.joinpath("dind")) as p:
             dind_script_path = p
 
-        with importlib.resources.path(static, "runit.sh") as p:
+        with as_file(static_files.joinpath("runit.sh")) as p:
             runit_script_path = p
 
         cache_volume = self._get_cache_volume()
 
         return {
             cache_volume.name: {"bind": "/var/lib/docker"},
             self._shared_data_volume_name: {"bind": config.remote_pipeline_dir},
```

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/static/dind` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/static/dind`

 * *Files identical despite different names*

### Comparing `bitbucket-pipeline-runner-0.3.6/pipeline_runner/utils.py` & `bitbucket_pipeline_runner-0.3.7/pipeline_runner/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,22 +62,21 @@
         value = sep.join(value)
 
     return value
 
 
 def escape_shell_string(value: str) -> str:
     for c in "\\$%{}\"'":
-        value = value.replace(c, fr"\x{ord(c):02x}")
+        value = value.replace(c, rf"\x{ord(c):02x}")
 
     return value
 
 
 def get_human_readable_size(num):
     for unit in ["B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB"]:
-
         if abs(num) < 1024.0:
             return f"{num:3.1f}{unit}"
 
         num /= 1024.0
 
     return f"{num:.1f}{unit}"
```

### Comparing `bitbucket-pipeline-runner-0.3.6/PKG-INFO` & `bitbucket_pipeline_runner-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipeline-runner
-Version: 0.3.6
+Version: 0.3.7
 Summary: Run a bitbucket pipeline locally
 Home-page: https://github.com/mathieu-lemay/pipeline-runner
 License: MIT
 Author: Mathieu Lemay
 Author-email: acidrain1@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.12,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: boto3 (>=1.16.63,<2.0.0)
+Requires-Dist: boto3 (==1.26.135)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0,<16.0)
-Requires-Dist: cryptography (>=36.0.1,<37.0.0)
-Requires-Dist: docker (>=5.0.2,<6.0.0)
+Requires-Dist: cryptography (>=40.0.2,<41.0.0)
+Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pyfzf (>=0.3.0,<0.4.0)
-Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
-Requires-Dist: python-slugify (>=5.0.2,<6.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: python-slugify (>=8.0.0,<9.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/mathieu-lemay/pipeline-runner
 Description-Content-Type: text/markdown
 
 # Bitbucket Pipeline Runner
```

