# Comparing `tmp/energinet-ml-sdk-0.9.2.dev87.tar.gz` & `tmp/energinet-ml-sdk-1.0.0.dev24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energinet-ml-sdk-0.9.2.dev87.tar", last modified: Thu Mar  3 11:38:06 2022, max compression
+gzip compressed data, was "energinet-ml-sdk-1.0.0.dev24.tar", last modified: Wed May 17 14:36:16 2023, max compression
```

## Comparing `energinet-ml-sdk-0.9.2.dev87.tar` & `energinet-ml-sdk-1.0.0.dev24.tar`

### file list

```diff
@@ -1,137 +1,102 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.072668 energinet-ml-sdk-0.9.2.dev87/
--rw-r--r--   0 root         (0) root         (0)      592 2022-03-03 11:38:06.072668 energinet-ml-sdk-0.9.2.dev87/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1733 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.032668 energinet-ml-sdk-0.9.2.dev87/energinetml/
--rw-r--r--   0 root         (0) root         (0)     1708 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      122 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.032668 energinet-ml-sdk-0.9.2.dev87/energinetml/azure/
--rw-r--r--   0 root         (0) root         (0)      210 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10809 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/azure/backend.py
--rw-r--r--   0 root         (0) root         (0)     6295 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/azure/datasets.py
--rw-r--r--   0 root         (0) root         (0)     4292 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/azure/interactive.py
--rw-r--r--   0 root         (0) root         (0)     2130 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/azure/logger.py
--rw-r--r--   0 root         (0) root         (0)     1135 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/azure/submitting.py
--rw-r--r--   0 root         (0) root         (0)     7209 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/azure/training.py
--rw-r--r--   0 root         (0) root         (0)      190 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.032668 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/
--rw-r--r--   0 root         (0) root         (0)     1041 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.042668 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/cluster/
--rw-r--r--   0 root         (0) root         (0)      382 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/cluster/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2038 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/cluster/change.py
--rw-r--r--   0 root         (0) root         (0)     6797 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/cluster/create.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.042668 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/infrastructure/
--rw-r--r--   0 root         (0) root         (0)      351 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/infrastructure/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7297 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/infrastructure/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.042668 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/
--rw-r--r--   0 root         (0) root         (0)      820 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      969 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/build.py
--rw-r--r--   0 root         (0) root         (0)      376 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/files.py
--rw-r--r--   0 root         (0) root         (0)     3885 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/init.py
--rw-r--r--   0 root         (0) root         (0)     2278 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/predict.py
--rw-r--r--   0 root         (0) root         (0)     5178 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/release.py
--rw-r--r--   0 root         (0) root         (0)     1041 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/serve.py
--rw-r--r--   0 root         (0) root         (0)     4081 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/submit.py
--rw-r--r--   0 root         (0) root         (0)     4674 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.042668 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/project/
--rw-r--r--   0 root         (0) root         (0)      281 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/project/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/project/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.042668 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/utils/
--rw-r--r--   0 root         (0) root         (0)      384 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9325 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)    10233 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/utils/projects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.052668 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/webapp/
--rw-r--r--   0 root         (0) root         (0)      410 2022-03-03 11:37:41.192669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/webapp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      562 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/webapp/build.py
--rw-r--r--   0 root         (0) root         (0)     4515 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/webapp/init.py
--rw-r--r--   0 root         (0) root         (0)      618 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/cli/webapp/serve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.052668 energinet-ml-sdk-0.9.2.dev87/energinetml/core/
--rw-r--r--   0 root         (0) root         (0)       33 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4530 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/backend.py
--rw-r--r--   0 root         (0) root         (0)     3649 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/configurable.py
--rw-r--r--   0 root         (0) root         (0)     3079 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/docker.py
--rw-r--r--   0 root         (0) root         (0)     3022 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/files.py
--rw-r--r--   0 root         (0) root         (0)     7681 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/http.py
--rw-r--r--   0 root         (0) root         (0)     4419 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/insight.py
--rw-r--r--   0 root         (0) root         (0)     3802 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/logger.py
--rw-r--r--   0 root         (0) root         (0)    16093 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/model.py
--rw-r--r--   0 root         (0) root         (0)    11449 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/predicting.py
--rw-r--r--   0 root         (0) root         (0)     4144 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/project.py
--rw-r--r--   0 root         (0) root         (0)     1871 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/requirements.py
--rw-r--r--   0 root         (0) root         (0)      595 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/submitting.py
--rw-r--r--   0 root         (0) root         (0)     8722 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/templates.py
--rw-r--r--   0 root         (0) root         (0)     2867 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/training.py
--rw-r--r--   0 root         (0) root         (0)    13644 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/validation.py
--rw-r--r--   0 root         (0) root         (0)     1265 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/core/webapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.052668 energinet-ml-sdk-0.9.2.dev87/energinetml/meta/
--rw-r--r--   0 root         (0) root         (0)       12 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/meta/COMMAND_NAME
--rw-r--r--   0 root         (0) root         (0)       17 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/meta/PACKAGE_NAME
--rw-r--r--   0 root         (0) root         (0)       11 2022-03-03 11:38:05.522668 energinet-ml-sdk-0.9.2.dev87/energinetml/meta/PACKAGE_VERSION
--rw-r--r--   0 root         (0) root         (0)        4 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/meta/PYTHON_VERSION
--rw-r--r--   0 root         (0) root         (0)     2479 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.052668 energinet-ml-sdk-0.9.2.dev87/energinetml/static/
--rw-r--r--   0 root         (0) root         (0)      531 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/static/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.052668 energinet-ml-sdk-0.9.2.dev87/energinetml/static/model_template/
--rw-r--r--   0 root         (0) root         (0)      233 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/static/model_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2079 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/energinetml/static/model_template/model.py
--rw-r--r--   0 root         (0) root         (0)     4742 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4730 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/ml/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/ml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      810 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/ml/model.py
--rw-r--r--   0 root         (0) root         (0)    15081 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/ml/smoke_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/ml_deployment/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/ml_deployment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1091 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/ml_deployment/deployment_smoke_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/webapp_deployment/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/webapp_deployment/__init__.py
--rw-r--r--   0 root         (0) root         (0)      515 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/smoketest/webapp_deployment/deployment_smoke_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/azure_/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/azure_/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9598 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/azure_/backend_test.py
--rw-r--r--   0 root         (0) root         (0)     4350 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/azure_/datasets_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/cluster/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/cluster/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2892 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/cluster/change_test.py
--rw-r--r--   0 root         (0) root         (0)     9457 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/cluster/create_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.062668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/infrastructure/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/infrastructure/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3517 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/infrastructure/init_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.072668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2371 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/build_test.py
--rw-r--r--   0 root         (0) root         (0)     2040 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/files_test.py
--rw-r--r--   0 root         (0) root         (0)     3739 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/init_test.py
--rw-r--r--   0 root         (0) root         (0)     6791 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/predict_test.py
--rw-r--r--   0 root         (0) root         (0)     2187 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/release_test.py
--rw-r--r--   0 root         (0) root         (0)     4562 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/submit_test.py
--rw-r--r--   0 root         (0) root         (0)     3424 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/train_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.072668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/project/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/project/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2310 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/project/init_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.072668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4480 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/utils/decorators_test.py
--rw-r--r--   0 root         (0) root         (0)     7760 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/utils/projects_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-03 11:38:06.072668 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/backend_test.py
--rw-r--r--   0 root         (0) root         (0)     1126 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/configurable_test.py
--rw-r--r--   0 root         (0) root         (0)     1889 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/docker_test.py
--rw-r--r--   0 root         (0) root         (0)     1069 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/files_test.py
--rw-r--r--   0 root         (0) root         (0)    11355 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/http_test.py
--rw-r--r--   0 root         (0) root         (0)    13338 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/insight_test.py
--rw-r--r--   0 root         (0) root         (0)     2106 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/logger_test.py
--rw-r--r--   0 root         (0) root         (0)     9230 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/model_test.py
--rw-r--r--   0 root         (0) root         (0)     1638 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/predicting_test.py
--rw-r--r--   0 root         (0) root         (0)     2387 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/predicting_validator_test.py
--rw-r--r--   0 root         (0) root         (0)     2874 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/project_test.py
--rw-r--r--   0 root         (0) root         (0)     2378 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/requirements_test.py
--rw-r--r--   0 root         (0) root         (0)      812 2022-03-03 11:37:41.202669 energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/submitting_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/
+-rw-r--r--   0 vsts      (1001) docker     (123)      592 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1733 2023-05-17 14:36:05.147612 energinet-ml-sdk-1.0.0.dev24/README
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/
+-rw-r--r--   0 vsts      (1001) docker     (123)      210 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13179 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8140 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/datasets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4352 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2130 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/submitting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6853 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/azure/training.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      190 2023-05-17 14:36:05.151613 energinet-ml-sdk-1.0.0.dev24/energinetml/backend.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)      833 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      581 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/files.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3886 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/init.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3133 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/release.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5525 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/submit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5250 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/train.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/project/init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7294 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11202 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/projects.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2062 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/verify.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/core/
+-rw-r--r--   0 vsts      (1001) docker     (123)       33 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4552 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4381 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/configurable.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3006 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/files.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3760 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27424 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2555 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1871 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/requirements.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/submitting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9048 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/templates.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3293 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/core/training.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/
+-rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/COMMAND_NAME
+-rw-r--r--   0 vsts      (1001) docker     (123)       17 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/PACKAGE_NAME
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-05-17 14:36:16.179858 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/PACKAGE_VERSION
+-rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/meta/PYTHON_VERSION
+-rw-r--r--   0 vsts      (1001) docker     (123)     2793 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/settings.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/static/
+-rw-r--r--   0 vsts      (1001) docker     (123)      492 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/static/Dockerfile
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.523867 energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      147 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1728 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4490 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      715 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/constants.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/ml_deployment/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/ml_deployment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/ml_deployment/deployment_smoke_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/webapp_deployment/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/webapp_deployment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      515 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/smoketest/webapp_deployment/deployment_smoke_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.155613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8099 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/backend_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4350 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/datasets_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      675 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/training_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      899 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/files_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3739 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/init_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/release_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9074 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/submit_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3566 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/train_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2310 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/project/init_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4922 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/decorators_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7759 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/projects_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:16.527868 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2197 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/backend_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1126 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/configurable_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/files_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/logger_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14679 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/model_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2874 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/project_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2378 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/requirements_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-05-17 14:36:05.159613 energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/submitting_test.py
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/PKG-INFO` & `energinet-ml-sdk-1.0.0.dev24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energinet-ml-sdk
-Version: 0.9.2.dev87
+Version: 1.0.0.dev24
 Summary: Energinet Machine Learning
 Home-page: UNKNOWN
 Author: Koncern Digitalisering Advanced Analytics Team
 Author-email: mny@energinet.dk, xjakk@energinet.dk
 License: Apache Software License 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/README` & `energinet-ml-sdk-1.0.0.dev24/README`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/azure/datasets.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/datasets.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,33 +5,39 @@
 import io
 import os
 from typing import TYPE_CHECKING, Dict, Iterable, List, Tuple, Union
 
 from azureml import exceptions
 from azureml.core import Dataset, Workspace
 from azureml.data import FileDataset, TabularDataset
+from pandas import DataFrame
 
 from energinetml.settings import DEFAULT_ENCODING
 
 if TYPE_CHECKING:
     from energinetml.core.model import Model
 
 
 class MLDataSet:
     """[summary]"""
 
-    def __init__(self, name: str, mount_path: str) -> None:
+    def __init__(
+        self, name: str, mount_path: str = None, dataframe: DataFrame = None
+    ) -> None:
         """[summary]
 
         Args:
             name (str): [description]
             mount_path (str): [description]
+            dataframe (DataFrame, optional): Dataframe of the dataset.
+            This is set if the dataset is tabular. Defaults to None.
         """
         self.name = name
         self.mount_path = mount_path
+        self.dataframe = dataframe
 
     def __str__(self) -> str:
         """[summary]
 
         Returns:
             str: [description]
         """
@@ -68,18 +74,42 @@
         Returns:
             bool: [description]
         """
         return os.path.exists(self.path(*relative_path))
 
 
 class MLDataStore(Dict[str, "MLDataSet"]):
-    """A class
+    """A class that works as a dictionary of registered datasets in
+    :func:`~energinetml.Model.train`.
+
+    Example:
+        When in the :func:`~energinetml.Model.train`-function,
+        you can acces a dataset in this way:
+        .. code-block:: python
+
+            # We access the "iris" dataset using its name as key:
+            iris_dataset = datasets['iris']
+
+            # To access files within the iris dataset, we can use the path() method,
+            # which returns an absolute path to a file in the dataset.
+            # In this case, the dataset has a "iris.csv" file:
+            iris_file_path = iris_dataset.path('iris.csv')
+
+            # Be aware that accessing files within sub-folders should be done
+            # using the same approach as when using os.path.join() to allow
+            # compatibility across different operating systems.
+            # The following returns the path to file "some-folder/iris2.csv":
+            iris_file_path2 = iris_dataset.path('some-folder', 'iris2.csv')
+
+            # With this we can open and read the file:
+            with open(iris_file_path, 'r') as fp:
+                iris_raw_data = fp.read()
+
+            # The rest of your training script goes here
 
-    Args:
-        Dict (str, MLDataSet): A dictionary of datasets
     """
 
     class DataSetNotFound(Exception):
         """[summary]"""
 
         pass
 
@@ -186,18 +216,24 @@
             model (Model): [description]
             azureml_dataset ([type]): [description]
             force_download (bool): [description]
 
         Returns:
             MLDataSet: [description]
         """
-        mount_context = azureml_dataset.mount()
-        mount_point = mount_context.mount_point
-        mount_context.start()
-        return MLDataSet(name=azureml_dataset.name, mount_path=mount_point)
+        # We don't need to download tabular datasets because we already know the schema.
+        if isinstance(azureml_dataset, TabularDataset):
+            df = azureml_dataset.to_pandas_dataframe()
+            return MLDataSet(name=azureml_dataset.name, dataframe=df)
+
+        else:
+            mount_context = azureml_dataset.mount()
+            mount_point = mount_context.mount_point
+            mount_context.start()
+            return MLDataSet(name=azureml_dataset.name, mount_path=mount_point)
 
 
 class DownloadedAzureMLDataStore(AzureMLDataStore):
     """[summary]"""
 
     @classmethod
     def mount(
@@ -209,17 +245,21 @@
             model (Model): [description]
             azureml_dataset (TabularDataset): [description]
             force_download (bool): [description]
 
         Returns:
             MLDataSet: [description]
         """
+
+        # We don't need to download tabular datasets because we already know the schema.
+        if isinstance(azureml_dataset, TabularDataset):
+            df = azureml_dataset.to_pandas_dataframe()
+            return MLDataSet(name=azureml_dataset.name, dataframe=df)
+
         mount_point = os.path.join(model.data_folder_path, azureml_dataset.name)
         try:
-            if isinstance(azureml_dataset, TabularDataset):
-                azureml_dataset = azureml_dataset.to_parquet_files()
             azureml_dataset.download(mount_point, overwrite=force_download)
         except exceptions._azureml_exception.UserErrorException:
             # Dataset already exists on filesystem
             # TODO Rethink this solution
             print("NOTICE: Using cached dataset (from filesystem)")
         return MLDataSet(name=azureml_dataset.name, mount_path=mount_point)
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/azure/interactive.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/interactive.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,34 +23,34 @@
     """Azure interactive context that enables an interactive session with Azure ML
 
     Args:
         experiment_name (str): [description]
         workspace_name (str): [description]
         subscription_id (str): [description]
         resource_group (str): [description]
-        dataset_dependecies (List[str]): [description]
+        dataset_dependencies (List[str]): [description]
         force_download (bool, optional): [description]. Defaults to False.
 
     Attributes:
         logger (MetricsLogger): a Logger
         seed: Your seed
         datasets (MLDataStore): datasets
 
     Raises:
         AbstractBackend.BackendException: [description]
 
     Example:
-        Your can do this:
+        You can do this:
 
         >>> ctx = AzureInteractiveTrainingContext(
         ...     experiment_name="",
         ...     workspace_name="",
         ...     subscription_id="",
         ...     resource_group="",
-        ...     dataset_dependecies=[])
+        ...     dataset_dependencies=[])
         >>> logger = ctx.logger
         >>> seed = ctx.seed
         >>> datasets = ctx.datasets
 
     """
 
     logger: MetricsLogger
@@ -59,41 +59,42 @@
 
     def __init__(
         self,
         experiment_name: str,
         workspace_name: str,
         subscription_id: str,
         resource_group: str,
-        dataset_dependecies: List[str],
+        dataset_dependencies: List[str],
         force_download: bool = False,
     ):
         """[summary]
 
         Args:
             experiment_name (str): [description]
             workspace_name (str): [description]
             subscription_id (str): [description]
             resource_group (str): [description]
-            dataset_dependecies (List[str]): [description]
+            dataset_dependencies (List[str]): [description]
             force_download (bool, optional): [description]. Defaults to False.
 
         Raises:
             AbstractBackend.BackendException: [description]
         """
         backend = AzureBackend()
 
-        az_workspace = backend.get_workspace(
-            name=workspace_name,
-            subscription_id=subscription_id,
-            resource_group=resource_group,
-        )
+        project_meta = {
+            "workspace_name": workspace_name,
+            "subscription_id": subscription_id,
+            "resource_group": resource_group,
+        }
+        az_workspace = backend.get_workspace(project_meta)
 
         az_experiment = Experiment(workspace=az_workspace, name=experiment_name)
 
-        datasets_parsed = [dataset.split(":") for dataset in dataset_dependecies]
+        datasets_parsed = [dataset.split(":") for dataset in dataset_dependencies]
 
         model_class = Mock()
         model_class.data_folder_path = "data"
 
         datasets = DownloadedAzureMLDataStore.from_model(
             model=model_class,
             datasets=datasets_parsed,
@@ -104,21 +105,21 @@
         try:
             self.az_run = az_experiment.start_logging(snapshot_directory=None)
         except azureml._common.exceptions.AzureMLException as e:
             raise self.backend.parse_azureml_exception(e)
 
         logger = AzureMlLogger(self.az_run)
 
-        seed = random.randint(0, 10 ** 9)
+        seed = random.randint(0, 10**9)
 
         tags = {
             "seed": seed,
             PACKAGE_NAME: PACKAGE_VERSION,
             "python-version": PYTHON_VERSION,
-            "datasets": dataset_dependecies,
+            "datasets": dataset_dependencies,
         }
 
         self.az_run.set_tags(tags)
 
         self.datasets = datasets
         self.logger = logger
         self.seed = seed
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/azure/logger.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/logger.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/azure/training.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/azure/training.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,131 @@
 """[summary]
 """
+import json
 import os
-from typing import TYPE_CHECKING, Any, Dict  # noqa TYP001
+from typing import TYPE_CHECKING, Any, Dict, List
 
 import azureml
 from azureml.core import Experiment, Run
 
 from energinetml.azure.datasets import (
     DownloadedAzureMLDataStore,
     MountedAzureMLDataStore,
 )
 from energinetml.azure.logger import AzureMlLogger
 from energinetml.core.logger import ConsoleLogger
-from energinetml.core.model import Model, TrainedModel
 from energinetml.core.training import AbstractTrainingContext
+from energinetml.settings import DEFAULT_RELATIVE_ARTIFACT_PATH
 
 if TYPE_CHECKING:
     from energinetml.azure.backend import AzureBackend
+    from energinetml.core.model import Model, TrainedModel
 
 
-class AzureLocalTrainingContext(AbstractTrainingContext):
+class AzureTrainingContext(AbstractTrainingContext):
+    def save_artifacts(self, model: "Model"):
+        """Save model artifacts to cloud.
+
+        Args:
+            model (Model): [description]
+
+        Raises:
+            AbstractBackend.BackendException: [description]
+        """
+        try:
+            self.az_run.upload_folder(
+                name=DEFAULT_RELATIVE_ARTIFACT_PATH, path=model.artifact_path
+            )
+        except azureml._common.exceptions.AzureMLException as ex:
+            raise self.backend.parse_azureml_exception(ex)
+
+    def save_logs(self, *cloggers: List[ConsoleLogger]):
+        try:
+            for clogger in cloggers:
+                clogger.flush()
+                self.az_run.upload_file(clogger.filename, clogger.filepath)
+        except azureml._common.exceptions.AzureMLException as ex:
+            raise self.backend.parse_azureml_exception(ex)
+
+    def save_meta_data(self, meta_data: Dict[str, str], meta_file_path: str):
+        """Create a meta json-file with the content from a meta_data dictionary
+        and save it to the path specified.
+
+        Args:
+            meta_data (Dict[str, str])): A dictionary of meta_data to persist in the
+            json-file
+            meta_file_path (str): The local path where the json-file is persisted.
+
+        """
+        json_object = json.dumps(meta_data, indent=4)
+        with open(meta_file_path, "w") as outfile:
+            outfile.write(json_object)
+
+    def get_portal_url(self) -> str:
+        """Retrieve the URL to the AzureML Run.
+
+        Raises:
+            AbstractBackend.BackendException: [description]
+
+        Returns:
+            str:
+        """
+        try:
+            return self.az_run.get_portal_url()
+        except azureml._common.exceptions.AzureMLException as ex:
+            raise self.backend.parse_azureml_exception(ex)
+
+
+class AzureLocalTrainingContext(AzureTrainingContext):
     """[summary]"""
 
     def __init__(self, backend: "AzureBackend", force_download: bool):
         """[summary]
 
         Args:
             backend (AzureBackend): [description]
             force_download (bool): [description]
         """
         self.backend = backend
         self.force_download = force_download
         self.az_run = None
 
-    def train_model(self, model: Model, tags: Dict[str, Any], **kwargs) -> TrainedModel:
+    def train_model(
+        self, model: "Model", tags: Dict[str, Any], **kwargs
+    ) -> "TrainedModel":
         """[summary]
 
         Args:
             model (Model): [description]
             tags (Dict[str, Any]): [description]
 
         Raises:
             AbstractBackend.BackendException: [description]
             AbstractBackend.BackendException: [description]
 
         Returns:
             TrainedModel: [description]
         """
-        az_workspace = self.backend.get_workspace(
-            name=model.project.workspace_name,
-            subscription_id=model.project.subscription_id,
-            resource_group=model.project.resource_group,
-        )
+        project_meta = model.project.as_dict()
+        az_workspace = self.backend.get_workspace(project_meta)
 
         az_experiment = Experiment(workspace=az_workspace, name=model.experiment)
 
         datasets = DownloadedAzureMLDataStore.from_model(
             model=model,
             datasets=model.datasets_parsed.local,
             workspace=az_workspace,
             force_download=self.force_download,
         )
 
         with model.temporary_folder() as temp_path:
             # The "outputs" parameter is provided here with a non-existing
             # folder path to avoid having azureml upload files. We will do
             # this manually somewhere else.
+
             try:
                 self.az_run = az_experiment.start_logging(
                     snapshot_directory=temp_path,
                     outputs=os.path.join(temp_path, "a-folder-that-does-not-exists"),
                 )
             except azureml._common.exceptions.AzureMLException as ex:
                 raise self.backend.parse_azureml_exception(ex)
@@ -81,91 +137,49 @@
                 )
             finally:
                 try:
                     self.az_run.complete()
                 except azureml._common.exceptions.AzureMLException as ex:
                     raise self.backend.parse_azureml_exception(ex)
 
-    def save_output_files(self, model: Model):
-        """[summary]
-
-        Args:
-            model (Model): [description]
-
-        Raises:
-            AbstractBackend.BackendException: [description]
-        """
-        try:
-            self.az_run.upload_file("outputs/model.pkl", model.trained_model_path)
-        except azureml._common.exceptions.AzureMLException as ex:
-            raise self.backend.parse_azureml_exception(ex)
-
-    def save_log_file(self, clog: ConsoleLogger) -> None:
-        """This function takes the log file generated from clog and
-        pushes the log into the azure ml expiremnt tab called output.
-
-        Args:
-            clog (ConsoleLogger): This argument is an object of our logger function
-
-        Raises:
-            AbstractBackend.BackendException: [description]
-        """
-        try:
-            clog.flush()
-            self.az_run.upload_file(clog.filename, clog.filepath)
-        except azureml._common.exceptions.AzureMLException as ex:
-            raise self.backend.parse_azureml_exception(ex)
-
-    def get_portal_url(self) -> str:
-        """[summary]
-
-        Raises:
-            AbstractBackend.BackendException: [description]
-
-        Returns:
-            str: [description]
-        """
-        try:
-            return self.az_run.get_portal_url()
-        except azureml._common.exceptions.AzureMLException as ex:
-            raise self.backend.parse_azureml_exception(ex)
-
-    def get_parameters(self, model: Model) -> Dict:
+    def get_parameters(self, model: "Model") -> Dict:
         """[summary]
 
         Args:
             model (Model): [description]
 
         Returns:
             Dict: [description]
         """
         params = {}
         params.update(model.parameters)
         params.update(model.parameters_local)
         return params
 
-    def get_tags(self, model: Model) -> Dict:
+    def get_tags(self, model: "Model") -> Dict:
         """[summary]
 
         Args:
             model (Model): [description]
 
         Returns:
             Dict: [description]
         """
         return {"datasets": ", ".join(model.datasets + model.datasets_local)}
 
 
-class AzureCloudTrainingContext(AbstractTrainingContext):
+class AzureCloudTrainingContext(AzureTrainingContext):
     """[summary]"""
 
     def __init__(self):
         self.az_run = None
 
-    def train_model(self, model: Model, tags: Dict[str, Any], **kwargs) -> TrainedModel:
+    def train_model(
+        self, model: "Model", tags: Dict[str, Any], **kwargs
+    ) -> "TrainedModel":
         """[summary]
 
         Args:
             model (Model): [description]
             tags (Dict[str, Any]): [description]
 
         Returns:
@@ -183,55 +197,31 @@
         try:
             return model.train(
                 datasets=datasets, logger=AzureMlLogger(self.az_run), **kwargs
             )
         finally:
             self.az_run.complete()
 
-    def get_portal_url(self) -> str:
-        """[summary]
-
-        Returns:
-            str: [description]
-        """
-        return self.az_run.get_portal_url()
-
-    def get_parameters(self, model: Model) -> Dict:
+    def get_parameters(self, model: "Model") -> Dict:
         """[summary]
 
         Args:
             model (Model): [description]
 
         Returns:
             Dict: [description]
         """
         params = {}
         params.update(model.parameters)
         params.update(model.parameters_cloud)
         return params
 
-    def get_tags(self, model: Model) -> Dict:
+    def get_tags(self, model: "Model") -> Dict:
         """[summary]
 
         Args:
             model (Model): [description]
 
         Returns:
             Dict: [description]
         """
         return {"datasets": ", ".join(model.datasets + model.datasets_cloud)}
-
-    def save_log_file(self, clog: ConsoleLogger) -> None:
-        """This function takes the log file generated from clog and
-        pushes the log into the azure ml expiremnt tab called output.
-
-        Args:
-            clog (ConsoleLogger): This argument is an object of our logger function.
-
-        Raises:
-            AbstractBackend.BackendException: [description]
-        """
-        try:
-            clog.flush()
-            self.az_run.upload_file(clog.filename, clog.filepath)
-        except azureml._common.exceptions.AzureMLException as ex:
-            raise self.backend.parse_azureml_exception(ex)
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/cli/__init__.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 # TODO How else to get azureml Datasets working?
 # TODO Move to somewhere else?
 runtime.version = ("18", "10", "0")
 
 from energinetml.settings import PACKAGE_VERSION  # noqa: E402
 
 from .cluster import cluster_group  # noqa: E402
-from .infrastructure import infrastructure_group  # noqa: E402
 from .model import model_group  # noqa: E402
 from .project import project_group  # noqa: E402
-from .webapp import webapp_group  # noqa: E402
 
 
 @click.command()
 def version():
     """
     Prints SDK version.
     """
@@ -35,10 +33,8 @@
     """
     pass
 
 
 main.add_command(project_group, "project")
 main.add_command(model_group, "model")
 main.add_command(cluster_group, "cluster")
-main.add_command(webapp_group, "webapp")
-main.add_command(infrastructure_group, "infrastructure")
 main.add_command(version)
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/cli/cluster/change.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/verify.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """[summary]
 """
+
 import click
 
-from energinetml.backend import default_backend as backend
-from energinetml.cli.utils import discover_model
+from energinetml.core.backend import AbstractBackend
 from energinetml.core.model import Model
 from energinetml.settings import PACKAGE_NAME
 
 
-@click.command()
-@discover_model()
-@click.option(
-    "--cluster-name",
-    "cluster_name",
-    required=False,
-    default=None,
-    type=str,
-    help="Name of compute cluster, if creating a new cluster",
-)
-def change(model: Model, cluster_name: str) -> None:
-    """Switch to use another (existing) compute cluster."""
-    workspace = backend.get_workspace(
-        subscription_id=model.project.subscription_id,
-        resource_group=model.project.resource_group,
-        name=model.project.workspace_name,
-    )
+def verify_compute_cluster(
+    backend: "AbstractBackend",
+    model: "Model",
+    cluster_name: str,
+    modify_vm_size: bool = False,
+):
+    """Verifies that the compute cluster exists.
+    If not, the user is asked to choose another one.
+
+    Args:
+        backend (AbstractBackend): The backend to use.
+        model (Model): Model which contains information about the compute cluster.
+        cluster_name (str): The name of the compute cluster. This could be a new one.
+        modify_vm_size (bool, optional): Boolean indicating if this method should
+        change the vm_size. Defaults to False.
 
+    Raises:
+        click.Abort: If no compute clusters exist.
+    """
+    workspace = backend.get_workspace(model.project.as_dict())
     existing_clusters = backend.get_compute_clusters(workspace)
     existing_clusters_mapped = {c.name: c for c in existing_clusters}
     existing_cluster_names = [c.name for c in existing_clusters]
 
     if not existing_clusters:
         click.echo('No compute clusters exists in workspace "%s".' % workspace.name)
         click.echo('Run "%s cluster create" to create a new cluster.' % PACKAGE_NAME)
         raise click.Abort()
 
     while cluster_name not in existing_cluster_names:
+        click.echo(
+            (
+                f"Could not find compute target '{cluster_name}' in the "
+                f"available compute targets: {existing_cluster_names}."
+            )
+        )
+
         cluster_name = click.prompt(
-            text="Please enter name of compute cluster to use",
+            text="Please enter name of a compute cluster to use",
             type=click.Choice(existing_cluster_names),
-            default=model.compute_target,
         )
 
-    click.echo('Using cluster "%s" from now on.' % cluster_name)
+        click.echo(f"Using cluster '{cluster_name}' from now on.")
 
     cluster = existing_clusters_mapped[cluster_name]
+    model.compute_target = cluster_name
 
-    _update_model_properties(
-        model=model, cluster_name=cluster_name, vm_size=cluster.vm_size
-    )
-
-
-def _update_model_properties(model: Model, cluster_name: str, vm_size: str) -> None:
-    """[summary]
+    if modify_vm_size:
+        model.vm_size = cluster.vm_size
 
-    Args:
-        model (Model): [description]
-        cluster_name (str): [description]
-        vm_size (str): [description]
-    """
-    model.compute_target = cluster_name
-    model.vm_size = vm_size
     model.save()
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/cli/infrastructure/init.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/decorators.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,282 +1,239 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """[summary]
 """
+from __future__ import annotations
 
 import os
-import re
-import subprocess
-import sys
-import tempfile
-from typing import Dict
+from typing import TYPE_CHECKING
 
 import click
-from jinja2 import Template
 
-from energinetml.settings import (
-    DEFAULT_ENCODING,
-    TEMPLATES_GIT_URL,
-    TEMPLATES_IP_WHITELIST,
-    TEMPLATES_SUBNET_WHITELIST,
-)
-
-FILES_TO_COPY = (".gitignore",)
-FOLDERS_TO_COPY = (".azuredevops", "terraform")
-
-
-# -- Input parsing and validation --------------------------------------------
-
-
-def _parse_input_path(ctx: click.Context, param: click.Parameter, value: str) -> str:
-    """[summary]
-
-    Args:
-        ctx (click.Context): [description]
-        param (click.Parameter): [description]
-        value (str): [description]
+if TYPE_CHECKING:
+    from energinetml import Project
 
-    Raises:
-        click.Abort: [description]
+from energinetml.core.model import (
+    Model,
+    ModelImportError,
+    ModelNotClassError,
+    ModelNotInheritModel,
+    import_model_class,
+)
 
-    Returns:
-        str: [description]
-    """
-    if value is None:
-        value = os.path.abspath(
-            click.prompt(
-                text="Enter project location",
-                default=os.path.abspath("."),
-                type=click.Path(dir_okay=True, resolve_path=True),
-            )
-        )
 
-    # Path points to a file?
-    if os.path.isfile(value):
-        click.echo("Failed to init project infrastructure.")
-        click.echo(
-            "The path you provided me with points to a file, and not a "
-            "folder. I need a folder to put the project files in. "
-            "Check your -p/--path parameter."
-        )
-        click.echo("You provided me with: %s" % value)
-        raise click.Abort()
-
-    return value
-
-
-def _parse_input_project_name(
-    ctx: click.Context, param: click.Parameter, value: str
-) -> str:
+def discover_project(project_cls: Project, required: bool = True) -> str:
     """[summary]
 
     Args:
-        ctx (click.Context): [description]
-        param (click.Parameter): [description]
-        value (str): [description]
+        project_cls (Project): [description]
+        required (bool, optional): [description]. Defaults to True.
 
     Returns:
         str: [description]
     """
-    while not value or not re.findall(r"^[a-z][a-z0-9]{,10}$", value):
-        if value is not None:
-            click.echo("Invalid name provided")
-
-        click.echo(
-            "Provisioning cloud resources requires a name for your project "
-            "which contains 11 (or less) characters. This name is used as part "
-            "of the resource names, can only contain lower case letters "
-            "and numbers, and must start with a letter."
-        )
-
-        value = click.prompt(text="Please enter a project name", type=click.STRING)
 
-    return value
+    def _project_from_path_callback(
+        ctx: click.Context, param: click.Parameter, value: str
+    ) -> str:
+        """[summary]
+
+        Args:
+            ctx (click.Context): [description]
+            param (click.Parameter): [description]
+            value (str): [description]
+
+        Raises:
+            click.Abort: [description]
+
+        Returns:
+            str: [description]
+        """
+        try:
+            return project_cls.from_directory(value)
+        except project_cls.ConfigNotFound:
+            if required:
+                click.echo(
+                    (
+                        "Could not find a project in this folder "
+                        f"(or any of its parents): {value}"
+                    )
+                )
+
+                click.echo(
+                    (
+                        "I am looking for a folder which contains a file "
+                        f"named '{project_cls._CONFIG_FILE_NAME}' - either in the "
+                        "folder itself or in one of its parent folders."
+                    )
+                )
+
+                click.echo(
+                    "Specify which project to use by providing the "
+                    "-p/--path parameter."
+                )
+
+                raise click.Abort()
+
+    return click.option(
+        "--path",
+        "-p",
+        "project",
+        default=".",
+        type=click.Path(dir_okay=True, resolve_path=True),
+        help="Project directory path (default: current directory)",
+        callback=_project_from_path_callback,
+    )
 
 
-def _parse_input_resource_group(
-    ctx: click.Context, param: click.Parameter, value: str
-) -> str:
+def discover_model(
+    required: bool = True, load_model: bool = True, param_name: str = "model"
+) -> None:
     """[summary]
 
     Args:
-        ctx (click.Context): [description]
-        param (click.Parameter): [description]
-        value (str): [description]
+        required (bool, optional): [description]. Defaults to True.
+        load_model (bool, optional): [description]. Defaults to True.
+        param_name (str, optional): [description]. Defaults to "model".
+    """
+
+    def _model_from_path_callback(
+        ctx: click.Context, param: click.Parameter, model_file_path: str
+    ) -> Model:
+        """[summary]
+
+        Args:
+            ctx (click.Context): [description]
+            param (click.Parameter): [description]
+            value (str): [description]
+
+        Raises:
+            click.Abort: [description]
+
+        Returns:
+            Model: [description]
+        """
+        # Does model module exist?
+        if not os.path.isdir(model_file_path):
+            click.echo(("Could not find this folder: %s") % model_file_path)
 
-    Returns:
-        str: [description]
-    """
-    if value is None:
-        value = click.prompt(text="Enter resource group name", type=str)
+            click.echo(("I am looking for a folder which contains a python module."))
 
-    return value
+            click.echo(
+                ("Specify which model to use by providing the " "-p/--path parameter.")
+            )
 
+            raise click.Abort()
 
-def _parse_input_service_connection(
-    ctx: click.Context, param: click.Parameter, value: str
-) -> str:
-    """[summary]
+        parent_levels = Model.from_directory(model_file_path).parent_levels
 
-    Args:
-        ctx (click.Context): [description]
-        param (click.Parameter): [description]
-        value (str): [description]
+        try:
+            model_class = import_model_class(model_file_path, parent_levels)
+        except ModelImportError:
+            # Imported script does not have a "model" attribute
+            click.echo(
+                f"Failed to import your model class from module: {model_file_path}"
+            )
 
-    Returns:
-        str: [description]
-    """
-    if value is None:
-        value = click.prompt(
-            text="Enter Azure DevOps service connection name", type=str
-        )
+            click.echo(
+                'Make sure you refer your model class and name it "model". '
+                'Do this by defining a global variable named "model" in your '
+                "module, and point it to your model class."
+            )
 
-    return value
+            click.echo("")
+            click.echo("Example:")
+            click.echo("")
+            click.echo("    class MyModel(Model):")
+            click.echo("        ...")
+            click.echo("")
+            click.echo("    model = MyModel")
+            click.echo("")
+
+            raise click.Abort()
+        except ModelNotClassError:
+            # Imported "model" attribute is not a Class type
+            click.echo(
+                f"Failed to import your model class from module: {model_file_path}"
+            )
 
+            click.echo(
+                'When you define the "model" object in your model script, '
+                "make sure not to instantiate it."
+            )
 
-# -- CLI Command -------------------------------------------------------------
+            click.echo("")
+            click.echo("Example of doing it correct:")
+            click.echo("")
+            click.echo("    class MyModel(Model):")
+            click.echo("        ...")
+            click.echo("")
+            click.echo("    model = MyModel")
+
+            click.echo("")
+            click.echo("Example of doing it WRONG:")
+            click.echo("")
+            click.echo("    class MyModel(Model):")
+            click.echo("        ...")
+            click.echo("")
+            click.echo("    model = MyModel()  # Notice the instantiation")
+            click.echo("")
+
+            raise click.Abort()
+        except ModelNotInheritModel:
+            # Imported "model" attribute does not inherit from Model
+            click.echo(
+                f"Failed to import your model class from module: {model_file_path}"
+            )
 
+            click.echo("The model you are referring to does not inherit from Model.")
 
-@click.command()
-@click.option(
-    "--path",
-    "-p",
-    default=None,
-    type=click.Path(dir_okay=True, resolve_path=True),
-    callback=_parse_input_path,
-    help="Project path (default to current)",
-)
-@click.option(
-    "--name",
-    "-n",
-    "project_name",
-    default=None,
-    type=str,
-    callback=_parse_input_project_name,
-    help="Project name",
-)
-@click.option(
-    "--resource-group",
-    "-g",
-    "resource_group",
-    default=None,
-    type=str,
-    callback=_parse_input_resource_group,
-    help="Azure resource group",
-)
-@click.option(
-    "--service-connection",
-    "-s",
-    "service_connection",
-    default=None,
-    type=str,
-    callback=_parse_input_service_connection,
-    help="Azure DevOps service connection name",
-)
-def init_infrastructure(
-    path: str, project_name: str, resource_group: str, service_connection: str
-):
-    """Create infrastructure files for a new AnalyticsOps project."""
-
-    # -- Clone repo ----------------------------------------------------------
-
-    click.echo("-" * 79)
-    click.echo(
-        "NOTICE: We need to clone a Git repository containing the "
-        "necessary template files. This requires Git to be "
-        "installed on your system."
+            click.echo("")
+            click.echo("Example of doing it correct:")
+            click.echo("")
+            click.echo("    from energinetml import Model")
+            click.echo("")
+            click.echo("    class MyModel(Model):  # Notice the inheritance")
+            click.echo("        ...")
+            click.echo("")
+            click.echo("    model = MyModel")
+            click.echo("")
+
+            raise click.Abort()
+
+        try:
+            return model_class.from_directory(model_file_path)
+        except Model.ConfigNotFound:
+            if required:
+                click.echo(
+                    (
+                        "Could not find a configuration in this folder "
+                        f"(or any of its parents): {model_file_path}"
+                    )
+                )
+
+                click.echo(
+                    (
+                        "I am looking for a folder which contains a file "
+                        f"named {Model._CONFIG_FILE_NAME} - either in the "
+                        "folder itself or in one of its parent folders."
+                    )
+                )
+
+                click.echo(
+                    (
+                        "Specify which model to use by providing the "
+                        "-p/--path parameter."
+                    )
+                )
+
+                raise click.Abort()
+
+    return click.option(
+        "--path",
+        "-p",
+        "model",
+        default=".",
+        type=click.Path(dir_okay=True, resolve_path=True),
+        help="Model directory path (default: current directory)",
+        callback=_model_from_path_callback,
     )
-    click.echo("-" * 79)
-
-    # -- Clone repo ----------------------------------------------------------
-
-    with tempfile.TemporaryDirectory() as clone_path:
-        _clone_pipeline_files(clone_path=clone_path)
-
-        _parse_cloned_files(
-            clone_path=clone_path,
-            target_path=path,
-            project_name=project_name,
-            resource_group=resource_group,
-            service_connection=service_connection,
-        )
-
-
-def _clone_pipeline_files(clone_path: str) -> None:
-    """[summary]
-
-    Args:
-        clone_path (str): [description]
-
-    Raises:
-        click.Abort: [description]
-    """
-    click.echo(f'Cloning "{TEMPLATES_GIT_URL}" into "{clone_path}"')
-
-    try:
-        subprocess.check_call(
-            args=["git", "clone", TEMPLATES_GIT_URL, clone_path],
-            stdout=sys.stdout,
-            stderr=subprocess.STDOUT,
-        )
-    except subprocess.CalledProcessError:
-        raise click.Abort()
-
-
-def _parse_cloned_files(
-    clone_path: str,
-    target_path: str,
-    project_name: str,
-    resource_group: str,
-    service_connection: str,
-) -> None:
-    """[summary]
-
-    Args:
-        clone_path (str): [description]
-        target_path (str): [description]
-        project_name (str): [description]
-        resource_group (str): [description]
-        service_connection (str): [description]
-    """
-    env = {
-        "projectName": project_name,
-        "resourceGroup": resource_group,
-        "serviceConnection": service_connection,
-        "subnetWhitelist": TEMPLATES_SUBNET_WHITELIST,
-        "ipWhitelist": TEMPLATES_IP_WHITELIST,
-    }
-
-    files_to_copy = []
-    files_to_copy.extend(os.path.join(clone_path, f) for f in FILES_TO_COPY)
-
-    for folder in FOLDERS_TO_COPY:
-        for root, subdirs, files in os.walk(os.path.join(clone_path, folder)):
-            for file_name in files:
-                files_to_copy.append(os.path.join(root, file_name))
-
-    for file_abs_path in files_to_copy:
-        rel_path = os.path.relpath(file_abs_path, clone_path)
-        dst_path = os.path.join(target_path, rel_path)
-
-        _copy_file(src=file_abs_path, dst=dst_path, env=env)
-
-
-def _copy_file(src: str, dst: str, env: Dict[str, str]) -> None:
-    """[summary]
-
-    Args:
-        src (str): [description]
-        dst (str): [description]
-        env (Dict[str, str]): [description]
-    """
-    dst_folder = os.path.split(dst)[0]
-
-    with open(src, encoding=DEFAULT_ENCODING) as f:
-        template = Template(f.read())
-        rendered = template.render(**env)
-
-    if not os.path.isdir(dst_folder):
-        os.makedirs(dst_folder)
-
-    with open(dst, "w", encoding=DEFAULT_ENCODING) as f:
-        f.write(rendered)
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/__init__.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """Manage machine learning models.
 """
 import click
 
-from .build import build as build_model
 from .files import files as model_files
 from .init import init_model
-from .predict import predict as predict_model
 from .release import release as release_model
-from .serve import serve as serve_model
 from .submit import submit as submit_model
 from .train import train as train_model
 
 
 @click.group()
 def model_group():
     """Manage machine learning models."""
     pass
 
 
 model_group.add_command(init_model, "init")
 model_group.add_command(train_model)
-model_group.add_command(predict_model)
-model_group.add_command(build_model)
-model_group.add_command(serve_model)
 model_group.add_command(submit_model)
 model_group.add_command(release_model)
 model_group.add_command(model_files)
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/init.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     click.echo("-" * 79)
     click.echo("Initialized the model at: %s" % path)
     click.echo("")
     click.echo(
         (
             "Next step is to implement your model script! I have created an "
-            f"empty model template for you. It is called {Model.SCRIPT_FILE_NAME} "
+            f"empty model template for you. It is called {Model._SCRIPT_FILE_NAME} "
             "and is located in the model directory. Also, remember to add your model's "
             "dependencies to requirements.txt (located at the root "
             "of your project)."
         )
     )
     click.echo("")
     click.echo(
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/cli/model/train.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/model/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """[summary]
 """
+import os
 import sys
 from typing import List, Union
 
 import click
 import click_spinner
 
 from energinetml.backend import default_backend as backend
@@ -116,27 +117,40 @@
             raise click.Abort()
 
         # -- Dump output to disk -------------------------------------------------
 
         print(f"Dumping trained model to: {model.trained_model_path}")
 
         trained_model.params.update(params)
-        trained_model.dump(model.trained_model_path)
+        model.dump(model.trained_model_path, trained_model)
+
+        meta_data = {"module_name": model.module_name, "run_id": context.az_run.id}
+
+        if context.az_run:
+            workspace = context.az_run.experiment.workspace
+            meta_data["subscription_id"] = workspace.subscription_id
+            meta_data["resource_group"] = workspace.resource_group
+            meta_data["workspace_name"] = workspace.name
+            meta_data["run_id"] = context.az_run.id
+            meta_data["portal_url"] = context.get_portal_url()
+
+        context.save_meta_data(
+            meta_data, os.path.join(model.artifact_path, model._META_FILE_NAME)
+        )
 
         # -- Upload output files -------------------------------------------------
 
         print("Uploading output files...")
 
         with click_spinner.spinner():
-            context.save_output_files(model)
+            context.save_artifacts(model)
 
     except Exception:
         raise
     finally:
         if context.az_run:
             # -- Print portal link ---------------------------------------------------
             print(f"Portal link: {context.get_portal_url()}")
 
             print("Uploading log files...")
             with click_spinner.spinner():
-                context.save_log_file(stdout_console_logger)
-                context.save_log_file(stderr_console_logger)
+                context.save_logs(stdout_console_logger, stderr_console_logger)
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/cli/project/init.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/project/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,19 +89,20 @@
     workspace_name: str,
     location: str,
 ):
     """Create a new, empty machine learning project."""
     if not os.path.isdir(path):
         os.makedirs(path)
 
-    workspace = backend.get_workspace(
-        subscription_id=subscription_id,
-        resource_group=resource_group,
-        name=workspace_name,
-    )
+    project_meta = {
+        "subscription_id": subscription_id,
+        "resource_group": resource_group,
+        "workspace_name": workspace_name,
+    }
+    workspace = backend.get_workspace(project_meta)
 
     MachineLearningProject.create(
         path=path,
         name=name,
         subscription_id=subscription_id,
         resource_group=resource_group,
         workspace_name=workspace_name,
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/cli/utils/projects.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/cli/utils/projects.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,14 +139,19 @@
             str: [description]
         """
         if value is None:
             default = (
                 os.path.split(ctx.params["path"])[1] if ctx.params.get("path") else None
             )
 
+            # Make default lower-case letters only.
+            if default:
+                default = default.lower()
+                default = "".join(c for c in default if c.isalpha())
+
             value = click.prompt(
                 text="Please enter a project name", default=default, type=str
             )
 
         return value
 
     return _parse_input_project_name
@@ -277,20 +282,21 @@
                 text="Please enter AzureML Workspace name",
                 default=existing_workspaces[0] if existing_workspaces else None,
                 type=ArbitraryChoice(existing_workspaces)
                 if existing_workspaces
                 else str,  # noqa: E501
             )
 
+        project_meta = {
+            "subscription_id": ctx.params["subscription_id"],
+            "resource_group": ctx.params["resource_group"],
+            "workspace_name": value,
+        }
         try:
-            backend.get_workspace(
-                subscription_id=ctx.params["subscription_id"],
-                resource_group=ctx.params["resource_group"],
-                name=value,
-            )
+            backend.get_workspace(project_meta)
         except BackendException:
             click.echo(
                 'Workspace "{}" not found in resource group: {}'.format(
                     value, ctx.params["resource_group"]
                 )
             )
             raise click.Abort()
@@ -361,7 +367,38 @@
                 text="Please enter webserver kind",
                 default=None,
                 type=click.Choice(["ASGI", "WSGI"]),
             )
         return value
 
     return _parse_input_webapp_kind
+
+
+def parse_pipeline_repo_version() -> Callable:
+    """[summary]
+
+    Returns:
+        Callable: [description]
+    """
+
+    def _parse_pipeline_repo_version(
+        ctx: click.Context, param: click.Parameter, value: str
+    ) -> str:
+        """[summary]
+
+        Args:
+            ctx (click.Context): [description]
+            param (click.Parameter): [description]
+            value (str): [description]
+
+        Returns:
+            str: [description]
+        """
+        if value is None:
+            value = click.prompt(
+                text="Please enter a version of the pipeline repository",
+                default="v0.7.0",
+                type=str,
+            )
+        return value
+
+    return _parse_pipeline_repo_version
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/backend.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """[summary]
 """
 
 from enum import Enum
-from typing import Any, List
+from typing import TYPE_CHECKING, Any, Dict, List
 
-from energinetml.core.model import Model
 from energinetml.core.submitting import SubmitContext
 from energinetml.core.training import AbstractTrainingContext
 
+if TYPE_CHECKING:
+    from energinetml.core.model import Model
+
 
 class ComputeType(Enum):
     """[summary]"""
 
     CPU = "CPU"
     GPU = "GPU"
 
@@ -71,15 +73,15 @@
             resource_group (str): [description]
 
         Raises:
             NotImplementedError: [description]
         """
         raise NotImplementedError
 
-    def get_workspace(self, subscription_id: str, resource_group: str, name: str):
+    def get_workspace(self, project_meta: Dict[str, str]):
         """[summary]
 
         Args:
             subscription_id (str): [description]
             resource_group (str): [description]
             name (str): [description]
 
@@ -168,15 +170,15 @@
             NotImplementedError: [description]
 
         Returns:
             AbstractTrainingContext: [description]
         """
         raise NotImplementedError
 
-    def submit_model(self, model: Model, params: List[str]) -> SubmitContext:
+    def submit_model(self, model: "Model", params: List[str]) -> SubmitContext:
         """[summary]
 
         Args:
             model (Model): [description]
             params (List[str]): [description]
 
         Raises:
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/configurable.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/configurable.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,46 @@
 # -*- coding: utf-8 -*-
 """[summary]
 """
 
 import json
 import os
 from dataclasses import asdict, dataclass
-from typing import Union
+from typing import Dict, Union
 
 from energinetml.settings import DEFAULT_ENCODING
 
 
 @dataclass
 class Configurable:
     """[summary]"""
 
-    class NotFound(Exception):
+    class ConfigNotFound(Exception):
         """[summary]"""
 
         pass
 
+    class ConfigError(Exception):
+        """_summary_
+
+        Args:
+            Exception (_type_): _description_
+
+        Raises:
+            RuntimeError: _description_
+            cls.NotFound: _description_
+
+        Returns:
+            _type_: _description_
+        """
+
+        pass
+
     # Constants
-    CONFIG_FILE_NAME = None
+    _CONFIG_FILE_NAME = None
 
     # Members
     path: str
 
     @classmethod
     def create(cls, path: str, **kwargs) -> "Configurable":
         """[summary]
@@ -63,23 +79,23 @@
         Raises:
             RuntimeError: [description]
             cls.NotFound: [description]
 
         Returns:
             Configurable: [description]
         """
-        if cls.CONFIG_FILE_NAME is None:
-            raise RuntimeError("Attribute CONFIG_FILE_NAME is None")
+        if cls._CONFIG_FILE_NAME is None:
+            raise RuntimeError("Attribute _CONFIG_FILE_NAME is None")
 
-        file_pointer = locate_file_upwards(path, cls.CONFIG_FILE_NAME)
+        file_pointer = locate_file_upwards(path, cls._CONFIG_FILE_NAME)
 
         if file_pointer is not None:
             return cls.from_config_file(file_pointer)
         else:
-            raise cls.NotFound()
+            raise cls.ConfigNotFound()
 
     def get_file_path(self, *relative_path: str) -> str:
         """Returns absolute path to a file at relative_path,
         where relative_path is relative to config file.
 
         Args:
             *relative_path (str): [description]
@@ -102,45 +118,55 @@
         """
         return os.path.relpath(absolute_path, self.path)
 
     def save(self) -> None:
         """Saved config as JSON to filesystem."""
         if not os.path.isdir(self.path):
             os.makedirs(self.path)
-        with open(
-            self.get_file_path(self.CONFIG_FILE_NAME), "w", encoding=DEFAULT_ENCODING
-        ) as f:
+
+        config_file_path = self.get_file_path(self._CONFIG_FILE_NAME)
+        with open(config_file_path, "w", encoding=DEFAULT_ENCODING) as f:
             d = asdict(self)
             d.pop("path")
             json.dump(d, f, indent=4, sort_keys=True)
 
+    def as_dict(self) -> Dict[str, str]:
+        """Get the object variables as a dictionary.
+        Helpful in creation of a meta_data dictionary
+
+        returns:
+            Dict[str, str]:
+        """
+        return self.__dict__
+
 
 def locate_file_upwards(path: str, filename: str) -> Union[str, None]:
-    """[summary]
+    """locate a file and return its path. starts from the path-parameter and searches
+    upwards to the root.
 
-    Args:
-        path (str): [description]
-        filename (str): [description]
+    args:
+        path (str): the path where the search will start
+        filename (str): the filename of the file to search for
 
-    Returns:
-        str: [description]
+    returns:
+        str: the path of the file if found
     """
 
     def __is_root(_path: str) -> str:
         """[summary]
 
-        Args:
+        args:
             _path (str): [description]
 
-        Returns:
+        returns:
             str: [description]
         """
         # you have yourself root.
-        # works on Windows and *nix paths.
-        # does NOT work on Windows shares (\\server\share)
+        # works on windows and *nix paths.
+        # does not work on windows shares (\\server\share)
         return os.path.dirname(_path) == _path
 
     while 1:
         file_pointer = os.path.join(path, filename)
         if os.path.isfile(file_pointer):
             return file_pointer
         elif __is_root(path):
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/files.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """[summary]
 """
 import contextlib
 import glob
 import os
 import shutil
 import tempfile
-from typing import ContextManager, Iterable, List, Set, Tuple  # noqa TYP001
+from typing import ContextManager, Iterable, List, Set, Tuple
 
 
 class FileMatcher:
     """[summary]"""
 
     def __init__(
         self,
@@ -72,15 +72,15 @@
 
 
 @contextlib.contextmanager
 def temporary_folder(files: Iterable[Tuple[str, str]]) -> ContextManager[None]:
     """Returns a context manager which creates a temporary folder on the
     filesystem and copies files into the folder.
 
-    The ´files` parameter is an iterable of tuples of (src, dst), where
+    The `files` parameter is an iterable of tuples of (src, dst), where
     src is absolute path on the filesystem (a file to copy), and dst
     is the destination in the temporary folder relative to its root.
 
     Usage example:
 
         files_to_copy = [
             ('/home/folder/some-file.txt', 'some-file.txt'),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/logger.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 if TYPE_CHECKING:
     import pandas as pd
 
 from energinetml.settings import (
     DEFAULT_LOG_ENCODING,
     DEFAULT_LOG_FILENAME,
-    DEFAULT_RELATIVE_ARTIFACT_PATH,
+    DEFAULT_LOG_PATH,
 )
 
 
 class ConsoleLogger:
     """This class enables logging of stdout and stderr.
     The class is used during local trainings and finally uploaded to the azure ml
     expirment.
@@ -46,17 +46,17 @@
         file_prefix, ext = DEFAULT_LOG_FILENAME.split(".")
         self.filename = f"{file_prefix}_{name}.{ext}"
 
         self.filepath, self.log = self._init_log_file(self.filename)
 
     def _init_log_file(self, filename: str) -> Tuple[str, io.TextIOWrapper]:
         """Performs Initialization of the log file and further enrich the object."""
-        os.makedirs(DEFAULT_RELATIVE_ARTIFACT_PATH, exist_ok=True)
+        os.makedirs(DEFAULT_LOG_PATH, exist_ok=True)
 
-        filepath = f"{DEFAULT_RELATIVE_ARTIFACT_PATH}/{filename}"
+        filepath = f"{DEFAULT_LOG_PATH}/{filename}"
         return filepath, open(filepath, "w", encoding=DEFAULT_LOG_ENCODING)
 
     def isatty(self) -> bool:
         """A requried function for sys.stdout and sys.stderr.
 
         Returns:
             bool: This function will only return False.
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/project.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/project.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,39 +3,36 @@
 """[summary]
 """
 
 from __future__ import annotations
 
 import os
 from dataclasses import dataclass, field
-from enum import Enum
 from functools import cached_property
 from typing import Any, Dict
 
-from energinetml.core.templates import WebAppTemplateResolver
-from energinetml.core.webapp import WebAppEngine
 from energinetml.settings import (
     DEFAULT_ENCODING,
     DEFAULT_LOCATION,
     PACKAGE_NAME,
     PACKAGE_VERSION,
 )
 
 from .configurable import Configurable
 from .requirements import RequirementList
-from .templates import ASGIWebAppTemplates, WSGIWebAppTemplates
-from .webapp import AsgiWebApp, WsgiWebApp
 
 
 @dataclass
 class Project(Configurable):
     """[summary]"""
 
-    CONFIG_FILE_NAME = "project.json"
-    REQUIREMENTS_FILE_NAME = "requirements.txt"
+    _CONFIG_FILE_NAME = "project.json"
+    _REQUIREMENTS_FILE_NAME = "requirements.txt"
+
+    name: str
 
     @classmethod
     def create(cls, *args: Any, **kwargs: Dict[str, Any]) -> Project:
         """[summary]
 
         Returns:
             [type]: [description]
@@ -51,15 +48,15 @@
     @property
     def requirements_file_path(self) -> str:
         """Absolute path to requirements.txt file.
 
         Returns:
             str: [description]
         """
-        return self.get_file_path(self.REQUIREMENTS_FILE_NAME)
+        return self.get_file_path(self._REQUIREMENTS_FILE_NAME)
 
     @cached_property
     def requirements(self) -> RequirementList:
         """Returns a list of project requirements from requirements.txt.
 
         Returns:
             RequirementList: [description]
@@ -73,15 +70,14 @@
 # -- Machine Learning --------------------------------------------------------
 
 
 @dataclass
 class MachineLearningProject(Project):
     """[summary]"""
 
-    name: str
     subscription_id: str
     resource_group: str
     workspace_name: str
     vnet_name: str
     subnet_name: str
     location: str = field(default=DEFAULT_LOCATION)
 
@@ -102,70 +98,7 @@
         Args:
             model_name (str): [description]
 
         Returns:
             str: [description]
         """
         return self.get_file_path(model_name)
-
-
-# -- Web Apps ----------------------------------------------------------------
-
-
-class WebAppProjectKind(str, Enum):
-    """[summary]"""
-
-    ASGI = "ASGI"
-    WSGI = "WSGI"
-
-
-@dataclass
-class WebAppProject(Project):
-    """[summary]"""
-
-    name: str
-    kind: WebAppProjectKind
-
-    RESOLVERS = {
-        WebAppProjectKind.ASGI: ASGIWebAppTemplates(),
-        WebAppProjectKind.WSGI: WSGIWebAppTemplates(),
-    }
-
-    ENGINES = {
-        WebAppProjectKind.ASGI: AsgiWebApp(),
-        WebAppProjectKind.WSGI: WsgiWebApp(),
-    }
-
-    def get_template_resolver(self) -> WebAppTemplateResolver:
-        """[summary]
-
-        Raises:
-            RuntimeError: [description]
-
-        Returns:
-            WebAppTemplateResolver: [description]
-        """
-        if self.kind in self.RESOLVERS:
-            return self.RESOLVERS[self.kind]
-        raise RuntimeError
-
-    def get_engine(self) -> WebAppEngine:
-        """[summary]
-
-        Raises:
-            RuntimeError: [description]
-
-        Returns:
-            WebAppEngine: [description]
-        """
-        if self.kind in self.ENGINES:
-            return self.ENGINES[self.kind]
-        raise RuntimeError
-
-    @property
-    def dockerfile_path(self) -> str:
-        """[summary]
-
-        Returns:
-            str: [description]
-        """
-        return os.path.join(self.path, "Dockerfile")
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/requirements.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/requirements.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/submitting.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/submitting.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/templates.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 
     def resolve(
         self,
         project_root_path: str,
         project_name: str,
         service_connection: str,
         resource_group: str,
+        pipeline_repo_version: str,
     ):
         """[summary]
 
         Args:
             project_root_path (str): [description]
             project_name (str): [description]
             service_connection (str): DevOps Service Connection for deploying to
@@ -154,14 +155,15 @@
             ),
         )
 
         env = {
             "serviceConnection": service_connection,
             "resourceGroup": resource_group,
             "projectName": project_name,
+            "pipelineRepoVersion": pipeline_repo_version,
         }
 
         self.clone_and_render(project_root_path=project_root_path, files=files, env=env)
 
 
 class WebAppTemplateResolver(TemplateResolver):
     """
@@ -211,14 +213,15 @@
 
     def resolve(
         self,
         project_root_path: str,
         project_name: str,
         service_connection: str,
         resource_group: str,
+        pipeline_repo_version: str,
     ):
         """[summary]
 
         Args:
             project_root_path (str): [description]
             project_name (str): [description]
             service_connection (str): DevOps Service Connection for deploying to
@@ -238,14 +241,15 @@
 
     def resolve(
         self,
         project_root_path: str,
         project_name: str,
         service_connection: str,
         resource_group: str,
+        pipeline_repo_version: str,
     ):
         """[summary]
 
         Args:
             project_root_path (str): [description]
             project_name (str): [description]
             service_connection (str): DevOps Service Connection for deploying to
@@ -255,14 +259,15 @@
         self.resolve_web_app(
             project_root_path=project_root_path,
             kind="ASGI",
             env={
                 "serviceConnection": service_connection,
                 "resourceGroup": resource_group,
                 "projectName": project_name,
+                "pipelineRepoVersion": pipeline_repo_version,
             },
         )
 
 
 class WSGIWebAppTemplates(WebAppTemplateResolver):
     """
     Templates specific for ASGI Web Apps.
@@ -270,14 +275,15 @@
 
     def resolve(
         self,
         project_root_path: str,
         project_name: str,
         service_connection: str,
         resource_group: str,
+        pipeline_repo_version: str,
     ):
         """[summary]
 
         Args:
             project_root_path (str): [description]
             project_name (str): [description]
             service_connection (str): DevOps Service Connection for deploying to
@@ -287,9 +293,10 @@
         self.resolve_web_app(
             project_root_path=project_root_path,
             kind="WSGI",
             env={
                 "serviceConnection": service_connection,
                 "resourceGroup": resource_group,
                 "projectName": project_name,
+                "pipelineRepoVersion": pipeline_repo_version,
             },
         )
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/core/training.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/core/training.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             tags (Dict[str, Any]): [description]
 
         Returns:
             TrainedModel: [description]
         """
         pass
 
-    def save_output_files(self, model: Model) -> None:
+    def save_artifacts(self, model: Model) -> None:
         """Saves output files from a training run if necessary.
 
         Args:
             model (Model): [description]
         """
         pass
 
@@ -60,24 +60,36 @@
             model (Model): [description]
 
         Returns:
             Dict[str, str]: [description]
         """
         return {}
 
-    def save_log_file(self, clog: ConsoleLogger) -> None:
+    def save_logs(self, clog: ConsoleLogger) -> None:
         """This function takes the log file generated from clog and
         pushes the log into the azure ml expiremnt tab called output.
 
         Args:
             clog (ConsoleLogger): This argument is an object of our logger function.
 
         """
         pass
 
+    def save_meta_data(self, meta_data: Dict[str, str], meta_file_path: str):
+        """Create a meta json-file with the content from a meta_data dictionary
+        and save it to the path specified.
+
+        Args:
+            meta_data (Dict[str, str])): A dictionary of meta_data to persist in the
+            json-file
+            meta_file_path (str): The local path where the json-file is persisted.
+
+        """
+        pass
+
 
 def requires_parameter(name, typ):
     """[summary]
 
     Args:
         name ([type]): [description]
         typ ([type]): [description]
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/settings.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,20 +28,18 @@
         os.path.join(__current_folder, "meta", filename), encoding=DEFAULT_ENCODING
     ) as handle:
         return handle.read().strip()
 
 
 # -- Local -------------------------------------------------------------------
 
-DEFAULT_RELATIVE_ARTIFACT_PATH = "./outputs"
+DEFAULT_RELATIVE_ARTIFACT_PATH = "outputs"
+DEFAULT_LOG_PATH = "logs"
 DEFAULT_LOG_FILENAME = "log.txt"
 DEFAULT_LOG_ENCODING = "utf-8"
-DEFAULT_RELATIVE_LOG_FILENAME = os.path.join(
-    DEFAULT_RELATIVE_ARTIFACT_PATH, DEFAULT_LOG_FILENAME
-)
 
 # -- Cloud --------------------------------------------------------------------
 
 DEFAULT_LOCATION = "westeurope"
 DEFAULT_VM_CPU = "Standard_D1_v2"
 DEFAULT_VM_GPU = "Standard_NV6"
 
@@ -59,11 +57,24 @@
 PACKAGE_REQUIREMENT = Requirement.parse(f"{PACKAGE_NAME}=={PACKAGE_VERSION}")
 
 
 # -- Misc --------------------------------------------------------------------
 
 APPINSIGHTS_INSTRUMENTATIONKEY = os.environ.get("APPINSIGHTS_INSTRUMENTATIONKEY")
 
+_not_set: str = "NOTUSED"
+# webappName-modelVersion
+APPINSIGHTS_SERVICE_NAME: str = os.environ.get("APPINSIGHTS_SERVICE_NAME", _not_set)
+# projectName
+APPINSIGHTS_SERVICE_NAMESPACE: str = os.environ.get(
+    "APPINSIGHTS_SERVICE_NAMESPACE", _not_set
+)
+# webappName-modelName-modelVersion
+APPINSIGHTS_SERVICE_INSTANCE_ID: str = os.environ.get(
+    "APPINSIGHTS_SERVICE_INSTANCE_ID", _not_set
+)
+
+
 # Git repository containing template files
 TEMPLATES_GIT_URL = "https://github.com/AnalyticsOps/templates.git"
 TEMPLATES_SUBNET_WHITELIST = "/subscriptions/d252b8da-1db8-44f7-bd6e-8010cc01382b/resourceGroups/rg-AnalyticsOpsAgents-U/providers/Microsoft.Network/virtualNetworks/vnet-devops-agent-001/subnets/agent-subnet"  # noqa: E501
 TEMPLATES_IP_WHITELIST = "194.239.2.0/24"
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/energinetml/static/model_template/model.py` & `energinet-ml-sdk-1.0.0.dev24/energinetml/static/model_template/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """This is the NewModel class which defines the training logic and
 inference logic.
 """
 
 import typing
 
-from energinetml import MetricsLogger, Model, PredictionInput, TrainedModel, main
+from energinetml import MetricsLogger, Model, TrainedModel
 from energinetml.azure.datasets import MLDataStore
 
 
 class NewModel(Model):
     """EML SDK model class. This class captures training logic and inference logic."""
 
     def train(
@@ -25,46 +25,35 @@
 
         Args:
             datasets (MLDataStore): A reference to the data set.
             logger (MetricsLogger): The logger argument handle metric logging, etc.
             seed (typing.Any): The seed argument tries to obtain a deterministic
             environment for model experiments.
 
-        Raises:
-            NotImplementedError: You need to implement the training logic.
-
         Returns:
             TrainedModel: A serializable object of the train model.
         """
 
         # TODO Train your model here and return it
 
         raise NotImplementedError
 
         return TrainedModel()
 
     def predict(
-        self, trained_model: TrainedModel, input_data: PredictionInput, identifier: str
+        self, trained_model: TrainedModel, df, identifier: str
     ) -> typing.List[typing.Any]:
         """Define your prediction logic.
 
         Args:
             trained_model (TrainedModel): Your trained model object.
             input_data (PredictionInput): Data used for inference.
             identifier (str): A unique identifier which refers to a specific model in
             the model obejct.
 
-        Raises:
-            NotImplementedError: You need to implement the prediction logic.
-
         Returns:
             typing.List[typing.Any]: The output(s) of the model.
         """
 
         # TODO Predict using the trained model and return the prediction
 
         raise NotImplementedError
-
-
-# Allow to invoke the CLI by executing this file (do not remove these lines)
-if __name__ == "__main__":
-    main()
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/setup.py` & `energinet-ml-sdk-1.0.0.dev24/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,32 +97,23 @@
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     # TODO SPECIFIC VERSION OF REQUIREMENTS!
     install_requires=[
         "requests",
-        "Jinja2==3.0.1",
         "pandas>=1.2.0",
         "packaging==20.9",
-        "pyjwt==1.7.1",
         "click==8.0.3",
         "click-spinner==0.1.10",
-        "fastapi==0.63.0",
-        "uvicorn==0.15.0",
-        "pydantic==1.8.1",
         "requirements-parser==0.2.0",
-        "azure-cli-core==2.20.0",
-        "azure-identity==1.7.0",
-        "azureml-core==1.36.0",
-        "azureml-dataset-runtime==1.36.0",
-        "azure-monitor-opentelemetry-exporter==1.0.0b4",
-        "pyopenssl<21.0.0",
-        "waitress",
-        "flask",
+        "azure-cli-core~=2.34.1",
+        "azure-identity~=1.7.0",
+        "azureml-core~=1.39.0",
+        "azureml-dataset-runtime~=1.39.0",
     ],
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={"dev": [], "build": [], "test": []},
     cmdclass={"sdist": sdist_hg},
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/conftest.py` & `energinet-ml-sdk-1.0.0.dev24/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,105 @@
 import tempfile
+from random import random
+from unittest.mock import Mock
 
 import pytest
 
-from energinetml.core.model import Model
+from energinetml.core.model import Model, TrainedModel, import_model_class
 from energinetml.core.project import MachineLearningProject
-
-# Project
-PROJECT_NAME = "NAME"
-SUBSCRIPTION_ID = "SUBSCRIPTION-ID"
-RESOURCE_GROUP = "RESOURCE-GROUP"
-WORKSPACE_NAME = "WORKSPACE-NAME"
-VNET = "VNET"
-SUBNET = "SUBNET"
-
-
-# Model
-MODEL_NAME = "NAME"
-EXPERIMENT = "EXPERIMENT"
-COMPUTE_TARGET = "COMPUTE-TARGET"
-VM_SIZE = "VM-SIZE"
-DATASETS = ["iris", "hades:2"]
-FEATURES = ["feature1", "feature2"]
-PARAMETERS = {"param1": "value1", "param2": "value2"}
+from tests.constants import (
+    COMPUTE_TARGET,
+    DATASETS,
+    DATASETS_CLOUD,
+    DATASETS_LOCAL,
+    EXPERIMENT,
+    FEATURES,
+    FILES_INCLUDE,
+    MODEL_NAME,
+    PARAMETERS,
+    PROJECT_NAME,
+    RESOURCE_GROUP,
+    SUBNET,
+    SUBSCRIPTION_ID,
+    VM_SIZE,
+    VNET,
+    WORKSPACE_NAME,
+)
+
+
+def create_model(path: str, files_include=FILES_INCLUDE):
+    return Model.create(
+        path=f"{path}/user_model_{int(random()*100000)}",
+        name=MODEL_NAME,
+        experiment=EXPERIMENT,
+        compute_target=COMPUTE_TARGET,
+        vm_size=VM_SIZE,
+        datasets=DATASETS,
+        datasets_local=DATASETS_LOCAL,
+        datasets_cloud=DATASETS_CLOUD,
+        features=FEATURES,
+        parameters=PARAMETERS,
+        files_include=files_include,
+    )
+
+
+def create_project(path: str):
+    return MachineLearningProject.create(
+        path=path + "/user_model_test",
+        name=PROJECT_NAME,
+        subscription_id=SUBSCRIPTION_ID,
+        resource_group=RESOURCE_GROUP,
+        workspace_name=WORKSPACE_NAME,
+        vnet_name=VNET,
+        subnet_name=SUBNET,
+    )
 
 
 @pytest.fixture
 def model_path():
     with tempfile.TemporaryDirectory() as path:
-        project = MachineLearningProject.create(
-            path=path,
-            name=PROJECT_NAME,
-            subscription_id=SUBSCRIPTION_ID,
-            resource_group=RESOURCE_GROUP,
-            workspace_name=WORKSPACE_NAME,
-            vnet_name=VNET,
-            subnet_name=SUBNET,
-        )
+        project = create_project(path)
 
-        model = Model.create(
-            path=project.default_model_path(MODEL_NAME),
-            name=MODEL_NAME,
-            experiment=EXPERIMENT,
-            compute_target=COMPUTE_TARGET,
-            vm_size=VM_SIZE,
-            datasets=DATASETS,
-            features=FEATURES,
-            parameters=PARAMETERS,
+        model = create_model(path=project.default_model_path(MODEL_NAME))
+
+        trained_model = TrainedModel(
+            model="123", params={"asd": 123}, features=FEATURES
         )
+        Model.dump(model.trained_model_path, trained_model)
 
         yield model.path
 
 
 @pytest.fixture
+def user_model():
+    with tempfile.TemporaryDirectory() as path:
+        model = create_model(path)
+        model_class = import_model_class(model.path, model.parent_levels)
+        yield model_class.from_directory(model.path)
+
+
+@pytest.fixture
 def model():
     with tempfile.TemporaryDirectory() as path:
-        project = MachineLearningProject.create(
-            path=path,
-            name=PROJECT_NAME,
-            subscription_id=SUBSCRIPTION_ID,
-            resource_group=RESOURCE_GROUP,
-            workspace_name=WORKSPACE_NAME,
-            vnet_name=VNET,
-            subnet_name=SUBNET,
-        )
+        yield create_model(path)
 
-        yield Model.create(
-            path=project.default_model_path(MODEL_NAME),
-            name=MODEL_NAME,
-            experiment=EXPERIMENT,
-            compute_target=COMPUTE_TARGET,
-            vm_size=VM_SIZE,
-            datasets=DATASETS,
-            features=FEATURES,
-            parameters=PARAMETERS,
-        )
+
+@pytest.fixture
+def model_with_project():
+    with tempfile.TemporaryDirectory() as path:
+        project = create_project(path)
+        yield create_model(project.default_model_path(MODEL_NAME))
+
+
+@pytest.fixture
+def clusters_mock():
+    cluster1 = Mock()
+    cluster1.name = COMPUTE_TARGET
+    cluster1.vm_size = VM_SIZE
+    return [cluster1]
 
 
 # -- Smoketest command-line options ------------------------------------------
 
 
 def pytest_addoption(parser):
     """
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/smoketest/ml_deployment/deployment_smoke_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/smoketest/ml_deployment/deployment_smoke_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/smoketest/webapp_deployment/deployment_smoke_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/smoketest/webapp_deployment/deployment_smoke_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/azure_/backend_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/backend_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from dataclasses import dataclass
 from unittest.mock import ANY, Mock, patch
 
 import pytest
 from azureml._common.exceptions import AzureMLException
 
 from energinetml.azure.backend import AzureBackend
+from energinetml.core.project import Project
 
 
 @pytest.fixture
 def azure_backend():
-    yield AzureBackend()
+    azure_backend = AzureBackend()
+    azure_backend._credential = Mock(return_value=Mock())
+    yield azure_backend
 
 
 class TestAzureBackend:
 
     # -- get_available_subscriptions() Tests -------------------------------------
 
     @patch("energinetml.azure.backend.SubscriptionClient")
@@ -173,108 +176,61 @@
     ):
         """
         :param Mock workspace_mock:
         :param AzureBackend azure_backend:
         """
         workspace = Mock()
         workspace_mock.get.return_value = workspace
+        project_meta = {
+            "subscription_id": "subscription_id",
+            "resource_group": "resource_group",
+            "workspace_name": "name",
+        }
 
         # Act
-        return_value = azure_backend.get_workspace(
-            "subscription_id", "resource_group", "name"
-        )
+        return_value = azure_backend.get_workspace(project_meta)
 
         # Assert
         workspace_mock.get.assert_called_once_with(
             auth=ANY,
             subscription_id="subscription_id",
             resource_group="resource_group",
             name="name",
         )
 
         assert return_value is workspace
 
     @patch("energinetml.azure.backend.Workspace")
-    def test__get_workspace__raises_azure_ml_exception__should_raise_backend_exception(  # noqa: E501
+    def test__get_workspace__should_raise_config_error(
         self, workspace_mock, azure_backend
     ):
         """
         :param Mock workspace_mock:
         :param AzureBackend azure_backend:
         """
-        workspace_mock.get.side_effect = AzureMLException("x")
-
-        # Act + Assert
-        with pytest.raises(AzureBackend.BackendException):
-            azure_backend.get_workspace("subscription_id", "resource_group", "name")
-
-    # -- get_compute_clusters() Tests --------------------------------------------
-
-    @patch("energinetml.azure.backend.AmlCompute")
-    def test__get_compute_clusters__should_return_compute_clisters(
-        self, aml_compute_mock, azure_backend
-    ):
-        """
-        :param Mock aml_compute_mock:
-        :param AzureBackend azure_backend:
-        """
-        compute_clusters = ["compute1", "compute2"]
-        aml_compute_mock.list.return_value = compute_clusters
-
-        # Act
-        return_value = azure_backend.get_compute_clusters("workspace")
-
-        # Assert
-        aml_compute_mock.list.assert_called_once_with(workspace="workspace")
-
-        assert return_value is compute_clusters
-
-    @patch("energinetml.azure.backend.AmlCompute")
-    def test__get_compute_clusters__raises_azure_ml_exception__should_raise_backend_exception(  # noqa: E501
-        self, aml_compute_mock, azure_backend
-    ):
-        """
-        :param Mock aml_compute_mock:
-        :param AzureBackend azure_backend:
-        """
-        aml_compute_mock.list.side_effect = AzureMLException("x")
+        workspace = Mock()
+        workspace_mock.get.return_value = workspace
+        # Config missing key: 'subscription_id'
+        project_meta = {"resource_group": "resource_group", "workspace_name": "name"}
 
         # Act + Assert
-        with pytest.raises(AzureBackend.BackendException):
-            azure_backend.get_compute_clusters("workspace")
-
-    # -- get_compute_clusters() Tests --------------------------------------------
-
-    @patch("energinetml.azure.backend.AmlCompute")
-    def test__get_available_vm_sizes__should_return_vm_sizes(
-        self, aml_compute_mock, azure_backend
-    ):
-        """
-        :param Mock aml_compute_mock:
-        :param AzureBackend azure_backend:
-        """
-        vm_sizes = ["vm1", "vm2"]
-        aml_compute_mock.supported_vmsizes.return_value = vm_sizes
-
-        # Act
-        return_value = azure_backend.get_available_vm_sizes("workspace")
-
-        # Assert
-        aml_compute_mock.supported_vmsizes.assert_called_once_with(
-            workspace="workspace"
-        )
-
-        assert return_value is vm_sizes
+        with pytest.raises(Project.ConfigError):
+            azure_backend.get_workspace(project_meta)
 
-    @patch("energinetml.azure.backend.AmlCompute")
-    def test__get_available_vm_sizes__raises_azure_ml_exception__should_raise_backend_exception(  # noqa: E501
-        self, aml_compute_mock, azure_backend
+    @patch("energinetml.azure.backend.Workspace")
+    def test__get_workspace__raises_azure_ml_exception__should_raise_backend_exception(  # noqa: E501
+        self, workspace_mock, azure_backend
     ):
         """
-        :param Mock aml_compute_mock:
+        :param Mock workspace_mock:
         :param AzureBackend azure_backend:
         """
-        aml_compute_mock.supported_vmsizes.side_effect = AzureMLException("x")
+        workspace_mock.get.side_effect = AzureMLException("x")
 
+        project_meta = {
+            "subscription_id": "subscription_id",
+            "resource_group": "resource_group",
+            "workspace_name": "name",
+        }
         # Act + Assert
         with pytest.raises(AzureBackend.BackendException):
-            azure_backend.get_available_vm_sizes("workspace")
+            azure_backend.get_workspace(project_meta)
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/azure_/datasets_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/azure_/datasets_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/init_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/init_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/model/train_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/model/train_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
         """
         :param Mock backend_mock:
         :param str model_path:
         """
         runner = CliRunner()
 
         context = Mock()
-        context.train_model.return_value = "not a TrainedModel object"
+        trained_model = Mock()
+        context.train_model.return_value = trained_model
         context.get_tags.return_value = {}
         context.get_parameters.return_value = {}
         backend_mock.get_local_training_context.return_value = context
 
         # Act
         result = runner.invoke(cli=train, args=["--path", model_path])
 
@@ -75,17 +76,20 @@
         # Act
         result = runner.invoke(cli=train, args=["--path", model_path])
 
         # Assert
         assert result.exit_code == 1
         assert isinstance(result.exception, SystemExit)
 
+    @patch("energinetml.core.model.Model.dump")
     @patch("energinetml.cli.model.train.backend")
     @patch("energinetml.cli.model.train.TrainedModel", new=Mock)
-    def test__should_dump_trained_model_correctly(self, backend_mock, model_path):
+    def test__should_dump_trained_model_correctly(
+        self, backend_mock, model_dump_mock, model_path
+    ):
         """
         :param Mock backend_mock:
         :param str model_path:
         """
         runner = CliRunner()
 
         trained_model = Mock()
@@ -98,9 +102,10 @@
 
         # Act
         result = runner.invoke(cli=train, args=["--path", model_path])
 
         # Assert
         assert result.exit_code == 0
 
-        trained_model.dump.assert_called_once()
-        context.save_output_files.assert_called_once()
+        model_dump_mock.assert_called_once()
+        context.save_artifacts.assert_called_once()
+        context.save_meta_data.assert_called_once()
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/project/init_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/project/init_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/utils/decorators_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/decorators_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 
 
 def test__discover_project__project_does_not_exist__should_exit_with_error():
     with tempfile.TemporaryDirectory() as path:
 
         runner = CliRunner()
         project_cls_mock = Mock()
-        project_cls_mock.from_directory.side_effect = MachineLearningProject.NotFound
+        project_cls_mock.from_directory.side_effect = (
+            MachineLearningProject.ConfigNotFound
+        )
 
         @click.command()
         @discover_project(project_cls_mock)
         def discover_project_testable(project):
             pass
 
         # Act
@@ -97,60 +99,66 @@
         # Assert
         assert result.exit_code == 1
         isdir_mock.assert_called_once_with(os.path.normpath(path))
 
 
 @patch("energinetml.cli.utils.decorators.os.path.isdir")
 @patch("energinetml.cli.utils.decorators.import_model_class")
+@patch("energinetml.core.configurable.Configurable.from_directory")
 @pytest.mark.parametrize(
     "exception", (ModelImportError, ModelNotClassError, ModelNotInheritModel)
 )
 def test__discover_model__import_model_class_raises_exception__should_exit_with_error(
-    import_model_class_mock, isdir_mock, exception
+    from_directory_mock, import_model_class_mock, isdir_mock, exception
 ):
     """
     :param Mock import_model_class_mock:
     :param Mock isdir_mock:
     :param Exception exception:
     """
+    parent_levels = 1
     with tempfile.TemporaryDirectory() as path:
         isdir_mock.return_value = True
+        from_directory_mock.return_value = Mock(parent_levels=parent_levels)
         import_model_class_mock.side_effect = exception
 
         runner = CliRunner()
 
         # Act
         result = runner.invoke(discover_model_testable, ["--path", path])
 
         # Assert
         assert result.exit_code == 1
 
         isdir_mock.assert_called_once_with(os.path.normpath(path))
-        import_model_class_mock.assert_called_once_with(path)
+        import_model_class_mock.assert_called_once_with(path, parent_levels)
 
 
 @patch("energinetml.cli.utils.decorators.os.path.isdir")
 @patch("energinetml.cli.utils.decorators.import_model_class")
+@patch("energinetml.core.configurable.Configurable.from_directory")
 def test__discover_model__model_not_found_in_directory__should_exit_with_error(
-    import_model_class_mock, isdir_mock
+    from_directory_mock, import_model_class_mock, isdir_mock
 ):
     """
     :param Mock import_model_class_mock:
     :param Mock isdir_mock:
     """
+    parent_levels = 1
     with tempfile.TemporaryDirectory() as path:
+        from_directory_mock.return_value = Mock(parent_levels=parent_levels)
         model_class = Mock()
-        model_class.from_directory.side_effect = Model.NotFound
+        model_class.from_directory.side_effect = Model.ConfigNotFound
         isdir_mock.return_value = True
         import_model_class_mock.return_value = model_class
 
         runner = CliRunner()
 
         # Act
         result = runner.invoke(discover_model_testable, ["--path", path])
 
         # Assert
         assert result.exit_code == 1
 
         isdir_mock.assert_called_once_with(os.path.normpath(path))
 
-        import_model_class_mock.assert_called_once_with(path)
+        import_model_class_mock.assert_called_once_with(path, parent_levels)
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/cli/utils/projects_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/cli/utils/projects_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     prompt_mock.return_value = NAME
 
     # Act
     value = parse_input_project_name()(ctx=Mock(params=params), param=None, value=None)
 
     # Assert
     prompt_mock.assert_called_once_with(
-        text="Please enter a project name", default="project-path", type=str
+        text="Please enter a project name", default="projectpath", type=str
     )
 
     assert value == NAME
 
 
 @patch("energinetml.cli.project.init.click.prompt")
 def test__parse_input_project_name__value_is_provided__should_return_value(
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/backend_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/backend_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -38,45 +38,21 @@
             backend.get_available_workspace_names("subscription_id", "resource_group")
 
     def test__get_workspace(self, backend):
         """
         :param AbstractBackend backend:
         """
         with pytest.raises(NotImplementedError):
-            backend.get_workspace("subscription_id", "resource_group", "name")
+            project_meta = {
+                "subscription_id": "subscription_id",
+                "resource_group": "resource_group",
+                "workspace_name": "name",
+            }
 
-    def test__get_compute_clusters(self, backend):
-        """
-        :param AbstractBackend backend:
-        """
-        with pytest.raises(NotImplementedError):
-            backend.get_compute_clusters("workspace")
-
-    def test__get_available_vm_sizes(self, backend):
-        """
-        :param AbstractBackend backend:
-        """
-        with pytest.raises(NotImplementedError):
-            backend.get_available_vm_sizes("workspace")
-
-    def test__create_compute_cluster(self, backend):
-        """
-        :param AbstractBackend backend:
-        """
-        with pytest.raises(NotImplementedError):
-            backend.create_compute_cluster(
-                "workspace",
-                "name",
-                "vm_size",
-                "min_nodes",
-                "max_nodes",
-                "vnet_resource_group_name",
-                "vnet_name",
-                "subnet_name",
-            )
+            backend.get_workspace(project_meta)
 
     def test__get_local_training_context(self, backend):
         """
         :param AbstractBackend backend:
         """
         with pytest.raises(NotImplementedError):
             backend.get_local_training_context("force_download")
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/configurable_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/configurable_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/files_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/files_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/logger_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/logger_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 from energinetml.core.logger import ConsoleLogger, MetricsLogger
 from energinetml.settings import DEFAULT_LOG_ENCODING
 
 
 @pytest.fixture()
 def clog(monkeypatch, tmp_path):
-    monkeypatch.setattr(
-        "energinetml.core.logger.DEFAULT_RELATIVE_ARTIFACT_PATH", tmp_path
-    )
+    monkeypatch.setattr("energinetml.core.logger.DEFAULT_LOG_PATH", tmp_path)
     yield ConsoleLogger(name="stdout", console=sys.stdout)
 
 
 LOG_TEXT = "This messages come from the unit test.\n"
 N_WRITES = 5
```

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/project_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/project_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/requirements_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/requirements_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-0.9.2.dev87/tests/unittests/core/submitting_test.py` & `energinet-ml-sdk-1.0.0.dev24/tests/unittests/core/submitting_test.py`

 * *Files identical despite different names*

