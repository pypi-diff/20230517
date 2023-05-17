# Comparing `tmp/cobald-tardis-0.7.0.tar.gz` & `tmp/cobald-tardis-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobald-tardis-0.7.0.tar", last modified: Mon Feb 27 08:06:24 2023, max compression
+gzip compressed data, was "cobald-tardis-0.7.1.tar", last modified: Wed May 17 07:39:38 2023, max compression
```

## Comparing `cobald-tardis-0.7.0.tar` & `cobald-tardis-0.7.1.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.039541 cobald-tardis-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-02-27 08:06:24.039541 cobald-tardis-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/cobald_tardis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-02-27 08:06:23.000000 cobald-tardis-0.7.0/cobald_tardis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-02-27 08:06:23.000000 cobald-tardis-0.7.0/cobald_tardis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 08:06:23.000000 cobald-tardis-0.7.0/cobald_tardis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-27 08:06:23.000000 cobald-tardis-0.7.0/cobald_tardis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 08:06:23.000000 cobald-tardis-0.7.0/cobald_tardis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-27 08:06:23.000000 cobald-tardis-0.7.0/cobald_tardis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-27 08:06:23.000000 cobald-tardis-0.7.0/cobald_tardis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-27 08:06:24.039541 cobald-tardis-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/tardis/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/tardis/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/tardis/adapters/batchsystems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/batchsystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/batchsystems/fakebatchsystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/batchsystems/htcondor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/batchsystems/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/tardis/adapters/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/cloudstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/fakesite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/htcondor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/lancium.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/moab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/openstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/adapters/sites/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/tardis/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/agents/batchsystemagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/agents/siteagent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/tardis/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/configuration/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/tardis/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/exceptions/executorexceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/exceptions/tardisexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.027541 cobald-tardis-0.7.0/tardis/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/interfaces/batchsystemadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/interfaces/borg.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/interfaces/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/interfaces/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/interfaces/siteadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/interfaces/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/plugins/auditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/plugins/elasticsearchmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/plugins/prometheusmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/plugins/sqliteregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/plugins/telegrafmonitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/resources/drone.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/resources/dronestates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/resources/poolfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/rest/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/rest/app/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/routers/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/routers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/routers/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/app/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/rest/hash_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/hash_credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/hash_credentials/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/hash_credentials/hash_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/rest/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/asyncbulkcall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/asynccachemap.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/attributedict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/utilities/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/executors/shellexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/executors/sshexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tardis/utilities/simulators/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/simulators/periodicvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/simulators/randomgauss.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/staticmapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tardis/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.023541 cobald-tardis-0.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tests/adapters_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.031541 cobald-tardis-0.7.0/tests/adapters_t/batchsystems_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/batchsystems_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/batchsystems_t/test_fakebatchsystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/batchsystems_t/test_htcondor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/batchsystems_t/test_slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/adapters_t/sites_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_cloudstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_fakesite.py
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_htcondorsiteadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_lancium.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_moab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_openstack.py
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/agents_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/agents_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/agents_t/test_batchsystemagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/agents_t/test_siteagent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/configuration_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/configuration_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/configuration_t/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/configuration_t/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/interfaces_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/interfaces_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/interfaces_t/test_batchsystemadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/interfaces_t/test_siteadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/plugins_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/plugins_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/plugins_t/test_auditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/plugins_t/test_elasticsearchmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/plugins_t/test_prometheusmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/plugins_t/test_sqliteregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/plugins_t/test_telegrafmonitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/resources_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/resources_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/resources_t/test_drone.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/resources_t/test_dronestates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/resources_t/test_poolfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/rest_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/rest_t/app_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/app_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/app_t/test_crutd.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/app_t/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/app_t/test_security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/rest_t/hash_credentials_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/hash_credentials_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/hash_credentials_t/test_hash_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/hash_credentials_t/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/rest_t/routers_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/routers_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/routers_t/base_test_case_routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/routers_t/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/routers_t/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/routers_t/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/rest_t/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.035541 cobald-tardis-0.7.0/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.039541 cobald-tardis-0.7.0/tests/utilities_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.039541 cobald-tardis-0.7.0/tests/utilities_t/executors_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/executors_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/executors_t/test_shellexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/executors_t/test_sshexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:24.039541 cobald-tardis-0.7.0/tests/utilities_t/simulators_t/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/simulators_t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/simulators_t/test_periodicvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/simulators_t/test_randomgauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/test_asyncbulkcall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/test_asynccachemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/test_attributedict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/test_staticmapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-02-27 08:06:12.000000 cobald-tardis-0.7.0/tests/utilities_t/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.490338 cobald-tardis-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-17 07:39:38.490338 cobald-tardis-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.474338 cobald-tardis-0.7.1/cobald_tardis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-17 07:39:38.000000 cobald-tardis-0.7.1/cobald_tardis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-17 07:39:38.000000 cobald-tardis-0.7.1/cobald_tardis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:39:38.000000 cobald-tardis-0.7.1/cobald_tardis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-17 07:39:38.000000 cobald-tardis-0.7.1/cobald_tardis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:39:38.000000 cobald-tardis-0.7.1/cobald_tardis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-17 07:39:38.000000 cobald-tardis-0.7.1/cobald_tardis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 07:39:38.000000 cobald-tardis-0.7.1/cobald_tardis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 07:39:38.490338 cobald-tardis-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.474338 cobald-tardis-0.7.1/tardis/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.474338 cobald-tardis-0.7.1/tardis/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.474338 cobald-tardis-0.7.1/tardis/adapters/batchsystems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/batchsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/batchsystems/fakebatchsystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/batchsystems/htcondor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/batchsystems/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.478338 cobald-tardis-0.7.1/tardis/adapters/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/cloudstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/fakesite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/htcondor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/lancium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/openstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/adapters/sites/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.478338 cobald-tardis-0.7.1/tardis/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/agents/batchsystemagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/agents/siteagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.478338 cobald-tardis-0.7.1/tardis/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/configuration/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.478338 cobald-tardis-0.7.1/tardis/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/exceptions/executorexceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/exceptions/tardisexceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.478338 cobald-tardis-0.7.1/tardis/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/interfaces/batchsystemadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/interfaces/borg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/interfaces/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/interfaces/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/interfaces/siteadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/interfaces/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.478338 cobald-tardis-0.7.1/tardis/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/plugins/auditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/plugins/elasticsearchmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/plugins/prometheusmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/plugins/sqliteregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/plugins/telegrafmonitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.478338 cobald-tardis-0.7.1/tardis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/resources/drone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/resources/dronestates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/resources/poolfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.478338 cobald-tardis-0.7.1/tardis/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.482338 cobald-tardis-0.7.1/tardis/rest/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.482338 cobald-tardis-0.7.1/tardis/rest/app/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/routers/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/routers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/routers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/app/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.482338 cobald-tardis-0.7.1/tardis/rest/hash_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/hash_credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/hash_credentials/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/hash_credentials/hash_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/rest/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.482338 cobald-tardis-0.7.1/tardis/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/asyncbulkcall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/asynccachemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/attributedict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.482338 cobald-tardis-0.7.1/tardis/utilities/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/executors/shellexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/executors/sshexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.482338 cobald-tardis-0.7.1/tardis/utilities/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/simulators/periodicvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/simulators/randomgauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/staticmapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tardis/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.474338 cobald-tardis-0.7.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.482338 cobald-tardis-0.7.1/tests/adapters_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.482338 cobald-tardis-0.7.1/tests/adapters_t/batchsystems_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/batchsystems_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/batchsystems_t/test_fakebatchsystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/batchsystems_t/test_htcondor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/batchsystems_t/test_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/adapters_t/sites_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_cloudstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_fakesite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_htcondorsiteadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_lancium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_openstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/agents_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/agents_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/agents_t/test_batchsystemagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/agents_t/test_siteagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/configuration_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/configuration_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/configuration_t/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/configuration_t/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/interfaces_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/interfaces_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/interfaces_t/test_batchsystemadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/interfaces_t/test_siteadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/plugins_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/plugins_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/plugins_t/test_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/plugins_t/test_elasticsearchmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/plugins_t/test_prometheusmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/plugins_t/test_sqliteregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/plugins_t/test_telegrafmonitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/resources_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/resources_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/resources_t/test_drone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/resources_t/test_dronestates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/resources_t/test_poolfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/rest_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/rest_t/app_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/app_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/app_t/test_crutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/app_t/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/app_t/test_security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.486338 cobald-tardis-0.7.1/tests/rest_t/hash_credentials_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/hash_credentials_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/hash_credentials_t/test_hash_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/hash_credentials_t/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.490338 cobald-tardis-0.7.1/tests/rest_t/routers_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/routers_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/routers_t/base_test_case_routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/routers_t/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/routers_t/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/routers_t/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/rest_t/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.490338 cobald-tardis-0.7.1/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.490338 cobald-tardis-0.7.1/tests/utilities_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.490338 cobald-tardis-0.7.1/tests/utilities_t/executors_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/executors_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/executors_t/test_shellexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/executors_t/test_sshexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:38.490338 cobald-tardis-0.7.1/tests/utilities_t/simulators_t/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/simulators_t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/simulators_t/test_periodicvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/simulators_t/test_randomgauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/test_asyncbulkcall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/test_asynccachemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/test_attributedict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/test_staticmapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-17 07:39:27.000000 cobald-tardis-0.7.1/tests/utilities_t/test_utils.py
```

### Comparing `cobald-tardis-0.7.0/LICENSE.txt` & `cobald-tardis-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/PKG-INFO` & `cobald-tardis-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobald-tardis
-Version: 0.7.0
+Version: 0.7.1
 Summary: Transparent Adaptive Resource Dynamic Integration System
 Home-page: https://github.com/matterminers/tardis
 Author: Manuel Giffels, Matthias Schnepf
 Author-email: giffels@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/matterminers/tardis/issues
 Project-URL: Source, https://github.com/matterminers/tardis
```

### Comparing `cobald-tardis-0.7.0/README.md` & `cobald-tardis-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/cobald_tardis.egg-info/PKG-INFO` & `cobald-tardis-0.7.1/cobald_tardis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobald-tardis
-Version: 0.7.0
+Version: 0.7.1
 Summary: Transparent Adaptive Resource Dynamic Integration System
 Home-page: https://github.com/matterminers/tardis
 Author: Manuel Giffels, Matthias Schnepf
 Author-email: giffels@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/matterminers/tardis/issues
 Project-URL: Source, https://github.com/matterminers/tardis
```

### Comparing `cobald-tardis-0.7.0/cobald_tardis.egg-info/SOURCES.txt` & `cobald-tardis-0.7.1/cobald_tardis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/cobald_tardis.egg-info/entry_points.txt` & `cobald-tardis-0.7.1/cobald_tardis.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/cobald_tardis.egg-info/requires.txt` & `cobald-tardis-0.7.1/cobald_tardis.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 elasticsearch<8.0.0,>=7.17
 aioprometheus>=21.9.0
 kubernetes_asyncio
 pydantic
 asyncstdlib
 typing_extensions
 backports.cached_property
-python-auditor==0.0.7
+python-auditor==0.1.0
 pytz
 tzlocal
 aiolancium
 fastapi-jwt-auth
 python-jose
 uvicorn[standard]<=0.14.0
 typer
```

### Comparing `cobald-tardis-0.7.0/setup.py` & `cobald-tardis-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         "elasticsearch>=7.17,<8.0.0",
         "aioprometheus>=21.9.0",
         "kubernetes_asyncio",
         "pydantic",
         "asyncstdlib",
         "typing_extensions",
         "backports.cached_property",
-        "python-auditor==0.0.7",
+        "python-auditor==0.1.0",
         "pytz",
         "tzlocal",
         "aiolancium",
         *REST_REQUIRES,
     ],
     extras_require={
         "docs": [
```

### Comparing `cobald-tardis-0.7.0/tardis/adapters/batchsystems/fakebatchsystem.py` & `cobald-tardis-0.7.1/tardis/adapters/batchsystems/fakebatchsystem.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/adapters/batchsystems/htcondor.py` & `cobald-tardis-0.7.1/tardis/adapters/batchsystems/htcondor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/adapters/batchsystems/slurm.py` & `cobald-tardis-0.7.1/tardis/adapters/batchsystems/slurm.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/adapters/sites/cloudstack.py` & `cobald-tardis-0.7.1/tardis/adapters/sites/cloudstack.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/adapters/sites/fakesite.py` & `cobald-tardis-0.7.1/tardis/adapters/sites/fakesite.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/adapters/sites/htcondor.py` & `cobald-tardis-0.7.1/tardis/adapters/sites/htcondor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from ...interfaces.siteadapter import ResourceStatus
 from ...interfaces.executor import Executor
 from ...utilities.asynccachemap import AsyncCacheMap
 from ...utilities.attributedict import AttributeDict
 from ...utilities.staticmapping import StaticMapping
 from ...utilities.executors.shellexecutor import ShellExecutor
 from ...utilities.asyncbulkcall import AsyncBulkCall
-from ...utilities.utils import csv_parser, machine_meta_data_translation
+from ...utilities.utils import (
+    csv_parser,
+    drone_environment_to_str,
+    machine_meta_data_translation,
+)
 
 from contextlib import contextmanager
 from datetime import datetime
 from functools import partial
 from string import Template
 
 import warnings
@@ -241,27 +245,25 @@
             jdl_template = Template(f.read())
 
         drone_environment = self.drone_environment(
             resource_attributes.drone_uuid,
             resource_attributes.obs_machine_meta_data_translation_mapping,
         )
 
-        def job_environment(seperator, prefix, customize_key=lambda x: x):
-            return seperator.join(
-                f"{prefix}{customize_key(key)}={value}"
-                for key, value in drone_environment.items()
-            )
-
         submit_jdl = jdl_template.substitute(
             machine_meta_data_translation(
                 self.machine_meta_data,
                 self.htcondor_machine_meta_data_translation_mapping,
             ),
-            Environment=job_environment(";", prefix="TardisDrone"),
-            Arguments=job_environment(" ", prefix="--", customize_key=str.lower),
+            Environment=drone_environment_to_str(
+                drone_environment, seperator=";", prefix="TardisDrone"
+            ),
+            Arguments=drone_environment_to_str(
+                drone_environment, seperator=" ", prefix="--", customize_key=str.lower
+            ),
         )
 
         job_id = await self._condor_submit(submit_jdl)
         response = AttributeDict(JobId=job_id)
         response.update(self.create_timestamps())
         return self.handle_response(response)
```

### Comparing `cobald-tardis-0.7.0/tardis/adapters/sites/kubernetes.py` & `cobald-tardis-0.7.1/tardis/adapters/sites/kubernetes.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/adapters/sites/lancium.py` & `cobald-tardis-0.7.1/tardis/adapters/sites/lancium.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/adapters/sites/moab.py` & `cobald-tardis-0.7.1/tardis/adapters/sites/moab.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from ...interfaces.siteadapter import ResourceStatus
 from ...interfaces.siteadapter import SiteAdapter
 from ...utilities.staticmapping import StaticMapping
 from ...utilities.attributedict import AttributeDict
 from ...utilities.attributedict import convert_to_attribute_dict
 from ...utilities.executors.shellexecutor import ShellExecutor
 from ...utilities.asynccachemap import AsyncCacheMap
-from ...utilities.utils import submit_cmd_option_formatter
+from ...utilities.utils import (
+    convert_to,
+    drone_environment_to_str,
+    submit_cmd_option_formatter,
+)
 
 from asyncio import TimeoutError
 from contextlib import contextmanager
 from functools import partial
 from datetime import datetime
 
 import asyncssh
@@ -116,24 +120,27 @@
             key_translator=key_translator,
             translator_functions=translator_functions,
         )
 
     async def deploy_resource(
         self, resource_attributes: AttributeDict
     ) -> AttributeDict:
-        request_command = f"msub {self.msub_cmdline_options()} {self._startup_command}"
+        msub_cmdline_option_string = self.msub_cmdline_options(
+            resource_attributes.drone_uuid,
+            resource_attributes.obs_machine_meta_data_translation_mapping,
+        )
+        request_command = f"msub {msub_cmdline_option_string} {self._startup_command}"
         result = await self._executor.run_command(request_command)
         logger.debug(f"{self.site_name} servers create returned {result}")
 
         remote_resource_uuid = int(result.stdout)
         resource_attributes.update(
             remote_resource_uuid=remote_resource_uuid,
             created=datetime.now(),
             updated=datetime.now(),
-            drone_uuid=self.drone_uuid(remote_resource_uuid),
             resource_status=ResourceStatus.Booting,
         )
         return resource_attributes
 
     @staticmethod
     def check_remote_resource_uuid(resource_attributes, regex, response):
         pattern = re.compile(regex, flags=re.MULTILINE)
@@ -200,30 +207,38 @@
             {"SystemJID": remote_resource_uuid}, **resource_attributes
         )
 
     async def stop_resource(self, resource_attributes: AttributeDict):
         logger.debug("MOAB jobs cannot be stopped gracefully. Terminating instead.")
         return await self.terminate_resource(resource_attributes)
 
-    def msub_cmdline_options(self):
+    def msub_cmdline_options(self, drone_uuid, machine_meta_data_translation_mapping):
         sbatch_options = self.machine_type_configuration.get(
             "SubmitOptions", AttributeDict()
         )
 
         walltime = self.machine_type_configuration.Walltime
         mem = self.machine_meta_data.Memory
         node_type = self.machine_type_configuration.NodeType
 
+        drone_environment = drone_environment_to_str(
+            self.drone_environment(drone_uuid, machine_meta_data_translation_mapping),
+            seperator=",",
+            prefix="TardisDrone",
+            customize_value=lambda x: convert_to(x, int, x),
+        )
+
         return submit_cmd_option_formatter(
             AttributeDict(
                 short=AttributeDict(
                     **sbatch_options.get("short", AttributeDict()),
                     j="oe",
                     m="p",
                     l=f"walltime={walltime},mem={mem}gb,nodes={node_type}",
+                    v=f"{drone_environment}",
                 ),
                 long=AttributeDict(
                     **sbatch_options.get("long", AttributeDict()),
                 ),
             )
         )
```

### Comparing `cobald-tardis-0.7.0/tardis/adapters/sites/openstack.py` & `cobald-tardis-0.7.1/tardis/adapters/sites/openstack.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/adapters/sites/slurm.py` & `cobald-tardis-0.7.1/tardis/adapters/sites/slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 from ...interfaces.siteadapter import ResourceStatus
 from ...interfaces.siteadapter import SiteAdapter
 from ...utilities.staticmapping import StaticMapping
 from ...utilities.attributedict import AttributeDict
 from ...utilities.attributedict import convert_to_attribute_dict
 from ...utilities.executors.shellexecutor import ShellExecutor
 from ...utilities.asynccachemap import AsyncCacheMap
-from ...utilities.utils import convert_to, csv_parser, submit_cmd_option_formatter
+from ...utilities.utils import (
+    convert_to,
+    drone_environment_to_str,
+    csv_parser,
+    submit_cmd_option_formatter,
+)
 
 from asyncio import TimeoutError
 from contextlib import contextmanager
 from functools import partial
 from datetime import datetime
 
 import logging
@@ -169,19 +174,19 @@
     def sbatch_cmdline_options(self, drone_uuid, machine_meta_data_translation_mapping):
         sbatch_options = self.machine_type_configuration.get(
             "SubmitOptions", AttributeDict()
         )
 
         walltime = self.machine_type_configuration.Walltime
 
-        drone_environment = ",".join(
-            f"TardisDrone{key}={convert_to(value, int, value)}"
-            for key, value in self.drone_environment(
-                drone_uuid, machine_meta_data_translation_mapping
-            ).items()
+        drone_environment = drone_environment_to_str(
+            self.drone_environment(drone_uuid, machine_meta_data_translation_mapping),
+            seperator=",",
+            prefix="TardisDrone",
+            customize_value=lambda x: convert_to(x, int, x),
         )
 
         return AttributeDict(
             short=AttributeDict(
                 **sbatch_options.get("short", AttributeDict()),
                 p=self.machine_type_configuration.Partition,
                 N=1,
```

### Comparing `cobald-tardis-0.7.0/tardis/agents/batchsystemagent.py` & `cobald-tardis-0.7.1/tardis/agents/batchsystemagent.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/agents/siteagent.py` & `cobald-tardis-0.7.1/tardis/agents/siteagent.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/configuration/configuration.py` & `cobald-tardis-0.7.1/tardis/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/configuration/utilities.py` & `cobald-tardis-0.7.1/tardis/configuration/utilities.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/exceptions/executorexceptions.py` & `cobald-tardis-0.7.1/tardis/exceptions/executorexceptions.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/interfaces/batchsystemadapter.py` & `cobald-tardis-0.7.1/tardis/interfaces/batchsystemadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/interfaces/borg.py` & `cobald-tardis-0.7.1/tardis/interfaces/borg.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/interfaces/siteadapter.py` & `cobald-tardis-0.7.1/tardis/interfaces/siteadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/interfaces/state.py` & `cobald-tardis-0.7.1/tardis/interfaces/state.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/plugins/auditor.py` & `cobald-tardis-0.7.1/tardis/plugins/auditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,20 @@
                 self._components[site.name][machine_type] = {}
                 for resource in getattr(config, site.name).MachineMetaData[
                     machine_type
                 ]:
                     self._resources[site.name][machine_type][resource] = getattr(
                         config, site.name
                     ).MachineMetaData[machine_type][resource]
-                    self._components[site.name][machine_type][resource] = getattr(
-                        config_auditor.components, machine_type
-                    ).get(resource, {})
+                    try:
+                        self._components[site.name][machine_type][resource] = getattr(
+                            config_auditor.components, machine_type
+                        ).get(resource, {})
+                    except AttributeError:
+                        continue
 
         self._user = getattr(config_auditor, "user", "tardis")
         self._group = getattr(config_auditor, "group", "tardis")
         auditor_timeout = getattr(config_auditor, "timeout", 30)
         self._local_timezone = get_localzone()
         self._client = (
             pyauditor.AuditorClientBuilder()
```

### Comparing `cobald-tardis-0.7.0/tardis/plugins/elasticsearchmonitoring.py` & `cobald-tardis-0.7.1/tardis/plugins/elasticsearchmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/plugins/prometheusmonitoring.py` & `cobald-tardis-0.7.1/tardis/plugins/prometheusmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/plugins/sqliteregistry.py` & `cobald-tardis-0.7.1/tardis/plugins/sqliteregistry.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/plugins/telegrafmonitoring.py` & `cobald-tardis-0.7.1/tardis/plugins/telegrafmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/resources/drone.py` & `cobald-tardis-0.7.1/tardis/resources/drone.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/resources/dronestates.py` & `cobald-tardis-0.7.1/tardis/resources/dronestates.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/resources/poolfactory.py` & `cobald-tardis-0.7.1/tardis/resources/poolfactory.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/rest/app/crud.py` & `cobald-tardis-0.7.1/tardis/rest/app/crud.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/rest/app/main.py` & `cobald-tardis-0.7.1/tardis/rest/app/main.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/rest/app/routers/resources.py` & `cobald-tardis-0.7.1/tardis/rest/app/routers/resources.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/rest/app/routers/types.py` & `cobald-tardis-0.7.1/tardis/rest/app/routers/types.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/rest/app/routers/user.py` & `cobald-tardis-0.7.1/tardis/rest/app/routers/user.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/rest/app/security.py` & `cobald-tardis-0.7.1/tardis/rest/app/security.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/rest/service.py` & `cobald-tardis-0.7.1/tardis/rest/service.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/asyncbulkcall.py` & `cobald-tardis-0.7.1/tardis/utilities/asyncbulkcall.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/asynccachemap.py` & `cobald-tardis-0.7.1/tardis/utilities/asynccachemap.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/attributedict.py` & `cobald-tardis-0.7.1/tardis/utilities/attributedict.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/executors/shellexecutor.py` & `cobald-tardis-0.7.1/tardis/utilities/executors/shellexecutor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/executors/sshexecutor.py` & `cobald-tardis-0.7.1/tardis/utilities/executors/sshexecutor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/pipeline.py` & `cobald-tardis-0.7.1/tardis/utilities/pipeline.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/simulators/periodicvalue.py` & `cobald-tardis-0.7.1/tardis/utilities/simulators/periodicvalue.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/simulators/randomgauss.py` & `cobald-tardis-0.7.1/tardis/utilities/simulators/randomgauss.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tardis/utilities/utils.py` & `cobald-tardis-0.7.1/tardis/utilities/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .attributedict import AttributeDict
 
 from contextlib import contextmanager
 from io import StringIO
-from typing import Any, Callable, List, TypeVar, Tuple
+from typing import Any, Callable, Dict, List, TypeVar, Tuple
 
 
 import csv
 import logging
 
 logger = logging.getLogger("cobald.runtime.tardis.utilities.utils")
 
@@ -138,7 +138,20 @@
 def convert_to(
     value: Any, convert_to_type: Callable[[Any], T], default: Any = sentinel
 ) -> T:
     try:
         return convert_to_type(value)
     except ValueError:
         return default
+
+
+def drone_environment_to_str(
+    drone_environment: Dict,
+    seperator: str,
+    prefix: str,
+    customize_key: Callable = lambda x: x,
+    customize_value: Callable = lambda x: x,
+) -> str:
+    return seperator.join(
+        f"{prefix}{customize_key(key)}={customize_value(value)}"
+        for key, value in drone_environment.items()
+    )
```

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/batchsystems_t/test_fakebatchsystem.py` & `cobald-tardis-0.7.1/tests/adapters_t/batchsystems_t/test_fakebatchsystem.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/batchsystems_t/test_htcondor.py` & `cobald-tardis-0.7.1/tests/adapters_t/batchsystems_t/test_htcondor.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,40 +255,37 @@
             MachineStatus.Available,
         )
         self.mock_executor.reset_mock()
 
         self.mock_executor.return_value.run_command.side_effect = (
             CommandExecutionFailure(message="Test", exit_code=123, stderr="Test")
         )
+
+        attributes = {
+            "Machine": "Machine",
+            "Name": "Name",
+            "State": "State",
+            "Activity": "Activity",
+            "TardisDroneUuid": "TardisDroneUuid",
+        }
+        # Escape htcondor expressions and add them to attributes
+        attributes.update(
+            {key: quote(value) for key, value in self.config.BatchSystem.ratios.items()}
+        )
         with self.assertLogs(level=logging.WARNING):
             with self.assertRaises(CommandExecutionFailure):
-                attributes = {
-                    "Machine": "Machine",
-                    "State": "State",
-                    "Activity": "Activity",
-                    "TardisDroneUuid": "TardisDroneUuid",
-                }
-                # Escape htcondor expressions and add them to attributes
-                attributes.update(
-                    {
-                        key: quote(value)
-                        for key, value in self.config.BatchSystem.ratios.items()
-                    }
-                )
                 run_async(
                     partial(
                         htcondor_status_updater,
                         self.config.BatchSystem.options,
                         attributes,
                         self.mock_executor.return_value,
                     )
                 )
-                self.mock_executor.return_value.run_command.assert_called_with(
-                    self.command
-                )
+        self.mock_executor.return_value.run_command.assert_called_with(self.command)
         self.mock_executor.return_value.run_command.side_effect = None
 
     @mock_executor_run_command(stdout=CONDOR_RETURN)
     def test_get_utilisation(self):
         self.assertEqual(
             run_async(self.htcondor_adapter.get_utilisation, drone_uuid="test"),
             min([self.cpu_ratio, self.memory_ratio]),
```

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/batchsystems_t/test_slurm.py` & `cobald-tardis-0.7.1/tests/adapters_t/batchsystems_t/test_slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,33 +177,33 @@
 
         self.mock_executor.reset_mock()
 
         self.mock_executor.return_value.run_command.side_effect = (
             CommandExecutionFailure(message="Test", exit_code=123, stderr="Test")
         )
 
+        attributes = {
+            "statelong": "statelong",
+            "cpusstate": "cpusstate",
+            "allocmem": "allocmem",
+            "memory": "memory",
+            "features": "features",
+            "nodehost": "nodehost",
+        }
         with self.assertLogs(level="WARN"):
             with self.assertRaises(CommandExecutionFailure):
-                attributes = {
-                    "Machine": "Machine",
-                    "State": "State",
-                    "Activity": "Activity",
-                    "TardisDroneUuid": "TardisDroneUuid",
-                }
                 run_async(
                     partial(
                         slurm_status_updater,
                         self.config.BatchSystem.options,
                         attributes,
                         self.mock_executor.return_value,
                     )
                 )
-                self.mock_executor.return_value.run_command.assert_called_with(
-                    self.command
-                )
+        self.mock_executor.return_value.run_command.assert_called_with(self.command)
 
         self.mock_executor.return_value.run_command.side_effect = None
 
     @mock_executor_run_command(stdout=SINFO_RETURN)
     def test_get_utilisation(self):
         self.assertEqual(
             run_async(self.slurm_adapter.get_utilisation, drone_uuid="VM-1"),
```

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_cloudstack.py` & `cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_cloudstack.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_fakesite.py` & `cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_fakesite.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_htcondorsiteadapter.py` & `cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_htcondorsiteadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_kubernetes.py` & `cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_lancium.py` & `cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_lancium.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_moab.py` & `cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_moab.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self.moab_adapter = MoabAdapter(machine_type="test2large", site_name="TestSite")
 
     def tearDown(self):
         pass
 
     @property
     def machine_meta_data(self):
-        return AttributeDict(test2large=AttributeDict(Cores=128, Memory="120"))
+        return AttributeDict(test2large=AttributeDict(Cores=128, Memory=120, Disk=100))
 
     @property
     def machine_type_configuration(self):
         return AttributeDict(
             test2large=AttributeDict(
                 NodeType="1:ppn=20", StartupCommand="startVM.py", Walltime="02:00:00:00"
             )
@@ -194,15 +194,20 @@
             resource_status=ResourceStatus.Booting,
             created=datetime.strptime(
                 "Wed Jan 23 2019 15:01:47", "%a %b %d %Y %H:%M:%S"
             ),
             updated=datetime.strptime(
                 "Wed Jan 23 2019 15:02:17", "%a %b %d %Y %H:%M:%S"
             ),
-            drone_uuid="testsite-4761849",
+            drone_uuid="testsite-abcdef",
+            obs_machine_meta_data_translation_mapping=AttributeDict(
+                Cores=1,
+                Memory=1,
+                Disk=1,
+            ),
         )
 
     def test_start_up_command_deprecation_warning(self):
         # Necessary to avoid annoying message in PyCharm
         filterwarnings(action="ignore", message="unclosed", category=ResourceWarning)
         del self.test_site_config.MachineTypeConfiguration.test2large.StartupCommand
 
@@ -222,17 +227,15 @@
     def test_deploy_resource(self):
         expected_resource_attributes = self.resource_attributes
         expected_resource_attributes.update(
             created=datetime.now(), updated=datetime.now()
         )
         return_resource_attributes = run_async(
             self.moab_adapter.deploy_resource,
-            resource_attributes=AttributeDict(
-                machine_type="test2large", site_name="TestSite"
-            ),
+            resource_attributes=self.resource_attributes,
         )
         if (
             return_resource_attributes.created - expected_resource_attributes.created
             > timedelta(seconds=1)
             or return_resource_attributes.updated - expected_resource_attributes.updated
             > timedelta(seconds=1)
         ):
@@ -241,15 +244,15 @@
             expected_resource_attributes.created,
             expected_resource_attributes.updated,
             return_resource_attributes.created,
             return_resource_attributes.updated,
         )
         self.assertEqual(return_resource_attributes, expected_resource_attributes)
         self.mock_executor.return_value.run_command.assert_called_with(
-            "msub -j oe -m p -l walltime=02:00:00:00,mem=120gb,nodes=1:ppn=20 startVM.py"  # noqa: B950
+            "msub -j oe -m p -l walltime=02:00:00:00,mem=120gb,nodes=1:ppn=20 -v TardisDroneCores=128,TardisDroneMemory=120,TardisDroneDisk=100,TardisDroneUuid=testsite-abcdef startVM.py"  # noqa: B950
         )
 
     @mock_executor_run_command(TEST_DEPLOY_RESOURCE_RESPONSE)
     def test_deploy_resource_w_submit_options(self):
         self.test_site_config.MachineTypeConfiguration.test2large.SubmitOptions = (
             AttributeDict(
                 short=AttributeDict(M="someone@somewhere.com"),
@@ -257,21 +260,18 @@
             )
         )
 
         moab_adapter = MoabAdapter(machine_type="test2large", site_name="TestSite")
 
         run_async(
             moab_adapter.deploy_resource,
-            resource_attributes=AttributeDict(
-                machine_type="test2large",
-                site_name="TestSite",
-            ),
+            resource_attributes=self.resource_attributes,
         )
         self.mock_executor.return_value.run_command.assert_called_with(
-            "msub -M someone@somewhere.com -j oe -m p -l walltime=02:00:00:00,mem=120gb,nodes=1:ppn=20 --timeout=60 startVM.py"  # noqa: B950
+            "msub -M someone@somewhere.com -j oe -m p -l walltime=02:00:00:00,mem=120gb,nodes=1:ppn=20 -v TardisDroneCores=128,TardisDroneMemory=120,TardisDroneDisk=100,TardisDroneUuid=testsite-abcdef --timeout=60 startVM.py"  # noqa: B950
         )
 
     def test_machine_meta_data(self):
         self.assertEqual(
             self.moab_adapter.machine_meta_data, self.machine_meta_data["test2large"]
         )
```

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_openstack.py` & `cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_openstack.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/adapters_t/sites_t/test_slurm.py` & `cobald-tardis-0.7.1/tests/adapters_t/sites_t/test_slurm.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/agents_t/test_batchsystemagent.py` & `cobald-tardis-0.7.1/tests/agents_t/test_batchsystemagent.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/agents_t/test_siteagent.py` & `cobald-tardis-0.7.1/tests/agents_t/test_siteagent.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/configuration_t/test_configuration.py` & `cobald-tardis-0.7.1/tests/configuration_t/test_configuration.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/configuration_t/test_utilities.py` & `cobald-tardis-0.7.1/tests/configuration_t/test_utilities.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/interfaces_t/test_batchsystemadapter.py` & `cobald-tardis-0.7.1/tests/interfaces_t/test_batchsystemadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/interfaces_t/test_siteadapter.py` & `cobald-tardis-0.7.1/tests/interfaces_t/test_siteadapter.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/plugins_t/test_auditor.py` & `cobald-tardis-0.7.1/tests/plugins_t/test_auditor.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,7 +159,12 @@
         self.assertEqual(record.components[0].scores[1].name, "BENCHMARK")
         self.assertEqual(record.components[0].scores[1].value, 3.0)
         self.assertEqual(record.components[1].name, "Memory")
         self.assertEqual(record.components[1].amount, 100)
         self.assertEqual(len(record.components[1].scores), 1)
         self.assertEqual(record.components[1].scores[0].name, "BLUBB")
         self.assertEqual(record.components[1].scores[0].value, 1.4)
+
+    def test_missing_components(self):
+        del self.config.Plugins.Auditor.components
+        plugin = Auditor()
+        self.assertEqual(plugin._components, {"testsite": {"test_machine_type": {}}})
```

### Comparing `cobald-tardis-0.7.0/tests/plugins_t/test_elasticsearchmonitoring.py` & `cobald-tardis-0.7.1/tests/plugins_t/test_elasticsearchmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/plugins_t/test_prometheusmonitoring.py` & `cobald-tardis-0.7.1/tests/plugins_t/test_prometheusmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/plugins_t/test_sqliteregistry.py` & `cobald-tardis-0.7.1/tests/plugins_t/test_sqliteregistry.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/plugins_t/test_telegrafmonitoring.py` & `cobald-tardis-0.7.1/tests/plugins_t/test_telegrafmonitoring.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/resources_t/test_drone.py` & `cobald-tardis-0.7.1/tests/resources_t/test_drone.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/resources_t/test_dronestates.py` & `cobald-tardis-0.7.1/tests/resources_t/test_dronestates.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/resources_t/test_poolfactory.py` & `cobald-tardis-0.7.1/tests/resources_t/test_poolfactory.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/rest_t/app_t/test_crutd.py` & `cobald-tardis-0.7.1/tests/rest_t/app_t/test_crutd.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/rest_t/app_t/test_security.py` & `cobald-tardis-0.7.1/tests/rest_t/app_t/test_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,26 +51,23 @@
         get_user.cache_clear()
 
     def test_check_scope_permissions(self):
         with self.assertRaises(HTTPException) as cm:
             check_scope_permissions(
                 ["user:get", "resources:get"], ["user:get", "user:put"]
             )
-            self.assertEqual(
-                cm.exception,
-                HTTPException(
-                    status_code=status.HTTP_403_FORBIDDEN,
-                    detail={
-                        "msg": "Not enough permissions",
-                        "failedAt": "resources:get",
-                        "allowedScopes": ["user:get", "user:put"],
-                    },
-                ),
-            )
-
+        self.assertEqual(cm.exception.status_code, status.HTTP_403_FORBIDDEN)
+        self.assertDictEqual(
+            cm.exception.detail,
+            {
+                "msg": "Not enough permissions",
+                "failedAt": "resources:get",
+                "allowedScopes": ["user:get", "user:put"],
+            },
+        )
         check_scope_permissions(["resources:get"], ["resources:get"])
 
     def test_check_authentication(self):
         self.clear_lru_cache()
 
         with self.assertRaises(HTTPException) as he:
             check_authentication(user_name="fails", password="test123")
```

### Comparing `cobald-tardis-0.7.0/tests/rest_t/hash_credentials_t/test_hash_credentials.py` & `cobald-tardis-0.7.1/tests/rest_t/hash_credentials_t/test_hash_credentials.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/rest_t/hash_credentials_t/test_main.py` & `cobald-tardis-0.7.1/tests/rest_t/hash_credentials_t/test_main.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/rest_t/routers_t/base_test_case_routers.py` & `cobald-tardis-0.7.1/tests/rest_t/routers_t/base_test_case_routers.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/rest_t/routers_t/test_resources.py` & `cobald-tardis-0.7.1/tests/rest_t/routers_t/test_resources.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/rest_t/routers_t/test_types.py` & `cobald-tardis-0.7.1/tests/rest_t/routers_t/test_types.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/rest_t/routers_t/test_user.py` & `cobald-tardis-0.7.1/tests/rest_t/routers_t/test_user.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/rest_t/test_service.py` & `cobald-tardis-0.7.1/tests/rest_t/test_service.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities/utilities.py` & `cobald-tardis-0.7.1/tests/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/executors_t/test_shellexecutor.py` & `cobald-tardis-0.7.1/tests/utilities_t/executors_t/test_shellexecutor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/executors_t/test_sshexecutor.py` & `cobald-tardis-0.7.1/tests/utilities_t/executors_t/test_sshexecutor.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/simulators_t/test_periodicvalue.py` & `cobald-tardis-0.7.1/tests/utilities_t/simulators_t/test_periodicvalue.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/simulators_t/test_randomgauss.py` & `cobald-tardis-0.7.1/tests/utilities_t/simulators_t/test_randomgauss.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/test_asyncbulkcall.py` & `cobald-tardis-0.7.1/tests/utilities_t/test_asyncbulkcall.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/test_asynccachemap.py` & `cobald-tardis-0.7.1/tests/utilities_t/test_asynccachemap.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/test_attributedict.py` & `cobald-tardis-0.7.1/tests/utilities_t/test_attributedict.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/test_pipeline.py` & `cobald-tardis-0.7.1/tests/utilities_t/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/test_staticmapping.py` & `cobald-tardis-0.7.1/tests/utilities_t/test_staticmapping.py`

 * *Files identical despite different names*

### Comparing `cobald-tardis-0.7.0/tests/utilities_t/test_utils.py` & `cobald-tardis-0.7.1/tests/utilities_t/test_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,83 @@
 import logging
 
 from tardis.resources.dronestates import RequestState
 from tardis.utilities.attributedict import AttributeDict
 from tardis.utilities.utils import (
+    convert_to,
     csv_parser,
     disable_logging,
+    drone_environment_to_str,
     htcondor_cmd_option_formatter,
     load_states,
     submit_cmd_option_formatter,
 )
 
 
 from unittest import TestCase
 
 
+class TestConvertTo(TestCase):
+    def test_convert_to(self):
+        for value, instance, converted_value in (
+            (1, int, 1),
+            ("1", int, 1),
+            (1, float, 1),
+            ("§$%", float, "§$%"),
+        ):
+            result = convert_to(value, instance, value)
+            self.assertEqual(converted_value, result)
+
+
+class TestDroneEnvironmentToStr(TestCase):
+    def test_drone_environment_to_str(self):
+        test_environment = {"Uuid": "test-abcfed", "Cores": 8, "Memory": 20.0}
+
+        for drone_environment_to_str_kwargs, result in (
+            (
+                {
+                    "seperator": ",",
+                    "prefix": "TardisDrone",
+                },
+                "TardisDroneUuid=test-abcfed,TardisDroneCores=8,TardisDroneMemory=20.0",
+            ),
+            (
+                {
+                    "seperator": " ",
+                    "prefix": "--",
+                },
+                "--Uuid=test-abcfed --Cores=8 --Memory=20.0",
+            ),
+            (
+                {
+                    "seperator": ",",
+                    "prefix": "TardisDrone",
+                    "customize_value": lambda x: convert_to(x, int, x),
+                },
+                "TardisDroneUuid=test-abcfed,TardisDroneCores=8,TardisDroneMemory=20",
+            ),
+            (
+                {
+                    "seperator": " ",
+                    "prefix": "--",
+                    "customize_key": str.lower,
+                    "customize_value": lambda x: convert_to(x, int, x),
+                },
+                "--uuid=test-abcfed --cores=8 --memory=20",
+            ),
+        ):
+            drone_environments_str = drone_environment_to_str(
+                test_environment, **drone_environment_to_str_kwargs
+            )
+            self.assertEqual(
+                drone_environments_str,
+                result,
+            )
+
+
 class TestHTCondorCMDOptionFormatter(TestCase):
     def test_htcondor_cmd_option_formatter(self):
         options = AttributeDict(pool="my-htcondor.local", test=None)
         option_string = htcondor_cmd_option_formatter(options)
 
         self.assertEqual(option_string, "-pool my-htcondor.local -test")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

