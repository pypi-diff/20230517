# Comparing `tmp/pyalpa-0.9.1.tar.gz` & `tmp/pyalpa-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.9.1.tar", max compression
+gzip compressed data, was "pyalpa-1.0.0.tar", max compression
```

## Comparing `pyalpa-0.9.1.tar` & `pyalpa-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-05-11 21:45:17.076266 pyalpa-0.9.1/LICENSE
--rw-r--r--   0        0        0      683 2023-05-11 21:45:17.076266 pyalpa-0.9.1/README.md
--rw-r--r--   0        0        0        0 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/cli/__init__.py
--rw-r--r--   0        0        0      732 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1203 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/cli/base.py
--rw-r--r--   0        0        0     6810 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/cli/local_repo.py
--rw-r--r--   0        0        0      160 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/__init__.py
--rw-r--r--   0        0        0     1264 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/alpa_local.py
--rw-r--r--   0        0        0     2599 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/base.py
--rw-r--r--   0        0        0     3344 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/config/metadata.py
--rw-r--r--   0        0        0     1233 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/constants.py
--rw-r--r--   0        0        0      158 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/exceptions.py
--rw-r--r--   0        0        0     4055 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/gh.py
--rw-r--r--   0        0        0     2735 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/git.py
--rw-r--r--   0        0        0     1553 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/messages.py
--rw-r--r--   0        0        0     2956 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/packit.py
--rw-r--r--   0        0        0      298 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/repository/__init__.py
--rw-r--r--   0        0        0    12145 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/repository/base.py
--rw-r--r--   0        0        0     5810 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/repository/branch.py
--rw-r--r--   0        0        0     1666 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/repository/subdirectory.py
--rw-r--r--   0        0        0     3879 2023-05-11 21:45:17.076266 pyalpa-0.9.1/alpa/upstream_integration.py
--rw-r--r--   0        0        0      846 2023-05-11 21:45:17.080266 pyalpa-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 pyalpa-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-16 22:53:44.048123 pyalpa-1.0.0/LICENSE
+-rw-r--r--   0        0        0      683 2023-05-16 22:53:44.048123 pyalpa-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      732 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1203 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/cli/base.py
+-rw-r--r--   0        0        0     6699 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      160 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1264 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2599 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/config/base.py
+-rw-r--r--   0        0        0     3344 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/config/metadata.py
+-rw-r--r--   0        0        0     1147 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/exceptions.py
+-rw-r--r--   0        0        0     4055 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/gh.py
+-rw-r--r--   0        0        0     2735 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/git.py
+-rw-r--r--   0        0        0     1553 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/messages.py
+-rw-r--r--   0        0        0     2956 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/packit.py
+-rw-r--r--   0        0        0      298 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    13060 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/repository/base.py
+-rw-r--r--   0        0        0     4902 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1666 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-05-16 22:53:44.048123 pyalpa-1.0.0/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      845 2023-05-16 22:53:44.056123 pyalpa-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 pyalpa-1.0.0/PKG-INFO
```

### Comparing `pyalpa-0.9.1/LICENSE` & `pyalpa-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/README.md` & `pyalpa-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/cli/alpa_repo.py` & `pyalpa-1.0.0/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/cli/base.py` & `pyalpa-1.0.0/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/cli/local_repo.py` & `pyalpa-1.0.0/alpa/cli/local_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,20 @@
 @click.option(
     "-m",
     "--message",
     type=str,
     default="",
     help="Your commit message not longer than 80 characters.",
 )
-@click.option("-n", "--no-verify", is_flag=True, help="Do not run pre-commit")
-def commit(message: str, no_verify: bool) -> None:
+def commit(message: str) -> None:
     """Commit your changes in your package's repository"""
     if len(message) > 80:
         raise ClickException("Message longer than 80 characters")
 
-    LocalRepoBranch(Path(getcwd())).commit(message, not no_verify)
+    LocalRepoBranch(Path(getcwd())).commit(message)
 
 
 @click.command("add")
 @click.argument("to_add", type=str, required=True)
 def add(to_add: str) -> None:
     """Add files to git history. Basically calls `git add <input>`"""
     LocalRepoBranch(Path(getcwd())).add(to_add)
```

### Comparing `pyalpa-0.9.1/alpa/config/alpa_local.py` & `pyalpa-1.0.0/alpa/config/alpa_local.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/config/alpa_repo.py` & `pyalpa-1.0.0/alpa/config/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/config/base.py` & `pyalpa-1.0.0/alpa/config/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/config/metadata.py` & `pyalpa-1.0.0/alpa/config/metadata.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/constants.py` & `pyalpa-1.0.0/alpa/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,19 +33,18 @@
     "metadata.yaml",
     "metadata.yml",
 ]
 
 ALPA_CONFIG_FILE_NAMES = [".alpa.yaml", ".alpa.yml", "alpa.yaml", "alpa.yml"]
 
 REQUEST_LABEL = "request"
+CREATE_PACKAGE_REQUEST_TITLE = (
+    "[alpa request-new-package] New request to create a package {package_name}"
+)
+DELETE_PACKAGE_REQUEST_TITLE = (
+    "[alpa delete-package] New request to delete a package {package_name}"
+)
 
 
-class PackageRequest(str, Enum):
-    TITLE = "[alpa request-new-package] New request for package {package_name}"
-    BODY = "@{user} requested {package_name}"
-    LABEL = REQUEST_LABEL
-
-
-class DeleteRequest(str, Enum):
-    TITLE = "[alpa delete-package] New request for deleting package {package_name}"
-    BODY = "@{user} requested to delete {package_name}"
-    LABEL = REQUEST_LABEL
+class RequestEnum(str, Enum):
+    delete = "delete"
+    create = "create"
```

### Comparing `pyalpa-0.9.1/alpa/gh.py` & `pyalpa-1.0.0/alpa/gh.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/git.py` & `pyalpa-1.0.0/alpa/git.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/messages.py` & `pyalpa-1.0.0/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/packit.py` & `pyalpa-1.0.0/alpa/packit.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/repository/base.py` & `pyalpa-1.0.0/alpa/repository/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """
 Set of commands that helps with integration of Alpa
 repository.
 """
 import logging
 import subprocess
 from abc import ABC, abstractmethod
+from json import dumps
 from os import getcwd
 from pathlib import Path
 from typing import Optional, Iterable
 from urllib.parse import urlparse
 
 from click import UsageError, ClickException
 import click
 
 from alpa.packit import Packit
 from alpa.constants import (
     ALPA_FEAT_BRANCH,
     ALPA_FEAT_BRANCH_PREFIX,
     ORIGIN_NAME,
     UPSTREAM_NAME,
+    RequestEnum,
+    REQUEST_LABEL,
+    DELETE_PACKAGE_REQUEST_TITLE,
+    CREATE_PACKAGE_REQUEST_TITLE,
 )
 from alpa.gh import GithubAPI, GithubRepo
 from alpa.git import GitCMD
 from alpa.messages import (
     CLONED_REPO_IS_NOT_FORK,
     NOT_IN_PREDEFINED_STATE,
     CLONED_REPO_IS_FORK,
@@ -233,15 +238,15 @@
 
         logger.debug(f"Branch {branch} does not exist in {branches}")
         return False
 
     def get_history_of_branch(self, branch: str, params: list[str]) -> str:
         return self.git_cmd(["log", "--decorate", "--graph"] + params + [branch]).stdout
 
-    def commit(self, message: str, pre_commit: bool) -> bool:
+    def commit(self, message: str) -> bool:
         packit_conf = Packit(self.package)
         if not packit_conf.packit_config_file_exists():
             packit_conf.create_packit_config()
             self.git_cmd(["add", ".packit.yaml"])
             self.git_cmd(
                 [
                     "commit",
@@ -317,21 +322,37 @@
         self.gh_api = gh_api or GithubAPI(self.repo_name)
         self.gh_repo = self.gh_api.get_repo(self.namespace, self.repo_name)
 
     @abstractmethod
     def create_package(self, package: str) -> None:
         pass
 
-    @abstractmethod
+    def _request_package_action(self, request_type: RequestEnum, pkg: str) -> None:
+        ensured_upstream = self.gh_repo.get_root_repo()
+        upstream_namespace = ensured_upstream.namespace
+        issue_repo = self.gh_api.get_repo(upstream_namespace, self.gh_repo.repo_name)
+
+        if request_type == RequestEnum.delete:
+            title = DELETE_PACKAGE_REQUEST_TITLE.format(package_name=pkg)
+        else:
+            title = CREATE_PACKAGE_REQUEST_TITLE.format(package_name=pkg)
+
+        body = {
+            "request_type": request_type,
+            "user": self.gh_api.gh_user,
+            "package": pkg,
+        }
+        issue = issue_repo.create_issue(title, dumps(body))
+        issue.add_to_labels(REQUEST_LABEL)
+
     def request_package(self, package_name: str) -> None:
-        pass
+        self._request_package_action(RequestEnum.create, package_name)
 
-    @abstractmethod
     def request_package_delete(self, package: str) -> None:
-        pass
+        self._request_package_action(RequestEnum.delete, package)
 
     @staticmethod
     def _prepare_cloned_repo(where_to_clone: str, gh_repo: GithubRepo) -> None:
         if not gh_repo.is_fork:
             return
 
         upstream_clone_url = gh_repo.upstream_clone_url
```

### Comparing `pyalpa-0.9.1/alpa/repository/branch.py` & `pyalpa-1.0.0/alpa/repository/branch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """
 Set of commands that helps with integration of Alpa
 repository.
 """
 
 from pathlib import Path
 import re
-from typing import Optional, Type
+from typing import Optional
 
 from click import ClickException
 import click
 
 from alpa.packit import Packit
 from alpa.constants import (
     ALPA_FEAT_BRANCH_PREFIX,
     MAIN_BRANCH,
-    PackageRequest,
-    DeleteRequest,
-    REQUEST_LABEL,
 )
 from alpa.gh import GithubAPI
 from alpa.messages import NO_WRITE_ACCESS_ERR
 from alpa.repository.base import LocalRepo, AlpaRepo
 
 
 class LocalRepoBranch(LocalRepo):
@@ -141,28 +138,7 @@
         if upstream and not upstream.has_write_access(self.gh_api.gh_user):
             raise ClickException(NO_WRITE_ACCESS_ERR)
 
         self.git_cmd(["switch", MAIN_BRANCH])
         self.git_cmd(["switch", "-c", package])
         self.git_cmd(["push", self.remote_name, package])
         click.echo(f"Package {package} created")
-
-    def _request_package_action(
-        self, action: Type[PackageRequest | DeleteRequest], pkg: str
-    ) -> None:
-        ensured_upstream = self.gh_repo.get_root_repo()
-        upstream_namespace = ensured_upstream.namespace
-        issue_repo = self.gh_api.get_repo(upstream_namespace, self.gh_repo.repo_name)
-        issue = issue_repo.create_issue(
-            action.TITLE.value.format(package_name=pkg),
-            action.BODY.value.format(
-                user=self.gh_api.gh_user,
-                package_name=pkg,
-            ),
-        )
-        issue.add_to_labels(REQUEST_LABEL)
-
-    def request_package(self, package_name: str) -> None:
-        self._request_package_action(PackageRequest, package_name)
-
-    def request_package_delete(self, package: str) -> None:
-        self._request_package_action(DeleteRequest, package)
```

### Comparing `pyalpa-0.9.1/alpa/repository/subdirectory.py` & `pyalpa-1.0.0/alpa/repository/subdirectory.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/alpa/upstream_integration.py` & `pyalpa-1.0.0/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.9.1/pyproject.toml` & `pyalpa-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.9.1"
+version = "1.0.0"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
@@ -29,14 +29,13 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
-
 [tool.poetry.scripts]
 alpa = "alpa.cli.base:entry_point"
 
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
```

### Comparing `pyalpa-0.9.1/PKG-INFO` & `pyalpa-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.9.1
+Version: 1.0.0
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
```

