# Comparing `tmp/pytest_kubernetes-0.2.0.tar.gz` & `tmp/pytest_kubernetes-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_kubernetes-0.2.0.tar", max compression
+gzip compressed data, was "pytest_kubernetes-0.3.0.tar", max compression
```

## Comparing `pytest_kubernetes-0.2.0.tar` & `pytest_kubernetes-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11356 2023-02-15 15:06:55.179537 pytest_kubernetes-0.2.0/LICENSE
--rw-r--r--   0        0        0     5555 2023-02-16 17:12:32.767922 pytest_kubernetes-0.2.0/README.md
--rw-r--r--   0        0        0     1000 2023-02-16 17:26:59.566810 pytest_kubernetes-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-09 16:16:38.627354 pytest_kubernetes-0.2.0/pytest_kubernetes/__init__.py
--rw-r--r--   0        0        0     2421 2023-02-16 17:25:36.938532 pytest_kubernetes-0.2.0/pytest_kubernetes/kubectl.py
--rw-r--r--   0        0        0      289 2023-02-15 09:21:50.826410 pytest_kubernetes-0.2.0/pytest_kubernetes/options.py
--rw-r--r--   0        0        0     2086 2023-02-15 13:53:56.197935 pytest_kubernetes-0.2.0/pytest_kubernetes/plugin.py
--rw-r--r--   0        0        0     3366 2023-02-16 17:26:51.086782 pytest_kubernetes-0.2.0/pytest_kubernetes/portforwarding.py
--rw-r--r--   0        0        0     1199 2023-02-15 13:51:40.626278 pytest_kubernetes-0.2.0/pytest_kubernetes/providers/__init__.py
--rw-r--r--   0        0        0     7182 2023-02-16 17:25:27.142499 pytest_kubernetes-0.2.0/pytest_kubernetes/providers/base.py
--rw-r--r--   0        0        0     1233 2023-02-15 09:19:11.110397 pytest_kubernetes-0.2.0/pytest_kubernetes/providers/k3d.py
--rw-r--r--   0        0        0      898 2023-02-15 09:19:21.538398 pytest_kubernetes-0.2.0/pytest_kubernetes/providers/kind.py
--rw-r--r--   0        0        0     1490 2023-02-15 13:50:17.734516 pytest_kubernetes-0.2.0/pytest_kubernetes/providers/minikube.py
--rw-r--r--   0        0        0     6468 1970-01-01 00:00:00.000000 pytest_kubernetes-0.2.0/setup.py
--rw-r--r--   0        0        0     6270 1970-01-01 00:00:00.000000 pytest_kubernetes-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-14 07:02:49.886399 pytest_kubernetes-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6013 2023-05-17 06:57:49.064102 pytest_kubernetes-0.3.0/README.md
+-rw-r--r--   0        0        0     1061 2023-05-17 06:57:49.064102 pytest_kubernetes-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 07:02:49.886399 pytest_kubernetes-0.3.0/pytest_kubernetes/__init__.py
+-rw-r--r--   0        0        0     2421 2023-04-14 07:02:49.886399 pytest_kubernetes-0.3.0/pytest_kubernetes/kubectl.py
+-rw-r--r--   0        0        0      289 2023-05-17 06:57:49.064102 pytest_kubernetes-0.3.0/pytest_kubernetes/options.py
+-rw-r--r--   0        0        0     2086 2023-04-14 07:02:49.886399 pytest_kubernetes-0.3.0/pytest_kubernetes/plugin.py
+-rw-r--r--   0        0        0     3366 2023-04-14 07:02:49.886399 pytest_kubernetes-0.3.0/pytest_kubernetes/portforwarding.py
+-rw-r--r--   0        0        0     1199 2023-04-14 07:02:49.886399 pytest_kubernetes-0.3.0/pytest_kubernetes/providers/__init__.py
+-rw-r--r--   0        0        0     7239 2023-05-17 06:57:49.064102 pytest_kubernetes-0.3.0/pytest_kubernetes/providers/base.py
+-rw-r--r--   0        0        0     1293 2023-05-17 06:57:49.064102 pytest_kubernetes-0.3.0/pytest_kubernetes/providers/k3d.py
+-rw-r--r--   0        0        0      946 2023-05-17 06:57:49.064102 pytest_kubernetes-0.3.0/pytest_kubernetes/providers/kind.py
+-rw-r--r--   0        0        0     1586 2023-05-17 06:57:49.064102 pytest_kubernetes-0.3.0/pytest_kubernetes/providers/minikube.py
+-rw-r--r--   0        0        0     6856 1970-01-01 00:00:00.000000 pytest_kubernetes-0.3.0/PKG-INFO
```

### Comparing `pytest_kubernetes-0.2.0/LICENSE` & `pytest_kubernetes-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_kubernetes-0.2.0/README.md` & `pytest_kubernetes-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 - `kubectl(...)`: Execute kubectl command against this cluster (defaults to `dict` as returning format)
 - `apply(...)`: Apply resources to this cluster, either from YAML file, or Python dict
 - `load_image(...)`: Load a container image into this cluster
 - `wait(...)`: Wait for a target and a condition
 - `port_forwarding(...)`: Port forward a target
 - `logs(...)`: Get the logs of a pod
 - `version()`: Get the Kubernetes version of this cluster
-- `create(...)`: Create this cluster
+- `create(...)`: Create this cluster (pass special cluster arguments with `options: List[str]` to the CLI command)
 - `delete()`: Delete this cluster
 - `reset()`: Delete this cluster (if it exists) and create it again
 
 The interface provides proper typing and should be easy to work with.
 
 **Example**
 
@@ -124,9 +124,17 @@
     yield cluster
     cluster.delete()
 ```
 In this example, the cluster remains active for the entire session and is only deleted once pytest is done.
 
 > Note that `yield` notation that is prefered by pytest to express clean up tasks for this fixture.
 
+#### Special cluster options
+You can pass more options using `kwargs['options']: List[str]` to the `create(options=...)` function when creating the cluster like so:
+```python
+    cluster = select_provider_manager("k3d")("my-cluster")
+    # bind ports of this k3d cluster
+    cluster.create(options=["--agents", "1", "-p", "8080:80@agent:0", "-p", "31820:31820/UDP@agent:0"])
+```
+
 ## Examples
 Please find more examples in *tests/vendor.py* in this repository. These test cases are written as users of pytest-kubernetes would write test cases in their projects.
```

### Comparing `pytest_kubernetes-0.2.0/pyproject.toml` & `pytest_kubernetes-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "pytest-kubernetes"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Michael Schilonka <michael@blueshoe.io>"]
 readme = "README.md"
 packages = [{include = "pytest_kubernetes"}]
+repository = "https://github.com/Blueshoe/pytest-kubernetes"
 classifiers = [
     "Framework :: Pytest",
     "Topic :: Software Development :: Testing",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
```

### Comparing `pytest_kubernetes-0.2.0/pytest_kubernetes/kubectl.py` & `pytest_kubernetes-0.3.0/pytest_kubernetes/kubectl.py`

 * *Files identical despite different names*

### Comparing `pytest_kubernetes-0.2.0/pytest_kubernetes/plugin.py` & `pytest_kubernetes-0.3.0/pytest_kubernetes/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_kubernetes-0.2.0/pytest_kubernetes/portforwarding.py` & `pytest_kubernetes-0.3.0/pytest_kubernetes/portforwarding.py`

 * *Files identical despite different names*

### Comparing `pytest_kubernetes-0.2.0/pytest_kubernetes/providers/__init__.py` & `pytest_kubernetes-0.3.0/pytest_kubernetes/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_kubernetes-0.2.0/pytest_kubernetes/providers/base.py` & `pytest_kubernetes-0.3.0/pytest_kubernetes/providers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,13 +219,14 @@
             raise RuntimeError(f"Cluster '{self.cluster_name}' is not ready")
 
     def delete(self) -> None:
         """Delete this cluster"""
         self._on_delete()
         if self.kubeconfig:
             self.kubeconfig.unlink(missing_ok=True)
+            self._cluster_options.kubeconfig_path = None
         sleep(1)
 
     def reset(self) -> None:
         """Reset this cluster (delete if exists and recreates)"""
         self.delete()
         self.create()
```

### Comparing `pytest_kubernetes-0.2.0/pytest_kubernetes/providers/k3d.py` & `pytest_kubernetes-0.3.0/pytest_kubernetes/providers/k3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,27 @@
     def get_binary_name(self) -> str:
         return "k3d"
 
     def _translate_version(self, version: str) -> str:
         return f"rancher/k3s:v{version}-k3s1"
 
     def _on_create(self, cluster_options: ClusterOptions, **kwargs) -> None:
+        opts = kwargs.get("options", [])
         self._exec(
             [
                 "cluster",
                 "create",
                 self.cluster_name,
                 "--kubeconfig-update-default=0",
                 "--image",
                 self._translate_version(cluster_options.api_version),
                 "--wait",
                 f"--timeout={cluster_options.cluster_timeout}s",
             ]
+            + opts
         )
         self._exec(
             [
                 "kubeconfig",
                 "get",
                 self.cluster_name,
                 ">",
```

### Comparing `pytest_kubernetes-0.2.0/pytest_kubernetes/providers/kind.py` & `pytest_kubernetes-0.3.0/pytest_kubernetes/providers/kind.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 
 class KindManager(AClusterManager):
     @classmethod
     def get_binary_name(self) -> str:
         return "kind"
 
     def _on_create(self, cluster_options: ClusterOptions, **kwargs) -> None:
+        opts = kwargs.get("options", [])
         _ = self._exec(
             [
                 "create",
                 "cluster",
                 "--name",
                 self.cluster_name,
                 "--kubeconfig",
                 str(cluster_options.kubeconfig_path),
                 "--image",
                 f"kindest/node:v{cluster_options.api_version}",
-            ]
+            ] + opts
         )
 
     def _on_delete(self) -> None:
         _ = self._exec(["delete", "cluster", "--name", self.cluster_name])
 
     def load_image(self, image: str) -> None:
         self._exec(["load", "docker-image", image, "--name", self.cluster_name])
```

### Comparing `pytest_kubernetes-0.2.0/pytest_kubernetes/providers/minikube.py` & `pytest_kubernetes-0.3.0/pytest_kubernetes/providers/minikube.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,37 +12,39 @@
 
     def load_image(self, image: str) -> None:
         self._exec(["image", "load", image, "-p", self.cluster_name])
 
 
 class MinikubeKVM2Manager(MinikubeManager):
     def _on_create(self, cluster_options: ClusterOptions, **kwargs) -> None:
+        opts = kwargs.get("options", [])
         self._exec(
             [
                 "start",
                 "-p",
                 self.cluster_name,
                 "--driver",
                 "kvm2",
                 "--embed-certs",
                 "--kubernetes-version",
                 f"v{cluster_options.api_version}",
-            ],
+            ] + opts,
             additional_env={"KUBECONFIG": str(cluster_options.kubeconfig_path)},
         )
 
 
 class MinikubeDockerManager(MinikubeManager):
     def _on_create(self, cluster_options: ClusterOptions, **kwargs) -> None:
+        opts = kwargs.get("options", [])
         self._exec(
             [
                 "start",
                 "-p",
                 self.cluster_name,
                 "--driver",
                 "docker",
                 "--embed-certs",
                 "--kubernetes-version",
                 f"v{cluster_options.api_version}",
-            ],
+            ] + opts,
             additional_env={"KUBECONFIG": str(cluster_options.kubeconfig_path)},
         )
```

### Comparing `pytest_kubernetes-0.2.0/setup.py` & `pytest_kubernetes-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,162 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-kubernetes
+Version: 0.3.0
+Summary: 
+Home-page: https://github.com/Blueshoe/pytest-kubernetes
+Author: Michael Schilonka
+Author-email: michael@blueshoe.io
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Framework :: Pytest
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: pytest (>=7.2.1,<8.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Repository, https://github.com/Blueshoe/pytest-kubernetes
+Description-Content-Type: text/markdown
+
+# pytest-kubernetes
+pytest-kubernetes is a lightweight pytest plugin that makes managing (local) Kubernetes clusters a breeze. You can easily spin up a Kubernetes cluster with one [pytest fixure](https://docs.pytest.org/en/latest/explanation/fixtures.html) and remove them again.
+The fixture comes with some simple functions to interact with the cluster, for example `kubectl(...)` that allows you to run typical *kubectl* commands against this cluster without worring 
+about the *kubeconfig* on the test machine.
+
+**Features:**
+- Set up and tear down (local) Kubernetes clusters with *minikube*, *k3d* and *kind*
+- Configure the cluster to recreate for each test case (default), or keep it across multiple test cases
+- Automatic management of the *kubeconfig*
+- Simple functions to run kubectl commands (with *dict* output), reading logs and load custom container images
+- Wait for certain conditions in the cluster
+- Port forward Kubernetes-based services (using kubectl port-forward) easily during a test case
+- Management utils for custom pytest-fixtures (for example pre-provisioned clusters)
+ 
+## Installation
+This plugin can be installed from PyPI:
+- `pip install pytest-kubernetes`
+- `poetry add -D pytest-kubernetes`
+
+Note that this package provides entrypoint hooks to be automatically loaded with pytest.
+
+## Requirements
+pytest-kubernetes expects the following components to be available on the test machine:
+- [`kubectl`](https://kubernetes.io/docs/reference/kubectl/)
+- [`minikube`](https://minikube.sigs.k8s.io/docs/start/) (optional for minikube-based clusters)
+- [`k3d`](https://k3d.io/) (optional for k3d-based clusters)
+- [`kind`](https://kind.sigs.k8s.io/) (optional for kind-based clusters)
+- [Docker](https://docs.docker.com/get-docker/) (optional for Docker-based Kubernetes clusters)
+
+Please make sure they are installed to run pytest-kubernetes properly.
+
+## Reference
+
+### Fixture
+
+#### k8s
+The _k8s_ fixture provides access to an automatically selected Kubernetes provider (depending on the availability on the host). The priority is: k3d, kind, minikube-docker and minikube-kvm2.
+
+The fixture passes a manager object of type *AClusterManager*.
+
+It provides the following interface:
+- `kubectl(...)`: Execute kubectl command against this cluster (defaults to `dict` as returning format)
+- `apply(...)`: Apply resources to this cluster, either from YAML file, or Python dict
+- `load_image(...)`: Load a container image into this cluster
+- `wait(...)`: Wait for a target and a condition
+- `port_forwarding(...)`: Port forward a target
+- `logs(...)`: Get the logs of a pod
+- `version()`: Get the Kubernetes version of this cluster
+- `create(...)`: Create this cluster (pass special cluster arguments with `options: List[str]` to the CLI command)
+- `delete()`: Delete this cluster
+- `reset()`: Delete this cluster (if it exists) and create it again
+
+The interface provides proper typing and should be easy to work with.
+
+**Example**
+
+```python
+def test_a_feature_with_k3d(k8s: AClusterManager):
+    k8s.create()
+    k8s.apply(
+        {
+            "apiVersion": "v1",
+            "kind": "ConfigMap",
+            "data": {"key": "value"},
+            "metadata": {"name": "myconfigmap"},
+        },
+    )
+    k8s.apply("./dependencies.yaml")
+    k8s.load_image("my-container-image:latest")
+    k8s.kubectl(
+        [
+            "run",
+            "test",
+            "--image",
+            "my-container-image:latest",
+            "--restart=Never",
+            "--image-pull-policy=Never",
+        ]
+    )
+```
+This cluster will be deleted once the test case is over.
+
+> Please note that you need to set *"--image-pull-policy=Never"* for images that you loaded into the cluster via the `k8s.load(name: str)` function (see example above).
+
+### Marks
+pytest-kubernetes uses [*pytest marks*](https://docs.pytest.org/en/7.1.x/how-to/mark.html) for specifying the cluster configuration for a test case
+
+Currently the following settings are supported:
+
+- *provider* (str): request a specific Kubernetes provider for the test case 
+- *cluster_name* (str): request a specific cluster name
+- *keep* (bool): keep the cluster across multiple test cases
+
+
+**Example**
+```python
+@pytest.mark.k8s(provider="minikube", cluster_name="test1", keep=True)
+def test_a_feature_in_minikube(k8s: AClusterManager):
+    ...
+```
+
+### Utils
+To write custom Kubernetes-based fixtures in your project you can make use of the following util functions.
+
+
+#### `select_provider_manager`
+This function returns a deriving class of *AClusterManager* that is not created and wrapped in a fixture yet.
+
+`select_provider_manager(name: Optional[str] = None) -> Type[AClusterManager]`
+
+The returning object gets called with the init parameters of *AClusterManager*, the `cluster_name: str`.
+
+**Example**
+```python
+@pytest.fixture(scope="session")
+def k8s_with_workload(request):
+    cluster = select_provider_manager("k3d")("my-cluster")
+    # if minikube should be used
+    # cluster = select_provider_manager("minikube")("my-cluster")
+    cluster.create()
+    # init the cluster with a workload
+    cluster.apply("./fixtures/hello.yaml")
+    cluster.wait("deployments/hello-nginxdemo", "condition=Available=True")
+    yield cluster
+    cluster.delete()
+```
+In this example, the cluster remains active for the entire session and is only deleted once pytest is done.
+
+> Note that `yield` notation that is prefered by pytest to express clean up tasks for this fixture.
+
+#### Special cluster options
+You can pass more options using `kwargs['options']: List[str]` to the `create(options=...)` function when creating the cluster like so:
+```python
+    cluster = select_provider_manager("k3d")("my-cluster")
+    # bind ports of this k3d cluster
+    cluster.create(options=["--agents", "1", "-p", "8080:80@agent:0", "-p", "31820:31820/UDP@agent:0"])
+```
 
-packages = \
-['pytest_kubernetes', 'pytest_kubernetes.providers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pytest>=7.2.1,<8.0.0', 'pyyaml>=6.0,<7.0']
-
-entry_points = \
-{'pytest11': ['pytest-kubernetes = pytest_kubernetes.plugin']}
-
-setup_kwargs = {
-    'name': 'pytest-kubernetes',
-    'version': '0.2.0',
-    'description': '',
-    'long_description': '# pytest-kubernetes\npytest-kubernetes is a lightweight pytest plugin that makes managing (local) Kubernetes clusters a breeze. You can easily spin up a Kubernetes cluster with one [pytest fixure](https://docs.pytest.org/en/latest/explanation/fixtures.html) and remove them again.\nThe fixture comes with some simple functions to interact with the cluster, for example `kubectl(...)` that allows you to run typical *kubectl* commands against this cluster without worring \nabout the *kubeconfig* on the test machine.\n\n**Features:**\n- Set up and tear down (local) Kubernetes clusters with *minikube*, *k3d* and *kind*\n- Configure the cluster to recreate for each test case (default), or keep it across multiple test cases\n- Automatic management of the *kubeconfig*\n- Simple functions to run kubectl commands (with *dict* output), reading logs and load custom container images\n- Wait for certain conditions in the cluster\n- Port forward Kubernetes-based services (using kubectl port-forward) easily during a test case\n- Management utils for custom pytest-fixtures (for example pre-provisioned clusters)\n \n## Installation\nThis plugin can be installed from PyPI:\n- `pip install pytest-kubernetes`\n- `poetry add -D pytest-kubernetes`\n\nNote that this package provides entrypoint hooks to be automatically loaded with pytest.\n\n## Requirements\npytest-kubernetes expects the following components to be available on the test machine:\n- [`kubectl`](https://kubernetes.io/docs/reference/kubectl/)\n- [`minikube`](https://minikube.sigs.k8s.io/docs/start/) (optional for minikube-based clusters)\n- [`k3d`](https://k3d.io/) (optional for k3d-based clusters)\n- [`kind`](https://kind.sigs.k8s.io/) (optional for kind-based clusters)\n- [Docker](https://docs.docker.com/get-docker/) (optional for Docker-based Kubernetes clusters)\n\nPlease make sure they are installed to run pytest-kubernetes properly.\n\n## Reference\n\n### Fixture\n\n#### k8s\nThe _k8s_ fixture provides access to an automatically selected Kubernetes provider (depending on the availability on the host). The priority is: k3d, kind, minikube-docker and minikube-kvm2.\n\nThe fixture passes a manager object of type *AClusterManager*.\n\nIt provides the following interface:\n- `kubectl(...)`: Execute kubectl command against this cluster (defaults to `dict` as returning format)\n- `apply(...)`: Apply resources to this cluster, either from YAML file, or Python dict\n- `load_image(...)`: Load a container image into this cluster\n- `wait(...)`: Wait for a target and a condition\n- `port_forwarding(...)`: Port forward a target\n- `logs(...)`: Get the logs of a pod\n- `version()`: Get the Kubernetes version of this cluster\n- `create(...)`: Create this cluster\n- `delete()`: Delete this cluster\n- `reset()`: Delete this cluster (if it exists) and create it again\n\nThe interface provides proper typing and should be easy to work with.\n\n**Example**\n\n```python\ndef test_a_feature_with_k3d(k8s: AClusterManager):\n    k8s.create()\n    k8s.apply(\n        {\n            "apiVersion": "v1",\n            "kind": "ConfigMap",\n            "data": {"key": "value"},\n            "metadata": {"name": "myconfigmap"},\n        },\n    )\n    k8s.apply("./dependencies.yaml")\n    k8s.load_image("my-container-image:latest")\n    k8s.kubectl(\n        [\n            "run",\n            "test",\n            "--image",\n            "my-container-image:latest",\n            "--restart=Never",\n            "--image-pull-policy=Never",\n        ]\n    )\n```\nThis cluster will be deleted once the test case is over.\n\n> Please note that you need to set *"--image-pull-policy=Never"* for images that you loaded into the cluster via the `k8s.load(name: str)` function (see example above).\n\n### Marks\npytest-kubernetes uses [*pytest marks*](https://docs.pytest.org/en/7.1.x/how-to/mark.html) for specifying the cluster configuration for a test case\n\nCurrently the following settings are supported:\n\n- *provider* (str): request a specific Kubernetes provider for the test case \n- *cluster_name* (str): request a specific cluster name\n- *keep* (bool): keep the cluster across multiple test cases\n\n\n**Example**\n```python\n@pytest.mark.k8s(provider="minikube", cluster_name="test1", keep=True)\ndef test_a_feature_in_minikube(k8s: AClusterManager):\n    ...\n```\n\n### Utils\nTo write custom Kubernetes-based fixtures in your project you can make use of the following util functions.\n\n\n#### `select_provider_manager`\nThis function returns a deriving class of *AClusterManager* that is not created and wrapped in a fixture yet.\n\n`select_provider_manager(name: Optional[str] = None) -> Type[AClusterManager]`\n\nThe returning object gets called with the init parameters of *AClusterManager*, the `cluster_name: str`.\n\n**Example**\n```python\n@pytest.fixture(scope="session")\ndef k8s_with_workload(request):\n    cluster = select_provider_manager("k3d")("my-cluster")\n    # if minikube should be used\n    # cluster = select_provider_manager("minikube")("my-cluster")\n    cluster.create()\n    # init the cluster with a workload\n    cluster.apply("./fixtures/hello.yaml")\n    cluster.wait("deployments/hello-nginxdemo", "condition=Available=True")\n    yield cluster\n    cluster.delete()\n```\nIn this example, the cluster remains active for the entire session and is only deleted once pytest is done.\n\n> Note that `yield` notation that is prefered by pytest to express clean up tasks for this fixture.\n\n## Examples\nPlease find more examples in *tests/vendor.py* in this repository. These test cases are written as users of pytest-kubernetes would write test cases in their projects.',
-    'author': 'Michael Schilonka',
-    'author_email': 'michael@blueshoe.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
+## Examples
+Please find more examples in *tests/vendor.py* in this repository. These test cases are written as users of pytest-kubernetes would write test cases in their projects.
```

