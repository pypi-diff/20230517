# Comparing `tmp/ddqa-0.1.0.tar.gz` & `tmp/ddqa-0.2.0.tar.gz`

## Comparing `ddqa-0.1.0.tar` & `ddqa-0.2.0.tar`

### file list

```diff
@@ -1,111 +1,108 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.1.0/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.1.0/.linkcheckerrc
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ddqa-0.1.0/HISTORY.md
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 ddqa-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 ddqa-0.1.0/app/pyoxidizer.bzl
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/index.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/install.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/.snippets/links.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/assets/css/custom.css
--rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/assets/images/logo.svg
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/config/repo.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/config/user.md
--rw-r--r--   0        0        0   193753 2020-02-02 00:00:00.000000 ddqa-0.1.0/screenshots/config.PNG
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/py.typed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/app/__init__.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/app/core.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/app/style.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/__init__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/edit.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/explore.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/find.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/restore.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/show.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/create/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/status/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/sync/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/__init__.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/constants.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/core.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/file.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/utils.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/data/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/data/logo.png
--rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/data/shame.png
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/github.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/jira.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/app.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/auth.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/repo.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/team.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/configure.py
--rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/create.py
--rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/status.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/ci.py
--rw-r--r--   0        0        0    25498 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/clipboard.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/errors.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/fs.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/git.py
--rw-r--r--   0        0        0     9054 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/github.py
--rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/jira.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/network.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/structures.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/time.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/toml.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/widgets.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/widgets/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/widgets/input.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/widgets/layout.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/widgets/static.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/create/__init__.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/create/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/sync/__init__.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/sync/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/helpers/api.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/__init__.py
--rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/test_configure.py
--rw-r--r--   0        0        0    34644 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/test_status.py
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_fs.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_git.py
--rw-r--r--   0        0        0    22414 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_github.py
--rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_jira.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_structures.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_time.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.1.0/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.1.0/README.md
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 ddqa-0.1.0/hatch.toml
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 ddqa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 ddqa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.2.0/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.2.0/.linkcheckerrc
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ddqa-0.2.0/HISTORY.md
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 ddqa-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 ddqa-0.2.0/pyoxidizer.bzl
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0    12674 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/install.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/.snippets/links.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/config/repo.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/config/user.md
+-rw-r--r--   0        0        0   193753 2020-02-02 00:00:00.000000 ddqa-0.2.0/screenshots/config.PNG
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/py.typed
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/app/__init__.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/app/core.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/app/style.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/__init__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/edit.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/explore.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/find.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/restore.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/show.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/create/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/status/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/sync/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/__init__.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/constants.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/core.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/file.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/utils.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/data/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/data/logo.png
+-rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/data/shame.png
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/github.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/jira.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/app.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/auth.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/repo.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/team.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/configure.py
+-rw-r--r--   0        0        0    15706 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/create.py
+-rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/status.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/ci.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/errors.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/fs.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/git.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/github.py
+-rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/jira.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/network.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/structures.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/time.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/widgets.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/widgets/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/widgets/input.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/widgets/layout.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/widgets/static.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/create/__init__.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/create/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/sync/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/sync/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/__init__.py
+-rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/test_configure.py
+-rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/test_status.py
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0    22924 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_github.py
+-rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_jira.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_time.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ddqa-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.2.0/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 ddqa-0.2.0/hatch.toml
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ddqa-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 ddqa-0.2.0/PKG-INFO
```

### Comparing `ddqa-0.1.0/mkdocs.yml` & `ddqa-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/.github/workflows/docs.yml` & `ddqa-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/.github/workflows/publish-docs.yml` & `ddqa-0.2.0/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/.github/workflows/test.yml` & `ddqa-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/docs/index.md` & `ddqa-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/docs/assets/css/custom.css` & `ddqa-0.2.0/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/docs/assets/images/favicon.ico` & `ddqa-0.2.0/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/docs/assets/images/logo.svg` & `ddqa-0.2.0/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/docs/config/repo.md` & `ddqa-0.2.0/docs/config/repo.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,7 +45,8 @@
 
 - `github_team` (***required***) - This is the team's GitHub name, excluding the organization `<ORG>/` prefix
 - `jira_project` (***required***) - This is the team's Jira project in which issues will be created. If there exists an issue `FOO-123`, the project name is `FOO`.
 - `jira_issue_type` (***required***) - This is the type of Jira issue that will be created and will most often be `Task`. The issue type can be found as the `fields.issuetype.name` returned value in the payload from the [`/rest/api/2/issue/{issueIdOrKey}`](https://developer.atlassian.com/cloud/jira/platform/rest/v2/api-group-issues/#api-rest-api-2-issue-issueidorkey-get) endpoint.
 - `jira_statuses` (***required***) - This is an array of Jira statuses that map to the top-level `qa_statuses` option. Alternatively, this may be a mapping of QA statuses to Jira statuses. The available Jira statuses may be found using the [`/rest/api/2/project/{projectIdOrKey}/statuses`](https://developer.atlassian.com/cloud/jira/platform/rest/v2/api-group-projects/#api-rest-api-2-project-projectidorkey-statuses-get) endpoint.
 - `github_labels` - This team will be assigned by default to any pull requests that are labeled with any of the entries (as long as the pull request has no labels that match any of those defined in the top-level `ignored_labels` option)
 - `jira_component` - This is the name of a Jira [project component](https://support.atlassian.com/jira-software-cloud/docs/organize-work-with-components/) with which to create issues
+- `exclude_members` - This is an array of members who should be excluded from QA participation
```

### Comparing `ddqa-0.1.0/docs/config/user.md` & `ddqa-0.2.0/docs/config/user.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/screenshots/config.PNG` & `ddqa-0.2.0/screenshots/config.PNG`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/app/core.py` & `ddqa-0.2.0/src/ddqa/app/core.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/cli/__init__.py` & `ddqa-0.2.0/src/ddqa/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
 import os
-import sys
 
 import click
 
 from ddqa._version import __version__
 from ddqa.cli.config import config
 from ddqa.cli.create import create
 from ddqa.cli.status import status
@@ -93,14 +92,10 @@
 
 def main():  # no cov
     try:
         return ddqa(prog_name='ddqa', windows_expand_args=False)
     except Exception:
         from rich.console import Console
 
-        suppressed_modules = []
-        if not getattr(sys, 'frozen', False):
-            suppressed_modules.append(click)
-
         console = Console()
-        console.print_exception(suppress=suppressed_modules)
+        console.print_exception(suppress=[click])
         return 1
```

### Comparing `ddqa-0.1.0/src/ddqa/cli/config/__init__.py` & `ddqa-0.2.0/src/ddqa/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/cli/config/show.py` & `ddqa-0.2.0/src/ddqa/cli/config/show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/cli/create/__init__.py` & `ddqa-0.2.0/src/ddqa/cli/create/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/cli/status/__init__.py` & `ddqa-0.2.0/src/ddqa/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/config/core.py` & `ddqa-0.2.0/src/ddqa/config/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
 import os
+import tomllib
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
 
 from ddqa.utils.fs import Path
-from ddqa.utils.toml import load_toml_data
 
 if TYPE_CHECKING:
     from ddqa.models.config.app import AppConfig
     from ddqa.models.config.auth import AuthConfig
     from ddqa.models.config.repo import RepoConfig
 
 
@@ -53,15 +53,15 @@
             repo_data = dict(original_repo_data)
             repo_config_file = (
                 Path(repo_data['path']) / '.ddqa' / 'config.toml'
                 if 'path' in repo_data and isinstance(repo_data['path'], str) and Path(repo_data['path']).is_dir()
                 else default_repo_config_file
             )
             if repo_config_file.is_file():
-                for key, value in load_toml_data(repo_config_file.read_text()).items():
+                for key, value in tomllib.loads(repo_config_file.read_text()).items():
                     repo_data.setdefault(key, value)
 
             if (
                 'global_config_source' in repo_data
                 and isinstance(repo_data['global_config_source'], str)
                 and not repo_data['global_config_source'].startswith('http')
             ):
```

### Comparing `ddqa-0.1.0/src/ddqa/config/file.py` & `ddqa-0.2.0/src/ddqa/config/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
+import tomllib
 from typing import cast
 
 from ddqa.config.core import Config
 from ddqa.config.utils import scrub_config
 from ddqa.utils.fs import Path
-from ddqa.utils.toml import load_toml_data
 
 
 class ConfigFile:
     def __init__(self, path: Path | None = None):
         self.path: Path = path or self.get_default_location()
         self.model = cast(Config, None)
 
@@ -22,23 +22,23 @@
         if not content:
             content = tomli_w.dumps(self.model.data)
 
         self.path.parent.ensure_dir_exists()
         self.path.write_atomic(content, 'w', encoding='utf-8')
 
     def load(self):
-        self.model = Config(load_toml_data(self.read()))
+        self.model = Config(tomllib.loads(self.read()))
 
     def read(self) -> str:
         return self.path.read_text()
 
     def read_scrubbed(self) -> str:
         import tomli_w
 
-        config = Config(load_toml_data(self.read()))
+        config = Config(tomllib.loads(self.read()))
         scrub_config(config.data)
 
         return tomli_w.dumps(config.data)
 
     def restore(self):
         import tomli_w
```

### Comparing `ddqa-0.1.0/src/ddqa/data/logo.png` & `ddqa-0.2.0/src/ddqa/data/logo.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/data/shame.png` & `ddqa-0.2.0/src/ddqa/data/shame.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/models/github.py` & `ddqa-0.2.0/src/ddqa/models/github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/models/jira.py` & `ddqa-0.2.0/src/ddqa/models/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/models/config/repo.py` & `ddqa-0.2.0/src/ddqa/models/config/repo.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/screens/configure.py` & `ddqa-0.2.0/src/ddqa/screens/configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/screens/create.py` & `ddqa-0.2.0/src/ddqa/screens/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
 import typing
+from collections import defaultdict
 
 from rich.markdown import Markdown as RichMarkdown
 from rich.markup import escape
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Container, HorizontalScroll, VerticalScroll
 from textual.screen import Screen
@@ -123,16 +124,14 @@
             self.sidebar.status.update(f'{self.previous_ref} -> {self.current_ref}')
             return
 
         self.app.print('Finished processing candidates')
         self.sidebar.update_assignment_status()
 
     async def create(self) -> None:
-        import secrets
-
         candidates: dict[int, Candidate] = {}
         for candidate in self.candidates.values():
             if candidate.assigned:
                 candidates[len(candidates)] = candidate
 
         self.candidates.clear()
         self.candidates.update(candidates)
@@ -143,29 +142,30 @@
         # Reset rows
         for index, candidate in self.candidates.items():
             self.add_row('', escape(candidate.data.title), key=str(index))
 
         self.focus()
         display_updated = False
 
+        assignment_counts: dict[str, dict[str, int]] = defaultdict(lambda: defaultdict(int))
+
         self.app.print(f'Candidates ready for creation: {total}')
         self.sidebar.status.update('Creating...')
         async with ResponsiveNetworkClient(self.sidebar.status) as client:
             for index, candidate in self.candidates.items():
                 self.app.print(f'Creating issue for {candidate.data.long_display()}')
 
                 assignments: dict[str, str] = {}
                 for team, assigned in candidate.assignments.items():
                     if not assigned:
                         continue
 
-                    potential_assignees = await self.__get_potential_assignees(
-                        client, candidate.data, self.app.repo.teams[team]
+                    assignments[team] = await self.__get_assignee(
+                        client, candidate.data, self.app.repo.teams[team], assignment_counts
                     )
-                    assignments[team] = secrets.choice(sorted(potential_assignees)) if potential_assignees else ''
 
                 try:
                     created_issues = await self.app.jira.create_issues(client, candidate.data, self.labels, assignments)
                 except Exception as e:
                     self.sidebar.status.update(escape(str(e)))
                     return
 
@@ -190,32 +190,45 @@
                 if not display_updated:
                     display_updated = True
 
         self.app.print('Finished creating issues')
         self.sidebar.status.update('Finished')
         self.sidebar.button.disabled = False
 
-    async def __get_potential_assignees(
-        self, client: ResponsiveNetworkClient, candidate: TestCandidate, team: TeamConfig
-    ) -> set:
+    async def __get_assignee(
+        self,
+        client: ResponsiveNetworkClient,
+        candidate: TestCandidate,
+        team: TeamConfig,
+        assignment_counts: dict[str, dict[str, int]],
+    ) -> str:
+        import secrets
+
         team_members = await self.app.github.get_team_members(client, team.github_team)
         if not team_members:
-            return team_members
+            return ''
 
         team_members.discard(candidate.user)
         team_members.difference_update(team.exclude_members)
         if not team_members:
-            return {candidate.user}
+            return candidate.user
+
+        counts = assignment_counts[team.github_team]
+        reviewers = {reviewer.name for reviewer in candidate.reviewers}
+        member_keys = {member: (counts[member], member in reviewers) for member in team_members}
+
+        priorities: dict[tuple[int, bool], list[str]] = defaultdict(list)
+        for member, key in member_keys.items():
+            priorities[key].append(member)
 
-        team_member_reviewers = {reviewer.name for reviewer in candidate.reviewers if reviewer.name in team_members}
-        if len(team_member_reviewers) == len(team_members):
-            return team_member_reviewers
+        potential_assignees = priorities[sorted(priorities)[0]]
+        assignee = secrets.choice(sorted(potential_assignees))
+        counts[assignee] += 1
 
-        team_members -= team_member_reviewers
-        return team_members
+        return assignee
 
 
 class CandidateSidebar(LabeledBox):
     DEFAULT_CSS = """
     #sidebar-status {
         height: auto;
         border-bottom: dashed #632CA6;
```

### Comparing `ddqa-0.1.0/src/ddqa/screens/status.py` & `ddqa-0.2.0/src/ddqa/screens/status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/screens/sync.py` & `ddqa-0.2.0/src/ddqa/screens/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
+import tomllib
+
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Container
 from textual.screen import Screen
 from textual.widget import Widget
 from textual.widgets import Button, Header, Label, TextLog
 
 from ddqa.utils.network import ResponsiveNetworkClient
-from ddqa.utils.toml import load_toml_data
 from ddqa.widgets.static import Placeholder
 
 
 class InteractiveSidebar(Widget):
     DEFAULT_CSS = """
     InteractiveSidebar > Label {
         width: 100%;
@@ -58,15 +59,15 @@
                 )
                 response.raise_for_status()
             except Exception as e:
                 status.update(str(e))
                 return
 
             try:
-                global_config = load_toml_data(response.text)
+                global_config = tomllib.loads(response.text)
             except Exception:
                 status.update('Unable to parse TOML source')
                 return
 
             if not global_config:
                 status.update('No members found in TOML source')
                 return
```

### Comparing `ddqa-0.1.0/src/ddqa/utils/fs.py` & `ddqa-0.2.0/src/ddqa/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/utils/git.py` & `ddqa-0.2.0/src/ddqa/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/utils/github.py` & `ddqa-0.2.0/src/ddqa/utils/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,17 @@
         directory = self.cache_dir / self.org / self.repo_name / 'team_members'
         directory.ensure_dir_exists()
         return directory
 
     @cached_property
     def repo_id(self) -> str:
         # https://github.com/foo/bar.git -> foo/bar
-        return self.repo.get_remote_url().split('github.com/', 1)[1].removesuffix('.git')
+        # or username@github.com:foo/bar.git -> foo/bar
+        repo = self.repo.get_remote_url().split('github.com', 1)[1]
+        return repo[1:].removesuffix('.git')
 
     @cached_property
     def org(self) -> str:
         return self.repo_id.partition('/')[0]
 
     @cached_property
     def repo_name(self) -> str:
```

### Comparing `ddqa-0.1.0/src/ddqa/utils/jira.py` & `ddqa-0.2.0/src/ddqa/utils/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/utils/network.py` & `ddqa-0.2.0/src/ddqa/utils/network.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/utils/structures.py` & `ddqa-0.2.0/src/ddqa/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/utils/time.py` & `ddqa-0.2.0/src/ddqa/utils/time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/widgets/input.py` & `ddqa-0.2.0/src/ddqa/widgets/input.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/widgets/layout.py` & `ddqa-0.2.0/src/ddqa/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/src/ddqa/widgets/static.py` & `ddqa-0.2.0/src/ddqa/widgets/static.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/conftest.py` & `ddqa-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/cli/config/test_find.py` & `ddqa-0.2.0/tests/cli/config/test_restore.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
-import os
-
-import pytest
-
-from ddqa.config.constants import ConfigEnvVars
-
-
-def test_copy(ddqa, config_file, mocker):
-    mock = mocker.patch('ddqa.utils.clipboard.copy')
-    result = ddqa('config', 'find', '-c')
-
-    assert result.exit_code == 0, result.output
-    mock.assert_called_once_with(str(config_file.path))
-
-
-def test_pipe_to_editor(ddqa, config_file, helpers):
-    config_file.path = config_file.path.parent / 'a space' / 'config.toml'
-    config_file.path.parent.ensure_dir_exists()
-    config_file.restore()
-    os.environ[ConfigEnvVars.CONFIG] = str(config_file.path)
+def test_standard(ddqa, config_file, helpers):
+    config_file.model.data.update({'repo': 'foo'})
+    config_file.save()
 
-    result = ddqa('config', 'find')
+    result = ddqa('config', 'restore')
 
     assert result.exit_code == 0, result.output
     assert result.output == helpers.dedent(
-        f"""
-        "{config_file.path}"
+        """
+        Settings were successfully restored.
         """,
         terminal=True,
     )
 
+    config_file.load()
+    assert not config_file.model.app.repo
 
-def test_standard(ddqa, config_file, helpers):
-    config_path = str(config_file.path)
-    if ' ' in config_path:  # no cov
-        pytest.xfail('Path to system temporary directory contains spaces')
 
-    result = ddqa('config', 'find')
+def test_allow_invalid_config(ddqa, config_file, helpers):
+    config_file.save(
+        helpers.dedent(
+            """
+            repo = [""]
+            """
+        )
+    )
+
+    result = ddqa('config', 'restore')
 
     assert result.exit_code == 0, result.output
     assert result.output == helpers.dedent(
-        f"""
-        {config_path}
+        """
+        Settings were successfully restored.
         """,
         terminal=True,
     )
```

### Comparing `ddqa-0.1.0/tests/cli/config/test_show.py` & `ddqa-0.2.0/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/cli/create/test_create.py` & `ddqa-0.2.0/tests/cli/create/test_create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/cli/status/test_status.py` & `ddqa-0.2.0/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/cli/sync/test_sync.py` & `ddqa-0.2.0/tests/cli/sync/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/helpers/api.py` & `ddqa-0.2.0/tests/helpers/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,44 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
+from __future__ import annotations
+
 import re
 from textwrap import dedent as _dedent
 
 import pytest
 from rich.console import Console
 
 # The default time to wait for all triggered events to complete
 ASYNC_WAIT = 0.5
 
+_initial_value = object()
+
+
+class MutatingEqualityValue:
+    def __init__(self, initial=_initial_value):
+        self.value = initial
+
+    def inverse(self):
+        return InverseEqualityValue(self)
+
+    def __eq__(self, other):
+        original = self.value
+        self.value = other
+        return original is _initial_value or original == other
+
+
+class InverseEqualityValue:
+    def __init__(self, value: MutatingEqualityValue):
+        self.value = value
+
+    def __eq__(self, other):
+        return self.value.value != other
+
 
 def dedent(text, *, terminal=False):
     text = _dedent(text[1:])
     if terminal:
         return text
 
     return text[:-1]
```

### Comparing `ddqa-0.1.0/tests/screens/test_configure.py` & `ddqa-0.2.0/tests/screens/test_configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/screens/test_create.py` & `ddqa-0.2.0/tests/screens/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -757,22 +757,27 @@
             await app.workers.wait_for_complete()
             await pilot.pause(helpers.ASYNC_WAIT)
 
             assert str(sidebar.status.render()) == 'Finished'
             assert str(sidebar.label.render()) == f' {num_candidates} / {num_candidates} '
             assert str(sidebar.button.label) == 'Exit'
 
+            # We use the following equality assertions as a way to match the progression of member assignment counts and
+            # remain agnostic to the random assignment
+            foo_team_value = helpers.MutatingEqualityValue(initial='jira-foo6')
+            bar_team_value = helpers.MutatingEqualityValue()
+
             assert response_mock.call_args_list == [
                 mocker.call(
                     'POST',
                     'https://foobarbaz.atlassian.net/rest/api/2/issue',
                     auth=('foo@bar.baz', 'bar'),
                     json={
                         'fields': {
-                            'assignee': {'id': 'jira-foo6'},
+                            'assignee': {'id': foo_team_value},
                             'description': helpers.dedent(
                                 """
                                 Pull request: [#2|https://github.com/org/repo/pull/2]
                                 Author: [github-foo1|https://github.com/github-foo1]
                                 Labels: {{foo-label}}
 
                                 foo2
@@ -788,15 +793,15 @@
                 ),
                 mocker.call(
                     'POST',
                     'https://foobarbaz.atlassian.net/rest/api/2/issue',
                     auth=('foo@bar.baz', 'bar'),
                     json={
                         'fields': {
-                            'assignee': {'id': mocker.ANY},
+                            'assignee': {'id': bar_team_value},
                             'description': helpers.dedent(
                                 """
                                 Commit: [hash3|https://github.com/org/repo/commit/hash3]
 
 
                                 """
                             ),
@@ -809,15 +814,15 @@
                 ),
                 mocker.call(
                     'POST',
                     'https://foobarbaz.atlassian.net/rest/api/2/issue',
                     auth=('foo@bar.baz', 'bar'),
                     json={
                         'fields': {
-                            'assignee': {'id': 'jira-foo6'},
+                            'assignee': {'id': foo_team_value.inverse()},
                             'description': helpers.dedent(
                                 """
                                 Pull request: [#1|https://github.com/org/repo/pull/1]
                                 Author: [github-bar1|https://github.com/github-bar1]
                                 Labels: {{foo-label}}, {{bar-label}}
 
                                 foo1
@@ -833,15 +838,15 @@
                 ),
                 mocker.call(
                     'POST',
                     'https://foobarbaz.atlassian.net/rest/api/2/issue',
                     auth=('foo@bar.baz', 'bar'),
                     json={
                         'fields': {
-                            'assignee': {'id': 'jira-bar6'},
+                            'assignee': {'id': bar_team_value.inverse()},
                             'description': helpers.dedent(
                                 """
                                 Pull request: [#1|https://github.com/org/repo/pull/1]
                                 Author: [github-bar1|https://github.com/github-bar1]
                                 Labels: {{foo-label}}, {{bar-label}}
 
                                 foo1
```

### Comparing `ddqa-0.1.0/tests/screens/test_sync.py` & `ddqa-0.2.0/tests/screens/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/utils/test_fs.py` & `ddqa-0.2.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/utils/test_git.py` & `ddqa-0.2.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/utils/test_github.py` & `ddqa-0.2.0/tests/utils/test_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,28 @@
 
 @pytest.fixture(scope='module', autouse=True)
 def mock_remote_url():
     with mock.patch('ddqa.utils.git.GitRepository.get_remote_url', return_value='https://github.com/org/repo.git'):
         yield
 
 
+@pytest.mark.parametrize(
+    'url, repo_id', [('https://github.com/foo/bar.git', 'foo/bar'), ('username@github.com:foo/bar.git', 'foo/bar')]
+)
+def test_repo_id(app, git_repository, url, repo_id):
+    app.configure(
+        git_repository,
+        caching=True,
+        data={'github': {'user': 'foo', 'token': 'bar'}, 'jira': {'email': 'foo@bar.baz', 'token': 'bar'}},
+    )
+
+    with mock.patch('ddqa.utils.git.GitRepository.get_remote_url', return_value=url):
+        assert app.github.repo_id == repo_id
+
+
 class TestCandidates:
     async def test_pr(self, app, git_repository, mocker):
         app.configure(
             git_repository,
             caching=True,
             data={'github': {'user': 'foo', 'token': 'bar'}, 'jira': {'email': 'foo@bar.baz', 'token': 'bar'}},
         )
```

### Comparing `ddqa-0.1.0/tests/utils/test_jira.py` & `ddqa-0.2.0/tests/utils/test_jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/utils/test_structures.py` & `ddqa-0.2.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/tests/utils/test_time.py` & `ddqa-0.2.0/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/LICENSE.txt` & `ddqa-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/README.md` & `ddqa-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.1.0/hatch.toml` & `ddqa-0.2.0/hatch.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [envs.default]
-python = "3.10"
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-asyncio",
   "pytest-mock",
 ]
 # pre-install-commands = [
@@ -17,25 +16,21 @@
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
-[[envs.all.matrix]]
-python = ["3.10"]
-
 [envs.lint]
 detached = true
-python = "3.11"
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "pydantic",
-  "ruff>=0.0.243",
+  "ruff<0.0.262",
 ]
 [envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/ddqa tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
@@ -74,31 +69,7 @@
 serve = "mkdocs serve --dev-addr localhost:8000 {args}"
 validate = "linkchecker --config .linkcheckerrc site"
 # https://github.com/linkchecker/linkchecker/issues/678
 build-check = [
   "build --no-directory-urls",
   "validate",
 ]
-
-[envs.build]
-detached = true
-dependencies = [
-  "pyoxidizer>=0.24.0",
-]
-
-[envs.build.env-vars]
-PIP_FIND_LINKS = "dist"
-
-[envs.build.scripts]
-_template = "pyoxidizer build --path app {args}"
-debug = [
-  "hatch build -t wheel",
-  "_template install",
-]
-release = [
-  "hatch build -t wheel",
-  "_template install --release",
-]
-msi = [
-  "hatch build -t wheel",
-  "_template msi --release",
-]
```

### Comparing `ddqa-0.1.0/pyproject.toml` & `ddqa-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 [build-system]
-requires = ["hatchling", "hatch-vcs"]
+requires = ["hatchling>=1.17.0", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ddqa"
 dynamic = ["version"]
 description = "Datadog's QA manager for releases of GitHub repositories"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 license = "MIT"
 keywords = [
   "datadog",
   "qa",
   "testing",
   "tooling",
 ]
 authors = [
   { name = "Datadog, Inc.", email = "dev@datadoghq.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
-  "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
   "click>=8.1.3",
   "httpx",
   "pillow",
   "platformdirs",
   "pydantic<2",
   "rich",
   "textual~=0.19.0",
   "textual-autocomplete>=2.1.0b0",
-  "tomli; python_version < '3.11'",
   "tomli-w",
 ]
 
 [project.urls]
 Source = "https://github.com/DataDog/ddqa"
 
 [project.scripts]
@@ -49,50 +47,40 @@
 source = "vcs"
 raw-options = { version_scheme = "python-simplified-semver", local_scheme = "no-local-version" }
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/ddqa/_version.py"
 
 [tool.black]
-target-version = ["py310"]
+target-version = ["py311"]
 line-length = 120
 skip-string-normalization = true
-extend-exclude = """
-src/ddqa/utils/clipboard.py
-"""
 
 [tool.mypy]
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 follow_imports = "normal"
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 warn_no_return = false
 warn_unused_ignores = true
 plugins = [
   "pydantic.mypy",
 ]
-exclude = [
-  "src/ddqa/utils/clipboard.py",
-]
-
-[[tool.mypy.overrides]]
-module = "ddqa.utils.clipboard"
-follow_imports = "skip"
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [tool.ruff]
-target-version = "py310"
+target-version = "py311"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -127,17 +115,14 @@
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
-extend-exclude = [
-  "src/ddqa/utils/clipboard.py",
-]
 
 [tool.ruff.isort]
 known-first-party = ["ddqa"]
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
```

### Comparing `ddqa-0.1.0/PKG-INFO` & `ddqa-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: ddqa
-Version: 0.1.0
+Version: 0.2.0
 Summary: Datadog's QA manager for releases of GitHub repositories
 Project-URL: Source, https://github.com/DataDog/ddqa
 Author-email: "Datadog, Inc." <dev@datadoghq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: datadog,qa,testing,tooling
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Requires-Dist: click>=8.1.3
 Requires-Dist: httpx
 Requires-Dist: pillow
 Requires-Dist: platformdirs
 Requires-Dist: pydantic<2
 Requires-Dist: rich
 Requires-Dist: textual-autocomplete>=2.1.0b0
 Requires-Dist: textual~=0.19.0
 Requires-Dist: tomli-w
-Requires-Dist: tomli; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # Datadog QA
 
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/DataDog/ddqa/actions/workflows/test.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/test.yml) [![CD - Build](https://github.com/DataDog/ddqa/actions/workflows/build.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/build.yml) |
```

