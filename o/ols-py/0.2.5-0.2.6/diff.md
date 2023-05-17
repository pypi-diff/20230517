# Comparing `tmp/ols_py-0.2.5.tar.gz` & `tmp/ols_py-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ols_py-0.2.5.tar", max compression
+gzip compressed data, was "ols_py-0.2.6.tar", max compression
```

## Comparing `ols_py-0.2.5.tar` & `ols_py-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     3406 2022-11-23 02:47:54.069059 ols_py-0.2.5/README.md
--rw-r--r--   0        0        0     2167 2022-11-23 02:47:54.069059 ols_py-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       55 2022-11-23 02:47:54.069059 ols_py-0.2.5/src/ols_py/__init__.py
--rw-r--r--   0        0        0    10451 2022-11-23 02:47:54.069059 ols_py-0.2.5/src/ols_py/client.py
--rw-r--r--   0        0        0     1596 2022-11-23 02:47:54.069059 ols_py-0.2.5/src/ols_py/instances.py
--rw-r--r--   0        0        0        0 2022-11-23 02:47:54.069059 ols_py-0.2.5/src/ols_py/py.typed
--rw-r--r--   0        0        0       89 2022-11-23 02:47:54.069059 ols_py-0.2.5/src/ols_py/schemas/__init__.py
--rw-r--r--   0        0        0      408 2022-11-23 02:47:54.069059 ols_py-0.2.5/src/ols_py/schemas/common.py
--rw-r--r--   0        0        0     4142 2022-11-23 02:47:54.069059 ols_py-0.2.5/src/ols_py/schemas/requests.py
--rw-r--r--   0        0        0     3752 2022-11-23 02:47:54.069059 ols_py-0.2.5/src/ols_py/schemas/responses.py
--rw-r--r--   0        0        0     4294 1970-01-01 00:00:00.000000 ols_py-0.2.5/setup.py
--rw-r--r--   0        0        0     4461 1970-01-01 00:00:00.000000 ols_py-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-05-17 03:38:57.503710 ols_py-0.2.6/README.md
+-rw-r--r--   0        0        0     2167 2023-05-17 03:38:57.503710 ols_py-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/__init__.py
+-rw-r--r--   0        0        0    10705 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/client.py
+-rw-r--r--   0        0        0     1596 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/instances.py
+-rw-r--r--   0        0        0        0 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/py.typed
+-rw-r--r--   0        0        0       89 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/schemas/__init__.py
+-rw-r--r--   0        0        0      408 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/schemas/common.py
+-rw-r--r--   0        0        0     4197 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/schemas/requests.py
+-rw-r--r--   0        0        0     3752 2023-05-17 03:38:57.503710 ols_py-0.2.6/src/ols_py/schemas/responses.py
+-rw-r--r--   0        0        0     4461 1970-01-01 00:00:00.000000 ols_py-0.2.6/PKG-INFO
```

### Comparing `ols_py-0.2.5/README.md` & `ols_py-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.5/pyproject.toml` & `ols_py-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ols-py"
-version = "0.2.5"
+version = "0.2.6"
 description = "Python client for the Ontology Lookup Service"
 authors = [
     "Marius Mather <marius.mather@sydney.edu.au>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `ols_py-0.2.5/src/ols_py/client.py` & `ols_py-0.2.6/src/ols_py/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,14 +184,21 @@
         :return: response object. the actual terms are in a list at
           ``response.embedded.terms``
         """
         return self._get_term_relatives(
             "parents", ontology_id=ontology_id, term_id=term_id
         )
 
+    def get_term_hierarchical_parents(
+        self, ontology_id: str, term_id: str
+    ) -> schemas.responses.MultipleTerms:
+        return self._get_term_relatives(
+            "hierarchicalParents", ontology_id=ontology_id, term_id=term_id
+        )
+
     def get_term_children(
         self, ontology_id: str, term_id: str
     ) -> schemas.responses.MultipleTerms:
         """
         Get children for a term.
         :param ontology_id: Name of ontology, e.g. "go"
         :param term_id: Term ID (URI, short form or obo ID)
```

### Comparing `ols_py-0.2.5/src/ols_py/instances.py` & `ols_py-0.2.6/src/ols_py/instances.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.5/src/ols_py/schemas/requests.py` & `ols_py-0.2.6/src/ols_py/schemas/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,15 +124,17 @@
                 value = ",".join(value)
             query_dict[field_name] = value
         return query_dict
 
 
 RelativeTypes = Literal[
     "parents",
+    "hierarchicalParents",
     "children",
+    "hierarchicalChildren",
     "ancestors",
     "descendants",
     "hierarchicalDescendants",
     "hierarchicalAncestors",
 ]
```

### Comparing `ols_py-0.2.5/src/ols_py/schemas/responses.py` & `ols_py-0.2.6/src/ols_py/schemas/responses.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.2.5/setup.py` & `ols_py-0.2.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,131 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ols-py
+Version: 0.2.6
+Summary: Python client for the Ontology Lookup Service
+Home-page: https://ahida-development.github.io/ols-py
+License: MIT
+Author: Marius Mather
+Author-email: marius.mather@sydney.edu.au
+Requires-Python: >=3.10.1,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: requests (>=2.0,<3.0)
+Project-URL: Documentation, https://ahida-development.github.io/ols-py
+Project-URL: Repository, https://github.com/ahida-development/ols-py
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# ols-py
 
-packages = \
-['ols_py', 'ols_py.schemas']
+[![PyPI](https://img.shields.io/pypi/v/ols-py?style=flat-square)](https://pypi.python.org/pypi/ols-py/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ols-py?style=flat-square)](https://pypi.python.org/pypi/ols-py/)
+[![PyPI - License](https://img.shields.io/pypi/l/ols-py?style=flat-square)](https://pypi.python.org/pypi/ols-py/)
+[![Tests][github actions badge]][github actions page]
+[![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic>=1.10.2,<2.0.0', 'requests>=2.0,<3.0']
-
-setup_kwargs = {
-    'name': 'ols-py',
-    'version': '0.2.5',
-    'description': 'Python client for the Ontology Lookup Service',
-    'long_description': "# ols-py\n\n[![PyPI](https://img.shields.io/pypi/v/ols-py?style=flat-square)](https://pypi.python.org/pypi/ols-py/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ols-py?style=flat-square)](https://pypi.python.org/pypi/ols-py/)\n[![PyPI - License](https://img.shields.io/pypi/l/ols-py?style=flat-square)](https://pypi.python.org/pypi/ols-py/)\n[![Tests][github actions badge]][github actions page]\n[![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)\n\n[github actions badge]: https://github.com/ahida-development/ols-py/workflows/Test/badge.svg\n[github actions page]: https://github.com/ahida-development/ols-py/actions?workflow=test\n\n---\n\n**Documentation**: [https://ahida-development.github.io/ols-py](https://ahida-development.github.io/ols-py)\n\n**Source Code**: [https://github.com/ahida-development/ols-py](https://github.com/ahida-development/ols-py)\n\n**PyPI**: [https://pypi.org/project/ols-py/](https://pypi.org/project/ols-py/)\n\n---\n\nPython client for the Ontology Lookup Service\n\n**Current status:** in development, some endpoints and schemas are not\nimplemented yet.\n\nFeatures:\n\n* Type annotated so you know which parameters can be used for each endpoint\n* Responses validated and parsed with [pydantic](https://github.com/pydantic/pydantic) for\n  easy access to response data\n\n## Installation\n\n```sh\npip install ols-py\n```\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.10+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings\n of the public signatures of the source code. The documentation is updated and published as a [Github project page\n ](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/ahida-development/ols-py/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/ahida-development/ols-py/releases) and publish it. When\n a release is published, it'll trigger [release](https://github.com/ahida-development/ols-py/blob/master/.github/workflows/release.yml) workflow which creates PyPI\n release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n\nThis project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.\n",
-    'author': 'Marius Mather',
-    'author_email': 'marius.mather@sydney.edu.au',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://ahida-development.github.io/ols-py',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10.1,<4.0',
-}
+[github actions badge]: https://github.com/ahida-development/ols-py/workflows/Test/badge.svg
+[github actions page]: https://github.com/ahida-development/ols-py/actions?workflow=test
 
+---
+
+**Documentation**: [https://ahida-development.github.io/ols-py](https://ahida-development.github.io/ols-py)
+
+**Source Code**: [https://github.com/ahida-development/ols-py](https://github.com/ahida-development/ols-py)
+
+**PyPI**: [https://pypi.org/project/ols-py/](https://pypi.org/project/ols-py/)
+
+---
+
+Python client for the Ontology Lookup Service
+
+**Current status:** in development, some endpoints and schemas are not
+implemented yet.
+
+Features:
+
+* Type annotated so you know which parameters can be used for each endpoint
+* Responses validated and parsed with [pydantic](https://github.com/pydantic/pydantic) for
+  easy access to response data
+
+## Installation
+
+```sh
+pip install ols-py
+```
+
+## Development
+
+* Clone this repository
+* Requirements:
+  * [Poetry](https://python-poetry.org/)
+  * Python 3.10+
+* Create a virtual environment and install the dependencies
+
+```sh
+poetry install
+```
+
+* Activate the virtual environment
+
+```sh
+poetry shell
+```
+
+### Testing
+
+```sh
+pytest
+```
+
+### Documentation
+
+The documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings
+ of the public signatures of the source code. The documentation is updated and published as a [Github project page
+ ](https://pages.github.com/) automatically as part each release.
+
+### Releasing
+
+Trigger the [Draft release workflow](https://github.com/ahida-development/ols-py/actions/workflows/draft_release.yml)
+(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.
+
+Find the draft release from the
+[GitHub releases](https://github.com/ahida-development/ols-py/releases) and publish it. When
+ a release is published, it'll trigger [release](https://github.com/ahida-development/ols-py/blob/master/.github/workflows/release.yml) workflow which creates PyPI
+ release and deploys updated documentation.
+
+### Pre-commit
+
+Pre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality
+ checks to make sure the changeset is in good shape before a commit/push happens.
+
+You can install the hooks with (runs for each commit):
+
+```sh
+pre-commit install
+```
+
+Or if you want them to run only for each push:
+
+```sh
+pre-commit install -t pre-push
+```
+
+Or if you want e.g. want to run all checks manually for all files:
+
+```sh
+pre-commit run --all-files
+```
+
+---
+
+This project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.
 
-setup(**setup_kwargs)
```

