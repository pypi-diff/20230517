# Comparing `tmp/django-axes-6.0.0b5.tar.gz` & `tmp/django-axes-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-6.0.0b5.tar", last modified: Sun May 14 21:43:55 2023, max compression
+gzip compressed data, was "django-axes-6.0.1.tar", last modified: Wed May 17 17:48:01 2023, max compression
```

## Comparing `django-axes-6.0.0b5.tar` & `django-axes-6.0.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.749219 django-axes-6.0.0b5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.737218 django-axes-6.0.0b5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.737218 django-axes-6.0.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    32155 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36421 2023-05-14 21:43:55.749219 django-axes-6.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.737218 django-axes-6.0.0b5/axes/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset_failure_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0008_accessfailurelog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.745219 django-axes-6.0.0b5/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36421 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.745219 django-axes-6.0.0b5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/9_contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.745219 django-axes-6.0.0b5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 21:43:55.749219 django-axes-6.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.749219 django-axes-6.0.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/urls_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.770362 django-axes-6.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 17:47:48.000000 django-axes-6.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-17 17:47:48.000000 django-axes-6.0.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-17 17:47:48.000000 django-axes-6.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-17 17:47:48.000000 django-axes-6.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-17 17:47:48.000000 django-axes-6.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 17:47:48.000000 django-axes-6.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-17 17:47:48.000000 django-axes-6.0.1/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    32218 2023-05-17 17:47:48.000000 django-axes-6.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-17 17:47:48.000000 django-axes-6.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-17 17:47:48.000000 django-axes-6.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-17 17:47:48.000000 django-axes-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-05-17 17:48:01.770362 django-axes-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-17 17:47:48.000000 django-axes-6.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-17 17:47:48.000000 django-axes-6.0.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.770362 django-axes-6.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/9_contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.770362 django-axes-6.0.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 17:47:48.000000 django-axes-6.0.1/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 17:47:48.000000 django-axes-6.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-17 17:47:48.000000 django-axes-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 17:47:48.000000 django-axes-6.0.1/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 17:47:48.000000 django-axes-6.0.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 17:47:48.000000 django-axes-6.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:48:01.770362 django-axes-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-17 17:47:48.000000 django-axes-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.770362 django-axes-6.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/urls_empty.py
```

### Comparing `django-axes-6.0.0b5/.github/workflows/codeql.yml` & `django-axes-6.0.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/.github/workflows/release.yml` & `django-axes-6.0.1/.github/workflows/release.yml`

 * *Files 12% similar despite different names*

```diff
@@ -32,12 +32,12 @@
         run: |
           python setup.py --version
           python setup.py sdist --format=gztar bdist_wheel
           twine check dist/*
 
       - name: Upload packages to Jazzband
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: jazzband
           password: ${{ secrets.JAZZBAND_RELEASE_KEY }}
           repository_url: https://jazzband.co/projects/django-axes/upload
```

### Comparing `django-axes-6.0.0b5/.github/workflows/test.yml` & `django-axes-6.0.1/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       max-parallel: 5
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
         django-version: ['3.2', '4.1', '4.2']
         include:
           # Tox configuration for QA environment
           - python-version: '3.11'
             django-version: 'qa'
           # Django main
           - python-version: '3.11'
@@ -30,21 +30,14 @@
           - python-version: 'pypy-3.8'
             django-version: '4.1'
             experimental: true
           - python-version: 'pypy-3.8'
             django-version: '4.2'
             experimental: true
         exclude:
-          # Exclude Python 3.7 for Django 4.x and Django main
-          - python-version: '3.7'
-            django-version: '4.1'
-          - python-version: '3.7'
-            django-version: '4.2'
-          - python-version: '3.7'
-            django-version: 'main'
           # Exclude Python 3.11 for Django 3.2 and Django 4.0
           - python-version: '3.11'
             django-version: '3.2'
 
 
     steps:
     - uses: actions/checkout@v3
```

### Comparing `django-axes-6.0.0b5/CHANGES.rst` & `django-axes-6.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 
 Changes
 =======
 
 
-6.0.0b5 (2023-05-15)
---------------------
+6.0.1 (2023-05-17)
+------------------
 
-- Deprecate ``is_admin_site`` API call with misleading naming.
-  [hirotasoshu]
+- Fine-tune CI pipelines and RTD build requirements.
+  [aleksihakli]
 
 
-6.0.0b4 (2023-05-13)
---------------------
+6.0.0 (2023-05-17)
+------------------
 
+Version 6 is a breaking release. Please see the documentation for upgrade instructions.
+
+- Deprecate Python 3.7 support.
+  [aleksihakli]
+- Deprecate ``is_admin_site`` API call with misleading naming.
+  [hirotasoshu]
 - Add ``AXES_LOCKOUT_PARAMETERS`` configuration flag that will supersede ``AXES_ONLY_USER_FAILURES``, ``AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP``, ``AXES_LOCK_OUT_BY_USER_OR_IP``, and ``AXES_USE_USER_AGENT`` configurations. Add deprecation warnings for old flags. See project documentation on RTD for update instructions.
   [hirotasoshu]
 - Improve translations.
   [hirotasoshu]
-
-
-6.0.0b3 (2023-05-01)
---------------------
-
 - Use Django ``cache.incr`` API for atomic cached failure counting
   [hirotasoshu, aleksihakli]
-
-
-6.0.0b2 (2023-04-28)
---------------------
-
 - Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
 - Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
    * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``,
    * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``,
    * ``AXES_PROXY_TRUSTED_IPS`` is now ``AXES_IPWARE_PROXY_TRUSTED_IPS``, and
    * ``AXES_META_PRECEDENCE_ORDER`` is now ``AXES_IPWARE_META_PRECEDENCE_ORDER``.
-
-
-6.0.0b1 (2023-04-25)
---------------------
-
 - Set 429 as the default lockout response code. [hirotasoshu]
 
 
 5.41.1 (2023-04-16)
 -------------------
 
 - Fix sensitive parameter logging for database handler. [stereodamage]
```

### Comparing `django-axes-6.0.0b5/CODE_OF_CONDUCT.md` & `django-axes-6.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/CONTRIBUTING.rst` & `django-axes-6.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/LICENSE` & `django-axes-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/PKG-INFO` & `django-axes-6.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.0b5
+Version: 6.0.1
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -21,15 +21,14 @@
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: Log Analysis
@@ -124,51 +123,42 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
-6.0.0b5 (2023-05-15)
---------------------
+6.0.1 (2023-05-17)
+------------------
 
-- Deprecate ``is_admin_site`` API call with misleading naming.
-  [hirotasoshu]
+- Fine-tune CI pipelines and RTD build requirements.
+  [aleksihakli]
 
 
-6.0.0b4 (2023-05-13)
---------------------
+6.0.0 (2023-05-17)
+------------------
 
+Version 6 is a breaking release. Please see the documentation for upgrade instructions.
+
+- Deprecate Python 3.7 support.
+  [aleksihakli]
+- Deprecate ``is_admin_site`` API call with misleading naming.
+  [hirotasoshu]
 - Add ``AXES_LOCKOUT_PARAMETERS`` configuration flag that will supersede ``AXES_ONLY_USER_FAILURES``, ``AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP``, ``AXES_LOCK_OUT_BY_USER_OR_IP``, and ``AXES_USE_USER_AGENT`` configurations. Add deprecation warnings for old flags. See project documentation on RTD for update instructions.
   [hirotasoshu]
 - Improve translations.
   [hirotasoshu]
-
-
-6.0.0b3 (2023-05-01)
---------------------
-
 - Use Django ``cache.incr`` API for atomic cached failure counting
   [hirotasoshu, aleksihakli]
-
-
-6.0.0b2 (2023-04-28)
---------------------
-
 - Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
 - Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
    * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``,
    * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``,
    * ``AXES_PROXY_TRUSTED_IPS`` is now ``AXES_IPWARE_PROXY_TRUSTED_IPS``, and
    * ``AXES_META_PRECEDENCE_ORDER`` is now ``AXES_IPWARE_META_PRECEDENCE_ORDER``.
-
-
-6.0.0b1 (2023-04-25)
---------------------
-
 - Set 429 as the default lockout response code. [hirotasoshu]
 
 
 5.41.1 (2023-04-16)
 -------------------
 
 - Fix sensitive parameter logging for database handler. [stereodamage]
```

### Comparing `django-axes-6.0.0b5/README.rst` & `django-axes-6.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/admin.py` & `django-axes-6.0.1/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/apps.py` & `django-axes-6.0.1/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/attempts.py` & `django-axes-6.0.1/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/backends.py` & `django-axes-6.0.1/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/checks.py` & `django-axes-6.0.1/axes/checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/conf.py` & `django-axes-6.0.1/axes/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/decorators.py` & `django-axes-6.0.1/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/handlers/base.py` & `django-axes-6.0.1/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/handlers/cache.py` & `django-axes-6.0.1/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/handlers/database.py` & `django-axes-6.0.1/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/handlers/dummy.py` & `django-axes-6.0.1/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/handlers/proxy.py` & `django-axes-6.0.1/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/handlers/test.py` & `django-axes-6.0.1/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/helpers.py` & `django-axes-6.0.1/axes/helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/django.mo` & `django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/django.po` & `django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.0.1/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.0.1/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/management/commands/axes_reset_failure_logs.py` & `django-axes-6.0.1/axes/management/commands/axes_reset_failure_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/management/commands/axes_reset_ip.py` & `django-axes-6.0.1/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/management/commands/axes_reset_logs.py` & `django-axes-6.0.1/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/management/commands/axes_reset_username.py` & `django-axes-6.0.1/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/middleware.py` & `django-axes-6.0.1/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/migrations/0001_initial.py` & `django-axes-6.0.1/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.0.1/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.0.1/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.0.1/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-6.0.1/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/migrations/0008_accessfailurelog.py` & `django-axes-6.0.1/axes/migrations/0008_accessfailurelog.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/models.py` & `django-axes-6.0.1/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/signals.py` & `django-axes-6.0.1/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/axes/utils.py` & `django-axes-6.0.1/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/django_axes.egg-info/PKG-INFO` & `django-axes-6.0.1/django_axes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.0b5
+Version: 6.0.1
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -21,15 +21,14 @@
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: Log Analysis
@@ -124,51 +123,42 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
-6.0.0b5 (2023-05-15)
---------------------
+6.0.1 (2023-05-17)
+------------------
 
-- Deprecate ``is_admin_site`` API call with misleading naming.
-  [hirotasoshu]
+- Fine-tune CI pipelines and RTD build requirements.
+  [aleksihakli]
 
 
-6.0.0b4 (2023-05-13)
---------------------
+6.0.0 (2023-05-17)
+------------------
 
+Version 6 is a breaking release. Please see the documentation for upgrade instructions.
+
+- Deprecate Python 3.7 support.
+  [aleksihakli]
+- Deprecate ``is_admin_site`` API call with misleading naming.
+  [hirotasoshu]
 - Add ``AXES_LOCKOUT_PARAMETERS`` configuration flag that will supersede ``AXES_ONLY_USER_FAILURES``, ``AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP``, ``AXES_LOCK_OUT_BY_USER_OR_IP``, and ``AXES_USE_USER_AGENT`` configurations. Add deprecation warnings for old flags. See project documentation on RTD for update instructions.
   [hirotasoshu]
 - Improve translations.
   [hirotasoshu]
-
-
-6.0.0b3 (2023-05-01)
---------------------
-
 - Use Django ``cache.incr`` API for atomic cached failure counting
   [hirotasoshu, aleksihakli]
-
-
-6.0.0b2 (2023-04-28)
---------------------
-
 - Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
 - Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
    * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``,
    * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``,
    * ``AXES_PROXY_TRUSTED_IPS`` is now ``AXES_IPWARE_PROXY_TRUSTED_IPS``, and
    * ``AXES_META_PRECEDENCE_ORDER`` is now ``AXES_IPWARE_META_PRECEDENCE_ORDER``.
-
-
-6.0.0b1 (2023-04-25)
---------------------
-
 - Set 429 as the default lockout response code. [hirotasoshu]
 
 
 5.41.1 (2023-04-16)
 -------------------
 
 - Fix sensitive parameter logging for database handler. [stereodamage]
```

### Comparing `django-axes-6.0.0b5/django_axes.egg-info/SOURCES.txt` & `django-axes-6.0.1/django_axes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/docs/1_requirements.rst` & `django-axes-6.0.1/docs/1_requirements.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _requirements:
 
 Requirements
 ============
 
-Axes requires a supported Django version and runs on Python versions 3.7 and above.
+Axes requires a supported Django version and runs on Python versions 3.8 and above.
 
 Refer to the project source code repository in
 `GitHub <https://github.com/jazzband/django-axes/>`_ and see the
 `pyproject.toml file <https://github.com/jazzband/django-axes/blob/master/pyproject.toml>`_ and
 `Python package definition <https://github.com/jazzband/django-axes/blob/master/setup.py>`_
 to check if your Django and Python version are supported.
```

### Comparing `django-axes-6.0.0b5/docs/3_usage.rst` & `django-axes-6.0.1/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/docs/4_configuration.rst` & `django-axes-6.0.1/docs/4_configuration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/docs/5_customization.rst` & `django-axes-6.0.1/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/docs/6_integration.rst` & `django-axes-6.0.1/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/docs/7_architecture.rst` & `django-axes-6.0.1/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/docs/Makefile` & `django-axes-6.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/docs/conf.py` & `django-axes-6.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/docs/images/flow.png` & `django-axes-6.0.1/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/pyproject.toml` & `django-axes-6.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 addopts = "--cov axes --cov-append --cov-branch --cov-report term-missing --cov-report=xml"
 DJANGO_SETTINGS_MODULE = "tests.settings"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{37,38,39,310,py38}-dj32
+    py{38,39,310,py38}-dj32
     py{38,39,310,311,py38}-dj41
     py{38,39,310,311,py38}-dj42
     py311-djmain
     py311-djqa
 
 [gh-actions]
 python =
-    3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
     pypy-3.8: pypy38
 
 [gh-actions:env]
```

### Comparing `django-axes-6.0.0b5/setup.py` & `django-axes-6.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet :: Log Analysis",
```

### Comparing `django-axes-6.0.0b5/tests/base.py` & `django-axes-6.0.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/settings.py` & `django-axes-6.0.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_admin.py` & `django-axes-6.0.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_attempts.py` & `django-axes-6.0.1/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_backends.py` & `django-axes-6.0.1/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_checks.py` & `django-axes-6.0.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_decorators.py` & `django-axes-6.0.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_failures.py` & `django-axes-6.0.1/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_handlers.py` & `django-axes-6.0.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_helpers.py` & `django-axes-6.0.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_logging.py` & `django-axes-6.0.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_login.py` & `django-axes-6.0.1/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_management.py` & `django-axes-6.0.1/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_middleware.py` & `django-axes-6.0.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b5/tests/test_models.py` & `django-axes-6.0.1/tests/test_models.py`

 * *Files identical despite different names*

