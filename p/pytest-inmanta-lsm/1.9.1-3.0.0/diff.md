# Comparing `tmp/pytest-inmanta-lsm-1.9.1.tar.gz` & `tmp/pytest-inmanta-lsm-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-inmanta-lsm-1.9.1.tar", last modified: Fri Sep 16 12:41:25 2022, max compression
+gzip compressed data, was "pytest-inmanta-lsm-3.0.0.tar", last modified: Wed May 17 11:00:03 2023, max compression
```

## Comparing `pytest-inmanta-lsm-1.9.1.tar` & `pytest-inmanta-lsm-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-09-16 12:41:25.636803 pytest-inmanta-lsm-1.9.1/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3431 2022-09-16 12:41:20.000000 pytest-inmanta-lsm-1.9.1/CHANGELOG.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       86 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       12 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11238 2022-09-16 12:41:25.636803 pytest-inmanta-lsm-1.9.1/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10390 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      228 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/pyproject.toml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      610 2022-09-16 12:41:25.636803 pytest-inmanta-lsm-1.9.1/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2339 2022-09-16 12:41:21.000000 pytest-inmanta-lsm-1.9.1/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-09-16 12:41:25.633802 pytest-inmanta-lsm-1.9.1/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-09-16 12:41:25.635802 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      775 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1846 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/exceptions.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2635 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/failed_resources_logs.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    17788 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/managed_service_instance.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10046 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/orchestrator_container.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10559 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/parameters.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    13415 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/plugin.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/py.typed
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    17457 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/remote_orchestrator.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-09-16 12:41:25.636803 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/resources/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      773 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/resources/docker-compose.yml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       25 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/resources/my-env-file
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3444 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/resources/my-server-conf.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3981 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/resources/setup_project.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7974 2022-09-16 12:41:14.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/wait_for_state.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2022-09-16 12:41:25.635802 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11238 2022-09-16 12:41:25.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      962 2022-09-16 12:41:25.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2022-09-16 12:41:25.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       51 2022-09-16 12:41:25.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       32 2022-09-16 12:41:25.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       19 2022-09-16 12:41:25.000000 pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-17 11:00:03.009626 pytest-inmanta-lsm-3.0.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4649 2023-05-17 10:59:56.000000 pytest-inmanta-lsm-3.0.0/CHANGELOG.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       86 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       12 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    13295 2023-05-17 11:00:03.009626 pytest-inmanta-lsm-3.0.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12447 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      228 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      610 2023-05-17 11:00:03.009626 pytest-inmanta-lsm-3.0.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1829 2023-05-17 10:59:56.000000 pytest-inmanta-lsm-3.0.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-17 11:00:03.005625 pytest-inmanta-lsm-3.0.0/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-17 11:00:03.007625 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      775 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1846 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/exceptions.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2635 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/failed_resources_logs.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12283 2023-05-17 10:59:54.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/lsm_project.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18069 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/managed_service_instance.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9637 2023-05-17 10:59:54.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/orchestrator_container.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6797 2023-05-17 10:59:54.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/parameters.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    17753 2023-05-17 10:59:54.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/plugin.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/py.typed
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    31479 2023-05-17 10:59:54.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/remote_orchestrator.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-17 11:00:03.008626 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/resources/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      773 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/resources/docker-compose.yml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       25 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/resources/my-env-file
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3444 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3611 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/resources/setup_project.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7974 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/wait_for_state.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-17 11:00:03.008626 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    13295 2023-05-17 11:00:02.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1091 2023-05-17 11:00:03.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-05-17 11:00:02.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       51 2023-05-17 11:00:02.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       32 2023-05-17 11:00:02.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       19 2023-05-17 11:00:02.000000 pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-05-17 11:00:03.009626 pytest-inmanta-lsm-3.0.0/tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1014 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/tests/test_basic_example.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2516 2023-05-17 10:59:46.000000 pytest-inmanta-lsm-3.0.0/tests/test_containerized_orchestrator.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1892 2023-05-17 10:59:54.000000 pytest-inmanta-lsm-3.0.0/tests/test_partial.py
```

### Comparing `pytest-inmanta-lsm-1.9.1/CHANGELOG.md` & `pytest-inmanta-lsm-3.0.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+# v 3.0.0 (2023-05-17)
+Changes in this release:
+- Fix bug about subprocesses started in the docker container that used the local venv of the composer venv and not the global venv.
+- Update caching mechanism, don't keep project venv in between test session.
+- Halt environment after the full test suite, resume it before each test run. (the environment can be left running using `--lsm-no-halt` option)
+- Don't sync local project's cfcache to the remote orchestrator
+- Sync all (v2) modules installed in editable mode in the local project. (#299)
+- Remove deprecated options (#212)
+
+# v 1.12.0 (2023-04-03)
+Changes in this release:
+- Add option to specify project and environment names
+- Extend LsmProject to mock ServiceEntityBindingV2
+
+# v 1.11.0 (2023-02-20)
+Changes in this release:
+- Make it possible to look back further into the history when reporting on failure
+
+# v 1.10.1 (2023-01-30)
+Changes in this release:
+
+- Fix lsm mocked tests support for iso4.
+
+# v 1.10.0 (2023-01-27)
+Changes in this release:
+
+- Add documentation regarding the structure of the test suite.
+- Install dev version of v2 module dependencies on remote orchestrator when install mode allows for it
+- Import helpers for lsm mocked tests.
+
 # v 1.9.1 (2022-09-16)
 Changes in this release:
 
 - Correctly reset pip environment variables after v2 modules installation on remote orchestrator
 
 
 # v 1.9.0 (2022-09-07)
```

### Comparing `pytest-inmanta-lsm-1.9.1/PKG-INFO` & `pytest-inmanta-lsm-3.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pytest-inmanta-lsm
-Version: 1.9.1
-Summary: Common fixtures for inmanta LSM related modules
-Home-page: https://github.com/inmanta/pytest-inmanta-lsm
-Author: Inmanta
-Author-email: code@inmanta.com
-License: inmanta EULA
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pytest-inmanta-lsm
 
 A pytest plugin to test inmanta modules that use lsm, it is built on top of `pytest-inmanta` and `pytest-inmanta-extensions`
 
 ## Installation
 
 ```bash
@@ -34,16 +11,17 @@
 ## Context
 
 This plugin is used to push code to a remote orchestrator and interact with it, via the LSM north-bound-api
 It requires an LSM enabled orchestrator, with no ssl or authentication enabled, in a default setup and ssh access to the orchestrator machine, with a user that has sudo permissions.
 
 ## Usage
 
-This plugin is built around the remote_orchestrator fixture. 
-It offers features to 
+### First case: using a remote orchestrator
+
+This plugin is built around the remote_orchestrator fixture.
 
 A typical testcase using this plugin looks as follows:
 ```python
 
 def test_full_cycle(project, remote_orchestrator):
     # get connection to remote_orchestrator
     client = remote_orchestrator.client
@@ -82,14 +60,52 @@
         wait_for_state="up",
     )
 
     # break it down
     service_instance.delete()
 
 ```
+
+### Second case: mocking the lsm api
+
+This toolbox comes with one more fixture: `lsm_project`.  This fixture allows to run compile using the lsm model locally.  It has as advantage that:
+ - You get a more fined grained control about what you want to see in your compile (choose the value of attributes, state, version, etc of your service).
+ - If you only care about testing one specific case it is much faster than going through the full lifecycle on the remote orchestrator.
+ - You don't need a running remote orchestrator, so you won't need to synchronize the full project anywhere.
+
+A simple usage would be as follow:
+```python
+def test_model(lsm_project: lsm_project.LsmProject) -> None:
+    # Create a service object, you can modify it as you wish, depending on what you are trying to test
+    service = inmanta_lsm.model.ServiceInstance(
+        id=uuid.uuid4(),
+        environment=lsm_project.environment,
+        service_entity="vlan-assignment",
+        version=1,
+        config={},
+        state="start",
+        candidate_attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
+        active_attributes=None,
+        rollback_attributes=None,
+        created_at=datetime.datetime.now(),
+        last_updated=datetime.datetime.now(),
+        callback=[],
+        deleted=False,
+        deployment_progress=None,
+        service_identity_attribute_value=None,
+    )
+
+    # Add the service to the mocked server.  From now on it will be taken into account
+    # for EACH compile
+    lsm_project.add_service(service)
+
+    # Run a compile, with central focus the service we just created
+    lsm_project.compile("import quickstart", service_id=service.id)
+```
+
 ## Options and environment variables
 
 The following options are available, each with a corresponding environment variable.
 
 
 ```
 pytest-inmanta-lsm:
@@ -169,14 +185,21 @@
                         orchestrator when authentication is enabled. (overrides
                         INMANTA_LSM_TOKEN)
 
 ```
 
 ## Running tests
 
+### How the test suite is structured
+
+The test suite consists of two parts:
+
+* The tests defined in `tests/test_containerized_orchestrator.py` file always run against a container started by the test suite itself.
+* All other tests run against the orchestrator specified by the options passed to the pytest command.
+
 ### Pre-requisites
  Testing (and using) pytest-inmanta-lsm requires:
 - an available orchestrator to test against
 - ssh access to this orchestrator
 
 ### Steps
 1. install dependencies:
@@ -187,20 +210,20 @@
 2. pass the config for pytest-inmanta-lsm via environment variables. e.g.
 ```bash
 export INMANTA_LSM_HOST=<the orchestrator>
 export INMANTA_LSM_USER=<user>
 ```
 
 3. set the repo for inmanta to pull LSM from
- 
+
  ```bash
 export INMANTA_MODULE_REPO=https://USER:LICENSE_TOKEN@modules.inmanta.com/git/inmanta-service-orchestrator/5/{}.git
 ```
 4. run the tests
- 
+
  ```bash
     pytest tests
 ```
 
 ### Deploy a local orchestrator
 
 It is possible to deploy an orchestrator locally and run the tests against it.  The orchestrator will be deployed as a container, using docker.  Here are the prerequisites in order to make it work:
```

### Comparing `pytest-inmanta-lsm-1.9.1/README.md` & `pytest-inmanta-lsm-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pytest-inmanta-lsm
+Version: 3.0.0
+Summary: Common fixtures for inmanta LSM related modules
+Home-page: https://github.com/inmanta/pytest-inmanta-lsm
+Author: Inmanta
+Author-email: code@inmanta.com
+License: inmanta EULA
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pytest-inmanta-lsm
 
 A pytest plugin to test inmanta modules that use lsm, it is built on top of `pytest-inmanta` and `pytest-inmanta-extensions`
 
 ## Installation
 
 ```bash
@@ -11,16 +34,17 @@
 ## Context
 
 This plugin is used to push code to a remote orchestrator and interact with it, via the LSM north-bound-api
 It requires an LSM enabled orchestrator, with no ssl or authentication enabled, in a default setup and ssh access to the orchestrator machine, with a user that has sudo permissions.
 
 ## Usage
 
-This plugin is built around the remote_orchestrator fixture. 
-It offers features to 
+### First case: using a remote orchestrator
+
+This plugin is built around the remote_orchestrator fixture.
 
 A typical testcase using this plugin looks as follows:
 ```python
 
 def test_full_cycle(project, remote_orchestrator):
     # get connection to remote_orchestrator
     client = remote_orchestrator.client
@@ -59,14 +83,52 @@
         wait_for_state="up",
     )
 
     # break it down
     service_instance.delete()
 
 ```
+
+### Second case: mocking the lsm api
+
+This toolbox comes with one more fixture: `lsm_project`.  This fixture allows to run compile using the lsm model locally.  It has as advantage that:
+ - You get a more fined grained control about what you want to see in your compile (choose the value of attributes, state, version, etc of your service).
+ - If you only care about testing one specific case it is much faster than going through the full lifecycle on the remote orchestrator.
+ - You don't need a running remote orchestrator, so you won't need to synchronize the full project anywhere.
+
+A simple usage would be as follow:
+```python
+def test_model(lsm_project: lsm_project.LsmProject) -> None:
+    # Create a service object, you can modify it as you wish, depending on what you are trying to test
+    service = inmanta_lsm.model.ServiceInstance(
+        id=uuid.uuid4(),
+        environment=lsm_project.environment,
+        service_entity="vlan-assignment",
+        version=1,
+        config={},
+        state="start",
+        candidate_attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
+        active_attributes=None,
+        rollback_attributes=None,
+        created_at=datetime.datetime.now(),
+        last_updated=datetime.datetime.now(),
+        callback=[],
+        deleted=False,
+        deployment_progress=None,
+        service_identity_attribute_value=None,
+    )
+
+    # Add the service to the mocked server.  From now on it will be taken into account
+    # for EACH compile
+    lsm_project.add_service(service)
+
+    # Run a compile, with central focus the service we just created
+    lsm_project.compile("import quickstart", service_id=service.id)
+```
+
 ## Options and environment variables
 
 The following options are available, each with a corresponding environment variable.
 
 
 ```
 pytest-inmanta-lsm:
@@ -146,14 +208,21 @@
                         orchestrator when authentication is enabled. (overrides
                         INMANTA_LSM_TOKEN)
 
 ```
 
 ## Running tests
 
+### How the test suite is structured
+
+The test suite consists of two parts:
+
+* The tests defined in `tests/test_containerized_orchestrator.py` file always run against a container started by the test suite itself.
+* All other tests run against the orchestrator specified by the options passed to the pytest command.
+
 ### Pre-requisites
  Testing (and using) pytest-inmanta-lsm requires:
 - an available orchestrator to test against
 - ssh access to this orchestrator
 
 ### Steps
 1. install dependencies:
@@ -164,20 +233,20 @@
 2. pass the config for pytest-inmanta-lsm via environment variables. e.g.
 ```bash
 export INMANTA_LSM_HOST=<the orchestrator>
 export INMANTA_LSM_USER=<user>
 ```
 
 3. set the repo for inmanta to pull LSM from
- 
+
  ```bash
 export INMANTA_MODULE_REPO=https://USER:LICENSE_TOKEN@modules.inmanta.com/git/inmanta-service-orchestrator/5/{}.git
 ```
 4. run the tests
- 
+
  ```bash
     pytest tests
 ```
 
 ### Deploy a local orchestrator
 
 It is possible to deploy an orchestrator locally and run the tests against it.  The orchestrator will be deployed as a container, using docker.  Here are the prerequisites in order to make it work:
```

### Comparing `pytest-inmanta-lsm-1.9.1/setup.cfg` & `pytest-inmanta-lsm-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-1.9.1/setup.py` & `pytest-inmanta-lsm-3.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-    :Copyright: 2022 Inmanta
+    Pytest Inmanta LSM
 
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
-
-    Contact: code@inmanta.com
+    :copyright: 2020 Inmanta
+    :contact: code@inmanta.com
+    :license: Inmanta EULA
 """
 
 import codecs
 import os
 
 from setuptools import setup
 
@@ -27,15 +17,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-inmanta-lsm",
-    version="1.9.1",
+    version="3.0.0",
     python_requires=">=3.6",  # also update classifiers
     author="Inmanta",
     author_email="code@inmanta.com",
     license="inmanta EULA",
     url="https://github.com/inmanta/pytest-inmanta-lsm",
     description="Common fixtures for inmanta LSM related modules",
     long_description=read("README.md"),
@@ -49,15 +39,15 @@
             "resources/my-server-conf.cfg",
             "resources/setup_project.py",
             "py.typed",
         ]
     },
     include_package_data=True,
     install_requires=[
-        "pytest-inmanta~=2.3",
+        "pytest-inmanta~=2.5",
         "inmanta-lsm",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.6",
```

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/__init__.py` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/exceptions.py` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/failed_resources_logs.py` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/failed_resources_logs.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/managed_service_instance.py` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/managed_service_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,26 @@
     DEFAULT_TIMEOUT = 600
 
     def __init__(
         self,
         remote_orchestrator: "r_orchestrator.RemoteOrchestrator",
         service_entity_name: str,
         service_id: Optional[UUID] = None,
+        lookback_depth: int = 1,
     ) -> None:
         """
         :param remote_orchestrator: remote_orchestrator to create the service instance  on
         :param service_entity_name: name of the service entity
         :param service_id: manually choose the id of the service instance
+        :param lookback_depth: the amount of states to search for failures if we detect a bad state
         """
         self.remote_orchestrator = remote_orchestrator
         self.service_entity_name = service_entity_name
         self._instance_id = service_id
+        self._lookback = lookback_depth
 
     @property
     def instance_id(self) -> UUID:
         if self._instance_id is None:
             raise RuntimeError("Instance id is unknown, did you call create already?")
         else:
             return self._instance_id
@@ -353,14 +356,16 @@
 
         def get_bad_state_error(current_state: State) -> FullDiagnosis:
             result = self.remote_orchestrator.client.lsm_services_diagnose(
                 tid=self.remote_orchestrator.environment,
                 service_entity=self.service_entity_name,
                 service_id=self.instance_id,
                 version=current_state.version,
+                rejection_lookbehind=self._lookback - 1,
+                failure_lookbehind=self._lookback,
             )
             assert result.code == 200, (
                 f"Wrong response code while trying to get the service diagnostic, got {result.code} (expected 200):\n"
                 f"{json.dumps(result.result or {}, indent=4)}"
             )
 
             return FullDiagnosis(**result.result["data"])
```

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/orchestrator_container.py` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/orchestrator_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 """
-    :Copyright: 2022 Inmanta
+    Pytest Inmanta LSM
 
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
-
-    Contact: code@inmanta.com
+    :copyright: 2020 Inmanta
+    :contact: code@inmanta.com
+    :license: Inmanta EULA
 """
 import json
 import logging
+import os
 import shutil
 import subprocess
 from configparser import Interpolation
 from ipaddress import IPv4Address
 from pathlib import Path
 from tempfile import mkdtemp
 from textwrap import dedent
@@ -34,22 +25,25 @@
 
 def run_cmd(*, cmd: List[str], cwd: Path) -> Tuple[str, str]:
     """
     Helper function to run command and log the results.  Raises a CalledProcessError
     if the command failed.
     """
     LOGGER.info(f"Running command: {cmd}")
+    env_vars = dict(os.environ)
+    env_vars.pop("PYTHONPATH", None)
     result = subprocess.run(
         args=cmd,
         cwd=str(cwd),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         text=True,
         universal_newlines=True,
+        env=env_vars,
     )
     LOGGER.debug(f"Return code: {result.returncode}")
     LOGGER.debug("Stdout: %s", result.stdout)
     LOGGER.debug("Stderr: %s", result.stderr)
     result.check_returncode()
     return result.stdout, result.stderr
```

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/plugin.py` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 """
 
 import logging
 import os
 import shutil
 import textwrap
 import time
+import uuid
 from typing import Dict, Generator, Iterator, Optional, Tuple, Union
 from uuid import UUID
 
+import pkg_resources
 import pytest
 import pytest_inmanta.plugin
 import requests
 from inmanta import module
-from pytest_inmanta.parameters import inm_mod_in_place
+from packaging import version
 from pytest_inmanta.plugin import Project
-from pytest_inmanta.test_parameter import ParameterNotSetException
+from pytest_inmanta.test_parameter import ParameterNotSetException, StringTestParameter
 
+from pytest_inmanta_lsm import lsm_project
 from pytest_inmanta_lsm.orchestrator_container import (
     DoNotCleanOrchestratorContainer,
     OrchestratorContainer,
 )
 from pytest_inmanta_lsm.parameters import (
     inm_lsm_ca_cert,
     inm_lsm_container_env,
@@ -35,38 +38,65 @@
     inm_lsm_ctr_db_version,
     inm_lsm_ctr_entitlement,
     inm_lsm_ctr_env,
     inm_lsm_ctr_image,
     inm_lsm_ctr_license,
     inm_lsm_ctr_pub_key,
     inm_lsm_env,
+    inm_lsm_env_name,
     inm_lsm_host,
     inm_lsm_no_clean,
+    inm_lsm_no_halt,
     inm_lsm_partial_compile,
+    inm_lsm_project_name,
     inm_lsm_srv_port,
     inm_lsm_ssh_port,
     inm_lsm_ssh_user,
     inm_lsm_ssl,
     inm_lsm_token,
 )
-from pytest_inmanta_lsm.remote_orchestrator import RemoteOrchestrator
+from pytest_inmanta_lsm.remote_orchestrator import (
+    OrchestratorEnvironment,
+    RemoteOrchestrator,
+)
 
 try:
     # make sure that lsm methods are loaded
     from inmanta_lsm import methods  # noqa
 except ImportError:
     # On the first run this is not available yet. However, this import is required because
     # the reset fixture clears the methods on the client. This import ensures that are
     # available.
     pass
 
 
 LOGGER = logging.getLogger(__name__)
 
 
+@pytest.fixture(name="lsm_project")
+def lsm_project_fixture(
+    monkeypatch: pytest.MonkeyPatch,
+    project: pytest_inmanta.plugin.Project,
+    remote_orchestrator_partial: bool,
+) -> "lsm_project.LsmProject":
+    core_version = version.Version(pkg_resources.get_distribution("inmanta-core").version)
+    if core_version < version.Version("6"):
+        # Before inmanta-core==6.0.0, the compile resets the inmanta plugins between each compile, which makes
+        # the monkeypatching of plugins impossible.  This makes this fixture irrelevant in such case.
+        # https://github.com/inmanta/inmanta-core/blob/fd44f3a765e4865cc7179d825fe345fe0540897a/src/inmanta/module.py#L1525
+        pytest.skip(f"The lsm_project fixture is not usable with this version of inmanta-core: {core_version} (< 6)")
+
+    return lsm_project.LsmProject(
+        uuid.uuid4(),
+        project,
+        monkeypatch,
+        partial_compile=remote_orchestrator_partial,
+    )
+
+
 @pytest.fixture(scope="session")
 def remote_orchestrator_container(
     request: pytest.FixtureRequest,
     remote_orchestrator_no_clean: bool,
 ) -> Generator[Optional[OrchestratorContainer], None, None]:
     """
     Deploy, if the user required it, an orchestrator in a container locally.
@@ -92,27 +122,41 @@
 
         if remote_orchestrator_no_clean:
             raise DoNotCleanOrchestratorContainer()
 
 
 @pytest.fixture(scope="session")
 def remote_orchestrator_environment(request: pytest.FixtureRequest) -> str:
+    """
+    Returns the id of the environment on the remote orchestrator that should be used for this
+    test suite.  If the environment doesn't exist, it will be created.
+    """
     return inm_lsm_env.resolve(request.config)
 
 
 @pytest.fixture(scope="session")
 def remote_orchestrator_no_clean(request: pytest.FixtureRequest) -> bool:
     """
     Check if the user specified that the orchestrator shouldn't be cleaned up after a failure.
     Returns True if the orchestrator should be left as is, False otherwise.
     """
     return inm_lsm_no_clean.resolve(request.config)
 
 
 @pytest.fixture(scope="session")
+def remote_orchestrator_no_halt(request: pytest.FixtureRequest) -> bool:
+    """
+    Check if the user specified that the orchestrator shouldn't be halted up after the test suite
+    has finished running.
+    Returns True if the orchestrator should be left running, False otherwise.
+    """
+    return inm_lsm_no_halt.resolve(request.config)
+
+
+@pytest.fixture(scope="session")
 def remote_orchestrator_host(
     remote_orchestrator_container: Optional[OrchestratorContainer],
     request: pytest.FixtureRequest,
 ) -> Tuple[str, int]:
     """
     Resolve the host and port options or take the values from the deployed docker orchestrator.
     Tries to reach the orchestrator 10 times, if it fails, raises a RuntimeError.
@@ -127,15 +171,15 @@
         if remote_orchestrator_container is None
         else (str(remote_orchestrator_container.orchestrator_ips[0]), remote_orchestrator_container.orchestrator_port)
     )
 
     for _ in range(0, 10):
         try:
             http = "https" if inm_lsm_ssl.resolve(request.config) else "http"
-            response = requests.get(f"{http}://{host}:{port}/api/v1/serverstatus", timeout=1, verify=False)
+            response = requests.get(f"{http}://{host}:{port}/api/v1/serverstatus", timeout=2, verify=False)
             response.raise_for_status()
         except Exception as exc:
             LOGGER.warning(str(exc))
             time.sleep(1)
             continue
 
         if response.status_code == 200:
@@ -156,106 +200,197 @@
 
 
 @pytest.fixture(scope="session")
 def remote_orchestrator_partial(request: pytest.FixtureRequest) -> Iterator[bool]:
     yield inm_lsm_partial_compile.resolve(request.config)
 
 
-@pytest.fixture(scope="session")
-def remote_orchestrator_project_shared(request: pytest.FixtureRequest, project_shared: Project) -> Iterator[None]:
+def verify_v2_editable_install() -> None:
     """
-    Shared project to be used by the remote orchestrator. Ensures the module being tested is synced to the remote orchestrator
-    even if it is a v2 module.
+    Verify that if our module is a v2, it is correctly installed, in editable mode.
     """
-    in_place = inm_mod_in_place.resolve(request.config)
-    # no need to do anything if this version of inmanta does not support v2 modules or if in_place already adds it to the path
-    if hasattr(module, "ModuleV2") and not in_place:
-        mod: module.Module
-        path: str
-        mod, _ = pytest_inmanta.plugin.get_module()
-
-        # mod object is constructed from the source dir: it does not contain all installation metadata
-        installed: Optional[module.ModuleV2] = module.ModuleV2Source(urls=[]).get_installed_module(None, mod.name)
-        if isinstance(mod, module.ModuleV1):
-            # no need to do anything for v1 module except raise a warning in some edge scenarios
-            if installed is not None:
-                LOGGER.warning(
-                    "The module being tested is a v1 module but it is also installed as a v2 module. Local compiles will use"
-                    "the v2, but only the v1 will by synced to the server."
-                )
-        else:
-            # put v2 module in libs dir so it will be rsynced to the server
-            if not installed.is_editable() or not os.path.samefile(installed.path, mod.path):
-                LOGGER.warning(
-                    "The module being tested is not installed in editable mode. To ensure the remote orchestrator uses the same"
-                    " code as the local project, please install the module with `inmanta module install -e .` before running"
-                    " the tests."
-                )
-            destination: str = os.path.join(project_shared._test_project_dir, "libs", mod.name)
-            assert not os.path.exists(
-                destination
-            ), "Invalid state: expected clean libs dir, this is most likely an issue with the implementation of this fixture"
-            # can't rsync and install a non-editable Python package the same way as an editable one (no pyproject.toml/setup.py)
-            # => always use the test dir, even if the module is installed in non-editable mode (the user has been warned)
-            shutil.copytree(mod.path, destination)
-    yield
+    mod: module.Module
+    mod, _ = pytest_inmanta.plugin.get_module()
 
+    if isinstance(mod, module.ModuleV1):
+        # Module v1 installed, it can't be badly installed, we exit here.
+        return
 
-@pytest.fixture
-def remote_orchestrator_project(remote_orchestrator_project_shared: None, project: Project) -> Iterator[Project]:
-    """
-    Project to be used by the remote orchestrator. Yields the same object as the plain project fixture but ensures the
-    module being tested is synced to the remote orchestrator even if it is a v2 module.
-    """
-    yield project
+    # mod object is constructed from the source dir: it does not contain all installation metadata
+    installed: Optional[module.ModuleV2] = module.ModuleV2Source(urls=[]).get_installed_module(None, mod.name)
 
+    # Generic message to help fix any of the problems reported below
+    how_to_fix = (
+        "To ensure the remote orchestrator uses the same code as the local project, please install the module"
+        " with `inmanta module install -e .` before running the tests."
+    )
 
-@pytest.fixture
-def remote_orchestrator(
+    if installed is None:
+        # Make sure that the module v2 source can be found, it should always be the case, unless
+        # this fixture is used outside of the context of a module test suite.
+        LOGGER.error("The module being tested is not installed.  %s", how_to_fix)
+    elif not installed.is_editable():
+        # Make sure that the module is installed in editable mode
+        LOGGER.error("The module being tested is not installed in editable mode.  %s", how_to_fix)
+    elif not os.path.samefile(installed.path, mod.path):
+        # Make sure that the source of the module installed in editable mode is the same one
+        # used by pytest-inmanta
+        LOGGER.error(
+            (
+                "%s is installed in editable mode but its path doesn't match the path of the module"
+                " being tested: %s != %s.  %s"
+            ),
+            mod.name,
+            installed.path,
+            mod.path,
+            how_to_fix,
+        )
+    else:
+        # Everything is okay, we exit here
+        return
+
+    # We didn't exit, there was a failure, so we raise an exception
+    raise RuntimeError(f"Module at {mod.path} should be installed in editable mode.  See logs for details.")
+
+
+@pytest.fixture(scope="session")
+def remote_orchestrator_shared(
     request: pytest.FixtureRequest,
-    remote_orchestrator_project: Project,
-    remote_orchestrator_settings: Dict[str, Union[str, int, bool]],
+    project_shared: Project,
     remote_orchestrator_container: Optional[OrchestratorContainer],
     remote_orchestrator_environment: str,
     remote_orchestrator_no_clean: bool,
+    remote_orchestrator_no_halt: bool,
     remote_orchestrator_host: Tuple[str, int],
-    remote_orchestrator_partial: bool,
 ) -> Iterator[RemoteOrchestrator]:
+    """
+    Session fixture to setup the `RemoteOrchestrator` object that will be used to sync our project
+    to the remote orchestrator environment.  This fixture also makes sure that if the module being
+    tested is v2, it is installed in editable mode, as it is required to send it to the remote
+    orchestrator.
+    """
+    # no need to do anything if this version of inmanta does not support v2 modules
+    if hasattr(module, "ModuleV2"):
+        verify_v2_editable_install()
+
     LOGGER.info("Setting up remote orchestrator")
 
     host, port = remote_orchestrator_host
 
     if remote_orchestrator_container is None:
         ssh_user = inm_lsm_ssh_user.resolve(request.config)
-        ssh_port = str(inm_lsm_ssh_port.resolve(request.config))
+        ssh_port = inm_lsm_ssh_port.resolve(request.config)
         container_env = inm_lsm_container_env.resolve(request.config)
     else:
         # If the orchestrator is running in a container we deployed ourself, we overwrite
         # a few configuration parameters with what matches the deployed orchestrator
         # If the container image behaves differently than assume, those value won't work,
         # no mechanism exists currently to work around this.
         ssh_user = "inmanta"
-        ssh_port = "22"
+        ssh_port = 22
         container_env = True
 
     ssl = inm_lsm_ssl.resolve(request.config)
     ca_cert: Optional[str] = None
     if ssl:
         ca_cert = str(inm_lsm_ca_cert.resolve(request.config))
         if (
             remote_orchestrator_container is not None
             and remote_orchestrator_container.compose_file == inm_lsm_ctr_compose.default
         ):
             LOGGER.warning("SSL currently doesn't work with the default docker-compose file.")
 
-    token: Optional[str]
-    try:
-        token = inm_lsm_token.resolve(request.config)
-    except ParameterNotSetException:
-        token = None
+    def get_optional_option(option: StringTestParameter) -> Optional[str]:
+        try:
+            return option.resolve(request.config)
+        except ParameterNotSetException:
+            return None
+
+    token = get_optional_option(inm_lsm_token)
+    environment_name = get_optional_option(inm_lsm_env_name)
+    project_name = get_optional_option(inm_lsm_project_name)
+
+    remote_orchestrator = RemoteOrchestrator(
+        OrchestratorEnvironment(
+            id=UUID(remote_orchestrator_environment),
+            name=environment_name,
+            project=project_name,
+        ),
+        host=host,
+        port=port,
+        ssh_user=ssh_user,
+        ssh_port=ssh_port,
+        ssl=ssl,
+        token=token,
+        ca_cert=ca_cert,
+        container_env=container_env,
+    )
+
+    # Make sure we start our test suite with a clean environment
+    remote_orchestrator.clear_environment()
+
+    # Get the former cached modules back into the project to speed up
+    # subsequent test cases
+    remote_orchestrator.restore_libs_folder()
+
+    yield remote_orchestrator
+
+    # Cache the content of the libs folder for later calls to the orchestrator
+    remote_orchestrator.cache_libs_folder()
+
+    # If --lsm-no-clean is used, leave the orchestrator as it is, with all its
+    # file, otherwise cleanup the project
+    if not remote_orchestrator_no_clean:
+        remote_orchestrator.clear_environment()
+
+    # If --lsm-no-halt is used, leave the orchestrator running at the end of the
+    # test suite.  Otherwise the environment is halted.
+    if not remote_orchestrator_no_halt:
+        remote_orchestrator.client.halt_environment(remote_orchestrator.environment)
+
+
+@pytest.fixture(scope="session")
+def remote_orchestrator_environment_name(remote_orchestrator_shared: RemoteOrchestrator) -> str:
+    """
+    Get the name of the environment in use on the remote orchestrator.  This value can be set
+    using the `--lsm-environment-name` option.
+    """
+    return remote_orchestrator_shared.orchestrator_environment.get_environment(remote_orchestrator_shared.client).name
+
+
+@pytest.fixture(scope="session")
+def remote_orchestrator_project_name(remote_orchestrator_shared: RemoteOrchestrator) -> str:
+    """
+    Get the name of the project the environment on the remote orchestrator is in.  This value can
+    be set using the `--lsm-project-name` option.
+    """
+    return remote_orchestrator_shared.orchestrator_environment.get_project(remote_orchestrator_shared.client).name
+
+
+@pytest.fixture
+def remote_orchestrator_project(remote_orchestrator_shared: RemoteOrchestrator, project: Project) -> Iterator[Project]:
+    """
+    Project to be used by the remote orchestrator. Yields the same object as the plain project fixture but ensures the
+    module being tested is synced to the remote orchestrator even if it is a v2 module.
+    """
+    # Reload the config after the project fixture has run
+    remote_orchestrator_shared.setup_config()
+
+    yield project
+
+
+@pytest.fixture
+def remote_orchestrator(
+    remote_orchestrator_shared: RemoteOrchestrator,
+    remote_orchestrator_project: Project,
+    remote_orchestrator_settings: Dict[str, Union[str, int, bool]],
+    remote_orchestrator_partial: bool,
+) -> RemoteOrchestrator:
+    # Clean environment, but keep project files
+    remote_orchestrator_shared.clear_environment(soft=True)
 
     # set the defaults here and lets the fixture override specific values
     settings: Dict[str, Union[bool, str, int]] = {
         "auto_deploy": True,
         "server_compile": True,
         "agent_trigger_method_on_auto_deploy": "push_incremental_deploy",
         "push_on_auto_deploy": True,
@@ -263,39 +398,26 @@
         "autostart_agent_deploy_interval": 600,
         "autostart_agent_repair_splay_time": 600,
         "autostart_agent_repair_interval": 0,
         "lsm_partial_compile": remote_orchestrator_partial,
     }
     settings.update(remote_orchestrator_settings)
 
-    remote_orchestrator = RemoteOrchestrator(
-        host=host,
-        ssh_user=ssh_user,
-        ssh_port=ssh_port,
-        environment=UUID(remote_orchestrator_environment),
-        project=remote_orchestrator_project,
-        settings=settings,
-        noclean=remote_orchestrator_no_clean,
-        ssl=ssl,
-        token=token,
-        ca_cert=ca_cert,
-        container_env=container_env,
-        port=port,
-    )
-    remote_orchestrator.clean()
+    # Update the settings on the orchestrator
+    for k, v in settings.items():
+        remote_orchestrator_shared.client.set_setting(remote_orchestrator_shared.environment, k, v)
 
-    yield remote_orchestrator
-    remote_orchestrator.pre_clean()
+    # Make sure the environment is running
+    remote_orchestrator_shared.client.resume_environment(remote_orchestrator_shared.environment)
 
-    if not remote_orchestrator_no_clean:
-        remote_orchestrator.clean()
+    return remote_orchestrator_shared
 
 
 @pytest.fixture
-def unittest_lsm(project) -> Iterator[None]:
+def unittest_lsm(project: Project) -> Iterator[None]:
     """
     Adds a module named unittest_lsm to the project with a simple resource that always deploys successfully. The module is
     compatible with the remote orchestrator fixtures.
     """
     name: str = "unittest_lsm"
     project.create_module(
         name,
```

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/resources/docker-compose.yml` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/resources/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/resources/my-server-conf.cfg` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/resources/setup_project.py` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/resources/setup_project.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 """
-    :Copyright: 2022 Inmanta
+    Pytest Inmanta LSM
 
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
-
-    Contact: code@inmanta.com
+    :copyright: 2020 Inmanta
+    :contact: code@inmanta.com
+    :license: Inmanta EULA
 """
 import contextlib
 import logging
 import os
 import pathlib
 import sys
 from collections import abc
@@ -100,14 +90,20 @@
 
 # Install all v2 modules in editable mode using the project's configured package sources
 if v2_modules:
     urls: abc.Sequence[str] = project.module_source.urls
     if not urls:
         raise Exception("No package repos configured for project")
     # plain Python install so core does not apply project's sources -> we need to configure pip index ourselves
-    with env_vars({"PIP_INDEX_URL": urls[0], "PIP_EXTRA_INDEX_URL": " ".join(urls[1:])}):
+    with env_vars(
+        {
+            "PIP_INDEX_URL": urls[0],
+            "PIP_PRE": "0" if project.install_mode == module.InstallMode.release else "1",
+            "PIP_EXTRA_INDEX_URL": " ".join(urls[1:]),
+        }
+    ):
         LOGGER.info(f"Installing modules from source: {[mod.name for mod in v2_modules]}")
         project.virtualenv.install_from_source([env.LocalPackagePath(mod.path, editable=True) for mod in v2_modules])
 
 # Install all other dependencies
 LOGGER.info("Installing other project dependencies")
 project.install_modules()
```

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm/wait_for_state.py` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm/wait_for_state.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/PKG-INFO` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-lsm
-Version: 1.9.1
+Version: 3.0.0
 Summary: Common fixtures for inmanta LSM related modules
 Home-page: https://github.com/inmanta/pytest-inmanta-lsm
 Author: Inmanta
 Author-email: code@inmanta.com
 License: inmanta EULA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -34,16 +34,17 @@
 ## Context
 
 This plugin is used to push code to a remote orchestrator and interact with it, via the LSM north-bound-api
 It requires an LSM enabled orchestrator, with no ssl or authentication enabled, in a default setup and ssh access to the orchestrator machine, with a user that has sudo permissions.
 
 ## Usage
 
-This plugin is built around the remote_orchestrator fixture. 
-It offers features to 
+### First case: using a remote orchestrator
+
+This plugin is built around the remote_orchestrator fixture.
 
 A typical testcase using this plugin looks as follows:
 ```python
 
 def test_full_cycle(project, remote_orchestrator):
     # get connection to remote_orchestrator
     client = remote_orchestrator.client
@@ -82,14 +83,52 @@
         wait_for_state="up",
     )
 
     # break it down
     service_instance.delete()
 
 ```
+
+### Second case: mocking the lsm api
+
+This toolbox comes with one more fixture: `lsm_project`.  This fixture allows to run compile using the lsm model locally.  It has as advantage that:
+ - You get a more fined grained control about what you want to see in your compile (choose the value of attributes, state, version, etc of your service).
+ - If you only care about testing one specific case it is much faster than going through the full lifecycle on the remote orchestrator.
+ - You don't need a running remote orchestrator, so you won't need to synchronize the full project anywhere.
+
+A simple usage would be as follow:
+```python
+def test_model(lsm_project: lsm_project.LsmProject) -> None:
+    # Create a service object, you can modify it as you wish, depending on what you are trying to test
+    service = inmanta_lsm.model.ServiceInstance(
+        id=uuid.uuid4(),
+        environment=lsm_project.environment,
+        service_entity="vlan-assignment",
+        version=1,
+        config={},
+        state="start",
+        candidate_attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
+        active_attributes=None,
+        rollback_attributes=None,
+        created_at=datetime.datetime.now(),
+        last_updated=datetime.datetime.now(),
+        callback=[],
+        deleted=False,
+        deployment_progress=None,
+        service_identity_attribute_value=None,
+    )
+
+    # Add the service to the mocked server.  From now on it will be taken into account
+    # for EACH compile
+    lsm_project.add_service(service)
+
+    # Run a compile, with central focus the service we just created
+    lsm_project.compile("import quickstart", service_id=service.id)
+```
+
 ## Options and environment variables
 
 The following options are available, each with a corresponding environment variable.
 
 
 ```
 pytest-inmanta-lsm:
@@ -169,14 +208,21 @@
                         orchestrator when authentication is enabled. (overrides
                         INMANTA_LSM_TOKEN)
 
 ```
 
 ## Running tests
 
+### How the test suite is structured
+
+The test suite consists of two parts:
+
+* The tests defined in `tests/test_containerized_orchestrator.py` file always run against a container started by the test suite itself.
+* All other tests run against the orchestrator specified by the options passed to the pytest command.
+
 ### Pre-requisites
  Testing (and using) pytest-inmanta-lsm requires:
 - an available orchestrator to test against
 - ssh access to this orchestrator
 
 ### Steps
 1. install dependencies:
@@ -187,20 +233,20 @@
 2. pass the config for pytest-inmanta-lsm via environment variables. e.g.
 ```bash
 export INMANTA_LSM_HOST=<the orchestrator>
 export INMANTA_LSM_USER=<user>
 ```
 
 3. set the repo for inmanta to pull LSM from
- 
+
  ```bash
 export INMANTA_MODULE_REPO=https://USER:LICENSE_TOKEN@modules.inmanta.com/git/inmanta-service-orchestrator/5/{}.git
 ```
 4. run the tests
- 
+
  ```bash
     pytest tests
 ```
 
 ### Deploy a local orchestrator
 
 It is possible to deploy an orchestrator locally and run the tests against it.  The orchestrator will be deployed as a container, using docker.  Here are the prerequisites in order to make it work:
```

### Comparing `pytest-inmanta-lsm-1.9.1/src/pytest_inmanta_lsm.egg-info/SOURCES.txt` & `pytest-inmanta-lsm-3.0.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/pytest_inmanta_lsm/__init__.py
 src/pytest_inmanta_lsm/exceptions.py
 src/pytest_inmanta_lsm/failed_resources_logs.py
+src/pytest_inmanta_lsm/lsm_project.py
 src/pytest_inmanta_lsm/managed_service_instance.py
 src/pytest_inmanta_lsm/orchestrator_container.py
 src/pytest_inmanta_lsm/parameters.py
 src/pytest_inmanta_lsm/plugin.py
 src/pytest_inmanta_lsm/py.typed
 src/pytest_inmanta_lsm/remote_orchestrator.py
 src/pytest_inmanta_lsm/wait_for_state.py
@@ -20,8 +21,11 @@
 src/pytest_inmanta_lsm.egg-info/dependency_links.txt
 src/pytest_inmanta_lsm.egg-info/entry_points.txt
 src/pytest_inmanta_lsm.egg-info/requires.txt
 src/pytest_inmanta_lsm.egg-info/top_level.txt
 src/pytest_inmanta_lsm/resources/docker-compose.yml
 src/pytest_inmanta_lsm/resources/my-env-file
 src/pytest_inmanta_lsm/resources/my-server-conf.cfg
-src/pytest_inmanta_lsm/resources/setup_project.py
+src/pytest_inmanta_lsm/resources/setup_project.py
+tests/test_basic_example.py
+tests/test_containerized_orchestrator.py
+tests/test_partial.py
```

