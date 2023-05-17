# Comparing `tmp/bigflow-1.7.1.tar.gz` & `tmp/bigflow-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigflow-1.7.1.tar", last modified: Tue May  9 07:24:49 2023, max compression
+gzip compressed data, was "bigflow-1.7.2.tar", last modified: Wed May 17 20:06:08 2023, max compression
```

## Comparing `bigflow-1.7.1.tar` & `bigflow-1.7.2.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-09 07:23:52.000000 bigflow-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 07:23:52.000000 bigflow-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-09 07:23:52.000000 bigflow-1.7.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-09 07:24:49.684204 bigflow-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-09 07:23:52.000000 bigflow-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.672204 bigflow-1.7.1/bigflow/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/dataset_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/bigquery/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/build/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/build/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/reflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/build/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    35088 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dagbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/dataflow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/konfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/infra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/scaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow/scaffold/templates/migrate-11/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/.gitignore.j2
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/deployment_config.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/scaffold/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/bigflow/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/testing/isolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-09 07:23:52.000000 bigflow-1.7.1/bigflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.676204 bigflow-1.7.1/bigflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 07:24:49.000000 bigflow-1.7.1/bigflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 07:23:52.000000 bigflow-1.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.680204 bigflow-1.7.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 07:23:52.000000 bigflow-1.7.1/scripts/bf
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 07:23:52.000000 bigflow-1.7.1/scripts/bigflow
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:24:49.684204 bigflow-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-09 07:23:52.000000 bigflow-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/buildd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/buildd/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_reflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/buildd/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/cli_logs_duplicated_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_duplicated_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_duplicated_workflows/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/cli_logs_log_name_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_log_name_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_log_name_workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/cli_logs_regular_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_regular_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/cli_logs_regular_workflows/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    41823 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/cli/test_module/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_module/Unused1.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_module/Unused2.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_module/Unused3.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/cli/test_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/dagbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/dagbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/dagbuilder/test_dagbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23905 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_konfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/test_user_commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_user_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_user_commons/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_user_commons/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:24:49.684204 bigflow-1.7.1/test/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/testing/nonpure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-09 07:23:52.000000 bigflow-1.7.1/test/testing/test_isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-17 20:05:12.000000 bigflow-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 20:05:12.000000 bigflow-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-17 20:05:12.000000 bigflow-1.7.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-17 20:06:08.810688 bigflow-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-17 20:05:12.000000 bigflow-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.798688 bigflow-1.7.2/bigflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.798688 bigflow-1.7.2/bigflow/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/dataset_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/build/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/reflect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35088 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dagbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/konfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/migrate-11/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/.gitignore.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/deployment_config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/bigflow/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/testing/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.798688 bigflow-1.7.2/bigflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 20:05:12.000000 bigflow-1.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 20:05:12.000000 bigflow-1.7.2/scripts/bf
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 20:05:12.000000 bigflow-1.7.2/scripts/bigflow
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:06:08.810688 bigflow-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-17 20:05:12.000000 bigflow-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/test/buildd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/buildd/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_reflect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/cli_logs_duplicated_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_duplicated_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_duplicated_workflows/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/cli_logs_log_name_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_log_name_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_log_name_workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/cli_logs_regular_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_regular_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_regular_workflows/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41823 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/test_module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_module/Unused1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_module/Unused2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_module/Unused3.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/dagbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/dagbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/dagbuilder/test_dagbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23905 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_konfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/test_user_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_user_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_user_commons/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_user_commons/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/testing/nonpure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/testing/test_isolate.py
```

### Comparing `bigflow-1.7.1/LICENSE` & `bigflow-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/NOTICE` & `bigflow-1.7.2/NOTICE`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/PKG-INFO` & `bigflow-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigflow
-Version: 1.7.1
+Version: 1.7.2
 Summary: BigQuery client wrapper with clean API
 Home-page: https://github.com/allegro/bigflow
 Author: Pogranicze
 Author-email: pogranicze-team@allegro.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `bigflow-1.7.1/README.md` & `bigflow-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/__init__.py` & `bigflow-1.7.2/bigflow/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/bigquery/__init__.py` & `bigflow-1.7.2/bigflow/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/bigquery/dataset_configuration.py` & `bigflow-1.7.2/bigflow/bigquery/dataset_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/bigquery/dataset_manager.py` & `bigflow-1.7.2/bigflow/bigquery/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/bigquery/interactive.py` & `bigflow-1.7.2/bigflow/bigquery/interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/bigquery/interface.py` & `bigflow-1.7.2/bigflow/bigquery/interface.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/bigquery/job.py` & `bigflow-1.7.2/bigflow/bigquery/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/build/dev.py` & `bigflow-1.7.2/bigflow/build/dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/build/dist.py` & `bigflow-1.7.2/bigflow/build/dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/build/legacy.py` & `bigflow-1.7.2/bigflow/build/legacy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/build/operate.py` & `bigflow-1.7.2/bigflow/build/operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/build/pip.py` & `bigflow-1.7.2/bigflow/build/pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/build/reflect.py` & `bigflow-1.7.2/bigflow/build/reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/build/spec.py` & `bigflow-1.7.2/bigflow/build/spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/cli.py` & `bigflow-1.7.2/bigflow/cli.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/commons.py` & `bigflow-1.7.2/bigflow/commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/configuration.py` & `bigflow-1.7.2/bigflow/configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/dagbuilder.py` & `bigflow-1.7.2/bigflow/dagbuilder.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,16 +62,17 @@
             from airflow.kubernetes.secret import Secret
             from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import KubernetesPodOperator
         except ImportError:
             # Fallback to older Airflow
             from airflow.contrib.kubernetes.secret import Secret
             from airflow.contrib.operators.kubernetes_pod_operator import KubernetesPodOperator
             
-        # BigFlow assumes that you use (airflow 1.x + composer 1.x) or (airflow 2.x + composer 2.x)
+        # To deploy BigFlow project, following requirements options are needed: (airflow 1.x + composer 1.x) or (airflow 2.x + composer >= 2.1.0)
         IS_COMPOSER_2_X = version.version >= '2.0.0'
+        IS_AIRFLOW_2_3_X = version.version >= '2.3.0'
         namespace = 'composer-user-workloads' if IS_COMPOSER_2_X else 'default'
             
         default_args = dict(
             owner='airflow',
             depends_on_past={workflow.depends_on_past!r},
             start_date={workflow_start_date!r},
             email_on_failure=False,
@@ -131,15 +132,15 @@
                 'image': {image_version!r},
                 'is_delete_operator_pod': True,
                 'retries': {retries!r},
                 'retry_delay': {retry_delay!r},
                 'secrets': {secrets_definition_list},
                 'execution_timeout': {execution_timeout!r},
             }}
-            if IS_COMPOSER_2_X:
+            if IS_AIRFLOW_2_3_X:
                 {pod_operator_params_var}['config_file'] = "/home/airflow/composer_kube_config"
                 {pod_operator_params_var}['kubernetes_conn_id'] = "kubernetes_default"
 
             {job_var} = KubernetesPodOperator(**{pod_operator_params_var})
             """))
 
         for d in dependencies:
```

### Comparing `bigflow-1.7.1/bigflow/dataflow/io.py` & `bigflow-1.7.2/bigflow/dataflow/io.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/dataflow/job.py` & `bigflow-1.7.2/bigflow/dataflow/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/dataflow/ml.py` & `bigflow-1.7.2/bigflow/dataflow/ml.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/dataflow/options.py` & `bigflow-1.7.2/bigflow/dataflow/options.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/deploy.py` & `bigflow-1.7.2/bigflow/deploy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/konfig.py` & `bigflow-1.7.2/bigflow/konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/migrate.py` & `bigflow-1.7.2/bigflow/migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/resources.py` & `bigflow-1.7.2/bigflow/resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/infra.py` & `bigflow-1.7.2/bigflow/scaffold/infra.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/scaffold.py` & `bigflow-1.7.2/bigflow/scaffold/scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/README.txt` & `bigflow-1.7.2/bigflow/scaffold/templates/README.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/.gitignore.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/Dockerfile` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/README.md` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/README.md`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/deployment_config.py.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/deployment_config.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2` & `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/scaffold/templating.py` & `bigflow-1.7.2/bigflow/scaffold/templating.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/testing/isolate.py` & `bigflow-1.7.2/bigflow/testing/isolate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/version.py` & `bigflow-1.7.2/bigflow/version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow/workflow.py` & `bigflow-1.7.2/bigflow/workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow.egg-info/PKG-INFO` & `bigflow-1.7.2/bigflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigflow
-Version: 1.7.1
+Version: 1.7.2
 Summary: BigQuery client wrapper with clean API
 Home-page: https://github.com/allegro/bigflow
 Author: Pogranicze
 Author-email: pogranicze-team@allegro.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `bigflow-1.7.1/bigflow.egg-info/SOURCES.txt` & `bigflow-1.7.2/bigflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/bigflow.egg-info/requires.txt` & `bigflow-1.7.2/bigflow.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/setup.py` & `bigflow-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/buildd/test_dev.py` & `bigflow-1.7.2/test/buildd/test_dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/buildd/test_dist.py` & `bigflow-1.7.2/test/buildd/test_dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/buildd/test_operate.py` & `bigflow-1.7.2/test/buildd/test_operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/buildd/test_pip.py` & `bigflow-1.7.2/test/buildd/test_pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/buildd/test_reflect.py` & `bigflow-1.7.2/test/buildd/test_reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/buildd/test_spec.py` & `bigflow-1.7.2/test/buildd/test_spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/cli/test_cli.py` & `bigflow-1.7.2/test/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/cli/test_module/Unused1.py` & `bigflow-1.7.2/test/cli/test_module/Unused1.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/dagbuilder/test_dagbuilder.py` & `bigflow-1.7.2/test/dagbuilder/test_dagbuilder.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_commons.py` & `bigflow-1.7.2/test/test_commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_configuration.py` & `bigflow-1.7.2/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_dataflow.py` & `bigflow-1.7.2/test/test_dataflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_deploy.py` & `bigflow-1.7.2/test/test_deploy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_interactive.py` & `bigflow-1.7.2/test/test_interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_job.py` & `bigflow-1.7.2/test/test_job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_konfig.py` & `bigflow-1.7.2/test/test_konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_migrate.py` & `bigflow-1.7.2/test/test_migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_resources.py` & `bigflow-1.7.2/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_scaffold.py` & `bigflow-1.7.2/test/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_user_commons/test_labels.py` & `bigflow-1.7.2/test/test_user_commons/test_labels.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_user_commons/test_sensor.py` & `bigflow-1.7.2/test/test_user_commons/test_sensor.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_version.py` & `bigflow-1.7.2/test/test_version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/test_workflow.py` & `bigflow-1.7.2/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.1/test/testing/test_isolate.py` & `bigflow-1.7.2/test/testing/test_isolate.py`

 * *Files identical despite different names*

