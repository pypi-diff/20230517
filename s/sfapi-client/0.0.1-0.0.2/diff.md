# Comparing `tmp/sfapi_client-0.0.1.tar.gz` & `tmp/sfapi_client-0.0.2.tar.gz`

## Comparing `sfapi_client-0.0.1.tar` & `sfapi_client-0.0.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/pytest.ini
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/.github/workflows/pypi.yml
--rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/gen_examples.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/gen_sync.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/index.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/community/contributing.md
--rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/examples/check_current_and_past_jobs.ipynb
--rw-r--r--   0        0        0    11955 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/examples/run_job_and_check_status.ipynb
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/javascript/apiselector.js
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/quickstart/index.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/SUMMARY.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/client/index.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/compute/index.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/exceptions/index.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/groups/index.md
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/jobs/index.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/paths/index.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/projects/index.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/resources/index.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/docs/reference/async/users/index.md
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/scripts/run.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_compute.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_jobs.py
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_monitor.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/client.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/compute.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/exceptions.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/groups.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/jobs.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/paths.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/projects.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/resources.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_async/__init__.py
--rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_async/client.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_async/compute.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_async/groups.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_async/jobs.py
--rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_async/paths.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_async/projects.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_async/users.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_models/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_models/job_status_response_sacct.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_models/job_status_response_squeue.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_models/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/__init__.py
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/_models.py
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/client.py
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/compute.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/groups.py
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/jobs.py
--rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/paths.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/projects.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/src/sfapi_client/_sync/users.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_api.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_api_async.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_client.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_client_async.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_compute.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_compute_async.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_groups.py
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_groups_async.py
--rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_jobs.py
--rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_jobs_async.py
--rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_paths.py
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_paths_async.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_projects.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_projects_async.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_resources.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_resources_async.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_users.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/tests/test_users_async.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/.gitignore
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/LICENSE
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 sfapi_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/pytest.ini
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/.github/workflows/pypi.yml
+-rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/gen_examples.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/gen_sync.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/index.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/community/contributing.md
+-rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/examples/check_current_and_past_jobs.ipynb
+-rw-r--r--   0        0        0    11955 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/examples/run_job_and_check_status.ipynb
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/javascript/apiselector.js
+-rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/quickstart/index.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/SUMMARY.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/client/index.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/compute/index.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/exceptions/index.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/groups/index.md
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/jobs/index.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/paths/index.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/projects/index.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/resources/index.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/docs/reference/async/users/index.md
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/scripts/run.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_compute.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_jobs.py
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_monitor.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/client.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/compute.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/exceptions.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/groups.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/jobs.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/paths.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/projects.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/resources.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/__init__.py
+-rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/client.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/compute.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/groups.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/jobs.py
+-rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/paths.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/projects.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_async/users.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_models/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_models/job_status_response_sacct.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_models/job_status_response_squeue.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_models/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/__init__.py
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/_models.py
+-rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/client.py
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/compute.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/groups.py
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/jobs.py
+-rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/paths.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/projects.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/src/sfapi_client/_sync/users.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_api.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_api_async.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_client.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_client_async.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_compute.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_compute_async.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_groups.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_groups_async.py
+-rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_jobs.py
+-rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_jobs_async.py
+-rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_paths.py
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_paths_async.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_projects.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_projects_async.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_resources.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_resources_async.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_users.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/tests/test_users_async.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 sfapi_client-0.0.2/PKG-INFO
```

### Comparing `sfapi_client-0.0.1/mkdocs.yml` & `sfapi_client-0.0.2/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 site_name: sfapi_client
 watch: [src/sfapi_client]
 nav:
   - Overview: index.md
   - Usage:
       - QuickStart: quickstart/
-      - Examples: examples/index.md
+      - Examples: examples/
   - API Reference: reference/
   - Community:
       - Contributing: community/contributing.md
 
 theme:
   name: "material"
   features:
```

### Comparing `sfapi_client-0.0.1/.github/workflows/mkdocs.yml` & `sfapi_client-0.0.2/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/.github/workflows/pypi.yml` & `sfapi_client-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/gen_examples.py` & `sfapi_client-0.0.2/docs/gen_examples.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/gen_sync.py` & `sfapi_client-0.0.2/docs/gen_sync.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/index.md` & `sfapi_client-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/examples/check_current_and_past_jobs.ipynb` & `sfapi_client-0.0.2/docs/examples/check_current_and_past_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/examples/run_job_and_check_status.ipynb` & `sfapi_client-0.0.2/docs/examples/run_job_and_check_status.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/javascript/apiselector.js` & `sfapi_client-0.0.2/docs/javascript/apiselector.js`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/reference/async/compute/index.md` & `sfapi_client-0.0.2/docs/reference/async/compute/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/reference/async/groups/index.md` & `sfapi_client-0.0.2/docs/reference/async/groups/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/reference/async/jobs/index.md` & `sfapi_client-0.0.2/docs/reference/async/jobs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/reference/async/paths/index.md` & `sfapi_client-0.0.2/docs/reference/async/paths/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/docs/reference/async/projects/index.md` & `sfapi_client-0.0.2/docs/reference/async/projects/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/scripts/run.py` & `sfapi_client-0.0.2/scripts/run.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_jobs.py` & `sfapi_client-0.0.2/src/sfapi_client/_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_monitor.py` & `sfapi_client-0.0.2/src/sfapi_client/_monitor.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_async/client.py` & `sfapi_client-0.0.2/src/sfapi_client/_async/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
 
 class AsyncClient:
     def __init__(
         self,
         client_id: Optional[str] = None,
         secret: Optional[str] = None,
-        key_name: Optional[Union[str, Path]] = None,
+        key: Optional[Union[str, Path]] = None,
         api_base_url: Optional[str] = SFAPI_BASE_URL,
         wait_interval: int = 10,
     ):
         """
         Create a client instance.
 
         Usage:
@@ -228,15 +228,15 @@
 
         :return: The client instance
         :rtype: AsyncClient
         """
         self._client_id = None
         self._secret = None
         if any(arg is None for arg in [client_id, secret]):
-            self._read_client_secret_from_file(key_name)
+            self._read_client_secret_from_file(key)
         else:
             self._client_id = client_id
             self._secret = secret
         self._api_base_url = api_base_url
         self._client_user = None
         self.__oauth2_session = None
         self._api = None
@@ -492,8 +492,7 @@
         """
         Resource related information.
         """
         if self._resources is None:
             self._resources = AsyncResources(self)
 
         return self._resources
-
```

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_async/compute.py` & `sfapi_client-0.0.2/src/sfapi_client/_async/compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_async/groups.py` & `sfapi_client-0.0.2/src/sfapi_client/_async/groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_async/jobs.py` & `sfapi_client-0.0.2/src/sfapi_client/_async/jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_async/paths.py` & `sfapi_client-0.0.2/src/sfapi_client/_async/paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_async/projects.py` & `sfapi_client-0.0.2/src/sfapi_client/_async/projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_async/users.py` & `sfapi_client-0.0.2/src/sfapi_client/_async/users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_models/__init__.py` & `sfapi_client-0.0.2/src/sfapi_client/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_models/job_status_response_sacct.py` & `sfapi_client-0.0.2/src/sfapi_client/_models/job_status_response_sacct.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_models/job_status_response_squeue.py` & `sfapi_client-0.0.2/src/sfapi_client/_models/job_status_response_squeue.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_models/resources.py` & `sfapi_client-0.0.2/src/sfapi_client/_models/resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_sync/_models.py` & `sfapi_client-0.0.2/src/sfapi_client/_sync/_models.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_sync/client.py` & `sfapi_client-0.0.2/src/sfapi_client/_sync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
 
 class Client:
     def __init__(
         self,
         client_id: Optional[str] = None,
         secret: Optional[str] = None,
-        key_name: Optional[Union[str, Path]] = None,
+        key: Optional[Union[str, Path]] = None,
         api_base_url: Optional[str] = SFAPI_BASE_URL,
         wait_interval: int = 10,
     ):
         """
         Create a client instance.
 
         Usage:
@@ -228,15 +228,15 @@
 
         :return: The client instance
         :rtype: Client
         """
         self._client_id = None
         self._secret = None
         if any(arg is None for arg in [client_id, secret]):
-            self._read_client_secret_from_file(key_name)
+            self._read_client_secret_from_file(key)
         else:
             self._client_id = client_id
             self._secret = secret
         self._api_base_url = api_base_url
         self._client_user = None
         self.__oauth2_session = None
         self._api = None
@@ -492,8 +492,7 @@
         """
         Resource related information.
         """
         if self._resources is None:
             self._resources = Resources(self)
 
         return self._resources
-
```

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_sync/compute.py` & `sfapi_client-0.0.2/src/sfapi_client/_sync/compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_sync/groups.py` & `sfapi_client-0.0.2/src/sfapi_client/_sync/groups.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,19 +5,25 @@
 from .users import User
 
 
 class GroupMember(GroupMemberBase):
     client: Optional["Client"]
 
     def user(self) -> "User":
+        """
+        Get the user associated with the membership.
+        """
         return User._fetch_user(self.client, self.name)
 
 
 # Note: We can't use our generated model as we want user => members ( to avoid confusion with User model )
 class Group(BaseModel):
+    """
+    A user group.
+    """
     client: Optional["Client"]
     gid: Optional[int]
     name: Optional[str]
     users_: Optional[List[GroupMemberBase]] = Field(..., alias="users")
 
     def _group_action(
         self,
@@ -46,21 +52,34 @@
             # See if we have validation error raise it
             if "details" in json_response:
                 raise SfApiError(r.text)
             else:
                 raise RuntimeError(r.text)
 
     def add(self, users: Union[List[str], List["User"]]):
+        """
+        Add users to the group.
+
+        :param users: The usernames to add
+        """
         self._group_action(users, GroupAction.batch_add)
 
     def remove(self, users: Union[List[str], List["User"]]):
+        """
+        Remove users from the group.
+
+        :param users: The usernames to remove
+        """
         self._group_action(users, GroupAction.batch_remove)
 
     @property
     def members(self):
+        """
+        The users in this group.
+        """
         members = [GroupMember.parse_obj(user_info) for user_info in self.users_]
 
         def _set_client(m):
             m.client = self.client
 
             return m
```

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_sync/jobs.py` & `sfapi_client-0.0.2/src/sfapi_client/_sync/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,18 @@
         user: Optional[str] = None,
         partition: Optional[str] = None,
     ):
         return _fetch_jobs(cls, compute, jobids, user, partition)
 
 
 class JobSqueue(Job, JobSqueueBase):
+    """
+    Models a job running on a compute resource, the informatio is
+    fetched using `squeue`.
+    """
     _command: ClassVar[JobCommand] = JobCommand.squeue
 
     def _fetch_state(self):
         jobs = self.compute._monitor.fetch_jobs(
             job_type=self.__class__, jobids=[self.jobid]
         )
         # If the job state comes back empty the job is probably no longer in
```

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_sync/paths.py` & `sfapi_client-0.0.2/src/sfapi_client/_sync/paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/src/sfapi_client/_sync/users.py` & `sfapi_client-0.0.2/src/sfapi_client/_sync/users.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
         user = User.parse_obj(json_response)
         user.client = client
 
         return user
 
     def groups(self) -> List["Group"]:
+        """
+        The groups that the user is a member of.
+        """
         # Avoid circular import
         from .groups import Group
 
         if self.name != (self.client._user()).name:
             raise SfApiError(f"Can only fetch groups for authenticated user.")
 
         r = self.client.get("account/groups")
@@ -43,14 +46,17 @@
             return g
 
         groups = map(_set_client, groups)
 
         return list(groups)
 
     def projects(self) -> List[Project]:
+        """
+        The projects the user is associate with.
+        """
         if self.name != (self.client._user()).name:
             raise SfApiError(f"Can only fetch projects for authenticated user.")
 
         r = self.client.get("account/roles")
 
         json_response = r.json()
```

### Comparing `sfapi_client-0.0.1/tests/conftest.py` & `sfapi_client-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_compute.py` & `sfapi_client-0.0.2/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_compute_async.py` & `sfapi_client-0.0.2/tests/test_compute_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_groups.py` & `sfapi_client-0.0.2/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_groups_async.py` & `sfapi_client-0.0.2/tests/test_groups_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_jobs.py` & `sfapi_client-0.0.2/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_jobs_async.py` & `sfapi_client-0.0.2/tests/test_jobs_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_paths.py` & `sfapi_client-0.0.2/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_paths_async.py` & `sfapi_client-0.0.2/tests/test_paths_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_projects.py` & `sfapi_client-0.0.2/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_projects_async.py` & `sfapi_client-0.0.2/tests/test_projects_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_resources.py` & `sfapi_client-0.0.2/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_resources_async.py` & `sfapi_client-0.0.2/tests/test_resources_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_users.py` & `sfapi_client-0.0.2/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/tests/test_users_async.py` & `sfapi_client-0.0.2/tests/test_users_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/LICENSE` & `sfapi_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/README.md` & `sfapi_client-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 ## Features
 
 * `async` interface and standard synchronous interface.
 * Fully type annotated.
 
 ## Documentation
 
-For the basics, head over to the [QuickStart](). We also have Jupyter Nodebook [examples]().
+For the basics, head over to the [QuickStart](https://nersc.github.io/sfapi_client/quickstart/). We also have Jupyter Nodebook [examples](https://nersc.github.io/sfapi_client/examples/).
 
-More in depth developer documentation can be found in the [API reference]().
+More in depth developer documentation can be found in the [API reference](https://nersc.github.io/sfapi_client/reference/async/client/).
 
 ## Dependencies
 
 The sfapi_client project relies on these libraries:
 
 * `httpx` - HTTP support.
 * `authlib` - OAuth 2.0 authentication.
@@ -47,8 +47,8 @@
 
 ## Installation
 
 Install with pip:
 
 ```shell
 $ pip install sfapi_client
-```
+```
```

### Comparing `sfapi_client-0.0.1/pyproject.toml` & `sfapi_client-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.1/PKG-INFO` & `sfapi_client-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfapi_client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python client for NERSC SF API
 Author-email: Chris Harris <cjh@lbl.gov>, Nicholas Tyler <tylern@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -52,17 +52,17 @@
 ## Features
 
 * `async` interface and standard synchronous interface.
 * Fully type annotated.
 
 ## Documentation
 
-For the basics, head over to the [QuickStart](). We also have Jupyter Nodebook [examples]().
+For the basics, head over to the [QuickStart](https://nersc.github.io/sfapi_client/quickstart/). We also have Jupyter Nodebook [examples](https://nersc.github.io/sfapi_client/examples/).
 
-More in depth developer documentation can be found in the [API reference]().
+More in depth developer documentation can be found in the [API reference](https://nersc.github.io/sfapi_client/reference/async/client/).
 
 ## Dependencies
 
 The sfapi_client project relies on these libraries:
 
 * `httpx` - HTTP support.
 * `authlib` - OAuth 2.0 authentication.
@@ -74,8 +74,8 @@
 
 ## Installation
 
 Install with pip:
 
 ```shell
 $ pip install sfapi_client
-```
+```
```

