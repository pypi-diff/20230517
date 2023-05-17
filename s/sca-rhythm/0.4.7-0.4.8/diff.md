# Comparing `tmp/sca_rhythm-0.4.7.tar.gz` & `tmp/sca_rhythm-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.4.7.tar", max compression
+gzip compressed data, was "sca_rhythm-0.4.8.tar", max compression
```

## Comparing `sca_rhythm-0.4.7.tar` & `sca_rhythm-0.4.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.7/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.7/README.md
--rw-r--r--   0        0        0      360 2023-05-17 21:01:16.354100 sca_rhythm-0.4.7/pyproject.toml
--rw-r--r--   0        0        0    16428 2023-05-17 21:00:55.050209 sca_rhythm-0.4.7/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     6872 2023-05-12 03:16:31.209319 sca_rhythm-0.4.7/sca_rhythm/progress.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 sca_rhythm-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.8/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.8/README.md
+-rw-r--r--   0        0        0      357 2023-05-17 21:32:08.438270 sca_rhythm-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0    16452 2023-05-17 21:09:30.369075 sca_rhythm-0.4.8/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     6872 2023-05-12 03:16:31.209319 sca_rhythm-0.4.8/sca_rhythm/progress.py
+-rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.4.8/PKG-INFO
```

### Comparing `sca_rhythm-0.4.7/LICENSE.md` & `sca_rhythm-0.4.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.7/README.md` & `sca_rhythm-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.7/sca_rhythm/__init__.py` & `sca_rhythm-0.4.8/sca_rhythm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,19 +168,19 @@
         If the task is resubmitted with the old task_id, task_runs will not be updated.
 
         :param step_name: name of the step that the task is running
         :param task_id: id of the task
         :return: None
         """
         step = self.get_step(step_name)
-        task_runs = step.get('task_runs', [])
+        step['task_runs'] = step.get('task_runs', [])
 
-        prev_task_ids_set = set(task_run.get('task_id', '') for task_run in task_runs)
+        prev_task_ids_set = set(task_run.get('task_id', '') for task_run in step['task_runs'])
         if task_id not in prev_task_ids_set:
-            task_runs.append({
+            step['task_runs'].append({
                 'date_start': datetime.datetime.utcnow(),
                 'task_id': task_id
             })
             self.update()
             # print(f' starting {step_name} with task id: {task_id}')
         else:
             print(f'on_step_start {step_name} {task_id} already in prev task runs. not adding.')
```

### Comparing `sca_rhythm-0.4.7/sca_rhythm/progress.py` & `sca_rhythm-0.4.8/sca_rhythm/progress.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.7/PKG-INFO` & `sca_rhythm-0.4.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.4.7
+Version: 0.4.8
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: celery (>=5.3.0rc1,<6.0.0)
+Requires-Dist: celery (>=5.2.7,<6.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Rhythm
 Rhythm allows you to design and control workflows made of Celery tasks. A workflow is a sequence of steps to run one after the other. Rhythm simplifies the process of executing workflows consisting of long-running tasks with reliability.
 
 The following are the features of Rhythm workflows:
```

