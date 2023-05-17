# Comparing `tmp/cloudinary-cli-1.7.0.tar.gz` & `tmp/cloudinary-cli-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudinary-cli-1.7.0.tar", last modified: Wed May 17 00:02:38 2023, max compression
+gzip compressed data, was "dist/cloudinary-cli-1.7.1.tar", last modified: Wed May 17 00:14:32 2023, max compression
```

## Comparing `cloudinary-cli-1.7.0.tar` & `cloudinary-cli-1.7.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1443 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1131 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_search_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/helper_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/test/test_modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2798 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_modules/test_cli_upload_dir.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4423 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_modules/test_cli_sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2516 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_modules/test_cli_make.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      812 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_samples.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1095 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_file_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5935 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1450 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_url.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4822 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9739 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/defaults.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1420 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/cli.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/json_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9846 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2931 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/config_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4061 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/file_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7563 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/api_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-17 00:02:35.000000 cloudinary-cli-1.7.0/cloudinary_cli/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2022 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/admin.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4488 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1397 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/provisioning.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2476 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/uploader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1608 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/overrides.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2174 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      532 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2100 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/migrate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/make.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14221 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3857 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/upload_dir.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      638 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/upload_widget
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/media_library_widget
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      386 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/product_gallery
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/video_player
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/ruby/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      250 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/ruby/upload
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/node/upload
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      230 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/upload
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      543 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/find_all_empty_folders
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/base
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/explicit
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/samples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/samples/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1631 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/cli_group.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9056 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9739 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1903 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1443 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1131 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_cli_search_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/helper_test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/test/test_modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2798 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_modules/test_cli_upload_dir.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4423 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_modules/test_cli_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2516 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_modules/test_cli_make.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      812 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_cli_samples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1095 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_file_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5935 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_cli_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1450 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_cli_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_cli_url.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4822 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/test_cli_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/test/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9739 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/defaults.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1420 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/cli.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/utils/json_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9846 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/utils/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2931 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/utils/config_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4061 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/utils/file_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7563 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/utils/api_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-17 00:14:30.000000 cloudinary-cli-1.7.1/cloudinary_cli/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2022 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/admin.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4488 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1397 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/provisioning.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2476 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/uploader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1608 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/overrides.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2174 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      532 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/core/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2100 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/modules/migrate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/modules/make.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14221 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/modules/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3857 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/modules/upload_dir.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/modules/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/html/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      638 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/html/upload_widget
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/html/media_library_widget
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      386 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/html/product_gallery
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/html/video_player
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/ruby/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      250 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/ruby/upload
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/node/upload
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/python/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      230 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/python/upload
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      543 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/python/find_all_empty_folders
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/python/base
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/templates/python/explicit
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli/samples/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/samples/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1631 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/cli_group.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/cloudinary_cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9056 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9739 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1920 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/cloudinary_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 00:14:32.000000 cloudinary-cli-1.7.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2023-05-17 00:14:27.000000 cloudinary-cli-1.7.1/requirements.txt
```

### Comparing `cloudinary-cli-1.7.0/setup.py` & `cloudinary-cli-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_cli_search_api.py` & `cloudinary-cli-1.7.1/test/test_cli_search_api.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/helper_test.py` & `cloudinary-cli-1.7.1/test/helper_test.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_modules/test_cli_upload_dir.py` & `cloudinary-cli-1.7.1/test/test_modules/test_cli_upload_dir.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_modules/test_cli_sync.py` & `cloudinary-cli-1.7.1/test/test_modules/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_modules/test_cli_make.py` & `cloudinary-cli-1.7.1/test/test_modules/test_cli_make.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_cli_samples.py` & `cloudinary-cli-1.7.1/test/test_cli_samples.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_cli.py` & `cloudinary-cli-1.7.1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_file_utils.py` & `cloudinary-cli-1.7.1/test/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_utils.py` & `cloudinary-cli-1.7.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_cli_utils.py` & `cloudinary-cli-1.7.1/test/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_cli_api.py` & `cloudinary-cli-1.7.1/test/test_cli_api.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_cli_url.py` & `cloudinary-cli-1.7.1/test/test_cli_url.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/test/test_cli_config.py` & `cloudinary-cli-1.7.1/test/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/PKG-INFO` & `cloudinary-cli-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudinary-cli
-Version: 1.7.0
+Version: 1.7.1
 Summary: A command line interface for Cloudinary with full API support
 Home-page: https://github.com/cloudinary/cloudinary-cli
 Author: Cloudinary, Brian Luk
 Author-email: info@cloudinary.com, lukitsbrian@gmail.com
 License: MIT
 Keywords: cloudinary cli pycloudinary image video digital asset management command line interface transformation friendly easy flexible
 Platform: UNKNOWN
```

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/defaults.py` & `cloudinary-cli-1.7.1/cloudinary_cli/defaults.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/cli.py` & `cloudinary-cli-1.7.1/cloudinary_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/utils/json_utils.py` & `cloudinary-cli-1.7.1/cloudinary_cli/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/utils/utils.py` & `cloudinary-cli-1.7.1/cloudinary_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/utils/config_utils.py` & `cloudinary-cli-1.7.1/cloudinary_cli/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/utils/file_utils.py` & `cloudinary-cli-1.7.1/cloudinary_cli/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/utils/api_utils.py` & `cloudinary-cli-1.7.1/cloudinary_cli/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/core/admin.py` & `cloudinary-cli-1.7.1/cloudinary_cli/core/admin.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/core/search.py` & `cloudinary-cli-1.7.1/cloudinary_cli/core/search.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/core/provisioning.py` & `cloudinary-cli-1.7.1/cloudinary_cli/core/provisioning.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/core/utils.py` & `cloudinary-cli-1.7.1/cloudinary_cli/core/utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/core/uploader.py` & `cloudinary-cli-1.7.1/cloudinary_cli/core/uploader.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/core/overrides.py` & `cloudinary-cli-1.7.1/cloudinary_cli/core/overrides.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/core/config.py` & `cloudinary-cli-1.7.1/cloudinary_cli/core/config.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/core/__init__.py` & `cloudinary-cli-1.7.1/cloudinary_cli/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/modules/migrate.py` & `cloudinary-cli-1.7.1/cloudinary_cli/modules/migrate.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/modules/make.py` & `cloudinary-cli-1.7.1/cloudinary_cli/modules/make.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/modules/sync.py` & `cloudinary-cli-1.7.1/cloudinary_cli/modules/sync.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/modules/upload_dir.py` & `cloudinary-cli-1.7.1/cloudinary_cli/modules/upload_dir.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/templates/html/upload_widget` & `cloudinary-cli-1.7.1/cloudinary_cli/templates/html/upload_widget`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/templates/html/media_library_widget` & `cloudinary-cli-1.7.1/cloudinary_cli/templates/html/media_library_widget`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/templates/html/video_player` & `cloudinary-cli-1.7.1/cloudinary_cli/templates/html/video_player`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/templates/python/find_all_empty_folders` & `cloudinary-cli-1.7.1/cloudinary_cli/templates/python/find_all_empty_folders`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/samples/__init__.py` & `cloudinary-cli-1.7.1/cloudinary_cli/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli/cli_group.py` & `cloudinary-cli-1.7.1/cloudinary_cli/cli_group.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/README.md` & `cloudinary-cli-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/LICENSE` & `cloudinary-cli-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli.egg-info/PKG-INFO` & `cloudinary-cli-1.7.1/cloudinary_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudinary-cli
-Version: 1.7.0
+Version: 1.7.1
 Summary: A command line interface for Cloudinary with full API support
 Home-page: https://github.com/cloudinary/cloudinary-cli
 Author: Cloudinary, Brian Luk
 Author-email: info@cloudinary.com, lukitsbrian@gmail.com
 License: MIT
 Keywords: cloudinary cli pycloudinary image video digital asset management command line interface transformation friendly easy flexible
 Platform: UNKNOWN
```

### Comparing `cloudinary-cli-1.7.0/cloudinary_cli.egg-info/SOURCES.txt` & `cloudinary-cli-1.7.1/cloudinary_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 cloudinary_cli/__init__.py
 cloudinary_cli/cli.py
 cloudinary_cli/cli_group.py
 cloudinary_cli/defaults.py
 cloudinary_cli/version.py
 cloudinary_cli.egg-info/PKG-INFO
```

