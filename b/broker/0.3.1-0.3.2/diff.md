# Comparing `tmp/broker-0.3.1.tar.gz` & `tmp/broker-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broker-0.3.1.tar", last modified: Mon May  1 19:33:11 2023, max compression
+gzip compressed data, was "broker-0.3.2.tar", last modified: Wed May 17 15:53:27 2023, max compression
```

## Comparing `broker-0.3.1.tar` & `broker-0.3.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.634777 broker-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.638778 broker-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 19:32:51.000000 broker-0.3.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-01 19:32:51.000000 broker-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-01 19:32:51.000000 broker-0.3.1/.github/workflows/update_broker_image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-01 19:32:51.000000 broker-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-01 19:32:51.000000 broker-0.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-01 19:32:51.000000 broker-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 19:32:51.000000 broker-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-01 19:33:11.646777 broker-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-01 19:32:51.000000 broker-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/broker/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 19:32:51.000000 broker-0.3.1/broker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/broker/binds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:32:51.000000 broker-0.3.1/broker/binds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-01 19:32:51.000000 broker-0.3.1/broker/binds/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-01 19:32:51.000000 broker-0.3.1/broker/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-01 19:32:51.000000 broker-0.3.1/broker/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-01 19:32:51.000000 broker-0.3.1/broker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-05-01 19:32:51.000000 broker-0.3.1/broker/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-01 19:32:51.000000 broker-0.3.1/broker/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-01 19:32:51.000000 broker-0.3.1/broker/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/broker/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-01 19:32:51.000000 broker-0.3.1/broker/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29309 2023-05-01 19:32:51.000000 broker-0.3.1/broker/providers/ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-05-01 19:32:52.000000 broker-0.3.1/broker/providers/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-01 19:32:52.000000 broker-0.3.1/broker/providers/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-01 19:32:52.000000 broker-0.3.1/broker/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-01 19:32:52.000000 broker-0.3.1/broker/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/broker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:32:59.000000 broker-0.3.1/broker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 19:33:11.000000 broker-0.3.1/broker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-01 19:32:52.000000 broker-0.3.1/broker_settings.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-01 19:32:52.000000 broker-0.3.1/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 19:32:52.000000 broker-0.3.1/logs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 19:32:52.000000 broker-0.3.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-01 19:33:11.650778 broker-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 19:32:52.000000 broker-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.642778 broker-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-01 19:32:52.000000 broker-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/ansible_tower/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/ansible_tower/fake_children.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/ansible_tower/fake_jobs.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/ansible_tower/fake_workflows.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/args_file.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/args_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/broker_args.json
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/broker_args.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.638778 broker-0.3.1/tests/data/cli_scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/cli_scenarios/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/cli_scenarios/satlab/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/checkout_rhel78.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/checkout_sat_69.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/cli_scenarios/satlab/execute_test_workflow.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/data/container/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/container/fake_containers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/container/fake_images.json
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-01 19:32:52.000000 broker-0.3.1/tests/data/fake_inventory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-01 19:32:52.000000 broker-0.3.1/tests/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-01 19:32:52.000000 broker-0.3.1/tests/functional/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-01 19:32:52.000000 broker-0.3.1/tests/functional/test_satlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:33:11.646777 broker-0.3.1/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-01 19:32:52.000000 broker-0.3.1/tests/providers/test_ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-01 19:32:52.000000 broker-0.3.1/tests/providers/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-01 19:32:52.000000 broker-0.3.1/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-01 19:32:52.000000 broker-0.3.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-01 19:32:52.000000 broker-0.3.1/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.159932 broker-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.163932 broker-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 15:53:11.000000 broker-0.3.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-17 15:53:11.000000 broker-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-17 15:53:11.000000 broker-0.3.2/.github/workflows/update_broker_image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-17 15:53:11.000000 broker-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-17 15:53:11.000000 broker-0.3.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-17 15:53:11.000000 broker-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 15:53:11.000000 broker-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-17 15:53:27.171933 broker-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-17 15:53:11.000000 broker-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/broker/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 15:53:11.000000 broker-0.3.2/broker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/broker/binds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:11.000000 broker-0.3.2/broker/binds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-17 15:53:11.000000 broker-0.3.2/broker/binds/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-17 15:53:11.000000 broker-0.3.2/broker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-17 15:53:11.000000 broker-0.3.2/broker/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 15:53:11.000000 broker-0.3.2/broker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-05-17 15:53:11.000000 broker-0.3.2/broker/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-17 15:53:11.000000 broker-0.3.2/broker/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-17 15:53:11.000000 broker-0.3.2/broker/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/broker/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-17 15:53:11.000000 broker-0.3.2/broker/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29309 2023-05-17 15:53:11.000000 broker-0.3.2/broker/providers/ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-05-17 15:53:11.000000 broker-0.3.2/broker/providers/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-17 15:53:11.000000 broker-0.3.2/broker/providers/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-17 15:53:11.000000 broker-0.3.2/broker/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-17 15:53:11.000000 broker-0.3.2/broker/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/broker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:53:17.000000 broker-0.3.2/broker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-17 15:53:11.000000 broker-0.3.2/broker_settings.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-17 15:53:11.000000 broker-0.3.2/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 15:53:11.000000 broker-0.3.2/logs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 15:53:11.000000 broker-0.3.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 15:53:27.171933 broker-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 15:53:11.000000 broker-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-17 15:53:11.000000 broker-0.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/data/ansible_tower/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/ansible_tower/fake_children.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/ansible_tower/fake_jobs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/ansible_tower/fake_workflows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/args_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/args_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/broker_args.json
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/broker_args.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.163932 broker-0.3.2/tests/data/cli_scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/data/cli_scenarios/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/data/cli_scenarios/satlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/checkout_rhel78.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/checkout_sat_69.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/execute_test_workflow.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/data/container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/container/fake_containers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/container/fake_images.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/fake_inventory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-17 15:53:11.000000 broker-0.3.2/tests/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-17 15:53:11.000000 broker-0.3.2/tests/functional/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-17 15:53:11.000000 broker-0.3.2/tests/functional/test_satlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-17 15:53:11.000000 broker-0.3.2/tests/providers/test_ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-17 15:53:11.000000 broker-0.3.2/tests/providers/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-17 15:53:11.000000 broker-0.3.2/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-17 15:53:11.000000 broker-0.3.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 15:53:11.000000 broker-0.3.2/tests/test_settings.py
```

### Comparing `broker-0.3.1/.github/workflows/codeql-analysis.yml` & `broker-0.3.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/.github/workflows/python-publish.yml` & `broker-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/.github/workflows/update_broker_image.yml` & `broker-0.3.2/.github/workflows/update_broker_image.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/.gitignore` & `broker-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/LICENSE` & `broker-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/PKG-INFO` & `broker-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broker
-Version: 0.3.1
+Version: 0.3.2
 Summary: The infrastructure middleman.
 Home-page: https://github.com/SatelliteQE/broker
 Author: Jacob J Callahan
 Author-email: jacob.callahan05@gmail.com
 License: GNU General Public License v3
 Keywords: broker,AnsibleTower
 Platform: UNKNOWN
```

### Comparing `broker-0.3.1/README.md` & `broker-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/binds/containers.py` & `broker-0.3.2/broker/binds/containers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/broker.py` & `broker-0.3.2/broker/broker.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/commands.py` & `broker-0.3.2/broker/commands.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/exceptions.py` & `broker-0.3.2/broker/exceptions.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/helpers.py` & `broker-0.3.2/broker/helpers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/hosts.py` & `broker-0.3.2/broker/hosts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-# from functools import cached_property
 from logzero import logger
 from broker.exceptions import NotImplementedError, HostError
 from broker.session import ContainerSession, Session
 from broker.settings import settings
 
 
 class Host:
-
     default_timeout = 0  # timeout in ms, 0 is infinite
 
-    def __init__(self, hostname=None, name=None, from_dict=False, **kwargs):
-        # Allow the class to construct itself from kwargs
-        if from_dict:
-            self.__dict__.update(kwargs)
-        else:
-            self.hostname = hostname or kwargs.get("ip", None)
-            if not self.hostname:
-                # check to see if we're being reconstructued, likely for checkin
-                import inspect
-                if any(f.function == "reconstruct_host" for f in inspect.stack()):
-                    logger.debug("Ignoring missing hostname and ip for checkin reconstruction.")
-                else:
-                    raise HostError("Host must be constructed with a hostname or ip")
-            self.name = name
-        self.username = kwargs.get("username", settings.HOST_USERNAME)
-        self.password = kwargs.get("password", settings.HOST_PASSWORD)
-        self.timeout = kwargs.get(
+    def __init__(self, **kwargs):
+        """Create a Host instance
+
+        Expected kwargs:
+          hostname: str - Hostname or IP address of the host, required
+          name: str - Name of the host
+          username: str - Username to use for SSH connection
+          password: str - Password to use for SSH connection
+          connection_timeout: int - Timeout for SSH connection
+          port: int - Port to use for SSH connection
+          key_filename: str - Path to SSH key file to use for SSH connection
+        """
+        logger.debug(f"Constructing host using {kwargs=}")
+        self.hostname = kwargs.get("hostname") or kwargs.get("ip")
+        if not self.hostname:
+            # check to see if we're being reconstructued, likely for checkin
+            import inspect
+            if any(f.function == "reconstruct_host" for f in inspect.stack()):
+                logger.debug("Ignoring missing hostname and ip for checkin reconstruction.")
+            else:
+                raise HostError("Host must be constructed with a hostname or ip")
+        self.name = kwargs.pop("name", None)
+        self.username = kwargs.pop("username", settings.HOST_USERNAME)
+        self.password = kwargs.pop("password", settings.HOST_PASSWORD)
+        self.timeout = kwargs.pop(
             "connection_timeout", settings.HOST_CONNECTION_TIMEOUT
         )
-        self.port = kwargs.get("port", settings.HOST_SSH_PORT)
-        self.key_filename = kwargs.get("key_filename", settings.HOST_SSH_KEY_FILENAME)
+        self.port = kwargs.pop("port", settings.HOST_SSH_PORT)
+        self.key_filename = kwargs.pop("key_filename", settings.HOST_SSH_KEY_FILENAME)
+        self.__dict__.update(kwargs) # Make every other kwarg an attribute
         self._session = None
 
     def __del__(self):
         """Try to close the connection on garbage collection of the host instance"""
         self.close()
         # object.__del__ DNE, so I don't have to call it here.
         # If host inherits from a different class with __del__, it should get called through super
@@ -64,14 +71,15 @@
         self.close()
         self._session = Session(
             hostname=_hostname,
             username=username,
             password=password,
             port=_port,
             key_filename=key_filename,
+            timeout=timeout
         )
 
     def close(self):
         # This attribute may be missing after pickling
         if isinstance(getattr(self, "_session", None), Session):
             self._session.session.disconnect()
         self._session = None
```

### Comparing `broker-0.3.1/broker/logger.py` & `broker-0.3.2/broker/logger.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/providers/__init__.py` & `broker-0.3.2/broker/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/providers/ansible_tower.py` & `broker-0.3.2/broker/providers/ansible_tower.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/providers/container.py` & `broker-0.3.2/broker/providers/container.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker/providers/test_provider.py` & `broker-0.3.2/broker/providers/test_provider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+from broker import helpers
 from dynaconf import Validator
 from broker.settings import settings
 from broker.providers import Provider
 
 
 HOST_PROPERTIES = {
     "basic": {
@@ -36,17 +37,20 @@
                 "_broker_provider": "TestProvider",
                 "_broker_provider_instance": self.instance,
                 "_broker_args": broker_args,
             }
         )
 
     def construct_host(self, provider_params, host_classes, **kwargs):
-        host_params = provider_params.copy()
-        host_params.update(kwargs)
-        host_inst = host_classes[host_params["host_type"]](**host_params)
+        if provider_params:
+            host_params = provider_params.copy()
+            host_params.update(kwargs)
+            host_inst = host_classes[host_params["host_type"]](**host_params)
+        else:  # if we are reconstructing the host from the inventory
+            host_inst = host_classes[kwargs.get("type", "host")](**kwargs)
         self._set_attributes(host_inst, broker_args=kwargs)
         return host_inst
 
     @Provider.register_action()
     def test_action(self, **kwargs):
         action = kwargs.get("test_action")
         if action == "release":
@@ -57,12 +61,14 @@
 
     def release(self, host_obj):
         return self.test_action(test_action="release", **host_obj.to_dict())
 
     def extend(self):
         pass
 
-    def get_inventory(self, **kwargs):
-        pass
+    def get_inventory(self, *args, **kwargs):
+        return helpers.load_inventory(
+            filter=f"_broker_provider={self.__class__.__name__}"
+        )
 
     def nick_help(self):
         pass
```

### Comparing `broker-0.3.1/broker/session.py` & `broker-0.3.2/broker/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import contextmanager
 import os
 import socket
 import tempfile
 from pathlib import Path
 from logzero import logger
 from ssh2.session import Session as ssh2_Session
 from ssh2 import sftp as ssh2_sftp
@@ -27,15 +28,16 @@
         """Wrapper around ssh2-python's auth/connection system"""
         host = kwargs.get("hostname", "localhost")
         user = kwargs.get("username", "root")
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.settimeout(kwargs.get("timeout"))
         port = kwargs.get("port", 22)
         key_filename = kwargs.get("key_filename")
-        helpers.simple_retry(sock.connect, [(host, port)])
+        timeout = kwargs.get("timeout", 60)
+        helpers.simple_retry(sock.connect, [(host, port)], max_timeout=timeout)
         self.session = ssh2_Session()
         self.session.handshake(sock)
         if key_filename:
             if not Path(key_filename).exists():
                 raise FileNotFoundError(f"Key not found in '{key_filename}'")
             self.session.userauth_publickey_fromfile(user, key_filename)
         elif kwargs.get("password"):
@@ -73,14 +75,31 @@
         return results
 
     def shell(self, pty=False):
         """Create and return an interactive shell instance"""
         channel = self.session.open_session()
         return InteractiveShell(channel, pty)
 
+    @contextmanager
+    def tail_file(self, filename):
+        """Simulate tailing a file on the remote host
+
+        example:
+            with my_host.session.tail_file("/var/log/messages") as res:
+                # do something that creates new messages
+            print(res.stdout)
+
+        returns a Result object with stdout, stderr, and status
+        """
+        initial_size = int(self.run(f"stat -c %s {filename}").stdout.strip())
+        yield (res := helpers.Result())
+        # get the contents of the file from the initial size to the end
+        result = self.run(f"tail -c +{initial_size} {filename}")
+        res.__dict__.update(result.__dict__)
+
     def sftp_read(self, source, destination=None, return_data=False):
         """read a remote file into a local destination or return a bytes object if return_data is True"""
         if not return_data:
             if not destination:
                 destination = source
             elif destination.endswith("/"):
                 destination = destination + Path(source).name
@@ -232,14 +251,23 @@
             result = helpers.Result.from_nonduplexed_exec(result)
         return result
 
     def disconnect(self):
         """Needed for simple compatability with Session"""
         pass
 
+    @contextmanager
+    def tail_file(self, filename):
+        """Simulate tailing a file on the remote host"""
+        initial_size = int(self.run(f"stat -c %s {filename}").stdout.strip())
+        yield (res := helpers.Result())
+        # get the contents of the file from the initial size to the end
+        result = self.run(f"tail -c +{initial_size} {filename}")
+        res.__dict__.update(result.__dict__)
+
     def sftp_write(self, source, destination=None, ensure_dir=True):
         """Add one of more files to the container"""
         # ensure source is a list of Path objects
         if not isinstance(source, list):
             source = [Path(source)]
         else:
             source = [Path(src) for src in source]
```

### Comparing `broker-0.3.1/broker/settings.py` & `broker-0.3.2/broker/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         f"Broker settings file not found at {settings_path.absolute()}.", fg="red"
     )
     init_settings(settings_path, interactive=interative_mode)
 
 validators = [
     Validator("HOST_USERNAME", default="root"),
     Validator("HOST_PASSWORD", default="toor"),
-    Validator("HOST_CONNECTION_TIMEOUT", default=None),
+    Validator("HOST_CONNECTION_TIMEOUT", default=60),
     Validator("HOST_SSH_PORT", default=22),
     Validator("HOST_SSH_KEY_FILENAME", default=None),
     Validator("LOGGING", is_type_of=dict),
     Validator(
         "LOGGING.CONSOLE_LEVEL",
         is_in=["error", "warning", "info", "debug", "trace", "silent"],
         default="info",
```

### Comparing `broker-0.3.1/broker.egg-info/PKG-INFO` & `broker-0.3.2/broker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broker
-Version: 0.3.1
+Version: 0.3.2
 Summary: The infrastructure middleman.
 Home-page: https://github.com/SatelliteQE/broker
 Author: Jacob J Callahan
 Author-email: jacob.callahan05@gmail.com
 License: GNU General Public License v3
 Keywords: broker,AnsibleTower
 Platform: UNKNOWN
```

### Comparing `broker-0.3.1/broker.egg-info/SOURCES.txt` & `broker-0.3.2/broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/broker_settings.yaml.example` & `broker-0.3.2/broker_settings.yaml.example`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/setup.cfg` & `broker-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/data/ansible_tower/fake_children.json` & `broker-0.3.2/tests/data/ansible_tower/fake_children.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/data/ansible_tower/fake_jobs.json` & `broker-0.3.2/tests/data/ansible_tower/fake_jobs.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/data/container/fake_containers.json` & `broker-0.3.2/tests/data/container/fake_containers.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/data/container/fake_images.json` & `broker-0.3.2/tests/data/container/fake_images.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/data/fake_inventory.yaml` & `broker-0.3.2/tests/data/fake_inventory.yaml`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/functional/README.md` & `broker-0.3.2/tests/functional/README.md`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/functional/test_containers.py` & `broker-0.3.2/tests/functional/test_containers.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,14 +85,21 @@
             assert (
                 loc_settings_path.read_bytes() == Path(tmp.file.name).read_bytes()
             ), "Local file is different from the received one"
             assert (
                 loc_settings_path.read_bytes() == data
             ), "Local file is different from the received one (return_data=True)"
             assert data == Path(tmp.file.name).read_bytes(), "Received files do not match"
+        # test the tail_file context manager
+        tailed_file = f"{remote_dir}/tail_me.txt"
+        c_host.execute(f"echo 'hello world' > {tailed_file}")
+        with c_host.session.tail_file(tailed_file) as tf:
+            c_host.execute(f"echo 'this is a new line' >> {tailed_file}")
+        assert 'this is a new line' in tf.stdout
+        assert 'hello world' not in tf.stdout
 
 
 def test_container_e2e_mp():
     with Broker(container_host="ubi8:latest", _count=7) as c_hosts:
         for c_host in c_hosts:
             assert c_host._cont_inst.top()['Processes']
             res = c_host.execute("hostname")
```

### Comparing `broker-0.3.1/tests/functional/test_satlab.py` & `broker-0.3.2/tests/functional/test_satlab.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,14 +82,21 @@
             assert (
                 loc_settings_path.read_bytes() == Path(tmp.file.name).read_bytes()
             ), "Local file is different from the received one"
             assert (
                 loc_settings_path.read_bytes() == data
             ), "Local file is different from the received one (return_data=True)"
             assert data == Path(tmp.file.name).read_bytes(), "Received files do not match"
+        # test the tail_file context manager
+        tailed_file = f"{remote_dir}/tail_me.txt"
+        r_host.execute(f"echo 'hello world' > {tailed_file}")
+        with r_host.session.tail_file(tailed_file) as tf:
+            r_host.execute(f"echo 'this is a new line' >> {tailed_file}")
+        assert 'this is a new line' in tf.stdout
+        assert 'hello world' not in tf.stdout
 
 
 def test_tower_host_mp():
     with Broker(workflow="deploy-base-rhel", _count=3) as r_hosts:
         for r_host in r_hosts:
             res = r_host.execute("hostname")
             assert res.stdout.strip() == r_host.hostname
```

### Comparing `broker-0.3.1/tests/providers/test_ansible_tower.py` & `broker-0.3.2/tests/providers/test_ansible_tower.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/providers/test_container.py` & `broker-0.3.2/tests/providers/test_container.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/test_broker.py` & `broker-0.3.2/tests/test_broker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from broker import broker
+from broker import broker, helpers
 from broker.providers import test_provider
 import pytest
 
 
 def test_empty_init():
     """Broker should be able to init without any arguments"""
     broker_inst = broker.Broker()
@@ -30,31 +30,53 @@
     assert not broker_inst._kwargs.get("nick")
     assert broker_inst._kwargs["test_action"] == "blank"
 
 
 def test_broker_e2e():
     """Run through the base functionality of broker"""
     broker_inst = broker.Broker(nick="test_nick")
-    broker_inst.checkout()
+    host_checkout = broker_inst.checkout()
     assert len(broker_inst._hosts) == 1
     broker_host = broker_inst._hosts[0]
     assert broker_host.hostname == "test.host.example.com"
+    assert broker_host == host_checkout
     broker_host_dict = broker_host.to_dict()
     assert broker_host_dict["_broker_provider"] == "TestProvider"
     broker_inst.checkin()
     assert len(broker_inst._hosts) == 0
 
 
 def test_broker_empty_checkin():
     """Try to checkin with no hosts on the instance"""
     broker_inst = broker.Broker(nick="test_nick")
     assert not broker_inst._hosts
     broker_inst.checkin()
 
 
+def test_broker_checkin_n_sync_empty_hostname():
+    """Test that broker can checkin and sync inventory with a host that has empty hostname"""
+    broker_inst = broker.Broker(nick="test_nick")
+    broker_inst.checkout()
+    inventory = helpers.load_inventory()
+    assert len(inventory) == 1
+    inventory[0]["hostname"] = None
+    # remove the host from the inventory
+    helpers.update_inventory(remove="test.host.example.com")
+    # add the host back with no hostname
+    helpers.update_inventory(add=inventory)
+    hosts = broker_inst.from_inventory()
+    assert len(hosts) == 1
+    assert hosts[0].hostname is None
+    broker_inst = broker.Broker(hosts=hosts)
+    broker_inst.checkin()
+    assert (
+        not broker_inst.from_inventory()
+    ), "Host was not removed from inventory after checkin"
+
+
 def test_mp_checkout():
     """Test that broker can checkout multiple hosts using multiprocessing"""
     VM_COUNT = 50  # This is intentionaly made high to catch run condition that
     # was discovered when reviewing
     # https://github.com/SatelliteQE/broker/pull/53
     # With count like this, I've got reproducibility probability
     # arround 0.5
```

### Comparing `broker-0.3.1/tests/test_helpers.py` & `broker-0.3.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.1/tests/test_settings.py` & `broker-0.3.2/tests/test_settings.py`

 * *Files identical despite different names*

