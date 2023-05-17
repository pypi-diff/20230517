# Comparing `tmp/obsidian_metadata-0.8.0.tar.gz` & `tmp/obsidian_metadata-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsidian_metadata-0.8.0.tar", max compression
+gzip compressed data, was "obsidian_metadata-0.9.0.tar", max compression
```

## Comparing `obsidian_metadata-0.8.0.tar` & `obsidian_metadata-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2023-03-12 18:14:17.434575 obsidian_metadata-0.8.0/LICENSE
--rw-r--r--   0        0        0     7929 2023-03-12 18:14:17.434575 obsidian_metadata-0.8.0/README.md
--rw-r--r--   0        0        0     6661 2023-03-12 18:14:17.438575 obsidian_metadata-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       33 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/__init__.py
--rw-r--r--   0        0        0       55 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/__version__.py
--rw-r--r--   0        0        0      149 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/_config/__init__.py
--rw-r--r--   0        0        0     6228 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/_config/config.py
--rw-r--r--   0        0        0      656 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/_utils/__init__.py
--rw-r--r--   0        0        0     7794 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/_utils/alerts.py
--rw-r--r--   0        0        0      101 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/_utils/console.py
--rw-r--r--   0        0        0     5527 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/_utils/utilities.py
--rw-r--r--   0        0        0     7979 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/cli.py
--rw-r--r--   0        0        0      723 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/models/__init__.py
--rw-r--r--   0        0        0    26443 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/models/application.py
--rw-r--r--   0        0        0      600 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/models/enums.py
--rw-r--r--   0        0        0    22085 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/models/metadata.py
--rw-r--r--   0        0        0    22686 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/models/notes.py
--rw-r--r--   0        0        0     3107 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/models/patterns.py
--rw-r--r--   0        0        0    17604 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/models/questions.py
--rw-r--r--   0        0        0    17963 2023-03-12 18:14:17.442575 obsidian_metadata-0.8.0/src/obsidian_metadata/models/vault.py
--rw-r--r--   0        0        0     8880 1970-01-01 00:00:00.000000 obsidian_metadata-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-03-20 22:23:33.798323 obsidian_metadata-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9408 2023-03-20 22:23:33.798323 obsidian_metadata-0.9.0/README.md
+-rw-r--r--   0        0        0     8083 2023-03-20 22:23:33.798323 obsidian_metadata-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-03-20 22:23:33.798323 obsidian_metadata-0.9.0/src/obsidian_metadata/__init__.py
+-rw-r--r--   0        0        0       55 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/__version__.py
+-rw-r--r--   0        0        0      149 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/_config/__init__.py
+-rw-r--r--   0        0        0     6227 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/_config/config.py
+-rw-r--r--   0        0        0      746 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/_utils/__init__.py
+-rw-r--r--   0        0        0     8055 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/_utils/alerts.py
+-rw-r--r--   0        0        0      101 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/_utils/console.py
+-rw-r--r--   0        0        0     7728 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/_utils/utilities.py
+-rw-r--r--   0        0        0     4988 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/cli.py
+-rw-r--r--   0        0        0      723 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/models/__init__.py
+-rw-r--r--   0        0        0    29076 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/models/application.py
+-rw-r--r--   0        0        0      600 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/models/enums.py
+-rw-r--r--   0        0        0    22444 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/models/metadata.py
+-rw-r--r--   0        0        0    23172 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/models/notes.py
+-rw-r--r--   0        0        0     3121 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/models/patterns.py
+-rw-r--r--   0        0        0    18679 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/models/questions.py
+-rw-r--r--   0        0        0    21657 2023-03-20 22:23:33.802323 obsidian_metadata-0.9.0/src/obsidian_metadata/models/vault.py
+-rw-r--r--   0        0        0    10403 1970-01-01 00:00:00.000000 obsidian_metadata-0.9.0/PKG-INFO
```

### Comparing `obsidian_metadata-0.8.0/LICENSE` & `obsidian_metadata-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obsidian_metadata-0.8.0/README.md` & `obsidian_metadata-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: obsidian-metadata
+Version: 0.9.0
+Summary: Make batch updates to Obsidian metadata
+Home-page: https://github.com/natelandau/obsidian-metadata
+License: GNU AFFERO
+Keywords: obsidian
+Author: Nate Landau
+Author-email: github@natenate.org
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: commitizen (>=2.42.1,<3.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Requires-Dist: regex (>=2022.10.31,<2023.0.0)
+Requires-Dist: rich (>=13.3.2,<14.0.0)
+Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
+Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
+Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Project-URL: Repository, https://github.com/natelandau/obsidian-metadata
+Description-Content-Type: text/markdown
+
 [![PyPI version](https://badge.fury.io/py/obsidian-metadata.svg)](https://badge.fury.io/py/obsidian-metadata) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/obsidian-metadata) [![Python Code Checker](https://github.com/natelandau/obsidian-metadata/actions/workflows/automated-tests.yml/badge.svg)](https://github.com/natelandau/obsidian-metadata/actions/workflows/automated-tests.yml) [![codecov](https://codecov.io/gh/natelandau/obsidian-metadata/branch/main/graph/badge.svg?token=3F2R43SSX4)](https://codecov.io/gh/natelandau/obsidian-metadata)
 
 # obsidian-metadata
 
 A script to make batch updates to metadata in an Obsidian vault. No changes are
 made to the Vault until they are explicitly committed.
 
@@ -39,30 +65,37 @@
 Once installed, run `obsidian-metadata` in your terminal to enter an interactive menu of sub-commands.
 
 **Vault Actions**
 
 -   Backup: Create a backup of the vault.
 -   Delete Backup: Delete a backup of the vault.
 
+**Export Metadata**
+
+-   Export all metadata to a CSV organized by metadata type
+-   Export all metadata to a CSV organized by note path
+-   Export all metadata to a JSON file organized by metadata type
+
 **Inspect Metadata**
 
 -   **View all metadata in the vault**
 -   View all **frontmatter**
 -   View all **inline metadata**
 -   View all **inline tags**
--   **Export all metadata to CSV or JSON file**
 
 **Filter Notes in Scope**: Limit the scope of notes to be processed with one or more filters.
 
 -   **Path filter (regex)**: Limit scope based on the path or filename
 -   **Metadata filter**: Limit scope based on a key or key/value pair
 -   **Tag filter**: Limit scope based on an in-text tag
 -   **List and clear filters**: List all current filters and clear one or all
 -   **List notes in scope**: List notes that will be processed.
 
+**Bulk Edit Metadata** from a CSV file (See the _making bulk edits_ section below)
+
 **Add Metadata**: Add new metadata to your vault.
 
 When adding a new key to inline metadata, the `insert location` value in the config file will specify where in the note it will be inserted.
 
 -   **Add new metadata to the frontmatter**
 -   **Add new inline metadata** - Set `insert_location` in the config to control where the new metadata is inserted. (Default: Bottom)
 -   **Add new inline tag** - Set `insert_location` in the config to control where the new tag is inserted. (Default: Bottom)
@@ -128,14 +161,44 @@
     path = "/path/to/second_vault"
     exclude_paths = [".git", ".obsidian", "daily_notes"]
     insert_location = "AFTER_TITLE"
 ```
 
 To bypass the configuration file and specify a vault to use at runtime use the `--vault-path` option.
 
+### Making bulk edits
+
+Bulk edits are supported by importing a CSV file containing the following columns. Column headers must be lowercase.
+
+1. `path` - Path to note relative to the vault root folder
+2. `type` - Type of metadata. One of `frontmatter`, `inline_metadata`, or `tag`
+3. `key` - The key to add (leave blank for a tag)
+4. `value` - the value to add to the key
+
+An example valid CSV file is
+
+```csv
+path,type,key,value
+folder 1/note1.md,frontmatter,fruits,apple
+folder 1/note1.md,frontmatter,fruits,banana
+folder 1/note1.md,inline_metadata,cars,toyota
+folder 1/note1.md,inline_metadata,cars,honda
+folder 1/note1.md,tag,,tag1
+folder 1/note1.md,tag,,tag2
+```
+
+How bulk imports work:
+
+-   Only notes which match the path in the CSV file are updated
+-   Effected notes will have ALL of their metadata changed to reflect the values in the CSV file
+-   Existing metadata in an effected note will be rewritten. This may result in it's location and/or formatting within the note being changed
+-   inline tags ignore any value added to the `key` column
+
+You can export all your notes with their associated metadata in this format from the "Export Metadata" section of the script to be used as a template for your bulk changes.
+
 # Contributing
 
 ## Setup: Once per project
 
 There are two ways to contribute to this project.
 
 ### 1. Containerized development
@@ -159,7 +222,12 @@
     -   When you're ready to commit changes run `cz c`
 -   Run `poe` from within the development environment to print a list of [Poe the Poet](https://github.com/nat-n/poethepoet) tasks available to run on this project. Common commands:
     -   `poe lint` runs all linters
     -   `poe test` runs all tests with Pytest
 -   Run `poetry add {package}` from within the development environment to install a run time dependency and add it to `pyproject.toml` and `poetry.lock`.
 -   Run `poetry remove {package}` from within the development environment to uninstall a run time dependency and remove it from `pyproject.toml` and `poetry.lock`.
 -   Run `poetry update` from within the development environment to upgrade all dependencies to the latest versions allowed by `pyproject.toml`.
+
+```
+
+```
+
```

### Comparing `obsidian_metadata-0.8.0/pyproject.toml` & `obsidian_metadata-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -7,105 +7,63 @@
     description = "Make batch updates to Obsidian metadata"
     homepage    = "https://github.com/natelandau/obsidian-metadata"
     keywords    = ["obsidian"]
     license     = "GNU AFFERO"
     name        = "obsidian-metadata"
     readme      = "README.md"
     repository  = "https://github.com/natelandau/obsidian-metadata"
-    version     = "0.8.0"
+    version     = "0.9.0"
 
     [tool.poetry.scripts] # https://python-poetry.org/docs/pyproject/#scripts
         obsidian-metadata = "obsidian_metadata.cli:app"
 
     [tool.poetry.dependencies]
         loguru      = "^0.6.0"
         python      = "^3.10"
         questionary = "^1.10.0"
         regex       = "^2022.10.31"
         rich        = "^13.3.2"
         ruamel-yaml = "^0.17.21"
         shellingham = "^1.5.0.post1"
         tomlkit     = "^0.11.6"
         typer       = "^0.7.0"
+    commitizen = "^2.42.1"
 
     [tool.poetry.group.test.dependencies]
         pytest                 = "^7.2.2"
         pytest-clarity         = "^1.0.1"
         pytest-mock            = "^3.10.0"
         pytest-pretty-terminal = "^1.1.0"
-        pytest-xdist           = "^3.2.0"
+        pytest-xdist           = "^3.2.1"
 
     [tool.poetry.group.dev.dependencies]
         black                 = "^23.1.0"
         commitizen            = "^2.42.1"
-        coverage              = "^7.2.1"
+        coverage              = "^7.2.2"
         interrogate           = "^1.5.0"
         mypy                  = "^1.1.1"
         pdoc                  = "^13.0.0"
         poethepoet            = "^0.18.1"
-        pre-commit            = "^3.1.1"
-        pysnooper             = "^1.1.1"
-        ruff                  = "^0.0.254"
-        typeguard             = "^2.13.3"
+        pre-commit            = "^3.2.0"
+        ruff                  = "0.0.257"
+        typeguard             = "^3.0.1"
         types-python-dateutil = "^2.8.19.10"
         vulture               = "^2.7"
+    sh = "2.0.3"
 
-[tool.ruff] # https://github.com/charliermarsh/ruff
-    fix = true
-    ignore = [
-        "B006",
-        "B008",
-        "D107",
-        "D203",
-        "D204",
-        "D213",
-        "D215",
-        "D404",
-        "D406",
-        "D407",
-        "D408",
-        "D409",
-        "D413",
-        "E501",
-        "N805",
-        "PGH001",
-        "PGH003",
-        "UP007",
-    ]
-    ignore-init-module-imports = true
+[tool.black]
     line-length = 100
-    per-file-ignores = { "cli.py" = ["PLR0912", "PLR0913"], "tests/*.py" = ["PLR0913", "PLR2004"] }
-    select = [
-        "A",
-        "B",
-        "BLE",
-        "C4",
-        "C90",
-        "D",
-        "E",
-        "ERA",
-        "F",
-        "I",
-        "N",
-        "PGH",
-        "PLC",
-        "PLE",
-        "PLR",
-        "PLW",
-        "RET",
-        "RUF",
-        "SIM",
-        "TID",
-        "UP",
-        "W",
-        "YTT",
-    ]
-    src = ["src", "tests"]
-    target-version = "py310"
-    unfixable = ["ERA001", "F401", "F841", "UP007"]
+
+[tool.commitizen]
+    bump_message             = "bump(release): v$current_version → v$new_version"
+    changelog_incremental    = true
+    tag_format               = "v$version"
+    update_changelog_on_bump = true
+    version                  = "0.9.0"
+    version_files            = ["pyproject.toml:version", "src/obsidian_metadata/__version__.py:__version__"]
 
 [tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html#report
     exclude_lines = [
         'def __repr__',
         'except [\w\s\._]+ as .*:',
         'log\.critical',
         'log\.debug',
@@ -130,25 +88,14 @@
     command_line = "--module pytest"
     data_file    = "reports/.coverage"
     source       = ["src"]
 
 [tool.coverage.xml]
     output = "reports/coverage.xml"
 
-[tool.black]
-    line-length = 100
-
-[tool.commitizen]
-    bump_message             = "bump(release): v$current_version → v$new_version"
-    changelog_incremental    = true
-    tag_format               = "v$version"
-    update_changelog_on_bump = true
-    version                  = "0.8.0"
-    version_files            = ["pyproject.toml:version", "src/obsidian_metadata/__version__.py:__version__"]
-
 [tool.interrogate]
     exclude            = ["build", "docs", "tests"]
     fail-under         = 90
     ignore-init-method = true
     verbose            = 2
 
 [tool.mypy] # https://mypy.readthedocs.io/en/latest/config_file.html
@@ -174,14 +121,116 @@
 
 [tool.pytest.ini_options]
     addopts        = "--color=yes --doctest-modules --exitfirst --failed-first --strict-config --strict-markers --verbosity=2 --junitxml=reports/pytest.xml"
     filterwarnings = ["error", "ignore::DeprecationWarning"]
     testpaths      = ["src", "tests"]
     xfail_strict   = true
 
+[tool.ruff] # https://github.com/charliermarsh/ruff
+    exclude = [
+        ".bzr",
+        ".direnv",
+        ".eggs",
+        ".git",
+        ".hg",
+        ".mypy_cache",
+        ".nox",
+        ".pants.d",
+        ".pytype",
+        ".ruff_cache",
+        ".svn",
+        ".tox",
+        ".venv",
+        "__pypackages__",
+        "_build",
+        "buck-out",
+        "build",
+        "dist",
+        "node_modules",
+        "venv",
+    ]
+    # Avoiding flagging (and removing) `V101` from any `# noqa`
+    # directives, despite Ruff's lack of support for `vulture`.
+    external = ["V101"]
+    fix = true
+    ignore = [
+        "B006",
+        "B008",
+        "D107",
+        "D203",
+        "D204",
+        "D213",
+        "D215",
+        "D404",
+        "D406",
+        "D407",
+        "D408",
+        "D409",
+        "D413",
+        "E501",
+        "N805",
+        "PGH001",
+        "PGH003",
+        "UP007",
+    ]
+    ignore-init-module-imports = true
+    line-length = 100
+    per-file-ignores = { "cli.py" = [
+        "PLR0912",
+        "PLR0913",
+    ], "tests/*.py" = [
+        "PLR0913",
+        "PLR2004",
+        "S101",
+    ] }
+    select = [
+        "A",   # flake8-builtins
+        "ARG", # flake8-unused-arguments
+        "B",   # flake8-bugbear
+        "BLE", # flake8-blind-exception
+        "C40", # flake8-comprehensions
+        "C90", # McCabe
+        "D",   # pydocstyle
+        "E",   # pycodestyle Errors
+        "ERA", # flake8-eradicate
+        "EXE", # flake8-executable
+        "F",   # pyflakes
+        "I",   # iSort
+        "N",   # Pep8-naming
+        "PGH", # pygrep-hooks
+        "PLC", # pylint Convention
+        "PLE", # pylint Error
+        "PLR", # pylint Refactor
+        "PLW", # pylint Warning
+        "PT",  # flake8-pytest-style
+        "PTH", # flake8-use-pathlib
+        "Q",   # flake8-quotes
+        "RET", # flake8-return
+        "RUF", # Ruff-specific rules
+        "S",   # flake8-bandit
+        "SIM", # flake8-simplify
+        "TID", # flake8-tidy-imports
+        "UP",  # pyupgrade
+        "W",   # pycodestyle Warnings
+        "YTT", # flake8-2020
+    ]
+    src = ["src", "tests"]
+    target-version = "py310"
+    unfixable = ["ERA001", "F401", "F841", "UP007"]
+
+    [tool.ruff.mccabe]
+        # Unlike Flake8, default to a complexity level of 10.
+        max-complexity = 10
+
+    [tool.ruff.pydocstyle]
+        convention = "google"
+
+    [tool.ruff.pylint]
+        max-args = 6
+
 [tool.vulture] # https://pypi.org/project/vulture/
     # exclude = ["file*.py", "dir/"]
     # ignore_decorators = ["@app.route", "@require_*"]
     ignore_names = ["args", "cls", "indentless", "kwargs", "request", "version"]
     # make_whitelist = true
     min_confidence = 80
     paths          = ["src", "tests"]
@@ -199,15 +248,15 @@
     """
         help = "Generate this package's docs"
 
     [tool.poe.tasks.lint]
         help = "Lint this package"
 
         [[tool.poe.tasks.lint.sequence]]
-            shell = "ruff --extend-ignore=I001,D301,D401 src/"
+            shell = "ruff src/ --no-fix"
 
         [[tool.poe.tasks.lint.sequence]]
             shell = "black --check src/ tests/"
 
         [[tool.poe.tasks.lint.sequence]]
             shell = "poetry check"
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/_config/config.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/_config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         """Define rich representation of the Config object."""
         yield "config_path", self.config_path
         yield "vaults", self.vaults
 
     def _load_config(self) -> dict[str, Any]:
         """Load the configuration file."""
         try:
-            with open(self.config_path, encoding="utf-8") as fp:
+            with self.config_path.open(encoding="utf-8") as fp:
                 return tomlkit.load(fp)
         except tomlkit.exceptions.TOMLKitError as e:
             alerts.error(f"Could not parse '{self.config_path}'")
             raise typer.Exit(code=1) from e
 
     def _validate_config_path(self, config_path: Path | None) -> Path:
         """Load the configuration path."""
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/_utils/__init__.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/_utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 from obsidian_metadata._utils import alerts
 from obsidian_metadata._utils.alerts import LoggerManager
 from obsidian_metadata._utils.utilities import (
     clean_dictionary,
     clear_screen,
     dict_contains,
+    dict_keys_to_lower,
     dict_values_to_lists_strings,
     docstring_parameter,
     merge_dictionaries,
     remove_markdown_sections,
+    validate_csv_bulk_imports,
     version_callback,
 )
 
 __all__ = [
     "alerts",
     "clean_dictionary",
     "clear_screen",
     "dict_contains",
+    "dict_keys_to_lower",
     "dict_values_to_lists_strings",
     "docstring_parameter",
     "LoggerManager",
     "merge_dictionaries",
     "remove_markdown_sections",
-    "vault_validation",
+    "validate_csv_bulk_imports",
     "version_callback",
 ]
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/_utils/alerts.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/_utils/alerts.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,21 +83,24 @@
 
     Args:
         msg: Message to print
     """
     console.print(f"INFO     | {msg}")
 
 
-def usage(msg: str, width: int = 80) -> None:
+def usage(msg: str, width: int = None) -> None:
     """Print a usage message without using logging.
 
     Args:
         msg: Message to print
         width (optional): Width of the message
     """
+    if width is None:
+        width = console.width - 15
+
     for _n, line in enumerate(wrap(msg, width=width)):
         if _n == 0:
             console.print(f"[dim]USAGE    | {line}")
         else:
             console.print(f"[dim]         | {line}")
 
 
@@ -122,17 +125,20 @@
 def _log_formatter(record: dict) -> str:
     """Create custom log formatter based on the log level.  This effects the logs sent to stdout/stderr but not the log file."""
     if (
         record["level"].name == "INFO"
         or record["level"].name == "SUCCESS"
         or record["level"].name == "WARNING"
     ):
-        return "<level>{level: <8}</level> | <level>{message}</level>\n{exception}"
+        return "<level><normal>{level: <8} | {message}</normal></level>\n{exception}"
+
+    if record["level"].name == "TRACE" or record["level"].name == "DEBUG":
+        return "<level><normal>{level: <8} | {message}</normal></level> <fg #c5c5c5>({name}:{function}:{line})</fg #c5c5c5>\n{exception}"
 
-    return "<level>{level: <8}</level> | <level>{message}</level> <fg #c5c5c5>({name}:{function}:{line})</fg #c5c5c5>\n{exception}"
+    return "<level>{level: <8} | {message}</level> <fg #c5c5c5>({name}:{function}:{line})</fg #c5c5c5>\n{exception}"
 
 
 @rich.repr.auto
 class LoggerManager:
     """Instantiate the loguru logging system with the following levels.
 
         - TRACE: Usage: log.trace("")
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/_utils/utilities.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/_utils/utilities.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Utility functions."""
+import csv
 import re
 from os import name, system
+from pathlib import Path
 from typing import Any
 
 import typer
 
 from obsidian_metadata.__version__ import __version__
+from obsidian_metadata._utils import alerts
+from obsidian_metadata._utils.alerts import logger as log
 from obsidian_metadata._utils.console import console
 
 
 def clean_dictionary(dictionary: dict[str, Any]) -> dict[str, Any]:
     """Clean up a dictionary by markdown formatting from keys and values.
 
     Args:
@@ -59,14 +63,26 @@
                     any(re.search(value, _v) for _v in dictionary[_key]),
                 )
         return any(found_keys)
 
     return key in dictionary and value in dictionary[key]
 
 
+def dict_keys_to_lower(dictionary: dict) -> dict:
+    """Convert all keys in a dictionary to lowercase.
+
+    Args:
+        dictionary (dict): Dictionary to convert
+
+    Returns:
+        dict: Dictionary with all keys converted to lowercase
+    """
+    return {key.lower(): value for key, value in dictionary.items()}
+
+
 def dict_values_to_lists_strings(
     dictionary: dict,
     strip_null_values: bool = False,
 ) -> dict:
     """Convert all values in a dictionary to lists of strings.
 
     Args:
@@ -82,15 +98,15 @@
 
     if strip_null_values:
         for key, value in dictionary.items():
             if isinstance(value, list):
                 new_dict[key] = sorted([str(item) for item in value if item is not None])
             elif isinstance(value, dict):
                 new_dict[key] = dict_values_to_lists_strings(value)  # type: ignore[assignment]
-            elif value is None or value == "None" or value == "":
+            elif value is None or value == "None" or not value:
                 new_dict[key] = []
             else:
                 new_dict[key] = [str(value)]
 
         return new_dict
 
     for key, value in dictionary.items():
@@ -175,15 +191,64 @@
 
     if strip_inlinecode:
         text = re.sub(r"`.*?`", "", text)
 
     if strip_frontmatter:
         text = re.sub(r"^\s*---.*?---", "", text, flags=re.DOTALL)
 
-    return text  # noqa: RET504
+    return text
+
+
+def validate_csv_bulk_imports(csv_path: Path, note_paths: list) -> dict[str, list[dict[str, str]]]:
+    """Validate the bulk import CSV file.
+
+    Args:
+        csv_path (dict): Dictionary to validate
+        note_paths (list): List of paths to all notes in vault
+
+    Returns:
+        dict: Validated dictionary
+    """
+    csv_dict: dict[str, Any] = {}
+    with csv_path.expanduser().open("r") as csv_file:
+        csv_reader = csv.DictReader(csv_file, delimiter=",")
+        row_num = 0
+        for row in csv_reader:
+            if row_num == 0:
+                if "path" not in row:
+                    raise typer.BadParameter("Missing 'path' column in CSV file")
+                if "type" not in row:
+                    raise typer.BadParameter("Missing 'type' column in CSV file")
+                if "key" not in row:
+                    raise typer.BadParameter("Missing 'key' column in CSV file")
+                if "value" not in row:
+                    raise typer.BadParameter("Missing 'value' column in CSV file")
+            row_num += 1
+
+            if row["path"] not in csv_dict:
+                csv_dict[row["path"]] = []
+
+            csv_dict[row["path"]].append(
+                {"type": row["type"], "key": row["key"], "value": row["value"]}
+            )
+
+        if row_num == 0 or row_num == 1:
+            raise typer.BadParameter("Empty CSV file")
+
+        paths_to_remove = [x for x in csv_dict if x not in note_paths]
+
+        for _path in paths_to_remove:
+            alerts.warning(f"'{_path}' does not exist in vault. Skipping...")
+            del csv_dict[_path]
+
+        if len(csv_dict) == 0:
+            log.error("No paths in the CSV file matched paths in the vault")
+            raise typer.Exit(1)
+
+    return csv_dict
 
 
 def version_callback(value: bool) -> None:
     """Print version and exit."""
     if value:
         console.print(f"{__package__.split('.')[0]}: v{__version__}")
         raise typer.Exit()
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/models/__init__.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/models/application.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/models/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import questionary
 import typer
 from rich import box
 from rich.table import Table
 
 from obsidian_metadata._config import VaultConfig
-from obsidian_metadata._utils import alerts
+from obsidian_metadata._utils import alerts, validate_csv_bulk_imports
 from obsidian_metadata._utils.console import console
 from obsidian_metadata.models import InsertLocation, Vault, VaultFilter
 from obsidian_metadata.models.enums import MetadataType
 from obsidian_metadata.models.questions import Questions
 
 
 class Application:
@@ -49,16 +49,20 @@
 
         while True:
             self.vault.info()
 
             match self.questions.ask_application_main():
                 case "vault_actions":
                     self.application_vault()
+                case "export_metadata":
+                    self.application_export_metadata()
                 case "inspect_metadata":
                     self.application_inspect_metadata()
+                case "import_from_csv":
+                    self.application_import_csv()
                 case "filter_notes":
                     self.application_filter()
                 case "add_metadata":
                     self.application_add_metadata()
                 case "rename_metadata":
                     self.application_rename_metadata()
                 case "delete_metadata":
@@ -69,15 +73,14 @@
                     self.review_changes()
                 case "commit_changes":
                     self.commit_changes()
                 case _:
                     break
 
         console.print("Done!")
-        return
 
     def application_add_metadata(self) -> None:
         """Add metadata."""
         alerts.usage(
             "Add new metadata to your vault. Currently only supports adding to the frontmatter of a note."
         )
 
@@ -121,14 +124,15 @@
                 return
 
     def application_delete_metadata(self) -> None:
         """Delete metadata."""
         alerts.usage("Delete either a key and all associated values, or a specific value.")
 
         choices = [
+            questionary.Separator(),
             {"name": "Delete inline tag", "value": "delete_inline_tag"},
             {"name": "Delete key", "value": "delete_key"},
             {"name": "Delete value", "value": "delete_value"},
             questionary.Separator(),
             {"name": "Back", "value": "back"},
         ]
         match self.questions.ask_selection(
@@ -144,14 +148,15 @@
                 return
 
     def application_rename_metadata(self) -> None:
         """Rename metadata."""
         alerts.usage("Select the type of metadata to rename.")
 
         choices = [
+            questionary.Separator(),
             {"name": "Rename inline tag", "value": "rename_inline_tag"},
             {"name": "Rename key", "value": "rename_key"},
             {"name": "Rename value", "value": "rename_value"},
             questionary.Separator(),
             {"name": "Back", "value": "back"},
         ]
         match self.questions.ask_selection(
@@ -167,27 +172,28 @@
                 return
 
     def application_filter(self) -> None:  # noqa: C901,PLR0911,PLR0912
         """Filter notes."""
         alerts.usage("Limit the scope of notes to be processed with one or more filters.")
 
         choices = [
+            questionary.Separator(),
             {"name": "Apply new regex path filter", "value": "apply_path_filter"},
             {"name": "Apply new metadata filter", "value": "apply_metadata_filter"},
             {"name": "Apply new in-text tag filter", "value": "apply_tag_filter"},
             {"name": "List and clear filters", "value": "list_filters"},
             {"name": "List notes in scope", "value": "list_notes"},
             questionary.Separator(),
             {"name": "Back", "value": "back"},
         ]
         while True:
             match self.questions.ask_selection(choices=choices, question="Select an action"):
                 case "apply_path_filter":
                     path = self.questions.ask_filter_path()
-                    if path is None or path == "":  # pragma: no cover
+                    if path is None or not path:  # pragma: no cover
                         return
 
                     self.filters.append(VaultFilter(path_filter=path))
                     self._load_vault()
 
                 case "apply_metadata_filter":
                     key = self.questions.ask_existing_key()
@@ -196,23 +202,23 @@
 
                     questions2 = Questions(vault=self.vault, key=key)
                     value = questions2.ask_existing_value(
                         question="Enter the value for the metadata filter",
                     )
                     if value is None:  # pragma: no cover
                         return
-                    if value == "":
+                    if not value:
                         self.filters.append(VaultFilter(key_filter=key))
                     else:
                         self.filters.append(VaultFilter(key_filter=key, value_filter=value))
                     self._load_vault()
 
                 case "apply_tag_filter":
                     tag = self.questions.ask_existing_inline_tag()
-                    if tag is None or tag == "":
+                    if tag is None or not tag:
                         return
 
                     self.filters.append(VaultFilter(tag_filter=tag))
                     self._load_vault()
 
                 case "list_filters":
                     if len(self.filters) == 0:
@@ -273,34 +279,102 @@
 
                 case "list_notes":
                     self.vault.list_editable_notes()
 
                 case _:
                     return
 
+    def application_import_csv(self) -> None:
+        """Import CSV for  bulk changes to metadata."""
+        alerts.usage(
+            "Import CSV to make build changes to metadata. The CSV must have the following columns: path, type, key, value. Where type is one of 'frontmatter', 'inline_metadata', or 'tag'. Note: this will not create new notes."
+        )
+
+        path = self.questions.ask_path(question="Enter path to a CSV file", valid_file=True)
+
+        if path is None:
+            return
+
+        csv_path = Path(path).expanduser()
+
+        if "csv" not in csv_path.suffix.lower():
+            alerts.error("File must be a CSV file")
+            return
+
+        note_paths = [
+            str(n.note_path.relative_to(self.vault.vault_path)) for n in self.vault.all_notes
+        ]
+
+        dict_from_csv = validate_csv_bulk_imports(csv_path, note_paths)
+        num_changed = self.vault.update_from_dict(dict_from_csv)
+
+        if num_changed == 0:
+            alerts.warning("No notes were changed")
+            return
+
+        alerts.success(f"Rewrote metadata for {num_changed} notes.")
+
+    def application_export_metadata(self) -> None:
+        """Export metadata to various formats."""
+        alerts.usage(
+            "Export the metadata in your vault. Note, uncommitted changes will be reflected in these files. The notes csv export can be used as template for importing bulk changes"
+        )
+        choices = [
+            questionary.Separator(),
+            {"name": "Metadata by type to CSV", "value": "export_csv"},
+            {"name": "Metadata by type to JSON", "value": "export_json"},
+            {
+                "name": "Metadata by note to CSV [Bulk import template]",
+                "value": "export_notes_csv",
+            },
+            questionary.Separator(),
+            {"name": "Back", "value": "back"},
+        ]
+        while True:
+            match self.questions.ask_selection(choices=choices, question="Export format"):
+                case "export_csv":
+                    path = self.questions.ask_path(question="Enter a path for the CSV file")
+                    if path is None:
+                        return
+                    self.vault.export_metadata(path=path, export_format="csv")
+                    alerts.success(f"CSV written to {path}")
+                case "export_json":
+                    path = self.questions.ask_path(question="Enter a path for the JSON file")
+                    if path is None:
+                        return
+                    self.vault.export_metadata(path=path, export_format="json")
+                    alerts.success(f"JSON written to {path}")
+                case "export_notes_csv":
+                    path = self.questions.ask_path(question="Enter a path for the CSV file")
+                    if path is None:
+                        return
+                    self.vault.export_notes_to_csv(path=path)
+                    alerts.success(f"CSV written to {path}")
+                    return
+                case _:
+                    return
+
     def application_inspect_metadata(self) -> None:
         """View metadata."""
         alerts.usage(
             "Inspect the metadata in your vault. Note, uncommitted changes will be reflected in these reports"
         )
 
         choices = [
+            questionary.Separator(),
             {"name": "View all frontmatter", "value": "all_frontmatter"},
             {"name": "View all inline metadata", "value": "all_inline"},
             {"name": "View all inline tags", "value": "all_tags"},
             {"name": "View all keys", "value": "all_keys"},
             {"name": "View all metadata", "value": "all_metadata"},
             questionary.Separator(),
-            {"name": "Write all metadata to CSV", "value": "export_csv"},
-            {"name": "Write all metadata to JSON file", "value": "export_json"},
-            questionary.Separator(),
             {"name": "Back", "value": "back"},
         ]
         while True:
-            match self.questions.ask_selection(choices=choices, question="Select a vault action"):
+            match self.questions.ask_selection(choices=choices, question="Select an action"):
                 case "all_metadata":
                     console.print("")
                     self.vault.metadata.print_metadata(area=MetadataType.ALL)
                     console.print("")
                 case "all_frontmatter":
                     console.print("")
                     self.vault.metadata.print_metadata(area=MetadataType.FRONTMATTER)
@@ -313,40 +387,29 @@
                     console.print("")
                     self.vault.metadata.print_metadata(area=MetadataType.KEYS)
                     console.print("")
                 case "all_tags":
                     console.print("")
                     self.vault.metadata.print_metadata(area=MetadataType.TAGS)
                     console.print("")
-                case "export_csv":
-                    path = self.questions.ask_path(question="Enter a path for the CSV file")
-                    if path is None:
-                        return
-                    self.vault.export_metadata(path=path, export_format="csv")
-                    alerts.success(f"Metadata written to {path}")
-                case "export_json":
-                    path = self.questions.ask_path(question="Enter a path for the JSON file")
-                    if path is None:
-                        return
-                    self.vault.export_metadata(path=path, export_format="json")
-                    alerts.success(f"Metadata written to {path}")
                 case _:
                     return
 
     def application_reorganize_metadata(self) -> None:
         """Reorganize metadata.
 
         This portion of the application deals with moving metadata between types (inline to frontmatter, etc.) and moving the location of inline metadata within a note.
 
         """
         alerts.usage("Move metadata within notes.")
         alerts.usage("    1. Transpose frontmatter to inline or vice versa.")
         alerts.usage("    2. Move the location of inline metadata within a note.")
 
         choices = [
+            questionary.Separator(),
             {"name": "Move inline metadata to top of note", "value": "move_to_top"},
             {
                 "name": "Move inline metadata beneath the first header",
                 "value": "move_to_after_header",
             },
             {"name": "Move inline metadata to bottom of the note", "value": "move_to_bottom"},
             {"name": "Transpose frontmatter to inline", "value": "frontmatter_to_inline"},
@@ -371,14 +434,15 @@
                 return
 
     def application_vault(self) -> None:
         """Vault actions."""
         alerts.usage("Create or delete a backup of your vault.")
 
         choices = [
+            questionary.Separator(),
             {"name": "Backup vault", "value": "backup_vault"},
             {"name": "Delete vault backup", "value": "delete_backup"},
             questionary.Separator(),
             {"name": "Back", "value": "back"},
         ]
 
         while True:
@@ -561,14 +625,15 @@
 
         if len(changed_notes) == 0:
             alerts.info("No changes to review.")
             return
 
         alerts.info(f"Found {len(changed_notes)} changed notes in the vault")
         choices: list[dict[str, Any] | questionary.Separator] = []
+        choices.append(questionary.Separator())
         for n, note in enumerate(changed_notes, start=1):
             _selection = {
                 "name": f"{n}: {note.note_path.relative_to(self.vault.vault_path)}",
                 "value": n - 1,
             }
             choices.append(_selection)
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/models/enums.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/models/enums.py`

 * *Files identical despite different names*

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/models/metadata.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/models/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
         return False
 
 
 class Frontmatter:
     """Representation of frontmatter metadata."""
 
-    def __init__(self, file_content: str):
+    def __init__(self, file_content: str) -> None:
         self.dict: dict[str, list[str]] = self._grab_note_frontmatter(file_content)
         self.dict_original: dict[str, list[str]] = copy.deepcopy(self.dict)
 
     def __repr__(self) -> str:  # pragma: no cover
         """Representation of the frontmatter.
 
         Returns:
@@ -241,14 +241,17 @@
         yaml = YAML(typ="safe")
         yaml.allow_unicode = False
         try:
             frontmatter: dict = yaml.load(frontmatter_block)
         except Exception as e:  # noqa: BLE001
             raise AttributeError(e) from e
 
+        if frontmatter is None or frontmatter == [None]:
+            return {}
+
         for k in frontmatter:
             if frontmatter[k] is None:
                 frontmatter[k] = []
 
         return dict_values_to_lists_strings(frontmatter, strip_null_values=True)
 
     def add(self, key: str, value: str | list[str] = None) -> bool:  # noqa: PLR0911
@@ -274,14 +277,15 @@
 
             self.dict[key] = [value]
             return True
 
         if key in self.dict and value not in self.dict[key]:
             if isinstance(value, list):
                 self.dict[key].extend(value)
+                self.dict[key] = list(sorted(set(self.dict[key])))
                 return True
 
             self.dict[key].append(value)
             return True
 
         return False
 
@@ -304,15 +308,15 @@
         Args:
             key (str): If no value, key to delete. If value, key containing the value.
             value_to_delete (str, optional): Value to delete.
 
         Returns:
             bool: True if a value was deleted
         """
-        new_dict = dict(self.dict)
+        new_dict = copy.deepcopy(self.dict)
 
         if value_to_delete is None:
             for _k in list(new_dict):
                 if re.search(key, _k):
                     del new_dict[_k]
         else:
             for _k, _v in new_dict.items():
@@ -322,14 +326,18 @@
 
         if new_dict != self.dict:
             self.dict = dict(new_dict)
             return True
 
         return False
 
+    def delete_all(self) -> None:
+        """Delete all Frontmatter from the note."""
+        self.dict = {}
+
     def has_changes(self) -> bool:
         """Check if the frontmatter has changes.
 
         Returns:
             bool: True if the frontmatter has changes.
         """
         return self.dict != self.dict_original
@@ -385,26 +393,50 @@
         string_stream.close()
         return yaml_value
 
 
 class InlineMetadata:
     """Representation of inline metadata in the form of `key:: value`."""
 
-    def __init__(self, file_content: str):
-        self.dict: dict[str, list[str]] = self.grab_inline_metadata(file_content)
+    def __init__(self, file_content: str) -> None:
+        self.dict: dict[str, list[str]] = self._grab_inline_metadata(file_content)
         self.dict_original: dict[str, list[str]] = copy.deepcopy(self.dict)
 
     def __repr__(self) -> str:  # pragma: no cover
         """Representation of inline metadata.
 
         Returns:
             str: inline metadata
         """
         return f"InlineMetadata(inline_metadata={self.dict})"
 
+    def _grab_inline_metadata(self, file_content: str) -> dict[str, list[str]]:
+        """Grab inline metadata from a note.
+
+        Returns:
+            dict[str, str]: Inline metadata from the note.
+        """
+        content = remove_markdown_sections(
+            file_content,
+            strip_codeblocks=True,
+            strip_inlinecode=True,
+            strip_frontmatter=True,
+        )
+        all_results = PATTERNS.find_inline_metadata.findall(content)
+        stripped_null_values = [tuple(filter(None, x)) for x in all_results]
+
+        inline_metadata: dict[str, list[str]] = {}
+        for k, v in stripped_null_values:
+            if k in inline_metadata:
+                inline_metadata[k].append(str(v))
+            else:
+                inline_metadata[k] = [str(v)]
+
+        return clean_dictionary(inline_metadata)
+
     def add(self, key: str, value: str | list[str] = None) -> bool:  # noqa: PLR0911
         """Add a key and value to the inline metadata.
 
         Args:
             key (str): Key to add.
             value (str, optional): Value to add.
 
@@ -424,14 +456,15 @@
 
             self.dict[key] = [value]
             return True
 
         if key in self.dict and value not in self.dict[key]:
             if isinstance(value, list):
                 self.dict[key].extend(value)
+                self.dict[key] = list(sorted(set(self.dict[key])))
                 return True
 
             self.dict[key].append(value)
             return True
 
         return False
 
@@ -472,38 +505,14 @@
 
         if new_dict != self.dict:
             self.dict = dict(new_dict)
             return True
 
         return False
 
-    def grab_inline_metadata(self, file_content: str) -> dict[str, list[str]]:
-        """Grab inline metadata from a note.
-
-        Returns:
-            dict[str, str]: Inline metadata from the note.
-        """
-        content = remove_markdown_sections(
-            file_content,
-            strip_codeblocks=True,
-            strip_inlinecode=True,
-            strip_frontmatter=True,
-        )
-        all_results = PATTERNS.find_inline_metadata.findall(content)
-        stripped_null_values = [tuple(filter(None, x)) for x in all_results]
-
-        inline_metadata: dict[str, list[str]] = {}
-        for k, v in stripped_null_values:
-            if k in inline_metadata:
-                inline_metadata[k].append(str(v))
-            else:
-                inline_metadata[k] = [str(v)]
-
-        return clean_dictionary(inline_metadata)
-
     def has_changes(self) -> bool:
         """Check if the metadata has changes.
 
         Returns:
             bool: True if the metadata has changes.
         """
         return self.dict != self.dict_original
@@ -531,15 +540,15 @@
 
         return False
 
 
 class InlineTags:
     """Representation of inline tags."""
 
-    def __init__(self, file_content: str):
+    def __init__(self, file_content: str) -> None:
         self.metadata_key = INLINE_TAG_KEY
         self.list: list[str] = self._grab_inline_tags(file_content)
         self.list_original: list[str] = self.list.copy()
 
     def __repr__(self) -> str:  # pragma: no cover
         """Representation of the inline tags.
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/models/notes.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/models/notes.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         dry_run (bool): Whether to run in dry-run mode.
         file_content (str): Total contents of the note file (frontmatter and content).
         frontmatter (dict): Frontmatter of the note.
         inline_tags (list): List of inline tags in the note.
         inline_metadata (dict): Dictionary of inline metadata in the note.
     """
 
-    def __init__(self, note_path: Path, dry_run: bool = False):
+    def __init__(self, note_path: Path, dry_run: bool = False) -> None:
         log.trace(f"Creating Note object for {note_path}")
         self.note_path: Path = Path(note_path)
         self.dry_run: bool = dry_run
 
         try:
             with self.note_path.open():
                 self.file_content: str = self.note_path.read_text()
@@ -142,15 +142,15 @@
         """
         p = self.note_path if path is None else path
         if self.dry_run:
             log.trace(f"DRY RUN: Writing note {p} to disk")
             return
 
         try:
-            with open(p, "w") as f:
+            with p.open(mode="w") as f:
                 log.trace(f"Writing note {p} to disk")
                 f.write(self.file_content)
         except FileNotFoundError as e:
             alerts.error(f"Note {p} not found. Exiting")
             raise typer.Exit(code=1) from e
 
     def contains_inline_tag(self, tag: str, is_regex: bool = False) -> bool:
@@ -186,14 +186,25 @@
         if self.frontmatter.contains(
             key, value, is_regex=is_regex
         ) or self.inline_metadata.contains(key, value, is_regex=is_regex):
             return True
 
         return False
 
+    def delete_all_metadata(self) -> None:
+        """Delete all metadata from the note. Removes all frontmatter and inline metadata and tags from the body of the note and from the associated metadata objects."""
+        for key in self.inline_metadata.dict:
+            self.delete_metadata(key=key, area=MetadataType.INLINE)
+
+        for tag in self.inline_tags.list:
+            self.delete_inline_tag(tag=tag)
+
+        self.frontmatter.delete_all()
+        self.write_frontmatter()
+
     def delete_inline_tag(self, tag: str) -> bool:
         """Delete an inline tag from the `inline_tags` attribute AND removes the tag from the text of the note if it exists.
 
         Args:
             tag (str): Tag to delete.
 
         Returns:
@@ -350,15 +361,15 @@
             is_regex (bool): Whether the pattern is a regex pattern or plain text.
         """
         if not is_regex:
             pattern = re.escape(pattern)
 
         self.file_content = re.sub(pattern, replacement, self.file_content, re.MULTILINE)
 
-    def transpose_metadata(  # noqa: C901, PLR0912, PLR0911, PLR0913
+    def transpose_metadata(  # noqa: C901, PLR0912, PLR0911
         self,
         begin: MetadataType,
         end: MetadataType,
         key: str = None,
         value: str | list[str] = None,
         location: InsertLocation = InsertLocation.BOTTOM,
     ) -> bool:
@@ -575,29 +586,29 @@
                 return True
             case InsertLocation.TOP:
                 try:
                     top = PATTERNS.frontmatter_block.search(self.file_content).group("frontmatter")
                 except AttributeError:
                     top = ""
 
-                if top == "":
+                if not top:
                     self.file_content = f"{new_string}\n{self.file_content}"
                     return True
 
                 new_string = f"{top}\n{new_string}"
                 top = re.escape(top)
                 self.sub(top, new_string, is_regex=True)
                 return True
             case InsertLocation.AFTER_TITLE:
                 try:
                     top = PATTERNS.top_with_header.search(self.file_content).group("top")
                 except AttributeError:
                     top = ""
 
-                if top == "":
+                if not top:
                     self.file_content = f"{new_string}\n{self.file_content}"
                     return True
 
                 new_string = f"{top}\n{new_string}"
                 top = re.escape(top)
                 self.sub(top, new_string, is_regex=True)
                 return True
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/models/patterns.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/models/patterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     find_inline_metadata: Pattern[str] = re.compile(
         r"""                                    # First look for in-text key values
         (?:^\[| \[)                             # Find key with starting bracket
         ([-_\w\d\/\*\u263a-\U0001f999]+?)::[ ]? # Find key
         (.*?)\]                                 # Find value until closing bracket
         |                                       # Else look for key values at start of line
-        (?:^|[^ \w\d]+| \[)                     # Any non-word or non-digit character
+        (?:^|[^ \w\d]+|^ *>?[-\d\|]?\.? )                     # Any non-word or non-digit character
         ([-_\w\d\/\*\u263a-\U0001f9995]+?)::(?!\n)(?:[ ](?!\n))?  # Capture the key if not a new line
         (.*?)$                                  # Capture the value
         """,
         re.X | re.MULTILINE,
     )
 
     frontmatter_block: Pattern[str] = re.compile(r"^\s*(?P<frontmatter>---.*?---)", flags=re.DOTALL)
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/models/questions.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/models/questions.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,31 @@
             bool | str: True if the number is valid, otherwise a string with the error message.
         """
         if not text.isdigit():
             return "Must be an integer"
 
         return True
 
+    def _validate_path_is_file(self, text: str) -> bool | str:
+        """Validate a path is a file.
+
+        Args:
+            text (str): The path to validate.
+
+        Returns:
+            bool | str: True if the path is valid, otherwise a string with the error message.
+        """
+        path_to_validate: Path = Path(text).expanduser().resolve()
+        if not path_to_validate.exists():
+            return f"Path does not exist: {path_to_validate}"
+        if not path_to_validate.is_file():
+            return f"Path is not a file: {path_to_validate}"
+
+        return True
+
     def _validate_valid_vault_regex(self, text: str) -> bool | str:
         """Validate a valid regex.
 
         Returns:
             bool | str: True if the regex is valid, otherwise a string with the error message.
         """
         try:
@@ -272,17 +289,19 @@
             str: The selected application.
         """
         return questionary.select(
             "What do you want to do?",
             choices=[
                 questionary.Separator("-------------------------------"),
                 {"name": "Vault Actions", "value": "vault_actions"},
+                {"name": "Export Metadata", "value": "export_metadata"},
                 {"name": "Inspect Metadata", "value": "inspect_metadata"},
                 {"name": "Filter Notes in Scope", "value": "filter_notes"},
                 questionary.Separator("-------------------------------"),
+                {"name": "Bulk changes from imported CSV", "value": "import_from_csv"},
                 {"name": "Add Metadata", "value": "add_metadata"},
                 {"name": "Delete Metadata", "value": "delete_metadata"},
                 {"name": "Rename Metadata", "value": "rename_metadata"},
                 {"name": "Reorganize Metadata", "value": "reorganize_metadata"},
                 questionary.Separator("-------------------------------"),
                 {"name": "Review Changes", "value": "review_changes"},
                 {"name": "Commit Changes", "value": "commit_changes"},
@@ -419,15 +438,15 @@
         """
         choices = []
         for metadata_location in InsertLocation:
             choices.append({"name": metadata_location.value, "value": metadata_location})
 
         return self.ask_selection(
             choices=choices,
-            question="Select the location for the metadata",
+            question=question,
         )
 
     def ask_new_key(self, question: str = "New key name") -> str:  # pragma: no cover
         """Ask the user for a new metadata key.
 
         Args:
             question (str, optional): The question to ask. Defaults to "New key name".
@@ -471,38 +490,49 @@
         Returns:
             int: A number.
         """
         return questionary.text(
             question, validate=self._validate_number, style=self.style, qmark="INPUT    |"
         ).ask()
 
-    def ask_path(self, question: str = "Enter a path") -> str:  # pragma: no cover
+    def ask_path(
+        self, question: str = "Enter a path", valid_file: bool = False
+    ) -> str:  # pragma: no cover
         """Ask the user for a path.
 
         Args:
             question (str, optional): The question to ask. Defaults to "Enter a path".
+            valid_file (bool, optional): Whether the path should be a valid file. Defaults to False.
 
         Returns:
             str: A path.
         """
+        if valid_file:
+            return questionary.path(
+                question,
+                only_directories=False,
+                style=self.style,
+                validate=self._validate_path_is_file,
+                qmark="INPUT    |",
+            ).ask()
+
         return questionary.path(question, style=self.style, qmark="INPUT    |").ask()
 
     def ask_selection(
         self, choices: list[Any], question: str = "Select an option"
     ) -> Any:  # pragma: no cover
         """Ask the user to select an item from a list.
 
         Args:
             question (str, optional): The question to ask. Defaults to "Select an option".
             choices (list[Any]): The list of choices.
 
         Returns:
             any: The selected item value.
         """
-        choices.insert(0, questionary.Separator())
         return questionary.select(
             question,
             choices=choices,
             use_shortcuts=False,
             style=self.style,
             qmark="INPUT    |",
         ).ask()
```

### Comparing `obsidian_metadata-0.8.0/src/obsidian_metadata/models/vault.py` & `obsidian_metadata-0.9.0/src/obsidian_metadata/models/vault.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import csv
 import json
 import re
 import shutil
 from dataclasses import dataclass
 from pathlib import Path
+from typing import Any
 
 import rich.repr
 import typer
 from rich import box
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.prompt import Confirm
 from rich.table import Table
@@ -43,15 +44,15 @@
     """
 
     def __init__(
         self,
         config: VaultConfig,
         dry_run: bool = False,
         filters: list[VaultFilter] = [],
-    ):
+    ) -> None:
         self.config = config.config
         self.vault_path: Path = config.path
         self.name = self.vault_path.name
         self.insert_location: InsertLocation = self._find_insert_location()
         self.dry_run: bool = dry_run
         self.backup_path: Path = self.vault_path.parent / f"{self.vault_path.name}.bak"
         self.metadata = VaultMetadata()
@@ -325,15 +326,15 @@
         export_file = Path(path).expanduser().resolve()
         if not export_file.parent.exists():
             alerts.error(f"Path does not exist: {export_file.parent}")
             raise typer.Exit(code=1)
 
         match export_format:
             case "csv":
-                with open(export_file, "w", encoding="UTF8") as f:
+                with export_file.open(mode="w", encoding="UTF8") as f:
                     writer = csv.writer(f)
                     writer.writerow(["Metadata Type", "Key", "Value"])
 
                     for key, value in self.metadata.frontmatter.items():
                         if isinstance(value, list):
                             if len(value) > 0:
                                 for v in value:
@@ -353,17 +354,55 @@
             case "json":
                 dict_to_dump = {
                     "frontmatter": self.metadata.dict,
                     "inline_metadata": self.metadata.inline_metadata,
                     "tags": self.metadata.tags,
                 }
 
-                with open(export_file, "w", encoding="UTF8") as f:
+                with export_file.open(mode="w", encoding="UTF8") as f:
                     json.dump(dict_to_dump, f, indent=4, ensure_ascii=False, sort_keys=True)
 
+    def export_notes_to_csv(self, path: str) -> None:
+        """Export notes and their associated metadata to a csv file. This is useful as a template for importing metadata changes to a vault.
+
+        Args:
+            path (str): Path to write csv file to.
+        """
+        export_file = Path(path).expanduser().resolve()
+        if not export_file.parent.exists():
+            alerts.error(f"Path does not exist: {export_file.parent}")
+            raise typer.Exit(code=1)
+
+        with export_file.open(mode="w", encoding="UTF8") as f:
+            writer = csv.writer(f)
+            writer.writerow(["path", "type", "key", "value"])
+
+            for _note in self.all_notes:
+                for key, value in _note.frontmatter.dict.items():
+                    for v in value:
+                        writer.writerow(
+                            [_note.note_path.relative_to(self.vault_path), "frontmatter", key, v]
+                        )
+
+                for key, value in _note.inline_metadata.dict.items():
+                    for v in value:
+                        writer.writerow(
+                            [
+                                _note.note_path.relative_to(self.vault_path),
+                                "inline_metadata",
+                                key,
+                                v,
+                            ]
+                        )
+
+                for tag in _note.inline_tags.list:
+                    writer.writerow(
+                        [_note.note_path.relative_to(self.vault_path), "tag", "", f"{tag}"]
+                    )
+
     def get_changed_notes(self) -> list[Note]:
         """Return a list of notes that have changes.
 
         Returns:
             list[Note]: List of notes that have changes.
         """
         changed_notes = []
@@ -467,15 +506,15 @@
                 num_changed += 1
 
         if num_changed > 0:
             self._rebuild_vault_metadata()
 
         return num_changed
 
-    def transpose_metadata(  # noqa: PLR0913
+    def transpose_metadata(
         self,
         begin: MetadataType,
         end: MetadataType,
         key: str = None,
         value: str | list[str] = None,
         location: InsertLocation = None,
     ) -> int:
@@ -506,7 +545,58 @@
                 num_changed += 1
                 log.trace(f"Transposed metadata in {_note.note_path}")
 
         if num_changed > 0:
             self._rebuild_vault_metadata()
 
         return num_changed
+
+    def update_from_dict(self, dictionary: dict[str, Any]) -> int:
+        """Update note metadata from a dictionary. This is a destructive operation. All metadata in the specified notes not in the dictionary will be removed.
+
+        Requires a dictionary with the note path as the key and a dictionary of metadata as the value.  Each key must have a list of associated dictionaries in the following format:
+
+            {
+                'type': 'frontmatter|inline_metadata|tag',
+                'key': 'string',
+                'value': 'string'
+            }
+
+        Args:
+            dictionary (dict[str, Any]): Dictionary to update metadata from.
+
+        Returns:
+            int: Number of notes that had metadata updated.
+        """
+        num_changed = 0
+
+        for _note in self.all_notes:
+            path = _note.note_path.relative_to(self.vault_path)
+            if str(path) in dictionary:
+                log.info(f"Updating metadata for '{path}'")
+                num_changed += 1
+                _note.delete_all_metadata()
+                for row in dictionary[str(path)]:
+                    if row["type"].lower() == "frontmatter":
+                        _note.add_metadata(
+                            area=MetadataType.FRONTMATTER, key=row["key"], value=row["value"]
+                        )
+
+                    if row["type"].lower() == "inline_metadata":
+                        _note.add_metadata(
+                            area=MetadataType.INLINE,
+                            key=row["key"],
+                            value=row["value"],
+                            location=self.insert_location,
+                        )
+
+                    if row["type"].lower() == "tag" or row["type"].lower() == "tags":
+                        _note.add_metadata(
+                            area=MetadataType.TAGS,
+                            value=row["value"],
+                            location=self.insert_location,
+                        )
+
+        if num_changed > 0:
+            self._rebuild_vault_metadata()
+
+        return num_changed
```

### Comparing `obsidian_metadata-0.8.0/PKG-INFO` & `obsidian_metadata-0.9.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: obsidian-metadata
-Version: 0.8.0
-Summary: Make batch updates to Obsidian metadata
-Home-page: https://github.com/natelandau/obsidian-metadata
-License: GNU AFFERO
-Keywords: obsidian
-Author: Nate Landau
-Author-email: github@natenate.org
-Requires-Python: >=3.10,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Requires-Dist: regex (>=2022.10.31,<2023.0.0)
-Requires-Dist: rich (>=13.3.2,<14.0.0)
-Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
-Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
-Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
-Project-URL: Repository, https://github.com/natelandau/obsidian-metadata
-Description-Content-Type: text/markdown
-
 [![PyPI version](https://badge.fury.io/py/obsidian-metadata.svg)](https://badge.fury.io/py/obsidian-metadata) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/obsidian-metadata) [![Python Code Checker](https://github.com/natelandau/obsidian-metadata/actions/workflows/automated-tests.yml/badge.svg)](https://github.com/natelandau/obsidian-metadata/actions/workflows/automated-tests.yml) [![codecov](https://codecov.io/gh/natelandau/obsidian-metadata/branch/main/graph/badge.svg?token=3F2R43SSX4)](https://codecov.io/gh/natelandau/obsidian-metadata)
 
 # obsidian-metadata
 
 A script to make batch updates to metadata in an Obsidian vault. No changes are
 made to the Vault until they are explicitly committed.
 
@@ -64,30 +39,37 @@
 Once installed, run `obsidian-metadata` in your terminal to enter an interactive menu of sub-commands.
 
 **Vault Actions**
 
 -   Backup: Create a backup of the vault.
 -   Delete Backup: Delete a backup of the vault.
 
+**Export Metadata**
+
+-   Export all metadata to a CSV organized by metadata type
+-   Export all metadata to a CSV organized by note path
+-   Export all metadata to a JSON file organized by metadata type
+
 **Inspect Metadata**
 
 -   **View all metadata in the vault**
 -   View all **frontmatter**
 -   View all **inline metadata**
 -   View all **inline tags**
--   **Export all metadata to CSV or JSON file**
 
 **Filter Notes in Scope**: Limit the scope of notes to be processed with one or more filters.
 
 -   **Path filter (regex)**: Limit scope based on the path or filename
 -   **Metadata filter**: Limit scope based on a key or key/value pair
 -   **Tag filter**: Limit scope based on an in-text tag
 -   **List and clear filters**: List all current filters and clear one or all
 -   **List notes in scope**: List notes that will be processed.
 
+**Bulk Edit Metadata** from a CSV file (See the _making bulk edits_ section below)
+
 **Add Metadata**: Add new metadata to your vault.
 
 When adding a new key to inline metadata, the `insert location` value in the config file will specify where in the note it will be inserted.
 
 -   **Add new metadata to the frontmatter**
 -   **Add new inline metadata** - Set `insert_location` in the config to control where the new metadata is inserted. (Default: Bottom)
 -   **Add new inline tag** - Set `insert_location` in the config to control where the new tag is inserted. (Default: Bottom)
@@ -153,14 +135,44 @@
     path = "/path/to/second_vault"
     exclude_paths = [".git", ".obsidian", "daily_notes"]
     insert_location = "AFTER_TITLE"
 ```
 
 To bypass the configuration file and specify a vault to use at runtime use the `--vault-path` option.
 
+### Making bulk edits
+
+Bulk edits are supported by importing a CSV file containing the following columns. Column headers must be lowercase.
+
+1. `path` - Path to note relative to the vault root folder
+2. `type` - Type of metadata. One of `frontmatter`, `inline_metadata`, or `tag`
+3. `key` - The key to add (leave blank for a tag)
+4. `value` - the value to add to the key
+
+An example valid CSV file is
+
+```csv
+path,type,key,value
+folder 1/note1.md,frontmatter,fruits,apple
+folder 1/note1.md,frontmatter,fruits,banana
+folder 1/note1.md,inline_metadata,cars,toyota
+folder 1/note1.md,inline_metadata,cars,honda
+folder 1/note1.md,tag,,tag1
+folder 1/note1.md,tag,,tag2
+```
+
+How bulk imports work:
+
+-   Only notes which match the path in the CSV file are updated
+-   Effected notes will have ALL of their metadata changed to reflect the values in the CSV file
+-   Existing metadata in an effected note will be rewritten. This may result in it's location and/or formatting within the note being changed
+-   inline tags ignore any value added to the `key` column
+
+You can export all your notes with their associated metadata in this format from the "Export Metadata" section of the script to be used as a template for your bulk changes.
+
 # Contributing
 
 ## Setup: Once per project
 
 There are two ways to contribute to this project.
 
 ### 1. Containerized development
@@ -185,7 +197,10 @@
 -   Run `poe` from within the development environment to print a list of [Poe the Poet](https://github.com/nat-n/poethepoet) tasks available to run on this project. Common commands:
     -   `poe lint` runs all linters
     -   `poe test` runs all tests with Pytest
 -   Run `poetry add {package}` from within the development environment to install a run time dependency and add it to `pyproject.toml` and `poetry.lock`.
 -   Run `poetry remove {package}` from within the development environment to uninstall a run time dependency and remove it from `pyproject.toml` and `poetry.lock`.
 -   Run `poetry update` from within the development environment to upgrade all dependencies to the latest versions allowed by `pyproject.toml`.
 
+```
+
+```
```

