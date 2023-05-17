# Comparing `tmp/sca_rhythm-0.4.5.tar.gz` & `tmp/sca_rhythm-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.4.5.tar", max compression
+gzip compressed data, was "sca_rhythm-0.4.6.tar", max compression
```

## Comparing `sca_rhythm-0.4.5.tar` & `sca_rhythm-0.4.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.5/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.5/README.md
--rw-r--r--   0        0        0      360 2023-05-12 20:24:14.051216 sca_rhythm-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    15285 2023-05-11 04:15:42.637455 sca_rhythm-0.4.5/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     6872 2023-05-12 03:16:31.209319 sca_rhythm-0.4.5/sca_rhythm/progress.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 sca_rhythm-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.6/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.6/README.md
+-rw-r--r--   0        0        0      360 2023-05-17 18:12:13.749693 sca_rhythm-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    15818 2023-05-13 03:48:44.262621 sca_rhythm-0.4.6/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     6872 2023-05-12 03:16:31.209319 sca_rhythm-0.4.6/sca_rhythm/progress.py
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 sca_rhythm-0.4.6/PKG-INFO
```

### Comparing `sca_rhythm-0.4.5/LICENSE.md` & `sca_rhythm-0.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.5/README.md` & `sca_rhythm-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.5/sca_rhythm/__init__.py` & `sca_rhythm-0.4.6/sca_rhythm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     return list((Counter(items) - Counter(set(items))).keys())
 
 
 class WFNotFound(Exception):
     pass
 
 
+class NonRetryableException(Exception):
+    pass
+
+
 class Workflow:
     def __init__(self, celery_app, workflow_id=None, steps=None, name=None, app_id=None, description=None):
         self.app = celery_app
         db = self.app.backend.database
         self.wf_col = db.get_collection('workflow_meta')
 
         assert workflow_id is not None or steps is not None, 'Either workflow_id or steps should not be None'
@@ -36,15 +40,15 @@
             # create workflow object and save to db
             assert len(steps) > 0, 'steps is empty'
             for i, step in enumerate(steps):
                 assert 'name' in step, f'step - {i} does not have "name" key'
                 assert len(step['name']) > 0, f'step - {i} name is empty'
                 assert 'task' in step, f'step - {i} does not have "task" key'
                 # assert step['task'] in self.app.tasks, \
-                #     f'step - {i} Task {step["task"]} is not registered in the celery application'
+                #     f' step - {i} Task {step["task"]} is not registered in the celery application'
             names = [step['name'] for step in steps]
             duplicate_names = duplicates(names)
             assert len(duplicate_names) == 0, f'Steps with duplicate names: {duplicate_names}'
 
             assert name, 'name cannot be empty'
             assert app_id, 'app_id cannot be empty'
             self.workflow = {
@@ -165,15 +169,15 @@
         step = self.get_step(step_name)
         step['task_runs'] = step.get('task_runs', [])
         step['task_runs'].append({
             'date_start': datetime.datetime.utcnow(),
             'task_id': task_id
         })
         self.update()
-        # print(f'starting {step_name} with task id: {task_id}')
+        # print(f' starting {step_name} with task id: {task_id}')
 
     def on_step_success(self, retval: tuple, step_name: str) -> None:
         """
         Called by an instance of WorkflowTask before after it completes work.
         calls the next step (if there is one) with the first element of the retval as an argument.
 
         :param retval: the return value of the task of tuple type. the first element is sent to the next step as an arg
@@ -189,15 +193,15 @@
 
             kwargs = {
                 'workflow_id': self.workflow['_id'],
                 'step': next_step['name']
             }
             # next_task.apply_async((retval[0],), kwargs)
             self.app.send_task(next_step['task'], (retval[0],), kwargs)
-            # print(f'starting next step {next_step["name"]}')
+            # print(f' starting next step {next_step["name"]}')
 
     def update(self):
         """
         Update the workflow object in mongo db
         :return: None
         """
         self.workflow['updated_at'] = datetime.datetime.utcnow()
@@ -344,38 +348,45 @@
             'steps_done': pending_step_idx if pending_step_idx is not None else len(steps),
             'total_steps': len(steps),
             'steps': steps
         }
 
 
 class WorkflowTask(Task):  # noqa
-    # autoretry_for = (Exception,)  # retry for all exceptions
-    # max_retries = 3
-    # default_retry_delay = 5  # wait for n seconds before adding the task back to the queue
+    autoretry_for = (Exception,)  # retry for all exceptions
+    dont_autoretry_for = (NonRetryableException,)
+    max_retries = 3
+    default_retry_delay = 5  # wait for n seconds before adding the task back to the queue
     add_to_parent = True
     trail = True
 
     def __init__(self):
         self.workflow = None
 
     def before_start(self, task_id, args, kwargs):
-        # print(f'before_start, task_id:{task_id}, kwargs:{kwargs} name:{self.name}')
-        self.update_progress({})
+        # print(f' before_start, task_id:{task_id}, kwargs:{kwargs} name:{self.name}')
+
+        # A task's result in the backend is not updated until the tasks succeeds, fails, revoked
+        # or updated through code after it start execution.
+        # To the observers that task will appear to be in a pending state.
+        # Programmatically setting the state to PROGRESS before starting execution.
+        # setting task_track_started=True accomplishes the same while setting state as started. (yet to be tested)
+        # self.update_progress({})
 
         if 'workflow_id' in kwargs and 'step' in kwargs:
             workflow_id = kwargs['workflow_id']
             self.workflow = Workflow(self.app, workflow_id)
             self.workflow.on_step_start(kwargs['step'], task_id)
 
     def on_success(self, retval, task_id, args, kwargs):
-        # print(f'on_success, task_id: {task_id}, kwargs: {kwargs}')
+        # print(f' on_success, task_id: {task_id}, kwargs: {kwargs}')
 
         if 'workflow_id' in kwargs and 'step' in kwargs:
             self.workflow.on_step_success(retval, kwargs['step'])
 
     def update_progress(self, progress_obj):
         # called_directly: This flag is set to true if the task was not executed by the worker.
         if not self.request.called_directly:
             self.update_state(
-                state='PROGRESS',
+                state='STARTED',
                 meta=progress_obj
             )
```

### Comparing `sca_rhythm-0.4.5/sca_rhythm/progress.py` & `sca_rhythm-0.4.6/sca_rhythm/progress.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.5/PKG-INFO` & `sca_rhythm-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.4.5
+Version: 0.4.6
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

