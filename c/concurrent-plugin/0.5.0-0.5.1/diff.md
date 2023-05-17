# Comparing `tmp/concurrent_plugin-0.5.0-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,19 @@
-Zip file size: 31320 bytes, number of entries: 18
--rw-rw-r--  2.0 unx        2 b- defN 22-Nov-27 22:37 concurrent_plugin/__init__.py
--rw-rw-r--  2.0 unx    32882 b- defN 23-May-11 17:15 concurrent_plugin/concurrent_backend.py
--rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-17 04:51 concurrent_plugin/concurrent_core.py
--rw-rw-r--  2.0 unx    15759 b- defN 23-Feb-15 23:54 concurrent_plugin/login.py
--rw-rw-r--  2.0 unx     3994 b- defN 22-Dec-20 19:35 concurrent_plugin/periodic_run.py
--rw-rw-r--  2.0 unx     1298 b- defN 23-Jan-19 23:36 concurrent_plugin/periodic_run_utils.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/__init__.py
--rw-rw-r--  2.0 unx      990 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_download.py
--rw-rw-r--  2.0 unx     1339 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_prefetch.py
--rw-rw-r--  2.0 unx    10783 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinfs.py
--rw-rw-r--  2.0 unx     5326 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinmount.py
--rw-rw-r--  2.0 unx     1140 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/mount_main.py
--rw-rw-r--  2.0 unx    16259 b- defN 23-May-11 16:02 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      205 b- defN 23-May-11 17:26 concurrent_plugin-0.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-11 17:26 concurrent_plugin-0.5.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx      182 b- defN 23-May-11 17:26 concurrent_plugin-0.5.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-May-11 17:26 concurrent_plugin-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1663 b- defN 23-May-11 17:26 concurrent_plugin-0.5.0.dist-info/RECORD
-18 files, 108752 bytes uncompressed, 28532 bytes compressed:  73.8%
+Zip file size: 31184 bytes, number of entries: 17
+-rw-rw-r--  2.0 unx        2 b- defN 22-Sep-22 06:22 concurrent_plugin/__init__.py
+-rw-rw-r--  2.0 unx    33825 b- defN 23-May-17 11:18 concurrent_plugin/concurrent_backend.py
+-rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-12 10:10 concurrent_plugin/concurrent_core.py
+-rw-rw-r--  2.0 unx    15759 b- defN 23-Feb-15 19:34 concurrent_plugin/login.py
+-rw-rw-r--  2.0 unx     3994 b- defN 23-Jan-10 17:33 concurrent_plugin/periodic_run.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Sep-22 06:22 concurrent_plugin/infinfs/__init__.py
+-rw-rw-r--  2.0 unx      990 b- defN 22-Oct-18 19:03 concurrent_plugin/infinfs/infin_download.py
+-rw-rw-r--  2.0 unx     1339 b- defN 22-Sep-22 06:22 concurrent_plugin/infinfs/infin_prefetch.py
+-rw-rw-r--  2.0 unx    10783 b- defN 22-Nov-11 07:23 concurrent_plugin/infinfs/infinfs.py
+-rw-rw-r--  2.0 unx     5326 b- defN 22-Oct-18 19:03 concurrent_plugin/infinfs/infinmount.py
+-rw-rw-r--  2.0 unx     1140 b- defN 22-Nov-11 07:23 concurrent_plugin/infinfs/mount_main.py
+-rw-rw-r--  2.0 unx    16627 b- defN 23-May-17 11:12 concurrent_plugin/infinfs/mount_service.py
+-rw-rw-r--  2.0 unx      307 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      181 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1567 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/RECORD
+17 files, 108770 bytes uncompressed, 28550 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -9,17 +9,14 @@
 
 Filename: concurrent_plugin/login.py
 Comment: 
 
 Filename: concurrent_plugin/periodic_run.py
 Comment: 
 
-Filename: concurrent_plugin/periodic_run_utils.py
-Comment: 
-
 Filename: concurrent_plugin/infinfs/__init__.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/infin_download.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/infin_prefetch.py
@@ -33,23 +30,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.5.0.dist-info/METADATA
+Filename: concurrent_plugin-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.5.0.dist-info/WHEEL
+Filename: concurrent_plugin-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.5.0.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.0.dist-info/top_level.txt
+Filename: concurrent_plugin-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.0.dist-info/RECORD
+Filename: concurrent_plugin-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/concurrent_backend.py

```diff
@@ -235,17 +235,15 @@
                     project, active_run)
         else:
             raise ValueError('kube_client_location must be either local or backend')
 
     def run_eks_on_backend(self, run_id, backend_type, bucket_name, path_in_bucket, work_dir, project_uri, entry_point, params,
             version, backend_config, tracking_store_uri, experiment_id, project, active_run):
         """
-        _summary_
-
-        _extended_summary_
+        calls the run_project() REST API to run the MLProject, instead of running the MLProject locally.  
 
         Args:
             run_id (_type_): _description_
             backend_type (_type_): _description_
             bucket_name (_type_): _description_
             path_in_bucket (_type_): _description_
             work_dir (_type_): _description_
@@ -369,16 +367,14 @@
             return wd
 
     def run_eks_on_local(self, backend_type, project_uri, entry_point, params,
             version, backend_config, tracking_store_uri, experiment_id, project, active_run, work_dir):
         """
         builds the docker image if needed, creates a k8s job, which then runs the docker image for the MLProject
 
-        _extended_summary_
-
         Args:
             backend_type (_type_): _description_
             project_uri (_type_): _description_
             entry_point (_type_): _description_
             params (_type_): _description_
             version (_type_): _description_
             backend_config (_type_): _description_
@@ -544,14 +540,17 @@
         if os.getenv('PERIODIC_RUN_START_TIME'):
           env_vars['PERIODIC_RUN_START_TIME'] = os.getenv('PERIODIC_RUN_START_TIME')
         if os.getenv('PERIODIC_RUN_END_TIME'):
           env_vars['PERIODIC_RUN_END_TIME'] = os.getenv('PERIODIC_RUN_END_TIME')
         env_vars['MLFLOW_CONCURRENT_URI'] = os.getenv('MLFLOW_CONCURRENT_URI')
         env_vars['DAG_EXECUTION_ID'] = os.getenv('DAG_EXECUTION_ID')
         env_vars['DAGID'] = os.getenv('DAGID')
+        # PYTHONUNBUFFERED is an environment variable in Python that can be used to disable output buffering for all streams. When this variable is set to a non-empty string, Python automatically sets the PYTHONUNBUFFERED flag, which forces Python to disable buffering for sys.stdout and sys.stderr.
+        if os.getenv("PYTHONUNBUFFERED"): env_vars['PYTHONUNBUFFERED'] = os.getenv("PYTHONUNBUFFERED")
+        
         job_template = mlflow.projects.kubernetes._get_kubernetes_job_definition(
             project_name, image_tag, image_digest, _get_run_command(command), env_vars, job_template
         )
         job_name = job_template["metadata"]["name"]
         job_namespace = job_template["metadata"]["namespace"]
         _load_kube_context(context=kube_context)
         kubernetes.client.configuration.retries = 10
@@ -613,16 +612,22 @@
         volume_mounts.append(kubernetes.client.V1VolumeMount(mount_path=CONCURRENT_FUSE_MOUNT_BASE,
                                                              name='sharedmount',
                                                              mount_propagation='HostToContainer'))
         side_car_volume_mounts.append(kubernetes.client.V1VolumeMount(mount_path=CONCURRENT_FUSE_MOUNT_BASE,
                                                     name='sharedmount',
                                                     mount_propagation='Bidirectional'))
 
-        job_template["spec"]["ttlSecondsAfterFinished"] = 7200
-
+        job_template["spec"]["ttlSecondsAfterFinished"] = int(os.getenv("CONCURRENT_KUBE_JOB_TEMPLATE_TTL", "7200"))
+        
+        if os.getenv("CONCURRENT_PRIVILEGED_MLFLOW_CONTAINER"): 
+            # create 'securityContext' if needed
+            if not job_template["spec"]["template"]["spec"]["containers"][0].get('securityContext'):
+                job_template["spec"]["template"]["spec"]["containers"][0]['securityContext'] = {}
+            job_template["spec"]["template"]["spec"]["containers"][0]['securityContext']['privileged'] = True
+            
         # Sometimes when auto-scaling is on, pods need to get rescheduled due to node scaledown.
         # The following snippet configures the rescheduling policy
         # See https://kubernetes.io/docs/concepts/workloads/controllers/job/#pod-failure-policy
         job_template["spec"]["template"]["spec"]["restartPolicy"] = "Never"
         job_template["spec"]["backoffLimit"] = 6
         podFailurePolicy = {"rules": [
                                         {
```

## concurrent_plugin/infinfs/mount_service.py

```diff
@@ -112,15 +112,15 @@
         logger.warning("Failed upload logs for {}, {}: {}".format(run_id, pod_name, ex))
 
 
 def update_mlflow_run(run_id, status):
     client = MlflowClient()
     client.set_terminated(run_id, status)
 
-def _filter_empty_in_dict_list_scalar(dict_list_scalar:Union[list, dict, Any]):
+def _filter_empty_in_dict_list_scalar(dict_list_scalar:Union[list, dict, Any]) -> Union[list, dict, Any]:
     """
     given a 'dict' or 'list' as input, removes all elements in these containers that are empty: scalars with None, strings that are '', lists and dicts that are empty.  Note that the filtering is in-place: modifies the passed list or dict
 
     Args:
         dict_list_scalar (Union[list, dict, Any]): see above
     """
     try:
@@ -135,27 +135,30 @@
                     # cannont do dict.pop(): RuntimeError: dictionary changed size during iteration
                     # dict_list_scalar.pop(k)
                     keys_to_del.append(k)
             
             # now delete the keys from the map
             for k in keys_to_del:
                 dict_list_scalar.pop(k)
+            
+            return dict_list_scalar
         elif isinstance(dict_list_scalar, list):
             i = 0; length = len(dict_list_scalar)
             while i < length: 
                 _filter_empty_in_dict_list_scalar(dict_list_scalar[i])
             
                 # check if element is now None (if scalar) or empty (if list or dict).  If so, remove the element from the list
                 if not dict_list_scalar[i]:
                     dict_list_scalar.remove(dict_list_scalar[i])
                     i -= 1; length -= 1
                 
                 i += 1
+            return dict_list_scalar
         else: # this must be a non container, like int, str, datatime.datetime
-            pass
+            return dict_list_scalar
     except Exception as e:
         # some excpetion, just log it..
         print(f"_filter_empty_in_dict_list_scalar(): Caught exception: {e}")
         traceback.print_exc()
 
 def log_describe_pod(k8s_client:kubernetes.client.CoreV1Api, run_id, pod_name, pod_namespace, pod_info:kubernetes.client.V1Pod):
     describe_file = "/tmp/describe-" + pod_name + ".txt"
@@ -216,29 +219,29 @@
             
         client = MlflowClient()
         client.log_artifact(run_id, describe_file, artifact_path='.concurrent/logs')
     except Exception as ex:
         logger.warning('Failed to log describe pod, try again later: ' + str(ex))
         return
 
-def fetch_upload_pod_status_logs(k8s_client:client.CoreV1Api, run_id, pod_name, pod_namespace):
+def _fetch_upload_pod_status_logs(k8s_client:client.CoreV1Api, run_id, pod_name, pod_namespace, log_suffix:int):
     try:
         pod_info:client.V1Pod = k8s_client.read_namespaced_pod(pod_name, pod_namespace)
         if pod_info.spec.containers[1].name.startswith('sidecar-'):
             sidecar_index = 1
             task_index = 0
         else:
             sidecar_index = 0
             task_index = 1
         task_container_name = pod_info.spec.containers[task_index].name
         side_car_container_name = pod_info.spec.containers[sidecar_index].name
         log_describe_pod(k8s_client, run_id, pod_name, pod_namespace, pod_info)
-        upload_logs_for_pod(k8s_client, run_id, pod_name, pod_namespace, "/tmp/run-logs.txt",
+        upload_logs_for_pod(k8s_client, run_id, pod_name, pod_namespace, f"/tmp/run-logs-{log_suffix}.txt",
                             container_name=task_container_name)
-        upload_logs_for_pod(k8s_client, run_id, pod_name, pod_namespace, f"/tmp/sidecar-logs.txt",
+        upload_logs_for_pod(k8s_client, run_id, pod_name, pod_namespace, f"/tmp/sidecar-logs-{log_suffix}.txt",
                             container_name=side_car_container_name)
         task_container_status = pod_info.status
         container_statuses = task_container_status.container_statuses
         task = container_statuses[task_index]
         task_container_state = task.state
         if task_container_state.running:
             print(f"Task container is in running state. Continuing to loop")
@@ -249,15 +252,15 @@
         elif task_container_state.waiting:
             print(f"Task container is in waiting state. Continuing to loop")
             return True
         else:
             print(f"Task container is in unknown state. Continuing to loop")
             return True
     except Exception as ex:
-        print(f"fetch_upload_pod_status_logs: caught {ex}. Continuing to loop")
+        print(f"_fetch_upload_pod_status_logs: caught {ex}. Continuing to loop")
         return True # continue looping
 
 def get_task_exit_code(k8s_client, pod_name, pod_namespace, num_attempt=1):
     max_attempts = 3
     pod_info = k8s_client.read_namespaced_pod(pod_name, pod_namespace)
     try:
         if pod_info.spec.containers[1].name.startswith('sidecar-'):
@@ -295,14 +298,15 @@
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             s.settimeout(15)
             s.bind((HOST, PORT))
             print('Mount/Monitor service starting for runid {0}, and podname {1}'.format(run_id, pod_name), flush=True)
             print('Listening on port {}:{}'.format(HOST, PORT), flush=True)
             s.listen()
             mount_service_ready()
+            i = 0
             while True:
                 print_info('Waiting for request..')
                 try:
                     conn, addr = s.accept()
                 except socket.timeout:
                     print_info('accept timed out')
                     pass
@@ -320,29 +324,30 @@
                             infinmount.perform_mount(mount_path, mount_spec, shadow_path=shadow_path, use_cache=use_cache)
                             response = "success".encode('utf-8')
                             print_info("mount successful")
                         except Exception as ex:
                             print_info('Exception in mounting: '+str(ex))
                             response = str(ex).encode('utf-8')
                         conn.send(response)
-                if not fetch_upload_pod_status_logs(k8s_client, run_id, pod_name, pod_namespace):
+                if not _fetch_upload_pod_status_logs(k8s_client, run_id, pod_name, pod_namespace, int(i/12)):   # i/12 so that we don't create a new log once every 15 seconds
                     print_info("Task process done, exiting mount service")
                     exitCode = get_task_exit_code(k8s_client, pod_name, pod_namespace)
                     if exitCode == 0:
                         update_mlflow_run(run_id, "FINISHED")
                         mlflow_run_status = "FINISHED"
                     else:
                         update_mlflow_run(run_id, "FAILED")
                         mlflow_run_status = "FAILED"
-                    fetch_upload_pod_status_logs(k8s_client, run_id, pod_name, pod_namespace)
+                    _fetch_upload_pod_status_logs(k8s_client, run_id, pod_name, pod_namespace, int(i/12))   # i/12 so that we don't create a new log once every 15 seconds
                     if dag_execution_id:
                         launch_dag_controller()
                     else:
                         print_info('Not a dag execution, skip dag controller')
                     exit(0)
+                i+=1
     except Exception as e1:
         if mlflow_run_status:
             print(f"mount_service: Caught {e1}. mlflow_run_status={mlflow_run_status}. Doing nothing", flush=True)
             if mlflow_run_status == "FINISHED":
                 exit(0)
             else:
                 exit(255)
```

## Comparing `concurrent_plugin-0.5.0.dist-info/RECORD` & `concurrent_plugin-0.5.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
-concurrent_plugin/concurrent_backend.py,sha256=uinSRfpa2Ar8niJ7836o66hLdzwnjoNeWRVHbr_iS_Q,32882
+concurrent_plugin/concurrent_backend.py,sha256=jtiJST2I56ZNGARles29-grG-D2kk9WFHMlw9MwG9kc,33825
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
-concurrent_plugin/periodic_run_utils.py,sha256=MZuX9uSFEuA7B8UFDAchsrWhidXT5QyuOA-GDtzIPOo,1298
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
-concurrent_plugin/infinfs/mount_service.py,sha256=mD3Y4oq1LMdNrBtKy2HeWL3JaWmqSbfJzpFTzthtgSI,16259
-concurrent_plugin-0.5.0.dist-info/METADATA,sha256=tP4qORs_hc-OVYQoj2pdhxmh6tPJEwSnMe4aDkHG6nM,205
-concurrent_plugin-0.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-concurrent_plugin-0.5.0.dist-info/entry_points.txt,sha256=5bYsI3RSqBvAjlcOeCbKKIRorBotB8wvo1p4Xfn3tXY,182
-concurrent_plugin-0.5.0.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.5.0.dist-info/RECORD,,
+concurrent_plugin/infinfs/mount_service.py,sha256=iPrGlkx4AS3aauPii77UZ7F09bfynQMnzxyZFOg02B8,16627
+concurrent_plugin-0.5.1.dist-info/METADATA,sha256=q01_DwrFNlEg3r8vIOHu0GT-bWxAmZbeXByq4hTsH0s,307
+concurrent_plugin-0.5.1.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
+concurrent_plugin-0.5.1.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
+concurrent_plugin-0.5.1.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.5.1.dist-info/RECORD,,
```

