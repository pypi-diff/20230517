# Comparing `tmp/openxlab-test-0.0.1.tar.gz` & `tmp/openxlab-test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-test-0.0.1.tar", last modified: Wed May 17 09:01:22 2023, max compression
+gzip compressed data, was "openxlab-test-0.0.2.tar", last modified: Wed May 17 09:15:06 2023, max compression
```

## Comparing `openxlab-test-0.0.1.tar` & `openxlab-test-0.0.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.687466 openxlab-test-0.0.1/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4035 2023-05-17 09:01:22.687205 openxlab-test-0.0.1/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3632 2023-05-17 07:32:10.000000 openxlab-test-0.0.1/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.659558 openxlab-test-0.0.1/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-test-0.0.1/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3207 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.661171 openxlab-test-0.0.1/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-test-0.0.1/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/config/const.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-17 09:01:21.000000 openxlab-test-0.0.1/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.661485 openxlab-test-0.0.1/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1057 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.662168 openxlab-test-0.0.1/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      397 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.664959 openxlab-test-0.0.1/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     7757 2023-05-17 08:42:30.000000 openxlab-test-0.0.1/openxlab/model/clients/openapi_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      853 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/clients/oss_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1877 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/clients/upload_service_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.670383 openxlab-test-0.0.1/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      875 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1021 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      536 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1105 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      765 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.672491 openxlab-test-0.0.1/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1750 2023-05-17 08:59:13.000000 openxlab-test-0.0.1/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/common/meta_file_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.677054 openxlab-test-0.0.1/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1401 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4328 2023-05-17 07:39:55.000000 openxlab-test-0.0.1/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/query_repo_model.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1023 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1094 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/update_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3711 2023-05-17 07:28:34.000000 openxlab-test-0.0.1/openxlab/model/handler/upload_file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.677720 openxlab-test-0.0.1/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-test-0.0.1/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-test-0.0.1/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.680566 openxlab-test-0.0.1/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-test-0.0.1/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      201 2023-05-17 07:32:10.000000 openxlab-test-0.0.1/openxlab/utils/auth.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      151 2023-05-17 07:32:10.000000 openxlab-test-0.0.1/openxlab/utils/env_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-test-0.0.1/openxlab/utils/file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      688 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/utils/time_util.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.680963 openxlab-test-0.0.1/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      488 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.681658 openxlab-test-0.0.1/openxlab/xlab/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/xlab/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2381 2023-05-17 07:32:10.000000 openxlab-test-0.0.1/openxlab/xlab/clients/auth_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.682580 openxlab-test-0.0.1/openxlab/xlab/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/xlab/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      679 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/xlab/commands/config_command.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.683392 openxlab-test-0.0.1/openxlab/xlab/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/xlab/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      851 2023-05-17 07:32:10.000000 openxlab-test-0.0.1/openxlab/xlab/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.684664 openxlab-test-0.0.1/openxlab/xlab/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/xlab/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1802 2023-05-17 07:28:28.000000 openxlab-test-0.0.1/openxlab/xlab/handler/user_config.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3883 2023-05-17 08:34:00.000000 openxlab-test-0.0.1/openxlab/xlab/handler/user_token.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:01:22.686824 openxlab-test-0.0.1/openxlab_test.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4035 2023-05-17 09:01:22.000000 openxlab-test-0.0.1/openxlab_test.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2029 2023-05-17 09:01:22.000000 openxlab-test-0.0.1/openxlab_test.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-17 09:01:22.000000 openxlab-test-0.0.1/openxlab_test.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       52 2023-05-17 09:01:22.000000 openxlab-test-0.0.1/openxlab_test.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      117 2023-05-17 09:01:22.000000 openxlab-test-0.0.1/openxlab_test.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-05-17 09:01:22.000000 openxlab-test-0.0.1/openxlab_test.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1426 2023-05-16 09:43:42.000000 openxlab-test-0.0.1/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-17 09:01:22.687559 openxlab-test-0.0.1/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1182 2023-05-17 09:01:14.000000 openxlab-test-0.0.1/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.685066 openxlab-test-0.0.2/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     4035 2023-05-17 09:15:06.684646 openxlab-test-0.0.2/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3632 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.647626 openxlab-test-0.0.2/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-test-0.0.2/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3207 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.649856 openxlab-test-0.0.2/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-test-0.0.2/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/config/const.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-17 09:14:44.000000 openxlab-test-0.0.2/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.650470 openxlab-test-0.0.2/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1057 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.651522 openxlab-test-0.0.2/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      397 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.655874 openxlab-test-0.0.2/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     7757 2023-05-17 08:42:30.000000 openxlab-test-0.0.2/openxlab/model/clients/openapi_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      853 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/clients/oss_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1877 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/clients/upload_service_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.661913 openxlab-test-0.0.2/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      875 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1021 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      536 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1105 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      765 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.664738 openxlab-test-0.0.2/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1750 2023-05-17 08:59:13.000000 openxlab-test-0.0.2/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.671193 openxlab-test-0.0.2/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1401 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     4328 2023-05-17 07:39:55.000000 openxlab-test-0.0.2/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1023 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1094 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/update_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3711 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/upload_file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.671993 openxlab-test-0.0.2/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-test-0.0.2/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-test-0.0.2/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.675520 openxlab-test-0.0.2/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-test-0.0.2/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      201 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/openxlab/utils/auth.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      151 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/openxlab/utils/env_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-test-0.0.2/openxlab/utils/file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      688 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/utils/time_util.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.676058 openxlab-test-0.0.2/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      488 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.677009 openxlab-test-0.0.2/openxlab/xlab/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2381 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/openxlab/xlab/clients/auth_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.678042 openxlab-test-0.0.2/openxlab/xlab/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      679 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/commands/config_command.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.679399 openxlab-test-0.0.2/openxlab/xlab/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      851 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/openxlab/xlab/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.681641 openxlab-test-0.0.2/openxlab/xlab/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1802 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/handler/user_config.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3883 2023-05-17 08:34:00.000000 openxlab-test-0.0.2/openxlab/xlab/handler/user_token.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.684023 openxlab-test-0.0.2/openxlab_test.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     4035 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2029 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       53 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      117 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1426 2023-05-16 09:43:42.000000 openxlab-test-0.0.2/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-17 09:15:06.685166 openxlab-test-0.0.2/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1183 2023-05-17 09:14:44.000000 openxlab-test-0.0.2/setup.py
```

### Comparing `openxlab-test-0.0.1/PKG-INFO` & `openxlab-test-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-test-0.0.1/README.md` & `openxlab-test-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/cli.py` & `openxlab-test-0.0.2/openxlab/cli.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/demo_cmd/__init__.py` & `openxlab-test-0.0.2/openxlab/demo_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/clients/openapi_client.py` & `openxlab-test-0.0.2/openxlab/model/clients/openapi_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/clients/oss_client.py` & `openxlab-test-0.0.2/openxlab/model/clients/oss_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/clients/upload_service_client.py` & `openxlab-test-0.0.2/openxlab/model/clients/upload_service_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/commands/__init__.py` & `openxlab-test-0.0.2/openxlab/model/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/commands/create.py` & `openxlab-test-0.0.2/openxlab/model/commands/create.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/commands/download.py` & `openxlab-test-0.0.2/openxlab/model/commands/download.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/commands/init.py` & `openxlab-test-0.0.2/openxlab/model/commands/init.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/commands/list.py` & `openxlab-test-0.0.2/openxlab/model/commands/list.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/commands/remove.py` & `openxlab-test-0.0.2/openxlab/model/commands/remove.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/commands/upload.py` & `openxlab-test-0.0.2/openxlab/model/commands/upload.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/commands/visibility.py` & `openxlab-test-0.0.2/openxlab/model/commands/visibility.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/common/constants.py` & `openxlab-test-0.0.2/openxlab/model/common/constants.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/common/meta_file_util.py` & `openxlab-test-0.0.2/openxlab/model/common/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/common/response_dto.py` & `openxlab-test-0.0.2/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/handler/create_repository.py` & `openxlab-test-0.0.2/openxlab/model/handler/create_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/handler/download_file.py` & `openxlab-test-0.0.2/openxlab/model/handler/download_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/handler/query_repo_model.py` & `openxlab-test-0.0.2/openxlab/model/handler/query_repo_model.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/handler/remove_repo_or_file.py` & `openxlab-test-0.0.2/openxlab/model/handler/remove_repo_or_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/handler/update_repository.py` & `openxlab-test-0.0.2/openxlab/model/handler/update_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/model/handler/upload_file.py` & `openxlab-test-0.0.2/openxlab/model/handler/upload_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/types/command_type.py` & `openxlab-test-0.0.2/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/utils/file.py` & `openxlab-test-0.0.2/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/utils/time_util.py` & `openxlab-test-0.0.2/openxlab/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/xlab/clients/auth_client.py` & `openxlab-test-0.0.2/openxlab/xlab/clients/auth_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/xlab/commands/config_command.py` & `openxlab-test-0.0.2/openxlab/xlab/commands/config_command.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/xlab/common/response_dto.py` & `openxlab-test-0.0.2/openxlab/xlab/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/xlab/handler/user_config.py` & `openxlab-test-0.0.2/openxlab/xlab/handler/user_config.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab/xlab/handler/user_token.py` & `openxlab-test-0.0.2/openxlab/xlab/handler/user_token.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/openxlab_test.egg-info/PKG-INFO` & `openxlab-test-0.0.2/openxlab_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-test-0.0.1/openxlab_test.egg-info/SOURCES.txt` & `openxlab-test-0.0.2/openxlab_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/pyproject.toml` & `openxlab-test-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.1/setup.py` & `openxlab-test-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
     extras_require={
         'tests': utils.parse_requirements('requirements/tests.txt'),
         'build': utils.parse_requirements('requirements/build.txt'),
         'optional': utils.parse_requirements('requirements/optional.txt'),
     },
     entry_points={
         'console_scripts': [
-              'openxlabtest = openxlab.cli:main'
+              'openxlab-test = openxlab.cli:main'
           ]
     },
     ext_modules=[],
 )
```

