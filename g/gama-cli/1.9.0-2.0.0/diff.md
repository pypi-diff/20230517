# Comparing `tmp/gama_cli-1.9.0.tar.gz` & `tmp/gama_cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_cli-1.9.0.tar", last modified: Sun Apr 16 23:29:12 2023, max compression
+gzip compressed data, was "gama_cli-2.0.0.tar", last modified: Wed May 17 09:10:31 2023, max compression
```

## Comparing `gama_cli-1.9.0.tar` & `gama_cli-2.0.0.tar`

### file list

```diff
@@ -1,56 +1,50 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2342 2023-04-16 23:29:12.377755 gama_cli-1.9.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1708 2023-04-16 23:28:20.000000 gama_cli-1.9.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.373755 gama_cli-1.9.0/gama_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/__init__.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.373755 gama_cli-1.9.0/gama_cli/assets/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/assets/greenstream/
--rw-rw-r--   0 runner    (1000) runner    (1001)      173 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/assets/greenstream/config.sim.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      597 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/assets/greenstream/config.stubs.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      583 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/assets/greenstream/config.variant.bravo.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      184 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/assets/greenstream/config.variant.educat.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2522 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.373755 gama_cli-1.9.0/gama_cli/docker/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/docker/gs/
--rw-rw-r--   0 runner    (1000) runner    (1001)      517 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      458 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/docker/sim/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1038 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/sim/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      744 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/sim/docker-compose.standalone.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/docker/vessel/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2632 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      193 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.gpu.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      175 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      459 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      912 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      308 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      735 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      619 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)     1970 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.377755 gama_cli-1.9.0/gama_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      839 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/attach.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      327 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/docker.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      249 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/git.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     6513 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1905 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/misc.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4772 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/sim.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    12958 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/groups/vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4697 2023-04-16 23:28:20.000000 gama_cli-1.9.0/gama_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:12.373755 gama_cli-1.9.0/gama_cli.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2342 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1643 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       46 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-04-16 23:29:12.000000 gama_cli-1.9.0/gama_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-16 23:28:58.000000 gama_cli-1.9.0/gama_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      992 2023-04-16 23:29:12.377755 gama_cli-1.9.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-16 23:28:20.000000 gama_cli-1.9.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-17 09:10:31.853843 gama_cli-2.0.0/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2342 2023-05-17 09:10:31.853843 gama_cli-2.0.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1708 2023-05-17 09:09:36.000000 gama_cli-2.0.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-17 09:10:31.853843 gama_cli-2.0.0/gama_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2563 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-17 09:10:31.853843 gama_cli-2.0.0/gama_cli/docker/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-17 09:10:31.853843 gama_cli-2.0.0/gama_cli/docker/gs/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      517 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      458 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-17 09:10:31.853843 gama_cli-2.0.0/gama_cli/docker/sim/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1308 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/sim/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      744 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/sim/docker-compose.standalone.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-17 09:10:31.853843 gama_cli-2.0.0/gama_cli/docker/vessel/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2736 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      193 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.gpu.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      175 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      459 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      912 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      308 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      800 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      676 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1900 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-17 09:10:31.853843 gama_cli-2.0.0/gama_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      839 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/attach.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      327 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/docker.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      249 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/git.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     6513 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1905 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/misc.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     5446 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/sim.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    11442 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/groups/vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4697 2023-05-17 09:09:36.000000 gama_cli-2.0.0/gama_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-17 09:10:31.853843 gama_cli-2.0.0/gama_cli.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2342 2023-05-17 09:10:31.000000 gama_cli-2.0.0/gama_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1448 2023-05-17 09:10:31.000000 gama_cli-2.0.0/gama_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-05-17 09:10:31.000000 gama_cli-2.0.0/gama_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       46 2023-05-17 09:10:31.000000 gama_cli-2.0.0/gama_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-05-17 09:10:31.000000 gama_cli-2.0.0/gama_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-05-17 09:10:31.000000 gama_cli-2.0.0/gama_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-05-17 09:10:15.000000 gama_cli-2.0.0/gama_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      992 2023-05-17 09:10:31.857843 gama_cli-2.0.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-05-17 09:09:36.000000 gama_cli-2.0.0/setup.py
```

### Comparing `gama_cli-1.9.0/PKG-INFO` & `gama_cli-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_cli
-Version: 1.9.0
+Version: 2.0.0
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-1.9.0/README.md` & `gama_cli-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/banner.py` & `gama_cli-2.0.0/gama_cli/banner.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/cli.py` & `gama_cli-2.0.0/gama_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         git.git.add_command(git.pull)
 
         gama_cli.add_command(sim.sim)
         sim.sim.add_command(sim.build)
         sim.sim.add_command(sim.up)
         sim.sim.add_command(sim.down)
         sim.sim.add_command(sim.base_ue)
+        sim.sim.add_command(sim.compile)
 
         gama_cli.add_command(setup.setup)
         setup.setup.add_command(setup.secrets)
         setup.setup.add_command(setup.env)
 
         vessel.vessel.add_command(vessel.build)
         vessel.vessel.add_command(vessel.bake)
```

### Comparing `gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.dev.yaml` & `gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml` & `gama_cli-2.0.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/docker/sim/docker-compose.standalone.yaml` & `gama_cli-2.0.0/gama_cli/docker/sim/docker-compose.standalone.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.dev.yaml` & `gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.dev.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       - ./projects/gama_ui/.eslintrc.js:/app/.eslintrc.js
       - ./projects/gama_ui/.nvmrc:/app/.nvmrc
       - ./projects/gama_ui/.prettierrc:/app/.prettierrc
       - ./projects/gama_ui/.yarnrc:/app/.yarnrc
       - ./projects/gama_ui/cypress:/app/cypress
       - ./projects/gama_ui/cypress.json:/app/cypress.json
       - ./projects/gama_ui/index.html:/app/index.html
-      - ./projects/gama_ui/jest.config.js:/app/jest.config.js
+      - ./projects/gama_ui/jest.config.ts:/app/jest.config.ts
       - ./projects/gama_ui/package.json:/app/package.json
       - ./projects/gama_ui/public:/app/public
       - ./projects/gama_ui/src:/app/src
       - ./projects/gama_ui/tsconfig.json:/app/tsconfig.json
       - ./projects/gama_ui/typings:/app/typings
       - ./projects/gama_ui/vite.config.ts:/app/vite.config.ts
       - ./projects/gama_ui/yarn.lock:/app/yarn.lock
@@ -65,14 +65,19 @@
       - ./projects/gama_docs/yarn.lock:/app/yarn.lock
       - ./projects/gama_docs/sidebars.js:/app/sidebars.js
       - ./projects/gama_docs/docusaurus.config.js:/app/docusaurus.config.js
       - ./projects/gama_docs/tsconfig.json:/app/tsconfig.json
       - ./docs:/app/docs
     command: yarn start
 
+  gama_greenstream:
+    build:
+      context: .
+      dockerfile: projects/gama_greenstream/Dockerfile
+
 networks:
   vessel:
 
 secrets:
   API_TOKEN_GITHUB:
     file: ./.secrets/API_TOKEN_GITHUB
   apt_conf:
```

### Comparing `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml` & `gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml` & `gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -16,11 +16,15 @@
       dockerfile: projects/gama_vessel/Dockerfile
       args:
         - PACKAGE_NAME=whiskey_bravo_bringup
     environment:
       - LOG_STALE_MINUTES=43800 # in minutes
     command: ./scripts/launch.sh whiskey_bravo_bringup vessel.launch.py ${GAMA_VESSEL_COMMAND_ARGS:-}
 
+  gama_docs:
+    environment:
+      GAMA_VARIANT: whiskey_bravo
+
   gama_greenstream:
     devices:
       - /dev/video0
       - /dev/video2
```

### Comparing `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml` & `gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -15,7 +15,11 @@
     build:
       dockerfile: projects/gama_vessel/Dockerfile
       args:
         - PACKAGE_NAME=educat_bringup
     environment:
       - LOG_STALE_MINUTES=43800 # in minutes
     command: ./scripts/launch.sh educat_bringup vessel.launch.py ${GAMA_VESSEL_COMMAND_ARGS:-}
+
+  gama_docs:
+    environment:
+      GAMA_VARIANT: educat
```

### Comparing `gama_cli-1.9.0/gama_cli/docker/vessel/docker-compose.yaml` & `gama_cli-2.0.0/gama_cli/docker/vessel/docker-compose.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -63,18 +63,17 @@
     volumes:
       - /tmp/.X11-unix:/tmp/.X11-unix:rw
     networks:
       - vessel
 
   gama_greenstream:
     container_name: gama_greenstream
-    image: ghcr.io/greenroom-robotics/greenstream:1.2.2
+    image: ghcr.io/greenroom-robotics/gama_greenstream:${GAMA_VERSION:-latest}
     volumes:
-      - /tmp/.X11-unix:/tmp/.X11-unix:rw
-      - ./.gama/greenstream/${GREENSTREAM_CONFIG_FILE:-config.yaml}:/config.yml
+      - ./.gama:/home/.gama
     privileged: true
     network_mode: host
 
   gama_docs:
     container_name: gama_docs
     image: ghcr.io/greenroom-robotics/gama_docs:${GAMA_VERSION:-latest}
     ports:
```

### Comparing `gama_cli-1.9.0/gama_cli/groups/attach.py` & `gama_cli-2.0.0/gama_cli/groups/attach.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/groups/gs.py` & `gama_cli-2.0.0/gama_cli/groups/gs.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/groups/misc.py` & `gama_cli-2.0.0/gama_cli/groups/misc.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/groups/setup.py` & `gama_cli-2.0.0/gama_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli/groups/sim.py` & `gama_cli-2.0.0/gama_cli/groups/sim.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 DOCKER_ORG = "ghcr.io/greenroom-robotics"
 
 DOCKER_SIM_DEV = docker_compose_path("./sim/docker-compose.dev.yaml")
 DOCKER_SIM_STANDALONE = docker_compose_path("./sim/docker-compose.standalone.yaml")
 
 Mode: Enum = Enum("mode", ("dev", "standalone"))
-
-mode_default = "standalone"
+mode_default = "dev"
 mode_help = f"The mode to run the sim. Default: {mode_default}"
 
 
 def _get_compose_files(mode: str) -> List[ValidPath]:
     if mode == "dev":
         return [DOCKER_SIM_DEV]
     else:
@@ -43,16 +42,16 @@
     type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
     default=mode_default,
     help=mode_help,
 )
 @click.option(
     "-c",
     "--clean",
-    help="Should the ue4 build assets be cleaned?",
-    type=bool,
+    help="Should the UE project be cleaned?",
+    is_flag=True,
 )
 @click.argument("args", nargs=-1)
 def build(mode: str, clean: bool, args: List[str]):
     """Builds the sim"""
     # If building standalone, we first build the dev sim
     # TODO move this to a multistage build
 
@@ -73,49 +72,81 @@
     )
     docker_dev = DockerClient(
         compose_files=_get_compose_files("dev"),
         compose_project_directory=get_project_root(),
     )
 
     # build ue-dev container
-    docker_dev.compose.build()
+    docker_dev.compose.build(cache=True)
 
     if mode == "standalone":
         if clean:
             clean_command = """cd "${PROJECTS_HOME}/${PROJECT_NAME}" && ue4 clean && rm -rf dist"""
             docker_dev.compose.run("whiskey_ue", ["bash", "-c", clean_command])
 
         # run UE package command to compile and cook the UE project, making the `dist` directory
         ue_project_package_command = """cd "${PROJECTS_HOME}/${PROJECT_NAME}" && source ${ROS_OVERLAY}/setup.bash && ue4 package Development"""
         docker_dev.compose.run("whiskey_ue", ["bash", "-c", ue_project_package_command])
         docker_standalone.compose.build()
 
 
 @click.command(name="up")
 @click.option(
-    "--build",
-    type=bool,
-    default=False,
-    help="Should we rebuild the docker containers? Default: False",
-)
-@click.option(
     "-m",
     "--mode",
     type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
     default=mode_default,
     help=mode_help,
 )
+@click.option(
+    "--spin",
+    help="Sleep indefinitely instead of bringing up Unreal",
+    is_flag=True,
+)
 @click.argument("args", nargs=-1)
-def up(build: bool, mode: str, args: List[str]):
-    """Starts the sim"""
+def up(mode: str, spin: bool, args: List[str]):
+    """Starts the simulator"""
     docker = DockerClient(
         compose_files=_get_compose_files(mode),
         compose_project_directory=get_project_root(),
     )
-    docker.compose.up(detach=True, build=build)
+    if spin:
+        docker.compose.run(
+            "gama_sim_dev",
+            ["sleep", "inf"],
+            remove=True,
+        )
+    else:
+        docker.compose.up(detach=True)
+
+
+@click.command(name="compile")
+@click.option(
+    "-c",
+    "--clean",
+    help="Should the UE project be cleaned?",
+    is_flag=True,
+)
+def compile(clean: bool = False):
+    """Compile the UE project"""
+    docker = DockerClient(
+        compose_files=[DOCKER_SIM_DEV],
+        compose_project_directory=get_project_root(),
+    )
+    if clean:
+        docker.compose.run(
+            "gama_sim_dev",
+            ["bash", "--login", "-c", 'cd "${PROJECTS_HOME}/${PROJECT_NAME}" && ue4 clean'],
+            remove=True,
+        )
+    docker.compose.run(
+        "gama_sim_dev",
+        ["bash", "--login", "-c", 'cd "${PROJECTS_HOME}/${PROJECT_NAME}" && ue4 build'],
+        remove=True,
+    )
 
 
 @click.command(name="down")
 @click.option(
     "-m",
     "--mode",
     type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
@@ -132,31 +163,32 @@
     docker.compose.down()
 
 
 @click.command(name="base-ue")
 @click.option(
     "--ue-version",
     type=str,
-    default="4.27.2",
+    default="5.2.0",
     help="The release version of Unreal Engine to build",
 )
 @click.option(
     "--memory",
     type=str,
     default=None,
     help="Set maximum memory for the docker build",
 )
 def base_ue(ue_version: str, memory: str):
     """Builds the base Unreal Engine image for development"""
 
-    cuda_ver = "11.8.0"
+    cuda_ver = "12.1.1"
     ubuntu_ver = "22.04"
 
     args = ""
     if memory is not None:
         args += f" --memory {memory}"
 
-    # docker org has to be provided as long as we have to build our own cudagl images. requires https://github.com/adamrehn/ue4-docker/pull/276
+    # --ue-version {ue_version}
+
     call(
-        f"ue4-docker build {ue_version} --cuda={cuda_ver} -basetag=ubuntu{ubuntu_ver} -baseorg={DOCKER_ORG} -username={os.environ['GHCR_USERNAME']} -password={os.environ['API_TOKEN_GITHUB']}{args} --opt credential_mode=secrets --exclude ddc",
+        f"ue4-docker build {ue_version} --cuda={cuda_ver} -basetag=ubuntu{ubuntu_ver} -username={os.environ['GH_USERNAME']} -password={os.environ['API_TOKEN_GITHUB']}{args} --opt credential_mode=secrets --exclude ddc",
         env={"UE4DOCKER_TAG_NAMESPACE": DOCKER_ORG},
     )
```

### Comparing `gama_cli-1.9.0/gama_cli/groups/vessel.py` & `gama_cli-2.0.0/gama_cli/groups/vessel.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,16 @@
     docker_bake,
     get_gama_version,
     maybe_ignore_build,
     maybe_ignore_prod,
 )
 from python_on_whales.docker_client import DockerClient
 from python_on_whales.utils import ValidPath
-from pathlib import Path
-import shutil
 
 
-GREENSTREAM_CONFIG_DEST_PATH = Path(".") / ".gama" / "greenstream"
-GREENSTREAM_CONFIG_SOURCE_PATH = Path(__file__).parent.parent / "assets" / "greenstream"
-
 DOCKER_VESSEL = docker_compose_path("vessel/docker-compose.yaml")
 DOCKER_VESSEL_GPU = docker_compose_path("vessel/docker-compose.gpu.yaml")
 DOCKER_VESSEL_VARIANT_EDUCAT = docker_compose_path("vessel/docker-compose.variant-educat.yaml")
 DOCKER_VESSEL_VARIANT_BRAVO = docker_compose_path("vessel/docker-compose.variant-bravo.yaml")
 DOCKER_VESSEL_PROD = docker_compose_path("vessel/docker-compose.prod.yaml")
 DOCKER_VESSEL_DEV = docker_compose_path("vessel/docker-compose.dev.yaml")
 DOCKER_VESSEL_NETWORK_SHARED = docker_compose_path("vessel/docker-compose.network-shared.yaml")
@@ -76,28 +71,14 @@
         compose_files.append(DOCKER_VESSEL_NETWORK_HOST)
     if prod:
         compose_files.append(DOCKER_VESSEL_PROD)
 
     return compose_files
 
 
-def _get_greenstream_config(variant: Variant, mode: Mode):
-    if mode == Mode.STUBS:
-        return "config.stubs.yml"
-    if mode == Mode.SIMULATOR:
-        print("SIM VIDEO STREAMING NO LONGER SUPPORTED")
-        return "config.sim.yml"
-    if mode == Mode.HARDWARE:
-        if variant == Variant.WHISKEY_BRAVO:
-            return "config.variant.bravo.yml"
-        if variant == Variant.EDUCAT:
-            return "config.variant.educat.yml"
-    raise Exception("Invalid mode/variant combination")
-
-
 @click.group(help="Commands for the vessel")
 def vessel():
     pass
 
 
 @click.command(name="build")
 @click.argument(
@@ -276,15 +257,14 @@
         if getattr(config, field):
             vessel_launch_command_args += f" {field}:='{getattr(config, field)}'"
 
     os.environ["GAMA_VERSION"] = get_gama_version()
     os.environ["GAMA_VARIANT"] = config.variant.value
     os.environ["GAMA_VESSEL_COMMAND_ARGS"] = vessel_launch_command_args
     os.environ["LOOKOUT_COMMAND_ARGS"] = f"mode:='{config.mode.value}'"
-    os.environ["GREENSTREAM_CONFIG_FILE"] = _get_greenstream_config(config.variant, config.mode)
 
     services = (
         [service]
         if service
         else [
             "gama_ui",
             "gama_chart_tiler",
@@ -402,27 +382,7 @@
             log_level=click.prompt(
                 "Log level",
                 default=LogLevel.INFO,
                 type=click.Choice([item.value for item in LogLevel]),
             ),
         )
         write_vessel_config(config)
-
-    # Now that the GAMA config has been written. Let's write the greenstream config...
-    # Check if it exists
-    if os.path.exists(GREENSTREAM_CONFIG_DEST_PATH):
-        click.echo(
-            click.style(
-                f"Greenstream config already exists: {GREENSTREAM_CONFIG_DEST_PATH}",
-                fg="yellow",
-            )
-        )
-        result = click.prompt(
-            "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
-        )
-        if result == "n":
-            return
-
-    # Copy the directory from the assets. If it exists, it will be overwritten
-    shutil.copytree(
-        GREENSTREAM_CONFIG_SOURCE_PATH, GREENSTREAM_CONFIG_DEST_PATH, dirs_exist_ok=True
-    )
```

### Comparing `gama_cli-1.9.0/gama_cli/helpers.py` & `gama_cli-2.0.0/gama_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.9.0/gama_cli.egg-info/PKG-INFO` & `gama_cli-2.0.0/gama_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama-cli
-Version: 1.9.0
+Version: 2.0.0
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-1.9.0/gama_cli.egg-info/SOURCES.txt` & `gama_cli-2.0.0/gama_cli.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 gama_cli.egg-info/PKG-INFO
 gama_cli.egg-info/SOURCES.txt
 gama_cli.egg-info/dependency_links.txt
 gama_cli.egg-info/entry_points.txt
 gama_cli.egg-info/requires.txt
 gama_cli.egg-info/top_level.txt
 gama_cli.egg-info/zip-safe
-gama_cli/assets/greenstream/config.sim.yml
-gama_cli/assets/greenstream/config.stubs.yml
-gama_cli/assets/greenstream/config.variant.bravo.yml
-gama_cli/assets/greenstream/config.variant.educat.yml
 gama_cli/docker/gs/docker-compose.dev.yaml
 gama_cli/docker/gs/docker-compose.network-host.yaml
 gama_cli/docker/gs/docker-compose.network-shared.yaml
 gama_cli/docker/gs/docker-compose.network-vpn.yaml
 gama_cli/docker/gs/docker-compose.prod.yaml
 gama_cli/docker/gs/docker-compose.warthog-combo.yaml
 gama_cli/docker/gs/docker-compose.yaml
```

### Comparing `gama_cli-1.9.0/setup.cfg` & `gama_cli-2.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_cli
-version = 1.9.0
+version = 2.0.0
 url = https://github.com/Greenroom-Robotics/gama
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

