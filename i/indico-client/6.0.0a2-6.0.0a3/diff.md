# Comparing `tmp/indico-client-6.0.0a2.tar.gz` & `tmp/indico-client-6.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indico-client-6.0.0a2.tar", last modified: Wed Feb  1 14:16:19 2023, max compression
+gzip compressed data, was "indico-client-6.0.0a3.tar", last modified: Wed May 17 17:32:29 2023, max compression
```

## Comparing `indico-client-6.0.0a2.tar` & `indico-client-6.0.0a3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.476552 indico-client-6.0.0a2/
--rw-r--r--   0 root         (0) root         (0)       57 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1086 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      697 2023-02-01 14:16:19.480552 indico-client-6.0.0a2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      370 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.480552 indico-client-6.0.0a2/indico/
--rw-r--r--   0 root         (0) root         (0)      308 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/__init__.py
--rw-r--r--   0 root         (0) root         (0)      504 2023-02-01 14:16:19.480552 indico-client-6.0.0a2/indico/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.468552 indico-client-6.0.0a2/indico/client/
--rw-r--r--   0 root         (0) root         (0)       45 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/client/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.468552 indico-client-6.0.0a2/indico/config/
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/config/config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.468552 indico-client-6.0.0a2/indico/filters/
--rw-r--r--   0 root         (0) root         (0)     5896 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.468552 indico-client-6.0.0a2/indico/http/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6649 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/http/client.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/http/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.472552 indico-client-6.0.0a2/indico/queries/
--rw-r--r--   0 root         (0) root         (0)      326 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16872 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/datasets.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/document_report.py
--rw-r--r--   0 root         (0) root         (0)     3694 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/documents.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/example.py
--rw-r--r--   0 root         (0) root         (0)     6752 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/export.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/forms.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/integration.py
--rw-r--r--   0 root         (0) root         (0)     2983 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/jobs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.472552 indico-client-6.0.0a2/indico/queries/model_groups/
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/model_groups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4179 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/model_groups/metrics.py
--rw-r--r--   0 root         (0) root         (0)    10723 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/model_groups/model_groups.py
--rw-r--r--   0 root         (0) root         (0)    10137 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     4529 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/storage.py
--rw-r--r--   0 root         (0) root         (0)    14363 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/submission.py
--rw-r--r--   0 root         (0) root         (0)     5791 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/usermetrics.py
--rw-r--r--   0 root         (0) root         (0)    16883 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/workflow.py
--rw-r--r--   0 root         (0) root         (0)    15819 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/workflow_components.py
--rw-r--r--   0 root         (0) root         (0)     5954 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/queries/workflow_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.472552 indico-client-6.0.0a2/indico/types/
--rw-r--r--   0 root         (0) root         (0)      257 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/base.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/datafile.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/dataset.py
--rw-r--r--   0 root         (0) root         (0)      482 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/document_report.py
--rw-r--r--   0 root         (0) root         (0)     1297 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/export.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/integration.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/jobs.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/model.py
--rw-r--r--   0 root         (0) root         (0)     2187 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/model_group.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/model_metrics.py
--rw-r--r--   0 root         (0) root         (0)      397 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/submission.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/submission_file.py
--rw-r--r--   0 root         (0) root         (0)     3543 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/user_metrics.py
--rw-r--r--   0 root         (0) root         (0)      357 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/utils.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/workflow.py
--rw-r--r--   0 root         (0) root         (0)     9438 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/indico/types/workflow_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.476552 indico-client-6.0.0a2/indico_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      697 2023-02-01 14:16:19.000000 indico-client-6.0.0a2/indico_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2402 2023-02-01 14:16:19.000000 indico-client-6.0.0a2/indico_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 14:16:19.000000 indico-client-6.0.0a2/indico_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-02-01 14:16:19.000000 indico-client-6.0.0a2/indico_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-01 14:16:19.000000 indico-client-6.0.0a2/indico_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      170 2023-02-01 14:16:19.480552 indico-client-6.0.0a2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      929 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.464552 indico-client-6.0.0a2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.476552 indico-client-6.0.0a2/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.476552 indico-client-6.0.0a2/tests/integration/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7269 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/data/datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.476552 indico-client-6.0.0a2/tests/integration/queries/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12117 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5233 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_document.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_document_report.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_export.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_job.py
--rw-r--r--   0 root         (0) root         (0)     8478 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_model_group.py
--rw-r--r--   0 root         (0) root         (0)     4408 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_user_metrics.py
--rw-r--r--   0 root         (0) root         (0)    14759 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_workflow.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_workflow_component.py
--rw-r--r--   0 root         (0) root         (0)     3079 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/queries/test_workflow_metrics.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/integration/test_base_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 14:16:19.476552 indico-client-6.0.0a2/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/tests/unit/test_filters.py
--rw-r--r--   0 root         (0) root         (0)    70238 2023-02-01 14:14:01.000000 indico-client-6.0.0a2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.135230 indico-client-6.0.0a3/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      697 2023-05-17 17:32:29.135230 indico-client-6.0.0a3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      370 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.135230 indico-client-6.0.0a3/indico/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-17 17:32:29.135230 indico-client-6.0.0a3/indico/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.123230 indico-client-6.0.0a3/indico/client/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/client/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.123230 indico-client-6.0.0a3/indico/config/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/config/config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.123230 indico-client-6.0.0a3/indico/filters/
+-rw-r--r--   0 root         (0) root         (0)     5896 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.123230 indico-client-6.0.0a3/indico/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6649 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/http/client.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/http/serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.127230 indico-client-6.0.0a3/indico/queries/
+-rw-r--r--   0 root         (0) root         (0)      326 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16872 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/document_report.py
+-rw-r--r--   0 root         (0) root         (0)     3694 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/documents.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/example.py
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/export.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/integration.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.127230 indico-client-6.0.0a3/indico/queries/model_groups/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/model_groups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/model_groups/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10356 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/model_groups/model_groups.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     4529 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/storage.py
+-rw-r--r--   0 root         (0) root         (0)    14363 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/submission.py
+-rw-r--r--   0 root         (0) root         (0)     5791 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/usermetrics.py
+-rw-r--r--   0 root         (0) root         (0)    18005 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/workflow.py
+-rw-r--r--   0 root         (0) root         (0)    15779 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/workflow_components.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/queries/workflow_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.131230 indico-client-6.0.0a3/indico/types/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/base.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/datafile.py
+-rw-r--r--   0 root         (0) root         (0)     3651 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/document_report.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/export.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/integration.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/jobs.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/model.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/model_group.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/model_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/submission.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/submission_file.py
+-rw-r--r--   0 root         (0) root         (0)     3543 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/user_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     9438 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/indico/types/workflow_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.131230 indico-client-6.0.0a3/indico_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-05-17 17:32:29.000000 indico-client-6.0.0a3/indico_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-05-17 17:32:29.000000 indico-client-6.0.0a3/indico_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 17:32:29.000000 indico-client-6.0.0a3/indico_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-17 17:32:29.000000 indico-client-6.0.0a3/indico_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 17:32:29.000000 indico-client-6.0.0a3/indico_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-17 17:32:29.135230 indico-client-6.0.0a3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      929 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.123230 indico-client-6.0.0a3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.131230 indico-client-6.0.0a3/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.131230 indico-client-6.0.0a3/tests/integration/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7904 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/data/datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.135230 indico-client-6.0.0a3/tests/integration/queries/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13233 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5233 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_document.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_document_report.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_export.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_job.py
+-rw-r--r--   0 root         (0) root         (0)     8927 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_model_group.py
+-rw-r--r--   0 root         (0) root         (0)     4685 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_user_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    15870 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_workflow.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_workflow_component.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/queries/test_workflow_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/integration/test_base_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 17:32:29.135230 indico-client-6.0.0a3/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/tests/unit/test_filters.py
+-rw-r--r--   0 root         (0) root         (0)    70238 2023-05-17 17:29:47.000000 indico-client-6.0.0a3/versioneer.py
```

### Comparing `indico-client-6.0.0a2/LICENSE` & `indico-client-6.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/PKG-INFO` & `indico-client-6.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indico-client
-Version: 6.0.0a2
+Version: 6.0.0a3
 Summary: A Python Wrapper for indico app API.
 Home-page: https://github.com/IndicoDataSolutions/indico-client-python
 Author: indico
 Author-email: engineering@indico.io
 License: MIT License (See LICENSE)
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `indico-client-6.0.0a2/indico/client/client.py` & `indico-client-6.0.0a3/indico/client/client.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/client/request.py` & `indico-client-6.0.0a3/indico/client/request.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/config/config.py` & `indico-client-6.0.0a3/indico/config/config.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/errors.py` & `indico-client-6.0.0a3/indico/errors.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/filters/__init__.py` & `indico-client-6.0.0a3/indico/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/http/client.py` & `indico-client-6.0.0a3/indico/http/client.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/http/serialization.py` & `indico-client-6.0.0a3/indico/http/serialization.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/datasets.py` & `indico-client-6.0.0a3/indico/queries/datasets.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/document_report.py` & `indico-client-6.0.0a3/indico/queries/document_report.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/documents.py` & `indico-client-6.0.0a3/indico/queries/documents.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/example.py` & `indico-client-6.0.0a3/indico/queries/example.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/export.py` & `indico-client-6.0.0a3/indico/queries/export.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/forms.py` & `indico-client-6.0.0a3/indico/queries/forms.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/integration.py` & `indico-client-6.0.0a3/indico/queries/integration.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/jobs.py` & `indico-client-6.0.0a3/indico/queries/jobs.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/model_groups/metrics.py` & `indico-client-6.0.0a3/indico/queries/model_groups/metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/model_groups/model_groups.py` & `indico-client-6.0.0a3/indico/queries/model_groups/model_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,15 +242,16 @@
             yield req
             while self.previous not in ["FAILED", "COMPLETE", "NOT_ENOUGH_DATA"]:
                 sleep(1)
                 yield req
 
         yield _GetModelGroup(id=model_group_id)
 
-
+@deprecation.deprecated(deprecated_in="6.0",
+                        details="Removed from platform. This call is a no-op.")
 class LoadModel(GraphQLRequest):
     """
     Load model into system cache (implicit in ModelGroupPredict unless load=False)
 
     Args:
         model_id= (int): selected model id use for predictions
 
@@ -268,15 +269,15 @@
         }
     """
 
     def __init__(self, model_id: int):
         super().__init__(self.query, variables={"modelId": model_id})
 
     def process_response(self, response):
-        return super().process_response(response)["modelLoad"]["status"]
+        return "ready"
 
 
 class _ModelGroupPredict(GraphQLRequest):
     query = """
         mutation ModelGroupPredict(<QUERY_ARGS>) {
             modelPredict(<MODEL_PREDICT_ARGS>) {
                 jobId
@@ -339,27 +340,15 @@
             model_id: int,
             data: List[str],
             load: bool = True,
             predict_options: Dict = None,
     ):
         self.model_id = model_id
         self.data = data
-        self.load = load
         self.predict_options = predict_options
 
     def requests(self):
-        retries = 0
-        if self.load:
-            while retries < 3 and self.previous != "ready":
-                retries += 1
-                yield LoadModel(self.model_id)
-                if retries > 0:
-                    sleep(1)
-            if self.previous != "ready":
-                raise IndicoError(
-                    f"Model {self.model_id} failed to load status {self.previous}"
-                )
 
         yield _ModelGroupPredict(
             model_id=self.model_id, data=self.data, predict_options=self.predict_options
         )
```

### Comparing `indico-client-6.0.0a2/indico/queries/questionnaire.py` & `indico-client-6.0.0a3/indico/queries/questionnaire.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from indico.client.request import (
     GraphQLRequest,
     RequestChain,
     Debouncer,
 )
 from indico.queries import AddModelGroupComponent
-from indico.types import NewLabelsetArguments, NewQuestionnaireArguments, Workflow
+from indico.types import NewLabelsetArguments, NewQuestionnaireArguments, Workflow, ModelTaskType
 
 from indico.types.questionnaire import Questionnaire, Example
 from indico.types.dataset import Dataset
 from indico.errors import IndicoNotFound, IndicoInputError, IndicoError
 
 
 class AddLabels(GraphQLRequest):
@@ -44,14 +44,15 @@
         """
 
     def __init__(
         self,
         labelset_id: int,
         labels: List[dict],
         model_group_id: int = None,
+        dataset_id: int = None
     ):
         super().__init__(
             query=self.query,
             variables={
                 "labels": labels,
                 "labelset_id": labelset_id,
                 "model_group_id": None,
@@ -293,18 +294,17 @@
         super().__init__()
 
     def requests(self):
         yield GetDataset(id=self.dataset_id)
         new_labelset_args = NewLabelsetArguments(
             datacolumn_id=self.previous.datacolumns[0].id,
             name=self.name,
-            task_type=self.task_type,
+            task_type=next(v for v in ModelTaskType if v.name == self.task_type),
             target_names=self.targets,
         )
-
         yield AddModelGroupComponent(
             workflow_id=self.workflow_id[0],
             source_column_id=self.previous.datacolumns[0].id,
             new_labelset_args=new_labelset_args,
             dataset_id=self.dataset_id,
             name=self.name,
             after_component_id=self.after_component_id,
```

### Comparing `indico-client-6.0.0a2/indico/queries/storage.py` & `indico-client-6.0.0a3/indico/queries/storage.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/submission.py` & `indico-client-6.0.0a3/indico/queries/submission.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/usermetrics.py` & `indico-client-6.0.0a3/indico/queries/usermetrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/queries/workflow.py` & `indico-client-6.0.0a3/indico/queries/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 import json
 from typing import List, Union, Dict
+import tempfile
 
 from indico.client.request import GraphQLRequest, RequestChain, Debouncer
 from indico.errors import IndicoError, IndicoInputError
 from indico.queries.storage import UploadDocument
 from indico.types import Job, Submission, Workflow, SUBMISSION_RESULT_VERSIONS
 from indico.types.utils import cc_to_snake, snake_to_cc
 
@@ -72,19 +73,20 @@
                   }
                 }
             }
         }
     """
 
     def __init__(
-            self, *, dataset_ids: List[int] = None, workflow_ids: List[int] = None, limit = 100
+            self, *, dataset_ids: List[int] = None, workflow_ids: List[int] = None, limit=100
     ):
         super().__init__(
             self.query,
-            variables={"datasetIds": dataset_ids, "workflowIds": workflow_ids, "limit": limit},
+            variables={"datasetIds": dataset_ids,
+                       "workflowIds": workflow_ids, "limit": limit},
         )
 
     def process_response(self, response) -> List[Workflow]:
         return [
             Workflow(**w)
             for w in super().process_response(response)["workflows"]["workflows"]
         ]
@@ -123,15 +125,16 @@
     """
 
     def __init__(self, workflow_id: int, enable_review: bool):
         query = self.query.replace("<QUERY NAME>", self.query_name)
         query = query.replace("<TOGGLE>", self.toggle)
         super().__init__(
             query,
-            variables={"workflowId": workflow_id, "reviewState": enable_review},
+            variables={"workflowId": workflow_id,
+                       "reviewState": enable_review},
         )
 
     def process_response(self, response) -> Workflow:
         return Workflow(**super().process_response(response)[self.query_name])
 
 
 class _ToggleAutoReview(_ToggleReview):
@@ -156,15 +159,16 @@
 
     def __init__(
             self,
             workflow: Union[Workflow, int],
             enable_review: bool = None,
             enable_auto_review: bool = None,
     ):
-        self.workflow_id = workflow.id if isinstance(workflow, Workflow) else workflow
+        self.workflow_id = workflow.id if isinstance(
+            workflow, Workflow) else workflow
         if enable_review is None and enable_auto_review is None:
             raise IndicoInputError("Must provide at least one review option")
 
         self.enable_review = enable_review
         self.enable_auto_review = enable_auto_review
 
     def requests(self):
@@ -239,30 +243,32 @@
             if detailed_response
             else self.query
         )
 
         args = [
             _arg for _arg in self.mutation_args.keys() if kwargs.get(cc_to_snake(_arg))
         ]
-        signature = ",".join(f"${_arg}: {self.mutation_args[_arg]}" for _arg in args)
+        signature = ",".join(
+            f"${_arg}: {self.mutation_args[_arg]}" for _arg in args)
         args = ",".join(f"{_arg}: ${_arg}" for _arg in args)
 
         super().__init__(
             query=q.format(
                 mutation_name=self.mutation_name, signature=signature, args=args
             ),
             variables={snake_to_cc(var): val for var, val in kwargs.items()},
         )
 
     def process_response(self, response):
         response = super().process_response(response)[self.mutation_name]
         if "submissions" in response:
             return [Submission(**s) for s in response["submissions"]]
         if not response["submissionIds"]:
-            raise IndicoError(f"Failed to submit to workflow {self.workflow_id}")
+            raise IndicoError(
+                f"Failed to submit to workflow {self.workflow_id}")
         else:
             return response["submissionIds"]
         return [Job(id=job_id) for job_id in response["jobIds"]]
 
 
 class _WorkflowUrlSubmission(_WorkflowSubmission):
     mutation_name = "workflowUrlSubmission"
@@ -284,14 +290,15 @@
         result_version (str, optional):
             The format of the submission result file. One of:
                 {SUBMISSION_RESULT_VERSIONS}
             If bundle is enabled, this must be version TWO or later.
         streams (Dict[str, io.BufferedIOBase]): List of filename keys mapped to streams
             for upload. Similar to files but mutually exclusive with files. 
             Can take for example: io.BufferedReader, io.BinaryIO, or io.BytesIO.
+        text (str, optional): text to submit. Note: submission may still go through OCR.
 
     Returns:
         List[int]: If `submission`, these will be submission ids.
             Otherwise, they will be AsyncJob ids.
 
     """
 
@@ -301,36 +308,45 @@
             self,
             workflow_id: int,
             files: List[str] = None,
             urls: List[str] = None,
             submission: bool = True,
             bundle: bool = False,
             result_version: str = None,
-            streams: Dict[str, io.BufferedIOBase] = None
+            streams: Dict[str, io.BufferedIOBase] = None,
+            text: str = ""
     ):
         self.workflow_id = workflow_id
         self.files = files
         self.urls = urls
         self.submission = submission
         self.bundle = bundle
         self.result_version = result_version
         self.has_streams = False
         if streams is not None:
             self.streams = streams.copy()
             self.has_streams = True
         else:
             self.streams = None
+        self.text = text
         if not submission:
-            raise IndicoInputError("This option is deprecated and no longer supported.")
-        if not self.files and not self.urls and not self.has_streams:
-            raise IndicoInputError("One of 'files', 'streams', or 'urls' must be specified")
-        elif self.files and self.has_streams:
-            raise IndicoInputError("Only one of 'files' or 'streams' or 'urls' may be specified.")
-        elif (self.files or self.has_streams) and self.urls:
-            raise IndicoInputError("Only one of 'files' or 'streams' or 'urls' may be specified")
+            raise IndicoInputError(
+                "This option is deprecated and no longer supported.")
+        if not self.files and not self.urls and not self.has_streams and not self.text:
+            raise IndicoInputError(
+                "One of 'files', 'streams', 'urls', or 'text' must be specified")
+        elif (self.files or self.urls or self.text) and self.has_streams:
+            raise IndicoInputError(
+                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified.")
+        elif (self.files or self.text) and self.urls:
+            raise IndicoInputError(
+                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified")
+        elif self.files and self.text:
+            raise IndicoInputError(
+                "Only one of 'files' or 'streams', 'urls', or 'text' may be specified")
 
     def requests(self):
         if self.files:
             yield UploadDocument(files=self.files)
             yield _WorkflowSubmission(
                 self.detailed_response,
                 workflow_id=self.workflow_id,
@@ -351,14 +367,29 @@
             yield _WorkflowSubmission(
                 self.detailed_response,
                 workflow_id=self.workflow_id,
                 files=self.previous,
                 bundle=self.bundle,
                 result_version=self.result_version,
             )
+        elif self.text:
+            temp = tempfile.NamedTemporaryFile(mode='w+', suffix='.txt')
+            try:
+                temp.write(self.text)
+                temp.seek(0)
+                yield UploadDocument(files=[temp.name])
+                yield _WorkflowSubmission(
+                    self.detailed_response,
+                    workflow_id=self.workflow_id,
+                    files=self.previous,
+                    bundle=self.bundle,
+                    result_version=self.result_version,
+                )
+            finally:
+                temp.close()
 
 
 class WorkflowSubmissionDetailed(WorkflowSubmission):
     f"""
     Submit files to a workflow for processing.
     One of `files` or `urls` is required.
     Submission recording is mandatory.
@@ -505,14 +536,15 @@
         )
 
     def process_response(self, response) -> Workflow:
         return Workflow(
             **super().process_response(response)["createWorkflow"]["workflow"]
         )
 
+
 class DeleteWorkflow(GraphQLRequest):
     """
     Mutation to delete workflow given workflow id. Note that this operation includes deleting 
     all components and models associated with this workflow.
 
     Args:
         workflow_id(int): id of workflow to delete
@@ -526,8 +558,8 @@
         }
     """
 
     def __init__(self, workflow_id: int):
         super().__init__(self.query, variables={"workflowId": workflow_id})
 
     def process_response(self, response) -> bool:
-        return super().process_response(response)["deleteWorkflow"]["success"]
+        return super().process_response(response)["deleteWorkflow"]["success"]
```

### Comparing `indico-client-6.0.0a2/indico/queries/workflow_components.py` & `indico-client-6.0.0a3/indico/queries/workflow_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,9 +440,7 @@
             variables={"workflowId": workflow_id, "componentId": component_id},
         )
 
     def process_response(self, response) -> Workflow:
         return Workflow(
             **super().process_response(response)["deleteWorkflowComponent"]["workflow"]
         )
-
- # TODO Add mutation to add output node
```

### Comparing `indico-client-6.0.0a2/indico/queries/workflow_metrics.py` & `indico-client-6.0.0a3/indico/queries/workflow_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/base.py` & `indico-client-6.0.0a3/indico/types/base.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/datafile.py` & `indico-client-6.0.0a3/indico/types/datafile.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/dataset.py` & `indico-client-6.0.0a3/indico/types/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 
 class OcrEngine(Enum):
     """
     Enum representing available OCR engines.
     """
     OMNIPAGE = 0
     READAPI = 1
+    READAPI_V2 = 2
     pass
 
 class OmnipageOcrOptionsInput(BaseType):
     """
     Omnipage specific OCR options for dataset creation.
 
     Args:
```

### Comparing `indico-client-6.0.0a2/indico/types/export.py` & `indico-client-6.0.0a3/indico/types/export.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/integration.py` & `indico-client-6.0.0a3/indico/types/integration.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/jobs.py` & `indico-client-6.0.0a3/indico/types/jobs.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/model.py` & `indico-client-6.0.0a3/indico/types/model.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/model_group.py` & `indico-client-6.0.0a3/indico/types/model_group.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/model_metrics.py` & `indico-client-6.0.0a3/indico/types/model_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/submission.py` & `indico-client-6.0.0a3/indico/types/submission.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/submission_file.py` & `indico-client-6.0.0a3/indico/types/submission_file.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/user_metrics.py` & `indico-client-6.0.0a3/indico/types/user_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/workflow.py` & `indico-client-6.0.0a3/indico/types/workflow.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico/types/workflow_metrics.py` & `indico-client-6.0.0a3/indico/types/workflow_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/indico_client.egg-info/PKG-INFO` & `indico-client-6.0.0a3/indico_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indico-client
-Version: 6.0.0a2
+Version: 6.0.0a3
 Summary: A Python Wrapper for indico app API.
 Home-page: https://github.com/IndicoDataSolutions/indico-client-python
 Author: indico
 Author-email: engineering@indico.io
 License: MIT License (See LICENSE)
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `indico-client-6.0.0a2/indico_client.egg-info/SOURCES.txt` & `indico-client-6.0.0a3/indico_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/setup.py` & `indico-client-6.0.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/data/datasets.py` & `indico-client-6.0.0a3/tests/integration/data/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,29 @@
         CreateDataset(
             name=f"TooSmall-test-{int(time.time())}", files=[dataset_filepath]
         )
     )
     assert response.status == "COMPLETE"
     return response
 
+@pytest.fixture(scope="module")
+def too_small_workflow(indico, too_small_dataset: Dataset) -> Workflow:
+    client = IndicoClient()
+    workflowreq = CreateWorkflow(dataset_id=too_small_dataset.id, name=f"TooSmall-test-{int(time.time())}")
+    wf = client.call(workflowreq)
+    # add default output node
+    client.call(_AddWorkflowComponent(after_component_id=wf.component_by_type("OUTPUT_JSON_FORMATTER").id,
+        component="{\"component_type\":\"default_output\",\"config\":{}}",
+        workflow_id=wf.id,
+        after_component_link=None
+    ))
+    response = client.call(GetWorkflow(workflow_id=wf.id))
+
+    return response
+
 
 @pytest.fixture(scope="module")
 def airlines_model_group(indico, airlines_dataset: Dataset, airlines_workflow: Workflow) -> ModelGroup:
     client = IndicoClient()
     name = f"TestCreateModelGroup-{int(time.time())}"
     after_component_id = airlines_workflow.component_by_type("INPUT_OCR_EXTRACTION").id
     modelgroupreq = AddModelGroupComponent(
```

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_dataset.py` & `indico-client-6.0.0a3/tests/integration/queries/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     DeleteDataset,
     CreateEmptyDataset,
     AddFiles,
     ProcessFiles,
     ProcessCSV,
 )
 from indico.queries.export import CreateExport, DownloadExport
-from indico.types.dataset import Dataset, OmnipageOcrOptionsInput, TableReadOrder, OcrEngine
+from indico.types.dataset import Dataset, OmnipageOcrOptionsInput, TableReadOrder, OcrEngine, ReadApiOcrOptionsInput
 from indico.errors import IndicoRequestError
 from tests.integration.data.datasets import airlines_dataset
 
 
 def test_create_dataset(indico):
     client = IndicoClient()
     dataset_filepath = str(Path(__file__).parents[1]) + "/data/AirlineComplaints.csv"
@@ -32,15 +32,14 @@
         )
     )
 
     assert isinstance(response, Dataset)
     assert response.status == "COMPLETE"
     assert isinstance(response.id, int)
 
-
 def test_get_datasets(indico, airlines_dataset):
     client = IndicoClient()
     dataset = client.call(GetDataset(id=airlines_dataset.id))
 
     assert isinstance(dataset, Dataset)
     assert dataset.id == airlines_dataset.id
 
@@ -185,15 +184,40 @@
         "force_render": False,
         "native_layout": False,
         "native_pdf": False,
         "table_read_order": TableReadOrder.ROW
     }
     dataset = client.call(CreateEmptyDataset(name=f"dataset-{int(time.time())}", ocr_engine=OcrEngine.OMNIPAGE,
                                              omnipage_ocr_options=config))
+    
+def test_create_with_options_readapi(indico):
+    client = IndicoClient()
+    config: ReadApiOcrOptionsInput = {
+        "auto_rotate": True,
+        "single_column": False,
+        "upscale_images": True,
+        "languages": ["AUTO"]
+    }
+    dataset = client.call(CreateEmptyDataset(name=f"dataset-{int(time.time())}", ocr_engine=OcrEngine.READAPI,
+                                             readapi_ocr_options=config))
+    
+def test_create_from_files_with_readapiv2(indico):
+    client = IndicoClient()
+    dataset = client.call(CreateEmptyDataset(name=f"dataset-{int(time.time())}", ocr_engine=OcrEngine.READAPI_V2))
+    file_names = ["us_doi.tiff", "mock.pdf"]
+    parent_path = str(Path(__file__).parent.parent / "data")
+    dataset_filepaths = [
+        os.path.join(parent_path, file_name) for file_name in file_names
+    ]
+
+    dataset = client.call(AddFiles(dataset_id=dataset.id, files=[dataset_filepaths[0]], autoprocess=True))
+    dataset = client.call(AddFiles(dataset_id=dataset.id, files=[dataset_filepaths[1]], autoprocess=True))
 
+    _dataset_complete(dataset)
+    
 
 def test_create_from_files_document_without_autoprocess(indico):
     client = IndicoClient()
     dataset = client.call(CreateEmptyDataset(name=f"dataset-{int(time.time())}"))
     file_names = ["us_doi.tiff", "mock.pdf"]
     parent_path = str(Path(__file__).parent.parent / "data")
     dataset_filepaths = [
```

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_document.py` & `indico-client-6.0.0a3/tests/integration/queries/test_document.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_document_report.py` & `indico-client-6.0.0a3/tests/integration/queries/test_document_report.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_export.py` & `indico-client-6.0.0a3/tests/integration/queries/test_export.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_integration.py` & `indico-client-6.0.0a3/tests/integration/queries/test_integration.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_job.py` & `indico-client-6.0.0a3/tests/integration/queries/test_job.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_model_group.py` & `indico-client-6.0.0a3/tests/integration/queries/test_model_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     cats_dogs_image_dataset,
     cats_dogs_modelgroup,
     org_annotate_model_group,
     org_annotate_dataset,
 cats_dogs_image_workflow,
 airlines_workflow
 )
-from indico.errors import IndicoNotFound
+from indico.errors import IndicoRequestError
 
 
 def test_create_model_group(airlines_dataset: Dataset, airlines_workflow: Workflow):
     client = IndicoClient()
 
     name = f"TestCreateModelGroup-{int(time.time())}"
     after_component = airlines_workflow.component_by_type("INPUT_OCR_EXTRACTION")
@@ -50,19 +50,18 @@
             source_column_id=airlines_dataset.datacolumn_by_name("Text").id,
             labelset_id=airlines_dataset.labelset_by_name("Target_1").id,
         )
     )
 
     assert mg.name == name
 
-
 def test_get_missing_model_group(indico):
     client = IndicoClient()
 
-    with pytest.raises(IndicoNotFound):
+    with pytest.raises(IndicoRequestError):
         client.call(GetModelGroup(id=500000))
 
 
 def test_object_detection(cats_dogs_image_dataset: Dataset, cats_dogs_image_workflow: Workflow):
     client = IndicoClient()
     name = f"TestCreateObjectDetectionMg-{int(time.time())}"
 
@@ -107,58 +106,63 @@
         )
     )
 
     assert mg.name == name
     assert mg.selected_model.status == "COMPLETE"
 
 
-def test_create_model_group_with_wait_not_enough_data(indico, too_small_dataset):
+def test_create_model_group_with_wait_not_enough_data(indico, too_small_dataset: Dataset, too_small_workflow: Workflow):
     client = IndicoClient()
 
     name = f"TestCreateModelGroup-{int(time.time())}"
+    after_component_id = too_small_workflow.component_by_type("INPUT_OCR_EXTRACTION").id
     mg: ModelGroup = client.call(
         CreateModelGroup(
             name=name,
+            workflow_id=too_small_workflow.id,
             dataset_id=too_small_dataset.id,
             source_column_id=too_small_dataset.datacolumn_by_name("Text").id,
             labelset_id=too_small_dataset.labelset_by_name("Target_1").id,
+            after_component_id=after_component_id,
             wait=True,
         )
     )
 
     assert mg.name == name
     assert mg.selected_model.status == "NOT_ENOUGH_DATA"
 
 
-def test_model_group_progress(indico, airlines_dataset: Dataset):
+def test_model_group_progress(indico, airlines_dataset: Dataset, airlines_workflow: Workflow):
     client = IndicoClient()
 
     name = f"TestCreateModelGroup-{int(time.time())}"
+    after_component_id = airlines_workflow.component_by_type("INPUT_OCR_EXTRACTION").id
     mg: ModelGroup = client.call(
         CreateModelGroup(
             name=name,
+            workflow_id=airlines_workflow.id,
             dataset_id=airlines_dataset.id,
             source_column_id=airlines_dataset.datacolumn_by_name("Text").id,
             labelset_id=airlines_dataset.labelset_by_name("Target_1").id,
             wait=False,
+            after_component_id=after_component_id
         )
     )
     time.sleep(1)
     model: Model = client.call((GetTrainingModelWithProgress(id=mg.id)))
 
     assert type(model) == Model
     assert model.status in ["CREATING", "TRAINING", "COMPLETE"]
     assert type(model.training_progress) == TrainingProgress
     assert model.training_progress.percent_complete < 101.0
 
-
 def test_model_group_progress_bad_model_group_id(indico, airlines_dataset: Dataset):
     client = IndicoClient()
 
-    with pytest.raises(IndicoNotFound):
+    with pytest.raises(IndicoRequestError):
         client.call((GetTrainingModelWithProgress(id=-1)))
 
 
 def test_predict(indico, airlines_dataset, airlines_model_group):
     client = IndicoClient()
 
     job = client.call(
```

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_questionnaire.py` & `indico-client-6.0.0a3/tests/integration/queries/test_questionnaire.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,20 +24,24 @@
     client = IndicoClient()
     datasets_dir = Path(__file__).parents[1] / "data"
     files = [str(datasets_dir / f"pdf{f}.pdf") for f in range(3)]
 
     dataset = client.call(
         CreateDataset(name=f"CreateDataset-test-{int(time.time())}", files=files)
     )
+    workflow: Workflow = client.call(CreateWorkflow(name=f"CreateWorkflow-test{int(time.time())}", dataset_id=dataset.id))
+    after_component = workflow.component_by_type("INPUT_OCR_EXTRACTION").id
 
     questionnaire = client.call(
         CreateQuestionaire(
             name=f"CreateDatasetTeach-test-{int(time.time())}",
             dataset_id=dataset.id,
             targets=["A", "B", "C"],
+            workflow_id=workflow.id,
+            after_component_id=after_component
         )
     )
     return {"dataset": dataset, "questionnaire": questionnaire}
 
 
 def test_create_questionnaire_no_labels(unlabeled_questionnaire):
     assert isinstance(unlabeled_questionnaire["questionnaire"], Questionnaire)
@@ -48,15 +52,14 @@
     datasets_dir = Path(__file__).parents[1] / "data"
     csv_path = datasets_dir / "staffer_large.csv"
     files = [str(datasets_dir / f"pdf{f}.pdf") for f in range(3)]
 
     dataset = client.call(
         CreateDataset(name=f"CreateDataset-test-{int(time.time())}", files=files)
     )
-
     workflow: Workflow = client.call(CreateWorkflow(name=f"CreateWorkflow-test{int(time.time())}", dataset_id=dataset.id))
     after_component = workflow.component_by_type("INPUT_OCR_EXTRACTION").id
     csv = pd.read_csv(csv_path)
     data = {
         string: json.loads(label) for string, label in zip(csv["text"], csv["labels"])
     }
     targets = list(set(t["label"] for sample in data.values() for t in sample))
@@ -70,29 +73,28 @@
             workflow_id=workflow.id,
             after_component_id=after_component
         )
     )
 
     assert isinstance(response, Questionnaire)
 
-
 def test_get_nonexistent_questionnaire(indico):
     client = IndicoClient()
     with pytest.raises(IndicoError):
         client.call(GetQuestionnaire(123454321))
 
 
 def test_get_questionnaire(indico, unlabeled_questionnaire):
     client = IndicoClient()
     response = client.call(
         GetQuestionnaire(unlabeled_questionnaire["questionnaire"].id)
     )
     assert isinstance(response, Questionnaire)
     assert response.id == unlabeled_questionnaire["questionnaire"].id
-    assert response.odl is True
+    assert not response.odl
     assert response.num_total_examples == 3
     assert response.num_fully_labeled == 0
 
 
 def test_get_examples(indico, unlabeled_questionnaire):
     client = IndicoClient()
     examples = client.call(
```

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_user_metrics.py` & `indico-client-6.0.0a3/tests/integration/queries/test_user_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_workflow.py` & `indico-client-6.0.0a3/tests/integration/queries/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,41 @@
     assert result["submission_id"] == submission_id
     assert result["file_version"] == 1
     client.call(UpdateSubmission(submission_id, retrieved=True))
     sub = client.call(GetSubmission(submission_id))
     assert isinstance(sub, Submission)
     assert sub.retrieved is True
 
+def test_workflow_submission_with_text(
+    indico, airlines_dataset, airlines_model_group: ModelGroup
+):
+    client = IndicoClient()
+    wfs = client.call(ListWorkflows(dataset_ids=[airlines_dataset.id]))
+    wf = max(wfs, key=lambda w: w.id)
+
+    submission_ids = client.call(WorkflowSubmission(workflow_id=wf.id, text="hello this is a test"))
+    submission_id = submission_ids[0]
+    assert submission_id is not None
+
+    with pytest.raises(IndicoInputError):
+        client.call(SubmissionResult(submission_id, "FAILED"))
+
+    with pytest.raises(IndicoInputError):
+        client.call(SubmissionResult(submission_id, "INVALID_STATUS"))
+
+    result_url = client.call(SubmissionResult(submission_id, "COMPLETE", wait=True))
+    result = client.call(RetrieveStorageObject(result_url.result))
+    assert isinstance(result, dict)
+    assert result["submission_id"] == submission_id
+    assert result["file_version"] == 1
+    client.call(UpdateSubmission(submission_id, retrieved=True))
+    sub = client.call(GetSubmission(submission_id))
+    assert isinstance(sub, Submission)
+    assert sub.retrieved is True
+
 
 
 @pytest.mark.parametrize(
     "_input",
     [
         {"urls": [PUBLIC_URL + "mock.pdf"] * 3},
         {"files": [str(Path(__file__).parents[1]) + "/data/mock.pdf"] * 3},
@@ -141,15 +168,15 @@
     submission_id = submission_ids[0]
     assert submission_id is not None
 
     submissions = client.call(WaitForSubmissions(submission_id))
     result = client.call(RetrieveStorageObject(submissions[0].result_file))
 
     assert isinstance(result, dict)
-    assert result["file_version"] == 2
+    assert result["file_version"] == 3
     assert len(result["submission_results"]) == 1
     assert result["submission_results"][0]["input_filename"] == "mock.pdf"
 
 
 @pytest.mark.parametrize(
     "_input",
     [
@@ -174,15 +201,15 @@
     submission_id = submission_ids[0]
     assert submission_id
 
     submissions = client.call(WaitForSubmissions(submission_id))
     result = client.call(RetrieveStorageObject(submissions[0].result_file))
 
     assert isinstance(result, dict)
-    assert result["file_version"] == 2
+    assert result["file_version"] == 3
     assert len(result["submission_results"]) == len(next(iter(_input.values())))
     assert result["submission_results"][0]["input_filename"] == "mock.pdf"
 
 
 @pytest.mark.parametrize(
     "_input,_output",
     [
```

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_workflow_component.py` & `indico-client-6.0.0a3/tests/integration/queries/test_workflow_component.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/queries/test_workflow_metrics.py` & `indico-client-6.0.0a3/tests/integration/queries/test_workflow_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/tests/integration/test_base_client.py` & `indico-client-6.0.0a3/tests/integration/test_base_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,26 +54,23 @@
         }
     }
     """
         )
     )
     assert "modelGroups" in response
 
-
 def test_graphql_with_ids():
     client = IndicoClient()
     response = client.call(
         GraphQLRequest(
             query="""
-            query modelGroupQueries($ids: [Int]) {
-	            modelGroups(modelGroupIds: $ids){
-                    modelGroups{
-                        id
-                    }
+            query datasetQueries($id: Int!) {
+	            dataset(id: $id){
+                    id
                 }
             }
         """,
-            variables={"ids": [1]},
+            variables={"id": 1},
         )
     )
 
-    assert "modelGroups" in response
+    assert "dataset" in response
```

### Comparing `indico-client-6.0.0a2/tests/unit/test_filters.py` & `indico-client-6.0.0a3/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.0.0a2/versioneer.py` & `indico-client-6.0.0a3/versioneer.py`

 * *Files identical despite different names*

