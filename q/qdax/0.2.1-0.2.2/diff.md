# Comparing `tmp/qdax-0.2.1.tar.gz` & `tmp/qdax-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdax-0.2.1.tar", last modified: Wed Dec  7 14:10:54 2022, max compression
+gzip compressed data, was "qdax-0.2.2.tar", last modified: Thu Mar 30 13:36:44 2023, max compression
```

## Comparing `qdax-0.2.1.tar` & `qdax-0.2.2.tar`

### file list

```diff
@@ -1,109 +1,116 @@
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.181643 qdax-0.2.1/
--rw-r--r--   0 looka      (501) staff       (20)     1112 2022-05-31 14:49:21.000000 qdax-0.2.1/LICENSE
--rw-r--r--   0 looka      (501) staff       (20)    12835 2022-12-07 14:10:54.181017 qdax-0.2.1/PKG-INFO
--rw-r--r--   0 looka      (501) staff       (20)    12029 2022-12-07 14:02:37.000000 qdax-0.2.1/README.md
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.137306 qdax-0.2.1/qdax/
--rw-r--r--   0 looka      (501) staff       (20)       22 2022-12-07 14:02:37.000000 qdax-0.2.1/qdax/__init__.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.144405 qdax-0.2.1/qdax/baselines/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-07-22 17:09:35.000000 qdax-0.2.1/qdax/baselines/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)    22764 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/baselines/dads.py
--rw-r--r--   0 looka      (501) staff       (20)     4718 2022-07-22 17:09:35.000000 qdax-0.2.1/qdax/baselines/dads_smerl.py
--rw-r--r--   0 looka      (501) staff       (20)    18948 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/baselines/diayn.py
--rw-r--r--   0 looka      (501) staff       (20)     4381 2022-07-22 17:09:35.000000 qdax-0.2.1/qdax/baselines/diayn_smerl.py
--rw-r--r--   0 looka      (501) staff       (20)     5633 2022-07-22 17:09:35.000000 qdax-0.2.1/qdax/baselines/genetic_algorithm.py
--rw-r--r--   0 looka      (501) staff       (20)     1857 2022-07-22 17:09:35.000000 qdax-0.2.1/qdax/baselines/nsga2.py
--rw-r--r--   0 looka      (501) staff       (20)    19039 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/baselines/sac.py
--rw-r--r--   0 looka      (501) staff       (20)     2266 2022-07-22 17:09:35.000000 qdax-0.2.1/qdax/baselines/spea2.py
--rw-r--r--   0 looka      (501) staff       (20)    13353 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/baselines/td3.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.146855 qdax-0.2.1/qdax/core/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-05-31 14:49:21.000000 qdax-0.2.1/qdax/core/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)    13237 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/cmaes.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.152326 qdax-0.2.1/qdax/core/containers/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-05-31 14:49:21.000000 qdax-0.2.1/qdax/core/containers/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)    11105 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/containers/archive.py
--rw-r--r--   0 looka      (501) staff       (20)     5804 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/core/containers/ga_repertoire.py
--rw-r--r--   0 looka      (501) staff       (20)    14273 2022-12-07 10:30:23.000000 qdax-0.2.1/qdax/core/containers/mapelites_repertoire.py
--rw-r--r--   0 looka      (501) staff       (20)    16246 2022-12-07 10:30:23.000000 qdax-0.2.1/qdax/core/containers/mome_repertoire.py
--rw-r--r--   0 looka      (501) staff       (20)     9413 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/core/containers/nsga2_repertoire.py
--rw-r--r--   0 looka      (501) staff       (20)     1319 2022-10-06 13:18:49.000000 qdax-0.2.1/qdax/core/containers/repertoire.py
--rw-r--r--   0 looka      (501) staff       (20)     4522 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/core/containers/spea2_repertoire.py
--rw-r--r--   0 looka      (501) staff       (20)     2735 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/containers/uniform_replacement_archive.py
--rw-r--r--   0 looka      (501) staff       (20)     7889 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/distributed_map_elites.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.160847 qdax-0.2.1/qdax/core/emitters/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-05-31 14:49:21.000000 qdax-0.2.1/qdax/core/emitters/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)    12944 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/cma_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     3041 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/cma_improvement_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)    10560 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/cma_mega_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     1617 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/cma_opt_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     5517 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/cma_pool_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     5806 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/cma_rnd_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)    12884 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/dpg_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     4877 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/emitter.py
--rw-r--r--   0 looka      (501) staff       (20)    26104 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/mees_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     7261 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/multi_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     7774 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/core/emitters/mutation_operators.py
--rw-r--r--   0 looka      (501) staff       (20)     9159 2022-12-07 10:30:23.000000 qdax-0.2.1/qdax/core/emitters/omg_mega_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     2898 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/pga_me_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     2317 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/qdpg_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)    20050 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/qpg_emitter.py
--rw-r--r--   0 looka      (501) staff       (20)     2853 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/emitters/standard_emitters.py
--rw-r--r--   0 looka      (501) staff       (20)     6367 2022-12-07 10:30:23.000000 qdax-0.2.1/qdax/core/map_elites.py
--rw-r--r--   0 looka      (501) staff       (20)     2612 2022-12-07 10:30:23.000000 qdax-0.2.1/qdax/core/mome.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.162444 qdax-0.2.1/qdax/core/neuroevolution/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-05-31 14:49:21.000000 qdax-0.2.1/qdax/core/neuroevolution/__init__.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.163549 qdax-0.2.1/qdax/core/neuroevolution/buffers/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-05-31 14:49:21.000000 qdax-0.2.1/qdax/core/neuroevolution/buffers/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)    12263 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/neuroevolution/buffers/buffer.py
--rw-r--r--   0 looka      (501) staff       (20)    12505 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/buffers/trajectory_buffer.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.165711 qdax-0.2.1/qdax/core/neuroevolution/losses/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-05-31 14:49:21.000000 qdax-0.2.1/qdax/core/neuroevolution/losses/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)     3094 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/losses/dads_loss.py
--rw-r--r--   0 looka      (501) staff       (20)     3415 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/losses/diayn_loss.py
--rw-r--r--   0 looka      (501) staff       (20)     4152 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/losses/sac_loss.py
--rw-r--r--   0 looka      (501) staff       (20)     3221 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/neuroevolution/losses/td3_loss.py
--rw-r--r--   0 looka      (501) staff       (20)     6856 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/core/neuroevolution/mdp_utils.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.168146 qdax-0.2.1/qdax/core/neuroevolution/networks/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-05-31 14:49:21.000000 qdax-0.2.1/qdax/core/neuroevolution/networks/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)     7339 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/networks/dads_networks.py
--rw-r--r--   0 looka      (501) staff       (20)     2570 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/networks/diayn_networks.py
--rw-r--r--   0 looka      (501) staff       (20)     2366 2022-08-17 12:03:33.000000 qdax-0.2.1/qdax/core/neuroevolution/networks/networks.py
--rw-r--r--   0 looka      (501) staff       (20)     1962 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/networks/sac_networks.py
--rw-r--r--   0 looka      (501) staff       (20)     1276 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/networks/td3_networks.py
--rw-r--r--   0 looka      (501) staff       (20)     1931 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/normalization_utils.py
--rw-r--r--   0 looka      (501) staff       (20)     4837 2022-07-14 22:50:30.000000 qdax-0.2.1/qdax/core/neuroevolution/sac_utils.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.171541 qdax-0.2.1/qdax/environments/
--rw-r--r--   0 looka      (501) staff       (20)     5626 2022-12-07 10:30:23.000000 qdax-0.2.1/qdax/environments/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)     3109 2022-08-01 16:40:26.000000 qdax-0.2.1/qdax/environments/base_wrappers.py
--rw-r--r--   0 looka      (501) staff       (20)     1264 2022-08-01 16:40:26.000000 qdax-0.2.1/qdax/environments/bd_extractors.py
--rw-r--r--   0 looka      (501) staff       (20)    12503 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/environments/exploration_wrappers.py
--rw-r--r--   0 looka      (501) staff       (20)     2146 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/environments/init_state_wrapper.py
--rw-r--r--   0 looka      (501) staff       (20)    10380 2022-10-11 16:11:37.000000 qdax-0.2.1/qdax/environments/locomotion_wrappers.py
--rw-r--r--   0 looka      (501) staff       (20)     9562 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/environments/pointmaze.py
--rw-r--r--   0 looka      (501) staff       (20)     2921 2022-11-01 13:24:49.000000 qdax-0.2.1/qdax/environments/wrappers.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.173832 qdax-0.2.1/qdax/tasks/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)     2569 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/arm.py
--rw-r--r--   0 looka      (501) staff       (20)    12173 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/brax_envs.py
--rw-r--r--   0 looka      (501) staff       (20)     2673 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/hypervolume_functions.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.176855 qdax-0.2.1/qdax/tasks/qd_suite/
--rw-r--r--   0 looka      (501) staff       (20)      952 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/qd_suite/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)     9188 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/qd_suite/archimedean_spiral.py
--rw-r--r--   0 looka      (501) staff       (20)     4736 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/qd_suite/deceptive_evolvability.py
--rw-r--r--   0 looka      (501) staff       (20)     2603 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/qd_suite/qd_suite_task.py
--rw-r--r--   0 looka      (501) staff       (20)     3697 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/qd_suite/ssf.py
--rw-r--r--   0 looka      (501) staff       (20)     3504 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/tasks/standard_functions.py
--rw-r--r--   0 looka      (501) staff       (20)     1037 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/types.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.180337 qdax-0.2.1/qdax/utils/
--rw-r--r--   0 looka      (501) staff       (20)        0 2022-05-31 14:49:21.000000 qdax-0.2.1/qdax/utils/__init__.py
--rw-r--r--   0 looka      (501) staff       (20)     4698 2022-10-06 13:18:49.000000 qdax-0.2.1/qdax/utils/metrics.py
--rw-r--r--   0 looka      (501) staff       (20)     4632 2022-07-22 17:09:35.000000 qdax-0.2.1/qdax/utils/pareto_front.py
--rw-r--r--   0 looka      (501) staff       (20)    26924 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/utils/plotting.py
--rw-r--r--   0 looka      (501) staff       (20)     2486 2022-12-01 14:18:14.000000 qdax-0.2.1/qdax/utils/sampling.py
-drwxr-xr-x   0 looka      (501) staff       (20)        0 2022-12-07 14:10:54.139217 qdax-0.2.1/qdax.egg-info/
--rw-r--r--   0 looka      (501) staff       (20)    12835 2022-12-07 14:10:54.000000 qdax-0.2.1/qdax.egg-info/PKG-INFO
--rw-r--r--   0 looka      (501) staff       (20)     3100 2022-12-07 14:10:54.000000 qdax-0.2.1/qdax.egg-info/SOURCES.txt
--rw-r--r--   0 looka      (501) staff       (20)       62 2022-12-07 14:10:54.000000 qdax-0.2.1/qdax.egg-info/dependency_links.txt
--rw-r--r--   0 looka      (501) staff       (20)      131 2022-12-07 14:10:54.000000 qdax-0.2.1/qdax.egg-info/requires.txt
--rw-r--r--   0 looka      (501) staff       (20)        5 2022-12-07 14:10:54.000000 qdax-0.2.1/qdax.egg-info/top_level.txt
--rw-r--r--   0 looka      (501) staff       (20)       38 2022-12-07 14:10:54.181779 qdax-0.2.1/setup.cfg
--rw-r--r--   0 looka      (501) staff       (20)     1577 2022-12-07 10:30:23.000000 qdax-0.2.1/setup.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.720307 qdax-0.2.2/
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1112 2022-08-04 20:48:21.000000 qdax-0.2.2/LICENSE
+-rw-r--r--   0 luca     (1000010) users    (1000001)    14697 2023-03-30 13:36:44.719307 qdax-0.2.2/PKG-INFO
+-rw-r--r--   0 luca     (1000010) users    (1000001)    13891 2023-03-30 13:35:01.000000 qdax-0.2.2/README.md
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:43.932318 qdax-0.2.2/qdax/
+-rw-r--r--   0 luca     (1000010) users    (1000001)       22 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/__init__.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.012317 qdax-0.2.2/qdax/baselines/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/baselines/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    22752 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/baselines/dads.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     4718 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/baselines/dads_smerl.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    18894 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/baselines/diayn.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     4381 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/baselines/diayn_smerl.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     5633 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/baselines/genetic_algorithm.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1857 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/baselines/nsga2.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     7049 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/baselines/pbt.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    23177 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/baselines/sac.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    16095 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/baselines/sac_pbt.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2266 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/baselines/spea2.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    16750 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/baselines/td3.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    18884 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/baselines/td3_pbt.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.066316 qdax-0.2.2/qdax/core/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    13237 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/cmaes.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.209314 qdax-0.2.2/qdax/core/containers/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/containers/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    11105 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/containers/archive.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     5804 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/containers/ga_repertoire.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    14315 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/containers/mapelites_repertoire.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    16273 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/containers/mome_repertoire.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     9413 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/containers/nsga2_repertoire.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1319 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/containers/repertoire.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     4522 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/containers/spea2_repertoire.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2735 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/containers/uniform_replacement_archive.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     7881 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/distributed_map_elites.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.504310 qdax-0.2.2/qdax/core/emitters/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/emitters/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    12944 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/cma_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3041 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/cma_improvement_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    10560 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/cma_mega_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1617 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/cma_opt_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     5517 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/cma_pool_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     5806 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/cma_rnd_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    12884 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/dpg_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     4877 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    26104 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/mees_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     7261 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/multi_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     7774 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/mutation_operators.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     9159 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/omg_mega_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    15387 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/emitters/pbt_me_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3516 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/emitters/pbt_variation_operators.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2898 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/pga_me_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2317 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/qdpg_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    20050 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/qpg_emitter.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2853 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/emitters/standard_emitters.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     6367 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/map_elites.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2612 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/mome.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.510310 qdax-0.2.2/qdax/core/neuroevolution/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/__init__.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.537310 qdax-0.2.2/qdax/core/neuroevolution/buffers/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/buffers/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    12263 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/core/neuroevolution/buffers/buffer.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    12505 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/buffers/trajectory_buffer.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.566309 qdax-0.2.2/qdax/core/neuroevolution/losses/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/losses/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3356 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/neuroevolution/losses/dads_loss.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3665 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/neuroevolution/losses/diayn_loss.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     6769 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/neuroevolution/losses/sac_loss.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     6285 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/neuroevolution/losses/td3_loss.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3547 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/neuroevolution/mdp_utils.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.581309 qdax-0.2.2/qdax/core/neuroevolution/networks/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/networks/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     7339 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/networks/dads_networks.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2570 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/networks/diayn_networks.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2366 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/networks/networks.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1962 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/networks/sac_networks.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1276 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/networks/td3_networks.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1931 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/core/neuroevolution/normalization_utils.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     4837 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/core/neuroevolution/sac_td3_utils.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.608309 qdax-0.2.2/qdax/environments/
+-rw-r--r--   0 luca     (1000010) users    (1000001)     6134 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/environments/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3109 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/environments/base_wrappers.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1264 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/environments/bd_extractors.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    12656 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/environments/exploration_wrappers.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    18893 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/environments/humanoidtrap.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2146 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/environments/init_state_wrapper.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    10412 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/environments/locomotion_wrappers.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     9562 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/environments/pointmaze.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2921 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/environments/wrappers.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.618309 qdax-0.2.2/qdax/tasks/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2569 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/arm.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    12139 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/tasks/brax_envs.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2673 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/hypervolume_functions.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     6058 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/tasks/jumanji_envs.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.641308 qdax-0.2.2/qdax/tasks/qd_suite/
+-rw-r--r--   0 luca     (1000010) users    (1000001)      952 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/qd_suite/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     9188 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/qd_suite/archimedean_spiral.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     4736 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/qd_suite/deceptive_evolvability.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2603 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/qd_suite/qd_suite_task.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3697 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/qd_suite/ssf.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3504 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/tasks/standard_functions.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1141 2023-03-30 13:35:01.000000 qdax-0.2.2/qdax/types.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:44.716307 qdax-0.2.2/qdax/utils/
+-rw-r--r--   0 luca     (1000010) users    (1000001)        0 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/utils/__init__.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     4698 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/utils/metrics.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     4632 2022-08-04 20:48:21.000000 qdax-0.2.2/qdax/utils/pareto_front.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)    26924 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/utils/plotting.py
+-rw-r--r--   0 luca     (1000010) users    (1000001)     2486 2023-01-23 19:39:43.000000 qdax-0.2.2/qdax/utils/sampling.py
+drwxr-xr-x   0 luca     (1000010) users    (1000001)        0 2023-03-30 13:36:43.939318 qdax-0.2.2/qdax.egg-info/
+-rw-r--r--   0 luca     (1000010) users    (1000001)    14697 2023-03-30 13:36:43.000000 qdax-0.2.2/qdax.egg-info/PKG-INFO
+-rw-r--r--   0 luca     (1000010) users    (1000001)     3322 2023-03-30 13:36:43.000000 qdax-0.2.2/qdax.egg-info/SOURCES.txt
+-rw-r--r--   0 luca     (1000010) users    (1000001)       62 2023-03-30 13:36:43.000000 qdax-0.2.2/qdax.egg-info/dependency_links.txt
+-rw-r--r--   0 luca     (1000010) users    (1000001)      159 2023-03-30 13:36:43.000000 qdax-0.2.2/qdax.egg-info/requires.txt
+-rw-r--r--   0 luca     (1000010) users    (1000001)        5 2023-03-30 13:36:43.000000 qdax-0.2.2/qdax.egg-info/top_level.txt
+-rw-r--r--   0 luca     (1000010) users    (1000001)       38 2023-03-30 13:36:44.720307 qdax-0.2.2/setup.cfg
+-rw-r--r--   0 luca     (1000010) users    (1000001)     1627 2023-03-30 13:35:01.000000 qdax-0.2.2/setup.py
```

### Comparing `qdax-0.2.1/LICENSE` & `qdax-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/PKG-INFO` & `qdax-0.2.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: qdax
-Version: 0.2.1
-Summary: A Python Library for Quality-Diversity and NeuroEvolution
-Home-page: https://github.com/adaptive-intelligent-robotics/QDax
-Author: AIRL and InstaDeep Ltd
-Author-email: adaptive.intelligent.robotics@gmail.com
-License: MIT
-Keywords: Quality-Diversity,NeuroEvolution,Reinforcement Learning,JAX
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 <img src="docs/img/qdax_logo.png" alt="qdax_logo" width="140"></img>
 </div>
 
 # QDax: Accelerated Quality-Diversity
 
 [![Documentation Status](https://readthedocs.org/projects/qdax/badge/?version=latest)](https://qdax.readthedocs.io/en/latest/?badge=latest)
@@ -138,37 +118,40 @@
 repertoire.genotypes, repertoire.fitnesses, repertoire.descriptors
 ```
 
 
 ## QDax core algorithms
 QDax currently supports the following algorithms:
 
-| Algorithm  | Example |
-| --- | --- |
-| [MAP-Elites](https://arxiv.org/abs/1504.04909) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mapelites.ipynb) |
-| [CVT MAP-Elites](https://arxiv.org/abs/1610.05729) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mapelites.ipynb) |
-| [Policy Gradient Assisted MAP-Elites (PGA-ME)](https://hal.archives-ouvertes.fr/hal-03135723v2/file/PGA_MAP_Elites_GECCO.pdf) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/pgame.ipynb) |
-| [QDPG](https://arxiv.org/abs/2006.08505) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/qdpg.ipynb) |
-| [CMA-ME](https://arxiv.org/pdf/1912.02400.pdf) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/cmame.ipynb) |
-| [OMG-MEGA](https://arxiv.org/abs/2106.03894) |  [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/omgmega.ipynb) |
-| [CMA-MEGA](https://arxiv.org/abs/2106.03894) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/cmamega.ipynb) |
-| [Multi-Objective MAP-Elites (MOME)](https://arxiv.org/abs/2202.03057) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mome.ipynb) |
-| [MAP-Elites Evolution Strategies (MEES)](https://dl.acm.org/doi/pdf/10.1145/3377930.3390217) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mees.ipynb) |
+| Algorithm                                                                                                                     | Example                                                                                                                                                                                         |
+|-------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [MAP-Elites](https://arxiv.org/abs/1504.04909)                                                                                | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mapelites.ipynb)  |
+| [CVT MAP-Elites](https://arxiv.org/abs/1610.05729)                                                                            | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mapelites.ipynb)  |
+| [Policy Gradient Assisted MAP-Elites (PGA-ME)](https://hal.archives-ouvertes.fr/hal-03135723v2/file/PGA_MAP_Elites_GECCO.pdf) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/pgame.ipynb)      |
+| [QDPG](https://arxiv.org/abs/2006.08505)                                                                                      | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/qdpg.ipynb)       |
+| [CMA-ME](https://arxiv.org/pdf/1912.02400.pdf)                                                                                | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/cmame.ipynb)      |
+| [OMG-MEGA](https://arxiv.org/abs/2106.03894)                                                                                  | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/omgmega.ipynb)    |
+| [CMA-MEGA](https://arxiv.org/abs/2106.03894)                                                                                  | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/cmamega.ipynb)    |
+| [Multi-Objective MAP-Elites (MOME)](https://arxiv.org/abs/2202.03057)                                                         | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mome.ipynb)       |
+| [MAP-Elites Evolution Strategies (MEES)](https://dl.acm.org/doi/pdf/10.1145/3377930.3390217)                                  | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mees.ipynb)       |
+| [MAP-Elites PBT (ME-PBT)](https://openreview.net/forum?id=CBfYffLqWqb)                                                        | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/me_sac_pbt.ipynb) |
+
 
 
 ## QDax baseline algorithms
 The QDax library also provides implementations for some useful baseline algorithms:
 
 | Algorithm  | Example |
 | --- | --- |
 | [DIAYN](https://arxiv.org/abs/1802.06070) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/diayn.ipynb) |
 | [DADS](https://arxiv.org/abs/1907.01657) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/dads.ipynb) |
 | [SMERL](https://arxiv.org/abs/2010.14484) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/smerl.ipynb) |
 | [NSGA2](https://ieeexplore.ieee.org/document/996017) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/nsga2_spea2.ipynb) |
 | [SPEA2](https://www.semanticscholar.org/paper/SPEA2%3A-Improving-the-strength-pareto-evolutionary-Zitzler-Laumanns/b13724cb54ae4171916f3f969d304b9e9752a57f) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/nsga2_spea2.ipynb) |
+| [Population Based Training (PBT)](https://arxiv.org/abs/1711.09846)                                                           | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/sac_pbt.ipynb)    |
 
 ## QDax Tasks
 The QDax library also provides numerous implementations for several standard Quality-Diversity tasks.
 
 All those implementations, and their descriptions are provided in the [tasks directory](./qdax/tasks).
 
 ## Contributing
```

### Comparing `qdax-0.2.1/README.md` & `qdax-0.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: qdax
+Version: 0.2.2
+Summary: A Python Library for Quality-Diversity and NeuroEvolution
+Home-page: https://github.com/adaptive-intelligent-robotics/QDax
+Author: AIRL and InstaDeep Ltd
+Author-email: adaptive.intelligent.robotics@gmail.com
+License: MIT
+Keywords: Quality-Diversity,NeuroEvolution,Reinforcement Learning,JAX
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 <img src="docs/img/qdax_logo.png" alt="qdax_logo" width="140"></img>
 </div>
 
 # QDax: Accelerated Quality-Diversity
 
 [![Documentation Status](https://readthedocs.org/projects/qdax/badge/?version=latest)](https://qdax.readthedocs.io/en/latest/?badge=latest)
@@ -118,37 +138,40 @@
 repertoire.genotypes, repertoire.fitnesses, repertoire.descriptors
 ```
 
 
 ## QDax core algorithms
 QDax currently supports the following algorithms:
 
-| Algorithm  | Example |
-| --- | --- |
-| [MAP-Elites](https://arxiv.org/abs/1504.04909) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mapelites.ipynb) |
-| [CVT MAP-Elites](https://arxiv.org/abs/1610.05729) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mapelites.ipynb) |
-| [Policy Gradient Assisted MAP-Elites (PGA-ME)](https://hal.archives-ouvertes.fr/hal-03135723v2/file/PGA_MAP_Elites_GECCO.pdf) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/pgame.ipynb) |
-| [QDPG](https://arxiv.org/abs/2006.08505) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/qdpg.ipynb) |
-| [CMA-ME](https://arxiv.org/pdf/1912.02400.pdf) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/cmame.ipynb) |
-| [OMG-MEGA](https://arxiv.org/abs/2106.03894) |  [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/omgmega.ipynb) |
-| [CMA-MEGA](https://arxiv.org/abs/2106.03894) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/cmamega.ipynb) |
-| [Multi-Objective MAP-Elites (MOME)](https://arxiv.org/abs/2202.03057) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mome.ipynb) |
-| [MAP-Elites Evolution Strategies (MEES)](https://dl.acm.org/doi/pdf/10.1145/3377930.3390217) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mees.ipynb) |
+| Algorithm                                                                                                                     | Example                                                                                                                                                                                         |
+|-------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [MAP-Elites](https://arxiv.org/abs/1504.04909)                                                                                | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mapelites.ipynb)  |
+| [CVT MAP-Elites](https://arxiv.org/abs/1610.05729)                                                                            | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mapelites.ipynb)  |
+| [Policy Gradient Assisted MAP-Elites (PGA-ME)](https://hal.archives-ouvertes.fr/hal-03135723v2/file/PGA_MAP_Elites_GECCO.pdf) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/pgame.ipynb)      |
+| [QDPG](https://arxiv.org/abs/2006.08505)                                                                                      | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/qdpg.ipynb)       |
+| [CMA-ME](https://arxiv.org/pdf/1912.02400.pdf)                                                                                | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/cmame.ipynb)      |
+| [OMG-MEGA](https://arxiv.org/abs/2106.03894)                                                                                  | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/omgmega.ipynb)    |
+| [CMA-MEGA](https://arxiv.org/abs/2106.03894)                                                                                  | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/cmamega.ipynb)    |
+| [Multi-Objective MAP-Elites (MOME)](https://arxiv.org/abs/2202.03057)                                                         | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mome.ipynb)       |
+| [MAP-Elites Evolution Strategies (MEES)](https://dl.acm.org/doi/pdf/10.1145/3377930.3390217)                                  | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/mees.ipynb)       |
+| [MAP-Elites PBT (ME-PBT)](https://openreview.net/forum?id=CBfYffLqWqb)                                                        | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/me_sac_pbt.ipynb) |
+
 
 
 ## QDax baseline algorithms
 The QDax library also provides implementations for some useful baseline algorithms:
 
 | Algorithm  | Example |
 | --- | --- |
 | [DIAYN](https://arxiv.org/abs/1802.06070) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/diayn.ipynb) |
 | [DADS](https://arxiv.org/abs/1907.01657) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/dads.ipynb) |
 | [SMERL](https://arxiv.org/abs/2010.14484) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/smerl.ipynb) |
 | [NSGA2](https://ieeexplore.ieee.org/document/996017) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/nsga2_spea2.ipynb) |
 | [SPEA2](https://www.semanticscholar.org/paper/SPEA2%3A-Improving-the-strength-pareto-evolutionary-Zitzler-Laumanns/b13724cb54ae4171916f3f969d304b9e9752a57f) | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/nsga2_spea2.ipynb) |
+| [Population Based Training (PBT)](https://arxiv.org/abs/1711.09846)                                                           | [![Open All Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adaptive-intelligent-robotics/QDax/blob/main/examples/sac_pbt.ipynb)    |
 
 ## QDax Tasks
 The QDax library also provides numerous implementations for several standard Quality-Diversity tasks.
 
 All those implementations, and their descriptions are provided in the [tasks directory](./qdax/tasks).
 
 ## Contributing
```

### Comparing `qdax-0.2.1/qdax/baselines/dads.py` & `qdax-0.2.2/qdax/baselines/dads.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 from qdax.core.neuroevolution.mdp_utils import TrainingState, get_first_episode
 from qdax.core.neuroevolution.networks.dads_networks import make_dads_networks
 from qdax.core.neuroevolution.normalization_utils import (
     RunningMeanStdState,
     normalize_with_rmstd,
     update_running_mean_std,
 )
-from qdax.core.neuroevolution.sac_utils import generate_unroll
-from qdax.environments import CompletedEvalWrapper
+from qdax.core.neuroevolution.sac_td3_utils import generate_unroll
 from qdax.types import Metrics, Params, Reward, RNGKey, Skill, StateDescriptor
 
 
 class DadsTrainingState(TrainingState):
     """Contains training state for the learner."""
 
     policy_optimizer_state: optax.OptState
@@ -84,16 +83,19 @@
         self._policy, self._critic, self._dynamics = make_dads_networks(
             action_size=action_size,
             descriptor_size=descriptor_size,
             omit_input_dynamics_dim=config.omit_input_dynamics_dim,
         )
 
         # define the action distribution
-        parametric_action_distribution = NormalTanhDistribution(event_size=action_size)
-        self._sample_action_fn = parametric_action_distribution.sample
+        self._action_size = action_size
+        self._parametric_action_distribution = NormalTanhDistribution(
+            event_size=action_size
+        )
+        self._sample_action_fn = self._parametric_action_distribution.sample
 
         # define the losses
         (
             self._alpha_loss_fn,
             self._policy_loss_fn,
             self._critic_loss_fn,
             self._dynamics_loss_fn,
@@ -101,15 +103,15 @@
             policy_fn=self._policy.apply,
             critic_fn=self._critic.apply,
             dynamics_fn=self._dynamics.apply,
             reward_scaling=self._config.reward_scaling,
             discount=self._config.discount,
             action_size=action_size,
             num_skills=self._config.num_skills,
-            parametric_action_distribution=parametric_action_distribution,
+            parametric_action_distribution=self._parametric_action_distribution,
         )
 
         # define the optimizers
         self._policy_optimizer = optax.adam(learning_rate=self._config.learning_rate)
         self._critic_optimizer = optax.adam(learning_rate=self._config.learning_rate)
         self._alpha_optimizer = optax.adam(learning_rate=self._config.learning_rate)
         self._dynamics_optimizer = optax.adam(learning_rate=self._config.learning_rate)
@@ -370,23 +372,17 @@
         state, training_state, transitions = generate_unroll(
             init_state=eval_env_first_state,
             training_state=training_state,
             episode_length=self._config.episode_length,
             play_step_fn=play_step_fn,
         )
 
-        eval_metrics_key = CompletedEvalWrapper.STATE_INFO_KEY
-        true_return = (
-            state.info[eval_metrics_key].completed_episodes_metrics["reward"]
-            / state.info[eval_metrics_key].completed_episodes
-        )
-
         transitions = get_first_episode(transitions)
-
         true_returns = jnp.nansum(transitions.rewards, axis=0)
+        true_return = jnp.mean(true_returns, axis=-1)
 
         reshaped_transitions = jax.tree_util.tree_map(
             lambda x: x.reshape((self._config.episode_length * env_batch_size, -1)),
             transitions,
         )
 
         if self._config.descriptor_full_state:
@@ -430,15 +426,15 @@
         """Update the dynamics network, independently of other networks. Called every
         `dynamics_update_freq` training steps.
         """
         training_state, transitions = operand
 
         dynamics_loss, dynamics_gradient = jax.value_and_grad(self._dynamics_loss_fn,)(
             training_state.dynamics_params,
-            transitions,
+            transitions=transitions,
         )
 
         (dynamics_updates, dynamics_optimizer_state,) = self._dynamics_optimizer.update(
             dynamics_gradient, training_state.dynamics_optimizer_state
         )
         dynamics_params = optax.apply_updates(
             training_state.dynamics_params, dynamics_updates
@@ -495,45 +491,45 @@
         # udpate alpha
         (
             alpha_params,
             alpha_optimizer_state,
             alpha_loss,
             random_key,
         ) = self._update_alpha(
+            alpha_lr=self._config.learning_rate,
             training_state=training_state,
             transitions=transitions,
             random_key=random_key,
         )
 
-        # use the previous alpha
-        alpha = jnp.exp(training_state.alpha_params)
-
         # update critic
         (
             critic_params,
             target_critic_params,
             critic_optimizer_state,
             critic_loss,
             random_key,
         ) = self._update_critic(
+            critic_lr=self._config.learning_rate,
+            reward_scaling=self._config.reward_scaling,
+            discount=self._config.discount,
             training_state=training_state,
-            alpha=alpha,
             transitions=transitions,
             random_key=random_key,
         )
 
         # update actor
         (
             policy_params,
             policy_optimizer_state,
             policy_loss,
             random_key,
         ) = self._update_actor(
+            policy_lr=self._config.learning_rate,
             training_state=training_state,
-            alpha=alpha,
             transitions=transitions,
             random_key=random_key,
         )
 
         # Create new training state
         new_training_state = DadsTrainingState(
             policy_optimizer_state=policy_optimizer_state,
@@ -550,15 +546,15 @@
             steps=training_state.steps + 1,
         )
         metrics = {
             "actor_loss": policy_loss,
             "critic_loss": critic_loss,
             "dynamics_loss": dynamics_loss,
             "alpha_loss": alpha_loss,
-            "alpha": alpha,
+            "alpha": jnp.exp(alpha_params),
             "training_observed_reward_mean": jnp.mean(transitions.rewards),
             "target_mean": jnp.mean(transitions.next_state_desc),
             "target_std": jnp.std(transitions.next_state_desc),
         }
 
         return new_training_state, metrics
```

### Comparing `qdax-0.2.1/qdax/baselines/dads_smerl.py` & `qdax-0.2.2/qdax/baselines/dads_smerl.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/baselines/diayn.py` & `qdax-0.2.2/qdax/baselines/diayn.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from brax.training.distribution import NormalTanhDistribution
 
 from qdax.baselines.sac import SAC, SacConfig
 from qdax.core.neuroevolution.buffers.buffer import QDTransition, ReplayBuffer
 from qdax.core.neuroevolution.losses.diayn_loss import make_diayn_loss_fn
 from qdax.core.neuroevolution.mdp_utils import TrainingState, get_first_episode
 from qdax.core.neuroevolution.networks.diayn_networks import make_diayn_networks
-from qdax.core.neuroevolution.sac_utils import generate_unroll
-from qdax.environments import CompletedEvalWrapper
+from qdax.core.neuroevolution.sac_td3_utils import generate_unroll
 from qdax.types import Metrics, Params, Reward, RNGKey, Skill, StateDescriptor
 
 
 class DiaynTrainingState(TrainingState):
     """Training state for the DIAYN algorithm"""
 
     policy_optimizer_state: optax.OptState
@@ -79,16 +78,19 @@
         self._policy, self._critic, self._discriminator = make_diayn_networks(
             num_skills=self._config.num_skills,
             action_size=action_size,
             hidden_layer_sizes=self._config.hidden_layer_sizes,
         )
 
         # define the action distribution
-        parametric_action_distribution = NormalTanhDistribution(event_size=action_size)
-        self._sample_action_fn = parametric_action_distribution.sample
+        self._action_size = action_size
+        self._parametric_action_distribution = NormalTanhDistribution(
+            event_size=action_size
+        )
+        self._sample_action_fn = self._parametric_action_distribution.sample
 
         # define the losses
         (
             self._alpha_loss_fn,
             self._policy_loss_fn,
             self._critic_loss_fn,
             self._discriminator_loss_fn,
@@ -96,15 +98,15 @@
             policy_fn=self._policy.apply,
             critic_fn=self._critic.apply,
             discriminator_fn=self._discriminator.apply,
             reward_scaling=self._config.reward_scaling,
             discount=self._config.discount,
             action_size=action_size,
             num_skills=self._config.num_skills,
-            parametric_action_distribution=parametric_action_distribution,
+            parametric_action_distribution=self._parametric_action_distribution,
         )
 
         # define the optimizers
         self._policy_optimizer = optax.adam(learning_rate=self._config.learning_rate)
         self._critic_optimizer = optax.adam(learning_rate=self._config.learning_rate)
         self._alpha_optimizer = optax.adam(learning_rate=self._config.learning_rate)
         self._discriminator_optimizer = optax.adam(
@@ -313,23 +315,17 @@
         state, training_state, transitions = generate_unroll(
             init_state=eval_env_first_state,
             training_state=training_state,
             episode_length=self._config.episode_length,
             play_step_fn=play_step_fn,
         )
 
-        eval_metrics_key = CompletedEvalWrapper.STATE_INFO_KEY
-        true_return = (
-            state.info[eval_metrics_key].completed_episodes_metrics["reward"]
-            / state.info[eval_metrics_key].completed_episodes
-        )
-
         transitions = get_first_episode(transitions)
-
-        true_return_per_env = jnp.nansum(transitions.rewards, axis=0)
+        true_returns = jnp.nansum(transitions.rewards, axis=0)
+        true_return = jnp.mean(true_returns, axis=-1)
 
         reshaped_transitions = jax.tree_util.tree_map(
             lambda x: x.reshape((self._config.episode_length * env_batch_size, -1)),
             transitions,
         )
 
         if self._config.descriptor_full_state:
@@ -346,15 +342,15 @@
             discriminator_params=training_state.discriminator_params,
         ).reshape((self._config.episode_length, env_batch_size))
 
         diversity_returns = jnp.nansum(diversity_rewards, axis=0)
 
         return (
             true_return,
-            true_return_per_env,
+            true_returns,
             diversity_returns,
             transitions.state_desc,
         )
 
     @partial(jax.jit, static_argnames=("self",))
     def _compute_reward(
         self, transition: QDTransition, training_state: DiaynTrainingState
@@ -414,45 +410,45 @@
         # udpate alpha
         (
             alpha_params,
             alpha_optimizer_state,
             alpha_loss,
             random_key,
         ) = self._update_alpha(
+            alpha_lr=self._config.learning_rate,
             training_state=training_state,
             transitions=transitions,
             random_key=random_key,
         )
 
-        # use the previous alpha
-        alpha = jnp.exp(training_state.alpha_params)
-
         # update critic
         (
             critic_params,
             target_critic_params,
             critic_optimizer_state,
             critic_loss,
             random_key,
         ) = self._update_critic(
+            critic_lr=self._config.learning_rate,
+            reward_scaling=self._config.reward_scaling,
+            discount=self._config.discount,
             training_state=training_state,
-            alpha=alpha,
             transitions=transitions,
             random_key=random_key,
         )
 
         # update actor
         (
             policy_params,
             policy_optimizer_state,
             policy_loss,
             random_key,
         ) = self._update_actor(
+            policy_lr=self._config.learning_rate,
             training_state=training_state,
-            alpha=alpha,
             transitions=transitions,
             random_key=random_key,
         )
 
         # Create new training state
         new_training_state = DiaynTrainingState(
             policy_optimizer_state=policy_optimizer_state,
```

### Comparing `qdax-0.2.1/qdax/baselines/diayn_smerl.py` & `qdax-0.2.2/qdax/baselines/diayn_smerl.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/baselines/genetic_algorithm.py` & `qdax-0.2.2/qdax/baselines/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/baselines/nsga2.py` & `qdax-0.2.2/qdax/baselines/nsga2.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/baselines/sac.py` & `qdax-0.2.2/qdax/baselines/td3.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,262 +1,256 @@
-"""
-A collection of functions and classes that define the algorithm Soft Actor Critic
-(SAC), ref: https://arxiv.org/abs/1801.01290
-"""
+""" Implements the TD3 algorithm in jax for brax environments, based on:
+https://arxiv.org/pdf/1802.09477.pdf"""
 
 from dataclasses import dataclass
 from functools import partial
 from typing import Callable, Tuple
 
 import jax
-import jax.numpy as jnp
 import optax
 from brax.envs import Env
 from brax.envs import State as EnvState
-from brax.training.distribution import NormalTanhDistribution
+from jax import numpy as jnp
 
-from qdax.core.neuroevolution.buffers.buffer import ReplayBuffer, Transition
-from qdax.core.neuroevolution.losses.sac_loss import make_sac_loss_fn
+from qdax.core.neuroevolution.buffers.buffer import (
+    QDTransition,
+    ReplayBuffer,
+    Transition,
+)
+from qdax.core.neuroevolution.losses.td3_loss import (
+    td3_critic_loss_fn,
+    td3_policy_loss_fn,
+)
 from qdax.core.neuroevolution.mdp_utils import TrainingState, get_first_episode
-from qdax.core.neuroevolution.networks.sac_networks import make_sac_networks
-from qdax.core.neuroevolution.normalization_utils import (
-    RunningMeanStdState,
-    normalize_with_rmstd,
-    update_running_mean_std,
+from qdax.core.neuroevolution.networks.td3_networks import make_td3_networks
+from qdax.core.neuroevolution.sac_td3_utils import generate_unroll
+from qdax.types import (
+    Action,
+    Descriptor,
+    Mask,
+    Metrics,
+    Observation,
+    Params,
+    Reward,
+    RNGKey,
 )
-from qdax.core.neuroevolution.sac_utils import generate_unroll
-from qdax.environments import CompletedEvalWrapper
-from qdax.types import Action, Metrics, Observation, Params, Reward, RNGKey
 
 
-class SacTrainingState(TrainingState):
-    """Training state for the SAC algorithm"""
+class TD3TrainingState(TrainingState):
+    """Contains training state for the learner."""
 
     policy_optimizer_state: optax.OptState
     policy_params: Params
     critic_optimizer_state: optax.OptState
     critic_params: Params
-    alpha_optimizer_state: optax.OptState
-    alpha_params: Params
     target_critic_params: Params
+    target_policy_params: Params
     random_key: RNGKey
     steps: jnp.ndarray
-    normalization_running_stats: RunningMeanStdState
 
 
 @dataclass
-class SacConfig:
-    """Configuration for the SAC algorithm."""
+class TD3Config:
+    """Configuration for the TD3 algorithm"""
 
-    batch_size: int
-    episode_length: int
-    grad_updates_per_step: float
-    tau: float = 0.005
-    normalize_observations: bool = False
-    learning_rate: float = 3e-4
-    alpha_init: float = 1.0
-    discount: float = 0.97
+    episode_length: int = 1000
+    batch_size: int = 256
+    policy_delay: int = 2
+    soft_tau_update: float = 0.005
+    expl_noise: float = 0.1
+    critic_hidden_layer_size: Tuple[int, ...] = (256, 256)
+    policy_hidden_layer_size: Tuple[int, ...] = (256, 256)
+    critic_learning_rate: float = 3e-4
+    policy_learning_rate: float = 3e-4
+    discount: float = 0.99
+    noise_clip: float = 0.5
+    policy_noise: float = 0.2
     reward_scaling: float = 1.0
-    hidden_layer_sizes: tuple = (256, 256)
-    fix_alpha: bool = False
 
 
-class SAC:
-    def __init__(self, config: SacConfig, action_size: int) -> None:
-        self._config = config
+class TD3:
+    """
+    A collection of functions that define the Twin Delayed Deep Deterministic Policy
+    Gradient agent (TD3), ref: https://arxiv.org/pdf/1802.09477.pdf
+    """
 
-        # define the networks
-        self._policy, self._critic = make_sac_networks(
-            action_size=action_size, hidden_layer_sizes=self._config.hidden_layer_sizes
-        )
+    def __init__(self, config: TD3Config, action_size: int):
+        self._config = config
 
-        # define the action distribution
-        parametric_action_distribution = NormalTanhDistribution(event_size=action_size)
-        self._sample_action_fn = parametric_action_distribution.sample
-
-        # define the losses
-        (
-            self._alpha_loss_fn,
-            self._policy_loss_fn,
-            self._critic_loss_fn,
-        ) = make_sac_loss_fn(
-            policy_fn=self._policy.apply,
-            critic_fn=self._critic.apply,
-            reward_scaling=self._config.reward_scaling,
-            discount=self._config.discount,
+        self._policy, self._critic, = make_td3_networks(
             action_size=action_size,
-            parametric_action_distribution=parametric_action_distribution,
+            critic_hidden_layer_sizes=self._config.critic_hidden_layer_size,
+            policy_hidden_layer_sizes=self._config.policy_hidden_layer_size,
         )
 
-        # define the optimizers
-        self._policy_optimizer = optax.adam(learning_rate=self._config.learning_rate)
-        self._critic_optimizer = optax.adam(learning_rate=self._config.learning_rate)
-        self._alpha_optimizer = optax.adam(learning_rate=self._config.learning_rate)
-
     def init(
         self, random_key: RNGKey, action_size: int, observation_size: int
-    ) -> SacTrainingState:
-        """Initialise the training state of the algorithm.
+    ) -> TD3TrainingState:
+        """Initialise the training state of the TD3 algorithm, through creation
+        of optimizer states and params.
 
         Args:
-            random_key: a jax random key
-            action_size: the size of the environment's action space
-            observation_size: the size of the environment's observation space
+            random_key: a random key used for random operations.
+            action_size: the size of the action array needed to interact with the
+                environment.
+            observation_size: the size of the observation array retrieved from the
+                environment.
 
         Returns:
-            the initial training state of SAC
+            the initial training state.
         """
 
-        # define policy and critic params
-        dummy_obs = jnp.zeros((1, observation_size))
-        dummy_action = jnp.zeros((1, action_size))
-
-        random_key, subkey = jax.random.split(random_key)
-        policy_params = self._policy.init(subkey, dummy_obs)
-
-        random_key, subkey = jax.random.split(random_key)
-        critic_params = self._critic.init(subkey, dummy_obs, dummy_action)
+        # Initialize critics and policy params
+        fake_obs = jnp.zeros(shape=(observation_size,))
+        fake_action = jnp.zeros(shape=(action_size,))
+        random_key, subkey_1, subkey_2 = jax.random.split(random_key, num=3)
+        critic_params = self._critic.init(subkey_1, obs=fake_obs, actions=fake_action)
+        policy_params = self._policy.init(subkey_2, fake_obs)
 
+        # Initialize target networks
         target_critic_params = jax.tree_util.tree_map(
             lambda x: jnp.asarray(x.copy()), critic_params
         )
+        target_policy_params = jax.tree_util.tree_map(
+            lambda x: jnp.asarray(x.copy()), policy_params
+        )
 
-        # define intitial optimizer states
-        policy_optimizer_state = self._policy_optimizer.init(policy_params)
-        critic_optimizer_state = self._critic_optimizer.init(critic_params)
-
-        log_alpha = jnp.asarray(jnp.log(self._config.alpha_init), dtype=jnp.float32)
-        alpha_optimizer_state = self._alpha_optimizer.init(log_alpha)
+        # Create and initialize optimizers
+        critic_optimizer_state = optax.adam(learning_rate=1.0).init(critic_params)
+        policy_optimizer_state = optax.adam(learning_rate=1.0).init(policy_params)
 
-        # create and retrieve the training state
-        training_state = SacTrainingState(
+        # Initial training state
+        training_state = TD3TrainingState(
             policy_optimizer_state=policy_optimizer_state,
             policy_params=policy_params,
             critic_optimizer_state=critic_optimizer_state,
             critic_params=critic_params,
-            alpha_optimizer_state=alpha_optimizer_state,
-            alpha_params=log_alpha,
+            target_policy_params=target_policy_params,
             target_critic_params=target_critic_params,
-            normalization_running_stats=RunningMeanStdState(
-                mean=jnp.zeros(
-                    observation_size,
-                ),
-                var=jnp.ones(
-                    observation_size,
-                ),
-                count=jnp.zeros(()),
-            ),
             random_key=random_key,
             steps=jnp.array(0),
         )
 
         return training_state
 
     @partial(jax.jit, static_argnames=("self", "deterministic"))
     def select_action(
         self,
         obs: Observation,
         policy_params: Params,
         random_key: RNGKey,
+        expl_noise: float,
         deterministic: bool = False,
     ) -> Tuple[Action, RNGKey]:
-        """Selects an action acording to SAC policy.
+        """Selects an action according to TD3 policy. The action can be deterministic
+        or stochastic by adding exploration noise.
 
         Args:
             obs: agent observation(s)
             policy_params: parameters of the agent's policy
             random_key: jax random key
-            deterministic: whether or not to select action in a deterministic way.
+            expl_noise: exploration noise
+            deterministic: whether to select action in a deterministic way.
                 Defaults to False.
 
         Returns:
-            The selected action and a new random key.
+            an action and an updated training state.
         """
 
-        dist_params = self._policy.apply(policy_params, obs)
+        actions = self._policy.apply(policy_params, obs)
         if not deterministic:
-            random_key, key_sample = jax.random.split(random_key)
-            actions = self._sample_action_fn(dist_params, key_sample)
-
-        else:
-            # The first half of parameters is for mean and the second half for variance
-            actions = jax.nn.tanh(dist_params[..., : dist_params.shape[-1] // 2])
-
+            random_key, subkey = jax.random.split(random_key)
+            noise = jax.random.normal(subkey, actions.shape) * expl_noise
+            actions = actions + noise
+            actions = jnp.clip(actions, -1.0, 1.0)
         return actions, random_key
 
-    @partial(jax.jit, static_argnames=("self", "env", "deterministic", "evaluation"))
+    @partial(jax.jit, static_argnames=("self", "env", "deterministic"))
     def play_step_fn(
         self,
         env_state: EnvState,
-        training_state: SacTrainingState,
+        training_state: TD3TrainingState,
         env: Env,
         deterministic: bool = False,
-        evaluation: bool = False,
-    ) -> Tuple[EnvState, SacTrainingState, Transition]:
-        """Plays a step in the environment. Selects an action according to SAC rule and
+    ) -> Tuple[EnvState, TD3TrainingState, Transition]:
+        """Plays a step in the environment. Selects an action according to TD3 rule and
         performs the environment step.
 
         Args:
             env_state: the current environment state
             training_state: the SAC training state
             env: the environment
-            deterministic: the whether or not to select action in a deterministic way.
+            deterministic: whether to select action in a deterministic way.
                 Defaults to False.
-            evaluation: if True, collected transitions are not used to update training
-                state. Defaults to False.
 
         Returns:
             the new environment state
-            the new SAC training state
+            the new TD3 training state
             the played transition
         """
-        random_key = training_state.random_key
-        policy_params = training_state.policy_params
-        obs = env_state.obs
-
-        if self._config.normalize_observations:
-            normalized_obs = normalize_with_rmstd(
-                obs, training_state.normalization_running_stats
-            )
-            normalization_running_stats = update_running_mean_std(
-                training_state.normalization_running_stats, obs
-            )
-
-        else:
-            normalized_obs = obs
-            normalization_running_stats = training_state.normalization_running_stats
 
         actions, random_key = self.select_action(
-            obs=normalized_obs,
-            policy_params=policy_params,
-            random_key=random_key,
+            obs=env_state.obs,
+            policy_params=training_state.policy_params,
+            random_key=training_state.random_key,
+            expl_noise=self._config.expl_noise,
             deterministic=deterministic,
         )
+        training_state = training_state.replace(
+            random_key=random_key,
+        )
+        next_env_state = env.step(env_state, actions)
+        transition = Transition(
+            obs=env_state.obs,
+            next_obs=next_env_state.obs,
+            rewards=next_env_state.reward,
+            dones=next_env_state.done,
+            truncations=next_env_state.info["truncation"],
+            actions=actions,
+        )
+        return next_env_state, training_state, transition
 
-        if not evaluation:
-            training_state = training_state.replace(
-                random_key=random_key,
-                normalization_running_stats=normalization_running_stats,
-            )
-        else:
-            training_state = training_state.replace(
-                random_key=random_key,
-            )
+    @partial(jax.jit, static_argnames=("self", "env", "deterministic"))
+    def play_qd_step_fn(
+        self,
+        env_state: EnvState,
+        training_state: TD3TrainingState,
+        env: Env,
+        deterministic: bool = False,
+    ) -> Tuple[EnvState, TD3TrainingState, QDTransition]:
+        """Plays a step in the environment. Selects an action according to TD3 rule and
+        performs the environment step.
 
-        next_env_state = env.step(env_state, actions)
-        next_obs = next_env_state.obs
+        Args:
+            env_state: the current environment state
+            training_state: the TD3 training state
+            env: the environment
+            deterministic: the whether to select action in a deterministic way.
+                Defaults to False.
+
+        Returns:
+            the new environment state
+            the new TD3 training state
+            the played transition
+        """
+        next_env_state, training_state, transition = self.play_step_fn(
+            env_state, training_state, env, deterministic
+        )
+        actions = transition.actions
 
         truncations = next_env_state.info["truncation"]
-        transition = Transition(
+        transition = QDTransition(
             obs=env_state.obs,
-            next_obs=next_obs,
+            next_obs=next_env_state.obs,
             rewards=next_env_state.reward,
             dones=next_env_state.done,
             actions=actions,
             truncations=truncations,
+            state_desc=env_state.info["state_descriptor"],
+            next_state_desc=next_env_state.info["state_descriptor"],
         )
 
         return (
             next_env_state,
             training_state,
             transition,
         )
@@ -266,282 +260,210 @@
         static_argnames=(
             "self",
             "play_step_fn",
         ),
     )
     def eval_policy_fn(
         self,
-        training_state: SacTrainingState,
+        training_state: TD3TrainingState,
         eval_env_first_state: EnvState,
         play_step_fn: Callable[
             [EnvState, Params, RNGKey],
-            Tuple[EnvState, SacTrainingState, Transition],
+            Tuple[EnvState, Params, RNGKey, Transition],
         ],
     ) -> Tuple[Reward, Reward]:
         """Evaluates the agent's policy over an entire episode, across all batched
         environments.
 
-
         Args:
-            training_state: the SAC training state
-            eval_env_first_state: the initial state for evaluation
-            play_step_fn: the play_step function used to collect the evaluation episode
+            training_state: TD3 training state.
+            eval_env_first_state: the first state of the environment.
+            play_step_fn: function defining how to play a step in the env.
 
         Returns:
-            the true return averaged over batch dimension, shape: (1,)
-            the true return per environment, shape: (env_batch_size,)
-
+            true return averaged over batch dimension, shape: (1,)
+            true return per env, shape: (env_batch_size,)
         """
-
+        # TODO: this generate unroll shouldn't take a random key
         state, training_state, transitions = generate_unroll(
             init_state=eval_env_first_state,
             training_state=training_state,
             episode_length=self._config.episode_length,
             play_step_fn=play_step_fn,
         )
 
-        eval_metrics_key = CompletedEvalWrapper.STATE_INFO_KEY
-        true_return = (
-            state.info[eval_metrics_key].completed_episodes_metrics["reward"]
-            / state.info[eval_metrics_key].completed_episodes
-        )
-
         transitions = get_first_episode(transitions)
 
         true_returns = jnp.nansum(transitions.rewards, axis=0)
+        true_return = jnp.mean(true_returns, axis=-1)
 
         return true_return, true_returns
 
-    @partial(jax.jit, static_argnames=("self"))
-    def _update_alpha(
+    @partial(
+        jax.jit,
+        static_argnames=(
+            "self",
+            "play_step_fn",
+            "bd_extraction_fn",
+        ),
+    )
+    def eval_qd_policy_fn(
         self,
-        training_state: SacTrainingState,
-        transitions: Transition,
-        random_key: RNGKey,
-    ) -> Tuple[Params, optax.OptState, jnp.ndarray, RNGKey]:
-        """Updates the alpha parameter if necessary. Else, it keeps the
-        current value.
+        training_state: TD3TrainingState,
+        eval_env_first_state: EnvState,
+        play_step_fn: Callable[
+            [EnvState, Params, RNGKey],
+            Tuple[EnvState, TD3TrainingState, QDTransition],
+        ],
+        bd_extraction_fn: Callable[[QDTransition, Mask], Descriptor],
+    ) -> Tuple[Reward, Descriptor, Reward, Descriptor]:
+        """Evaluates the agent's policy over an entire episode, across all batched
+        environments for QD environments. Averaged BDs are returned as well.
+
 
         Args:
-            training_state: the current training state.
-            transitions: a sample of transitions from the replay buffer.
-            random_key: a random key to handle stochastic operations.
+            training_state: the SAC training state
+            eval_env_first_state: the initial state for evaluation
+            play_step_fn: the play_step function used to collect the evaluation episode
 
         Returns:
-            New alpha params, optimizer state, loss and a new random key.
+            the true return averaged over batch dimension, shape: (1,)
+            the descriptor averaged over batch dimension, shape: (num_descriptors,)
+            the true return per environment, shape: (env_batch_size,)
+            the descriptor per environment, shape: (env_batch_size, num_descriptors)
+
         """
-        if not self._config.fix_alpha:
-            # update alpha
-            random_key, subkey = jax.random.split(random_key)
-            alpha_loss, alpha_gradient = jax.value_and_grad(self._alpha_loss_fn)(
-                training_state.alpha_params,
-                training_state.policy_params,
-                transitions=transitions,
-                random_key=subkey,
-            )
 
-            (alpha_updates, alpha_optimizer_state,) = self._alpha_optimizer.update(
-                alpha_gradient, training_state.alpha_optimizer_state
-            )
-            alpha_params = optax.apply_updates(
-                training_state.alpha_params, alpha_updates
-            )
-        else:
-            alpha_params = training_state.alpha_params
-            alpha_optimizer_state = training_state.alpha_optimizer_state
-            alpha_loss = jnp.array(0.0)
+        state, training_state, transitions = generate_unroll(
+            init_state=eval_env_first_state,
+            training_state=training_state,
+            episode_length=self._config.episode_length,
+            play_step_fn=play_step_fn,
+        )
+        transitions = get_first_episode(transitions)
+        true_returns = jnp.nansum(transitions.rewards, axis=0)
+        true_return = jnp.mean(true_returns, axis=-1)
+
+        transitions = jax.tree_util.tree_map(
+            lambda x: jnp.swapaxes(x, 0, 1), transitions
+        )
+        masks = jnp.isnan(transitions.rewards)
+        bds = bd_extraction_fn(transitions, masks)
 
-        return alpha_params, alpha_optimizer_state, alpha_loss, random_key
+        mean_bd = jnp.mean(bds, axis=0)
+        return true_return, mean_bd, true_returns, bds
 
-    @partial(jax.jit, static_argnames=("self"))
-    def _update_critic(
+    @partial(jax.jit, static_argnames=("self",))
+    def update(
         self,
-        training_state: SacTrainingState,
-        alpha: Params,
-        transitions: Transition,
-        random_key: RNGKey,
-    ) -> Tuple[Params, Params, optax.OptState, jnp.ndarray, RNGKey]:
-        """Updates the critic following the method described in the
-        Soft Actor Critic paper.
+        training_state: TD3TrainingState,
+        replay_buffer: ReplayBuffer,
+    ) -> Tuple[TD3TrainingState, ReplayBuffer, Metrics]:
+        """Performs a single training step: updates policy params and critic params
+        through gradient descent.
 
         Args:
-            training_state: the current training state.
-            alpha: the alpha parameter that controls the importance of
-                the entropy term.
-            transitions: a batch of transitions sampled from the replay buffer.
-            random_key: a random key to handle stochastic operations.
+            training_state: the current training state, containing the optimizer states
+                and the params of the policy and critic.
+            replay_buffer: the replay buffer, filled with transitions experienced in
+                the environment.
 
         Returns:
-            New parameters of the critic and its target. New optimizer state,
-            loss and a new random key.
+            A new training state, the buffer with new transitions and metrics about the
+            training process.
         """
-        # update critic
+
+        # Sample a batch of transitions in the buffer
+        random_key = training_state.random_key
+        samples, random_key = replay_buffer.sample(
+            random_key, sample_size=self._config.batch_size
+        )
+
+        # Update Critic
         random_key, subkey = jax.random.split(random_key)
-        critic_loss, critic_gradient = jax.value_and_grad(self._critic_loss_fn)(
+        critic_loss, critic_gradient = jax.value_and_grad(td3_critic_loss_fn)(
             training_state.critic_params,
-            training_state.policy_params,
-            training_state.target_critic_params,
-            alpha,
-            transitions=transitions,
+            target_policy_params=training_state.target_policy_params,
+            target_critic_params=training_state.target_critic_params,
+            policy_fn=self._policy.apply,
+            critic_fn=self._critic.apply,
+            policy_noise=self._config.policy_noise,
+            noise_clip=self._config.noise_clip,
+            reward_scaling=self._config.reward_scaling,
+            discount=self._config.discount,
+            transitions=samples,
             random_key=subkey,
         )
-
-        (critic_updates, critic_optimizer_state,) = self._critic_optimizer.update(
+        critic_optimizer = optax.adam(learning_rate=self._config.critic_learning_rate)
+        critic_updates, critic_optimizer_state = critic_optimizer.update(
             critic_gradient, training_state.critic_optimizer_state
         )
         critic_params = optax.apply_updates(
             training_state.critic_params, critic_updates
         )
+        # Soft update of target critic network
         target_critic_params = jax.tree_util.tree_map(
-            lambda x1, x2: (1.0 - self._config.tau) * x1 + self._config.tau * x2,
+            lambda x1, x2: (1.0 - self._config.soft_tau_update) * x1
+            + self._config.soft_tau_update * x2,
             training_state.target_critic_params,
             critic_params,
         )
 
-        return (
-            critic_params,
-            target_critic_params,
-            critic_optimizer_state,
-            critic_loss,
-            random_key,
-        )
-
-    @partial(jax.jit, static_argnames=("self"))
-    def _update_actor(
-        self,
-        training_state: SacTrainingState,
-        alpha: Params,
-        transitions: Transition,
-        random_key: RNGKey,
-    ) -> Tuple[Params, optax.OptState, jnp.ndarray, RNGKey]:
-        """Updates the actor parameters following the stochastic
-        policy gradient theorem with the method introduced in SAC.
-
-        Args:
-            training_state: the currrent training state.
-            alpha: the alpha parameter that controls the importance
-                of the entropy term.
-            transitions: a batch of transitions sampled from the replay
-                buffer.
-            random_key: a random key to handle stochastic operations.
-
-        Returns:
-            New params and optimizer state. Current loss. New random key.
-        """
-        random_key, subkey = jax.random.split(random_key)
-        policy_loss, policy_gradient = jax.value_and_grad(self._policy_loss_fn)(
+        # Update policy
+        policy_loss, policy_gradient = jax.value_and_grad(td3_policy_loss_fn)(
             training_state.policy_params,
-            training_state.critic_params,
-            alpha,
-            transitions=transitions,
-            random_key=subkey,
-        )
-        (policy_updates, policy_optimizer_state,) = self._policy_optimizer.update(
-            policy_gradient, training_state.policy_optimizer_state
-        )
-        policy_params = optax.apply_updates(
-            training_state.policy_params, policy_updates
-        )
-
-        return policy_params, policy_optimizer_state, policy_loss, random_key
-
-    @partial(jax.jit, static_argnames=("self"))
-    def update(
-        self,
-        training_state: SacTrainingState,
-        replay_buffer: ReplayBuffer,
-    ) -> Tuple[SacTrainingState, ReplayBuffer, Metrics]:
-        """Performs a training step to update the policy and the critic parameters.
-
-        Args:
-            training_state: the current SAC training state
-            replay_buffer: the replay buffer
-
-        Returns:
-            the updated SAC training state
-            the replay buffer
-            the training metrics
-        """
-
-        # sample a batch of transitions in the buffer
-        random_key = training_state.random_key
-        transitions, random_key = replay_buffer.sample(
-            random_key,
-            sample_size=self._config.batch_size,
+            critic_params=training_state.critic_params,
+            policy_fn=self._policy.apply,
+            critic_fn=self._critic.apply,
+            transitions=samples,
         )
 
-        # normalise observations if necessary
-        if self._config.normalize_observations:
-            normalization_running_stats = training_state.normalization_running_stats
-            normalized_obs = normalize_with_rmstd(
-                transitions.obs, normalization_running_stats
+        def update_policy_step() -> Tuple[Params, Params, optax.OptState]:
+            policy_optimizer = optax.adam(
+                learning_rate=self._config.policy_learning_rate
             )
-            normalized_next_obs = normalize_with_rmstd(
-                transitions.next_obs, normalization_running_stats
+            (policy_updates, policy_optimizer_state,) = policy_optimizer.update(
+                policy_gradient, training_state.policy_optimizer_state
             )
-            transitions = transitions.replace(
-                obs=normalized_obs, next_obs=normalized_next_obs
+            policy_params = optax.apply_updates(
+                training_state.policy_params, policy_updates
             )
+            # Soft update of target policy
+            target_policy_params = jax.tree_util.tree_map(
+                lambda x1, x2: (1.0 - self._config.soft_tau_update) * x1
+                + self._config.soft_tau_update * x2,
+                training_state.target_policy_params,
+                policy_params,
+            )
+            return policy_params, target_policy_params, policy_optimizer_state
 
-        # udpate alpha
-        (
-            alpha_params,
-            alpha_optimizer_state,
-            alpha_loss,
-            random_key,
-        ) = self._update_alpha(
-            training_state=training_state,
-            transitions=transitions,
-            random_key=random_key,
-        )
-
-        # use the previous alpha
-        alpha = jnp.exp(training_state.alpha_params)
-
-        # update critic
-        (
-            critic_params,
-            target_critic_params,
-            critic_optimizer_state,
-            critic_loss,
-            random_key,
-        ) = self._update_critic(
-            training_state=training_state,
-            alpha=alpha,
-            transitions=transitions,
-            random_key=random_key,
+        # Delayed update
+        current_policy_state = (
+            training_state.policy_params,
+            training_state.target_policy_params,
+            training_state.policy_optimizer_state,
         )
-
-        # update actor
-        (
-            policy_params,
-            policy_optimizer_state,
-            policy_loss,
-            random_key,
-        ) = self._update_actor(
-            training_state=training_state,
-            alpha=alpha,
-            transitions=transitions,
-            random_key=random_key,
+        policy_params, target_policy_params, policy_optimizer_state = jax.lax.cond(
+            training_state.steps % self._config.policy_delay == 0,
+            lambda _: update_policy_step(),
+            lambda _: current_policy_state,
+            operand=None,
         )
 
-        # create new training state
-        new_training_state = SacTrainingState(
-            policy_optimizer_state=policy_optimizer_state,
-            policy_params=policy_params,
-            critic_optimizer_state=critic_optimizer_state,
+        # Create new training state
+        new_training_state = training_state.replace(
             critic_params=critic_params,
-            alpha_optimizer_state=alpha_optimizer_state,
-            alpha_params=alpha_params,
-            normalization_running_stats=training_state.normalization_running_stats,
+            critic_optimizer_state=critic_optimizer_state,
+            policy_params=policy_params,
+            policy_optimizer_state=policy_optimizer_state,
             target_critic_params=target_critic_params,
+            target_policy_params=target_policy_params,
             random_key=random_key,
             steps=training_state.steps + 1,
         )
+
         metrics = {
             "actor_loss": policy_loss,
             "critic_loss": critic_loss,
-            "alpha_loss": alpha_loss,
-            "obs_mean": jnp.mean(transitions.obs),
-            "obs_std": jnp.std(transitions.obs),
         }
+
         return new_training_state, replay_buffer, metrics
```

### Comparing `qdax-0.2.1/qdax/baselines/spea2.py` & `qdax-0.2.2/qdax/baselines/spea2.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/cmaes.py` & `qdax-0.2.2/qdax/core/cmaes.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/containers/archive.py` & `qdax-0.2.2/qdax/core/containers/archive.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/containers/ga_repertoire.py` & `qdax-0.2.2/qdax/core/containers/ga_repertoire.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/containers/mapelites_repertoire.py` & `qdax-0.2.2/qdax/core/containers/mapelites_repertoire.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,16 @@
         Returns:
             an initialized MAP-Elite repertoire
         """
         warnings.warn(
             (
                 "This type of repertoire does not store the extra scores "
                 "computed by the scoring function"
-            )
+            ),
+            stacklevel=2,
         )
 
         # retrieve one genotype from the population
         first_genotype = jax.tree_util.tree_map(lambda x: x[0], genotypes)
 
         # create a repertoire with default values
         repertoire = cls.init_default(genotype=first_genotype, centroids=centroids)
@@ -382,15 +383,15 @@
         num_centroids = centroids.shape[0]
 
         # default fitness is -inf
         default_fitnesses = -jnp.inf * jnp.ones(shape=num_centroids)
 
         # default genotypes is all 0
         default_genotypes = jax.tree_util.tree_map(
-            lambda x: jnp.zeros(shape=(num_centroids,) + x.shape),
+            lambda x: jnp.zeros(shape=(num_centroids,) + x.shape, dtype=x.dtype),
             genotype,
         )
 
         # default descriptor is all zeros
         default_descriptors = jnp.zeros_like(centroids)
 
         return cls(
```

### Comparing `qdax-0.2.1/qdax/core/containers/mome_repertoire.py` & `qdax-0.2.2/qdax/core/containers/mome_repertoire.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,15 +385,16 @@
             An initialized MAP-Elite repertoire
         """
 
         warnings.warn(
             (
                 "This type of repertoire does not store the extra scores "
                 "computed by the scoring function"
-            )
+            ),
+            stacklevel=2,
         )
 
         # get dimensions
         num_criteria = fitnesses.shape[1]
         num_descriptors = descriptors.shape[1]
         num_centroids = centroids.shape[0]
```

### Comparing `qdax-0.2.1/qdax/core/containers/nsga2_repertoire.py` & `qdax-0.2.2/qdax/core/containers/nsga2_repertoire.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/containers/repertoire.py` & `qdax-0.2.2/qdax/core/containers/repertoire.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/containers/spea2_repertoire.py` & `qdax-0.2.2/qdax/core/containers/spea2_repertoire.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/containers/uniform_replacement_archive.py` & `qdax-0.2.2/qdax/core/containers/uniform_replacement_archive.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/distributed_map_elites.py` & `qdax-0.2.2/qdax/core/distributed_map_elites.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,16 @@
     @partial(jax.jit, static_argnames=("self",))
     def update(
         self,
         repertoire: MapElitesRepertoire,
         emitter_state: Optional[EmitterState],
         random_key: RNGKey,
     ) -> Tuple[MapElitesRepertoire, Optional[EmitterState], Metrics, RNGKey]:
-        """
-        Performs one iteration of the MAP-Elites algorithm.
+        """Performs one iteration of the MAP-Elites algorithm.
+
         1. A batch of genotypes is sampled in the repertoire and the genotypes
             are copied.
         2. The copies are mutated and crossed-over
         3. The obtained offsprings are scored and then added to the repertoire.
 
         Before the repertoire is updated, individuals are gathered from all the
         devices.
```

### Comparing `qdax-0.2.1/qdax/core/emitters/cma_emitter.py` & `qdax-0.2.2/qdax/core/emitters/cma_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/cma_improvement_emitter.py` & `qdax-0.2.2/qdax/core/emitters/cma_improvement_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/cma_mega_emitter.py` & `qdax-0.2.2/qdax/core/emitters/cma_mega_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/cma_opt_emitter.py` & `qdax-0.2.2/qdax/core/emitters/cma_opt_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/cma_pool_emitter.py` & `qdax-0.2.2/qdax/core/emitters/cma_pool_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/cma_rnd_emitter.py` & `qdax-0.2.2/qdax/core/emitters/cma_rnd_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/dpg_emitter.py` & `qdax-0.2.2/qdax/core/emitters/dpg_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/emitter.py` & `qdax-0.2.2/qdax/core/emitters/emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/mees_emitter.py` & `qdax-0.2.2/qdax/core/emitters/mees_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/multi_emitter.py` & `qdax-0.2.2/qdax/core/emitters/multi_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/mutation_operators.py` & `qdax-0.2.2/qdax/core/emitters/mutation_operators.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/omg_mega_emitter.py` & `qdax-0.2.2/qdax/core/emitters/omg_mega_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/pga_me_emitter.py` & `qdax-0.2.2/qdax/core/emitters/pga_me_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/qdpg_emitter.py` & `qdax-0.2.2/qdax/core/emitters/qdpg_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/qpg_emitter.py` & `qdax-0.2.2/qdax/core/emitters/qpg_emitter.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/emitters/standard_emitters.py` & `qdax-0.2.2/qdax/core/emitters/standard_emitters.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/map_elites.py` & `qdax-0.2.2/qdax/core/map_elites.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/mome.py` & `qdax-0.2.2/qdax/core/mome.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/buffers/buffer.py` & `qdax-0.2.2/qdax/core/neuroevolution/buffers/buffer.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/buffers/trajectory_buffer.py` & `qdax-0.2.2/qdax/core/neuroevolution/buffers/trajectory_buffer.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/losses/diayn_loss.py` & `qdax-0.2.2/qdax/core/neuroevolution/losses/diayn_loss.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 from typing import Callable, Tuple
 
 import jax
 import jax.numpy as jnp
 from brax.training.distribution import ParametricDistribution
 
 from qdax.core.neuroevolution.buffers.buffer import QDTransition
@@ -48,45 +49,54 @@
         critic_fn=critic_fn,
         reward_scaling=reward_scaling,
         discount=discount,
         action_size=action_size,
         parametric_action_distribution=parametric_action_distribution,
     )
 
-    @jax.jit
-    def _discriminator_loss_fn(
-        discriminator_params: Params,
-        transitions: QDTransition,
-    ) -> jnp.ndarray:
-        """Computes the loss used to train the discriminator. The
-        discriminator is trained to predict the skill that has been
-        used to generate transitions. In our case, skills are one
-        hot encoded, the discriminator is hence trained like a
-        multi-label classifier, using the categorical cross entropy
-        loss.
-
-        In this loss, log softmax outputs the log probabilities for
-        each skill. By multiplying by the skills (that are one hot
-        vectors), we filter to keep only the log probability of the
-        true skill.
-
-        Args:
-            discriminator_params: the parameters of the neural network
-                used to discriminate the skills.
-            transitions: the transitions sampled from the replay buffer.
-
-        Returns:
-            The loss of the discriminator on those transitions.
-        """
-
-        state_desc = transitions.state_desc
-        skills = transitions.obs[:, -num_skills:]
-        logits = jnp.sum(
-            jax.nn.log_softmax(discriminator_fn(discriminator_params, state_desc))
-            * skills,
-            axis=1,
-        )
-
-        loss = -jnp.mean(logits)
-        return loss
+    _discriminator_loss_fn = functools.partial(
+        diayn_discriminator_loss_fn,
+        discriminator_fn=discriminator_fn,
+        num_skills=num_skills,
+    )
 
     return _alpha_loss_fn, _policy_loss_fn, _critic_loss_fn, _discriminator_loss_fn
+
+
+def diayn_discriminator_loss_fn(
+    discriminator_params: Params,
+    discriminator_fn: Callable[[Params, StateDescriptor], jnp.ndarray],
+    num_skills: int,
+    transitions: QDTransition,
+) -> jnp.ndarray:
+    """Computes the loss used to train the discriminator. The
+    discriminator is trained to predict the skill that has been
+    used to generate transitions. In our case, skills are one
+    hot encoded, the discriminator is hence trained like a
+    multi-label classifier, using the categorical cross entropy
+    loss.
+
+    In this loss, log softmax outputs the log probabilities for
+    each skill. By multiplying by the skills (that are one hot
+    vectors), we filter to keep only the log probability of the
+    true skill.
+
+    Args:
+        discriminator_params: the parameters of the neural network
+            used to discriminate the skills.
+        discriminator_fn: the apply function of the discriminator.
+        num_skills: the number of skills.
+        transitions: the transitions sampled from the replay buffer.
+
+    Returns:
+        The loss of the discriminator on those transitions.
+    """
+
+    state_desc = transitions.state_desc
+    skills = transitions.obs[:, -num_skills:]
+    logits = jnp.sum(
+        jax.nn.log_softmax(discriminator_fn(discriminator_params, state_desc)) * skills,
+        axis=1,
+    )
+
+    loss = -jnp.mean(logits)
+    return loss
```

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/losses/td3_loss.py` & `qdax-0.2.2/qdax/core/neuroevolution/losses/dads_loss.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,97 @@
-""" Implements a function to create critic and actor losses for the TD3 algorithm."""
-
+import functools
 from typing import Callable, Tuple
 
-import jax
 import jax.numpy as jnp
+from brax.training.distribution import ParametricDistribution
 
-from qdax.core.neuroevolution.buffers.buffer import Transition
-from qdax.types import Action, Observation, Params, RNGKey
+from qdax.core.neuroevolution.buffers.buffer import QDTransition
+from qdax.core.neuroevolution.losses.sac_loss import make_sac_loss_fn
+from qdax.types import Action, Observation, Params, RNGKey, Skill, StateDescriptor
 
 
-def make_td3_loss_fn(
+def make_dads_loss_fn(
     policy_fn: Callable[[Params, Observation], jnp.ndarray],
     critic_fn: Callable[[Params, Observation, Action], jnp.ndarray],
+    dynamics_fn: Callable[
+        [Params, StateDescriptor, Skill, StateDescriptor], jnp.ndarray
+    ],
+    parametric_action_distribution: ParametricDistribution,
     reward_scaling: float,
     discount: float,
-    noise_clip: float,
-    policy_noise: float,
+    action_size: int,
+    num_skills: int,
 ) -> Tuple[
-    Callable[[Params, Params, Transition], jnp.ndarray],
-    Callable[[Params, Params, Params, Transition, RNGKey], jnp.ndarray],
+    Callable[[jnp.ndarray, Params, QDTransition, RNGKey], jnp.ndarray],
+    Callable[[Params, Params, jnp.ndarray, QDTransition, RNGKey], jnp.ndarray],
+    Callable[[Params, Params, Params, QDTransition, RNGKey], jnp.ndarray],
+    Callable[[Params, QDTransition, RNGKey], jnp.ndarray],
 ]:
-    """Creates the loss functions for TD3.
+    """Creates the loss used in DADS.
 
     Args:
-        policy_fn: forward pass through the neural network defining the policy.
-        critic_fn: forward pass through the neural network defining the critic.
-        reward_scaling: value to multiply the reward given by the environment.
-        discount: discount factor.
-        noise_clip: value that clips the noise to avoid extreme values.
-        policy_noise: noise applied to smooth the bootstrapping.
+        policy_fn: the apply function of the policy
+        critic_fn: the apply function of the critic
+        dynamics_fn: the apply function of the dynamics network
+        parametric_action_distribution: the distribution over action
+        reward_scaling: a multiplicative factor to the reward
+        discount: the discount factor
+        action_size: the size of the environment's action space
+        num_skills: the number of skills set
 
     Returns:
-        Return the loss functions used to train the policy and the critic in TD3.
+        the loss of the entropy parameter auto-tuning
+        the loss of the policy
+        the loss of the critic
+        the loss of the dynamics network
     """
 
-    @jax.jit
-    def _policy_loss_fn(
-        policy_params: Params,
-        critic_params: Params,
-        transitions: Transition,
-    ) -> jnp.ndarray:
-        """Policy loss function for TD3 agent"""
-
-        action = policy_fn(policy_params, transitions.obs)
-        q_value = critic_fn(
-            critic_params, obs=transitions.obs, actions=action  # type: ignore
-        )
-        q1_action = jnp.take(q_value, jnp.asarray([0]), axis=-1)
-        policy_loss = -jnp.mean(q1_action)
-        return policy_loss
-
-    @jax.jit
-    def _critic_loss_fn(
-        critic_params: Params,
-        target_policy_params: Params,
-        target_critic_params: Params,
-        transitions: Transition,
-        random_key: RNGKey,
-    ) -> jnp.ndarray:
-        """Critics loss function for TD3 agent"""
-        noise = (
-            jax.random.normal(random_key, shape=transitions.actions.shape)
-            * policy_noise
-        ).clip(-noise_clip, noise_clip)
-
-        next_action = (
-            policy_fn(target_policy_params, transitions.next_obs) + noise
-        ).clip(-1.0, 1.0)
-        next_q = critic_fn(  # type: ignore
-            target_critic_params, obs=transitions.next_obs, actions=next_action
-        )
-        next_v = jnp.min(next_q, axis=-1)
-        target_q = jax.lax.stop_gradient(
-            transitions.rewards * reward_scaling
-            + (1.0 - transitions.dones) * discount * next_v
-        )
-        q_old_action = critic_fn(  # type: ignore
-            critic_params,
-            obs=transitions.obs,
-            actions=transitions.actions,
-        )
-        q_error = q_old_action - jnp.expand_dims(target_q, -1)
-
-        # Better bootstrapping for truncated episodes.
-        q_error = q_error * jnp.expand_dims(1.0 - transitions.truncations, -1)
-
-        # compute the loss
-        q_losses = jnp.mean(jnp.square(q_error), axis=-2)
-        q_loss = jnp.sum(q_losses, axis=-1)
+    _alpha_loss_fn, _policy_loss_fn, _critic_loss_fn = make_sac_loss_fn(
+        policy_fn=policy_fn,
+        critic_fn=critic_fn,
+        reward_scaling=reward_scaling,
+        discount=discount,
+        action_size=action_size,
+        parametric_action_distribution=parametric_action_distribution,
+    )
+
+    _dynamics_loss_fn = functools.partial(
+        dads_dynamics_loss_fn, dynamics_fn=dynamics_fn, num_skills=num_skills
+    )
+
+    return _alpha_loss_fn, _policy_loss_fn, _critic_loss_fn, _dynamics_loss_fn
+
+
+def dads_dynamics_loss_fn(
+    dynamics_params: Params,
+    dynamics_fn: Callable[
+        [Params, StateDescriptor, Skill, StateDescriptor], jnp.ndarray
+    ],
+    num_skills: int,
+    transitions: QDTransition,
+) -> jnp.ndarray:
+    """Computes the loss used to train the dynamics network.
+
+    Args:
+        dynamics_params: the parameters of the neural network
+            used to predict the dynamics.
+        dynamics_fn: the apply function of the dynamics network
+        num_skills: the number of skills.
+        transitions: the batch of transitions used to train. They
+            have been sampled from a replay buffer beforehand.
 
-        return q_loss
+    Returns:
+        The loss obtained on the batch of transitions.
+    """
 
-    return _policy_loss_fn, _critic_loss_fn
+    active_skills = transitions.obs[:, -num_skills:]
+    target = transitions.next_state_desc
+    log_prob = dynamics_fn(  # type: ignore
+        dynamics_params,
+        obs=transitions.state_desc,
+        skill=active_skills,
+        target=target,
+    )
+
+    # prevent training on malformed target
+    loss = -jnp.mean(log_prob * (1 - transitions.dones))
+    return loss
```

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/networks/dads_networks.py` & `qdax-0.2.2/qdax/core/neuroevolution/networks/dads_networks.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/networks/diayn_networks.py` & `qdax-0.2.2/qdax/core/neuroevolution/networks/diayn_networks.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/networks/networks.py` & `qdax-0.2.2/qdax/core/neuroevolution/networks/networks.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/networks/sac_networks.py` & `qdax-0.2.2/qdax/core/neuroevolution/networks/sac_networks.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/networks/td3_networks.py` & `qdax-0.2.2/qdax/core/neuroevolution/networks/td3_networks.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/normalization_utils.py` & `qdax-0.2.2/qdax/core/neuroevolution/normalization_utils.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/core/neuroevolution/sac_utils.py` & `qdax-0.2.2/qdax/core/neuroevolution/sac_td3_utils.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/environments/__init__.py` & `qdax-0.2.2/qdax/environments/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,63 +6,72 @@
 
 from qdax.environments.base_wrappers import QDEnv, StateDescriptorResetWrapper
 from qdax.environments.bd_extractors import (
     get_feet_contact_proportion,
     get_final_xy_position,
 )
 from qdax.environments.exploration_wrappers import MazeWrapper, TrapWrapper
+from qdax.environments.humanoidtrap import HumanoidTrap
 from qdax.environments.init_state_wrapper import FixedInitialStateWrapper
 from qdax.environments.locomotion_wrappers import (
     FeetContactWrapper,
     NoForwardRewardWrapper,
     XYPositionWrapper,
 )
 from qdax.environments.pointmaze import PointMaze
 from qdax.environments.wrappers import CompletedEvalWrapper
 
 # experimentally determinated offset (except for antmaze)
 # should be sufficient to have only positive rewards but no guarantee
 reward_offset = {
     "pointmaze": 2.3431,
     "anttrap": 3.38,
+    "humanoidtrap": 0.0,
     "antnotrap": 3.38,
     "antmaze": 40.32,
     "ant_omni": 3.0,
     "humanoid_omni": 0.0,
     "ant_uni": 3.24,
     "humanoid_uni": 0.0,
     "halfcheetah_uni": 9.231,
     "hopper_uni": 0.9,
     "walker2d_uni": 1.413,
 }
 
 behavior_descriptor_extractor = {
     "pointmaze": get_final_xy_position,
     "anttrap": get_final_xy_position,
+    "humanoidtrap": get_final_xy_position,
     "antnotrap": get_final_xy_position,
     "antmaze": get_final_xy_position,
     "ant_omni": get_final_xy_position,
     "humanoid_omni": get_final_xy_position,
     "ant_uni": get_feet_contact_proportion,
     "humanoid_uni": get_feet_contact_proportion,
     "halfcheetah_uni": get_feet_contact_proportion,
     "hopper_uni": get_feet_contact_proportion,
     "walker2d_uni": get_feet_contact_proportion,
 }
 
 _qdax_envs = {
     "pointmaze": PointMaze,
+    "humanoid_w_trap": HumanoidTrap,
 }
 
 _qdax_custom_envs = {
     "anttrap": {
         "env": "ant",
         "wrappers": [XYPositionWrapper, TrapWrapper],
         "kwargs": [{"minval": [0.0, -8.0], "maxval": [30.0, 8.0]}, {}],
     },
+    "humanoidtrap": {
+        "env": "humanoid_w_trap",
+        "wrappers": [XYPositionWrapper],
+        "kwargs": [{"minval": [0.0, -8.0], "maxval": [30.0, 8.0]}],
+    },
     "antnotrap": {
         "env": "ant",
         "wrappers": [XYPositionWrapper],
         "kwargs": [{"minval": [0.0, -8.0], "maxval": [70.0, 8.0]}],
     },
     "antmaze": {
         "env": "ant",
@@ -121,15 +130,18 @@
 
     if env_name in brax.envs._envs.keys():
         env = brax.envs._envs[env_name](legacy_spring=True, **kwargs)
     elif env_name in _qdax_envs.keys():
         env = _qdax_envs[env_name](**kwargs)
     elif env_name in _qdax_custom_envs.keys():
         base_env_name = _qdax_custom_envs[env_name]["env"]
-        env = brax.envs._envs[base_env_name](legacy_spring=True, **kwargs)
+        if base_env_name in brax.envs._envs.keys():
+            env = brax.envs._envs[base_env_name](legacy_spring=True, **kwargs)
+        elif base_env_name in _qdax_envs.keys():
+            env = _qdax_envs[base_env_name](**kwargs)  # type: ignore
     else:
         raise NotImplementedError("This environment name does not exist!")
 
     if env_name in _qdax_custom_envs.keys():
         # roll with qdax wrappers
         wrappers = _qdax_custom_envs[env_name]["wrappers"]
         if qdax_wrappers_kwargs is None:
```

### Comparing `qdax-0.2.1/qdax/environments/base_wrappers.py` & `qdax-0.2.2/qdax/environments/base_wrappers.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/environments/bd_extractors.py` & `qdax-0.2.2/qdax/environments/bd_extractors.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/environments/exploration_wrappers.py` & `qdax-0.2.2/qdax/environments/exploration_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,18 @@
         if (
             env_name not in ENV_SYSTEM_CONFIG.keys()
             or env_name not in COG_NAMES.keys()
             or env_name not in ENV_TRAP_COLLISION.keys()
         ):
             raise NotImplementedError(f"This wrapper does not support {env_name} yet.")
         if env_name not in ["ant", "humanoid"]:
-            warnings.warn("Make sure your agent can move in two dimensions!")
+            warnings.warn(
+                "Make sure your agent can move in two dimensions!",
+                stacklevel=2,
+            )
         super().__init__(env)
         self._env_name = env_name
         # update the env config to add the trap
         self._config = (
             ENV_SYSTEM_CONFIG[env_name] + TRAP_CONFIG + ENV_TRAP_COLLISION[env_name]
         )
         # update the associated physical system
@@ -363,17 +366,22 @@
 
     def __init__(self, env: env.Env, env_name: str) -> None:
         if (
             env_name not in ENV_SYSTEM_CONFIG.keys()
             or env_name not in COG_NAMES.keys()
             or env_name not in ENV_MAZE_COLLISION.keys()
         ):
-            raise NotImplementedError(f"This wrapper does not support {env_name} yet.")
+            raise NotImplementedError(
+                f"This wrapper does not support {env_name} yet.",
+            )
         if env_name not in ["ant", "humanoid"]:
-            warnings.warn("Make sure your agent can move in two dimensions!")
+            warnings.warn(
+                "Make sure your agent can move in two dimensions!",
+                stacklevel=2,
+            )
         super().__init__(env)
         self._env_name = env_name
         self._config = (
             ENV_SYSTEM_CONFIG[env_name] + MAZE_CONFIG + ENV_MAZE_COLLISION[env_name]
         )
         config = text_format.Parse(self._config, brax.Config())
         if not hasattr(self.unwrapped, "sys"):
```

### Comparing `qdax-0.2.1/qdax/environments/init_state_wrapper.py` & `qdax-0.2.2/qdax/environments/init_state_wrapper.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/environments/locomotion_wrappers.py` & `qdax-0.2.2/qdax/environments/locomotion_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 # name of the center of gravity
 COG_NAMES = {
     "ant": "$ Torso",
     "halfcheetah": "torso",
     "walker2d": "torso",
     "hopper": "torso",
     "humanoid": "torso",
+    "humanoid_w_trap": "torso",
 }
 
 
 class XYPositionWrapper(QDEnv):
     """Wraps gym environments to add the position data.
 
     Utilisation is simple: create an environment with Brax, pass
```

### Comparing `qdax-0.2.1/qdax/environments/pointmaze.py` & `qdax-0.2.2/qdax/environments/pointmaze.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/environments/wrappers.py` & `qdax-0.2.2/qdax/environments/wrappers.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/tasks/arm.py` & `qdax-0.2.2/qdax/tasks/arm.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/tasks/brax_envs.py` & `qdax-0.2.2/qdax/tasks/brax_envs.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Fitness,
     Genotype,
     Params,
     RNGKey,
 )
 
 
-def create_policy_network_play_step_fn(
+def make_policy_network_play_step_fn_brax(
     env: brax.envs.Env,
     policy_network: nn.Module,
 ) -> Callable[
     [EnvState, Params, RNGKey], Tuple[EnvState, Params, RNGKey, QDTransition]
 ]:
     """
     Creates a function that when called, plays a step of the environment.
@@ -134,15 +134,15 @@
     _final_state, data = jax.vmap(unroll_fn)(init_states, policies_params)
 
     # create a mask to extract data properly
     is_done = jnp.clip(jnp.cumsum(data.dones, axis=1), 0, 1)
     mask = jnp.roll(is_done, 1, axis=1)
     mask = mask.at[:, 0].set(0)
 
-    # Scores - add offset to ensure positive fitness (through positive rewards)
+    # scores
     fitnesses = jnp.sum(data.rewards * (1.0 - mask), axis=1)
     descriptors = behavior_descriptor_extractor(data, mask)
 
     return (
         fitnesses,
         descriptors,
         {
@@ -195,15 +195,17 @@
         fitness: Array of fitnesses of all evaluated policies
         descriptor: Behavioural descriptors of all evaluated policies
         extra_scores: Additional information resulting from the evaluation
         random_key: The updated random key.
     """
 
     random_key, subkey = jax.random.split(random_key)
-    keys = jax.random.split(subkey, jax.tree_leaves(policies_params)[0].shape[0])
+    keys = jax.random.split(
+        subkey, jax.tree_util.tree_leaves(policies_params)[0].shape[0]
+    )
     reset_fn = jax.vmap(play_reset_fn)
     init_states = reset_fn(keys)
 
     fitnesses, descriptors, extra_scores, random_key = scoring_function_brax_envs(
         policies_params=policies_params,
         random_key=random_key,
         init_states=init_states,
@@ -237,30 +239,30 @@
 
     Args:
         env: The BRAX environment.
         policy_network: The policy network controller.
         bd_extraction_fn: The behaviour descriptor extraction function.
         random_key: a random key used for stochastic operations.
         play_step_fn: the function used to perform environment rollouts and collect
-            evaluation episodes. If None, we use create_policy_network_play_step_fn
+            evaluation episodes. If None, we use make_policy_network_play_step_fn_brax
             to generate it.
         episode_length: The maximal episode length.
         deterministic: Whether we reset the initial state of the robot to the same
             deterministic init_state or if we use the reset() function of the env.
         play_reset_fn: the function used to reset the environment to an initial state.
             Only used if deterministic is False. If None, we take env.reset as
             default reset function.
 
     Returns:
         The scoring function: a function that takes a batch of genotypes and compute
             their fitnesses and descriptors
         The updated random key.
     """
     if play_step_fn is None:
-        play_step_fn = create_policy_network_play_step_fn(env, policy_network)
+        play_step_fn = make_policy_network_play_step_fn_brax(env, policy_network)
 
     # Deterministic case
     if deterministic:
         # Create the initial environment states
         random_key, subkey = jax.random.split(random_key)
         init_state = env.reset(subkey)
```

### Comparing `qdax-0.2.1/qdax/tasks/hypervolume_functions.py` & `qdax-0.2.2/qdax/tasks/hypervolume_functions.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/tasks/qd_suite/__init__.py` & `qdax-0.2.2/qdax/tasks/qd_suite/__init__.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/tasks/qd_suite/archimedean_spiral.py` & `qdax-0.2.2/qdax/tasks/qd_suite/archimedean_spiral.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/tasks/qd_suite/deceptive_evolvability.py` & `qdax-0.2.2/qdax/tasks/qd_suite/deceptive_evolvability.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/tasks/qd_suite/qd_suite_task.py` & `qdax-0.2.2/qdax/tasks/qd_suite/qd_suite_task.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/tasks/qd_suite/ssf.py` & `qdax-0.2.2/qdax/tasks/qd_suite/ssf.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/tasks/standard_functions.py` & `qdax-0.2.2/qdax/tasks/standard_functions.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/types.py` & `qdax-0.2.2/qdax/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-"""Defines some types used in PaRL"""
+"""Defines some types used in QDax"""
 
 from typing import Dict, Generic, TypeVar, Union
 
 import brax.envs
 import jax
 import jax.numpy as jnp
+import jumanji
 from chex import ArrayTree
 from typing_extensions import TypeAlias
 
+JumanjiState: TypeAlias = ArrayTree
+JumanjiTimeStep: TypeAlias = jumanji.types.TimeStep
+
 # MDP types
 Observation: TypeAlias = jnp.ndarray
 Action: TypeAlias = jnp.ndarray
 Reward: TypeAlias = jnp.ndarray
 Done: TypeAlias = jnp.ndarray
 EnvState: TypeAlias = brax.envs.State
 Params: TypeAlias = ArrayTree
```

### Comparing `qdax-0.2.1/qdax/utils/metrics.py` & `qdax-0.2.2/qdax/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/utils/pareto_front.py` & `qdax-0.2.2/qdax/utils/pareto_front.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/utils/plotting.py` & `qdax-0.2.2/qdax/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax/utils/sampling.py` & `qdax-0.2.2/qdax/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `qdax-0.2.1/qdax.egg-info/SOURCES.txt` & `qdax-0.2.2/qdax.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 qdax/baselines/__init__.py
 qdax/baselines/dads.py
 qdax/baselines/dads_smerl.py
 qdax/baselines/diayn.py
 qdax/baselines/diayn_smerl.py
 qdax/baselines/genetic_algorithm.py
 qdax/baselines/nsga2.py
+qdax/baselines/pbt.py
 qdax/baselines/sac.py
+qdax/baselines/sac_pbt.py
 qdax/baselines/spea2.py
 qdax/baselines/td3.py
+qdax/baselines/td3_pbt.py
 qdax/core/__init__.py
 qdax/core/cmaes.py
 qdax/core/distributed_map_elites.py
 qdax/core/map_elites.py
 qdax/core/mome.py
 qdax/core/containers/__init__.py
 qdax/core/containers/archive.py
@@ -41,22 +44,24 @@
 qdax/core/emitters/cma_rnd_emitter.py
 qdax/core/emitters/dpg_emitter.py
 qdax/core/emitters/emitter.py
 qdax/core/emitters/mees_emitter.py
 qdax/core/emitters/multi_emitter.py
 qdax/core/emitters/mutation_operators.py
 qdax/core/emitters/omg_mega_emitter.py
+qdax/core/emitters/pbt_me_emitter.py
+qdax/core/emitters/pbt_variation_operators.py
 qdax/core/emitters/pga_me_emitter.py
 qdax/core/emitters/qdpg_emitter.py
 qdax/core/emitters/qpg_emitter.py
 qdax/core/emitters/standard_emitters.py
 qdax/core/neuroevolution/__init__.py
 qdax/core/neuroevolution/mdp_utils.py
 qdax/core/neuroevolution/normalization_utils.py
-qdax/core/neuroevolution/sac_utils.py
+qdax/core/neuroevolution/sac_td3_utils.py
 qdax/core/neuroevolution/buffers/__init__.py
 qdax/core/neuroevolution/buffers/buffer.py
 qdax/core/neuroevolution/buffers/trajectory_buffer.py
 qdax/core/neuroevolution/losses/__init__.py
 qdax/core/neuroevolution/losses/dads_loss.py
 qdax/core/neuroevolution/losses/diayn_loss.py
 qdax/core/neuroevolution/losses/sac_loss.py
@@ -67,22 +72,24 @@
 qdax/core/neuroevolution/networks/networks.py
 qdax/core/neuroevolution/networks/sac_networks.py
 qdax/core/neuroevolution/networks/td3_networks.py
 qdax/environments/__init__.py
 qdax/environments/base_wrappers.py
 qdax/environments/bd_extractors.py
 qdax/environments/exploration_wrappers.py
+qdax/environments/humanoidtrap.py
 qdax/environments/init_state_wrapper.py
 qdax/environments/locomotion_wrappers.py
 qdax/environments/pointmaze.py
 qdax/environments/wrappers.py
 qdax/tasks/__init__.py
 qdax/tasks/arm.py
 qdax/tasks/brax_envs.py
 qdax/tasks/hypervolume_functions.py
+qdax/tasks/jumanji_envs.py
 qdax/tasks/standard_functions.py
 qdax/tasks/qd_suite/__init__.py
 qdax/tasks/qd_suite/archimedean_spiral.py
 qdax/tasks/qd_suite/deceptive_evolvability.py
 qdax/tasks/qd_suite/qd_suite_task.py
 qdax/tasks/qd_suite/ssf.py
 qdax/utils/__init__.py
```

### Comparing `qdax-0.2.1/setup.py` & `qdax-0.2.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     description="A Python Library for Quality-Diversity and NeuroEvolution",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "absl-py>=1.0.0",
         "jax>=0.3.16",
         "jaxlib>=0.3.15",  # necessary to build the doc atm
+        "jinja2<3.1.0",
+        "jumanji>=0.1.3",
         "flax>=0.6, <0.6.2",
         "brax>=0.0.15",
         "gym>=0.23.1",
         "numpy>=1.22.3",
         "scikit-learn>=1.0.2",
         "scipy>=1.8.0",
     ],
```

