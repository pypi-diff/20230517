# Comparing `tmp/rockingester-2.2.3.tar.gz` & `tmp/rockingester-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-2.2.3.tar", last modified: Wed May 10 15:50:11 2023, max compression
+gzip compressed data, was "rockingester-2.3.0.tar", last modified: Wed May 17 17:46:18 2023, max compression
```

## Comparing `rockingester-2.2.3.tar` & `rockingester-2.3.0.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.588741 rockingester-2.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-10 15:49:50.000000 rockingester-2.2.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 15:49:50.000000 rockingester-2.2.3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.572741 rockingester-2.2.3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-10 15:49:50.000000 rockingester-2.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-10 15:49:50.000000 rockingester-2.2.3/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-10 15:49:50.000000 rockingester-2.2.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 15:49:50.000000 rockingester-2.2.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-10 15:49:50.000000 rockingester-2.2.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-10 15:49:50.000000 rockingester-2.2.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-10 15:49:50.000000 rockingester-2.2.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 15:49:50.000000 rockingester-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-10 15:50:11.588741 rockingester-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-10 15:49:50.000000 rockingester-2.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-10 15:49:50.000000 rockingester-2.2.3/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.572741 rockingester-2.2.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-10 15:49:50.000000 rockingester-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:50:11.588741 rockingester-2.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.572741 rockingester-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/direct_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.013771 rockingester-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 17:46:06.000000 rockingester-2.3.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-17 17:46:06.000000 rockingester-2.3.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-17 17:46:06.000000 rockingester-2.3.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:17.993770 rockingester-2.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-17 17:46:06.000000 rockingester-2.3.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-17 17:46:06.000000 rockingester-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-17 17:46:06.000000 rockingester-2.3.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-17 17:46:06.000000 rockingester-2.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 17:46:06.000000 rockingester-2.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-17 17:46:06.000000 rockingester-2.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 17:46:06.000000 rockingester-2.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-17 17:46:06.000000 rockingester-2.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 17:46:06.000000 rockingester-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-17 17:46:18.013771 rockingester-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-17 17:46:06.000000 rockingester-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-17 17:46:06.000000 rockingester-2.3.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:17.997770 rockingester-2.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.001771 rockingester-2.3.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 17:46:06.000000 rockingester-2.3.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-17 17:46:06.000000 rockingester-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:46:18.013771 rockingester-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:17.997770 rockingester-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.005771 rockingester-2.3.0/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 17:46:17.000000 rockingester-2.3.0/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17957 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/collectors/direct_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/src/rockingester_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 17:46:06.000000 rockingester-2.3.0/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:46:18.009771 rockingester-2.3.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-17 17:46:06.000000 rockingester-2.3.0/tests/test_platewait.py
```

### Comparing `rockingester-2.2.3/.dae-devops/Makefile` & `rockingester-2.3.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.dae-devops/docs/conventions.rst` & `rockingester-2.3.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.dae-devops/docs/developing.rst` & `rockingester-2.3.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.dae-devops/docs/devops.rst` & `rockingester-2.3.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.dae-devops/docs/docs_structure.rst` & `rockingester-2.3.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.dae-devops/docs/installing.rst` & `rockingester-2.3.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.dae-devops/docs/testing.rst` & `rockingester-2.3.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.dae-devops/project.yaml` & `rockingester-2.3.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.devcontainer/Dockerfile` & `rockingester-2.3.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.devcontainer/devcontainer.json` & `rockingester-2.3.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.github/CONTRIBUTING.rst` & `rockingester-2.3.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.github/actions/install_requirements/action.yml` & `rockingester-2.3.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.github/dependabot.yml` & `rockingester-2.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.github/pages/make_switcher.py` & `rockingester-2.3.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.github/workflows/code.yml` & `rockingester-2.3.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.github/workflows/docs.yml` & `rockingester-2.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.github/workflows/docs_clean.yml` & `rockingester-2.3.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.github/workflows/linkcheck.yml` & `rockingester-2.3.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.gitignore` & `rockingester-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.gitlab-ci.yml` & `rockingester-2.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/.vscode/launch.json` & `rockingester-2.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/LICENSE` & `rockingester-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/PKG-INFO` & `rockingester-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.2.3
+Version: 2.3.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.2.3/README.rst` & `rockingester-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/configurations/development.yaml` & `rockingester-2.3.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/docs/conf.py` & `rockingester-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/docs/images/dls-favicon.ico` & `rockingester-2.3.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/docs/images/dls-logo.svg` & `rockingester-2.3.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/docs/index.rst` & `rockingester-2.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/docs/user/explanations/25-docs-structure.rst` & `rockingester-2.3.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/docs/user/index.rst` & `rockingester-2.3.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/pyproject.toml` & `rockingester-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester.egg-info/PKG-INFO` & `rockingester-2.3.0/src/rockingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.2.3
+Version: 2.3.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.2.3/src/rockingester.egg-info/SOURCES.txt` & `rockingester-2.3.0/src/rockingester.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,9 +85,10 @@
 src/rockingester_lib/collectors/direct_poll.py
 src/rockingester_lib/contexts/__init__.py
 src/rockingester_lib/contexts/base.py
 tests/__init__.py
 tests/base.py
 tests/conftest.py
 tests/test_collector.py
+tests/test_platewait.py
 tests/configurations/direct_poll.yaml
 tests/configurations/service.yaml
```

### Comparing `rockingester-2.2.3/src/rockingester_api/collectors/aiohttp.py` & `rockingester-2.3.0/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_api/collectors/collectors.py` & `rockingester-2.3.0/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_api/collectors/context.py` & `rockingester-2.3.0/src/rockingester_api/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_api/context_base.py` & `rockingester-2.3.0/src/rockingester_api/context_base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_api/exceptions.py` & `rockingester-2.3.0/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_api/thing.py` & `rockingester-2.3.0/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_api/things.py` & `rockingester-2.3.0/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_cli/main.py` & `rockingester-2.3.0/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_cli/subcommands/base.py` & `rockingester-2.3.0/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_cli/subcommands/service.py` & `rockingester-2.3.0/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_cli/version.py` & `rockingester-2.3.0/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_lib/__main__.py` & `rockingester-2.3.0/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-2.3.0/src/rockingester_lib/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_lib/collectors/base.py` & `rockingester-2.3.0/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_lib/collectors/collectors.py` & `rockingester-2.3.0/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_lib/collectors/context.py` & `rockingester-2.3.0/src/rockingester_lib/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-2.3.0/src/rockingester_lib/collectors/direct_poll.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import logging
 import os
 import shutil
+import time
 from pathlib import Path
 from typing import Dict, List
 
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain2
 from dls_utilpack.require import require
 from dls_utilpack.visit import VisitNotFound, get_xchem_directory
@@ -67,14 +68,17 @@
         self.__visit_plates_subdirectory = Path(
             require(s, type_specific_tbd, "visit_plates_subdirectory")
         )
 
         # Explicit list of barcodes to process (used when testing a deployment).
         self.__ingest_only_barcodes = type_specific_tbd.get("ingest_only_barcodes")
 
+        # Maximum time to wait for final image to arrive, relative to time of last arrived image.
+        self.__max_wait_seconds = require(s, type_specific_tbd, "max_wait_seconds")
+
         # Database where we will get plate barcodes and add new wells.
         self.__xchembku_client_context = None
         self.__xchembku = None
 
         # This flag will stop the ticking async task.
         self.__keep_ticking = True
         self.__tick_future = None
@@ -314,31 +318,56 @@
             # Update the path stem in the crystal plate record.
             # TODO: Consider if important to report/record same barcodes on different rockmaker directories.
             crystal_plate_model.rockminer_collected_stem = plate_directory.stem
             await self.__xchembku.upsert_crystal_plates(
                 [crystal_plate_model], "update rockminer_collected_stem"
             )
 
-        # Get all the well images in the plate directory.
-        subwell_names = [
-            entry.name for entry in os.scandir(plate_directory) if entry.is_file()
-        ]
+        # Get all the well images in the plate directory and the latest arrival time.
+        subwell_names = []
+        max_wait_seconds = self.__max_wait_seconds
+        max_mtime = os.stat(plate_directory).st_mtime
+
+        with os.scandir(plate_directory) as entries:
+            for entry in entries:
+                subwell_names.append(entry.name)
+                max_mtime = max(max_mtime, entry.stat().st_mtime)
+
+        # TODO: Verify that time.time() where rockingester runs matches os.stat() on filesystem from which images are collected.
+        waited_seconds = time.time() - max_mtime
 
         # Make an object corresponding to the crystal plate model's type.
         crystal_plate_object = CrystalPlateObjects().build_object(
             {"type": crystal_plate_model.thing_type}
         )
 
-        # Don't handle the plate directory until all images have arrived.
-        # TODO: Put in some kind of failsafe in direct_poll.py to handle case where all the well images never arrive.
+        # Don't handle the plate directory until all images have arrived or some maximum wait has exceeded.
         if len(subwell_names) < crystal_plate_object.get_well_count():
+            if waited_seconds < max_wait_seconds:
+                logger.debug(
+                    f"[PLATEWAIT] waiting longer since found only {len(subwell_names)}"
+                    f" out of {crystal_plate_object.get_well_count()} subwell images"
+                    f" in {plate_directory}"
+                    f" after waiting {'%0.1f' % waited_seconds} out of {max_wait_seconds} seconds"
+                )
+                return
+            else:
+                logger.warning(
+                    f"[PLATEDONE] done waiting even though found only {len(subwell_names)}"
+                    f" out of {crystal_plate_object.get_well_count()} subwell images"
+                    f" in {plate_directory}"
+                    f" after waiting {'%0.1f' % waited_seconds} out of {max_wait_seconds} seconds"
+                )
+        else:
             logger.debug(
-                f"[PLATEWAIT] found only {len(subwell_names)} out of {crystal_plate_object.get_well_count()} subwell images in {plate_directory}"
+                f"[PLATEDONE] done waiting since found all {len(subwell_names)}"
+                f" out of {crystal_plate_object.get_well_count()} subwell images"
+                f" in {plate_directory}"
+                f" after waiting {'%0.1f' % waited_seconds} out of {max_wait_seconds} seconds"
             )
-            return
 
         # Sort wells by name so that tests are deterministic.
         subwell_names.sort()
 
         crystal_well_models: List[CrystalWellModel] = []
         for subwell_name in subwell_names:
             # Make the well model, including image width/height.
```

### Comparing `rockingester-2.2.3/src/rockingester_lib/contexts/base.py` & `rockingester-2.3.0/src/rockingester_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_lib/exceptions.py` & `rockingester-2.3.0/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/src/rockingester_lib/version.py` & `rockingester-2.3.0/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/tests/base.py` & `rockingester-2.3.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/tests/configurations/direct_poll.yaml` & `rockingester-2.3.0/tests/configurations/direct_poll.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 # The rockingester direct access.
 rockingester_collector_specification:
     type: "rockingester_lib.collectors.direct_poll"
     type_specific_tbd:
         plates_directories:
             - "${output_directory}/SubwellImages"
+        max_wait_seconds: 3.0
         visits_directory: *VISITS_DIRECTORY
         visit_plates_subdirectory: *VISIT_PLATES_SUBDIRECTORY
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
         ingest_only_barcodes:
             - 98ab
             - 98ac
             - 98ad
```

### Comparing `rockingester-2.2.3/tests/configurations/service.yaml` & `rockingester-2.3.0/tests/configurations/service.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 # The rockingester direct access.
 rockingester_collector_specification_direct_poll:
     &ROCKINGESTER_COLLECTOR_SPECIFICATION_DIRECT_POLL
     type: "rockingester_lib.collectors.direct_poll"
     type_specific_tbd:
         plates_directories:
             - "${output_directory}/SubwellImages"
+        max_wait_seconds: 3.0
         visits_directory: *VISITS_DIRECTORY
         visit_plates_subdirectory: *VISIT_PLATES_SUBDIRECTORY
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
         ingest_only_barcodes:
             - 98ab
             - 98ac
             - 98ad
```

### Comparing `rockingester-2.2.3/tests/conftest.py` & `rockingester-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.3/tests/test_collector.py` & `rockingester-2.3.0/tests/test_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         First it starts the xchembku and collector and loads a single plate barcode into the database.
 
         Then, while the collector thread is running, it creates some scrapable images.
 
         The test then waits a while for the scraping to be done, and verifies the outputs.
 
-        These are in 3 barcodes.  The first matches the barcode in the database, so it gets scraped.
+        These are 4 barcodes.  The first matches the barcode in the database, so it gets scraped.
         The second matches no barcode in the database, so it is ignored.
         The third matches a barcode, but the visit is improperly formatted, so it is ignored.
         The fourth barcode is not scraped because it is not configured in the ingest_only_barcodes list.
         """
 
         # Get the multiconf from the testing configuration yaml.
         multiconf = self.get_multiconf()
```

