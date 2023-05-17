# Comparing `tmp/typed_settings-23.0.0.tar.gz` & `tmp/typed_settings-23.0.1.tar.gz`

## Comparing `typed_settings-23.0.0.tar` & `typed_settings-23.0.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/Makefile
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/apiref.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/changelog.md
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/conf.py
--rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/conftest.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/development.rst
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples.rst
--rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/getting-started.rst
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/index.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/license.md
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/why.md
--rw-r--r--   0        0        0   366071 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/1password-test-dark.png
--rw-r--r--   0        0        0   351000 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/1password-test-light.png
--rw-r--r--   0        0        0   387873 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/cli-argparse-dark.png
--rw-r--r--   0        0        0   361129 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/cli-argparse-light.png
--rw-r--r--   0        0        0   596177 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/cli-click-dark.png
--rw-r--r--   0        0        0   562046 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/cli-click-light.png
--rw-r--r--   0        0        0   394639 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/cli-rich_click-dark.png
--rw-r--r--   0        0        0   373242 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/cli-rich_click-light.png
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/custom.css
--rw-r--r--   0        0        0    33208 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/typed-settings-spacing.svg
--rw-r--r--   0        0        0    36882 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/typed-settings.png
--rw-r--r--   0        0        0    24668 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/_static/typed-settings.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/black-pyproject.toml/black.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/black-pyproject.toml/pyproject.toml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/black-pyproject.toml/test.console
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/pypirc_0/pypirc.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/pypirc_0/pypirc_0.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/pypirc_0/test.console
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/pypirc_1/pypirc.toml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/pypirc_1/pypirc_1.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/pypirc_1/test.console
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/pytest-plugins/pytest.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/pytest-plugins/test.console
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/python-gitlab/python-gitlab.toml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/python-gitlab/python_gitlab.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/examples/python-gitlab/test.console
--rw-r--r--   0        0        0    29386 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/guides/cli.rst
--rw-r--r--   0        0        0    37110 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/guides/core.rst
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 typed_settings-23.0.0/docs/guides/index.rst
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/_compat.py
--rw-r--r--   0        0        0     8502 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/_core.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/_file_utils.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/_onepassword.py
--rw-r--r--   0        0        0    20647 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/argparse_utils.py
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/cli_utils.py
--rw-r--r--   0        0        0    20264 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/click_utils.py
--rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/converters.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/dict_utils.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/exceptions.py
--rw-r--r--   0        0        0    15499 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/loaders.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/mypy.py
--rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/processors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/py.typed
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/types.py
--rw-r--r--   0        0        0    13465 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/attrs/__init__.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 typed_settings-23.0.0/src/typed_settings/attrs/hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_api.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_argparse.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_attrs.py
--rw-r--r--   0        0        0    25161 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_cli_param_types.py
--rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_cli_utils.py
--rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_click.py
--rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_converters.py
--rw-r--r--   0        0        0    14911 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_core.py
--rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_dict_utils.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_file_utils.py
--rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_hooks.py
--rw-r--r--   0        0        0    18060 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_loaders.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_onepassword.py
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_processors.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_readme.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 typed_settings-23.0.0/tests/test_types.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 typed_settings-23.0.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 typed_settings-23.0.0/LICENSE
--rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 typed_settings-23.0.0/README.md
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 typed_settings-23.0.0/pyproject.toml
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 typed_settings-23.0.0/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/Makefile
+-rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/apiref.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/changelog.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/conf.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/conftest.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/development.rst
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples.rst
+-rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/getting-started.rst
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/index.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/license.md
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/why.md
+-rw-r--r--   0        0        0   366071 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/1password-test-dark.png
+-rw-r--r--   0        0        0   351000 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/1password-test-light.png
+-rw-r--r--   0        0        0   387873 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/cli-argparse-dark.png
+-rw-r--r--   0        0        0   361129 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/cli-argparse-light.png
+-rw-r--r--   0        0        0   596177 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/cli-click-dark.png
+-rw-r--r--   0        0        0   562046 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/cli-click-light.png
+-rw-r--r--   0        0        0   394639 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/cli-rich_click-dark.png
+-rw-r--r--   0        0        0   373242 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/cli-rich_click-light.png
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/custom.css
+-rw-r--r--   0        0        0    33208 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/typed-settings-spacing.svg
+-rw-r--r--   0        0        0    36882 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/typed-settings.png
+-rw-r--r--   0        0        0    24668 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/_static/typed-settings.svg
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/black-pyproject.toml/black.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/black-pyproject.toml/pyproject.toml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/black-pyproject.toml/test.console
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/pypirc_0/pypirc.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/pypirc_0/pypirc_0.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/pypirc_0/test.console
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/pypirc_1/pypirc.toml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/pypirc_1/pypirc_1.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/pypirc_1/test.console
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/pytest-plugins/pytest.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/pytest-plugins/test.console
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/python-gitlab/python-gitlab.toml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/python-gitlab/python_gitlab.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/examples/python-gitlab/test.console
+-rw-r--r--   0        0        0    29386 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/guides/cli.rst
+-rw-r--r--   0        0        0    37110 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/guides/core.rst
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 typed_settings-23.0.1/docs/guides/index.rst
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/_compat.py
+-rw-r--r--   0        0        0     8502 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/_core.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/_file_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/_onepassword.py
+-rw-r--r--   0        0        0    20647 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/argparse_utils.py
+-rw-r--r--   0        0        0    15009 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/cli_utils.py
+-rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/click_utils.py
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/converters.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/dict_utils.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/exceptions.py
+-rw-r--r--   0        0        0    15499 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/loaders.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/mypy.py
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/processors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/py.typed
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/types.py
+-rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/attrs/__init__.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 typed_settings-23.0.1/src/typed_settings/attrs/hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_api.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_argparse.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_attrs.py
+-rw-r--r--   0        0        0    25161 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_cli_param_types.py
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_cli_utils.py
+-rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_click.py
+-rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_converters.py
+-rw-r--r--   0        0        0    14911 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_core.py
+-rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_dict_utils.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_file_utils.py
+-rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_hooks.py
+-rw-r--r--   0        0        0    18060 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_loaders.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_onepassword.py
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_processors.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_readme.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 typed_settings-23.0.1/tests/test_types.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 typed_settings-23.0.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 typed_settings-23.0.1/LICENSE
+-rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 typed_settings-23.0.1/README.md
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 typed_settings-23.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 typed_settings-23.0.1/PKG-INFO
```

### Comparing `typed_settings-23.0.0/docs/Makefile` & `typed_settings-23.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/apiref.rst` & `typed_settings-23.0.1/docs/apiref.rst`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/conf.py` & `typed_settings-23.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/conftest.py` & `typed_settings-23.0.1/docs/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             else:
                 cmds[last_cmd].append(line)
 
         for cmd, output_lines in cmds.items():
             expected = "\n".join(output_lines)
             output = subprocess.run(
                 cmd,
-                shell=True,
+                shell=True,  # noqa: S602
                 cwd=self.path.parent,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
                 text=True,
                 check=True,
             ).stdout
             # Normalize whitespace:
```

### Comparing `typed_settings-23.0.0/docs/development.rst` & `typed_settings-23.0.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/examples.rst` & `typed_settings-23.0.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/getting-started.rst` & `typed_settings-23.0.1/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/index.rst` & `typed_settings-23.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/why.md` & `typed_settings-23.0.1/docs/why.md`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/1password-test-dark.png` & `typed_settings-23.0.1/docs/_static/1password-test-dark.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/1password-test-light.png` & `typed_settings-23.0.1/docs/_static/1password-test-light.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/cli-argparse-dark.png` & `typed_settings-23.0.1/docs/_static/cli-argparse-dark.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/cli-argparse-light.png` & `typed_settings-23.0.1/docs/_static/cli-argparse-light.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/cli-click-dark.png` & `typed_settings-23.0.1/docs/_static/cli-click-dark.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/cli-click-light.png` & `typed_settings-23.0.1/docs/_static/cli-click-light.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/cli-rich_click-dark.png` & `typed_settings-23.0.1/docs/_static/cli-rich_click-dark.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/cli-rich_click-light.png` & `typed_settings-23.0.1/docs/_static/cli-rich_click-light.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/custom.css` & `typed_settings-23.0.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/typed-settings-spacing.svg` & `typed_settings-23.0.1/docs/_static/typed-settings-spacing.svg`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/typed-settings.png` & `typed_settings-23.0.1/docs/_static/typed-settings.png`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/_static/typed-settings.svg` & `typed_settings-23.0.1/docs/_static/typed-settings.svg`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/examples/black-pyproject.toml/black.py` & `typed_settings-23.0.1/docs/examples/black-pyproject.toml/black.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/examples/black-pyproject.toml/test.console` & `typed_settings-23.0.1/docs/examples/black-pyproject.toml/test.console`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/examples/pytest-plugins/pytest.py` & `typed_settings-23.0.1/docs/examples/pytest-plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/examples/pytest-plugins/test.console` & `typed_settings-23.0.1/docs/examples/pytest-plugins/test.console`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/examples/python-gitlab/python_gitlab.py` & `typed_settings-23.0.1/docs/examples/python-gitlab/python_gitlab.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/guides/cli.rst` & `typed_settings-23.0.1/docs/guides/cli.rst`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/docs/guides/core.rst` & `typed_settings-23.0.1/docs/guides/core.rst`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/__init__.py` & `typed_settings-23.0.1/src/typed_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/_compat.py` & `typed_settings-23.0.1/src/typed_settings/_compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 
     from typing_extensions import (  # type: ignore
         Final,
         Protocol,
         runtime_checkable,
     )
 
-    def get_origin(tp: Any) -> Optional[Any]:
+    def get_origin(tp: Any) -> Optional[Any]:  # type: ignore[no-redef]
         # Backported from py38
         if isinstance(tp, _GenericAlias):
             return tp.__origin__
         if tp is Generic:  # pragma: no cover
             return Generic
         return None
 
-    def get_args(tp: Any) -> Tuple[Any, ...]:
+    def get_args(tp: Any) -> Tuple[Any, ...]:  # type: ignore[no-redef]
         # Backported from py38
         if isinstance(tp, _GenericAlias) and not tp._special:
             res = tp.__args__
             if (  # pragma: no cover
                 get_origin(tp) is collections.abc.Callable
                 and res[0] is not Ellipsis  # noqa: W503
             ):
```

### Comparing `typed_settings-23.0.0/src/typed_settings/_core.py` & `typed_settings-23.0.1/src/typed_settings/_core.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/_file_utils.py` & `typed_settings-23.0.1/src/typed_settings/_file_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/_onepassword.py` & `typed_settings-23.0.1/src/typed_settings/_onepassword.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Raise:
         ValueError: If the CLI is not properly installed or the invocation
             failed.
     """
     cmd = ("op",) + args
     try:
         result = subprocess.run(  # noqa: S603
-            cmd, capture_output=True, text=True, check=True
+            cmd, capture_output=True, text=True, check=True  # noqa: S603
         )
     except FileNotFoundError:
         raise ValueError(
             "The 1Password CLI is not properly installed.  You can find help "
             "here: https://developer.1password.com/docs/cli/"
         ) from None
     except subprocess.CalledProcessError as e:
```

### Comparing `typed_settings-23.0.0/src/typed_settings/argparse_utils.py` & `typed_settings-23.0.1/src/typed_settings/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/cli_utils.py` & `typed_settings-23.0.1/src/typed_settings/cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,74 +122,74 @@
             given type.
         """
         ...
 
     def handle_tuple(
         self,
         type_args_maker: "TypeArgsMaker",
-        args: Tuple[Any, ...],
+        types: Tuple[Any, ...],
         default: Optional[Tuple],
         is_optional: bool,
     ) -> StrDict:
         """
         Handle options for structured tuples (i.e., not list-like tuples).
 
         Args:
             type_args_maker: The :class:`TypeArgsMaker` that called this
                 function.
-            args: The types of all tuple items.
+            types: The types of all tuple items.
             default: Either a tuple of default values or ``None``.
             is_optional: Whether or not the option type was marked as option
                 or not.
 
         Return:
             A dictionary with keyword arguments for creating an option for the
             tuple.
         """
         ...
 
     def handle_collection(
         self,
         type_args_maker: "TypeArgsMaker",
-        args: Tuple[Any, ...],
+        types: Tuple[Any, ...],
         default: Optional[List[Any]],
         is_optional: bool,
     ) -> StrDict:
         """
         Handle collections, add options to allow multiple values and to
         collect them in a list/collection.
 
         Args:
             type_args_maker: The :class:`TypeArgsMaker` that called this
                 function.
-            args: The types of the list items.
+            types: The types of the list items.
             default: Either a collection of default values or ``None``.
             is_optional: Whether or not the option type was marked as option
                 or not.
 
         Return:
             A dictionary with keyword arguments for creating an option for the
             list type.
         """
         ...
 
     def handle_mapping(
         self,
         type_args_maker: "TypeArgsMaker",
-        args: Tuple[Any, ...],
+        types: Tuple[Any, ...],
         default: Default,
         is_optional: bool,
     ) -> StrDict:
         """
         Handle dictionaries.
 
         Args:
             type_args_maker: The :class:`TypeArgsMaker` that called this
                 function.
-            args: The types of keys and values.
+            types: The types of keys and values.
             default: Either a mapping of default values, ``None`` or
                 :data:`attrs.NOTHING`.
             is_optional: Whether or not the option type was marked as option
                 or not.
 
         Return:
             A dictionary with keyword arguments for creating an option for the
@@ -327,29 +327,30 @@
         """
         if len(args) == 2 and args[1] == ...:
             # "Immutable list" variant of tuple
             return self._handle_collection(type, args, default, is_optional)
 
         # "struct" variant of tuple
 
+        default_val: Optional[Tuple]
         if isinstance(default, tuple):
             if not len(default) == len(args):
                 raise TypeError(
                     f"Default value must be of len {len(args)}: {len(default)}"
                 )
             kwargs = {"strict": True} if PY_310 else {}
-            default = tuple(
+            default_val = tuple(
                 self.get_kwargs(a, d)["default"]
                 for a, d in zip(args, default, **kwargs)  # noqa: B905
             )
         else:
-            default = None
+            default_val = None
 
         kwargs = self.type_handler.handle_tuple(
-            self, args, default, is_optional
+            self, args, default_val, is_optional
         )
         return kwargs
 
     def _handle_collection(
         self,
         type: type,
         args: Tuple[Any, ...],
```

### Comparing `typed_settings-23.0.0/src/typed_settings/click_utils.py` & `typed_settings-23.0.1/src/typed_settings/click_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
        ``TypeArgsMaker``.
     .. versionchanged:: 23.0.0
        Made *converter*, *type_args_maker*, *argname*, and *decorator_factory*
        a keyword-only argument
     .. versionchanged:: 23.0.0
        Added the *processors* argument
     """
-    cls = attrs.resolve_types(settings_cls)
+    cls = attrs.resolve_types(settings_cls)  # type: ignore[type-var]
     options = [opt for opt in deep_options(cls) if opt.field.init is not False]
     grouped_options = group_options(cls, options)
 
     if isinstance(loaders, str):
         loaders = default_loaders(loaders)
 
     env_loader: Optional[EnvLoader] = None
```

### Comparing `typed_settings-23.0.0/src/typed_settings/converters.py` & `typed_settings-23.0.1/src/typed_settings/converters.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/dict_utils.py` & `typed_settings-23.0.1/src/typed_settings/dict_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         *path* is a dot (``.``) separted path to the attribute, e.g.
         ``"parent_attr.child_attr.grand_child_attr``.
 
     Raises:
         NameError: if the type annotations can not be resolved.  This is, e.g.,
           the case when recursive classes are being used.
     """
-    cls = attrs.resolve_types(cls)
+    cls = attrs.resolve_types(cls)  # type: ignore[type-var]
     result = []
 
     def iter_attribs(r_cls: type, prefix: str) -> None:
         for field in attrs.fields(r_cls):
             if field.type is not None and attrs.has(field.type):
                 iter_attribs(field.type, f"{prefix}{field.name}.")
             else:
```

### Comparing `typed_settings-23.0.0/src/typed_settings/exceptions.py` & `typed_settings-23.0.1/src/typed_settings/exceptions.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/loaders.py` & `typed_settings-23.0.1/src/typed_settings/loaders.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/mypy.py` & `typed_settings-23.0.1/src/typed_settings/mypy.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/processors.py` & `typed_settings-23.0.1/src/typed_settings/processors.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/src/typed_settings/types.py` & `typed_settings-23.0.1/src/typed_settings/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 Internal data structures.
 """
 from collections.abc import Collection
 from enum import Enum
-from typing import Any, ClassVar, Dict, Generic, List, Type, TypeVar
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    List,
+    Type,
+    TypeVar,
+)
 
 import attrs
 
-from ._compat import Final, Protocol, runtime_checkable
+from ._compat import Final
 
 
 SECRET_REPR: Final[str] = "*******"
 
 
-# A protocol to be able to statically accept an attrs class.
-# Copied from attrs b/c they only have this in their *.pyi file.
-@runtime_checkable
-class AttrsInstance(Protocol):
-    __attrs_attrs__: ClassVar[Any]
-
-
 T = TypeVar("T")
 ET = TypeVar("ET", bound=Enum)  # Enum type
-ST = TypeVar("ST", bound=AttrsInstance)  # SettingsInstance
-SettingsClass = Type[AttrsInstance]
-SettingsInstance = AttrsInstance
+ST = TypeVar("ST", bound=attrs.AttrsInstance)  # SettingsInstance
+SettingsClass = Type[attrs.AttrsInstance]
+SettingsInstance = attrs.AttrsInstance
 SettingsDict = Dict[str, Any]
 
 
 class _Auto:
     """
     Sentinel class to indicate the lack of a value when ``None`` is ambiguous.
```

### Comparing `typed_settings-23.0.0/src/typed_settings/attrs/__init__.py` & `typed_settings-23.0.1/src/typed_settings/attrs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     Type,
     overload,
 )
 
 import attr  # The old namespaces is needed in "combine()"
 import attrs
 
-from .._compat import PY_38
-from ..types import SECRET_REPR, AttrsInstance
+from ..types import SECRET_REPR
 from .hooks import auto_convert
 
 
 if TYPE_CHECKING:
     from attr import (
         _T,
         _ConverterType,
@@ -41,16 +40,14 @@
     "settings",
 ]
 
 METADATA_KEY = "typed_settings"
 CLICK_KEY = "click"
 ARGPARSE_KEY = "argparse"
 
-AttrsClass = Type[AttrsInstance]
-
 
 class _SecretRepr:
     def __call__(self, v: Any) -> str:
         return repr(v if not v and isinstance(v, Collection) else SECRET_REPR)
 
     def __repr__(self) -> str:
         return "***"
@@ -362,15 +359,15 @@
     ts_meta = metadata.setdefault(METADATA_KEY, {})
     ts_meta["help"] = help
     ts_meta[CLICK_KEY] = click_config
     ts_meta[ARGPARSE_KEY] = argparse_config
     return metadata
 
 
-def evolve(inst: "AttrsInstance", **changes: Any) -> "AttrsInstance":
+def evolve(inst: attrs.AttrsInstance, **changes: Any) -> attrs.AttrsInstance:
     """
     Create a new instance, based on *inst* with *changes* applied.
 
     If the old value of an attribute is an ``attrs`` class and the new value
     is a dict, the old value is updated recursively.
 
     .. warning::
@@ -402,24 +399,24 @@
         init_name = attr_name if attr_name[0] != "_" else attr_name[1:]
         old_value = getattr(inst, attr_name)
         if init_name not in changes:
             # Add original value to changes
             changes[init_name] = old_value
         elif attrs.has(old_value) and isinstance(changes[init_name], Mapping):
             # Evolve nested attrs classes
-            if PY_38:
-                assert isinstance(old_value, AttrsInstance)  # noqa: S101
             changes[init_name] = evolve(old_value, **changes[init_name])  # type: ignore[arg-type]  # noqa
 
     return cls(**changes)
 
 
 def combine(
-    name: str, base_cls: "AttrsClass", nested: Dict[str, "AttrsInstance"]
-) -> "AttrsClass":
+    name: str,
+    base_cls: Type[attrs.AttrsInstance],
+    nested: Dict[str, attrs.AttrsInstance],
+) -> Type[attrs.AttrsInstance]:
     """
     Create a new class called *name* based on *base_class* with additional
     attributes for *nested* classes.
 
     The same effect can be achieved by manually composing settings classes.
     A use case for this method is to combine settings classes from dynamically
     loaded plugins with the base settings of the main program.
```

### Comparing `typed_settings-23.0.0/src/typed_settings/attrs/hooks.py` & `typed_settings-23.0.1/src/typed_settings/attrs/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def auto_convert(
         cls: SettingsClass, attribs: List["Attribute[Any]"]
     ) -> List["Attribute[Any]"]:
         """
         A field transformer that tries to convert all attribs of a class to
         their annotated type.
         """
-        attrs.resolve_types(cls, attribs=attribs)
+        attrs.resolve_types(cls, attribs=attribs)  # type: ignore[type-var]
         results = []
         for attrib in attribs:
             # Do not override explicitly defined converters!
             if attrib.converter is None:
                 c = partial(converter.structure, cl=attrib.type)
                 attrib = attrib.evolve(converter=c)
             results.append(attrib)
```

### Comparing `typed_settings-23.0.0/tests/conftest.py` & `typed_settings-23.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_api.py` & `typed_settings-23.0.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_argparse.py` & `typed_settings-23.0.1/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_attrs.py` & `typed_settings-23.0.1/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_cli_param_types.py` & `typed_settings-23.0.1/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_cli_utils.py` & `typed_settings-23.0.1/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_click.py` & `typed_settings-23.0.1/tests/test_click.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_converters.py` & `typed_settings-23.0.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_core.py` & `typed_settings-23.0.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_dict_utils.py` & `typed_settings-23.0.1/tests/test_dict_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,31 +5,26 @@
 
 from typed_settings import dict_utils as du
 from typed_settings.types import OptionInfo
 
 
 def mkattr(name: str, typ: type) -> attrs.Attribute:
     """Creates an Attribute with *name* and *type*."""
-    try:
-        return attrs.Attribute(  # type: ignore
-            name,
-            attrs.NOTHING,
-            None,
-            True,
-            None,
-            None,
-            True,
-            False,
-            type=typ,
-            alias=name,
-        )
-    except TypeError:
-        return attrs.Attribute(  # type: ignore
-            name, attrs.NOTHING, None, True, None, None, True, False, type=typ
-        )
+    return attrs.Attribute(  # type: ignore
+        name,
+        attrs.NOTHING,
+        None,
+        True,
+        None,
+        None,
+        True,
+        False,
+        type=typ,
+        alias=name,
+    )
 
 
 class TestDeepOptions:
     """Tests for deep_options()."""
 
     def test_deep_options(self) -> None:
         @attrs.define
```

### Comparing `typed_settings-23.0.0/tests/test_file_utils.py` & `typed_settings-23.0.1/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_hooks.py` & `typed_settings-23.0.1/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_loaders.py` & `typed_settings-23.0.1/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_onepassword.py` & `typed_settings-23.0.1/tests/test_onepassword.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_processors.py` & `typed_settings-23.0.1/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/tests/test_readme.py` & `typed_settings-23.0.1/tests/test_readme.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """
     All commands in the *console* block of an example produce the exact same
     results as shown in the example.
     """
     for cmd, expected in example.items():  # pragma: no-cover
         result = subprocess.run(
             cmd,
-            shell=True,
+            shell=True,  # noqa: S602
             cwd=str(tmp_path),
             capture_output=True,
             text=True,
             check=False,
         )
         assert result.stderr == ""
         assert result.stdout.splitlines() == expected
```

### Comparing `typed_settings-23.0.0/tests/test_types.py` & `typed_settings-23.0.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/LICENSE` & `typed_settings-23.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/README.md` & `typed_settings-23.0.1/README.md`

 * *Files identical despite different names*

### Comparing `typed_settings-23.0.0/pyproject.toml` & `typed_settings-23.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "typed-settings"
-version = "23.0.0"
+version = "23.0.1"
 description = "Typed settings based on attrs classes"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
 authors = [
     { name = "Stefan Scherfke", email = "stefan@sofa-rockers.org" },
 ]
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "attrs>=22.1",
+    "attrs>=23.1",
     "cattrs>=22.2",
     "tomli>=2; python_version<'3.11'",
 ]
 
 [project.optional-dependencies]
 click = [
     "click>=7,<9",
```

### Comparing `typed_settings-23.0.0/PKG-INFO` & `typed_settings-23.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-settings
-Version: 23.0.0
+Version: 23.0.1
 Summary: Typed settings based on attrs classes
 Project-URL: Homepage, https://gitlab.com/sscherfke/typed-settings
 Project-URL: Documentation, https://typed-settings.readthedocs.io
 Project-URL: Changelog, https://typed-settings.readthedocs.io/en/latest/changelog.html
 Project-URL: Bug Tracker, https://gitlab.com/sscherfke/typed-settings/-/issues
 Project-URL: Source Code, https://gitlab.com/sscherfke/typed-settings
 Author-email: Stefan Scherfke <stefan@sofa-rockers.org>
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: attrs>=22.1
+Requires-Dist: attrs>=23.1
 Requires-Dist: cattrs>=22.2
 Requires-Dist: tomli>=2; python_version < '3.11'
 Provides-Extra: all
 Requires-Dist: typed-settings[click,jinja,option-groups]; extra == 'all'
 Provides-Extra: click
 Requires-Dist: click<9,>=7; extra == 'click'
 Provides-Extra: dev
```

