# Comparing `tmp/sca_rhythm-0.4.6.tar.gz` & `tmp/sca_rhythm-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.4.6.tar", max compression
+gzip compressed data, was "sca_rhythm-0.4.7.tar", max compression
```

## Comparing `sca_rhythm-0.4.6.tar` & `sca_rhythm-0.4.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.6/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.6/README.md
--rw-r--r--   0        0        0      360 2023-05-17 18:12:13.749693 sca_rhythm-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    15818 2023-05-13 03:48:44.262621 sca_rhythm-0.4.6/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     6872 2023-05-12 03:16:31.209319 sca_rhythm-0.4.6/sca_rhythm/progress.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 sca_rhythm-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.7/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.7/README.md
+-rw-r--r--   0        0        0      360 2023-05-17 21:01:16.354100 sca_rhythm-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    16428 2023-05-17 21:00:55.050209 sca_rhythm-0.4.7/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     6872 2023-05-12 03:16:31.209319 sca_rhythm-0.4.7/sca_rhythm/progress.py
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 sca_rhythm-0.4.7/PKG-INFO
```

### Comparing `sca_rhythm-0.4.6/LICENSE.md` & `sca_rhythm-0.4.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.6/README.md` & `sca_rhythm-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.6/sca_rhythm/__init__.py` & `sca_rhythm-0.4.7/sca_rhythm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 import itertools
 import json
 import uuid
 from collections import Counter
 
 import celery
@@ -94,16 +96,17 @@
         if first_step_not_succeeded:
             i, status = first_step_not_succeeded
             if status not in [celery.states.SUCCESS, celery.states.FAILURE]:
                 step = self.workflow['steps'][i]
                 task_runs = step.get('task_runs', [])
                 if task_runs is not None and len(task_runs) > 0:
                     task_id = task_runs[-1]['task_id']
+                    # https://docs.celeryq.dev/en/stable/userguide/workers.html#revoke-revoking-tasks
                     self.app.control.revoke(task_id, terminate=True)
-                    print(f'revoked task: {task_id} in step-{i + 1} {step["name"]}')
+                    # print(f' revoked task: {task_id} in step-{i + 1} {step["name"]}')
                     return {
                         'paused': True,
                         'revoked_step': {
                             'task_id': task_id,
                             'task': step['task'],
                             'name': step['name']
                         }
@@ -141,43 +144,50 @@
 
                 kwargs = {
                     'workflow_id': self.workflow['_id'],
                     'step': step['name']
                 }
                 # task.apply_async(task_args, kwargs)
                 self.app.send_task(step['task'], task_args, kwargs)
-                print(f'resuming step {step["name"]}')
+                # print(f' resuming step {step["name"]}')
                 return {
                     'resumed': True,
                     'restarted_step': {
                         'name': step['name'],
                         'task': step['task']
                     }
                 }
         return {
             'resumed': False
         }
 
     def on_step_start(self, step_name: str, task_id: str) -> None:
         """
         Called by an instance of WorkflowTask before it starts work.
-        Updates the workflow object's step with the task_id and date_start
+        Updates the workflow object's step with the task_id and date_start.
+
+        If the task is resubmitted with the old task_id, task_runs will not be updated.
 
         :param step_name: name of the step that the task is running
         :param task_id: id of the task
         :return: None
         """
         step = self.get_step(step_name)
-        step['task_runs'] = step.get('task_runs', [])
-        step['task_runs'].append({
-            'date_start': datetime.datetime.utcnow(),
-            'task_id': task_id
-        })
-        self.update()
-        # print(f' starting {step_name} with task id: {task_id}')
+        task_runs = step.get('task_runs', [])
+
+        prev_task_ids_set = set(task_run.get('task_id', '') for task_run in task_runs)
+        if task_id not in prev_task_ids_set:
+            task_runs.append({
+                'date_start': datetime.datetime.utcnow(),
+                'task_id': task_id
+            })
+            self.update()
+            # print(f' starting {step_name} with task id: {task_id}')
+        else:
+            print(f'on_step_start {step_name} {task_id} already in prev task runs. not adding.')
 
     def on_step_success(self, retval: tuple, step_name: str) -> None:
         """
         Called by an instance of WorkflowTask before after it completes work.
         calls the next step (if there is one) with the first element of the retval as an argument.
 
         :param retval: the return value of the task of tuple type. the first element is sent to the next step as an arg
@@ -232,38 +242,38 @@
         if len(task_runs) > 0:
             task_id = task_runs[-1]['task_id']
             task_status = self.app.backend.get_status(task_id)
             return task_status
         else:
             return celery.states.PENDING
 
-    def get_pending_step(self) -> tuple:
+    def get_pending_step(self) -> tuple[int, celery.states.state] | None:
         """
         finds the index of the first step whose status is not celery.states.SUCCESS
         if all steps have succeeded, it returns None
         :return: tuple (index:int, status:CELERY.states.STATE)
         """
         statuses = [(i, self.get_step_status(step)) for i, step in enumerate(self.workflow['steps'])]
         return next((s for s in statuses if s[1] != celery.states.SUCCESS), None)
 
     def get_workflow_status(self) -> celery.states.state:
         """
-        The workflow status is decided based on the status of the first step which is not done (FS).
-        - PENDING  - the first step is yet to be processed
-        - STARTED  - if status of FS is either of STARTED, RETRY, or PENDING
-        - PROGRESS - a step is running and has updated the task object with progress
-        - REVOKED  - running step is REVOKED, the Workflow is considered paused and can be resumed
-        - FAILURE  - FS has failed
+        The workflow status is decided based on the status of the first step which is not done (pending step).
+        - PENDING  - the pending step is the first step and is yet to be received by the worker
+        - STARTED  - else, if the status of the pending step is one of STARTED, RETRY, PENDING
+        - PROGRESS - a step is running and has updated the task object with its progress
+        - REVOKED  - the pending step was revoked, the Workflow is considered paused and can be resumed
+        - FAILURE  - the pending step was failed, the workflow is considered failed and can be resumed
         - SUCCESS  - all steps have succeeded
 
         :return: celery.states.state
         """
-        first_step_not_succeeded = self.get_pending_step()
-        if first_step_not_succeeded:
-            step_idx, task_status = first_step_not_succeeded
+        pending_step = self.get_pending_step()
+        if pending_step:
+            step_idx, task_status = pending_step
             if step_idx == 0 and task_status == celery.states.PENDING:
                 return celery.states.PENDING
             if task_status in [celery.states.STARTED, celery.states.RETRY, celery.states.PENDING]:
                 return celery.states.STARTED
             else:
                 return task_status
         else:
@@ -348,20 +358,19 @@
             'steps_done': pending_step_idx if pending_step_idx is not None else len(steps),
             'total_steps': len(steps),
             'steps': steps
         }
 
 
 class WorkflowTask(Task):  # noqa
-    autoretry_for = (Exception,)  # retry for all exceptions
-    dont_autoretry_for = (NonRetryableException,)
-    max_retries = 3
-    default_retry_delay = 5  # wait for n seconds before adding the task back to the queue
-    add_to_parent = True
-    trail = True
+    # autoretry_for = (Exception,)  # retry for all exceptions
+    # dont_autoretry_for = (NonRetryableException,)
+    # max_retries = 3
+    # default_retry_delay = 5  # wait for n seconds before adding the task back to the queue
+    # trail = True
 
     def __init__(self):
         self.workflow = None
 
     def before_start(self, task_id, args, kwargs):
         # print(f' before_start, task_id:{task_id}, kwargs:{kwargs} name:{self.name}')
```

### Comparing `sca_rhythm-0.4.6/sca_rhythm/progress.py` & `sca_rhythm-0.4.7/sca_rhythm/progress.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.6/PKG-INFO` & `sca_rhythm-0.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.4.6
+Version: 0.4.7
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

