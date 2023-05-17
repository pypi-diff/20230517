# Comparing `tmp/pyapp-4.8.2.tar.gz` & `tmp/pyapp-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapp-4.8.2.tar", max compression
+gzip compressed data, was "pyapp-4.9.0.tar", max compression
```

## Comparing `pyapp-4.8.2.tar` & `pyapp-4.9.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     5344 2022-06-23 23:06:02.770337 pyapp-4.8.2/HISTORY
--rw-r--r--   0        0        0     1501 2022-06-23 23:06:02.770337 pyapp-4.8.2/LICENSE
--rw-r--r--   0        0        0     7422 2022-06-23 23:06:02.770337 pyapp-4.8.2/README.rst
--rw-r--r--   0        0        0     1652 2022-06-23 23:06:02.770337 pyapp-4.8.2/pyproject.toml
--rw-r--r--   0        0        0      387 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/__init__.py
--rw-r--r--   0        0        0    18726 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/app/__init__.py
--rw-r--r--   0        0        0     6024 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/app/argument_actions.py
--rw-r--r--   0        0        0     1298 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/app/argument_types.py
--rw-r--r--   0        0        0    16299 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/app/arguments.py
--rw-r--r--   0        0        0     2779 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/app/builtin_handlers.py
--rw-r--r--   0        0        0     1145 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/app/init_logger.py
--rw-r--r--   0        0        0     1350 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/app/logging_formatter.py
--rw-r--r--   0        0        0     1444 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/checks/__init__.py
--rw-r--r--   0        0        0      459 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/checks/built_in.py
--rw-r--r--   0        0        0     3865 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/checks/messages.py
--rw-r--r--   0        0        0     4174 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/checks/registry.py
--rw-r--r--   0        0        0     9719 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/checks/report.py
--rw-r--r--   0        0        0      838 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/compatability.py
--rw-r--r--   0        0        0    11464 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/__init__.py
--rw-r--r--   0        0        0     2809 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/base_settings.py
--rw-r--r--   0        0        0    10083 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/helpers/__init__.py
--rw-r--r--   0        0        0     2633 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/helpers/bases.py
--rw-r--r--   0        0        0    12492 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/helpers/plugins.py
--rw-r--r--   0        0        0     7063 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/helpers/providers.py
--rw-r--r--   0        0        0     4418 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/loaders/__init__.py
--rw-r--r--   0        0        0      962 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/loaders/base.py
--rw-r--r--   0        0        0     2747 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/loaders/content_types.py
--rw-r--r--   0        0        0     2035 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/loaders/file_loader.py
--rw-r--r--   0        0        0     3395 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/loaders/http_loader.py
--rw-r--r--   0        0        0     1823 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/conf/report.py
--rw-r--r--   0        0        0     7787 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/events.py
--rw-r--r--   0        0        0     1520 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/exceptions.py
--rw-r--r--   0        0        0     3166 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/extensions/__init__.py
--rw-r--r--   0        0        0     4241 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/extensions/registry.py
--rw-r--r--   0        0        0     3030 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/extensions/report.py
--rw-r--r--   0        0        0     4785 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/feature_flags.py
--rw-r--r--   0        0        0     4809 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/injection.py
--rw-r--r--   0        0        0        8 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/py.typed
--rw-r--r--   0        0        0     1982 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/utils/__init__.py
--rw-r--r--   0        0        0     1219 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/utils/compatibility.py
--rw-r--r--   0        0        0     1581 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/utils/inspect.py
--rw-r--r--   0        0        0     1259 2022-06-23 23:06:02.774337 pyapp-4.8.2/src/pyapp/versioning.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/app/__init__.py
--rw-r--r--   0        0        0     5145 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/app/test_app.py
--rw-r--r--   0        0        0     3544 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/app/test_argument_actions.py
--rw-r--r--   0        0        0      755 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/app/test_argument_types.py
--rw-r--r--   0        0        0     5279 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/app/test_arguments.py
--rw-r--r--   0        0        0     9532 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/app/test_arguments_signatures.py
--rw-r--r--   0        0        0      545 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/app/test_init_logger.py
--rw-r--r--   0        0        0      570 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/app/test_logging_formatter.py
--rw-r--r--   0        0        0      511 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/checks/test_built_in.py
--rw-r--r--   0        0        0     4538 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/checks/test_checks_registry.py
--rw-r--r--   0        0        0     3155 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/checks/test_messages.py
--rw-r--r--   0        0        0     1321 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/checks/test_report.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/__init__.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/helpers/__init__.py
--rw-r--r--   0        0        0     5622 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/helpers/test_.py
--rw-r--r--   0        0        0    13051 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/helpers/test_plugin_factories.py
--rw-r--r--   0        0        0     5001 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/helpers/test_providers_factories.py
--rw-r--r--   0        0        0     1382 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/helpers/test_singleton_factories.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/loaders/__init__.py
--rw-r--r--   0        0        0     3548 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/loaders/test_.py
--rw-r--r--   0        0        0     2055 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/loaders/test_content_types.py
--rw-r--r--   0        0        0     1449 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/loaders/test_file_loader.py
--rw-r--r--   0        0        0     4564 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/loaders/test_http_loader.py
--rw-r--r--   0        0        0     6305 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/test_.py
--rw-r--r--   0        0        0      200 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conf/test_report.py
--rw-r--r--   0        0        0      362 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/extensions/__init__.py
--rw-r--r--   0        0        0     5257 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/extensions/test_registry.py
--rw-r--r--   0        0        0     1652 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/extensions/test_report.py
--rw-r--r--   0        0        0      494 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/factory/__init__.py
--rw-r--r--   0        0        0       85 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/fixtures/settings-invalid-container.json
--rw-r--r--   0        0        0       24 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/fixtures/settings-invalid-file.json
--rw-r--r--   0        0        0       71 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/fixtures/settings.json
--rw-r--r--   0        0        0      537 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/mock.py
--rw-r--r--   0        0        0       60 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/runtime_settings.py
--rw-r--r--   0        0        0      111 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/runtime_settings_with_imports.py
--rw-r--r--   0        0        0       22 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_app/__init__.py
--rw-r--r--   0        0        0     1636 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_app/__main__.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_app/alt_checks.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_app/checks.py
--rw-r--r--   0        0        0      128 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_app/default_settings.py
--rw-r--r--   0        0        0      130 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_app/logging_settings.py
--rw-r--r--   0        0        0      109 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_app_simple.py
--rw-r--r--   0        0        0      361 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_ext/__init__.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_ext/checks.py
--rw-r--r--   0        0        0       25 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_ext/default_settings.py
--rw-r--r--   0        0        0      271 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/sample_ext_simple/__init__.py
--rw-r--r--   0        0        0     1240 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/settings.py
--rw-r--r--   0        0        0      273 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/test_compatability.py
--rw-r--r--   0        0        0     6153 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/test_events.py
--rw-r--r--   0        0        0     4436 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/test_feature_flags.py
--rw-r--r--   0        0        0     2939 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/test_injection.py
--rw-r--r--   0        0        0       82 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/test_pyapp.py
--rw-r--r--   0        0        0     1683 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/test_versioning.py
--rw-r--r--   0        0        0        0 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/utils/__init__.py
--rw-r--r--   0        0        0     1134 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/utils/test_.py
--rw-r--r--   0        0        0      747 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/utils/test_compatibility.py
--rw-r--r--   0        0        0     1803 2022-06-23 23:06:02.774337 pyapp-4.8.2/tests/utils/test_inspect.py
--rw-r--r--   0        0        0     8776 2022-06-23 23:06:14.564504 pyapp-4.8.2/setup.py
--rw-r--r--   0        0        0     8875 2022-06-23 23:06:14.565328 pyapp-4.8.2/PKG-INFO
+-rw-r--r--   0        0        0     5622 2022-09-15 01:04:10.622802 pyapp-4.9.0/HISTORY
+-rw-r--r--   0        0        0     1501 2022-09-15 01:04:10.622802 pyapp-4.9.0/LICENSE
+-rw-r--r--   0        0        0     7422 2022-09-15 01:04:10.622802 pyapp-4.9.0/README.rst
+-rw-r--r--   0        0        0     1650 2022-09-15 01:04:10.626802 pyapp-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0      387 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/__init__.py
+-rw-r--r--   0        0        0    18726 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/app/__init__.py
+-rw-r--r--   0        0        0     6024 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/app/argument_actions.py
+-rw-r--r--   0        0        0     1298 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/app/argument_types.py
+-rw-r--r--   0        0        0    16340 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/app/arguments.py
+-rw-r--r--   0        0        0     2779 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/app/builtin_handlers.py
+-rw-r--r--   0        0        0     1145 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/app/init_logger.py
+-rw-r--r--   0        0        0     1350 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/app/logging_formatter.py
+-rw-r--r--   0        0        0     1444 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/checks/__init__.py
+-rw-r--r--   0        0        0      459 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/checks/built_in.py
+-rw-r--r--   0        0        0     3865 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/checks/messages.py
+-rw-r--r--   0        0        0     4174 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/checks/registry.py
+-rw-r--r--   0        0        0     9719 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/checks/report.py
+-rw-r--r--   0        0        0      109 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/compatability.py
+-rw-r--r--   0        0        0    12769 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/__init__.py
+-rw-r--r--   0        0        0     2809 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/base_settings.py
+-rw-r--r--   0        0        0    10083 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/helpers/__init__.py
+-rw-r--r--   0        0        0     2633 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/helpers/bases.py
+-rw-r--r--   0        0        0    12492 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/helpers/plugins.py
+-rw-r--r--   0        0        0     7063 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/helpers/providers.py
+-rw-r--r--   0        0        0     4418 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/loaders/__init__.py
+-rw-r--r--   0        0        0      962 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/loaders/base.py
+-rw-r--r--   0        0        0     2747 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/loaders/content_types.py
+-rw-r--r--   0        0        0     2035 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/loaders/file_loader.py
+-rw-r--r--   0        0        0     3395 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/loaders/http_loader.py
+-rw-r--r--   0        0        0     1823 2022-09-15 01:04:10.626802 pyapp-4.9.0/src/pyapp/conf/report.py
+-rw-r--r--   0        0        0     7787 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/events.py
+-rw-r--r--   0        0        0     1520 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/exceptions.py
+-rw-r--r--   0        0        0     3166 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/extensions/__init__.py
+-rw-r--r--   0        0        0     4241 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/extensions/registry.py
+-rw-r--r--   0        0        0     3030 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/extensions/report.py
+-rw-r--r--   0        0        0     4785 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/feature_flags.py
+-rw-r--r--   0        0        0     4809 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/injection.py
+-rw-r--r--   0        0        0        8 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/py.typed
+-rw-r--r--   0        0        0     1982 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/utils/__init__.py
+-rw-r--r--   0        0        0     1219 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/utils/compatibility.py
+-rw-r--r--   0        0        0     1581 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/utils/inspect.py
+-rw-r--r--   0        0        0     1259 2022-09-15 01:04:10.630802 pyapp-4.9.0/src/pyapp/versioning.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/app/__init__.py
+-rw-r--r--   0        0        0     5145 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/app/test_app.py
+-rw-r--r--   0        0        0     3544 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/app/test_argument_actions.py
+-rw-r--r--   0        0        0      755 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/app/test_argument_types.py
+-rw-r--r--   0        0        0     5279 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/app/test_arguments.py
+-rw-r--r--   0        0        0     9532 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/app/test_arguments_signatures.py
+-rw-r--r--   0        0        0      545 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/app/test_init_logger.py
+-rw-r--r--   0        0        0      570 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/app/test_logging_formatter.py
+-rw-r--r--   0        0        0      511 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/checks/test_built_in.py
+-rw-r--r--   0        0        0     4538 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/checks/test_checks_registry.py
+-rw-r--r--   0        0        0     3155 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/checks/test_messages.py
+-rw-r--r--   0        0        0     1321 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/checks/test_report.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/helpers/__init__.py
+-rw-r--r--   0        0        0     5622 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/helpers/test_.py
+-rw-r--r--   0        0        0    13051 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/helpers/test_plugin_factories.py
+-rw-r--r--   0        0        0     5001 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/helpers/test_providers_factories.py
+-rw-r--r--   0        0        0     1382 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/helpers/test_singleton_factories.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/loaders/__init__.py
+-rw-r--r--   0        0        0     3548 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/loaders/test_.py
+-rw-r--r--   0        0        0     2055 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/loaders/test_content_types.py
+-rw-r--r--   0        0        0     1449 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/loaders/test_file_loader.py
+-rw-r--r--   0        0        0     4564 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/loaders/test_http_loader.py
+-rw-r--r--   0        0        0     8250 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/test_.py
+-rw-r--r--   0        0        0      200 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conf/test_report.py
+-rw-r--r--   0        0        0      362 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/extensions/__init__.py
+-rw-r--r--   0        0        0     5257 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/extensions/test_registry.py
+-rw-r--r--   0        0        0     1652 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/extensions/test_report.py
+-rw-r--r--   0        0        0      451 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/factory/__init__.py
+-rw-r--r--   0        0        0       85 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/fixtures/settings-invalid-container.json
+-rw-r--r--   0        0        0       24 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/fixtures/settings-invalid-file.json
+-rw-r--r--   0        0        0       71 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/fixtures/settings.json
+-rw-r--r--   0        0        0      537 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/mock.py
+-rw-r--r--   0        0        0       60 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/runtime_settings.py
+-rw-r--r--   0        0        0      111 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/runtime_settings_with_imports.py
+-rw-r--r--   0        0        0       22 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_app/__init__.py
+-rw-r--r--   0        0        0     1636 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_app/__main__.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_app/alt_checks.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_app/checks.py
+-rw-r--r--   0        0        0      128 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_app/default_settings.py
+-rw-r--r--   0        0        0      130 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_app/logging_settings.py
+-rw-r--r--   0        0        0      109 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_app_simple.py
+-rw-r--r--   0        0        0      361 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_ext/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_ext/checks.py
+-rw-r--r--   0        0        0       25 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_ext/default_settings.py
+-rw-r--r--   0        0        0      271 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/sample_ext_simple/__init__.py
+-rw-r--r--   0        0        0     1240 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/settings.py
+-rw-r--r--   0        0        0      273 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/test_compatability.py
+-rw-r--r--   0        0        0     6153 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/test_events.py
+-rw-r--r--   0        0        0     4436 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/test_feature_flags.py
+-rw-r--r--   0        0        0     2939 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/test_injection.py
+-rw-r--r--   0        0        0       82 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/test_pyapp.py
+-rw-r--r--   0        0        0     1683 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/test_versioning.py
+-rw-r--r--   0        0        0        0 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1134 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/utils/test_.py
+-rw-r--r--   0        0        0      747 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/utils/test_compatibility.py
+-rw-r--r--   0        0        0     1803 2022-09-15 01:04:10.630802 pyapp-4.9.0/tests/utils/test_inspect.py
+-rw-r--r--   0        0        0     8780 1970-01-01 00:00:00.000000 pyapp-4.9.0/setup.py
+-rw-r--r--   0        0        0     9024 1970-01-01 00:00:00.000000 pyapp-4.9.0/PKG-INFO
```

### Comparing `pyapp-4.8.2/HISTORY` & `pyapp-4.9.0/HISTORY`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+4.9.0
+=====
+
+Changes
+--------
+
+- Changed settings to be support being pickled.
+
+- Added feature to export and restore settings into a serialised form for
+  use-cases where settings need to be duplicated (eg deploying tasks into a
+  spark cluster where settings are required).
+
+
 4.8.2
 =====
 
 Changes
 --------
 
 - Extend change to RegexType to allow for any custom ArgumentType by extending
```

### Comparing `pyapp-4.8.2/LICENSE` & `pyapp-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/README.rst` & `pyapp-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/pyproject.toml` & `pyapp-4.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1.0", "rtd-poetry-tmp"]
 build-backend = "rtd_poetry"
 
 [tool.poetry]
 name = "pyapp"
-version = "4.8.2"
+version = "4.9.0"
 description = "A Python application framework - Let us handle the boring stuff!"
 authors = ["Tim Savage <tim@savage.company>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 repository = "https://github.com/pyapp-org/pyapp"
 documentation = "https://docs.pyapp.info"
 keywords = ["framework", "application"]
@@ -29,28 +29,28 @@
 packages = [
     { include = "pyapp", from = "src" },
     { include = "tests", format = "sdist" },
 ]
 include = ["HISTORY"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 argcomplete = "*"
 colorama = "*"
 yarl = "*"
 
 pyyaml = {version = "*", optional = true }
 toml = {version = "*", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
-pytest-asyncio = "^0.18.3"
+pytest-asyncio = "^0.19"
 nox = "*"
-sphinx = "^4.5.0"
+sphinx = "^5.0.2"
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
 toml = ["toml"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/pyapp-org/pyapp/issues"
```

### Comparing `pyapp-4.8.2/src/pyapp/app/__init__.py` & `pyapp-4.9.0/src/pyapp/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/app/argument_actions.py` & `pyapp-4.9.0/src/pyapp/app/argument_actions.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/app/argument_types.py` & `pyapp-4.9.0/src/pyapp/app/argument_types.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/app/arguments.py` & `pyapp-4.9.0/src/pyapp/app/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,17 @@
 class ArgumentType(abc.ABC):
     """
     Custom argument type
     """
 
     @abc.abstractmethod
     def __call__(self, value: str) -> Any:
-        ...
+        """
+        Construct a value from type
+        """
 
 
 class Argument:
     """
     Decorator for adding arguments to a handler.
 
     This decorator can be used before or after the handler registration
@@ -166,15 +168,15 @@
     :param name_or_flags: Either a name or a list of option strings, e.g. foo or -f, --foo.
     :param action: The basic type of action to be taken when this argument is encountered at the command line.
     :param nargs: The number of command-line arguments that should be consumed.
     :param const: A constant value required by some action and nargs selections.
     :param default: The value produced if the argument is absent from the command line.
     :param type: The type to which the command-line argument should be converted.
     :param choices: A container of the allowable values for the argument.
-    :param required: Whether or not the command-line option may be omitted (optionals only).
+    :param required: Whether the command-line option may be omitted (optionals only).
     :param help_text: A brief description of what the argument does.
     :param metavar: A name for the argument in usage messages.
     :param dest: The name of the attribute to be added to the object returned by parse_args().
 
     """
 
     __slots__ = ("kwargs", "name_or_flags")
```

### Comparing `pyapp-4.8.2/src/pyapp/app/builtin_handlers.py` & `pyapp-4.9.0/src/pyapp/app/builtin_handlers.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/app/init_logger.py` & `pyapp-4.9.0/src/pyapp/app/init_logger.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/app/logging_formatter.py` & `pyapp-4.9.0/src/pyapp/app/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/checks/__init__.py` & `pyapp-4.9.0/src/pyapp/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/checks/messages.py` & `pyapp-4.9.0/src/pyapp/checks/messages.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/checks/registry.py` & `pyapp-4.9.0/src/pyapp/checks/registry.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/checks/report.py` & `pyapp-4.9.0/src/pyapp/checks/report.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/__init__.py` & `pyapp-4.9.0/src/pyapp/conf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,19 +90,22 @@
 .. autoclass:: HttpLoader
 
 """
 import logging
 import os
 import warnings
 from typing import Any
+from typing import Dict
 from typing import Iterable
 from typing import List
+from typing import Protocol
 from typing import Sequence
 from typing import Tuple
 from typing import Union
+from typing.io import IO
 
 from pyapp.conf import base_settings
 from pyapp.conf.loaders import Loader
 from pyapp.conf.loaders import ModuleLoader
 
 from . import loaders
 
@@ -197,24 +200,24 @@
 
         # Save and remove existing settings
         saved_settings = [(key, container.__dict__.pop(key)) for key in container.keys]
 
         # Initialise base settings
         container._populate_base_settings()  # pylint: disable=protected-access
 
-        def restore_settings():
+        def restore_():
             # Remove new settings
             for key in container.keys:
                 del container.__dict__[key]
 
             # Restore saved settings
             container.__dict__.update(saved_settings)
 
         # Add restore action
-        action = restore_settings, ()
+        action = restore_, ()
         self._roll_back.append(action)
 
 
 class Settings:
     """
     Settings container
     """
@@ -227,14 +230,20 @@
 
     def __setattr__(self, key, value):
         raise AttributeError("Readonly object")
 
     def __getitem__(self, item):
         return self.__dict__[item]
 
+    def __getstate__(self) -> Dict[str, Any]:
+        return dict(self.items())
+
+    def __setstate__(self, state: Dict[str, Any]):
+        self.__dict__.update(state)
+
     def __repr__(self) -> str:
         sources = self.SETTINGS_SOURCES or "UN-CONFIGURED"
         return f"{self.__class__.__name__}({sources})"
 
     def _populate_base_settings(self, base_settings_=None):
         base_settings_ = base_settings_ or base_settings
 
@@ -371,7 +380,49 @@
         :rtype: ModifySettingsContext
 
         """
         return ModifySettingsContext(self)
 
 
 settings = Settings()  # pylint: disable=invalid-name
+
+
+class Serialiser(Protocol):
+    """
+    Protocol a serialiser must meet
+    """
+
+    def dump(self, obj: Dict[str, Any], file: IO):
+        """
+        Dump data into the file(like) object
+        """
+
+    def load(self, file: IO) -> Dict[str, Any]:
+        """
+        Load data from a file(like) object
+        """
+
+
+def export_settings(file: IO, *, serialiser: Serialiser = None):
+    """
+    Export settings into specified file(like) object using specified serialiser.
+
+    The default serialiser is pickle
+    """
+    if serialiser is None:
+        import pickle as serialiser  # pylint: disable=import-outside-toplevel
+
+    state = settings.__getstate__()
+    serialiser.dump(state, file)
+
+
+def restore_settings(file: IO, *, serialiser: Serialiser = None):
+    """
+    Restore settings from specified file(like) object using specified serialiser.
+
+    The default serialiser is pickle
+    """
+    if serialiser is None:
+        import pickle as serialiser  # pylint: disable=import-outside-toplevel
+
+    state = serialiser.load(file)
+    settings.__setstate__(state)
```

### Comparing `pyapp-4.8.2/src/pyapp/conf/base_settings.py` & `pyapp-4.9.0/src/pyapp/conf/base_settings.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/helpers/__init__.py` & `pyapp-4.9.0/src/pyapp/conf/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/helpers/bases.py` & `pyapp-4.9.0/src/pyapp/conf/helpers/bases.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/helpers/plugins.py` & `pyapp-4.9.0/src/pyapp/conf/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/helpers/providers.py` & `pyapp-4.9.0/src/pyapp/conf/helpers/providers.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/loaders/__init__.py` & `pyapp-4.9.0/src/pyapp/conf/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/loaders/base.py` & `pyapp-4.9.0/src/pyapp/conf/loaders/base.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/loaders/content_types.py` & `pyapp-4.9.0/src/pyapp/conf/loaders/content_types.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/loaders/file_loader.py` & `pyapp-4.9.0/src/pyapp/conf/loaders/file_loader.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/loaders/http_loader.py` & `pyapp-4.9.0/src/pyapp/conf/loaders/http_loader.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/conf/report.py` & `pyapp-4.9.0/src/pyapp/conf/report.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/events.py` & `pyapp-4.9.0/src/pyapp/events.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/exceptions.py` & `pyapp-4.9.0/src/pyapp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/extensions/__init__.py` & `pyapp-4.9.0/src/pyapp/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/extensions/registry.py` & `pyapp-4.9.0/src/pyapp/extensions/registry.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/extensions/report.py` & `pyapp-4.9.0/src/pyapp/extensions/report.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/feature_flags.py` & `pyapp-4.9.0/src/pyapp/feature_flags.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/injection.py` & `pyapp-4.9.0/src/pyapp/injection.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/utils/__init__.py` & `pyapp-4.9.0/src/pyapp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/utils/compatibility.py` & `pyapp-4.9.0/src/pyapp/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/utils/inspect.py` & `pyapp-4.9.0/src/pyapp/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/src/pyapp/versioning.py` & `pyapp-4.9.0/src/pyapp/versioning.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/app/test_app.py` & `pyapp-4.9.0/tests/app/test_app.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/app/test_argument_actions.py` & `pyapp-4.9.0/tests/app/test_argument_actions.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/app/test_argument_types.py` & `pyapp-4.9.0/tests/app/test_argument_types.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/app/test_arguments.py` & `pyapp-4.9.0/tests/app/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/app/test_arguments_signatures.py` & `pyapp-4.9.0/tests/app/test_arguments_signatures.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/app/test_init_logger.py` & `pyapp-4.9.0/tests/app/test_init_logger.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/app/test_logging_formatter.py` & `pyapp-4.9.0/tests/app/test_logging_formatter.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/checks/test_checks_registry.py` & `pyapp-4.9.0/tests/checks/test_checks_registry.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/checks/test_messages.py` & `pyapp-4.9.0/tests/checks/test_messages.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/checks/test_report.py` & `pyapp-4.9.0/tests/checks/test_report.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/helpers/test_.py` & `pyapp-4.9.0/tests/conf/helpers/test_.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/helpers/test_plugin_factories.py` & `pyapp-4.9.0/tests/conf/helpers/test_plugin_factories.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/helpers/test_providers_factories.py` & `pyapp-4.9.0/tests/conf/helpers/test_providers_factories.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/helpers/test_singleton_factories.py` & `pyapp-4.9.0/tests/conf/helpers/test_singleton_factories.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/loaders/test_.py` & `pyapp-4.9.0/tests/conf/loaders/test_.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/loaders/test_content_types.py` & `pyapp-4.9.0/tests/conf/loaders/test_content_types.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/loaders/test_file_loader.py` & `pyapp-4.9.0/tests/conf/loaders/test_file_loader.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/loaders/test_http_loader.py` & `pyapp-4.9.0/tests/conf/loaders/test_http_loader.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/conf/test_.py` & `pyapp-4.9.0/tests/conf/test_.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import json
+from io import BytesIO
+from io import StringIO
+from unittest.mock import patch
+
 import pyapp.conf
 import pytest
 
 
 class TestSettings:
     @pytest.fixture
     def target(self) -> pyapp.conf.Settings:
@@ -165,7 +170,58 @@
             assert isinstance(target.LOGGING, dict), "Base settings missing"
 
         # Check items have been restored
         assert initial_keys == target.keys, "All settings not restored"
         assert target.SETTINGS_SOURCES == [
             "python:tests.settings"
         ], "Sources not restored"
+
+    def test_getitem(self, target: pyapp.conf.Settings):
+        actual = target["UPPER_VALUE"]
+
+        assert actual == "foo"
+
+
+class TestExportRestoreSettings:
+    def test_roundtrip_default_serialiser(self, monkeypatch):
+        file = BytesIO()
+
+        source_settings = pyapp.conf.Settings()
+        source_settings.__dict__["FOO"] = "foo"
+        source_settings.__dict__["BAR"] = "bar"
+        source_settings.SETTINGS_SOURCES.append("self")
+        with patch("pyapp.conf.settings", source_settings):
+            pyapp.conf.export_settings(file)
+
+            assert len(file.getvalue()) > 0
+
+        file.seek(0)
+
+        target_settings = pyapp.conf.Settings()
+        with patch("pyapp.conf.settings", target_settings):
+            pyapp.conf.restore_settings(file)
+
+            assert target_settings.FOO == source_settings.FOO
+            assert target_settings.BAR == source_settings.BAR
+            assert target_settings.SETTINGS_SOURCES == source_settings.SETTINGS_SOURCES
+
+    def test_roundtrip_json_serialiser(self, monkeypatch):
+        file = StringIO()
+
+        source_settings = pyapp.conf.Settings()
+        source_settings.__dict__["FOO"] = "foo"
+        source_settings.__dict__["BAR"] = "bar"
+        source_settings.SETTINGS_SOURCES.append("self")
+        with patch("pyapp.conf.settings", source_settings):
+            pyapp.conf.export_settings(file, serialiser=json)
+
+            assert len(file.getvalue()) > 0
+
+        file.seek(0)
+
+        target_settings = pyapp.conf.Settings()
+        with patch("pyapp.conf.settings", target_settings):
+            pyapp.conf.restore_settings(file, serialiser=json)
+
+            assert target_settings.FOO == source_settings.FOO
+            assert target_settings.BAR == source_settings.BAR
+            assert target_settings.SETTINGS_SOURCES == source_settings.SETTINGS_SOURCES
```

### Comparing `pyapp-4.8.2/tests/extensions/test_registry.py` & `pyapp-4.9.0/tests/extensions/test_registry.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/extensions/test_report.py` & `pyapp-4.9.0/tests/extensions/test_report.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/mock.py` & `pyapp-4.9.0/tests/mock.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/sample_app/__main__.py` & `pyapp-4.9.0/tests/sample_app/__main__.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/settings.py` & `pyapp-4.9.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/test_events.py` & `pyapp-4.9.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/test_feature_flags.py` & `pyapp-4.9.0/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/test_injection.py` & `pyapp-4.9.0/tests/test_injection.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/test_versioning.py` & `pyapp-4.9.0/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/utils/test_.py` & `pyapp-4.9.0/tests/utils/test_.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/utils/test_compatibility.py` & `pyapp-4.9.0/tests/utils/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/tests/utils/test_inspect.py` & `pyapp-4.9.0/tests/utils/test_inspect.py`

 * *Files identical despite different names*

### Comparing `pyapp-4.8.2/setup.py` & `pyapp-4.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
 ['argcomplete', 'colorama', 'yarl']
 
 extras_require = \
 {'toml': ['toml'], 'yaml': ['pyyaml']}
 
 setup_kwargs = {
     'name': 'pyapp',
-    'version': '4.8.2',
+    'version': '4.9.0',
     'description': 'A Python application framework - Let us handle the boring stuff!',
     'long_description': '######################################\npyApp - A python application framework\n######################################\n\n*Let us handle the boring stuff!*\n\n+---------+------------------------------------------------------------------------------------------------------------+\n| Docs    | .. image:: https://readthedocs.org/projects/pyapp/badge/?version=latest                                    |\n|         |    :target: https://docs.pyapp.info/                                                                       |\n|         |    :alt: ReadTheDocs                                                                                       |\n+---------+------------------------------------------------------------------------------------------------------------+\n| Build   | .. image:: https://api.dependabot.com/badges/status?host=github&repo=pyapp-org/pyapp                       |\n|         |    :target: https://dependabot.com                                                                         |\n|         |    :alt: Dependabot Status                                                                                 |\n+---------+------------------------------------------------------------------------------------------------------------+\n| Quality | .. image:: https://sonarcloud.io/api/project_badges/measure?project=pyapp-org_pyapp&metric=sqale_rating    |\n|         |    :target: https://sonarcloud.io/dashboard?id=pyapp-org_pyapp                                             |\n|         |    :alt: Maintainability                                                                                   |\n|         | .. image:: https://sonarcloud.io/api/project_badges/measure?project=pyapp-org_pyapp&metric=security_rating |\n|         |    :target: https://sonarcloud.io/project/security_hotspots                                                |\n|         |    :alt: Security                                                                                          |\n|         | .. image:: https://sonarcloud.io/api/project_badges/measure?project=pyapp-org_pyapp&metric=coverage        |\n|         |    :target: https://sonarcloud.io/code?id=pyapp-org_pyapp                                                  |\n|         |    :alt: Test Coverage                                                                                     |\n|         | .. image:: https://img.shields.io/badge/code%20style-black-000000.svg                                      |\n|         |    :target: https://github.com/ambv/black                                                                  |\n|         |    :alt: Once you go Black...                                                                              |\n+---------+------------------------------------------------------------------------------------------------------------+\n| Package | .. image:: https://img.shields.io/pypi/v/pyapp                                                             |\n|         |    :target: https://pypi.io/pypi/pyapp/                                                                    |\n|         |    :alt: Latest Version                                                                                    |\n|         | .. image:: https://img.shields.io/pypi/pyversions/pyapp                                                    |\n|         |    :target: https://pypi.io/pypi/pyapp/                                                                    |\n|         | .. image:: https://img.shields.io/pypi/l/pyapp                                                             |\n|         |    :target: https://pypi.io/pypi/pyapp/                                                                    |\n|         | .. image:: https://img.shields.io/pypi/wheel/pyapp                                                         |\n|         |    :alt: PyPI - Wheel                                                                                      |\n|         |    :target: https://pypi.io/pypi/pyapp/                                                                    |\n+---------+------------------------------------------------------------------------------------------------------------+\n\npyApp takes care of the boring boilerplate code for building a CLI, managing\nsettings and much more so you can focus on your application logic.\n\nSo what does pyApp handle?\n==========================\n\n- **Configuration** - Loading, merging your settings from different sources\n\n  + Python modules\n  + File and HTTP(S) endpoints for JSON and YAML files.\n\n- **Instance Factories** - Configuration of plugins, database connections, or just\n  implementations of an ``ABC``.\n  Leveraging settings to make setup of your application easy and reduce coupling.\n\n- **Dependency Injection** - Easy to use dependency injection without complicated setup.\n\n- **Checks** - A framework for checking settings are correct and environment is\n  operating correctly (your ops team will love you)?\n\n- **Extensions** - Extend the basic framework with extensions. Provides deterministic\n  startup, extension of the CLI and the ability to register checks and extension\n  specific default settings.\n\n- **Application** - Provides a extensible and simple CLI interface for running\n  commands (including async), comes with built-in commands to execute check, setting\n  and extension reports.\n\n- **Logging** - Initialise and apply sane logging defaults.\n\n- Highly tested and ready for production use.\n\n\nExtensions\n==========\n\n- 🔌 SQLAlchemy - `pyapp.sqlalchemy`_\n- 🔌 Redis - `pyapp.redis`_\n\nIn Beta\n-------\n\n- 🐛 Rollbar - `pyapp.rollbar`_\n\n- 📧 AIO SMTPlib - `pyapp.aiosmtplib`_ Extension for aiosmtplib\n\n- ☁ Boto3 - `pyapp.boto3`_\n\n- ☁ AIOBotocore - `pyapp.aiobotocore`_\n\n- 📨 Messaging - `pyapp.messaging`_ - Extension to provide abstract interfaces for Message Queues.\n\n  - 📨 AWS Messaging - `pyapp.messaging-aws`_ - Messaging extension for AWS (SQS/SNS)\n\nIn development\n--------------\n\n- 📧 SMTP - `pyapp.SMTP`_\n\n- 📨 Aio-Pika - `pyapp.aiopika`_ - Messaging extension for pika (RabbitMQ/AMQP)\n\n- 🔌 PySpark - `pyapp.pyspark`_ - Extension for PySpark\n\n- 🔎 Elastic Search - `pyapp.elasticsearch`_ - Extension for Elasticsearch\n\nComing soon\n-----------\n\n- 📨 AMQP Messaging - Messaging extension for AMQP (RabbitMQ)\n\n\n.. _pyapp.sqlalchemy: https://www.github.com/pyapp-org/pyapp.sqlalchemy\n.. _pyapp.redis: https://www.github.com/pyapp-org/pyapp.redis\n.. _pyapp.aiobotocore: https://www.github.com/pyapp-org/pyapp.aiobotocore\n.. _pyapp.SMTP: https://www.github.com/pyapp-org/pyapp.SMTP\n.. _pyapp.boto3: https://www.github.com/pyapp-org/pyapp.boto3\n.. _pyapp.rollbar: https://www.github.com/pyapp-org/pyapp.rollbar\n.. _pyapp.aiosmtplib: https://www.github.com/pyapp-org/pyapp.aiosmtplib\n.. _pyapp.messaging: https://www.github.com/pyapp-org/pyapp-messaging\n.. _pyapp.messaging-aws: https://www.github.com/pyapp-org/pyapp-messaging-aws\n.. _pyapp.aiopika: https://www.github.com/pyapp-org/pyapp.aiopika\n.. _pyapp.pyspark: https://www.github.com/pyapp-org/pyapp.pyspark\n.. _pyapp.elasticsearch: https://www.github.com/pyapp-org/pyapp.elasticsearch\n\n\nContributions\n=============\n\nContributions are most welcome, be it in the form of a extension and factories\nfor your favourite service client of bug reports, feature enhancements.\n\nThe core of pyApp is intended to remain simple and only provide required features\nwith extensions providing optional more specific functionality.\n\n',
     'author': 'Tim Savage',
     'author_email': 'tim@savage.company',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/pyapp-org/pyapp',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pyapp-4.8.2/PKG-INFO` & `pyapp-4.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pyapp
-Version: 4.8.2
+Version: 4.9.0
 Summary: A Python application framework - Let us handle the boring stuff!
 Home-page: https://github.com/pyapp-org/pyapp
 License: BSD-3-Clause
 Keywords: framework,application
 Author: Tim Savage
 Author-email: tim@savage.company
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: toml
```

