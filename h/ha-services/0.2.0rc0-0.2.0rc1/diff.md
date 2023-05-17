# Comparing `tmp/ha-services-0.2.0rc0.tar.gz` & `tmp/ha-services-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-services-0.2.0rc0.tar", last modified: Thu May 11 20:19:16 2023, max compression
+gzip compressed data, was "ha-services-0.2.0rc1.tar", last modified: Wed May 17 15:25:02 2023, max compression
```

## Comparing `ha-services-0.2.0rc0.tar` & `ha-services-0.2.0rc1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.596986 ha-services-0.2.0rc0/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-11 20:19:16.596986 ha-services-0.2.0rc0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)      823 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.2.0rc0/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/
--rw-rw-r--   0 jens      (1000) users      (100)      168 2023-05-11 20:09:11.000000 ha-services-0.2.0rc0/ha_services/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     8387 2023-05-11 19:19:19.000000 ha-services-0.2.0rc0/ha_services/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/cli/dev.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/cli_tools/
--rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.2.0rc0/ha_services/cli_tools/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.2.0rc0/ha_services/cli_tools/path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.2.0rc0/ha_services/cli_tools/richt_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/cli_tools/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc0/ha_services/cli_tools/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1042 2023-05-11 07:10:26.000000 ha-services-0.2.0rc0/ha_services/cli_tools/test_utils/assertion.py
--rw-rw-r--   0 jens      (1000) users      (100)      649 2023-05-11 07:16:45.000000 ha-services-0.2.0rc0/ha_services/cli_tools/test_utils/environment_fixtures.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/cli_tools/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc0/ha_services/cli_tools/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.2.0rc0/ha_services/cli_tools/tests/test_environ_fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.2.0rc0/ha_services/cli_tools/tests/test_path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.2.0rc0/ha_services/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     2686 2023-05-09 20:53:43.000000 ha-services-0.2.0rc0/ha_services/example.py
--rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/log_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     4083 2023-05-11 19:00:09.000000 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/tests/test_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/utilities/string_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services/systemd/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc0/ha_services/systemd/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     7245 2023-05-11 20:06:09.000000 ha-services-0.2.0rc0/ha_services/systemd/api.py
--rw-rw-r--   0 jens      (1000) users      (100)     3321 2023-05-11 17:07:16.000000 ha-services-0.2.0rc0/ha_services/systemd/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.2.0rc0/ha_services/systemd/defaults.py
--rw-rw-r--   0 jens      (1000) users      (100)      331 2023-05-09 19:57:06.000000 ha-services-0.2.0rc0/ha_services/systemd/service_template.txt
--rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.2.0rc0/ha_services/systemd/template.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.596986 ha-services-0.2.0rc0/ha_services/systemd/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc0/ha_services/systemd/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3155 2023-05-11 20:03:06.000000 ha-services-0.2.0rc0/ha_services/systemd/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     1491 2023-05-10 07:43:13.000000 ha-services-0.2.0rc0/ha_services/systemd/tests/test_data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.2.0rc0/ha_services/systemd/tests/test_template.py
--rw-rw-r--   0 jens      (1000) users      (100)     1752 2023-05-10 20:50:36.000000 ha-services-0.2.0rc0/ha_services/systemd/tests/utilities.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.596986 ha-services-0.2.0rc0/ha_services/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/tests/test_project_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.596986 ha-services-0.2.0rc0/ha_services/toml_settings/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/toml_settings/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4305 2023-05-11 20:06:55.000000 ha-services-0.2.0rc0/ha_services/toml_settings/api.py
--rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.2.0rc0/ha_services/toml_settings/data_class_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.2.0rc0/ha_services/toml_settings/debug.py
--rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.2.0rc0/ha_services/toml_settings/deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/toml_settings/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/toml_settings/sensible_editor.py
--rw-rw-r--   0 jens      (1000) users      (100)     1647 2023-05-09 20:53:17.000000 ha-services-0.2.0rc0/ha_services/toml_settings/serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.596986 ha-services-0.2.0rc0/ha_services/toml_settings/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc0/ha_services/toml_settings/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1229 2023-05-09 20:53:54.000000 ha-services-0.2.0rc0/ha_services/toml_settings/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1158 2023-05-09 20:43:45.000000 ha-services-0.2.0rc0/ha_services/toml_settings/tests/test_demo_settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     5607 2023-05-09 17:48:29.000000 ha-services-0.2.0rc0/ha_services/toml_settings/tests/test_deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     2758 2023-05-09 19:41:27.000000 ha-services-0.2.0rc0/ha_services/toml_settings/tests/test_serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-11 20:19:16.592986 ha-services-0.2.0rc0/ha_services.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-11 20:19:16.000000 ha-services-0.2.0rc0/ha_services.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     2405 2023-05-11 20:19:16.000000 ha-services-0.2.0rc0/ha_services.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-11 20:19:16.000000 ha-services-0.2.0rc0/ha_services.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-11 20:19:16.000000 ha-services-0.2.0rc0/ha_services.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-11 20:19:16.000000 ha-services-0.2.0rc0/ha_services.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-11 20:19:16.000000 ha-services-0.2.0rc0/ha_services.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.2.0rc0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53002 2023-05-09 17:59:29.000000 ha-services-0.2.0rc0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-09 17:59:13.000000 ha-services-0.2.0rc0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-11 20:19:16.596986 ha-services-0.2.0rc0/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.281539 ha-services-0.2.0rc1/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.281539 ha-services-0.2.0rc1/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)      823 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.2.0rc1/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/
+-rw-rw-r--   0 jens      (1000) users      (100)      168 2023-05-17 15:21:29.000000 ha-services-0.2.0rc1/ha_services/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8343 2023-05-17 15:18:45.000000 ha-services-0.2.0rc1/ha_services/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/cli/dev.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/cli_tools/
+-rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.2.0rc1/ha_services/cli_tools/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.2.0rc1/ha_services/cli_tools/path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.2.0rc1/ha_services/cli_tools/richt_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1042 2023-05-11 07:10:26.000000 ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/assertion.py
+-rw-rw-r--   0 jens      (1000) users      (100)      649 2023-05-11 07:16:45.000000 ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/environment_fixtures.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/cli_tools/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc1/ha_services/cli_tools/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.2.0rc1/ha_services/cli_tools/tests/test_environ_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.2.0rc1/ha_services/cli_tools/tests/test_path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.2.0rc1/ha_services/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3437 2023-05-17 15:17:40.000000 ha-services-0.2.0rc1/ha_services/example.py
+-rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/log_setup.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4083 2023-05-11 19:00:09.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/tests/test_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/utilities/string_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/systemd/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc1/ha_services/systemd/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7253 2023-05-17 15:14:11.000000 ha-services-0.2.0rc1/ha_services/systemd/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3185 2023-05-17 15:08:18.000000 ha-services-0.2.0rc1/ha_services/systemd/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.2.0rc1/ha_services/systemd/defaults.py
+-rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.2.0rc1/ha_services/systemd/service_template.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.2.0rc1/ha_services/systemd/template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/systemd/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3266 2023-05-17 15:21:16.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1439 2023-05-17 15:21:02.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/test_data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/test_template.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1934 2023-05-17 15:16:21.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/utilities.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/tests/test_project_setup.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/toml_settings/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/toml_settings/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4305 2023-05-11 20:06:55.000000 ha-services-0.2.0rc1/ha_services/toml_settings/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.2.0rc1/ha_services/toml_settings/data_class_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.2.0rc1/ha_services/toml_settings/debug.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.2.0rc1/ha_services/toml_settings/deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/toml_settings/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/toml_settings/sensible_editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1647 2023-05-09 20:53:17.000000 ha-services-0.2.0rc1/ha_services/toml_settings/serialize.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/toml_settings/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1229 2023-05-09 20:53:54.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_demo_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5607 2023-05-09 17:48:29.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2758 2023-05-09 19:41:27.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_serialize.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     2405 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.2.0rc1/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53002 2023-05-09 17:59:29.000000 ha-services-0.2.0rc1/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-09 17:59:13.000000 ha-services-0.2.0rc1/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/setup.cfg
```

### Comparing `ha-services-0.2.0rc0/.github/workflows/tests.yml` & `ha-services-0.2.0rc1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/PKG-INFO` & `ha-services-0.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ha-services-0.2.0rc0/README.md` & `ha-services-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/cli.py` & `ha-services-0.2.0rc1/cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/dev-cli.py` & `ha-services-0.2.0rc1/dev-cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/cli/cli_app.py` & `ha-services-0.2.0rc1/ha_services/cli/cli_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 from rich import print  # noqa
 from rich.console import Console
 from rich.traceback import install as rich_traceback_install
 from rich_click import RichGroup
 
 import ha_services
 from ha_services import __version__, constants
-from ha_services.example import DemoSettings, publish_forever
+from ha_services.example import DemoSettings, SystemdServiceInfo, publish_forever
 from ha_services.log_setup import basic_log_setup
 from ha_services.mqtt4homeassistant.data_classes import MqttSettings
 from ha_services.mqtt4homeassistant.mqtt import get_connected_client
 from ha_services.systemd.api import ServiceControl
-from ha_services.systemd.data_classes import SystemdServiceInfo
 from ha_services.toml_settings.api import TomlSettings
 
 
 logger = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = Path(ha_services.__file__).parent.parent
```

### Comparing `ha-services-0.2.0rc0/ha_services/cli/dev.py` & `ha-services-0.2.0rc1/ha_services/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/cli_tools/path_utils.py` & `ha-services-0.2.0rc1/ha_services/cli_tools/path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/cli_tools/richt_utils.py` & `ha-services-0.2.0rc1/ha_services/cli_tools/richt_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/cli_tools/test_utils/assertion.py` & `ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/assertion.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/cli_tools/test_utils/environment_fixtures.py` & `ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/environment_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/cli_tools/tests/test_environ_fixtures.py` & `ha-services-0.2.0rc1/ha_services/cli_tools/tests/test_environ_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/cli_tools/tests/test_path_utils.py` & `ha-services-0.2.0rc1/ha_services/cli_tools/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/converter.py` & `ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/data_classes.py` & `ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/mqtt.py` & `ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/mqtt4homeassistant/tests/test_converter.py` & `ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/systemd/api.py` & `ha-services-0.2.0rc1/ha_services/systemd/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 from manageprojects.utilities.subprocess_utils import verbose_check_call
 from rich import print  # noqa
 from rich.console import Console
 from rich.highlighter import ReprHighlighter
 
 from ha_services.cli_tools.richt_utils import PanelPrinter, human_error, print_code, print_unified_diff
-from ha_services.systemd.data_classes import SystemdServiceInfo
+from ha_services.systemd.data_classes import BaseSystemdServiceInfo
 
 
 logger = logging.getLogger(__name__)
 
 
 class SystemdServiceError(RuntimeError):
     pass
 
 
 class ServiceControl:
     """
     Manage Systemd service
     """
 
-    def __init__(self, info: SystemdServiceInfo):
+    def __init__(self, info: BaseSystemdServiceInfo):
         self.info = info
         self.service_name = info.service_file_path.name
 
     ##################################################################################################
     # Helper
 
     def sudo_hint_exception_exit(self, err, exit_code=1):
```

### Comparing `ha-services-0.2.0rc0/ha_services/systemd/data_classes.py` & `ha-services-0.2.0rc1/ha_services/systemd/data_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 import dataclasses
 from pathlib import Path
 from string import Template
 
 from bx_py_utils.path import assert_is_dir, assert_is_file
 
-from ha_services import __version__
 from ha_services.cli_tools.richt_utils import human_error
 from ha_services.mqtt4homeassistant.utilities.string_utils import slugify
 from ha_services.systemd.defaults import (
     get_demo_exec_start,
     get_template_path,
     get_user_group,
     get_user_name,
     get_work_directory,
 )
 from ha_services.systemd.template import InvalidTemplate, validate_template
 
 
 @dataclasses.dataclass
-class SystemdServiceTemplateContext:
+class BaseSystemdServiceTemplateContext:
     """
-    Context values for the systemd service file content.
-    Defaults are for the "DEMO publish-loop"
+    Context values for the systemd service file content
     """
 
-    verbose_service_name: str = 'HaServices Demo'
+    verbose_service_name: str  # Must be set in child class!
 
-    version: str = __version__
     user: str = dataclasses.field(default_factory=get_user_name)
     group: str = dataclasses.field(default_factory=get_user_group)
     work_dir: Path = dataclasses.field(default_factory=get_work_directory)
 
     exec_start: str = dataclasses.field(default_factory=get_demo_exec_start)
 
     # Optional values, will be automatically filled:
     syslog_identifier: str = None
 
 
 @dataclasses.dataclass
-class SystemdServiceInfo:
+class BaseSystemdServiceInfo:
     """
-    Information for systemd helper functions.
-    Defaults are for the "DEMO publish-loop"
+    Information for systemd helper functions
     """
 
+    template_context: BaseSystemdServiceTemplateContext  # Must be set in child class!
+
     template_path: Path = dataclasses.field(default_factory=get_template_path)
 
     systemd_base_path: Path = Path('/etc/systemd/system/')
 
-    # Set by post init:
+    # Set by post init from "template_context" information:
     service_slug: str = None
     service_file_path: Path = None
 
-    template_context: SystemdServiceTemplateContext = dataclasses.field(default_factory=SystemdServiceTemplateContext)
-
     def __post_init__(self):
         assert_is_dir(self.systemd_base_path)
         assert_is_dir(self.template_context.work_dir)
         assert_is_file(self.template_path)
 
         if not self.service_slug:
             self.service_slug = slugify(self.template_context.verbose_service_name, sep='_').lower()
```

### Comparing `ha-services-0.2.0rc0/ha_services/systemd/template.py` & `ha-services-0.2.0rc1/ha_services/systemd/template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/systemd/tests/test_api.py` & `ha-services-0.2.0rc1/ha_services/systemd/tests/test_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,43 +2,46 @@
 from unittest.mock import patch
 
 from bx_py_utils.path import assert_is_file
 from bx_py_utils.test_utils.redirect import RedirectOut
 from manageprojects.test_utils.subprocess import SubprocessCallMock
 from manageprojects.utilities import subprocess_utils
 
-from ha_services import __version__
+
 from ha_services.cli_tools.test_utils.assertion import assert_in
+from ha_services.example import SystemdServiceInfo
 from ha_services.systemd.api import ServiceControl
 from ha_services.systemd.tests.utilities import MockedSystemdServiceInfo
 
 
 class MockedShutilWhich:
     def which(self, command, path=None):
         return f'/usr/bin/{command}'
 
 
 class SystemdApiTestCase(TestCase):
     def test_print_systemd_file(self):
-        with MockedSystemdServiceInfo(prefix='test_print_systemd_file_') as info, RedirectOut() as buffer:
+        with MockedSystemdServiceInfo(
+            prefix='test_print_systemd_file_', SystemdServiceInfoClass=SystemdServiceInfo
+        ) as info, RedirectOut() as buffer:
             ServiceControl(info=info).debug_systemd_config()
 
         self.assertEqual(buffer.stderr, '')
         assert_in(
             content=buffer.stdout,
             parts=(
                 '[Unit]',
-                f'Description=HaServices Demo {__version__}',
+                'Description=HaServices Demo',
                 'ExecStart=/mocked/.venv/bin/python3 -m ha_services_app publish-loop',
                 'SyslogIdentifier=haservices_demo',
             ),
         )
 
     def test_service_control(self):
-        with MockedSystemdServiceInfo(prefix='test_') as info:
+        with MockedSystemdServiceInfo(prefix='test_', SystemdServiceInfoClass=SystemdServiceInfo) as info:
             service_control = ServiceControl(info=info)
 
             for func_name in ('enable', 'restart', 'stop', 'status', 'remove_systemd_service'):
                 with self.subTest(func_name):
                     service_control_func = getattr(service_control, func_name)
                     with RedirectOut() as buffer, self.assertRaises(SystemExit):
                         service_control_func()
```

### Comparing `ha-services-0.2.0rc0/ha_services/systemd/tests/test_data_classes.py` & `ha-services-0.2.0rc1/ha_services/systemd/tests/test_data_classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import tempfile
 from pathlib import Path
 from unittest import TestCase
 
-from ha_services import __version__
-from ha_services.systemd.data_classes import SystemdServiceInfo
+from ha_services.example import SystemdServiceInfo
 from ha_services.systemd.tests.utilities import MockedSystemdServiceInfo
 
 
 class SystemdDataClassesTestCase(TestCase):
     def test_systemd_service_info(self):
         info = SystemdServiceInfo()
 
         # Check some samples:
         self.assertEqual(info.template_context.verbose_service_name, 'HaServices Demo')
-        self.assertEqual(info.template_context.version, __version__)
         self.assertEqual(info.service_slug, 'haservices_demo')
         self.assertEqual(info.template_context.syslog_identifier, 'haservices_demo')
         self.assertEqual(info.service_file_path, Path('/etc/systemd/system/haservices_demo.service'))
 
-        with MockedSystemdServiceInfo(prefix='test_systemd_service_info_') as info:
+        with MockedSystemdServiceInfo(
+            prefix='test_systemd_service_info_', SystemdServiceInfoClass=SystemdServiceInfo
+        ) as info:
             self.assertIsInstance(info, SystemdServiceInfo)
             self.assertEqual(info.template_context.user, 'MockedUserName')
             self.assertEqual(info.template_context.group, 'MockedUserName')
             self.assertEqual(
                 info.template_context.exec_start, '/mocked/.venv/bin/python3 -m ha_services_app publish-loop'
             )
```

### Comparing `ha-services-0.2.0rc0/ha_services/systemd/tests/test_template.py` & `ha-services-0.2.0rc1/ha_services/systemd/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/tests/test_project_setup.py` & `ha-services-0.2.0rc1/ha_services/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/api.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/debug.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/debug.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/deserialize.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/deserialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/sensible_editor.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/sensible_editor.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/serialize.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/serialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/tests/fixtures.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/tests/test_demo_settings.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_demo_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 from unittest import TestCase
 
 from tomlkit import TOMLDocument
 
 from ha_services.example import DemoSettings
-from ha_services.systemd.data_classes import SystemdServiceInfo
 from ha_services.toml_settings.deserialize import toml2dataclass
 from ha_services.toml_settings.serialize import dataclass2toml
 
 
 class TomlSettingsTestCase(TestCase):
     def test_demo_settings(self):
         document = dataclass2toml(instance=DemoSettings())
@@ -16,13 +15,13 @@
         data = document.unwrap()
 
         self.assertEqual(data['app']['device_name'], 'ha-services-demo')
         self.assertEqual(data['mqtt']['host'], 'mqtt.eclipseprojects.io')
         self.assertEqual(data['systemd']['service_slug'], 'haservices_demo')
         self.assertEqual(data['systemd']['systemd_base_path'], '/etc/systemd/system')
 
-        instance = DemoSettings(systemd=SystemdServiceInfo(service_slug='foo bar'))
+        instance = DemoSettings()
         instance.systemd.systemd_base_path = Path('/foo/bar')
 
         toml2dataclass(document=document, instance=instance)
 
         self.assertEqual(instance.systemd.systemd_base_path, Path('/etc/systemd/system'))
```

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/tests/test_deserialize.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_deserialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services/toml_settings/tests/test_serialize.py` & `ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/ha_services.egg-info/PKG-INFO` & `ha-services-0.2.0rc1/ha_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ha-services-0.2.0rc0/ha_services.egg-info/SOURCES.txt` & `ha-services-0.2.0rc1/ha_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/pyproject.toml` & `ha-services-0.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/requirements.dev.txt` & `ha-services-0.2.0rc1/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc0/requirements.txt` & `ha-services-0.2.0rc1/requirements.txt`

 * *Files identical despite different names*

