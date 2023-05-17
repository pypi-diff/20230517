# Comparing `tmp/safir-4.1.0.tar.gz` & `tmp/safir-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safir-4.1.0.tar", last modified: Mon May  8 18:06:39 2023, max compression
+gzip compressed data, was "safir-4.2.1.tar", last modified: Wed May 17 20:28:46 2023, max compression
```

## Comparing `safir-4.1.0.tar` & `safir-4.2.1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.485432 safir-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 18:06:21.000000 safir-4.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-08 18:06:21.000000 safir-4.1.0/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 18:06:21.000000 safir-4.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 18:06:21.000000 safir-4.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-08 18:06:21.000000 safir-4.1.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-08 18:06:21.000000 safir-4.1.0/.github/workflows/periodic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-08 18:06:21.000000 safir-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 18:06:21.000000 safir-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-05-08 18:06:21.000000 safir-4.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-08 18:06:21.000000 safir-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 18:06:21.000000 safir-4.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-08 18:06:39.485432 safir-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-08 18:06:21.000000 safir-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-08 18:06:21.000000 safir-4.1.0/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 18:06:21.000000 safir-4.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-05-08 18:06:21.000000 safir-4.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 18:06:21.000000 safir-4.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-08 18:06:21.000000 safir-4.1.0/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-08 18:06:21.000000 safir-4.1.0/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-08 18:06:21.000000 safir-4.1.0/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-08 18:06:21.000000 safir-4.1.0/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-08 18:06:21.000000 safir-4.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/arq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/fastapi-errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/gafaelfawr.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/gcs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.473431 safir-4.1.0/docs/user-guide/github-apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/api-resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/create-a-github-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/handling-webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/webhook-models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/http-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/ivoa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/kubernetes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/pydantic-redis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/pydantic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/set-up-from-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/slack-webhook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/uvicorn.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/x-forwarded.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-08 18:06:21.000000 safir-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:06:39.485432 safir-4.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.465431 safir-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.473431 safir-4.1.0/src/safir/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/db_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/gafaelfawr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/github/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/github/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/github/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/github/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/middleware/ivoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/middleware/x_forwarded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/slack/blockkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/slack/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49522 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.473431 safir-4.1.0/src/safir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.481431 safir-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 18:06:21.000000 safir-4.1.0/tests/asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 18:06:21.000000 safir-4.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-08 18:06:21.000000 safir-4.1.0/tests/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-08 18:06:21.000000 safir-4.1.0/tests/datetime_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.481431 safir-4.1.0/tests/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/arq_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/db_session_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/gafaelfawr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/http_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/logger_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-08 18:06:21.000000 safir-4.1.0/tests/fastapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 18:06:21.000000 safir-4.1.0/tests/gcs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.481431 safir-4.1.0/tests/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.465431 safir-4.1.0/tests/github/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.481431 safir-4.1.0/tests/github/data/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/check_run_created.json
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/check_suite_completed.json
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/installation.json
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/installation_repositories.json
--rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/pull_request_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/push_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/webhooks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-08 18:06:21.000000 safir-4.1.0/tests/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-05-08 18:06:21.000000 safir-4.1.0/tests/logging_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-08 18:06:21.000000 safir-4.1.0/tests/metadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.485432 safir-4.1.0/tests/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-08 18:06:21.000000 safir-4.1.0/tests/middleware/ivoa_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-08 18:06:21.000000 safir-4.1.0/tests/middleware/x_forwarded_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-08 18:06:21.000000 safir-4.1.0/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-08 18:06:21.000000 safir-4.1.0/tests/pydantic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-08 18:06:21.000000 safir-4.1.0/tests/redis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-08 18:06:21.000000 safir-4.1.0/tests/safir_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.485432 safir-4.1.0/tests/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-08 18:06:21.000000 safir-4.1.0/tests/slack/blockkit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-08 18:06:21.000000 safir-4.1.0/tests/slack/webhook_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.485432 safir-4.1.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-08 18:06:21.000000 safir-4.1.0/tests/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-08 18:06:21.000000 safir-4.1.0/tests/testing/gcs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-08 18:06:21.000000 safir-4.1.0/tests/testing/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-08 18:06:21.000000 safir-4.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 20:28:30.000000 safir-4.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.485092 safir-4.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 20:28:30.000000 safir-4.2.1/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 20:28:30.000000 safir-4.2.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-17 20:28:30.000000 safir-4.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.485092 safir-4.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 20:28:30.000000 safir-4.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-17 20:28:30.000000 safir-4.2.1/.github/workflows/periodic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-17 20:28:30.000000 safir-4.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-17 20:28:30.000000 safir-4.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-05-17 20:28:30.000000 safir-4.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 20:28:30.000000 safir-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 20:28:30.000000 safir-4.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 20:28:46.505092 safir-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-17 20:28:30.000000 safir-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.485092 safir-4.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 20:28:30.000000 safir-4.2.1/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-17 20:28:30.000000 safir-4.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-05-17 20:28:30.000000 safir-4.2.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 20:28:30.000000 safir-4.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.489092 safir-4.2.1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-17 20:28:30.000000 safir-4.2.1/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 20:28:30.000000 safir-4.2.1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-17 20:28:30.000000 safir-4.2.1/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-17 20:28:30.000000 safir-4.2.1/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-17 20:28:30.000000 safir-4.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.489092 safir-4.2.1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/arq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/fastapi-errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/gafaelfawr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/gcs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.493092 safir-4.2.1/docs/user-guide/github-apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/api-resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/create-a-github-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/handling-webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/github-apps/webhook-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/http-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/ivoa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/kubernetes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/pydantic-redis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/pydantic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/set-up-from-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/slack-webhook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/uvicorn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-17 20:28:30.000000 safir-4.2.1/docs/user-guide/x-forwarded.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-17 20:28:30.000000 safir-4.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:28:46.505092 safir-4.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.481092 safir-4.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.493092 safir-4.2.1/src/safir/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.497092 safir-4.2.1/src/safir/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/db_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/gafaelfawr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/dependencies/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.497092 safir-4.2.1/src/safir/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/github/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/github/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/github/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.497092 safir-4.2.1/src/safir/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/middleware/ivoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/middleware/x_forwarded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.497092 safir-4.2.1/src/safir/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/slack/blockkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/slack/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.501092 safir-4.2.1/src/safir/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74799 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-17 20:28:30.000000 safir-4.2.1/src/safir/testing/uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.493092 safir-4.2.1/src/safir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 20:28:46.000000 safir-4.2.1/src/safir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.501092 safir-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-17 20:28:30.000000 safir-4.2.1/tests/asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 20:28:30.000000 safir-4.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-17 20:28:30.000000 safir-4.2.1/tests/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-17 20:28:30.000000 safir-4.2.1/tests/datetime_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.501092 safir-4.2.1/tests/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/arq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/db_session_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/gafaelfawr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/http_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-17 20:28:30.000000 safir-4.2.1/tests/dependencies/logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-17 20:28:30.000000 safir-4.2.1/tests/fastapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-17 20:28:30.000000 safir-4.2.1/tests/gcs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.501092 safir-4.2.1/tests/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.485092 safir-4.2.1/tests/github/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/tests/github/data/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/check_run_created.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/check_suite_completed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/installation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/installation_repositories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/pull_request_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/data/webhooks/push_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-17 20:28:30.000000 safir-4.2.1/tests/github/webhooks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-17 20:28:30.000000 safir-4.2.1/tests/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-05-17 20:28:30.000000 safir-4.2.1/tests/logging_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-17 20:28:30.000000 safir-4.2.1/tests/metadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/tests/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-17 20:28:30.000000 safir-4.2.1/tests/middleware/ivoa_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-17 20:28:30.000000 safir-4.2.1/tests/middleware/x_forwarded_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 20:28:30.000000 safir-4.2.1/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-17 20:28:30.000000 safir-4.2.1/tests/pydantic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-17 20:28:30.000000 safir-4.2.1/tests/redis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-17 20:28:30.000000 safir-4.2.1/tests/safir_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/tests/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-17 20:28:30.000000 safir-4.2.1/tests/slack/blockkit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-17 20:28:30.000000 safir-4.2.1/tests/slack/webhook_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:46.505092 safir-4.2.1/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:28:30.000000 safir-4.2.1/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 20:28:30.000000 safir-4.2.1/tests/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-17 20:28:30.000000 safir-4.2.1/tests/testing/gcs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-17 20:28:30.000000 safir-4.2.1/tests/testing/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-17 20:28:30.000000 safir-4.2.1/tox.ini
```

### Comparing `safir-4.1.0/.github/workflows/ci.yaml` & `safir-4.2.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/.github/workflows/periodic.yaml` & `safir-4.2.1/.github/workflows/periodic.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/.gitignore` & `safir-4.2.1/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -124,7 +124,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# MacOS modern day resource fork
+.DS_Store
```

### Comparing `safir-4.1.0/.pre-commit-config.yaml` & `safir-4.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/CHANGELOG.md` & `safir-4.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Change log
 
 <!--
 Headline template:
 X.Y.Z (YYYY-MM-DD)
 -->
 
+## 4.2.0 (unreleased)
+
+### New features
+
+- Add `create_namespaced_persistent_volume_claim` to the mock Kubernetes API for testing.
+
+### Bug fixes
+
+- `SlackWebException` now extracts the method and URL of the request from more httpx exceptions, and avoids exceptions when the request information is not present.
+
 ## 4.1.0 (2023-05-08)
 
 ### New features
 
 - Add `read_*` methods for `ConfigMap` and `ResourceQuota` to the mock Kubernetes API for testing.
 - Add `patch_namespaced_pod_status` to the mock Kubernetes API for testing. Application code is unlikely to call this, but it's useful for test suites.
 - The mock `list_namespaced_pod` Kubernetes API now supports watches (but be aware that all changes must be made through the API).
```

### Comparing `safir-4.1.0/LICENSE` & `safir-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/PKG-INFO` & `safir-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.1.0
+Version: 4.2.1
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.1.0/README.md` & `safir-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/_rst_epilog.rst` & `safir-4.2.1/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/api.rst` & `safir-4.2.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/changelog.md` & `safir-4.2.1/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Change log
 
 <!--
 Headline template:
 X.Y.Z (YYYY-MM-DD)
 -->
 
+## 4.2.0 (unreleased)
+
+### New features
+
+- Add `create_namespaced_persistent_volume_claim` to the mock Kubernetes API for testing.
+
+### Bug fixes
+
+- `SlackWebException` now extracts the method and URL of the request from more httpx exceptions, and avoids exceptions when the request information is not present.
+
 ## 4.1.0 (2023-05-08)
 
 ### New features
 
 - Add `read_*` methods for `ConfigMap` and `ResourceQuota` to the mock Kubernetes API for testing.
 - Add `patch_namespaced_pod_status` to the mock Kubernetes API for testing. Application code is unlikely to call this, but it's useful for test suites.
 - The mock `list_namespaced_pod` Kubernetes API now supports watches (but be aware that all changes must be made through the API).
```

### Comparing `safir-4.1.0/docs/dev/development.rst` & `safir-4.2.1/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/dev/release.rst` & `safir-4.2.1/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/documenteer.toml` & `safir-4.2.1/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/index.rst` & `safir-4.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/arq.rst` & `safir-4.2.1/docs/user-guide/arq.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/database.rst` & `safir-4.2.1/docs/user-guide/database.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/datetime.rst` & `safir-4.2.1/docs/user-guide/datetime.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/fastapi-errors.rst` & `safir-4.2.1/docs/user-guide/fastapi-errors.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/gafaelfawr.rst` & `safir-4.2.1/docs/user-guide/gafaelfawr.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/gcs.rst` & `safir-4.2.1/docs/user-guide/gcs.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/github-apps/api-resources.rst` & `safir-4.2.1/docs/user-guide/github-apps/api-resources.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/github-apps/create-a-github-client.rst` & `safir-4.2.1/docs/user-guide/github-apps/create-a-github-client.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/github-apps/handling-webhooks.rst` & `safir-4.2.1/docs/user-guide/github-apps/handling-webhooks.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/github-apps/index.rst` & `safir-4.2.1/docs/user-guide/github-apps/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/github-apps/webhook-models.rst` & `safir-4.2.1/docs/user-guide/github-apps/webhook-models.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/http-client.rst` & `safir-4.2.1/docs/user-guide/http-client.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/ivoa.rst` & `safir-4.2.1/docs/user-guide/ivoa.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/kubernetes.rst` & `safir-4.2.1/docs/user-guide/kubernetes.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/logging.rst` & `safir-4.2.1/docs/user-guide/logging.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/pydantic-redis.rst` & `safir-4.2.1/docs/user-guide/pydantic-redis.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/pydantic.rst` & `safir-4.2.1/docs/user-guide/pydantic.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/set-up-from-template.rst` & `safir-4.2.1/docs/user-guide/set-up-from-template.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/slack-webhook.rst` & `safir-4.2.1/docs/user-guide/slack-webhook.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/uvicorn.rst` & `safir-4.2.1/docs/user-guide/uvicorn.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/docs/user-guide/x-forwarded.rst` & `safir-4.2.1/docs/user-guide/x-forwarded.rst`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/pyproject.toml` & `safir-4.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/__init__.py` & `safir-4.2.1/src/safir/__init__.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/arq.py` & `safir-4.2.1/src/safir/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/asyncio.py` & `safir-4.2.1/src/safir/asyncio.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/database.py` & `safir-4.2.1/src/safir/database.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/datetime.py` & `safir-4.2.1/src/safir/datetime.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/dependencies/arq.py` & `safir-4.2.1/src/safir/dependencies/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/dependencies/db_session.py` & `safir-4.2.1/src/safir/dependencies/db_session.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/dependencies/gafaelfawr.py` & `safir-4.2.1/src/safir/dependencies/gafaelfawr.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/dependencies/http_client.py` & `safir-4.2.1/src/safir/dependencies/http_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/dependencies/logger.py` & `safir-4.2.1/src/safir/dependencies/logger.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/fastapi.py` & `safir-4.2.1/src/safir/fastapi.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/gcs.py` & `safir-4.2.1/src/safir/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/github/_client.py` & `safir-4.2.1/src/safir/github/_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/github/models.py` & `safir-4.2.1/src/safir/github/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/github/webhooks.py` & `safir-4.2.1/src/safir/github/webhooks.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/kubernetes.py` & `safir-4.2.1/src/safir/kubernetes.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/logging.py` & `safir-4.2.1/src/safir/logging.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/metadata.py` & `safir-4.2.1/src/safir/metadata.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/middleware/ivoa.py` & `safir-4.2.1/src/safir/middleware/ivoa.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/middleware/x_forwarded.py` & `safir-4.2.1/src/safir/middleware/x_forwarded.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/models.py` & `safir-4.2.1/src/safir/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/pydantic.py` & `safir-4.2.1/src/safir/pydantic.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/redis.py` & `safir-4.2.1/src/safir/redis.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/slack/blockkit.py` & `safir-4.2.1/src/safir/slack/blockkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
 from typing import Any, ClassVar, Optional, Self
 
-from httpx import HTTPError, HTTPStatusError, RequestError
+from httpx import HTTPError, HTTPStatusError
 from pydantic import BaseModel, validator
 
 from safir.datetime import current_datetime, format_datetime_for_logging
 
 __all__ = [
     "SlackBaseBlock",
     "SlackBaseField",
@@ -334,22 +334,30 @@
                 url=str(exc.request.url),
                 user=user,
                 status=status,
                 body=exc.response.text,
             )
         else:
             message = f"{type(exc).__name__}: {str(exc)}"
-            if isinstance(exc, RequestError):
+
+            # All httpx.HTTPError exceptions have a slot for the request,
+            # initialized to None and then sometimes added by child
+            # constructors or during exception processing. The request
+            # property is a property method that raises RuntimeError if
+            # request has not been set, so we can't just check for None.
+            # Hence this approach of attempting to use the request and falling
+            # back on reporting less data if that raised any exception.
+            try:
                 return cls(
                     message,
                     method=exc.request.method,
                     url=str(exc.request.url),
                     user=user,
                 )
-            else:
+            except Exception:
                 return cls(message, user=user)
 
     def __init__(
         self,
         message: str,
         *,
         failed_at: Optional[datetime] = None,
@@ -383,15 +391,15 @@
         message = super().to_slack()
         message.message = self.message
         if self.url:
             if self.method:
                 text = f"{self.method} {self.url}"
             else:
                 text = self.url
-            message.blocks.append(SlackTextField(heading="URL", text=text))
+            message.blocks.append(SlackTextBlock(heading="URL", text=text))
         if self.body:
             block = SlackCodeBlock(heading="Response", code=self.body)
             message.blocks.append(block)
         return message
 
 
 def _format_and_truncate_at_end(string: str, max_length: int) -> str:
```

### Comparing `safir-4.1.0/src/safir/slack/webhook.py` & `safir-4.2.1/src/safir/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/testing/gcs.py` & `safir-4.2.1/src/safir/testing/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/testing/kubernetes.py` & `safir-4.2.1/src/safir/testing/kubernetes.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,39 +15,111 @@
 
 from kubernetes_asyncio import client, config
 from kubernetes_asyncio.client import (
     ApiException,
     CoreV1Event,
     CoreV1EventList,
     V1ConfigMap,
+    V1Ingress,
+    V1IngressList,
+    V1IngressStatus,
+    V1Job,
+    V1JobList,
+    V1JobStatus,
+    V1LoadBalancerStatus,
     V1Namespace,
     V1NamespaceList,
     V1NetworkPolicy,
     V1Node,
     V1NodeList,
     V1ObjectMeta,
     V1ObjectReference,
+    V1PersistentVolumeClaim,
     V1Pod,
     V1PodList,
     V1PodStatus,
     V1ResourceQuota,
     V1Secret,
     V1Service,
+    V1ServiceList,
     V1Status,
 )
 
 from ..datetime import current_datetime
 
 __all__ = [
     "MockKubernetesApi",
     "patch_kubernetes",
     "strip_none",
 ]
 
 
+def _parse_label_selector(label_selector: str) -> dict[str, str]:
+    """Parse a label selector.
+
+    Only equality is supported (with ``=`` or ``==``).
+
+    Parameters
+    ----------
+    label_selector
+        Label selector string to parse.
+
+    Returns
+    -------
+    dict of str to str
+        Dictionary of required labels to their required values.
+
+    Raises
+    ------
+    AssertionError
+        Raised if the label selector string is not a supported syntax.
+    """
+    result = {}
+    for requirement in label_selector.split(","):
+        match = re.match(r"([^!=]+)==?(.*)", requirement)
+        assert match and match.group(1) and match.group(2)
+        result[match.group(1)] = match.group(2)
+    return result
+
+
+def _check_labels(
+    obj_labels: Optional[dict[str, str]], label_selector: Optional[str]
+) -> bool:
+    """Check whether an object's labels match the label selector supplied.
+
+    Parameters
+    ----------
+    obj_labels
+        Kubernetes object labels
+
+    label_selector
+        label selector in string form
+
+    Returns
+    -------
+    bool
+        Did all of the supplied label_selector labels match
+        the object labels?
+    """
+    if label_selector is None or label_selector == "":
+        # Everything matches the absence of a selector.
+        return True
+    if obj_labels is None or not obj_labels:
+        # If there are no labels but a non-empty selector, it doesn't
+        # match.
+        return False
+    labels = _parse_label_selector(label_selector)
+    for lbl in labels:
+        if lbl not in obj_labels or labels[lbl] != obj_labels[lbl]:
+            # Label isn't present or its value isn't right
+            return False
+    # The whole selector is correct.
+    return True
+
+
 def strip_none(model: dict[str, Any]) -> dict[str, Any]:
     """Strip `None` values from a serialized Kubernetes object.
 
     Comparing Kubernetes objects against serialized expected output is a bit
     of a pain, since Kubernetes objects often contain tons of optional
     parameters and the ``to_dict`` serialization includes every parameter.
     The naive result is therefore tedious to read or understand.
@@ -124,14 +196,15 @@
 
     def build_watch_response(
         self,
         resource_version: Optional[str] = None,
         timeout_seconds: Optional[int] = None,
         *,
         field_selector: Optional[str] = None,
+        label_selector: Optional[str] = None,
     ) -> Mock:
         """Construct a response to a watch request.
 
         Wraps a watch iterator in the appropriate mock to behave as expected
         when called from ``kubernetes_asyncio``. This simulates an aiohttp
         response.
 
@@ -156,15 +229,15 @@
 
         Raises
         ------
         AssertionError
             Some other ``field_selector`` was provided.
         """
         generator = self._build_watcher(
-            resource_version, timeout_seconds, field_selector
+            resource_version, timeout_seconds, field_selector, label_selector
         )
 
         async def readline() -> bytes:
             return await generator.__anext__()
 
         response = Mock()
         response.content.readline = AsyncMock()
@@ -172,14 +245,15 @@
         return response
 
     def _build_watcher(
         self,
         resource_version: str | None,
         timeout_seconds: int | None,
         field_selector: str | None,
+        label_selector: str | None,
     ) -> AsyncIterator[bytes]:
         """Construct a watcher for this event stream.
 
         Parameters
         ----------
         resource_version
             Starting resource version for the watch. The resource version
@@ -188,14 +262,17 @@
         timeout_seconds
             How long to watch. This is total elapsed time, not the time
             between events. It matches the corresponding parameter in the
             Kubernetes API. If `None`, watch forever.
         field_selector
             Which events to retrieve when performing a watch. If set, it must
             be set to ``metadata.name=...`` to match a specific object name.
+        label_selector
+            Which events to retrieve when performing a watch.  All
+            labels must match.
 
         Returns
         -------
         AsyncIterator
             An async iterator that will return each new event in the stream,
             encoded as expected by the Kubernetes API, until the timeout
             occurs.
@@ -227,14 +304,18 @@
             else:
                 position = len(self._events)
             while True:
                 for event in self._events[position:]:
                     position += 1
                     if name and event["object"]["metadata"]["name"] != name:
                         continue
+                    if not _check_labels(
+                        event["object"]["metadata"]["labels"], label_selector
+                    ):
+                        continue
                     yield json.dumps(event).encode()
                 if not timeout:
                     await trigger.wait()
                 else:
                     now = current_datetime()
                     timeout_left = (timeout - now).total_seconds()
                     if timeout_left <= 0:
@@ -252,17 +333,18 @@
         # Return the iterator.
         return next_event()
 
 
 class MockKubernetesApi:
     """Mock Kubernetes API for testing.
 
-    This object simulates (with almost everything left out) the ``CoreV1Api``,
-    ``CustomObjectApi``, and ``NetworkingV1Api`` client objects while keeping
-    simple internal state. It is intended to be used as a mock inside tests.
+    This object simulates (with almost everything left out) the ``BatchV1Api``,
+    ``CoreV1Api``, ``CustomObjectApi``, and ``NetworkingV1Api`` client
+    objects while keeping simple internal state. It is intended to be used
+    as a mock inside tests.
 
     Methods ending with ``_for_test`` are outside of the API and are intended
     for use by the test suite.
 
     This mock does not enforce namespace creation before creating objects in a
     namespace. Creating an object in a namespace will implicitly create that
     namespace if it doesn't exist. However, it will not store a
@@ -275,16 +357,18 @@
     copied. The object provided will be stored, so changing that object will
     change the object returned by subsequent API calls. Likewise, the object
     returned by ``read_*`` calls will be the same object stored in the mock,
     and changing it will change the mock's data. (Sometimes this is the
     desired behavior, sometimes it isn't; we had to pick one and this is the
     approach we picked.)
 
-    Most APIs do not support watches. The only current exception is
-    `list_namespaced_event`.
+    Most APIs do not support watches. The current exceptions are
+    ``list_namespaced_event``, ``list_namespaced_ingress``,
+    ``list_namespaced_job``, ``list_namespaced_pod``, and
+    ``list_namespaced_service``.
 
     Attributes
     ----------
     initial_pod_phase
         String value to set the status of pods to when created. If this is set
         to ``Running`` (the default), a pod start event will also be
         generated when the pod is created.
@@ -415,14 +499,51 @@
         if body["kind"] in self._custom_kinds:
             assert key == self._custom_kinds[body["kind"]]
         else:
             self._custom_kinds[body["kind"]] = key
         assert namespace == body["metadata"]["namespace"]
         self._store_object(namespace, key, body["metadata"]["name"], body)
 
+    async def delete_namespaced_custom_object(
+        self,
+        group: str,
+        version: str,
+        namespace: str,
+        plural: str,
+        name: str,
+    ) -> Any:
+        """Delete a custom namespaced object.
+
+        Parameters
+        ----------
+        group
+            API group for this custom object.
+        version
+            API version for this custom object.
+        namespace
+            Namespace in which to delete the object.
+        plural
+            API plural for this custom object.
+        name
+            Custom object to delete.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Status
+            Success status if object was deleted.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 409 status if the object already exists.
+        """
+        self._maybe_error("delete_namespaced_custom_object", name, namespace)
+        key = f"{group}/{version}/{plural}"
+        return self._delete_object(namespace, key, name)
+
     async def get_namespaced_custom_object(
         self,
         group: str,
         version: str,
         namespace: str,
         plural: str,
         name: str,
@@ -738,14 +859,434 @@
         # This is done by the Kubernetes API Watch object.
         assert not _preload_content
 
         # Return the mock response expected by the Kubernetes API.
         stream = self._event_streams[namespace]["Event"]
         return stream.build_watch_response(resource_version, timeout_seconds)
 
+    # INGRESS API
+
+    async def create_namespaced_ingress(
+        self, namespace: str, body: V1Ingress
+    ) -> None:
+        """Create an ingress object.
+
+        In real life, it usually takes some time for the Ingress controller
+        to set the ``status.load_balancer.ingress`` field.  It appears that
+        status.load_balancer is created when the Ingress is but is empty,
+        so that's what we do too.
+
+        Use ``patch_namespaced_ingress_status()`` to update the field to
+        indicate that the ingress is ready.
+
+        Parameters
+        ----------
+        namespace
+            Namespace in which to create the object.
+        body
+            Object to create.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 409 status if the object already exists.
+        """
+        self._maybe_error("create_namespaced_ingress", namespace, body)
+        self._update_metadata(
+            body, "networking.k8s.io/v1", "Ingress", namespace
+        )
+        name = body.metadata.name
+        body.status = V1IngressStatus(
+            load_balancer=V1LoadBalancerStatus(ingress=[])
+        )
+        self._store_object(namespace, "Ingress", name, body)
+        stream = self._event_streams[namespace]["Ingress"]
+        stream.add_event({"type": "ADDED", "object": body.to_dict()})
+
+    async def delete_namespaced_ingress(
+        self, name: str, namespace: str
+    ) -> V1Status:
+        """Delete an ingress object.
+
+        Parameters
+        ----------
+        name
+            Name of ingress to delete.
+        namespace
+            Namespace of ingress to delete.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Status
+            Success status.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the ingress was not found.
+        """
+        self._maybe_error("delete_namespaced_ingress", name, namespace)
+        ingress = self._get_object(namespace, "Ingress", name)
+        stream = self._event_streams[namespace]["Ingress"]
+        stream.add_event({"type": "DELETED", "object": ingress.to_dict()})
+        return self._delete_object(namespace, "Ingress", name)
+
+    async def read_namespaced_ingress(
+        self, name: str, namespace: str
+    ) -> V1Ingress:
+        """Read a ingress object.
+
+        Parameters
+        ----------
+        name
+            Name of the ingress.
+        namespace
+            Namespace of the ingress.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Ingress
+            Ingress object.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the ingress was not found.
+        """
+        self._maybe_error("read_namespaced_ingress", name, namespace)
+        return self._get_object(namespace, "Ingress", name)
+
+    async def list_namespaced_ingress(
+        self,
+        namespace: str,
+        *,
+        field_selector: Optional[str] = None,
+        label_selector: Optional[str] = None,
+        resource_version: Optional[str] = None,
+        timeout_seconds: Optional[int] = None,
+        watch: bool = False,
+        _preload_content: bool = True,
+        _request_timeout: Optional[int] = None,
+    ) -> V1IngressList | Mock:
+        """List ingress objects in a namespace.
+
+        This does support watches.
+
+        Parameters
+        ----------
+        namespace
+            Namespace of ingresss to list.
+        field_selector
+            Only ``metadata.name=...`` is supported. It is parsed to find the
+            ingress name and only ingresss matching that name will be returned.
+        label_selector
+            Which events to retrieve when performing a watch.  All
+            labels must match.
+        resource_version
+            Where to start in the event stream when performing a watch. If
+            `None`, starts with the next change.
+        timeout_seconds
+            How long to return events for before exiting when performing a
+            watch.
+        watch
+            Whether to act as a watch.
+        _preload_content
+            Verified to be `False` when performing a watch.
+        _request_timeout
+            Ignored, accepted for compatibility with the watch API.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1IngressList or unittest.mock.Mock
+            List of ingresss in that namespace, when not called as a watch. If
+            called as a watch, returns a mock ``aiohttp.Response`` with a
+            ``readline`` metehod that yields the events.
+
+        Raises
+        ------
+        AssertionError
+            Some other ``field_selector`` was provided.
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the namespace does not exist.
+        """
+        self._maybe_error("list_namespaced_ingress", namespace, field_selector)
+        if namespace not in self._objects:
+            msg = f"Namespace {namespace} not found"
+            raise ApiException(status=404, reason=msg)
+        if not watch:
+            if field_selector:
+                match = re.match(r"metadata\.name=(.*)$", field_selector)
+                assert match and match.group(1)
+                try:
+                    ingress = self._get_object(
+                        namespace, "Ingress", match.group(1)
+                    )
+                    return V1IngressList(kind="Ingress", items=[ingress])
+                except ApiException:
+                    return V1IngressList(kind="Ingress", items=[])
+            else:
+                ingresss = []
+                if "Ingress" in self._objects[namespace]:
+                    for obj in self._objects[namespace]["Ingress"].values():
+                        if _check_labels(obj.metadata.labels, label_selector):
+                            ingresss.append(obj)
+                return V1IngressList(kind="Ingress", items=ingresss)
+
+        # All watches must not preload content since we're returning raw JSON.
+        # This is done by the Kubernetes API Watch object.
+        assert not _preload_content
+
+        # Return the mock response expected by the Kubernetes API.
+        stream = self._event_streams[namespace]["Ingress"]
+        return stream.build_watch_response(
+            resource_version,
+            timeout_seconds,
+            field_selector=field_selector,
+            label_selector=label_selector,
+        )
+
+    async def patch_namespaced_ingress_status(
+        self, name: str, namespace: str, body: list[dict[str, Any]]
+    ) -> V1Secret:
+        """Patch the status of an ingress object.
+
+        Parameters
+        ----------
+        name
+            Name of ingress object.
+        namespace
+            Namespace of ingress object.
+        body
+            Patches to apply. Only patches with ``op`` of ``replace`` are
+            supported, and only with ``path`` of
+            ``/status/loadBalancer/ingress``.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Ingress
+            Corresponding object.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the ingress does not exist.
+        AssertionError
+            Raised if any other type of patch was provided.
+        """
+        self._maybe_error("patch_namespaced_ingress", name, namespace)
+        ingress = copy.deepcopy(self._get_object(namespace, "Ingress", name))
+        for change in body:
+            assert change["op"] == "replace"
+            assert change["path"] == "/status/loadBalancer/ingress"
+            ingress.status.load_balancer.ingress = change["value"]
+        stream = self._event_streams[namespace]["Ingress"]
+        ingress.metadata.resource_version = stream.next_resource_version
+        self._store_object(namespace, "Ingress", name, ingress, replace=True)
+        stream.add_event({"type": "MODIFIED", "object": ingress.to_dict()})
+        return ingress
+
+    # JOB API
+
+    async def create_namespaced_job(self, namespace: str, body: V1Job) -> None:
+        """Create a job object.
+
+        A pod corresponding to this job will also be created. The pod will
+        have a label ``job-name`` set to the name of the Job object. Its
+        name will be the job's name prepended to ``-abcde``. If
+        ``initial_pod_phase`` on the mock is set to ``Running``, the
+        ``status.active`` field of the job will be set to 1.
+
+        Parameters
+        ----------
+        namespace
+            Namespace in which to create the object.
+        body
+            Object to create.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 409 status if the object already exists.
+        """
+        self._maybe_error("create_namespaced_job", namespace, body)
+        self._update_metadata(body, "batch/v1", "Job", namespace)
+        name = body.metadata.name
+        self._store_object(namespace, "Job", name, body)
+        # Pretend to spawn a pod
+        # If there is no metadata, create a V1ObjectMeta object with just
+        # namespace, a "generateName" of the job name, and a "job-name"
+        # label, which appears to be what Kubernetes does.
+        template = body.spec.template
+        podmd = template.metadata
+        if podmd is None:
+            podmd = V1ObjectMeta(
+                namespace=namespace,
+                generate_name=f"{name}-",
+            )
+        # In real life, the name has five random alphanumeric characters,
+        # but for testing we'd like to know what the spawned pod is going to
+        # be called.  But in real life, if you set "generateName" you can't
+        # also set the pod name.
+        podmd.name = name + "-abcde"
+        podmd.labels["job-name"] = name
+        pod = V1Pod(metadata=podmd, spec=template.spec)
+        await self.create_namespaced_pod(namespace, pod)
+        if pod.status.phase == "Running":
+            body.status = V1JobStatus(active=1)
+
+    async def delete_namespaced_job(
+        self, name: str, namespace: str, propagation_policy: str
+    ) -> V1Status:
+        """Delete a job object.
+
+        Will also propagate to pods.
+
+        Parameters
+        ----------
+        name
+            Name of job to delete.
+        namespace
+            Namespace of job to delete.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Status
+            Success status.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the job was not found.
+        """
+        assert (
+            propagation_policy == "Foreground"
+        ), "Only 'Foreground' propagation_policy is currently supported"
+        self._maybe_error("delete_namespaced_job", name, namespace)
+        stream = self._event_streams[namespace]["Job"]
+        pods = await self.list_namespaced_pod(
+            namespace, label_selector=f"job-name=={name}"
+        )
+        # This simulates a foreground deletion, where the Job is blocked
+        # from deletion until all its pods are deleted.
+        for pod in pods.items:
+            await self.delete_namespaced_pod(pod.metadata.name, namespace)
+        job = self._get_object(namespace, "Job", name)
+        stream.add_event({"type": "DELETED", "object": job.to_dict()})
+        return self._delete_object(namespace, "Job", name)
+
+    async def list_namespaced_job(
+        self,
+        namespace: str,
+        *,
+        field_selector: Optional[str] = None,
+        label_selector: Optional[str] = None,
+        resource_version: Optional[str] = None,
+        timeout_seconds: Optional[int] = None,
+        watch: bool = False,
+        _preload_content: bool = True,
+        _request_timeout: Optional[int] = None,
+    ) -> V1JobList | Mock:
+        """List job objects in a namespace.
+
+        This does support watches.
+
+        Parameters
+        ----------
+        namespace
+            Namespace of jobs to list.
+        field_selector
+            Only ``metadata.name=...`` is supported. It is parsed to find the
+            job name and only jobs matching that name will be returned.
+        label_selector
+            Which events to retrieve when performing a watch.  All
+            labels must match.
+        resource_version
+            Where to start in the event stream when performing a watch. If
+            `None`, starts with the next change.
+        timeout_seconds
+            How long to return events for before exiting when performing a
+            watch.
+        watch
+            Whether to act as a watch.
+        _preload_content
+            Verified to be `False` when performing a watch.
+        _request_timeout
+            Ignored, accepted for compatibility with the watch API.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1JobList or unittest.mock.Mock
+            List of jobs in that namespace, when not called as a watch. If
+            called as a watch, returns a mock ``aiohttp.Response`` with a
+            ``readline`` metehod that yields the events.
+
+        Raises
+        ------
+        AssertionError
+            Some other ``field_selector`` was provided.
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the namespace does not exist.
+        """
+        self._maybe_error("list_namespaced_job", namespace, field_selector)
+        if namespace not in self._objects:
+            msg = f"Namespace {namespace} not found"
+            raise ApiException(status=404, reason=msg)
+        if not watch:
+            if field_selector:
+                match = re.match(r"metadata\.name=(.*)$", field_selector)
+                assert match and match.group(1)
+                try:
+                    job = self._get_object(namespace, "Job", match.group(1))
+                    return V1JobList(kind="Job", items=[job])
+                except ApiException:
+                    return V1JobList(kind="Job", items=[])
+            else:
+                jobs = []
+                if "Job" in self._objects[namespace]:
+                    for obj in self._objects[namespace]["Job"].values():
+                        if _check_labels(obj.metadata.labels, label_selector):
+                            jobs.append(obj)
+                return V1JobList(kind="Job", items=jobs)
+
+        # All watches must not preload content since we're returning raw JSON.
+        # This is done by the Kubernetes API Watch object.
+        assert not _preload_content
+
+        # Return the mock response expected by the Kubernetes API.
+        stream = self._event_streams[namespace]["Job"]
+        return stream.build_watch_response(
+            resource_version,
+            timeout_seconds,
+            field_selector=field_selector,
+            label_selector=label_selector,
+        )
+
+    async def read_namespaced_job(self, name: str, namespace: str) -> V1Job:
+        """Read a job object.
+
+        Parameters
+        ----------
+        name
+            Name of the job.
+        namespace
+            Namespace of the job.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Job
+            Job object.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the job was not found.
+        """
+        self._maybe_error("read_namespaced_job", name, namespace)
+        return self._get_object(namespace, "Job", name)
+
     # NAMESPACE API
 
     async def create_namespace(self, body: V1Namespace) -> None:
         """Create a namespace.
 
         The mock doesn't truly track namespaces since it autocreates them when
         an object is created in that namespace (maybe that behavior should be
@@ -872,14 +1413,42 @@
         kubernetes_asyncio.client.V1NodeList
             The node information previouslyl stored with `set_nodes_for_test`,
             if any.
         """
         self._maybe_error("list_node")
         return self._nodes
 
+    # PERSISTENTVOLUMECLAIM API
+
+    async def create_namespaced_persistent_volume_claim(
+        self, namespace: str, body: V1PersistentVolumeClaim
+    ) -> None:
+        """Create a persistent volume claim.
+
+        Parameters
+        ----------
+        namespace
+            Namespace in which to create the persistent volume claim.
+        body
+            Persistent volume claim to create.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 409 status if the persistent volume claim already
+            exists.
+        """
+        self._maybe_error(
+            "create_namespaced_persistent_volume_claim", namespace, body
+        )
+        self._update_metadata(body, "v1", "PersistentVolumeClaim", namespace)
+        self._store_object(
+            namespace, "PersistentVolumeClaim", body.metadata.name, body
+        )
+
     # POD API
 
     async def create_namespaced_pod(self, namespace: str, body: V1Pod) -> None:
         """Create a pod object.
 
         If ``initial_pod_phase`` on the mock Kubernetes object is set to
         ``Running``, set the state to ``Running`` and generate a startup
@@ -947,14 +1516,15 @@
         return result
 
     async def list_namespaced_pod(
         self,
         namespace: str,
         *,
         field_selector: Optional[str] = None,
+        label_selector: Optional[str] = None,
         resource_version: Optional[str] = None,
         timeout_seconds: Optional[int] = None,
         watch: bool = False,
         _preload_content: bool = True,
         _request_timeout: Optional[int] = None,
     ) -> V1PodList | Mock:
         """List pod objects in a namespace.
@@ -964,14 +1534,16 @@
         Parameters
         ----------
         namespace
             Namespace of pods to list.
         field_selector
             Only ``metadata.name=...`` is supported. It is parsed to find the
             pod name and only pods matching that name will be returned.
+        label_selector
+            Only pods with labels matching all of these will be returned.
         resource_version
             Where to start in the event stream when performing a watch. If
             `None`, starts with the next change.
         timeout_seconds
             How long to return events for before exiting when performing a
             watch.
         watch
@@ -1001,31 +1573,38 @@
             raise ApiException(status=404, reason=msg)
         if not watch:
             if field_selector:
                 match = re.match(r"metadata\.name=(.*)$", field_selector)
                 assert match and match.group(1)
                 try:
                     pod = self._get_object(namespace, "Pod", match.group(1))
-                    return V1PodList(kind="Pod", items=[pod])
+                    if _check_labels(pod.metadata.labels, label_selector):
+                        return V1PodList(kind="Pod", items=[pod])
+                    return V1PodList(kind="Pod", items=[])
                 except ApiException:
                     return V1PodList(kind="Pod", items=[])
             else:
                 pods = []
-                for obj in self._objects[namespace]["Pod"].values():
-                    pods.append(obj)
+                if "Pod" in self._objects[namespace]:
+                    for obj in self._objects[namespace]["Pod"].values():
+                        if _check_labels(obj.metadata.labels, label_selector):
+                            pods.append(obj)
                 return V1PodList(kind="Pod", items=pods)
 
         # All watches must not preload content since we're returning raw JSON.
         # This is done by the Kubernetes API Watch object.
         assert not _preload_content
 
         # Return the mock response expected by the Kubernetes API.
         stream = self._event_streams[namespace]["Pod"]
         return stream.build_watch_response(
-            resource_version, timeout_seconds, field_selector=field_selector
+            resource_version,
+            timeout_seconds,
+            field_selector=field_selector,
+            label_selector=label_selector,
         )
 
     async def patch_namespaced_pod_status(
         self, name: str, namespace: str, body: list[dict[str, Any]]
     ) -> V1Secret:
         """Patch the status of a pod object.
 
@@ -1292,14 +1871,153 @@
         kubernetes_asyncio.client.ApiException
             Raised with 409 status if the object already exists.
         """
         self._maybe_error("create_namespaced_service", namespace, body)
         self._update_metadata(body, "v1", "Service", namespace)
         self._store_object(namespace, "Service", body.metadata.name, body)
 
+    async def delete_namespaced_service(
+        self, name: str, namespace: str
+    ) -> V1Status:
+        """Delete a service object.
+
+        Parameters
+        ----------
+        name
+            Name of service to delete.
+        namespace
+            Namespace of service to delete.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Status
+            Success status.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the service was not found.
+        """
+        self._maybe_error("delete_namespaced_service", name, namespace)
+        return self._delete_object(namespace, "Service", name)
+
+    async def list_namespaced_service(
+        self,
+        namespace: str,
+        *,
+        field_selector: Optional[str] = None,
+        label_selector: Optional[str] = None,
+        resource_version: Optional[str] = None,
+        timeout_seconds: Optional[int] = None,
+        watch: bool = False,
+        _preload_content: bool = True,
+        _request_timeout: Optional[int] = None,
+    ) -> V1ServiceList | Mock:
+        """List service objects in a namespace.
+
+        This does support watches.
+
+        Parameters
+        ----------
+        namespace
+            Namespace of services to list.
+        field_selector
+            Only ``metadata.name=...`` is supported. It is parsed to find the
+            service name and only services matching that name will be returned.
+        label_selector
+            Which events to retrieve when performing a watch.  All
+            labels must match.
+        resource_version
+            Where to start in the event stream when performing a watch. If
+            `None`, starts with the next change.
+        timeout_seconds
+            How long to return events for before exiting when performing a
+            watch.
+        watch
+            Whether to act as a watch.
+        _preload_content
+            Verified to be `False` when performing a watch.
+        _request_timeout
+            Ignored, accepted for compatibility with the watch API.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1ServiceList or unittest.mock.Mock
+            List of services in that namespace, when not called as a watch. If
+            called as a watch, returns a mock ``aiohttp.Response`` with a
+            ``readline`` metehod that yields the events.
+
+        Raises
+        ------
+        AssertionError
+            Some other ``field_selector`` was provided.
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the namespace does not exist.
+        """
+        self._maybe_error("list_namespaced_service", namespace, field_selector)
+        if namespace not in self._objects:
+            msg = f"Namespace {namespace} not found"
+            raise ApiException(status=404, reason=msg)
+        if not watch:
+            if field_selector:
+                match = re.match(r"metadata\.name=(.*)$", field_selector)
+                assert match and match.group(1)
+                try:
+                    service = self._get_object(
+                        namespace, "Service", match.group(1)
+                    )
+                    return V1ServiceList(kind="Service", items=[service])
+                except ApiException:
+                    return V1ServiceList(kind="Service", items=[])
+            else:
+                services = []
+                if "Service" in self._objects[namespace]:
+                    for obj in self._objects[namespace]["Service"].values():
+                        if _check_labels(obj.metadata.labels, label_selector):
+                            services.append(obj)
+                return V1ServiceList(kind="Service", items=services)
+
+        # All watches must not preload content since we're returning raw JSON.
+        # This is done by the Kubernetes API Watch object.
+        assert not _preload_content
+
+        # Return the mock response expected by the Kubernetes API.
+        stream = self._event_streams[namespace]["Service"]
+        return stream.build_watch_response(
+            resource_version,
+            timeout_seconds,
+            field_selector=field_selector,
+            label_selector=label_selector,
+        )
+
+    async def read_namespaced_service(
+        self, name: str, namespace: str
+    ) -> V1Service:
+        """Read a service.
+
+        Parameters
+        ----------
+        name
+            Name of service.
+        namespace
+            Namespace of service.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Service
+            Requested service.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the service does not exist.
+        """
+        self._maybe_error("read_namespaced_service", name, namespace)
+        return self._get_object(namespace, "Service", name)
+
     # Internal helper functions.
 
     def _delete_object(self, namespace: str, key: str, name: str) -> V1Status:
         """Delete an object from internal data structures.
 
         Returns
         -------
@@ -1472,15 +2190,20 @@
        @pytest.fixture
        def mock_kubernetes() -> Iterator[MockKubernetesApi]:
            yield from patch_kubernetes()
     """
     mock_api = MockKubernetesApi()
     with patch.object(config, "load_incluster_config"):
         patchers = []
-        for api in ("CoreV1Api", "CustomObjectsApi", "NetworkingV1Api"):
+        for api in (
+            "BatchV1Api",
+            "CoreV1Api",
+            "CustomObjectsApi",
+            "NetworkingV1Api",
+        ):
             patcher = patch.object(client, api)
             mock_class = patcher.start()
             mock_class.return_value = mock_api
             patchers.append(patcher)
         mock_api_client = Mock(spec=client.ApiClient)
         mock_api_client.close = AsyncMock()
         with patch.object(client, "ApiClient") as mock_client:
```

### Comparing `safir-4.1.0/src/safir/testing/slack.py` & `safir-4.2.1/src/safir/testing/slack.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir/testing/uvicorn.py` & `safir-4.2.1/src/safir/testing/uvicorn.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/src/safir.egg-info/PKG-INFO` & `safir-4.2.1/src/safir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.1.0
+Version: 4.2.1
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.1.0/src/safir.egg-info/SOURCES.txt` & `safir-4.2.1/src/safir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/conftest.py` & `safir-4.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/database_test.py` & `safir-4.2.1/tests/database_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/datetime_test.py` & `safir-4.2.1/tests/datetime_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/dependencies/arq_test.py` & `safir-4.2.1/tests/dependencies/arq_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/dependencies/db_session_test.py` & `safir-4.2.1/tests/dependencies/db_session_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/dependencies/gafaelfawr_test.py` & `safir-4.2.1/tests/dependencies/gafaelfawr_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/dependencies/http_client_test.py` & `safir-4.2.1/tests/dependencies/http_client_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/dependencies/logger_test.py` & `safir-4.2.1/tests/dependencies/logger_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/fastapi_test.py` & `safir-4.2.1/tests/fastapi_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/gcs_test.py` & `safir-4.2.1/tests/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/github/data/webhooks/check_run_created.json` & `safir-4.2.1/tests/github/data/webhooks/check_run_created.json`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/github/data/webhooks/check_suite_completed.json` & `safir-4.2.1/tests/github/data/webhooks/check_suite_completed.json`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/github/data/webhooks/installation.json` & `safir-4.2.1/tests/github/data/webhooks/installation.json`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/github/data/webhooks/installation_repositories.json` & `safir-4.2.1/tests/github/data/webhooks/installation_repositories.json`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/github/data/webhooks/pull_request_event.json` & `safir-4.2.1/tests/github/data/webhooks/pull_request_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/github/data/webhooks/push_event.json` & `safir-4.2.1/tests/github/data/webhooks/push_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/github/webhooks_test.py` & `safir-4.2.1/tests/github/webhooks_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/logging_test.py` & `safir-4.2.1/tests/logging_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/metadata_test.py` & `safir-4.2.1/tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/middleware/ivoa_test.py` & `safir-4.2.1/tests/middleware/ivoa_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/middleware/x_forwarded_test.py` & `safir-4.2.1/tests/middleware/x_forwarded_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/pydantic_test.py` & `safir-4.2.1/tests/pydantic_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/redis_test.py` & `safir-4.2.1/tests/redis_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/slack/blockkit_test.py` & `safir-4.2.1/tests/slack/blockkit_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/slack/webhook_test.py` & `safir-4.2.1/tests/slack/webhook_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/testing/conftest.py` & `safir-4.2.1/tests/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/testing/gcs_test.py` & `safir-4.2.1/tests/testing/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tests/testing/kubernetes_test.py` & `safir-4.2.1/tests/testing/kubernetes_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.1.0/tox.ini` & `safir-4.2.1/tox.ini`

 * *Files identical despite different names*

