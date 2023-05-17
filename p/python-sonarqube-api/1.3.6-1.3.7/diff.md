# Comparing `tmp/python-sonarqube-api-1.3.6.tar.gz` & `tmp/python-sonarqube-api-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sonarqube-api-1.3.6.tar", last modified: Tue Dec 27 08:06:29 2022, max compression
+gzip compressed data, was "python-sonarqube-api-1.3.7.tar", last modified: Wed May 17 06:54:34 2023, max compression
```

## Comparing `python-sonarqube-api-1.3.6.tar` & `python-sonarqube-api-1.3.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-27 08:06:29.012265 python-sonarqube-api-1.3.6/
--rw-r--r--   0 shijialiang   (501) staff       (20)     1069 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/LICENSE
--rw-r--r--   0 shijialiang   (501) staff       (20)       33 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/MANIFEST.in
--rw-r--r--   0 shijialiang   (501) staff       (20)     4928 2022-12-27 08:06:29.011745 python-sonarqube-api-1.3.6/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     3810 2022-11-27 10:32:42.000000 python-sonarqube-api-1.3.6/README.rst
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-27 08:06:28.915853 python-sonarqube-api-1.3.6/python_sonarqube_api.egg-info/
--rw-r--r--   0 shijialiang   (501) staff       (20)     4928 2022-12-27 08:06:28.000000 python-sonarqube-api-1.3.6/python_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     2330 2022-12-27 08:06:28.000000 python-sonarqube-api-1.3.6/python_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        1 2022-12-27 08:06:28.000000 python-sonarqube-api-1.3.6/python_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2022-12-27 08:06:28.000000 python-sonarqube-api-1.3.6/python_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       10 2022-12-27 08:06:28.000000 python-sonarqube-api-1.3.6/python_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/requirements.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       38 2022-12-27 08:06:29.012317 python-sonarqube-api-1.3.6/setup.cfg
--rw-r--r--   0 shijialiang   (501) staff       (20)     2213 2022-12-27 07:56:32.000000 python-sonarqube-api-1.3.6/setup.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-27 08:06:28.917192 python-sonarqube-api-1.3.6/sonarqube/
--rw-r--r--   0 shijialiang   (501) staff       (20)      218 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/__init__.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-27 08:06:28.934280 python-sonarqube-api-1.3.6/sonarqube/cloud/
--rw-r--r--   0 shijialiang   (501) staff       (20)     7413 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      536 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/auth.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1639 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/ce.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1289 2022-12-27 07:56:32.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/components.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     7513 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/issues.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    10994 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/permissions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1553 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/project_badges.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3369 2022-12-27 07:56:32.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     6722 2022-12-27 07:56:32.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/qualitygates.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     7311 2022-12-27 07:56:32.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/qualityprofiles.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     9982 2022-12-27 07:56:32.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/rules.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3010 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3657 2022-12-27 07:56:32.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/user_groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1836 2022-12-27 07:56:32.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/users.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1548 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/cloud/webhooks.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-27 08:06:28.997445 python-sonarqube-api-1.3.6/sonarqube/community/
--rw-r--r--   0 shijialiang   (501) staff       (20)    11056 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4082 2022-08-11 14:17:02.000000 python-sonarqube-api-1.3.6/sonarqube/community/alm_integrations.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    12395 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/alm_settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1089 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/auth.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3529 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/ce.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3908 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/components.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      814 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/duplications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1504 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/favorites.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2614 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/hotspots.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    13593 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/issues.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      723 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/languages.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5441 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/measures.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      947 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/metrics.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      890 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/monitoring.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2593 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/new_code_periods.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2503 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/notifications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    14234 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/permissions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4195 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/plugins.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4319 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/project_analyses.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2677 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/project_badges.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2031 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/project_branches.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1064 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/project_dump.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1314 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/project_links.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1097 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/project_pull_requests.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1066 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/project_tags.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     6476 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     9227 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/qualitygates.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    11215 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/qualityprofiles.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    11342 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/rules.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      623 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/server.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2216 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/settings.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2262 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/sources.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5528 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/system.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4279 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/user_groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/user_tokens.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5841 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/users.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3378 2022-12-27 07:46:25.000000 python-sonarqube-api-1.3.6/sonarqube/community/webhooks.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1258 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/community/webservices.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-27 08:06:29.006215 python-sonarqube-api-1.3.6/sonarqube/enterprise/
--rw-r--r--   0 shijialiang   (501) staff       (20)      954 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/enterprise/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4860 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/enterprise/applications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      981 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/enterprise/audit_logs.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      666 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/enterprise/editions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    12235 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/enterprise/views.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-27 08:06:29.011044 python-sonarqube-api-1.3.6/sonarqube/utils/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/utils/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5192 2022-10-01 05:24:19.000000 python-sonarqube-api-1.3.6/sonarqube/utils/common.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    17562 2022-10-01 05:54:29.000000 python-sonarqube-api-1.3.6/sonarqube/utils/config.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      401 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/utils/exceptions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.6/sonarqube/utils/rest_client.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.975991 python-sonarqube-api-1.3.7/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1069 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/LICENSE
+-rw-r--r--   0 shijialiang   (501) staff       (20)       33 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/MANIFEST.in
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5057 2023-05-17 06:54:34.975767 python-sonarqube-api-1.3.7/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3939 2023-05-17 05:23:41.000000 python-sonarqube-api-1.3.7/README.rst
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.929038 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5057 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2330 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/requires.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-05-17 06:54:34.000000 python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/requirements.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-05-17 06:54:34.976033 python-sonarqube-api-1.3.7/setup.cfg
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2496 2023-05-17 06:51:30.000000 python-sonarqube-api-1.3.7/setup.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.931913 python-sonarqube-api-1.3.7/sonarqube/
+-rw-r--r--   0 shijialiang   (501) staff       (20)      240 2023-05-17 06:36:16.000000 python-sonarqube-api-1.3.7/sonarqube/__init__.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.946527 python-sonarqube-api-1.3.7/sonarqube/cloud/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     7413 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      536 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/auth.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1639 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/ce.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1289 2022-12-27 07:15:12.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/components.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     7513 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/issues.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    10994 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/permissions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1553 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/project_badges.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3369 2022-12-27 07:08:47.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/projects.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6722 2022-12-27 07:17:05.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/qualitygates.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     7311 2022-12-27 07:12:06.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/qualityprofiles.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     9982 2022-12-27 07:14:27.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/rules.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3010 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/settings.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3657 2022-12-27 07:13:24.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/user_groups.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1870 2023-05-17 06:00:39.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/users.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1548 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/cloud/webhooks.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.970188 python-sonarqube-api-1.3.7/sonarqube/community/
+-rw-r--r--   0 shijialiang   (501) staff       (20)    11056 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4082 2022-08-11 14:17:02.000000 python-sonarqube-api-1.3.7/sonarqube/community/alm_integrations.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    12791 2023-05-17 06:06:55.000000 python-sonarqube-api-1.3.7/sonarqube/community/alm_settings.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1089 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/auth.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3529 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/ce.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3908 2022-12-27 06:30:07.000000 python-sonarqube-api-1.3.7/sonarqube/community/components.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      814 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/duplications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1504 2022-12-27 06:51:59.000000 python-sonarqube-api-1.3.7/sonarqube/community/favorites.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2614 2022-12-27 06:53:53.000000 python-sonarqube-api-1.3.7/sonarqube/community/hotspots.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    13630 2023-05-17 06:00:39.000000 python-sonarqube-api-1.3.7/sonarqube/community/issues.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      723 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/languages.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5441 2022-12-27 06:57:44.000000 python-sonarqube-api-1.3.7/sonarqube/community/measures.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      947 2022-12-27 06:33:08.000000 python-sonarqube-api-1.3.7/sonarqube/community/metrics.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      890 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/monitoring.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2593 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/new_code_periods.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2503 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/notifications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    14234 2022-12-27 06:43:16.000000 python-sonarqube-api-1.3.7/sonarqube/community/permissions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4195 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/plugins.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4319 2022-12-27 06:32:02.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_analyses.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2677 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_badges.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2031 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_branches.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1064 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_dump.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1314 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_links.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1097 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_pull_requests.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1066 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/project_tags.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6521 2023-05-17 06:03:35.000000 python-sonarqube-api-1.3.7/sonarqube/community/projects.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     9227 2022-12-27 07:04:18.000000 python-sonarqube-api-1.3.7/sonarqube/community/qualitygates.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    11215 2022-12-27 06:46:00.000000 python-sonarqube-api-1.3.7/sonarqube/community/qualityprofiles.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    11376 2023-05-17 06:01:22.000000 python-sonarqube-api-1.3.7/sonarqube/community/rules.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      623 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/server.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2216 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/settings.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2262 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/sources.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5528 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/system.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4316 2023-05-17 06:00:39.000000 python-sonarqube-api-1.3.7/sonarqube/community/user_groups.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/user_tokens.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     5874 2023-05-17 06:00:39.000000 python-sonarqube-api-1.3.7/sonarqube/community/users.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3378 2022-12-27 07:07:40.000000 python-sonarqube-api-1.3.7/sonarqube/community/webhooks.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1258 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/community/webservices.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.972945 python-sonarqube-api-1.3.7/sonarqube/enterprise/
+-rw-r--r--   0 shijialiang   (501) staff       (20)      954 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4860 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/applications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      981 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/audit_logs.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      666 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/editions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    12235 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/enterprise/views.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-17 06:54:34.975358 python-sonarqube-api-1.3.7/sonarqube/utils/
+-rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/utils/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-17 05:23:33.000000 python-sonarqube-api-1.3.7/sonarqube/utils/common.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)    17635 2023-05-17 06:06:28.000000 python-sonarqube-api-1.3.7/sonarqube/utils/config.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      401 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/utils/exceptions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2022-05-23 11:32:43.000000 python-sonarqube-api-1.3.7/sonarqube/utils/rest_client.py
```

### Comparing `python-sonarqube-api-1.3.6/LICENSE` & `python-sonarqube-api-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/PKG-INFO` & `python-sonarqube-api-1.3.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sonarqube-api
-Version: 1.3.6
+Version: 1.3.7
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api sonarqube sonar client wrapper sonarcloud
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,14 +28,16 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
     :target: https://pypi.python.org/pypi/python-sonarqube-api
 .. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
     :target: https://pypi.python.org/pypi/python-sonarqube-api
 .. image:: https://pepy.tech/badge/python-sonarqube-api
     :target: https://pepy.tech/project/python-sonarqube-api
+.. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
+    :target: https://pepy.tech/project/python-sonarqube-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
```

### Comparing `python-sonarqube-api-1.3.6/README.rst` & `python-sonarqube-api-1.3.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
     :target: https://pypi.python.org/pypi/python-sonarqube-api
 .. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
     :target: https://pypi.python.org/pypi/python-sonarqube-api
 .. image:: https://pepy.tech/badge/python-sonarqube-api
     :target: https://pepy.tech/project/python-sonarqube-api
+.. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
+    :target: https://pepy.tech/project/python-sonarqube-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
```

### Comparing `python-sonarqube-api-1.3.6/python_sonarqube_api.egg-info/PKG-INFO` & `python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sonarqube-api
-Version: 1.3.6
+Version: 1.3.7
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api sonarqube sonar client wrapper sonarcloud
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,14 +28,16 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
     :target: https://pypi.python.org/pypi/python-sonarqube-api
 .. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
     :target: https://pypi.python.org/pypi/python-sonarqube-api
 .. image:: https://pepy.tech/badge/python-sonarqube-api
     :target: https://pepy.tech/project/python-sonarqube-api
+.. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
+    :target: https://pepy.tech/project/python-sonarqube-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
```

### Comparing `python-sonarqube-api-1.3.6/python_sonarqube_api.egg-info/SOURCES.txt` & `python-sonarqube-api-1.3.7/python_sonarqube_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/setup.py` & `python-sonarqube-api-1.3.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,30 @@
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
+
+def get_version() -> str:
+    version = ""
+    with open("sonarqube/__init__.py", "r", encoding="utf-8") as f:
+        for line in f:
+            if line.startswith("__version__"):
+                version = eval(line.split("=")[-1])
+                break
+    return version
+
+
 setup(
     name='python-sonarqube-api',
 
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.3.6',
+    version=get_version(),
 
     description='Python wrapper for the SonarQube and SonarCloud API.',
     long_description=long_description,
     url='https://github.com/shijl0925/python-sonarqube-api',
     author='Jialiang Shi',
     author_email='kevin09254930sjl@gmail.com',
     license='MIT',
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/__init__.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/auth.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/auth.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/ce.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/ce.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/components.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/components.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/issues.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/issues.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/permissions.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/permissions.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/project_badges.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/project_badges.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/projects.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/projects.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/qualitygates.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/qualitygates.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/qualityprofiles.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/qualityprofiles.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/rules.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/rules.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/settings.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/settings.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/user_groups.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/user_groups.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/users.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,18 @@
         """
 
         :param kwargs:
         """
         super(SonarCloudUsers, self).__init__(**kwargs)
 
     def get(self, login):
-        result = list(self.search_users(q=login))
-        for user in result:
+        result = self.search_users(q=login)
+        users = result.get("users", [])
+
+        for user in users:
             if user["login"] == login:
                 return user
 
     @GET(API_USERS_SEARCH_ENDPOINT)
     def search_users(self, q=None, p=None, ps=None):
         """
         Get a list of active users.
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/cloud/webhooks.py` & `python-sonarqube-api-1.3.7/sonarqube/cloud/webhooks.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/__init__.py` & `python-sonarqube-api-1.3.7/sonarqube/community/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/alm_integrations.py` & `python-sonarqube-api-1.3.7/sonarqube/community/alm_integrations.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/alm_settings.py` & `python-sonarqube-api-1.3.7/sonarqube/community/alm_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from sonarqube.utils.common import GET, POST
 from sonarqube.utils.rest_client import RestClient
 
 from sonarqube.utils.config import (
     API_ALM_SETTINGS_VALIDATE,
+    API_ALM_SETTINGS_VALIDATE_BINDING,
     API_ALM_SETTINGS_UPDATE_GITLAB,
     API_ALM_SETTINGS_UPDATE_GITHUB,
     API_ALM_SETTINGS_UPDATE_BITBUCKET,
     API_ALM_SETTINGS_UPDATE_BITBUCKETCLOUD,
     API_ALM_SETTINGS_UPDATE_AZURE,
     API_ALM_SETTINGS_SET_GITLAB_BINDING,
     API_ALM_SETTINGS_SET_GITHUB_BINDING,
@@ -335,7 +336,19 @@
         since 8.6
         Validate an ALM Setting by checking connectivity and permissions
         Requires the 'Administer System' permission
 
         :param key: Unique key of the ALM settings
         :return:
         """
+
+    @GET(API_ALM_SETTINGS_VALIDATE_BINDING)
+    def validate_binding(self, project):
+        """
+        since 9.0
+        Validate a project binding setting by checking connectivity and permissions
+        Requires project 'Browse' permission
+
+        :param project: Project key
+        :raises ValidationError:
+        :return:
+        """
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/auth.py` & `python-sonarqube-api-1.3.7/sonarqube/community/auth.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/ce.py` & `python-sonarqube-api-1.3.7/sonarqube/community/ce.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/components.py` & `python-sonarqube-api-1.3.7/sonarqube/community/components.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/duplications.py` & `python-sonarqube-api-1.3.7/sonarqube/community/duplications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/favorites.py` & `python-sonarqube-api-1.3.7/sonarqube/community/favorites.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/hotspots.py` & `python-sonarqube-api-1.3.7/sonarqube/community/hotspots.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/issues.py` & `python-sonarqube-api-1.3.7/sonarqube/community/issues.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,18 @@
         """
 
         :param kwargs:
         """
         super(SonarQubeIssues, self).__init__(**kwargs)
 
     def get(self, key):
-        result = list(self.search_issues(issues=key))
-        for issue in result:
+        result = self.search_issues(issues=key)
+        issues = result.get("issues", [])
+
+        for issue in issues:
             if issue["key"] == key:
                 return issue
 
     @GET(API_ISSUES_SEARCH_ENDPOINT)
     def search_issues(
         self,
         componentKeys=None,
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/languages.py` & `python-sonarqube-api-1.3.7/sonarqube/community/languages.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/measures.py` & `python-sonarqube-api-1.3.7/sonarqube/community/measures.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/metrics.py` & `python-sonarqube-api-1.3.7/sonarqube/community/metrics.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/monitoring.py` & `python-sonarqube-api-1.3.7/sonarqube/community/monitoring.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/new_code_periods.py` & `python-sonarqube-api-1.3.7/sonarqube/community/new_code_periods.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/notifications.py` & `python-sonarqube-api-1.3.7/sonarqube/community/notifications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/permissions.py` & `python-sonarqube-api-1.3.7/sonarqube/community/permissions.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/plugins.py` & `python-sonarqube-api-1.3.7/sonarqube/community/plugins.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/project_analyses.py` & `python-sonarqube-api-1.3.7/sonarqube/community/project_analyses.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/project_badges.py` & `python-sonarqube-api-1.3.7/sonarqube/community/project_badges.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/project_branches.py` & `python-sonarqube-api-1.3.7/sonarqube/community/project_branches.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/project_dump.py` & `python-sonarqube-api-1.3.7/sonarqube/community/project_dump.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/project_links.py` & `python-sonarqube-api-1.3.7/sonarqube/community/project_links.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/project_pull_requests.py` & `python-sonarqube-api-1.3.7/sonarqube/community/project_pull_requests.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/project_tags.py` & `python-sonarqube-api-1.3.7/sonarqube/community/project_tags.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/projects.py` & `python-sonarqube-api-1.3.7/sonarqube/community/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,18 @@
         """
 
         :param kwargs:
         """
         super(SonarQubeProjects, self).__init__(**kwargs)
 
     def get(self, key):
-        result = list(self.search_projects(projects=key))
-        for project in result:
+        result = self.search_projects(projects=key)
+        projects = result.get("components", [])
+
+        for project in projects:
             if project["key"] == key:
                 return project
 
     @GET(API_PROJECTS_SEARCH_ENDPOINT)
     def search_projects(
         self,
         analyzedBefore=None,
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/qualitygates.py` & `python-sonarqube-api-1.3.7/sonarqube/community/qualitygates.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/qualityprofiles.py` & `python-sonarqube-api-1.3.7/sonarqube/community/qualityprofiles.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/rules.py` & `python-sonarqube-api-1.3.7/sonarqube/community/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,18 @@
         """
 
         :param kwargs:
         """
         super(SonarQubeRules, self).__init__(**kwargs)
 
     def get(self, key):
-        result = list(self.search_rules(rule_key=key))
-        for rule in result:
+        result = self.search_rules(rule_key=key)
+        rules = result.get("rules", [])
+
+        for rule in rules:
             if rule["key"] == key:
                 return rule
 
     @GET(API_RULES_SEARCH_ENDPOINT)
     def search_rules(
         self,
         activation=None,
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/server.py` & `python-sonarqube-api-1.3.7/sonarqube/community/server.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/settings.py` & `python-sonarqube-api-1.3.7/sonarqube/community/settings.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/sources.py` & `python-sonarqube-api-1.3.7/sonarqube/community/sources.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/system.py` & `python-sonarqube-api-1.3.7/sonarqube/community/system.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/user_groups.py` & `python-sonarqube-api-1.3.7/sonarqube/community/user_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,18 @@
         """
 
         :param kwargs:
         """
         super(SonarQubeUserGroups, self).__init__(**kwargs)
 
     def get(self, name):
-        result = list(self.search_user_groups(q=name))
-        for group in result:
+        result = self.search_user_groups(q=name)
+        groups = result.get("groups", [])
+
+        for group in groups:
             if group["name"] == name:
                 return group
 
     @GET(API_USER_GROUPS_SEARCH_ENDPOINT)
     def search_user_groups(self, f=None, q=None, p=None, ps=None):
         """
         SINCE 5.2
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/user_tokens.py` & `python-sonarqube-api-1.3.7/sonarqube/community/user_tokens.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/users.py` & `python-sonarqube-api-1.3.7/sonarqube/community/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,21 @@
         """
 
         :param kwargs:
         """
         super(SonarQubeUsers, self).__init__(**kwargs)
 
     def get(self, login):
-        result = list(self.search_users(q=login))
-        for user in result:
+        result = self.search_users(q=login)
+        users = result.get("users", [])
+
+        for user in users:
             if user["login"] == login:
                 return user
 
-
     @POST(API_USERS_ANONYMIZE_ENDPOINT)
     def anonymize_deactivated_user(self, login):
         """
         SINCE 9.7
         Anonymize a deactivated user.
 
         :param login: User login
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/webhooks.py` & `python-sonarqube-api-1.3.7/sonarqube/community/webhooks.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/community/webservices.py` & `python-sonarqube-api-1.3.7/sonarqube/community/webservices.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/enterprise/__init__.py` & `python-sonarqube-api-1.3.7/sonarqube/enterprise/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/enterprise/applications.py` & `python-sonarqube-api-1.3.7/sonarqube/enterprise/applications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/enterprise/audit_logs.py` & `python-sonarqube-api-1.3.7/sonarqube/enterprise/audit_logs.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/enterprise/editions.py` & `python-sonarqube-api-1.3.7/sonarqube/enterprise/editions.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/enterprise/views.py` & `python-sonarqube-api-1.3.7/sonarqube/enterprise/views.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-1.3.6/sonarqube/utils/common.py` & `python-sonarqube-api-1.3.7/sonarqube/utils/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -143,68 +143,14 @@
                     return response.content
 
         return inner_func
 
     return wrapped_func
 
 
-def page_endpoint(url_pattern, item=None):
-    """
-
-    :param url_pattern:
-    :param item:
-    :return:
-    """
-
-    def wrapped_func(f):
-        @wraps(f)
-        def inner_func(self, *args, **kwargs):
-            """
-
-            :param self:
-            :param args:
-            :param kwargs:
-            :return:
-            """
-            func_params = translate_params(f, *args, **kwargs)
-            params = translate_special_params(func_params, self.special_attributes_map)
-
-            page_num = 1
-            page_size = 1
-            total = 2
-
-            flag = "p" in params.keys()
-
-            while page_num * page_size < total:
-                response = self._get(url_pattern, params=params).json()
-                if "paging" in response:
-                    page_num = response["paging"]["pageIndex"]
-                    page_size = response["paging"]["pageSize"]
-                    total = response["paging"]["total"]
-                else:
-                    page_num = response["p"]
-                    page_size = response["ps"]
-                    total = response["total"]
-
-                params["p"] = page_num + 1
-
-                for i in response[item]:
-                    yield i
-
-                if flag:
-                    break
-
-                if page_num >= self.MAX_SEARCH_NUM:
-                    break
-
-        return inner_func
-
-    return wrapped_func
-
-
 def GET(url_pattern):
     """
 
     :param url_pattern:
     :return:
     """
     return endpoint(url_pattern, method="GET")
@@ -213,17 +159,7 @@
 def POST(url_pattern):
     """
 
     :param url_pattern:
     :return:
     """
     return endpoint(url_pattern, method="POST")
-
-
-def PAGES_GET(url_pattern, item):
-    """
-
-    :param url_pattern:
-    :param item:
-    :return:
-    """
-    return page_endpoint(url_pattern, item=item)
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/utils/config.py` & `python-sonarqube-api-1.3.7/sonarqube/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,14 +263,15 @@
 API_ALM_INTEGRATION_SEARCH_BITBUCKETCLOUD_REPOS = "/api/alm_integrations/search_bitbucketcloud_repos"
 API_ALM_INTEGRATION_SEARCH_AZURE_REPOS = "/api/alm_integrations/search_azure_repos"
 API_ALM_INTEGRATION_LIST_BITBUCKETSERVER_PROJECTS = "/api/alm_integrations/list_bitbucketserver_projects"
 API_ALM_INTEGRATION_LIST_AZURE_PROJECTS = "/api/alm_integrations/list_azure_projects"
 API_ALM_INTEGRATION_IMPORT_GITLAB_PROJECT = "/api/alm_integrations/import_gitlab_project"
 
 API_ALM_SETTINGS_VALIDATE = "/api/alm_settings/validate"
+API_ALM_SETTINGS_VALIDATE_BINDING = "/api/alm_settings/validate_binding"
 API_ALM_SETTINGS_UPDATE_GITLAB = "/api/alm_settings/update_gitlab"
 API_ALM_SETTINGS_UPDATE_GITHUB = "/api/alm_settings/update_github"
 API_ALM_SETTINGS_UPDATE_BITBUCKET = "/api/alm_settings/update_bitbucket"
 API_ALM_SETTINGS_UPDATE_BITBUCKETCLOUD = "/api/alm_settings/update_bitbucketcloud"
 API_ALM_SETTINGS_UPDATE_AZURE = "/api/alm_settings/update_azure"
 API_ALM_SETTINGS_SET_GITLAB_BINDING = "/api/alm_settings/set_gitlab_binding"
 API_ALM_SETTINGS_SET_GITHUB_BINDING = "/api/alm_settings/set_github_binding"
```

### Comparing `python-sonarqube-api-1.3.6/sonarqube/utils/rest_client.py` & `python-sonarqube-api-1.3.7/sonarqube/utils/rest_client.py`

 * *Files identical despite different names*

