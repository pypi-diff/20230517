# Comparing `tmp/python-adjutantclient-0.9.0.tar.gz` & `tmp/python-adjutantclient-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-adjutantclient-0.9.0.tar", last modified: Fri Sep 17 16:38:13 2021, max compression
+gzip compressed data, was "python-adjutantclient-1.0.0.tar", last modified: Wed May 17 10:58:44 2023, max compression
```

## Comparing `python-adjutantclient-0.9.0.tar` & `python-adjutantclient-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.798098 python-adjutantclient-0.9.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2021-09-17 16:38:13.798098 python-adjutantclient-0.9.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.790098 python-adjutantclient-0.9.0/adjutantclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.790098 python-adjutantclient-0.9.0/adjutantclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17249 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4855 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4849 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/exc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.790098 python-adjutantclient-0.9.0/adjutantclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.794098 python-adjutantclient-0.9.0/adjutantclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5120 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/signup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5275 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8635 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/osc/v1/users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.794098 python-adjutantclient-0.9.0/adjutantclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.794098 python-adjutantclient-0.9.0/adjutantclient/tests/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/tests/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/tests/v1/test_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.794098 python-adjutantclient-0.9.0/adjutantclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3046 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/signup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1727 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3981 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/adjutantclient/v1/users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-17 16:38:13.798098 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-09-17 16:38:13.000000 python-adjutantclient-0.9.0/python_adjutantclient.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2858 2021-09-17 16:38:13.798098 python-adjutantclient-0.9.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2021-09-17 16:37:30.000000 python-adjutantclient-0.9.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.736973 python-adjutantclient-1.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2023-05-17 10:58:44.736973 python-adjutantclient-1.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.728973 python-adjutantclient-1.0.0/adjutantclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.728973 python-adjutantclient-1.0.0/adjutantclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17342 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4855 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4849 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/exc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.728973 python-adjutantclient-1.0.0/adjutantclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.732973 python-adjutantclient-1.0.0/adjutantclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/v1/notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5053 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/v1/signup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/v1/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5275 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/v1/tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/v1/tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8520 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/osc/v1/users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.732973 python-adjutantclient-1.0.0/adjutantclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.732973 python-adjutantclient-1.0.0/adjutantclient/tests/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/tests/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/tests/v1/test_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.732973 python-adjutantclient-1.0.0/adjutantclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1579 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1330 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/signup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3971 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/adjutantclient/v1/users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 10:58:44.736973 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2023-05-17 10:58:44.000000 python-adjutantclient-1.0.0/python_adjutantclient.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2023-05-17 10:58:44.736973 python-adjutantclient-1.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2023-05-17 10:58:16.000000 python-adjutantclient-1.0.0/tox.ini
```

### Comparing `python-adjutantclient-0.9.0/AUTHORS` & `python-adjutantclient-1.0.0/AUTHORS`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Adrian Turjak <adriant@catalyst.net.nz>
 Adrian Turjak <adriant@catalystcloud.nz>
 Amelia Cordwell <ameliacordwell@catalyst.net.nz>
 Anand Bhat <anandgvbhat@gmail.com>
 Andreas Jaeger <aj@suse.com>
 Arundhati Surpur <arundhati@nectechnologies.in>
 Dale Smith <dale@catalyst-eu.net>
+Dale Smith <dale@catalyst.net.nz>
+Dale Smith <dale@catalystcloud.nz>
 Doug Hellmann <doug@doughellmann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Hervé Beraud <hberaud@redhat.com>
+OpenStack Release Bot <infra-root@openstack.org>
 Sean McGinnis <sean.mcginnis@gmail.com>
 adrian-turjak <adriant@catalyst.net.nz>
 adriant <adriant@catalyst.net.nz>
 jiasirui <jiasirui@inspur.com>
 maaoyu <maaoyu@inspur.com>
 tonybrad <zhangyuan1@chinaunicom.cn>
+wangzihao <wangzihao@yovole.com>
```

### Comparing `python-adjutantclient-0.9.0/ChangeLog` & `python-adjutantclient-1.0.0/ChangeLog`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 CHANGES
 =======
 
-0.9.0
+1.0.0
 -----
 
+* Fix listing and removing roles from users
+* Fix typo in help text
+* Bugfix: Six removal introduced regression in v1/users
+* Add check-requirements to Zuul tests
+
+0.12.0
+------
+
+* Switch to 2023.1 Python3 unit tests and generic template name
+* Remove six
+
+0.11.0
+------
+
+* Update python testing for zed cycle testing runtime
+
+0.10.0
+------
+
 * Migrate from testr to stestr
 
 0.8.0
 -----
 
 * bump py37 to py38 in tox.ini
 * Add expected zuul jobs
```

### Comparing `python-adjutantclient-0.9.0/LICENSE` & `python-adjutantclient-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/PKG-INFO` & `python-adjutantclient-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-adjutantclient
-Version: 0.9.0
+Version: 1.0.0
 Summary: Adjutant API Client Library
 Home-page: https://github.com/openstack/python-adjutantclient
 Author: Adrian Turjak
 Author-email: adriant@catalyst.net.nz
 License: UNKNOWN
 Description: AdjutantClient is a command-line and python client for Adjutant.
         
@@ -57,11 +57,10 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
```

### Comparing `python-adjutantclient-0.9.0/README.rst` & `python-adjutantclient-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/__init__.py` & `python-adjutantclient-1.0.0/adjutantclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/_i18n.py` & `python-adjutantclient-1.0.0/adjutantclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/client.py` & `python-adjutantclient-1.0.0/adjutantclient/client.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/common/base.py` & `python-adjutantclient-1.0.0/adjutantclient/common/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,18 @@
 #    under the License.
 
 """
 Base utilities to build API operation managers and objects on top of.
 """
 import abc
 import copy
-import six
 
 from oslo_utils import reflection
 from oslo_utils import strutils
-from six.moves.urllib import parse
+from urllib import parse
 
 from adjutantclient._i18n import _
 from adjutantclient import exc as exceptions
 
 
 def getid(obj):
     """Return id if argument is a Resource.
@@ -195,24 +194,25 @@
         """
         body = self.client.patch(url, json=json).json()
         if response_key is not None:
             return self.resource_class(self, body[response_key])
         else:
             return self.resource_class(self, body)
 
-    def _delete(self, url):
+    def _delete(self, url, json=None):
         """Delete an object.
 
         :param url: a partial URL, e.g., '/servers/my-server'
+        :param json: data that will be encoded as JSON and sent with the
+            DELETE request.
         """
-        return self.client.delete(url)
+        return self.client.delete(url, json=json)
 
 
-@six.add_metaclass(abc.ABCMeta)
-class ManagerWithFind(BaseManager):
+class ManagerWithFind(BaseManager, metaclass=abc.ABCMeta):
     """Manager with additional `find()`/`findall()` methods."""
 
     @abc.abstractmethod
     def list(self):
         pass
 
     def find(self, **kwargs):
```

### Comparing `python-adjutantclient-0.9.0/adjutantclient/common/http.py` & `python-adjutantclient-1.0.0/adjutantclient/common/http.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/exc.py` & `python-adjutantclient-1.0.0/adjutantclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/osc/plugin.py` & `python-adjutantclient-1.0.0/adjutantclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/osc/v1/notifications.py` & `python-adjutantclient-1.0.0/adjutantclient/osc/v1/notifications.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/osc/v1/quota.py` & `python-adjutantclient-1.0.0/adjutantclient/osc/v1/quota.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import logging
-import six
 
 from osc_lib.command import command
 from osc_lib.i18n import _
 
 
 LOG = logging.getLogger(__name__)
 
@@ -57,17 +56,16 @@
             return headers, rows
         else:
             quota_data = client.quota.get(regions=parsed_args.region)
             headers = ['Service', 'Resource', 'Current Quota', 'Current Usage']
             region = quota_data['regions'][0]
 
             rows = []
-            for service, service_detail in six.iteritems(
-                    region['current_usage']):
-                for resource, value in six.iteritems(service_detail):
+            for service, service_detail in region['current_usage'].items():
+                for resource, value in service_detail.items():
                     current_quota = region['current_quota'][service].get(
                         resource)
                     rows.append([service, resource, current_quota, value])
             return headers, rows
 
 
 class QuotaSizes(command.Lister):
@@ -78,17 +76,17 @@
 
         quota_data = client.quota.get()
 
         headers = [
             'Size Name', 'Service', 'Resource', 'Value']
 
         rows = []
-        for size, size_details in six.iteritems(quota_data['quota_sizes']):
-            for service, service_details in six.iteritems(size_details):
-                for resource, value in six.iteritems(service_details):
+        for size, size_details in quota_data['quota_sizes'].items():
+            for service, service_details in size_details.items():
+                for resource, value in service_details.items():
                     rows.append([size, service, resource, value])
 
         return headers, rows
 
 
 class QuotaTasks(command.Lister):
     """Displays quota tasks."""
```

### Comparing `python-adjutantclient-0.9.0/adjutantclient/osc/v1/signup.py` & `python-adjutantclient-1.0.0/adjutantclient/osc/v1/signup.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/osc/v1/status.py` & `python-adjutantclient-1.0.0/adjutantclient/osc/v1/status.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/osc/v1/tasks.py` & `python-adjutantclient-1.0.0/adjutantclient/osc/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/osc/v1/tokens.py` & `python-adjutantclient-1.0.0/adjutantclient/osc/v1/tokens.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/osc/v1/users.py` & `python-adjutantclient-1.0.0/adjutantclient/osc/v1/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     def get_parser(self, prog_name):
         parser = super(UserRoleRemove, self).get_parser(prog_name)
 
         parser.add_argument(
             'user', metavar='<user>',
             help=_("The user's name or id.."))
         parser.add_argument(
-            'role', metavar='<user>',
+            'role', metavar='<role>',
             help=_("The role's name or id."))
         return parser
 
     def take_action(self, parsed_args):
         client = self.app.client_manager.admin_logic
         role = utils.find_resource(client.managed_roles, parsed_args.role)
         user = utils.find_resource(client.users, parsed_args.user)
@@ -167,18 +167,16 @@
             help=_("Name or ID of user."))
         return parser
 
     def take_action(self, parsed_args):
         client = self.app.client_manager.admin_logic
 
         user = utils.find_resource(client.users, parsed_args.user)
-        kwargs = {'user': user.id}
-        roles = [[role.id, role.name] for role
-                 in client.user_roles.list(**kwargs)]
-        return ['id', 'name'], roles
+
+        return ['name'], [[role] for role in user.roles]
 
 
 class ManageableRolesList(command.Lister):
     """Lists roles able to be managed by the current user """
     def take_action(self, parsed_args):
         client = self.app.client_manager.admin_logic
         roles = client.managed_roles.list()
```

### Comparing `python-adjutantclient-0.9.0/adjutantclient/tests/v1/test_client.py` & `python-adjutantclient-1.0.0/adjutantclient/tests/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/__init__.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/client.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/notifications.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/notifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from six.moves.urllib import parse
+from urllib import parse
 
 from adjutantclient.common import base
 
 
 class Notification(base.Resource):
     pass
```

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/quota.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/quota.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from six.moves.urllib import parse
+from urllib import parse
 
 from adjutantclient.common import base
 
 
 class QuotaManager(base.BaseManager):
 
     def get(self, regions=None):
```

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/roles.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/roles.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from six.moves.urllib import parse
+from urllib import parse
 
 from adjutantclient.common import base
 from adjutantclient import exc
 
 
 class Role(base.Resource):
     pass
@@ -83,25 +83,26 @@
             print(e.message)
             return False
 
         return True
 
     def remove(self, user_id, role=None, roles=None):
         """Remove a role or roles from a user"""
+
         if role:
             params = {
                 'roles': [role]
             }
         elif roles:
             params = {
                 'roles': roles
             }
 
         route = '/openstack/users/%s/roles'
         url = route % (user_id)
         try:
-            self._delete(url, json=params, response_key=None)
+            self._delete(url, json=params)
         except exc.HTTPBadRequest as e:
             print(e.message)
             return False
 
         return True
```

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/signup.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/signup.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/status.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/status.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/tasks.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-from six.moves.urllib import parse
+from urllib import parse
 
 from adjutantclient.common import base
 
 
 class Task(base.Resource):
     pass
```

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/tokens.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/tokens.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from adjutantclient.common import base
 
-from six.moves.urllib import parse
+from urllib import parse
 
 
 class Token(base.Resource):
     pass
 
 
 class TokenParam(base.Resource):
```

### Comparing `python-adjutantclient-0.9.0/adjutantclient/v1/users.py` & `python-adjutantclient-1.0.0/adjutantclient/v1/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 
-from six.moves.urllib import parse
+from urllib import parse
 
 from adjutantclient.common import base
 
 
 class User(base.Resource):
     def __repr__(self):
         return "<User %s>" % self._info
```

### Comparing `python-adjutantclient-0.9.0/python_adjutantclient.egg-info/PKG-INFO` & `python-adjutantclient-1.0.0/python_adjutantclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-adjutantclient
-Version: 0.9.0
+Version: 1.0.0
 Summary: Adjutant API Client Library
 Home-page: https://github.com/openstack/python-adjutantclient
 Author: Adrian Turjak
 Author-email: adriant@catalyst.net.nz
 License: UNKNOWN
 Description: AdjutantClient is a command-line and python client for Adjutant.
         
@@ -57,11 +57,10 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
```

### Comparing `python-adjutantclient-0.9.0/python_adjutantclient.egg-info/SOURCES.txt` & `python-adjutantclient-1.0.0/python_adjutantclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/python_adjutantclient.egg-info/entry_points.txt` & `python-adjutantclient-1.0.0/python_adjutantclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/requirements.txt` & `python-adjutantclient-1.0.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 
 pbr>=3.0.0 # Apache-2.0
 cliff>=2.6.0 # Apache-2.0
 iso8601>=0.1.11 # MIT
-osc-lib>=1.5.1 # Apache-2.0
-PrettyTable<0.8,>=0.7.1 # BSD
+osc-lib>=1.8.0 # Apache-2.0
+PrettyTable>=0.7.1 # BSD
 python-openstackclient>=3.11.0
 oslo.i18n>=2.1.0 # Apache-2.0
 oslo.serialization>=1.10.0 # Apache-2.0
 oslo.utils>=3.20.0 # Apache-2.0
 keystoneauth1>=2.20.0 # Apache-2.0
 PyYAML>=3.10.0 # MIT
-requests!=2.12.2,!=2.13.0,>=2.10.0 # Apache-2.0
-six>=1.9.0 # MIT
+requests>=2.14.2 # Apache-2.0
```

### Comparing `python-adjutantclient-0.9.0/setup.cfg` & `python-adjutantclient-1.0.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 name = python-adjutantclient
 summary = Adjutant API Client Library
 description-file = 
 	README.rst
 author = Adrian Turjak
 author-email = adriant@catalyst.net.nz
 home-page = https://github.com/openstack/python-adjutantclient
-python-requires = >=3.6
+python-requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 
 [files]
 packages = 
 	adjutantclient
 
 [entry_points]
 openstack.cli.extension =
```

### Comparing `python-adjutantclient-0.9.0/setup.py` & `python-adjutantclient-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-adjutantclient-0.9.0/tox.ini` & `python-adjutantclient-1.0.0/tox.ini`

 * *Files identical despite different names*

