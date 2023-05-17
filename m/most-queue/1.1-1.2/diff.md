# Comparing `tmp/most-queue-1.1.tar.gz` & `tmp/most_queue-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "most-queue-1.1.tar", last modified: Mon May  8 07:41:53 2023, max compression
+gzip compressed data, was "most_queue-1.2.tar", last modified: Wed May 17 17:27:29 2023, max compression
```

## Comparing `most-queue-1.1.tar` & `most_queue-1.2.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.767445 most-queue-1.1/
--rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most-queue-1.1/LICENSE
--rw-rw-rw-   0        0        0      504 2023-05-08 07:41:53.766930 most-queue-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4326 2022-12-01 21:12:39.000000 most-queue-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.732009 most-queue-1.1/most_queue/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most-queue-1.1/most_queue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.740430 most-queue-1.1/most_queue/sim/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/sim/__init__.py
--rw-rw-rw-   0        0        0    14664 2022-09-15 16:47:38.000000 most-queue-1.1/most_queue/sim/fj_delta_im.py
--rw-rw-rw-   0        0        0    11132 2022-09-23 20:35:51.000000 most-queue-1.1/most_queue/sim/fj_im.py
--rw-rw-rw-   0        0        0    10099 2022-09-15 12:02:16.000000 most-queue-1.1/most_queue/sim/flow_sum_im.py
--rw-rw-rw-   0        0        0    10619 2022-12-01 20:31:07.000000 most-queue-1.1/most_queue/sim/network_im_prty.py
--rw-rw-rw-   0        0        0    13161 2022-11-30 19:30:09.000000 most-queue-1.1/most_queue/sim/queue_finite_source_sim.py
--rw-rw-rw-   0        0        0    37331 2023-01-25 13:05:08.000000 most-queue-1.1/most_queue/sim/rand_destribution.py
--rw-rw-rw-   0        0        0     3913 2022-11-30 19:31:29.000000 most-queue-1.1/most_queue/sim/smo_batch_sim.py
--rw-rw-rw-   0        0        0    25978 2022-11-30 17:51:13.000000 most-queue-1.1/most_queue/sim/smo_im.py
--rw-rw-rw-   0        0        0    39946 2022-09-25 20:15:14.000000 most-queue-1.1/most_queue/sim/smo_im_prty.py
--rw-rw-rw-   0        0        0     7724 2022-11-29 20:49:52.000000 most-queue-1.1/most_queue/sim/smo_impatient_im.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.749931 most-queue-1.1/most_queue/tests/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most-queue-1.1/most_queue/tests/__init__.py
--rw-rw-rw-   0        0        0     3826 2022-09-16 06:55:00.000000 most-queue-1.1/most_queue/tests/ek_d_n.py
--rw-rw-rw-   0        0        0     4997 2022-09-16 07:21:38.000000 most-queue-1.1/most_queue/tests/fj_calc.py
--rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most-queue-1.1/most_queue/tests/fj_im.py
--rw-rw-rw-   0        0        0     4262 2023-05-08 07:37:15.000000 most-queue-1.1/most_queue/tests/flow_sum.py
--rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most-queue-1.1/most_queue/tests/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most-queue-1.1/most_queue/tests/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most-queue-1.1/most_queue/tests/m_d_n_calc.py
--rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most-queue-1.1/most_queue/tests/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most-queue-1.1/most_queue/tests/mg1_calc.py
--rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most-queue-1.1/most_queue/tests/mg1_warm_calc.py
--rw-rw-rw-   0        0        0     4747 2023-05-08 07:36:11.000000 most-queue-1.1/most_queue/tests/mgn_tt.py
--rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most-queue-1.1/most_queue/tests/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most-queue-1.1/most_queue/tests/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most-queue-1.1/most_queue/tests/network_im_prty.py
--rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most-queue-1.1/most_queue/tests/passage_time.py
--rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most-queue-1.1/most_queue/tests/smo_im.py
--rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most-queue-1.1/most_queue/tests/smo_im_prty.py
--rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most-queue-1.1/most_queue/tests/weibull.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.764028 most-queue-1.1/most_queue/theory/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/theory/__init__.py
--rw-rw-rw-   0        0        0     2092 2022-09-15 12:02:16.000000 most-queue-1.1/most_queue/theory/approx_cdf_make.py
--rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most-queue-1.1/most_queue/theory/batch_mm1.py
--rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/theory/diff5dots.py
--rw-rw-rw-   0        0        0     6193 2022-09-15 16:51:31.000000 most-queue-1.1/most_queue/theory/ek_d_n_calc.py
--rw-rw-rw-   0        0        0     4760 2022-11-30 19:14:27.000000 most-queue-1.1/most_queue/theory/engset_model.py
--rw-rw-rw-   0        0        0    19414 2022-09-16 07:43:39.000000 most-queue-1.1/most_queue/theory/fj_calc.py
--rw-rw-rw-   0        0        0    10650 2022-09-15 16:54:06.000000 most-queue-1.1/most_queue/theory/flow_sum.py
--rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most-queue-1.1/most_queue/theory/generate_pareto_noise.py
--rw-rw-rw-   0        0        0     5943 2022-09-15 16:55:04.000000 most-queue-1.1/most_queue/theory/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     7888 2022-09-15 16:55:53.000000 most-queue-1.1/most_queue/theory/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most-queue-1.1/most_queue/theory/impatience_calc.py
--rw-rw-rw-   0        0        0     4474 2022-09-15 16:56:34.000000 most-queue-1.1/most_queue/theory/m_d_n_calc.py
--rw-rw-rw-   0        0        0    29777 2022-09-15 16:57:11.000000 most-queue-1.1/most_queue/theory/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     7316 2022-09-15 16:57:53.000000 most-queue-1.1/most_queue/theory/mg1_calc.py
--rw-rw-rw-   0        0        0     1625 2022-09-15 16:58:37.000000 most-queue-1.1/most_queue/theory/mg1_warm_calc.py
--rw-rw-rw-   0        0        0    22510 2022-09-20 18:47:52.000000 most-queue-1.1/most_queue/theory/mgn_tt.py
--rw-rw-rw-   0        0        0    18992 2022-09-15 17:02:09.000000 most-queue-1.1/most_queue/theory/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0    26829 2022-09-15 17:03:10.000000 most-queue-1.1/most_queue/theory/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     2010 2022-09-15 17:01:13.000000 most-queue-1.1/most_queue/theory/mmnr_calc.py
--rw-rw-rw-   0        0        0     5816 2022-09-23 20:42:20.000000 most-queue-1.1/most_queue/theory/network_calc.py
--rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most-queue-1.1/most_queue/theory/network_viewer.py
--rw-rw-rw-   0        0        0    40783 2022-09-15 17:04:24.000000 most-queue-1.1/most_queue/theory/passage_time.py
--rw-rw-rw-   0        0        0    17732 2022-09-15 17:05:30.000000 most-queue-1.1/most_queue/theory/prty_calc.py
--rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most-queue-1.1/most_queue/theory/q_poisson_arrival_calc.py
--rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/theory/student_stat.py
--rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/theory/sv_sum_calc.py
--rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most-queue-1.1/most_queue/theory/weibull.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.764584 most-queue-1.1/most_queue/visualisation/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most-queue-1.1/most_queue/visualisation/__init__.py
--rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most-queue-1.1/most_queue/visualisation/smo_im_vis.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.766430 most-queue-1.1/most_queue/visualisation/utils/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most-queue-1.1/most_queue/visualisation/utils/__init__.py
--rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most-queue-1.1/most_queue/visualisation/utils/result_table.py
--rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most-queue-1.1/most_queue/visualisation/utils/settings_window.py
--rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most-queue-1.1/most_queue/visualisation/utils/splash_screen.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.735552 most-queue-1.1/most_queue.egg-info/
--rw-rw-rw-   0        0        0      504 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2414 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most-queue-1.1/most_queue.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      105 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      508 2023-05-08 07:41:19.000000 most-queue-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 07:41:53.767445 most-queue-1.1/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-05-08 07:41:44.000000 most-queue-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.311880 most_queue-1.2/
+-rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.2/LICENSE
+-rw-rw-rw-   0        0        0     6336 2023-05-17 17:27:29.311880 most_queue-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.101980 most_queue-1.2/most_queue/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.2/most_queue/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.130440 most_queue-1.2/most_queue/sim/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/sim/__init__.py
+-rw-rw-rw-   0        0        0    14589 2023-05-17 17:16:20.000000 most_queue-1.2/most_queue/sim/fj_delta_im.py
+-rw-rw-rw-   0        0        0    11132 2022-09-23 20:35:51.000000 most_queue-1.2/most_queue/sim/fj_im.py
+-rw-rw-rw-   0        0        0    10099 2022-09-15 12:02:16.000000 most_queue-1.2/most_queue/sim/flow_sum_im.py
+-rw-rw-rw-   0        0        0    10619 2022-12-01 20:31:07.000000 most_queue-1.2/most_queue/sim/network_im_prty.py
+-rw-rw-rw-   0        0        0    13161 2022-11-30 19:30:09.000000 most_queue-1.2/most_queue/sim/queue_finite_source_sim.py
+-rw-rw-rw-   0        0        0    37331 2023-01-25 13:05:08.000000 most_queue-1.2/most_queue/sim/rand_destribution.py
+-rw-rw-rw-   0        0        0     3913 2022-11-30 19:31:29.000000 most_queue-1.2/most_queue/sim/smo_batch_sim.py
+-rw-rw-rw-   0        0        0    25978 2022-11-30 17:51:13.000000 most_queue-1.2/most_queue/sim/smo_im.py
+-rw-rw-rw-   0        0        0    39946 2022-09-25 20:15:14.000000 most_queue-1.2/most_queue/sim/smo_im_prty.py
+-rw-rw-rw-   0        0        0     7724 2022-11-29 20:49:52.000000 most_queue-1.2/most_queue/sim/smo_impatient_im.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.193428 most_queue-1.2/most_queue/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.2/most_queue/tests/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-05-17 17:18:04.000000 most_queue-1.2/most_queue/tests/ek_d_n.py
+-rw-rw-rw-   0        0        0     4997 2022-09-16 07:21:38.000000 most_queue-1.2/most_queue/tests/fj_calc.py
+-rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most_queue-1.2/most_queue/tests/fj_im.py
+-rw-rw-rw-   0        0        0     4278 2023-05-11 04:35:32.000000 most_queue-1.2/most_queue/tests/flow_sum.py
+-rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most_queue-1.2/most_queue/tests/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most_queue-1.2/most_queue/tests/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most_queue-1.2/most_queue/tests/m_d_n_calc.py
+-rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most_queue-1.2/most_queue/tests/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most_queue-1.2/most_queue/tests/mg1_calc.py
+-rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most_queue-1.2/most_queue/tests/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0     4747 2023-05-08 07:36:11.000000 most_queue-1.2/most_queue/tests/mgn_tt.py
+-rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most_queue-1.2/most_queue/tests/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most_queue-1.2/most_queue/tests/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most_queue-1.2/most_queue/tests/network_im_prty.py
+-rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most_queue-1.2/most_queue/tests/passage_time.py
+-rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most_queue-1.2/most_queue/tests/smo_im.py
+-rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most_queue-1.2/most_queue/tests/smo_im_prty.py
+-rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.2/most_queue/tests/weibull.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.297156 most_queue-1.2/most_queue/theory/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/theory/__init__.py
+-rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.2/most_queue/theory/batch_mm1.py
+-rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/theory/diff5dots.py
+-rw-rw-rw-   0        0        0     6193 2022-09-15 16:51:31.000000 most_queue-1.2/most_queue/theory/ek_d_n_calc.py
+-rw-rw-rw-   0        0        0     4719 2023-05-17 17:21:01.000000 most_queue-1.2/most_queue/theory/engset_model.py
+-rw-rw-rw-   0        0        0    19414 2022-09-16 07:43:39.000000 most_queue-1.2/most_queue/theory/fj_calc.py
+-rw-rw-rw-   0        0        0    10650 2022-09-15 16:54:06.000000 most_queue-1.2/most_queue/theory/flow_sum.py
+-rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.2/most_queue/theory/generate_pareto_noise.py
+-rw-rw-rw-   0        0        0     5943 2022-09-15 16:55:04.000000 most_queue-1.2/most_queue/theory/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     7888 2022-09-15 16:55:53.000000 most_queue-1.2/most_queue/theory/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.2/most_queue/theory/impatience_calc.py
+-rw-rw-rw-   0        0        0     4474 2022-09-15 16:56:34.000000 most_queue-1.2/most_queue/theory/m_d_n_calc.py
+-rw-rw-rw-   0        0        0    22232 2023-05-17 14:00:37.000000 most_queue-1.2/most_queue/theory/m_h2_h2warm.py
+-rw-rw-rw-   0        0        0    29777 2022-09-15 16:57:11.000000 most_queue-1.2/most_queue/theory/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     7316 2022-09-15 16:57:53.000000 most_queue-1.2/most_queue/theory/mg1_calc.py
+-rw-rw-rw-   0        0        0     1625 2022-09-15 16:58:37.000000 most_queue-1.2/most_queue/theory/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0    23133 2023-05-16 19:00:21.000000 most_queue-1.2/most_queue/theory/mgn_tt.py
+-rw-rw-rw-   0        0        0    18992 2022-09-15 17:02:09.000000 most_queue-1.2/most_queue/theory/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0    26829 2022-09-15 17:03:10.000000 most_queue-1.2/most_queue/theory/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     2010 2022-09-15 17:01:13.000000 most_queue-1.2/most_queue/theory/mmnr_calc.py
+-rw-rw-rw-   0        0        0     5816 2022-09-23 20:42:20.000000 most_queue-1.2/most_queue/theory/network_calc.py
+-rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.2/most_queue/theory/network_viewer.py
+-rw-rw-rw-   0        0        0    40783 2022-09-15 17:04:24.000000 most_queue-1.2/most_queue/theory/passage_time.py
+-rw-rw-rw-   0        0        0    17732 2022-09-15 17:05:30.000000 most_queue-1.2/most_queue/theory/prty_calc.py
+-rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.2/most_queue/theory/q_poisson_arrival_calc.py
+-rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/theory/student_stat.py
+-rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.2/most_queue/theory/sv_sum_calc.py
+-rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.2/most_queue/theory/weibull.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.299414 most_queue-1.2/most_queue/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.2/most_queue/utils/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.2/most_queue/utils/approx_cdf_make.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.300880 most_queue-1.2/most_queue/visualisation/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.2/most_queue/visualisation/__init__.py
+-rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.2/most_queue/visualisation/smo_im_vis.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.310819 most_queue-1.2/most_queue/visualisation/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.2/most_queue/visualisation/utils/__init__.py
+-rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.2/most_queue/visualisation/utils/result_table.py
+-rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.2/most_queue/visualisation/utils/settings_window.py
+-rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.2/most_queue/visualisation/utils/splash_screen.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:27:29.105404 most_queue-1.2/most_queue.egg-info/
+-rw-rw-rw-   0        0        0     6336 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2475 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.2/most_queue.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      105 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-17 17:27:29.000000 most_queue-1.2/most_queue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      508 2023-05-17 17:21:55.000000 most_queue-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 17:27:29.311880 most_queue-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      975 2023-05-17 17:25:23.000000 most_queue-1.2/setup.py
```

### Comparing `most-queue-1.1/LICENSE` & `most_queue-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/README.md` & `most_queue-1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 | 19.  | weibull | Selection of Weibull distribution parameters, calculation of CDF, PDF, Tail values |
 | 20.  | flow_sum | Flow summation, numerical calculation |
 | 21.  | impatience_calc | Calculation of M/M/1 with exponential impatience |
 | 22.  | batch_mm1 | Calculation of Queue M/M/1 with batch arrival |
 | 23.  | engset_model.py | Calculation of Queue M/M/1 with finite sources |
 | 24.  | generate_pareto_noise.py.py | Create noise by Pareto dist |
 | 25.  | network_viewer.py | Utility to view network structure |
+| 26.  | m_h2_h2warm.py | Multichannel queuing system with H2 service time and H2 warm-up. The system uses complex parameters, which allows you to calculate systems with arbitrary service time variation coefficients |
 ### Package .sim
 | #  | Pakage name | Description |
 | ------------- | ------------- |------------- |
 | 1.  | fj_delta_im | Simulation of Queue fork-join with a delay in the start of processing between channels | 
 | 2.  | fj_im | Simulation of Queue with fork-join process | 
 | 3.  | network_im_prty | Simulation of queuing network with priorities in nodes | 
 | 4.  | rand_destribution | A set of functions and classes designed to generate a PRNG and select parameters for distributions H2, C2, Ek, Pa, Gamma |
```

### Comparing `most-queue-1.1/most_queue/sim/fj_delta_im.py` & `most_queue-1.2/most_queue/sim/fj_delta_im.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import most_queue.sim.rand_destribution as rd
-from most_queue.sim.fj_im import SmoFJ as SmoFJ
-from most_queue.sim.fj_im import SubTask as SubTask
-from most_queue.sim.fj_im import Task as Task
-from most_queue.sim.smo_im import Server
+import rand_destribution as rd
+from fj_im import SmoFJ as SmoFJ
+from fj_im import SubTask as SubTask
+from fj_im import Task as Task
+from smo_im import Server
 from most_queue.theory import sv_sum_calc
 
 
 class ServerWarmUp(Server):
     """
     Канал обслуживания
     """
```

### Comparing `most-queue-1.1/most_queue/sim/fj_im.py` & `most_queue-1.2/most_queue/sim/fj_im.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/sim/flow_sum_im.py` & `most_queue-1.2/most_queue/sim/flow_sum_im.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/sim/network_im_prty.py` & `most_queue-1.2/most_queue/sim/network_im_prty.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/sim/queue_finite_source_sim.py` & `most_queue-1.2/most_queue/sim/queue_finite_source_sim.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/sim/rand_destribution.py` & `most_queue-1.2/most_queue/sim/rand_destribution.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/sim/smo_batch_sim.py` & `most_queue-1.2/most_queue/sim/smo_batch_sim.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/sim/smo_im.py` & `most_queue-1.2/most_queue/sim/smo_im.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/sim/smo_im_prty.py` & `most_queue-1.2/most_queue/sim/smo_im_prty.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/sim/smo_impatient_im.py` & `most_queue-1.2/most_queue/sim/smo_impatient_im.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/ek_d_n.py` & `most_queue-1.2/most_queue/tests/ek_d_n.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/fj_calc.py` & `most_queue-1.2/most_queue/tests/fj_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/fj_im.py` & `most_queue-1.2/most_queue/tests/fj_im.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/flow_sum.py` & `most_queue-1.2/most_queue/tests/flow_sum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from most_queue.theory.flow_sum import SummatorNumeric
-from .. sim import flow_sum_im
-from .. sim import rand_destribution as rd
+from most_queue.sim import flow_sum_im
+from most_queue.sim import rand_destribution as rd
 import matplotlib.pyplot as plt
 
 
 def test():
     """
     Тестирование суммирования потоков
     """
```

### Comparing `most-queue-1.1/most_queue/tests/gi_m_1_calc.py` & `most_queue-1.2/most_queue/tests/gi_m_1_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/gi_m_n_calc.py` & `most_queue-1.2/most_queue/tests/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/m_d_n_calc.py` & `most_queue-1.2/most_queue/tests/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/m_ph_n_prty.py` & `most_queue-1.2/most_queue/tests/m_ph_n_prty.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/mg1_calc.py` & `most_queue-1.2/most_queue/tests/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/mg1_warm_calc.py` & `most_queue-1.2/most_queue/tests/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/mgn_tt.py` & `most_queue-1.2/most_queue/tests/mgn_tt.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/mmn3_pnz_cox_approx.py` & `most_queue-1.2/most_queue/tests/mmn3_pnz_cox_approx.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/mmn_prty_pnz_approx.py` & `most_queue-1.2/most_queue/tests/mmn_prty_pnz_approx.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/network_im_prty.py` & `most_queue-1.2/most_queue/tests/network_im_prty.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/passage_time.py` & `most_queue-1.2/most_queue/tests/passage_time.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/smo_im.py` & `most_queue-1.2/most_queue/tests/smo_im.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/smo_im_prty.py` & `most_queue-1.2/most_queue/tests/smo_im_prty.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/tests/weibull.py` & `most_queue-1.2/most_queue/tests/weibull.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/approx_cdf_make.py` & `most_queue-1.2/most_queue/utils/approx_cdf_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import most_queue.sim.rand_destribution as rd
 import math
 from tqdm import tqdm
 import numpy as np
-import scipy
 import matplotlib.pyplot as plt
 
 
 # Входные данные
 
 b1 = 3      # мат. ожидание
 coev = 1.2  # коэффициент вариации
```

### Comparing `most-queue-1.1/most_queue/theory/batch_mm1.py` & `most_queue-1.2/most_queue/theory/batch_mm1.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/diff5dots.py` & `most_queue-1.2/most_queue/theory/diff5dots.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/ek_d_n_calc.py` & `most_queue-1.2/most_queue/theory/ek_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/engset_model.py` & `most_queue-1.2/most_queue/theory/engset_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import math
-from most_queue.theory.diff5dots import diff5dots
-from most_queue.theory import sv_sum_calc
+from diff5dots import diff5dots
+import sv_sum_calc
 
 
 class Engset:
     """
     Расчет СМО М\М\1 с конечным числом источников m
     """
```

### Comparing `most-queue-1.1/most_queue/theory/fj_calc.py` & `most_queue-1.2/most_queue/theory/fj_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/flow_sum.py` & `most_queue-1.2/most_queue/theory/flow_sum.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/generate_pareto_noise.py` & `most_queue-1.2/most_queue/theory/generate_pareto_noise.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/gi_m_1_calc.py` & `most_queue-1.2/most_queue/theory/gi_m_1_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/gi_m_n_calc.py` & `most_queue-1.2/most_queue/theory/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/impatience_calc.py` & `most_queue-1.2/most_queue/theory/impatience_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/m_d_n_calc.py` & `most_queue-1.2/most_queue/theory/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/m_ph_n_prty.py` & `most_queue-1.2/most_queue/theory/m_ph_n_prty.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/mg1_calc.py` & `most_queue-1.2/most_queue/theory/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/mg1_warm_calc.py` & `most_queue-1.2/most_queue/theory/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/mgn_tt.py` & `most_queue-1.2/most_queue/theory/mgn_tt.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
 
     def __init__(self, n, l, b, buffer=None, N=150, accuracy=1e-6, dtype="c16", verbose=False):
 
         """
         n: число каналов
         l: интенсивность вх. потока
-        h2_params: содержит список параметров H2-распределения [y1, mu1, mu2]
+        b: начальные моменты времени обслуживания
         N: число ярусов
         accuracy: точность, параметр для остановки итерации
         """
         self.dt = np.dtype(dtype)
         if buffer:
             self.R = buffer + n  # максимальное число заявок в сисетеме - очередь + каналы
             self.N = self.R + 1  # число ярусов на один больше + нулевое состояние
@@ -333,56 +333,81 @@
         """
         for i in range(self.N):
             self.A.append(self.buildA(i))
             self.B.append(self.buildB(i))
             self.C.append(self.buildC(i))
             self.D.append(self.buildD(i))
 
+    def calc_g_matrices(self):
+        self.G = []
+        for j in range(0, self.N):
+            self.G.append(np.linalg.inv(self.D[j] - self.C[j]))
+
+    def calc_ag_matrices(self):
+        self.AG = [0]
+        for j in range(1, self.N):
+            self.AG.append(np.dot(self.A[j - 1], self.G[j]))
+
+    def calc_bg_matrices(self):
+        self.BG = [0]
+        for j in range(1, self.N):
+            if j != (self.N - 1):
+                self.BG.append(np.dot(self.B[j + 1], self.G[j]))
+            else:
+                self.BG.append(np.dot(self.B[j], self.G[j]))
+
+    def calc_support_matrices(self):
+        self.calc_g_matrices()
+        self.calc_ag_matrices()
+        self.calc_bg_matrices()
+
     def run(self):
         """
         Запускает расчет
         """
         self.b1[0][0, 0] = 0.0 + 0.0j
         self.b2[0][0, 0] = 0.0 + 0.0j
         x_max1 = 0.0 + 0.0j
         x_max2 = 0.0 + 0.0j
+
+        self.calc_support_matrices()
+
+
         self.num_of_iter_ = 0  # кол-во итераций алгоритма
         for i in range(self.N):
             if self.x[i].real > x_max1.real:
                 x_max1 = self.x[i]
 
         while math.fabs(x_max2.real - x_max1.real) >= self.e1:
             x_max2 = x_max1
             self.num_of_iter_ += 1
 
             for j in range(1, self.N):  # по всем ярусам, кроме первого.
 
-                G = np.linalg.inv(self.D[j] - self.C[j])
-
                 # b':
-                self.b1[j] = np.dot(self.t[j - 1], np.dot(self.A[j - 1], G))
+                self.b1[j] = np.dot(self.t[j - 1], self.AG[j])
 
                 # b":
                 if j != (self.N - 1):
-                    self.b2[j] = np.dot(self.t[j + 1], np.dot(self.B[j + 1], G))
+                    self.b2[j] = np.dot(self.t[j + 1], self.BG[j])
                 else:
-                    self.b2[j] = np.dot(self.t[j - 1], np.dot(self.B[j], G))
+                    self.b2[j] = np.dot(self.t[j - 1], self.BG[j])
 
                 c = self.calculate_c(j)
 
                 x_znam = np.dot(c, self.b1[j]) + self.b2[j]
                 self.x[j] = 0.0 + 0.0j
                 for k in range(x_znam.shape[1]):
                     self.x[j] += x_znam[0, k]
 
                 self.x[j] = (1.0 + 0.0j) / self.x[j]
 
                 if self.R and j == (self.N - 1):
                     tA = np.dot(self.t[j - 1], self.A[j - 1])
-                    tag = np.dot(tA, G)
+                    tag = np.dot(tA, self.G[j])
                     tag_sum = 0
                     for t_i in range(tag.shape[1]):
                         tag_sum += tag[0, t_i]
                     self.z[j] = 1.0 / tag_sum
                     self.t[j] = self.z[j] * tag
 
                 else:
@@ -390,15 +415,15 @@
                     self.z[j] = np.dot(c, self.x[j])
                     self.t[j] = np.dot(self.z[j], self.b1[j]) + np.dot(self.x[j], self.b2[j])
 
             self.x[0] = (1.0 + 0.0j) / self.z[1]
 
             t1B1 = np.dot(self.t[1], self.B[1])
             self.t[0] = np.dot(self.x[0], t1B1)
-            self.t[0] = np.dot(self.t[0], np.linalg.inv(self.D[0] - self.C[0]))
+            self.t[0] = np.dot(self.t[0], self.G[0])
 
             x_max1 = 0.0 + 0.0j
 
             for i in range(self.N):
                 if self.x[i].real > x_max1.real:
                     x_max1 = self.x[i]
```

### Comparing `most-queue-1.1/most_queue/theory/mmn3_pnz_cox_approx.py` & `most_queue-1.2/most_queue/theory/mmn3_pnz_cox_approx.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/mmn_prty_pnz_approx.py` & `most_queue-1.2/most_queue/theory/mmn_prty_pnz_approx.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/mmnr_calc.py` & `most_queue-1.2/most_queue/theory/mmnr_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/network_calc.py` & `most_queue-1.2/most_queue/theory/network_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/network_viewer.py` & `most_queue-1.2/most_queue/theory/network_viewer.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/passage_time.py` & `most_queue-1.2/most_queue/theory/passage_time.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/prty_calc.py` & `most_queue-1.2/most_queue/theory/prty_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/q_poisson_arrival_calc.py` & `most_queue-1.2/most_queue/theory/q_poisson_arrival_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/student_stat.py` & `most_queue-1.2/most_queue/theory/student_stat.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/sv_sum_calc.py` & `most_queue-1.2/most_queue/theory/sv_sum_calc.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/theory/weibull.py` & `most_queue-1.2/most_queue/theory/weibull.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/visualisation/smo_im_vis.py` & `most_queue-1.2/most_queue/visualisation/smo_im_vis.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/visualisation/utils/result_table.py` & `most_queue-1.2/most_queue/visualisation/utils/result_table.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/visualisation/utils/settings_window.py` & `most_queue-1.2/most_queue/visualisation/utils/settings_window.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue/visualisation/utils/splash_screen.py` & `most_queue-1.2/most_queue/visualisation/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `most-queue-1.1/most_queue.egg-info/SOURCES.txt` & `most_queue-1.2/most_queue.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,26 @@
 most_queue/tests/mmn_prty_pnz_approx.py
 most_queue/tests/network_im_prty.py
 most_queue/tests/passage_time.py
 most_queue/tests/smo_im.py
 most_queue/tests/smo_im_prty.py
 most_queue/tests/weibull.py
 most_queue/theory/__init__.py
-most_queue/theory/approx_cdf_make.py
 most_queue/theory/batch_mm1.py
 most_queue/theory/diff5dots.py
 most_queue/theory/ek_d_n_calc.py
 most_queue/theory/engset_model.py
 most_queue/theory/fj_calc.py
 most_queue/theory/flow_sum.py
 most_queue/theory/generate_pareto_noise.py
 most_queue/theory/gi_m_1_calc.py
 most_queue/theory/gi_m_n_calc.py
 most_queue/theory/impatience_calc.py
 most_queue/theory/m_d_n_calc.py
+most_queue/theory/m_h2_h2warm.py
 most_queue/theory/m_ph_n_prty.py
 most_queue/theory/mg1_calc.py
 most_queue/theory/mg1_warm_calc.py
 most_queue/theory/mgn_tt.py
 most_queue/theory/mmn3_pnz_cox_approx.py
 most_queue/theory/mmn_prty_pnz_approx.py
 most_queue/theory/mmnr_calc.py
@@ -63,13 +63,15 @@
 most_queue/theory/network_viewer.py
 most_queue/theory/passage_time.py
 most_queue/theory/prty_calc.py
 most_queue/theory/q_poisson_arrival_calc.py
 most_queue/theory/student_stat.py
 most_queue/theory/sv_sum_calc.py
 most_queue/theory/weibull.py
+most_queue/utils/__init__.py
+most_queue/utils/approx_cdf_make.py
 most_queue/visualisation/__init__.py
 most_queue/visualisation/smo_im_vis.py
 most_queue/visualisation/utils/__init__.py
 most_queue/visualisation/utils/result_table.py
 most_queue/visualisation/utils/settings_window.py
 most_queue/visualisation/utils/splash_screen.py
```

### Comparing `most-queue-1.1/setup.py` & `most_queue-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='most-queue',
-      version='1.01',
+      version='1.02',
       description="Software package for calculation and simulation of queuing systems",
       author='Xabarov Roman',
       author_email='xabarov1985@gmail.com',
       url='https://github.com/xabarov/mps',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
```

