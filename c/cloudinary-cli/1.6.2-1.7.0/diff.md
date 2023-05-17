# Comparing `tmp/cloudinary-cli-1.6.2.tar.gz` & `tmp/cloudinary-cli-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudinary-cli-1.6.2.tar", last modified: Wed Apr  5 13:02:13 2023, max compression
+gzip compressed data, was "dist/cloudinary-cli-1.7.0.tar", last modified: Wed May 17 00:02:38 2023, max compression
```

## Comparing `cloudinary-cli-1.6.2.tar` & `cloudinary-cli-1.7.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1509 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_cli_search_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/helper_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/test/test_modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2798 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_modules/test_cli_upload_dir.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4423 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_modules/test_cli_sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2516 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_modules/test_cli_make.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_modules/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      812 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_cli_samples.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1095 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_file_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4749 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_cli_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1450 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_cli_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_cli_url.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4822 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/test_cli_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/test/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9739 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/defaults.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1420 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/cli.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/utils/json_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9066 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/utils/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2931 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/utils/config_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4061 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/utils/file_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7563 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/utils/api_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-05 13:02:10.000000 cloudinary-cli-1.6.2/cloudinary_cli/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2022 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/admin.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4236 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1397 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/provisioning.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2476 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/uploader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1608 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/overrides.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2174 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      532 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/core/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/modules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2100 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/modules/migrate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/modules/make.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14221 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/modules/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3856 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/modules/upload_dir.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/modules/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/html/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      638 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/html/upload_widget
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/html/media_library_widget
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      386 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/html/product_gallery
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/html/video_player
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/ruby/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      250 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/ruby/upload
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/node/upload
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/python/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      230 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/python/upload
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      543 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/python/find_all_empty_folders
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/python/base
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/templates/python/explicit
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli/samples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/samples/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1631 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/cli_group.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/cloudinary_cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9056 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-04-05 13:02:07.000000 cloudinary-cli-1.6.2/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9739 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1903 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/cloudinary_cli.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-05 13:02:13.000000 cloudinary-cli-1.6.2/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1443 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1131 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_search_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/helper_test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/test/test_modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2798 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_modules/test_cli_upload_dir.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4423 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_modules/test_cli_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2516 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_modules/test_cli_make.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_modules/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      812 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_samples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1095 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_file_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5935 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1450 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_url.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4822 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/test_cli_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/test/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9739 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/defaults.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1420 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/cli.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/json_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9846 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2931 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/config_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4061 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/file_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7563 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/api_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-17 00:02:35.000000 cloudinary-cli-1.7.0/cloudinary_cli/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2022 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/admin.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4488 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1397 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/provisioning.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2476 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/uploader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1608 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/overrides.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2174 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      532 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/core/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2100 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/migrate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/make.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14221 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3857 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/upload_dir.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/modules/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      638 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/upload_widget
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/media_library_widget
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      386 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/product_gallery
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/html/video_player
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/ruby/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      250 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/ruby/upload
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/node/upload
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      230 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/upload
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      543 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/find_all_empty_folders
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/base
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/templates/python/explicit
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli/samples/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/samples/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1631 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/cli_group.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/cloudinary_cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9056 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-05-17 00:02:32.000000 cloudinary-cli-1.7.0/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9739 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1903 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 00:02:37.000000 cloudinary-cli-1.7.0/cloudinary_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 00:02:38.000000 cloudinary-cli-1.7.0/setup.cfg
```

### Comparing `cloudinary-cli-1.6.2/setup.py` & `cloudinary-cli-1.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 with open("README.md", "r") as rmf:
     long_description = rmf.read()
 
 with open('cloudinary_cli/version.py') as vf:
     version = vf.readline().strip().split('"')[1]
 
+with open('requirements.txt') as rqf:
+    requirements = rqf.read().splitlines()
+
 setuptools.setup(
     name="cloudinary-cli",
     version=version,
     author="Cloudinary, Brian Luk",
     author_email="info@cloudinary.com, lukitsbrian@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
@@ -31,19 +34,11 @@
     packages=setuptools.find_packages(),
     keywords='cloudinary cli pycloudinary image video digital asset management command line interface transformation '
              'friendly easy flexible',
     license="MIT",
     python_requires='>=3.6.0',
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "mock", "urllib3"],
-    install_requires=[
-        "cloudinary>=1.28.1",
-        "pygments",
-        "jinja2",
-        "click",
-        "click-log",
-        "requests",
-        "docstring-parser"
-    ],
+    install_requires=requirements,
     include_package_data=True,
     zip_safe=False
 )
```

### Comparing `cloudinary-cli-1.6.2/test/helper_test.py` & `cloudinary-cli-1.7.0/test/helper_test.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_modules/test_cli_upload_dir.py` & `cloudinary-cli-1.7.0/test/test_modules/test_cli_upload_dir.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_modules/test_cli_sync.py` & `cloudinary-cli-1.7.0/test/test_modules/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_modules/test_cli_make.py` & `cloudinary-cli-1.7.0/test/test_modules/test_cli_make.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_cli_samples.py` & `cloudinary-cli-1.7.0/test/test_cli_samples.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_cli.py` & `cloudinary-cli-1.7.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_file_utils.py` & `cloudinary-cli-1.7.0/test/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_utils.py` & `cloudinary-cli-1.7.0/test/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import unittest
 
 from cloudinary_cli.utils.utils import parse_option_value, parse_args_kwargs, whitelist_keys, merge_responses, \
-    normalize_list_params, chunker
+    normalize_list_params, chunker, group_params
 
 
 class UtilsTest(unittest.TestCase):
     def test_parse_option_value(self):
         """ should parse option values correctly """
         self.assertEqual("haha,123,1234", parse_option_value("haha,123,1234"))
         self.assertTrue(parse_option_value("True"))
         self.assertFalse(parse_option_value("false"))
         self.assertListEqual(["test", "123"], parse_option_value('["test","123"]'))
         self.assertDictEqual({"foo": "bar"}, parse_option_value('{"foo":"bar"}'))
         self.assertDictEqual({"an": "object", "or": "dict"}, parse_option_value('{"an":"object","or":"dict"}'))
-        self.assertListEqual(["this", "will", "be", "read", "as",
-                              "a", "list"], parse_option_value('["this","will","be","read","as","a","list"]'))
+        self.assertListEqual(
+            ["this", "will", "be", "read", "as","a", "list"],
+            parse_option_value('["this","will","be","read","as","a","list"]')
+        )
+        self.assertListEqual(
+            [True, False, 123, '0', ['test', '123']],
+            parse_option_value(["True", "false", "123", "0", '["test","123"]'])
+        )
 
     def test_parse_option_value_converts_int_to_str(self):
         """ should convert a parsed 0 to a str """
         self.assertEqual("0", parse_option_value(0))
         self.assertEqual(1, parse_option_value(1))
 
     def test_parse_args_kwargs(self):
@@ -43,14 +49,33 @@
         self.assertDictEqual({"arg2": {"k2": "a2"}}, kwargs)
 
         # should allow passing optional args as positional
         args, kwargs = parse_args_kwargs(_args_kwargs_test_func, ["a1", "a2"])
         self.assertListEqual(["a1", "a2"], args)
         self.assertEqual(0, len(kwargs))
 
+        # should allow passing positional as optional
+        args, kwargs = parse_args_kwargs(_only_args_test_func, ["a1"], {"arg2": "a2"})
+        self.assertListEqual(["a1"], args)
+        self.assertDictEqual({"arg2": "a2"}, kwargs)
+
+        args, kwargs = parse_args_kwargs(_only_args_test_func, [], {"arg1": "a1", "arg2": "a2"})
+        self.assertEqual(0, len(args))
+        self.assertDictEqual({"arg1": "a1", "arg2": "a2"}, kwargs)
+
+    def test_group_params(self):
+        self.assertDictEqual({}, group_params([]))
+        self.assertDictEqual({"k1": "v1", "k2": "v2"}, group_params([("k1", "v1"), ("k2", "v2")]))
+        self.assertDictEqual({"k1": ["v1", "v2"]}, group_params([("k1", "v1"), ("k1", "v2")]))
+        self.assertDictEqual({"k1": "v1", "k2": ["v2", "v3"]}, group_params([("k1", "v1"), ("k2", "v2"), ("k2", "v3")]))
+        self.assertDictEqual(
+            {"k1": ["v1", "v2", "v3"]},
+            group_params([("k1", "v1")], [("k1", "v2")], [("k1", "v3")])
+        )
+
     def test_whitelist_keys(self):
         """ should whitelist keys correctly """
         self.assertEqual([{"k1": "v1"}], whitelist_keys([{"k1": "v1", "k2": "v2"}], ["k1"]))
         self.assertEqual([{"k1": "v1", "k2": "v2"}], whitelist_keys([{"k1": "v1", "k2": "v2"}], []))
         self.assertEqual([{"k1": "v1"}], whitelist_keys([{"k1": "v1", "k2": "v2"}], ["k1", "k3"]))
 
     def test_merge_responses(self):
```

### Comparing `cloudinary-cli-1.6.2/test/test_cli_utils.py` & `cloudinary-cli-1.7.0/test/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_cli_api.py` & `cloudinary-cli-1.7.0/test/test_cli_api.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_cli_url.py` & `cloudinary-cli-1.7.0/test/test_cli_url.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/test/test_cli_config.py` & `cloudinary-cli-1.7.0/test/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/PKG-INFO` & `cloudinary-cli-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudinary-cli
-Version: 1.6.2
+Version: 1.7.0
 Summary: A command line interface for Cloudinary with full API support
 Home-page: https://github.com/cloudinary/cloudinary-cli
 Author: Cloudinary, Brian Luk
 Author-email: info@cloudinary.com, lukitsbrian@gmail.com
 License: MIT
 Keywords: cloudinary cli pycloudinary image video digital asset management command line interface transformation friendly easy flexible
 Platform: UNKNOWN
```

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/defaults.py` & `cloudinary-cli-1.7.0/cloudinary_cli/defaults.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/cli.py` & `cloudinary-cli-1.7.0/cloudinary_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/utils/json_utils.py` & `cloudinary-cli-1.7.0/cloudinary_cli/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/utils/utils.py` & `cloudinary-cli-1.7.0/cloudinary_cli/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,42 +91,52 @@
         logger.error(f"Failed rendering template: '{template_name}' for language: '{language}'")
         raise
 
     return result
 
 
 def parse_option_value(value):
+    if isinstance(value, list):
+        return list(map(parse_option_value, value))
+
     if value == "True" or value == "true":
         return True
     elif value == "False" or value == "false":
         return False
     try:
         value = json.loads(value)
     except Exception:
         pass
     # serialize 0 to "0" string, otherwise it will be omitted (counted as False)
     if isinstance(value, int) and not value:
         value = str(value)
     return value
 
 
-def parse_args_kwargs(func, params):
+def parse_args_kwargs(func, params=None, kwargs=None):
+    if params is None:
+        params = []
+    if kwargs is None:
+        kwargs = {}
+
     spec = getfullargspec(func)
-    n_args = len(spec.args) if spec.args else 0
-    n_defaults = len(spec.defaults) if spec.defaults else 0
 
-    n_req = n_args - n_defaults
-    if len(params) < n_req:
+    num_args = len(spec.args) if spec.args else 0
+    num_defaults = len(spec.defaults) if spec.defaults else 0
+
+    num_req = num_args - num_defaults
+    num_provided_args = len(params)
+    num_overall_provided = num_provided_args + len([p for p in kwargs.keys() if p in spec.args[num_provided_args:]])
+    if num_overall_provided < num_req:
         func_sig = signature(func)
-        raise Exception(f"Function '{func.__name__}{func_sig}' requires {n_req} positional arguments")
+        raise Exception(f"Function '{func.__name__}{func_sig}' requires {num_req} positional arguments")
     # consume required args
-    args = [parse_option_value(p) for p in params[:n_req]]
-    kwargs = {}
+    args = [parse_option_value(p) for p in params[:num_req]]
 
-    for p in params[n_req:]:
+    for p in params[num_req:]:
         if '=' not in p:
             # named/positional with default value args passed as positional
             args.append(parse_option_value(p))
             continue
 
         k, v = p.split('=', 1)
         kwargs[k] = parse_option_value(v)
@@ -203,25 +213,39 @@
         raise Exception(f"Method {params[0]} does not exist in {module_name.capitalize()}.")
 
     func = module.__dict__.get(method)
 
     if not callable(func):
         raise Exception(f"{params[0]} is not callable.")
 
-    args, kwargs = parse_args_kwargs(func, params[1:])
+    kwargs = group_params(optional_parameter, ((k, parse_option_value(v)) for k, v in optional_parameter_parsed))
 
-    kwargs = {
-        **kwargs,
-        **{k: v for k, v in optional_parameter},
-        **{k: parse_option_value(v) for k, v in optional_parameter_parsed},
-    }
+    args, kwargs = parse_args_kwargs(func, params[1:], kwargs)
 
     return func, args, kwargs
 
 
+def group_params(*params):
+    """
+    Groups parameters (which are passed as list of tuples) by keys. Duplicate keys' values are combined into lists.
+
+    :param params: the list of parameters to group
+    :return: dict
+    """
+    res = {}
+    for param in params:
+        for k, v in param:
+            if k in res:
+                res[k] = (res[k] if isinstance(res[k], list) else [res[k]]) + [v]
+                continue
+            res[k] = v
+
+    return res
+
+
 def print_help_and_exit():
     """
     Prints help for the current command and exits.
     """
     ctx = click.get_current_context()
     click.echo(ctx.get_help())
     ctx.exit()
```

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/utils/config_utils.py` & `cloudinary-cli-1.7.0/cloudinary_cli/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/utils/file_utils.py` & `cloudinary-cli-1.7.0/cloudinary_cli/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/utils/api_utils.py` & `cloudinary-cli-1.7.0/cloudinary_cli/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/core/admin.py` & `cloudinary-cli-1.7.0/cloudinary_cli/core/admin.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/core/search.py` & `cloudinary-cli-1.7.0/cloudinary_cli/core/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,46 +23,54 @@
         help="Specify the attribute for which an aggregation count should be calculated and returned.")
 @option("-n", "--max_results", nargs=1, default=10,
         help="The maximum number of results to return. Default: 10, maximum: 500.")
 @option("-c", "--next_cursor", nargs=1, help="Continue a search using an existing cursor.")
 @option("-A", "--auto_paginate", is_flag=True, help="Return all results. Will call Admin API multiple times.")
 @option("-F", "--force", is_flag=True, help="Skip confirmation when running --auto-paginate.")
 @option("-ff", "--filter_fields", multiple=True, help="Filter fields to return.")
+@option("-t", "--ttl", nargs=1, default=300, help="Set the Search URL TTL in seconds. Default: 300.")
+@option("-u", "--url", is_flag=True, help="Build a signed search URL.")
 @option("--json", nargs=1, help="Save JSON output to a file. Usage: --json <filename>")
 @option("--csv", nargs=1, help="Save CSV output to a file. Usage: --csv <filename>")
 @option("-d", "--doc", is_flag=True, help="Open Search API documentation page.")
 def search(query, with_field, sort_by, aggregate, max_results, next_cursor,
-           auto_paginate, force, filter_fields, json, csv, doc):
+           auto_paginate, force, filter_fields, ttl, url, json, csv, doc):
     if doc:
         return launch("https://cloudinary.com/documentation/search_api")
 
     fields_to_keep = []
     if filter_fields:
         fields_to_keep = tuple(normalize_list_params(filter_fields)) + with_field
 
-    expression = cloudinary.search.Search().expression(" ".join(query))
+    search = cloudinary.search.Search().expression(" ".join(query))
 
     if auto_paginate:
         max_results = DEFAULT_MAX_RESULTS
     if with_field:
         for f in with_field:
-            expression.with_field(f)
+            search.with_field(f)
     if sort_by:
-        expression.sort_by(*sort_by)
+        search.sort_by(*sort_by)
     if aggregate:
-        expression.aggregate(aggregate)
+        search.aggregate(aggregate)
     if next_cursor:
-        expression.next_cursor(next_cursor)
+        search.next_cursor(next_cursor)
+    if ttl:
+        search.ttl(ttl)
 
-    expression.max_results(max_results)
+    search.max_results(max_results)
 
-    res = execute_single_request(expression, fields_to_keep)
+    if url:
+        print(search.to_url())
+        return True
+
+    res = execute_single_request(search, fields_to_keep)
 
     if auto_paginate:
-        res = handle_auto_pagination(res, expression, force, fields_to_keep)
+        res = handle_auto_pagination(res, search, force, fields_to_keep)
 
     print_json(res)
 
     if json:
         write_json_to_file(res['resources'], json)
         logger.info(f"Saved search JSON to '{json}' file")
```

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/core/provisioning.py` & `cloudinary-cli-1.7.0/cloudinary_cli/core/provisioning.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/core/utils.py` & `cloudinary-cli-1.7.0/cloudinary_cli/core/utils.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/core/uploader.py` & `cloudinary-cli-1.7.0/cloudinary_cli/core/uploader.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/core/overrides.py` & `cloudinary-cli-1.7.0/cloudinary_cli/core/overrides.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/core/config.py` & `cloudinary-cli-1.7.0/cloudinary_cli/core/config.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/core/__init__.py` & `cloudinary-cli-1.7.0/cloudinary_cli/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/modules/migrate.py` & `cloudinary-cli-1.7.0/cloudinary_cli/modules/migrate.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/modules/make.py` & `cloudinary-cli-1.7.0/cloudinary_cli/modules/make.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/modules/sync.py` & `cloudinary-cli-1.7.0/cloudinary_cli/modules/sync.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/modules/upload_dir.py` & `cloudinary-cli-1.7.0/cloudinary_cli/modules/upload_dir.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os.path import dirname, join as path_join
 from pathlib import Path
 
 from click import command, argument, option, style, launch
 
 from cloudinary_cli.utils.api_utils import upload_file
 from cloudinary_cli.utils.file_utils import get_destination_folder, is_hidden_path
-from cloudinary_cli.utils.utils import parse_option_value, logger, run_tasks_concurrently
+from cloudinary_cli.utils.utils import parse_option_value, logger, run_tasks_concurrently, group_params
 
 
 @command("upload_dir", help="""Upload a folder of assets, maintaining the folder structure.""")
 @argument("directory", default=".")
 @option("-g", "--glob-pattern", default="**/*", help="The glob pattern. "
                                                      "For example use '**/*.jpg' to upload only jpg files.")
 @option("-H", "--include-hidden", is_flag=True, help="Include hidden files.")
@@ -58,16 +58,15 @@
         "use_filename": True,
         "raw_transformation": transformation,
         "upload_preset": preset
     }
 
     options = {
         **defaults,
-        **{k: v for k, v in optional_parameter},
-        **{k: parse_option_value(v) for k, v in optional_parameter_parsed},
+        **group_params(optional_parameter, ((k, parse_option_value(v)) for k, v in optional_parameter_parsed)),
     }
 
     uploads = []
 
     for file_path in dir_to_upload.glob(glob_pattern):
         if file_path.is_file():
             if not include_hidden and is_hidden_path(file_path):
```

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/templates/html/upload_widget` & `cloudinary-cli-1.7.0/cloudinary_cli/templates/html/upload_widget`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/templates/html/media_library_widget` & `cloudinary-cli-1.7.0/cloudinary_cli/templates/html/media_library_widget`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/templates/html/video_player` & `cloudinary-cli-1.7.0/cloudinary_cli/templates/html/video_player`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/templates/python/find_all_empty_folders` & `cloudinary-cli-1.7.0/cloudinary_cli/templates/python/find_all_empty_folders`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/samples/__init__.py` & `cloudinary-cli-1.7.0/cloudinary_cli/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli/cli_group.py` & `cloudinary-cli-1.7.0/cloudinary_cli/cli_group.py`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/README.md` & `cloudinary-cli-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/LICENSE` & `cloudinary-cli-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli.egg-info/PKG-INFO` & `cloudinary-cli-1.7.0/cloudinary_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudinary-cli
-Version: 1.6.2
+Version: 1.7.0
 Summary: A command line interface for Cloudinary with full API support
 Home-page: https://github.com/cloudinary/cloudinary-cli
 Author: Cloudinary, Brian Luk
 Author-email: info@cloudinary.com, lukitsbrian@gmail.com
 License: MIT
 Keywords: cloudinary cli pycloudinary image video digital asset management command line interface transformation friendly easy flexible
 Platform: UNKNOWN
```

### Comparing `cloudinary-cli-1.6.2/cloudinary_cli.egg-info/SOURCES.txt` & `cloudinary-cli-1.7.0/cloudinary_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

