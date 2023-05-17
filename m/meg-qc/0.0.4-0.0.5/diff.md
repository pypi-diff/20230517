# Comparing `tmp/meg_qc-0.0.4.tar.gz` & `tmp/meg_qc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meg_qc-0.0.4.tar", last modified: Thu May 11 13:15:23 2023, max compression
+gzip compressed data, was "meg_qc-0.0.5.tar", last modified: Wed May 17 14:23:10 2023, max compression
```

## Comparing `meg_qc-0.0.4.tar` & `meg_qc-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:15:23.698626 meg_qc-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-11 13:15:11.000000 meg_qc-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-11 13:15:23.698626 meg_qc-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-11 13:15:11.000000 meg_qc-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:15:23.698626 meg_qc-0.0.4/meg_qc/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 13:15:11.000000 meg_qc-0.0.4/meg_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-11 13:15:11.000000 meg_qc-0.0.4/meg_qc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-11 13:15:23.698626 meg_qc-0.0.4/meg_qc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17943 2023-05-11 13:15:11.000000 meg_qc-0.0.4/meg_qc/meg_qc_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:15:23.698626 meg_qc-0.0.4/meg_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-11 13:15:23.000000 meg_qc-0.0.4/meg_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-11 13:15:23.000000 meg_qc-0.0.4/meg_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:15:23.000000 meg_qc-0.0.4/meg_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 13:15:23.000000 meg_qc-0.0.4/meg_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 13:15:11.000000 meg_qc-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-11 13:15:23.698626 meg_qc-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-11 13:15:11.000000 meg_qc-0.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-11 13:15:11.000000 meg_qc-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:10.229741 meg_qc-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-17 14:22:51.000000 meg_qc-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-17 14:23:10.229741 meg_qc-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-17 14:22:51.000000 meg_qc-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:10.229741 meg_qc-0.0.5/meg_qc/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 14:22:51.000000 meg_qc-0.0.5/meg_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-17 14:22:51.000000 meg_qc-0.0.5/meg_qc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 14:23:10.229741 meg_qc-0.0.5/meg_qc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-17 14:22:51.000000 meg_qc-0.0.5/meg_qc/meg_qc_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:23:10.229741 meg_qc-0.0.5/meg_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-17 14:23:10.000000 meg_qc-0.0.5/meg_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-17 14:23:10.000000 meg_qc-0.0.5/meg_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:23:10.000000 meg_qc-0.0.5/meg_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 14:23:10.000000 meg_qc-0.0.5/meg_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 14:22:51.000000 meg_qc-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-17 14:23:10.229741 meg_qc-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-17 14:22:51.000000 meg_qc-0.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-17 14:22:51.000000 meg_qc-0.0.5/versioneer.py
```

### Comparing `meg_qc-0.0.4/LICENSE` & `meg_qc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meg_qc-0.0.4/PKG-INFO` & `meg_qc-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg_qc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/ANCPLabOldenburg/MEG-QC-code
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.0.4/README.md` & `meg_qc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `meg_qc-0.0.4/meg_qc/__main__.py` & `meg_qc-0.0.5/meg_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.0.4/meg_qc/meg_qc_pipeline.py` & `meg_qc-0.0.5/meg_qc/meg_qc_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,21 +174,22 @@
 
                 if all_qc_params['default']['run_ECG'] is True:
                     print('___MEG QC___: ', 'Starting ECG...')
                     start_time = time.time()
                     ecg_derivs, simple_metrics_ecg, ecg_str, avg_objects_ecg = ECG_meg_qc(all_qc_params['ECG'], raw_cropped, channels, chs_by_lobe, m_or_g_chosen, verbose_plots)
                     print('___MEG QC___: ', "Finished ECG. --- Execution %s seconds ---" % (time.time() - start_time))
 
+                    avg_ecg += avg_objects_ecg
+
                 if all_qc_params['default']['run_EOG'] is True:
                     print('___MEG QC___: ', 'Starting EOG...')
                     start_time = time.time()
                     eog_derivs, simple_metrics_eog, eog_str, avg_objects_eog = EOG_meg_qc(all_qc_params['EOG'], raw_cropped, channels, chs_by_lobe, m_or_g_chosen, verbose_plots)
                     print('___MEG QC___: ', "Finished EOG. --- Execution %s seconds ---" % (time.time() - start_time))
 
-                    avg_ecg += avg_objects_ecg
                     avg_eog += avg_objects_eog
 
                 if all_qc_params['default']['run_Head'] is True:
                     print('___MEG QC___: ', 'Starting Head movement calculation...')
                     head_derivs, simple_metrics_head, head_str, df_head_pos, head_pos = HEAD_movement_meg_qc(raw_cropped, verbose_plots, plot_with_lines=True, plot_annotations=False)
                     print('___MEG QC___: ', "Finished Head movement calculation. --- Execution %s seconds ---" % (time.time() - start_time))
 
@@ -243,15 +244,15 @@
                 #         print(f"Set type of data found in key '{key}'")
                 
 
                 #Make report and add to QC_derivs:
                 # report_html_string = make_joined_report(QC_derivs, shielding_str, m_or_g_skipped_str, epoching_skipped_str, no_ecg_str, no_eog_str, no_head_pos_str, muscle_str)
                 # QC_derivs['Report']= [QC_derivative(report_html_string, 'Report', 'report')]
 
-                report_html_string = make_joined_report_mne(raw, QC_derivs, report_strings)
+                report_html_string = make_joined_report_mne(raw, QC_derivs, report_strings, default_settings=all_qc_params['default'])
                 QC_derivs['Report_MNE']= [QC_derivative(report_html_string, 'REPORTmne', 'report mne')]
 
                 #Collect all simple metrics into a dictionary and add to QC_derivs:
                 QC_derivs['Simple_metrics']=[QC_derivative(QC_simple, 'SimpleMetrics', 'json')]
 
 
                 # d=0
```

### Comparing `meg_qc-0.0.4/meg_qc.egg-info/PKG-INFO` & `meg_qc-0.0.5/meg_qc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg-qc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/ANCPLabOldenburg/MEG-QC-code
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.0.4/setup.cfg` & `meg_qc-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `meg_qc-0.0.4/versioneer.py` & `meg_qc-0.0.5/versioneer.py`

 * *Files identical despite different names*

