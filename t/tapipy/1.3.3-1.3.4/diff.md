# Comparing `tmp/tapipy-1.3.3.tar.gz` & `tmp/tapipy-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapipy-1.3.3.tar", max compression
+gzip compressed data, was "tapipy-1.3.4.tar", max compression
```

## Comparing `tapipy-1.3.3.tar` & `tapipy-1.3.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1539 2022-05-17 23:01:20.810838 tapipy-1.3.3/LICENSE.md
--rw-r--r--   0        0        0     8639 2022-09-27 22:55:39.801480 tapipy-1.3.3/README.md
--rw-r--r--   0        0        0      970 2023-04-18 21:53:08.470903 tapipy-1.3.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-18 21:53:04.234943 tapipy-1.3.3/tapipy/__init__.py
--rw-r--r--   0        0        0    13502 2022-09-27 22:40:07.902909 tapipy-1.3.3/tapipy/actors.py
--rw-r--r--   0        0        0     2071 2022-10-13 22:38:48.858613 tapipy-1.3.3/tapipy/errors.py
--rw-r--r--   0        0        0    38703 2022-05-17 23:01:20.818838 tapipy-1.3.3/tapipy/resources/openapi_v3-actors.yml
--rw-r--r--   0        0        0    65073 2023-04-14 14:57:18.237004 tapipy-1.3.3/tapipy/resources/openapi_v3-apps.yml
--rw-r--r--   0        0        0    23554 2022-10-13 22:47:01.777739 tapipy-1.3.3/tapipy/resources/openapi_v3-authenticator.yml
--rw-r--r--   0        0        0    73801 2023-04-18 21:51:45.271692 tapipy-1.3.3/tapipy/resources/openapi_v3-files.yml
--rw-r--r--   0        0        0    65257 2023-03-22 22:25:39.039342 tapipy-1.3.3/tapipy/resources/openapi_v3-jobs.yml
--rw-r--r--   0        0        0    28625 2022-05-17 23:01:20.822838 tapipy-1.3.3/tapipy/resources/openapi_v3-meta.yml
--rw-r--r--   0        0        0    52031 2023-04-14 14:57:21.296975 tapipy-1.3.3/tapipy/resources/openapi_v3-notifications.yml
--rw-r--r--   0        0        0    33814 2023-03-22 22:25:37.527357 tapipy-1.3.3/tapipy/resources/openapi_v3-pgrest.yml
--rw-r--r--   0        0        0    30728 2022-12-13 18:05:18.840827 tapipy-1.3.3/tapipy/resources/openapi_v3-pods.yml
--rw-r--r--   0        0        0   145319 2022-10-25 21:18:32.853350 tapipy-1.3.3/tapipy/resources/openapi_v3-sk.yml
--rw-r--r--   0        0        0   108752 2023-03-22 22:25:35.307379 tapipy-1.3.3/tapipy/resources/openapi_v3-streams.yml
--rw-r--r--   0        0        0    90114 2023-04-14 14:57:14.489040 tapipy-1.3.3/tapipy/resources/openapi_v3-systems.yml
--rw-r--r--   0        0        0    25448 2022-05-17 23:01:20.826838 tapipy-1.3.3/tapipy/resources/openapi_v3-tenants.yml
--rw-r--r--   0        0        0     8406 2022-10-13 22:47:04.421713 tapipy-1.3.3/tapipy/resources/openapi_v3-tokens.yml
--rw-r--r--   0        0        0    87200 2023-04-14 14:57:20.564982 tapipy-1.3.3/tapipy/resources/openapi_v3-workflows.yml
--rw-r--r--   0        0        0      907 2023-04-18 21:51:51.319634 tapipy-1.3.3/tapipy/resources/resource_etags.json
--rw-r--r--   0        0        0    24325 2023-04-18 21:51:54.179607 tapipy-1.3.3/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle
--rw-r--r--   0        0        0    30512 2023-04-18 21:51:51.895629 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
--rw-r--r--   0        0        0    49315 2023-04-18 21:51:54.827601 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
--rw-r--r--   0        0        0    19368 2023-04-18 21:51:51.995628 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
--rw-r--r--   0        0        0    55698 2023-04-18 21:51:52.423624 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
--rw-r--r--   0        0        0    49485 2023-04-18 21:51:54.527604 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
--rw-r--r--   0        0        0    21718 2023-04-18 21:51:52.115627 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
--rw-r--r--   0        0        0    40403 2023-04-18 21:51:55.043599 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
--rw-r--r--   0        0        0    27737 2023-04-18 21:51:54.019609 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
--rw-r--r--   0        0        0   117394 2023-04-18 21:51:52.911619 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
--rw-r--r--   0        0        0    81328 2023-04-18 21:51:53.375615 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
--rw-r--r--   0        0        0    69380 2023-04-18 21:51:53.715612 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
--rw-r--r--   0        0        0    20570 2023-04-18 21:51:53.839611 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
--rw-r--r--   0        0        0     7112 2023-04-18 21:51:53.887610 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
--rw-r--r--   0        0        0    64540 2023-04-18 21:51:56.747583 tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
--rw-r--r--   0        0        0    14089 2022-05-17 23:01:20.830838 tapipy-1.3.3/tapipy/specs/tapis-project-tapis-client-java-dev-jobs-client-src-main-resources-jobsapi.pickle
--rw-r--r--   0        0        0    70890 2023-04-14 15:12:33.374927 tapipy-1.3.3/tapipy/tapis.py
--rw-r--r--   0        0        0      144 2022-05-17 23:01:20.834838 tapipy-1.3.3/tapipy/util.py
--rw-r--r--   0        0        0    10018 1970-01-01 00:00:00.000000 tapipy-1.3.3/setup.py
--rw-r--r--   0        0        0    10051 1970-01-01 00:00:00.000000 tapipy-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1539 2022-05-17 23:01:20.810838 tapipy-1.3.4/LICENSE.md
+-rw-r--r--   0        0        0     8639 2022-09-27 22:55:39.801480 tapipy-1.3.4/README.md
+-rw-r--r--   0        0        0      970 2023-05-16 23:04:32.628702 tapipy-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-16 23:04:32.628702 tapipy-1.3.4/tapipy/__init__.py
+-rw-r--r--   0        0        0    13502 2022-09-27 22:40:07.902909 tapipy-1.3.4/tapipy/actors.py
+-rw-r--r--   0        0        0     2071 2022-10-13 22:38:48.858613 tapipy-1.3.4/tapipy/errors.py
+-rw-r--r--   0        0        0    38703 2022-05-17 23:01:20.818838 tapipy-1.3.4/tapipy/resources/openapi_v3-actors.yml
+-rw-r--r--   0        0        0    65073 2023-04-14 14:57:18.237004 tapipy-1.3.4/tapipy/resources/openapi_v3-apps.yml
+-rw-r--r--   0        0        0    23782 2023-05-16 23:04:32.628702 tapipy-1.3.4/tapipy/resources/openapi_v3-authenticator.yml
+-rw-r--r--   0        0        0    73801 2023-04-18 21:51:45.271692 tapipy-1.3.4/tapipy/resources/openapi_v3-files.yml
+-rw-r--r--   0        0        0    65915 2023-05-16 23:04:32.628702 tapipy-1.3.4/tapipy/resources/openapi_v3-jobs.yml
+-rw-r--r--   0        0        0    28625 2022-05-17 23:01:20.822838 tapipy-1.3.4/tapipy/resources/openapi_v3-meta.yml
+-rw-r--r--   0        0        0    52031 2023-04-14 14:57:21.296975 tapipy-1.3.4/tapipy/resources/openapi_v3-notifications.yml
+-rw-r--r--   0        0        0    33814 2023-03-22 22:25:37.527357 tapipy-1.3.4/tapipy/resources/openapi_v3-pgrest.yml
+-rw-r--r--   0        0        0    30728 2022-12-13 18:05:18.840827 tapipy-1.3.4/tapipy/resources/openapi_v3-pods.yml
+-rw-r--r--   0        0        0   145319 2022-10-25 21:18:32.853350 tapipy-1.3.4/tapipy/resources/openapi_v3-sk.yml
+-rw-r--r--   0        0        0   108752 2023-03-22 22:25:35.307379 tapipy-1.3.4/tapipy/resources/openapi_v3-streams.yml
+-rw-r--r--   0        0        0    90114 2023-04-14 14:57:14.489040 tapipy-1.3.4/tapipy/resources/openapi_v3-systems.yml
+-rw-r--r--   0        0        0    25448 2022-05-17 23:01:20.826838 tapipy-1.3.4/tapipy/resources/openapi_v3-tenants.yml
+-rw-r--r--   0        0        0     8406 2022-10-13 22:47:04.421713 tapipy-1.3.4/tapipy/resources/openapi_v3-tokens.yml
+-rw-r--r--   0        0        0    87200 2023-04-14 14:57:20.564982 tapipy-1.3.4/tapipy/resources/openapi_v3-workflows.yml
+-rw-r--r--   0        0        0      907 2023-05-16 23:04:32.628702 tapipy-1.3.4/tapipy/resources/resource_etags.json
+-rw-r--r--   0        0        0    24325 2023-05-16 22:45:44.293279 tapipy-1.3.4/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle
+-rw-r--r--   0        0        0    30512 2023-05-16 22:45:42.217290 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
+-rw-r--r--   0        0        0    49315 2023-05-16 22:45:44.897276 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
+-rw-r--r--   0        0        0    19592 2023-05-16 23:04:32.628702 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
+-rw-r--r--   0        0        0    55698 2023-05-16 22:45:42.685288 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
+-rw-r--r--   0        0        0    49993 2023-05-16 23:04:32.628702 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
+-rw-r--r--   0        0        0    21718 2023-05-16 22:45:42.425289 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
+-rw-r--r--   0        0        0    40403 2023-05-16 22:45:45.093275 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
+-rw-r--r--   0        0        0    27737 2023-05-16 22:45:44.153280 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
+-rw-r--r--   0        0        0   117394 2023-05-16 22:45:43.129285 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
+-rw-r--r--   0        0        0    81328 2023-05-16 22:45:43.545283 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
+-rw-r--r--   0        0        0    69380 2023-05-16 22:45:43.889281 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
+-rw-r--r--   0        0        0    20570 2023-05-16 22:45:43.989281 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
+-rw-r--r--   0        0        0     7112 2023-05-16 22:45:44.033280 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
+-rw-r--r--   0        0        0    64540 2023-05-16 22:45:46.757266 tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
+-rw-r--r--   0        0        0    14089 2022-05-17 23:01:20.830838 tapipy-1.3.4/tapipy/specs/tapis-project-tapis-client-java-dev-jobs-client-src-main-resources-jobsapi.pickle
+-rw-r--r--   0        0        0    70890 2023-04-14 15:12:33.374927 tapipy-1.3.4/tapipy/tapis.py
+-rw-r--r--   0        0        0      695 2023-05-16 23:05:07.120400 tapipy-1.3.4/tapipy/util.py
+-rw-r--r--   0        0        0    10018 1970-01-01 00:00:00.000000 tapipy-1.3.4/setup.py
+-rw-r--r--   0        0        0    10051 1970-01-01 00:00:00.000000 tapipy-1.3.4/PKG-INFO
```

### Comparing `tapipy-1.3.3/LICENSE.md` & `tapipy-1.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/README.md` & `tapipy-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/actors.py` & `tapipy-1.3.4/tapipy/actors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/errors.py` & `tapipy-1.3.4/tapipy/errors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-actors.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-actors.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-apps.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-apps.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-authenticator.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-authenticator.yml`

 * *Files 2% similar despite different names*

```diff
@@ -729,14 +729,15 @@
     arrayOfClients:
       type: array
       items:
         $ref: '#/components/schemas/Client'
 
     Profile:
       type: object
+      description: The profile associated with a Tapis identity. NOTE -the fields in the Profile object are populated on a best-effort basis and should not be relied upon. Only the username field is guaranteed to be populated. 
       properties:
         username:
           type: string
           description: The username associated with the profile.
         email:
           type: string
           description: The email address associated with the profile.
```

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-files.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-files.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-jobs.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-jobs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -499,21 +499,28 @@
       security:
         - TapisJWT: []
   /jobs/{jobUuid}/output/download/{outputPath}:
     get:
       tags:
         - jobs
       description: >-
-        Download job's output files for previously submitted job by its UUID.
-        The job must be in a terminal state (FINISHED or FAILED or CANCELLED).  
+        Download job's output files for previously submitted job by its UUID. 
+
+        The job must be in a terminal state (FINISHED or FAILED or CANCELLED).
+        By default, allowIfRunning=false. 
+
+        allowIfRunning=true allows job output download even if job is not in the
+        terminal state.  
 
 
         The caller must be the job owner, creator or a tenant administrator.
 
         The URL must ends with '/' even if there is no outputPath is specified. 
+
+        outputPath is relative to the job output path. 
       operationId: getJobOutputDownload
       parameters:
         - name: jobUuid
           in: path
           required: true
           schema:
             type: string
@@ -529,14 +536,19 @@
             type: boolean
             default: false
         - name: format
           in: query
           schema:
             type: string
             default: zip
+        - name: allowIfRunning
+          in: query
+          schema:
+            type: boolean
+            default: false
         - name: pretty
           in: query
           schema:
             type: boolean
             default: false
       responses:
         '200':
@@ -580,21 +592,28 @@
         - TapisJWT: []
   /jobs/{jobUuid}/output/list/{outputPath}:
     get:
       tags:
         - jobs
       description: >-
         Retrieve job's output files list for previously submitted job by its
-        UUID. The job must be in a terminal state (FINISHED or FAILED or
-        CANCELLED)  
+        UUID. 
+
+        The job must be in a terminal state (FINISHED or FAILED or CANCELLED).
+        By default, allowIfRunning=false. 
+
+        allowIfRunning=true allows job output listing even if job is not in the
+        terminal state.  
 
 
         The caller must be the job owner, creator or a tenant administrator.
 
-        The URL must ends with '/' even if there is no outputPath is specified. 
+        The URL must ends with '/' even if there is no outputPath is specified.
+
+        outputPath is relative to the job output path. 
       operationId: getJobOutputList
       parameters:
         - name: jobUuid
           in: path
           required: true
           schema:
             type: string
@@ -610,14 +629,19 @@
             type: integer
             format: int32
         - name: skip
           in: query
           schema:
             type: integer
             format: int32
+        - name: allowIfRunning
+          in: query
+          schema:
+            type: boolean
+            default: false
         - name: pretty
           in: query
           schema:
             type: boolean
             default: false
       responses:
         '200':
@@ -1824,15 +1848,15 @@
             - FORK
             - BATCH
         mpiCmd:
           type: string
         cmdPrefix:
           type: string
         sharedAppCtx:
-          type: boolean
+          type: string
         sharedAppCtxAttribs:
           type: array
           items:
             type: string
             enum:
               - SAC_EXEC_SYSTEM_ID
               - SAC_EXEC_SYSTEM_EXEC_DIR
```

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-meta.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-meta.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-notifications.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-notifications.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-pgrest.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-pgrest.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-pods.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-pods.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-sk.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-sk.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-streams.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-streams.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-systems.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-systems.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-tenants.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-tenants.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-tokens.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-tokens.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/openapi_v3-workflows.yml` & `tapipy-1.3.4/tapipy/resources/openapi_v3-workflows.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/resources/resource_etags.json` & `tapipy-1.3.4/tapipy/resources/resource_etags.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'authenticator'": '\'W/"16fca2e73ad502ffcc2da2c755df8d3abf680a6e"\'',*

 * * "'jobs'": '\'W/"eceba29d169471ccee3d1a1d0db8bff8374fffe2"\''}*

```diff
@@ -1,13 +1,13 @@
 {
     "actors": "W/\"790d47ac8c8c65e702080db8e564c154ee3ba420\"",
     "apps": "W/\"a1560cf120d77dcbc4adf9ad31646a2b504d2a96\"",
-    "authenticator": "W/\"e81fcd4d421ec0a30d25bcfe7bb039af27c9acd1\"",
+    "authenticator": "W/\"16fca2e73ad502ffcc2da2c755df8d3abf680a6e\"",
     "files": "W/\"a5877986f5ce5feefc53dda54f64b913415e32b6\"",
-    "jobs": "W/\"ed61f6fb359161059940c6eb0a28175b58dc42c9\"",
+    "jobs": "W/\"eceba29d169471ccee3d1a1d0db8bff8374fffe2\"",
     "meta": "W/\"e49bc20f1b1e3296278db40fdd6b33d92c44beea\"",
     "notifications": "W/\"93c92b6a473db7d5e02a0cebde5c91b2c706c63a\"",
     "pgrest": "W/\"6494d146379036fdd95de0ed7da22d1bec1335cd\"",
     "pods": "W/\"d0f92c40b0ccec6f194257b75e335bb2352b00dc\"",
     "sk": "W/\"1d60d95dc6576e129817e90c107bd4daf0200e4c\"",
     "streams": "W/\"d48bb1cdc3a01f8b4b42ecacc9f41585c29a660b\"",
     "systems": "W/\"f829e4bef48b3b2e8d05ffa73af2f5f5f1ad6dcf\"",
```

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-pods_service-prod-docs-openapi_v3-pods.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 959d 4b00 0000 0000 007d 9428 8c07  ....K......}.(..
+00000000: 8004 957d 4c00 0000 0000 007d 9428 8c07  ...}L......}.(..
 00000010: 6f70 656e 6170 6994 8c05 332e 302e 3294  openapi...3.0.2.
 00000020: 8c04 696e 666f 947d 9428 8c05 7469 746c  ..info.}.(..titl
 00000030: 6594 8c0d 4175 7468 656e 7469 6361 746f  e...Authenticato
 00000040: 7294 8c0b 6465 7363 7269 7074 696f 6e94  r...description.
 00000050: 8c49 5245 5354 2041 5049 2061 6e64 2077  .IREST API and w
 00000060: 6562 2073 6572 7665 7220 7072 6f76 6964  eb server provid
 00000070: 696e 6720 6175 7468 656e 7469 6361 7469  ing authenticati
@@ -1182,30 +1182,44 @@
 000049d0: 758c 0e61 7272 6179 4f66 436c 6965 6e74  u..arrayOfClient
 000049e0: 7394 7d94 288c 0474 7970 6594 8c05 6172  s.}.(..type...ar
 000049f0: 7261 7994 8c05 6974 656d 7394 7d94 8c04  ray...items.}...
 00004a00: 2472 6566 948c 1b23 2f63 6f6d 706f 6e65  $ref...#/compone
 00004a10: 6e74 732f 7363 6865 6d61 732f 436c 6965  nts/schemas/Clie
 00004a20: 6e74 9473 758c 0750 726f 6669 6c65 947d  nt.su..Profile.}
 00004a30: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
-00004a40: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
-00004a50: 9428 8c08 7573 6572 6e61 6d65 947d 9428  .(..username.}.(
-00004a60: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00004a70: 8c0b 6465 7363 7269 7074 696f 6e94 8c29  ..description..)
-00004a80: 5468 6520 7573 6572 6e61 6d65 2061 7373  The username ass
-00004a90: 6f63 6961 7465 6420 7769 7468 2074 6865  ociated with the
-00004aa0: 2070 726f 6669 6c65 2e94 758c 0565 6d61   profile..u..ema
-00004ab0: 696c 947d 9428 8c04 7479 7065 948c 0673  il.}.(..type...s
-00004ac0: 7472 696e 6794 8c0b 6465 7363 7269 7074  tring...descript
-00004ad0: 696f 6e94 8c2e 5468 6520 656d 6169 6c20  ion...The email 
-00004ae0: 6164 6472 6573 7320 6173 736f 6369 6174  address associat
-00004af0: 6564 2077 6974 6820 7468 6520 7072 6f66  ed with the prof
-00004b00: 696c 652e 9475 8c04 6e61 6d65 947d 9428  ile..u..name.}.(
-00004b10: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00004b20: 8c0b 6465 7363 7269 7074 696f 6e94 8c1a  ..description...
-00004b30: 5468 6520 6675 6c6c 206e 616d 6520 6f66  The full name of
-00004b40: 2074 6865 2075 7365 722e 9475 7575 8c0f   the user..uuu..
-00004b50: 6172 7261 794f 6650 726f 6669 6c65 7394  arrayOfProfiles.
-00004b60: 7d94 288c 0474 7970 6594 8c05 6172 7261  }.(..type...arra
-00004b70: 7994 8c05 6974 656d 7394 7d94 8c04 2472  y...items.}...$r
-00004b80: 6566 948c 1c23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-00004b90: 732f 7363 6865 6d61 732f 5072 6f66 696c  s/schemas/Profil
-00004ba0: 6594 7375 7573 752e                      e.suusu.
+00004a40: 7494 8c0b 6465 7363 7269 7074 696f 6e94  t...description.
+00004a50: 8ccf 5468 6520 7072 6f66 696c 6520 6173  ..The profile as
+00004a60: 736f 6369 6174 6564 2077 6974 6820 6120  sociated with a 
+00004a70: 5461 7069 7320 6964 656e 7469 7479 2e20  Tapis identity. 
+00004a80: 4e4f 5445 202d 7468 6520 6669 656c 6473  NOTE -the fields
+00004a90: 2069 6e20 7468 6520 5072 6f66 696c 6520   in the Profile 
+00004aa0: 6f62 6a65 6374 2061 7265 2070 6f70 756c  object are popul
+00004ab0: 6174 6564 206f 6e20 6120 6265 7374 2d65  ated on a best-e
+00004ac0: 6666 6f72 7420 6261 7369 7320 616e 6420  ffort basis and 
+00004ad0: 7368 6f75 6c64 206e 6f74 2062 6520 7265  should not be re
+00004ae0: 6c69 6564 2075 706f 6e2e 204f 6e6c 7920  lied upon. Only 
+00004af0: 7468 6520 7573 6572 6e61 6d65 2066 6965  the username fie
+00004b00: 6c64 2069 7320 6775 6172 616e 7465 6564  ld is guaranteed
+00004b10: 2074 6f20 6265 2070 6f70 756c 6174 6564   to be populated
+00004b20: 2e94 8c0a 7072 6f70 6572 7469 6573 947d  ....properties.}
+00004b30: 9428 8c08 7573 6572 6e61 6d65 947d 9428  .(..username.}.(
+00004b40: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+00004b50: 8c0b 6465 7363 7269 7074 696f 6e94 8c29  ..description..)
+00004b60: 5468 6520 7573 6572 6e61 6d65 2061 7373  The username ass
+00004b70: 6f63 6961 7465 6420 7769 7468 2074 6865  ociated with the
+00004b80: 2070 726f 6669 6c65 2e94 758c 0565 6d61   profile..u..ema
+00004b90: 696c 947d 9428 8c04 7479 7065 948c 0673  il.}.(..type...s
+00004ba0: 7472 696e 6794 8c0b 6465 7363 7269 7074  tring...descript
+00004bb0: 696f 6e94 8c2e 5468 6520 656d 6169 6c20  ion...The email 
+00004bc0: 6164 6472 6573 7320 6173 736f 6369 6174  address associat
+00004bd0: 6564 2077 6974 6820 7468 6520 7072 6f66  ed with the prof
+00004be0: 696c 652e 9475 8c04 6e61 6d65 947d 9428  ile..u..name.}.(
+00004bf0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+00004c00: 8c0b 6465 7363 7269 7074 696f 6e94 8c1a  ..description...
+00004c10: 5468 6520 6675 6c6c 206e 616d 6520 6f66  The full name of
+00004c20: 2074 6865 2075 7365 722e 9475 7575 8c0f   the user..uuu..
+00004c30: 6172 7261 794f 6650 726f 6669 6c65 7394  arrayOfProfiles.
+00004c40: 7d94 288c 0474 7970 6594 8c05 6172 7261  }.(..type...arra
+00004c50: 7994 8c05 6974 656d 7394 7d94 8c04 2472  y...items.}...$r
+00004c60: 6566 948c 1c23 2f63 6f6d 706f 6e65 6e74  ef...#/component
+00004c70: 732f 7363 6865 6d61 732f 5072 6f66 696c  s/schemas/Profil
+00004c80: 6594 7375 7573 752e                      e.suusu.
```

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9542 c100 0000 0000 007d 9428 8c07  ...B.......}.(..
+00000000: 8004 953e c300 0000 0000 007d 9428 8c07  ...>.......}.(..
 00000010: 6f70 656e 6170 6994 8c05 332e 302e 3194  openapi...3.0.1.
 00000020: 8c04 696e 666f 947d 9428 8c05 7469 746c  ..info.}.(..titl
 00000030: 6594 8c0e 5461 7069 7320 4a6f 6273 2041  e...Tapis Jobs A
 00000040: 5049 948c 0b64 6573 6372 6970 7469 6f6e  PI...description
 00000050: 948c 3254 6865 2054 6170 6973 204a 6f62  ..2The Tapis Job
 00000060: 7320 4150 4920 6578 6563 7574 6573 206a  s API executes j
 00000070: 6f62 7320 6f6e 2054 6170 6973 2073 7973  obs on Tapis sys
@@ -656,2438 +656,2470 @@
 000028f0: 7269 7479 945d 947d 948c 0854 6170 6973  rity.].}...Tapis
 00002900: 4a57 5494 5d94 7361 7573 8c2c 2f6a 6f62  JWT.].saus.,/job
 00002910: 732f 7b6a 6f62 5575 6964 7d2f 6f75 7470  s/{jobUuid}/outp
 00002920: 7574 2f64 6f77 6e6c 6f61 642f 7b6f 7574  ut/download/{out
 00002930: 7075 7450 6174 687d 947d 948c 0367 6574  putPath}.}...get
 00002940: 947d 9428 8c04 7461 6773 945d 948c 046a  .}.(..tags.]...j
 00002950: 6f62 7394 618c 0b64 6573 6372 6970 7469  obs.a..descripti
-00002960: 6f6e 9458 1d01 0000 446f 776e 6c6f 6164  on.X....Download
+00002960: 6f6e 9458 ca01 0000 446f 776e 6c6f 6164  on.X....Download
 00002970: 206a 6f62 2773 206f 7574 7075 7420 6669   job's output fi
 00002980: 6c65 7320 666f 7220 7072 6576 696f 7573  les for previous
 00002990: 6c79 2073 7562 6d69 7474 6564 206a 6f62  ly submitted job
-000029a0: 2062 7920 6974 7320 5555 4944 2e20 5468   by its UUID. Th
-000029b0: 6520 6a6f 6220 6d75 7374 2062 6520 696e  e job must be in
-000029c0: 2061 2074 6572 6d69 6e61 6c20 7374 6174   a terminal stat
-000029d0: 6520 2846 494e 4953 4845 4420 6f72 2046  e (FINISHED or F
-000029e0: 4149 4c45 4420 6f72 2043 414e 4345 4c4c  AILED or CANCELL
-000029f0: 4544 292e 2020 0a0a 5468 6520 6361 6c6c  ED).  ..The call
-00002a00: 6572 206d 7573 7420 6265 2074 6865 206a  er must be the j
-00002a10: 6f62 206f 776e 6572 2c20 6372 6561 746f  ob owner, creato
-00002a20: 7220 6f72 2061 2074 656e 616e 7420 6164  r or a tenant ad
-00002a30: 6d69 6e69 7374 7261 746f 722e 0a54 6865  ministrator..The
-00002a40: 2055 524c 206d 7573 7420 656e 6473 2077   URL must ends w
-00002a50: 6974 6820 272f 2720 6576 656e 2069 6620  ith '/' even if 
-00002a60: 7468 6572 6520 6973 206e 6f20 6f75 7470  there is no outp
-00002a70: 7574 5061 7468 2069 7320 7370 6563 6966  utPath is specif
-00002a80: 6965 642e 2094 8c0b 6f70 6572 6174 696f  ied. ...operatio
-00002a90: 6e49 6494 8c14 6765 744a 6f62 4f75 7470  nId...getJobOutp
-00002aa0: 7574 446f 776e 6c6f 6164 948c 0a70 6172  utDownload...par
-00002ab0: 616d 6574 6572 7394 5d94 287d 9428 8c04  ameters.].(}.(..
-00002ac0: 6e61 6d65 948c 076a 6f62 5575 6964 948c  name...jobUuid..
-00002ad0: 0269 6e94 8c04 7061 7468 948c 0872 6571  .in...path...req
-00002ae0: 7569 7265 6494 888c 0673 6368 656d 6194  uired....schema.
-00002af0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-00002b00: 6794 7375 7d94 288c 046e 616d 6594 8c0a  g.su}.(..name...
-00002b10: 6f75 7470 7574 5061 7468 948c 0269 6e94  outputPath...in.
-00002b20: 8c04 7061 7468 948c 0872 6571 7569 7265  ..path...require
-00002b30: 6494 888c 0673 6368 656d 6194 7d94 288c  d....schema.}.(.
-00002b40: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
-00002b50: 0764 6566 6175 6c74 948c 0094 7575 7d94  .default....uu}.
-00002b60: 288c 046e 616d 6594 8c08 636f 6d70 7265  (..name...compre
-00002b70: 7373 948c 0269 6e94 8c05 7175 6572 7994  ss...in...query.
-00002b80: 8c06 7363 6865 6d61 947d 9428 8c04 7479  ..schema.}.(..ty
-00002b90: 7065 948c 0762 6f6f 6c65 616e 948c 0764  pe...boolean...d
-00002ba0: 6566 6175 6c74 9489 7575 7d94 288c 046e  efault..uu}.(..n
-00002bb0: 616d 6594 8c06 666f 726d 6174 948c 0269  ame...format...i
-00002bc0: 6e94 8c05 7175 6572 7994 8c06 7363 6865  n...query...sche
-00002bd0: 6d61 947d 9428 8c04 7479 7065 948c 0673  ma.}.(..type...s
-00002be0: 7472 696e 6794 8c07 6465 6661 756c 7494  tring...default.
-00002bf0: 8c03 7a69 7094 7575 7d94 288c 046e 616d  ..zip.uu}.(..nam
-00002c00: 6594 8c06 7072 6574 7479 948c 0269 6e94  e...pretty...in.
-00002c10: 8c05 7175 6572 7994 8c06 7363 6865 6d61  ..query...schema
-00002c20: 947d 9428 8c04 7479 7065 948c 0762 6f6f  .}.(..type...boo
-00002c30: 6c65 616e 948c 0764 6566 6175 6c74 9489  lean...default..
-00002c40: 7575 658c 0972 6573 706f 6e73 6573 947d  uue..responses.}
-00002c50: 9428 8c03 3230 3094 7d94 288c 0b64 6573  .(..200.}.(..des
-00002c60: 6372 6970 7469 6f6e 948c 1e4a 6f62 2773  cription...Job's
-00002c70: 206f 7574 7075 7420 6669 6c65 7320 646f   output files do
-00002c80: 776e 6c6f 6164 6564 2e94 8c07 636f 6e74  wnloaded....cont
-00002c90: 656e 7494 7d94 8c18 6170 706c 6963 6174  ent.}...applicat
-00002ca0: 696f 6e2f 6f63 7465 742d 7374 7265 616d  ion/octet-stream
-00002cb0: 947d 948c 0673 6368 656d 6194 7d94 288c  .}...schema.}.(.
-00002cc0: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
-00002cd0: 0666 6f72 6d61 7494 8c06 6269 6e61 7279  .format...binary
-00002ce0: 9475 7373 758c 0334 3030 947d 9428 8c0b  .ussu..400.}.(..
-00002cf0: 6465 7363 7269 7074 696f 6e94 8c0c 496e  description...In
-00002d00: 7075 7420 6572 726f 722e 948c 0763 6f6e  put error....con
-00002d10: 7465 6e74 947d 948c 1861 7070 6c69 6361  tent.}...applica
-00002d20: 7469 6f6e 2f6f 6374 6574 2d73 7472 6561  tion/octet-strea
-00002d30: 6d94 7d94 8c06 7363 6865 6d61 947d 948c  m.}...schema.}..
-00002d40: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
-00002d50: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
-00002d60: 7042 6173 6963 9473 7373 758c 0334 3031  pBasic.sssu..401
-00002d70: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-00002d80: 6e94 8c0f 4e6f 7420 6175 7468 6f72 697a  n...Not authoriz
-00002d90: 6564 2e94 8c07 636f 6e74 656e 7494 7d94  ed....content.}.
-00002da0: 8c18 6170 706c 6963 6174 696f 6e2f 6f63  ..application/oc
-00002db0: 7465 742d 7374 7265 616d 947d 948c 0673  tet-stream.}...s
-00002dc0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00002dd0: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
-00002de0: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
-00002df0: 7373 7375 8c03 3430 3394 7d94 288c 0b64  sssu..403.}.(..d
-00002e00: 6573 6372 6970 7469 6f6e 948c 0a46 6f72  escription...For
-00002e10: 6269 6464 656e 2e94 8c07 636f 6e74 656e  bidden....conten
-00002e20: 7494 7d94 8c18 6170 706c 6963 6174 696f  t.}...applicatio
-00002e30: 6e2f 6f63 7465 742d 7374 7265 616d 947d  n/octet-stream.}
-00002e40: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-00002e50: 6566 948c 1e23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-00002e60: 732f 7363 6865 6d61 732f 5265 7370 4261  s/schemas/RespBa
-00002e70: 7369 6394 7373 7375 8c03 3430 3494 7d94  sic.sssu..404.}.
-00002e80: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-00002e90: 0e4a 6f62 206e 6f74 2066 6f75 6e64 2e94  .Job not found..
-00002ea0: 8c07 636f 6e74 656e 7494 7d94 8c18 6170  ..content.}...ap
-00002eb0: 706c 6963 6174 696f 6e2f 6f63 7465 742d  plication/octet-
-00002ec0: 7374 7265 616d 947d 948c 0673 6368 656d  stream.}...schem
-00002ed0: 6194 7d94 8c04 2472 6566 948c 1d23 2f63  a.}...$ref...#/c
-00002ee0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-00002ef0: 732f 5265 7370 4e61 6d65 9473 7373 758c  s/RespName.sssu.
-00002f00: 0335 3030 947d 9428 8c0b 6465 7363 7269  .500.}.(..descri
-00002f10: 7074 696f 6e94 8c0d 5365 7276 6572 2065  ption...Server e
-00002f20: 7272 6f72 2e94 8c07 636f 6e74 656e 7494  rror....content.
-00002f30: 7d94 8c18 6170 706c 6963 6174 696f 6e2f  }...application/
-00002f40: 6f63 7465 742d 7374 7265 616d 947d 948c  octet-stream.}..
-00002f50: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00002f60: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
-00002f70: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
-00002f80: 6394 7373 7375 758c 0873 6563 7572 6974  c.sssuu..securit
-00002f90: 7994 5d94 7d94 8c08 5461 7069 734a 5754  y.].}...TapisJWT
-00002fa0: 945d 9473 6175 738c 282f 6a6f 6273 2f7b  .].saus.(/jobs/{
-00002fb0: 6a6f 6255 7569 647d 2f6f 7574 7075 742f  jobUuid}/output/
-00002fc0: 6c69 7374 2f7b 6f75 7470 7574 5061 7468  list/{outputPath
-00002fd0: 7d94 7d94 8c03 6765 7494 7d94 288c 0474  }.}...get.}.(..t
-00002fe0: 6167 7394 5d94 8c04 6a6f 6273 9461 8c0b  ags.]...jobs.a..
-00002ff0: 6465 7363 7269 7074 696f 6e94 5821 0100  description.X!..
-00003000: 0052 6574 7269 6576 6520 6a6f 6227 7320  .Retrieve job's 
-00003010: 6f75 7470 7574 2066 696c 6573 206c 6973  output files lis
-00003020: 7420 666f 7220 7072 6576 696f 7573 6c79  t for previously
-00003030: 2073 7562 6d69 7474 6564 206a 6f62 2062   submitted job b
-00003040: 7920 6974 7320 5555 4944 2e20 5468 6520  y its UUID. The 
-00003050: 6a6f 6220 6d75 7374 2062 6520 696e 2061  job must be in a
-00003060: 2074 6572 6d69 6e61 6c20 7374 6174 6520   terminal state 
-00003070: 2846 494e 4953 4845 4420 6f72 2046 4149  (FINISHED or FAI
-00003080: 4c45 4420 6f72 2043 414e 4345 4c4c 4544  LED or CANCELLED
-00003090: 2920 200a 0a54 6865 2063 616c 6c65 7220  )  ..The caller 
-000030a0: 6d75 7374 2062 6520 7468 6520 6a6f 6220  must be the job 
-000030b0: 6f77 6e65 722c 2063 7265 6174 6f72 206f  owner, creator o
-000030c0: 7220 6120 7465 6e61 6e74 2061 646d 696e  r a tenant admin
-000030d0: 6973 7472 6174 6f72 2e0a 5468 6520 5552  istrator..The UR
-000030e0: 4c20 6d75 7374 2065 6e64 7320 7769 7468  L must ends with
-000030f0: 2027 2f27 2065 7665 6e20 6966 2074 6865   '/' even if the
-00003100: 7265 2069 7320 6e6f 206f 7574 7075 7450  re is no outputP
-00003110: 6174 6820 6973 2073 7065 6369 6669 6564  ath is specified
-00003120: 2e20 948c 0b6f 7065 7261 7469 6f6e 4964  . ...operationId
-00003130: 948c 1067 6574 4a6f 624f 7574 7075 744c  ...getJobOutputL
-00003140: 6973 7494 8c0a 7061 7261 6d65 7465 7273  ist...parameters
-00003150: 945d 9428 7d94 288c 046e 616d 6594 8c07  .].(}.(..name...
-00003160: 6a6f 6255 7569 6494 8c02 696e 948c 0470  jobUuid...in...p
-00003170: 6174 6894 8c08 7265 7175 6972 6564 9488  ath...required..
-00003180: 8c06 7363 6865 6d61 947d 948c 0474 7970  ..schema.}...typ
-00003190: 6594 8c06 7374 7269 6e67 9473 757d 9428  e...string.su}.(
-000031a0: 8c04 6e61 6d65 948c 0a6f 7574 7075 7450  ..name...outputP
-000031b0: 6174 6894 8c02 696e 948c 0470 6174 6894  ath...in...path.
-000031c0: 8c08 7265 7175 6972 6564 9488 8c06 7363  ..required....sc
-000031d0: 6865 6d61 947d 9428 8c04 7479 7065 948c  hema.}.(..type..
-000031e0: 0673 7472 696e 6794 8c07 6465 6661 756c  .string...defaul
-000031f0: 7494 6adc 0300 0075 757d 9428 8c04 6e61  t.j....uu}.(..na
-00003200: 6d65 948c 056c 696d 6974 948c 0269 6e94  me...limit...in.
-00003210: 8c05 7175 6572 7994 8c06 7363 6865 6d61  ..query...schema
-00003220: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
-00003230: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
-00003240: 696e 7433 3294 7575 7d94 288c 046e 616d  int32.uu}.(..nam
-00003250: 6594 8c04 736b 6970 948c 0269 6e94 8c05  e...skip...in...
-00003260: 7175 6572 7994 8c06 7363 6865 6d61 947d  query...schema.}
-00003270: 9428 8c04 7479 7065 948c 0769 6e74 6567  .(..type...integ
-00003280: 6572 948c 0666 6f72 6d61 7494 8c05 696e  er...format...in
-00003290: 7433 3294 7575 7d94 288c 046e 616d 6594  t32.uu}.(..name.
-000032a0: 8c06 7072 6574 7479 948c 0269 6e94 8c05  ..pretty...in...
-000032b0: 7175 6572 7994 8c06 7363 6865 6d61 947d  query...schema.}
-000032c0: 9428 8c04 7479 7065 948c 0762 6f6f 6c65  .(..type...boole
-000032d0: 616e 948c 0764 6566 6175 6c74 9489 7575  an...default..uu
-000032e0: 658c 0972 6573 706f 6e73 6573 947d 9428  e..responses.}.(
-000032f0: 8c03 3230 3094 7d94 288c 0b64 6573 6372  ..200.}.(..descr
-00003300: 6970 7469 6f6e 948c 224a 6f62 2773 206f  iption.."Job's o
-00003310: 7574 7075 7420 6669 6c65 7320 6c69 7374  utput files list
-00003320: 2072 6574 7269 6576 6564 2e94 8c07 636f   retrieved....co
-00003330: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00003340: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00003350: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00003360: 2923 2f63 6f6d 706f 6e65 6e74 732f 7363  )#/components/sc
-00003370: 6865 6d61 732f 5265 7370 4765 744a 6f62  hemas/RespGetJob
-00003380: 4f75 7470 7574 4c69 7374 9473 7373 758c  OutputList.sssu.
-00003390: 0334 3030 947d 9428 8c0b 6465 7363 7269  .400.}.(..descri
-000033a0: 7074 696f 6e94 8c0c 496e 7075 7420 6572  ption...Input er
-000033b0: 726f 722e 948c 0763 6f6e 7465 6e74 947d  ror....content.}
-000033c0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-000033d0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-000033e0: 948c 0424 7265 6694 8c1e 232f 636f 6d70  ...$ref...#/comp
-000033f0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
-00003400: 6573 7042 6173 6963 9473 7373 758c 0334  espBasic.sssu..4
-00003410: 3031 947d 9428 8c0b 6465 7363 7269 7074  01.}.(..descript
-00003420: 696f 6e94 8c0f 4e6f 7420 6175 7468 6f72  ion...Not author
-00003430: 697a 6564 2e94 8c07 636f 6e74 656e 7494  ized....content.
-00003440: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00003450: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00003460: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
-00003470: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00003480: 5265 7370 4261 7369 6394 7373 7375 8c03  RespBasic.sssu..
-00003490: 3430 3394 7d94 288c 0b64 6573 6372 6970  403.}.(..descrip
-000034a0: 7469 6f6e 948c 0a46 6f72 6269 6464 656e  tion...Forbidden
-000034b0: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
-000034c0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-000034d0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-000034e0: 2472 6566 948c 1e23 2f63 6f6d 706f 6e65  $ref...#/compone
-000034f0: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
-00003500: 4261 7369 6394 7373 7375 8c03 3430 3494  Basic.sssu..404.
-00003510: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00003520: 948c 0e4a 6f62 206e 6f74 2066 6f75 6e64  ...Job not found
-00003530: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
-00003540: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00003550: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00003560: 2472 6566 948c 1d23 2f63 6f6d 706f 6e65  $ref...#/compone
-00003570: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
-00003580: 4e61 6d65 9473 7373 758c 0335 3030 947d  Name.sssu..500.}
-00003590: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-000035a0: 8c0d 5365 7276 6572 2065 7272 6f72 2e94  ..Server error..
-000035b0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
-000035c0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
-000035d0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-000035e0: 6566 948c 1e23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-000035f0: 732f 7363 6865 6d61 732f 5265 7370 4261  s/schemas/RespBa
-00003600: 7369 6394 7373 7375 758c 0873 6563 7572  sic.sssuu..secur
-00003610: 6974 7994 5d94 7d94 8c08 5461 7069 734a  ity.].}...TapisJ
-00003620: 5754 945d 9473 6175 738c 0c2f 6a6f 6273  WT.].saus../jobs
-00003630: 2f73 6561 7263 6894 7d94 288c 0367 6574  /search.}.(..get
-00003640: 947d 9428 8c04 7461 6773 945d 948c 046a  .}.(..tags.]...j
-00003650: 6f62 7394 618c 0b64 6573 6372 6970 7469  obs.a..descripti
-00003660: 6f6e 948c f552 6574 7269 6576 6520 6c69  on...Retrieve li
-00003670: 7374 206f 6620 6a6f 6273 2066 6f72 2074  st of jobs for t
-00003680: 6865 2075 7365 7220 6261 7365 6420 6f6e  he user based on
-00003690: 2073 6561 7263 6820 636f 6e64 6974 696f   search conditio
-000036a0: 6e73 2069 6e20 7468 6520 7175 6572 7920  ns in the query 
-000036b0: 7061 7261 6d74 6572 206f 6e20 7468 6520  paramter on the 
-000036c0: 6465 6469 6361 7465 6420 7365 6172 6368  dedicated search
-000036d0: 2065 6e64 2d70 6f69 6e74 2e0a 0a54 6865   end-point...The
-000036e0: 2063 616c 6c65 7220 6d75 7374 2062 6520   caller must be 
-000036f0: 7468 6520 6a6f 6220 6f77 6e65 722c 2063  the job owner, c
-00003700: 7265 6174 6f72 206f 7220 6120 7465 6e61  reator or a tena
-00003710: 6e74 2061 646d 696e 6973 7472 6174 6f72  nt administrator
-00003720: 2e20 0a0a 4c69 7374 206f 6620 4a6f 6273  . ..List of Jobs
-00003730: 2073 6861 7265 6420 7769 7468 2074 6865   shared with the
-00003740: 2075 7365 7220 6361 6e20 616c 736f 2062   user can also b
-00003750: 6520 7365 6172 6368 6564 948c 0b6f 7065  e searched...ope
-00003760: 7261 7469 6f6e 4964 948c 1067 6574 4a6f  rationId...getJo
-00003770: 6253 6561 7263 684c 6973 7494 8c0a 7061  bSearchList...pa
-00003780: 7261 6d65 7465 7273 945d 9428 7d94 288c  rameters.].(}.(.
-00003790: 046e 616d 6594 8c05 6c69 6d69 7494 8c02  .name...limit...
-000037a0: 696e 948c 0571 7565 7279 948c 0673 6368  in...query...sch
-000037b0: 656d 6194 7d94 288c 0474 7970 6594 8c07  ema.}.(..type...
-000037c0: 696e 7465 6765 7294 8c06 666f 726d 6174  integer...format
-000037d0: 948c 0569 6e74 3332 9475 757d 9428 8c04  ...int32.uu}.(..
-000037e0: 6e61 6d65 948c 0473 6b69 7094 8c02 696e  name...skip...in
-000037f0: 948c 0571 7565 7279 948c 0673 6368 656d  ...query...schem
-00003800: 6194 7d94 288c 0474 7970 6594 8c07 696e  a.}.(..type...in
-00003810: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
-00003820: 0569 6e74 3332 9475 757d 9428 8c04 6e61  .int32.uu}.(..na
-00003830: 6d65 948c 0a73 7461 7274 4166 7465 7294  me...startAfter.
-00003840: 8c02 696e 948c 0571 7565 7279 948c 0673  ..in...query...s
-00003850: 6368 656d 6194 7d94 288c 0474 7970 6594  chema.}.(..type.
-00003860: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
-00003870: 6174 948c 0569 6e74 3332 9475 757d 9428  at...int32.uu}.(
-00003880: 8c04 6e61 6d65 948c 076f 7264 6572 4279  ..name...orderBy
-00003890: 948c 0269 6e94 8c05 7175 6572 7994 8c06  ...in...query...
-000038a0: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
-000038b0: 8c06 7374 7269 6e67 9473 757d 9428 8c04  ..string.su}.(..
-000038c0: 6e61 6d65 948c 0c63 6f6d 7075 7465 546f  name...computeTo
-000038d0: 7461 6c94 8c02 696e 948c 0571 7565 7279  tal...in...query
-000038e0: 948c 0673 6368 656d 6194 7d94 8c04 7479  ...schema.}...ty
-000038f0: 7065 948c 0762 6f6f 6c65 616e 9473 757d  pe...boolean.su}
-00003900: 9428 8c04 6e61 6d65 948c 0673 656c 6563  .(..name...selec
-00003910: 7494 8c02 696e 948c 0571 7565 7279 948c  t...in...query..
-00003920: 0673 6368 656d 6194 7d94 8c04 7479 7065  .schema.}...type
-00003930: 948c 0673 7472 696e 6794 7375 7d94 288c  ...string.su}.(.
-00003940: 046e 616d 6594 8c08 6c69 7374 5479 7065  .name...listType
-00003950: 948c 0269 6e94 8c05 7175 6572 7994 8c06  ...in...query...
-00003960: 7363 6865 6d61 947d 9428 8c04 7479 7065  schema.}.(..type
-00003970: 948c 0673 7472 696e 6794 8c07 6465 6661  ...string...defa
-00003980: 756c 7494 8c07 4d59 5f4a 4f42 5394 7575  ult...MY_JOBS.uu
-00003990: 7d94 288c 046e 616d 6594 8c06 7072 6574  }.(..name...pret
-000039a0: 7479 948c 0269 6e94 8c05 7175 6572 7994  ty...in...query.
-000039b0: 8c06 7363 6865 6d61 947d 9428 8c04 7479  ..schema.}.(..ty
-000039c0: 7065 948c 0762 6f6f 6c65 616e 948c 0764  pe...boolean...d
-000039d0: 6566 6175 6c74 9489 7575 658c 0972 6573  efault..uue..res
-000039e0: 706f 6e73 6573 947d 9428 8c03 3230 3094  ponses.}.(..200.
-000039f0: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00003a00: 948c 1b4a 6f62 7320 5365 6172 6368 204c  ...Jobs Search L
-00003a10: 6973 7420 7265 7472 6965 7665 642e 948c  ist retrieved...
-00003a20: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00003a30: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-00003a40: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00003a50: 6694 8c2f 232f 636f 6d70 6f6e 656e 7473  f../#/components
-00003a60: 2f73 6368 656d 6173 2f52 6573 704a 6f62  /schemas/RespJob
-00003a70: 5365 6172 6368 416c 6c41 7474 7269 6275  SearchAllAttribu
-00003a80: 7465 7394 7373 7375 8c03 3430 3094 7d94  tes.sssu..400.}.
-00003a90: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-00003aa0: 0c49 6e70 7574 2065 7272 6f72 2e94 8c07  .Input error....
-00003ab0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00003ac0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00003ad0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00003ae0: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
-00003af0: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
-00003b00: 6394 7373 7375 8c03 3430 3194 7d94 288c  c.sssu..401.}.(.
-00003b10: 0b64 6573 6372 6970 7469 6f6e 948c 0f4e  .description...N
-00003b20: 6f74 2061 7574 686f 7269 7a65 642e 948c  ot authorized...
-00003b30: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00003b40: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-00003b50: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00003b60: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
-00003b70: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
-00003b80: 6963 9473 7373 758c 0334 3033 947d 9428  ic.sssu..403.}.(
-00003b90: 8c0b 6465 7363 7269 7074 696f 6e94 8c0a  ..description...
-00003ba0: 466f 7262 6964 6465 6e2e 948c 0763 6f6e  Forbidden....con
-00003bb0: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00003bc0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00003bd0: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
-00003be0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-00003bf0: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
-00003c00: 7373 758c 0334 3034 947d 9428 8c0b 6465  ssu..404.}.(..de
-00003c10: 7363 7269 7074 696f 6e94 8c0f 4a6f 6273  scription...Jobs
-00003c20: 206e 6f74 2066 6f75 6e64 2e94 8c07 636f   not found....co
-00003c30: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00003c40: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00003c50: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00003c60: 1d23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
-00003c70: 6865 6d61 732f 5265 7370 4e61 6d65 9473  hemas/RespName.s
-00003c80: 7373 758c 0335 3030 947d 9428 8c0b 6465  ssu..500.}.(..de
-00003c90: 7363 7269 7074 696f 6e94 8c0d 5365 7276  scription...Serv
-00003ca0: 6572 2065 7272 6f72 2e94 8c07 636f 6e74  er error....cont
-00003cb0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00003cc0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00003cd0: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-00003ce0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00003cf0: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-00003d00: 7375 758c 0873 6563 7572 6974 7994 5d94  suu..security.].
-00003d10: 7d94 8c08 5461 7069 734a 5754 945d 9473  }...TapisJWT.].s
-00003d20: 6175 8c04 706f 7374 947d 9428 8c04 7461  au..post.}.(..ta
-00003d30: 6773 945d 948c 046a 6f62 7394 618c 0b64  gs.]...jobs.a..d
-00003d40: 6573 6372 6970 7469 6f6e 948c ed52 6574  escription...Ret
-00003d50: 7269 6576 6520 6c69 7374 206f 6620 6a6f  rieve list of jo
-00003d60: 6273 2066 6f72 2074 6865 2075 7365 7220  bs for the user 
-00003d70: 6261 7365 6420 6f6e 2073 6561 7263 6820  based on search 
-00003d80: 636f 6e64 6974 696f 6e73 2069 6e20 7468  conditions in th
-00003d90: 6520 7265 7175 6573 7420 626f 6479 2061  e request body a
-00003da0: 6e64 2070 6167 696e 6174 696f 6e20 696e  nd pagination in
-00003db0: 666f 726d 6174 696f 6e20 6672 6f6d 2074  formation from t
-00003dc0: 6865 2071 7565 7279 2070 6172 616d 7465  he query paramte
-00003dd0: 7220 6f6e 2074 6865 2064 6564 6963 6174  r on the dedicat
-00003de0: 6564 2073 6561 7263 6820 656e 642d 706f  ed search end-po
-00003df0: 696e 742e 0a0a 5468 6520 6361 6c6c 6572  int...The caller
-00003e00: 206d 7573 7420 6265 2074 6865 206a 6f62   must be the job
-00003e10: 206f 776e 6572 2c20 6372 6561 746f 7220   owner, creator 
-00003e20: 6f72 2061 2074 656e 616e 7420 6164 6d69  or a tenant admi
-00003e30: 6e69 7374 7261 746f 722e 948c 0b6f 7065  nistrator....ope
-00003e40: 7261 7469 6f6e 4964 948c 1c67 6574 4a6f  rationId...getJo
-00003e50: 6253 6561 7263 684c 6973 7442 7950 6f73  bSearchListByPos
-00003e60: 7453 716c 5374 7294 8c0a 7061 7261 6d65  tSqlStr...parame
-00003e70: 7465 7273 945d 9428 7d94 288c 046e 616d  ters.].(}.(..nam
-00003e80: 6594 8c05 6c69 6d69 7494 8c02 696e 948c  e...limit...in..
-00003e90: 0571 7565 7279 948c 0673 6368 656d 6194  .query...schema.
-00003ea0: 7d94 288c 0474 7970 6594 8c07 696e 7465  }.(..type...inte
-00003eb0: 6765 7294 8c06 666f 726d 6174 948c 0569  ger...format...i
-00003ec0: 6e74 3332 9475 757d 9428 8c04 6e61 6d65  nt32.uu}.(..name
-00003ed0: 948c 0473 6b69 7094 8c02 696e 948c 0571  ...skip...in...q
-00003ee0: 7565 7279 948c 0673 6368 656d 6194 7d94  uery...schema.}.
-00003ef0: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
-00003f00: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
-00003f10: 3332 9475 757d 9428 8c04 6e61 6d65 948c  32.uu}.(..name..
-00003f20: 0a73 7461 7274 4166 7465 7294 8c02 696e  .startAfter...in
-00003f30: 948c 0571 7565 7279 948c 0673 6368 656d  ...query...schem
-00003f40: 6194 7d94 288c 0474 7970 6594 8c07 696e  a.}.(..type...in
-00003f50: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
-00003f60: 0569 6e74 3332 9475 757d 9428 8c04 6e61  .int32.uu}.(..na
-00003f70: 6d65 948c 076f 7264 6572 4279 948c 0269  me...orderBy...i
-00003f80: 6e94 8c05 7175 6572 7994 8c06 7363 6865  n...query...sche
-00003f90: 6d61 947d 948c 0474 7970 6594 8c06 7374  ma.}...type...st
-00003fa0: 7269 6e67 9473 757d 9428 8c04 6e61 6d65  ring.su}.(..name
-00003fb0: 948c 0c63 6f6d 7075 7465 546f 7461 6c94  ...computeTotal.
-00003fc0: 8c02 696e 948c 0571 7565 7279 948c 0673  ..in...query...s
-00003fd0: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
-00003fe0: 0762 6f6f 6c65 616e 9473 757d 9428 8c04  .boolean.su}.(..
-00003ff0: 6e61 6d65 948c 0673 656c 6563 7494 8c02  name...select...
-00004000: 696e 948c 0571 7565 7279 948c 0673 6368  in...query...sch
-00004010: 656d 6194 7d94 8c04 7479 7065 948c 0673  ema.}...type...s
-00004020: 7472 696e 6794 7375 7d94 288c 046e 616d  tring.su}.(..nam
-00004030: 6594 8c08 6c69 7374 5479 7065 948c 0269  e...listType...i
-00004040: 6e94 8c05 7175 6572 7994 8c06 7363 6865  n...query...sche
-00004050: 6d61 947d 9428 8c04 7479 7065 948c 0673  ma.}.(..type...s
-00004060: 7472 696e 6794 8c07 6465 6661 756c 7494  tring...default.
-00004070: 8c07 4d59 5f4a 4f42 5394 7575 7d94 288c  ..MY_JOBS.uu}.(.
-00004080: 046e 616d 6594 8c06 7072 6574 7479 948c  .name...pretty..
-00004090: 0269 6e94 8c05 7175 6572 7994 8c06 7363  .in...query...sc
-000040a0: 6865 6d61 947d 9428 8c04 7479 7065 948c  hema.}.(..type..
-000040b0: 0762 6f6f 6c65 616e 948c 0764 6566 6175  .boolean...defau
-000040c0: 6c74 9489 7575 658c 0b72 6571 7565 7374  lt..uue..request
-000040d0: 426f 6479 947d 948c 0763 6f6e 7465 6e74  Body.}...content
-000040e0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-000040f0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00004100: 947d 948c 0474 7970 6594 8c06 6f62 6a65  .}...type...obje
-00004110: 6374 9473 7373 738c 0972 6573 706f 6e73  ct.ssss..respons
-00004120: 6573 947d 9428 8c03 3230 3094 7d94 288c  es.}.(..200.}.(.
-00004130: 0b64 6573 6372 6970 7469 6f6e 948c 1b4a  .description...J
-00004140: 6f62 7320 5365 6172 6368 204c 6973 7420  obs Search List 
-00004150: 7265 7472 6965 7665 642e 948c 0763 6f6e  retrieved....con
-00004160: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00004170: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00004180: 6865 6d61 947d 948c 0424 7265 6694 8c2f  hema.}...$ref../
-00004190: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-000041a0: 656d 6173 2f52 6573 704a 6f62 5365 6172  emas/RespJobSear
-000041b0: 6368 416c 6c41 7474 7269 6275 7465 7394  chAllAttributes.
-000041c0: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
-000041d0: 6573 6372 6970 7469 6f6e 948c 0c49 6e70  escription...Inp
-000041e0: 7574 2065 7272 6f72 2e94 8c07 636f 6e74  ut error....cont
-000041f0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00004200: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00004210: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-00004220: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00004230: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-00004240: 7375 8c03 3430 3194 7d94 288c 0b64 6573  su..401.}.(..des
-00004250: 6372 6970 7469 6f6e 948c 0f4e 6f74 2061  cription...Not a
-00004260: 7574 686f 7269 7a65 642e 948c 0763 6f6e  uthorized....con
-00004270: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00004280: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00004290: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
-000042a0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-000042b0: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
-000042c0: 7373 758c 0334 3033 947d 9428 8c0b 6465  ssu..403.}.(..de
-000042d0: 7363 7269 7074 696f 6e94 8c0a 466f 7262  scription...Forb
-000042e0: 6964 6465 6e2e 948c 0763 6f6e 7465 6e74  idden....content
-000042f0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00004300: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00004310: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
-00004320: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00004330: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
-00004340: 0334 3034 947d 9428 8c0b 6465 7363 7269  .404.}.(..descri
-00004350: 7074 696f 6e94 8c0f 4a6f 6273 206e 6f74  ption...Jobs not
-00004360: 2066 6f75 6e64 2e94 8c07 636f 6e74 656e   found....conten
-00004370: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
-00004380: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
-00004390: 6194 7d94 8c04 2472 6566 948c 1d23 2f63  a.}...$ref...#/c
-000043a0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-000043b0: 732f 5265 7370 4e61 6d65 9473 7373 758c  s/RespName.sssu.
-000043c0: 0335 3030 947d 9428 8c0b 6465 7363 7269  .500.}.(..descri
-000043d0: 7074 696f 6e94 8c0d 5365 7276 6572 2065  ption...Server e
-000043e0: 7272 6f72 2e94 8c07 636f 6e74 656e 7494  rror....content.
-000043f0: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00004400: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00004410: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
-00004420: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00004430: 5265 7370 4261 7369 6394 7373 7375 758c  RespBasic.sssuu.
-00004440: 0873 6563 7572 6974 7994 5d94 7d94 8c08  .security.].}...
-00004450: 5461 7069 734a 5754 945d 9473 6175 758c  TapisJWT.].sauu.
-00004460: 1c2f 6a6f 6273 2f7b 6a6f 6255 7569 647d  ./jobs/{jobUuid}
-00004470: 2f73 6861 7265 2f7b 7573 6572 7d94 7d94  /share/{user}.}.
-00004480: 8c06 6465 6c65 7465 947d 9428 8c04 7461  ..delete.}.(..ta
-00004490: 6773 945d 948c 0573 6861 7265 9461 8c0b  gs.]...share.a..
-000044a0: 6465 7363 7269 7074 696f 6e94 8c91 4465  description...De
-000044b0: 6c65 7465 2061 6c6c 2073 6861 7265 2069  lete all share i
-000044c0: 6e66 6f72 6d61 7469 6f6e 206f 6620 6120  nformation of a 
-000044d0: 7072 6576 696f 7573 6c79 2073 6861 7265  previously share
-000044e0: 6420 6a6f 6220 666f 7220 6120 7370 6563  d job for a spec
-000044f0: 6966 6963 2075 7365 720a 0a54 6865 2063  ific user..The c
-00004500: 616c 6c65 7220 6d75 7374 2062 6520 7468  aller must be th
-00004510: 6520 6a6f 6220 6f77 6e65 722c 2063 7265  e job owner, cre
-00004520: 6174 6f72 206f 7220 6120 7465 6e61 6e74  ator or a tenant
-00004530: 2061 646d 696e 6973 7472 6174 6f72 2e94   administrator..
-00004540: 8c0b 6f70 6572 6174 696f 6e49 6494 8c0e  ..operationId...
-00004550: 6465 6c65 7465 4a6f 6253 6861 7265 948c  deleteJobShare..
-00004560: 0a70 6172 616d 6574 6572 7394 5d94 287d  .parameters.].(}
-00004570: 9428 8c04 6e61 6d65 948c 076a 6f62 5575  .(..name...jobUu
-00004580: 6964 948c 0269 6e94 8c04 7061 7468 948c  id...in...path..
-00004590: 0872 6571 7569 7265 6494 888c 0673 6368  .required....sch
-000045a0: 656d 6194 7d94 8c04 7479 7065 948c 0673  ema.}...type...s
-000045b0: 7472 696e 6794 7375 7d94 288c 046e 616d  tring.su}.(..nam
-000045c0: 6594 8c04 7573 6572 948c 0269 6e94 8c04  e...user...in...
-000045d0: 7061 7468 948c 0872 6571 7569 7265 6494  path...required.
-000045e0: 888c 0673 6368 656d 6194 7d94 8c04 7479  ...schema.}...ty
-000045f0: 7065 948c 0673 7472 696e 6794 7375 7d94  pe...string.su}.
-00004600: 288c 046e 616d 6594 8c06 7072 6574 7479  (..name...pretty
-00004610: 948c 0269 6e94 8c05 7175 6572 7994 8c06  ...in...query...
-00004620: 7363 6865 6d61 947d 9428 8c04 7479 7065  schema.}.(..type
-00004630: 948c 0762 6f6f 6c65 616e 948c 0764 6566  ...boolean...def
-00004640: 6175 6c74 9489 7575 658c 0972 6573 706f  ault..uue..respo
-00004650: 6e73 6573 947d 9428 8c03 3230 3094 7d94  nses.}.(..200.}.
-00004660: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-00004670: 344a 6f62 2773 2073 6861 7265 2069 6e66  4Job's share inf
-00004680: 6f72 6d61 7469 6f6e 2064 656c 6574 6564  ormation deleted
-00004690: 2066 6f72 2061 2073 7065 6369 6669 6320   for a specific 
-000046a0: 7573 6572 2e94 8c07 636f 6e74 656e 7494  user....content.
-000046b0: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-000046c0: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-000046d0: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
-000046e0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-000046f0: 5265 7370 556e 5368 6172 654a 6f62 9473  RespUnShareJob.s
-00004700: 7373 758c 0334 3030 947d 9428 8c0b 6465  ssu..400.}.(..de
-00004710: 7363 7269 7074 696f 6e94 8c0c 496e 7075  scription...Inpu
-00004720: 7420 6572 726f 722e 948c 0763 6f6e 7465  t error....conte
-00004730: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00004740: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00004750: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
-00004760: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00004770: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
-00004780: 758c 0334 3031 947d 9428 8c0b 6465 7363  u..401.}.(..desc
-00004790: 7269 7074 696f 6e94 8c0f 4e6f 7420 6175  ription...Not au
-000047a0: 7468 6f72 697a 6564 2e94 8c07 636f 6e74  thorized....cont
-000047b0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-000047c0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-000047d0: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-000047e0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-000047f0: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-00004800: 7375 8c03 3430 3394 7d94 288c 0b64 6573  su..403.}.(..des
-00004810: 6372 6970 7469 6f6e 948c 0a46 6f72 6269  cription...Forbi
-00004820: 6464 656e 2e94 8c07 636f 6e74 656e 7494  dden....content.
-00004830: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00004840: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00004850: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
-00004860: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00004870: 5265 7370 4261 7369 6394 7373 7375 8c03  RespBasic.sssu..
-00004880: 3430 3494 7d94 288c 0b64 6573 6372 6970  404.}.(..descrip
-00004890: 7469 6f6e 948c 0e4a 6f62 206e 6f74 2066  tion...Job not f
-000048a0: 6f75 6e64 2e94 8c07 636f 6e74 656e 7494  ound....content.
-000048b0: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-000048c0: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-000048d0: 7d94 8c04 2472 6566 948c 1d23 2f63 6f6d  }...$ref...#/com
-000048e0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-000048f0: 5265 7370 4e61 6d65 9473 7373 758c 0335  RespName.sssu..5
-00004900: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00004910: 696f 6e94 8c0d 5365 7276 6572 2065 7272  ion...Server err
-00004920: 6f72 2e94 8c07 636f 6e74 656e 7494 7d94  or....content.}.
-00004930: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-00004940: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-00004950: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
-00004960: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
-00004970: 7370 4261 7369 6394 7373 7375 758c 0873  spBasic.sssuu..s
-00004980: 6563 7572 6974 7994 5d94 7d94 8c08 5461  ecurity.].}...Ta
-00004990: 7069 734a 5754 945d 9473 6175 738c 152f  pisJWT.].saus../
-000049a0: 6a6f 6273 2f7b 6a6f 6255 7569 647d 2f73  jobs/{jobUuid}/s
-000049b0: 6861 7265 947d 9428 8c03 6765 7494 7d94  hare.}.(..get.}.
-000049c0: 288c 0474 6167 7394 5d94 8c05 7368 6172  (..tags.]...shar
-000049d0: 6594 618c 0b64 6573 6372 6970 7469 6f6e  e.a..description
-000049e0: 948c 7652 6574 7269 6576 6520 7368 6172  ..vRetrieve shar
-000049f0: 6520 696e 666f 726d 6174 696f 6e20 6f66  e information of
-00004a00: 2061 206a 6f62 2062 7920 6974 7320 5555   a job by its UU
-00004a10: 4944 2e0a 0a54 6865 2063 616c 6c65 7220  ID...The caller 
-00004a20: 6d75 7374 2062 6520 7468 6520 6a6f 6220  must be the job 
-00004a30: 6f77 6e65 722c 2063 7265 6174 6f72 206f  owner, creator o
-00004a40: 7220 6120 7465 6e61 6e74 2061 646d 696e  r a tenant admin
-00004a50: 6973 7472 6174 6f72 2e94 8c0b 6f70 6572  istrator....oper
-00004a60: 6174 696f 6e49 6494 8c0b 6765 744a 6f62  ationId...getJob
-00004a70: 5368 6172 6594 8c0a 7061 7261 6d65 7465  Share...paramete
-00004a80: 7273 945d 9428 7d94 288c 046e 616d 6594  rs.].(}.(..name.
-00004a90: 8c07 6a6f 6255 7569 6494 8c02 696e 948c  ..jobUuid...in..
-00004aa0: 0470 6174 6894 8c08 7265 7175 6972 6564  .path...required
-00004ab0: 9488 8c06 7363 6865 6d61 947d 948c 0474  ....schema.}...t
-00004ac0: 7970 6594 8c06 7374 7269 6e67 9473 757d  ype...string.su}
-00004ad0: 9428 8c04 6e61 6d65 948c 056c 696d 6974  .(..name...limit
-00004ae0: 948c 0269 6e94 8c05 7175 6572 7994 8c06  ...in...query...
-00004af0: 7363 6865 6d61 947d 9428 8c04 7479 7065  schema.}.(..type
-00004b00: 948c 0769 6e74 6567 6572 948c 0666 6f72  ...integer...for
-00004b10: 6d61 7494 8c05 696e 7433 3294 7575 7d94  mat...int32.uu}.
-00004b20: 288c 046e 616d 6594 8c04 736b 6970 948c  (..name...skip..
-00004b30: 0269 6e94 8c05 7175 6572 7994 8c06 7363  .in...query...sc
-00004b40: 6865 6d61 947d 9428 8c04 7479 7065 948c  hema.}.(..type..
-00004b50: 0769 6e74 6567 6572 948c 0666 6f72 6d61  .integer...forma
-00004b60: 7494 8c05 696e 7433 3294 7575 7d94 288c  t...int32.uu}.(.
-00004b70: 046e 616d 6594 8c06 7072 6574 7479 948c  .name...pretty..
-00004b80: 0269 6e94 8c05 7175 6572 7994 8c06 7363  .in...query...sc
-00004b90: 6865 6d61 947d 9428 8c04 7479 7065 948c  hema.}.(..type..
-00004ba0: 0762 6f6f 6c65 616e 948c 0764 6566 6175  .boolean...defau
-00004bb0: 6c74 9489 7575 658c 0972 6573 706f 6e73  lt..uue..respons
-00004bc0: 6573 947d 9428 8c03 3230 3094 7d94 288c  es.}.(..200.}.(.
-00004bd0: 0b64 6573 6372 6970 7469 6f6e 948c 224a  .description.."J
-00004be0: 6f62 2773 2073 6861 7265 2069 6e66 6f72  ob's share infor
-00004bf0: 6d61 7469 6f6e 2072 6574 7269 6576 6564  mation retrieved
-00004c00: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
-00004c10: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00004c20: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00004c30: 2472 6566 948c 2823 2f63 6f6d 706f 6e65  $ref..(#/compone
-00004c40: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
-00004c50: 4765 744a 6f62 5368 6172 654c 6973 7494  GetJobShareList.
-00004c60: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
-00004c70: 6573 6372 6970 7469 6f6e 948c 0c49 6e70  escription...Inp
-00004c80: 7574 2065 7272 6f72 2e94 8c07 636f 6e74  ut error....cont
-00004c90: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00004ca0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00004cb0: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-00004cc0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00004cd0: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-00004ce0: 7375 8c03 3430 3194 7d94 288c 0b64 6573  su..401.}.(..des
-00004cf0: 6372 6970 7469 6f6e 948c 0f4e 6f74 2061  cription...Not a
-00004d00: 7574 686f 7269 7a65 642e 948c 0763 6f6e  uthorized....con
-00004d10: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00004d20: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00004d30: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
-00004d40: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-00004d50: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
-00004d60: 7373 758c 0334 3033 947d 9428 8c0b 6465  ssu..403.}.(..de
-00004d70: 7363 7269 7074 696f 6e94 8c0a 466f 7262  scription...Forb
-00004d80: 6964 6465 6e2e 948c 0763 6f6e 7465 6e74  idden....content
-00004d90: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00004da0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00004db0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
-00004dc0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00004dd0: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
-00004de0: 0334 3034 947d 9428 8c0b 6465 7363 7269  .404.}.(..descri
-00004df0: 7074 696f 6e94 8c0e 4a6f 6220 6e6f 7420  ption...Job not 
-00004e00: 666f 756e 642e 948c 0763 6f6e 7465 6e74  found....content
-00004e10: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00004e20: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00004e30: 947d 948c 0424 7265 6694 8c1d 232f 636f  .}...$ref...#/co
-00004e40: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00004e50: 2f52 6573 704e 616d 6594 7373 7375 8c03  /RespName.sssu..
-00004e60: 3530 3094 7d94 288c 0b64 6573 6372 6970  500.}.(..descrip
-00004e70: 7469 6f6e 948c 0d53 6572 7665 7220 6572  tion...Server er
-00004e80: 726f 722e 948c 0763 6f6e 7465 6e74 947d  ror....content.}
-00004e90: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00004ea0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00004eb0: 948c 0424 7265 6694 8c1e 232f 636f 6d70  ...$ref...#/comp
-00004ec0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
-00004ed0: 6573 7042 6173 6963 9473 7373 7575 8c08  espBasic.sssuu..
-00004ee0: 7365 6375 7269 7479 945d 947d 948c 0854  security.].}...T
-00004ef0: 6170 6973 4a57 5494 5d94 7361 758c 0470  apisJWT.].sau..p
-00004f00: 6f73 7494 7d94 288c 0474 6167 7394 5d94  ost.}.(..tags.].
-00004f10: 8c05 7368 6172 6594 618c 0b64 6573 6372  ..share.a..descr
-00004f20: 6970 7469 6f6e 948c 6b53 6861 7265 2061  iption..kShare a
-00004f30: 206a 6f62 2077 6974 6820 6120 7573 6572   job with a user
-00004f40: 206f 6620 7468 6520 7465 6e61 6e74 2e20   of the tenant. 
-00004f50: 5468 6520 6361 6c6c 6572 206d 7573 7420  The caller must 
-00004f60: 6265 2074 6865 206a 6f62 206f 776e 6572  be the job owner
-00004f70: 2c20 6372 6561 746f 7220 6f72 2061 2074  , creator or a t
-00004f80: 656e 616e 7420 6164 6d69 6e69 7374 7261  enant administra
-00004f90: 746f 722e 948c 0b6f 7065 7261 7469 6f6e  tor....operation
-00004fa0: 4964 948c 0873 6861 7265 4a6f 6294 8c0a  Id...shareJob...
-00004fb0: 7061 7261 6d65 7465 7273 945d 9428 7d94  parameters.].(}.
-00004fc0: 288c 046e 616d 6594 8c07 6a6f 6255 7569  (..name...jobUui
-00004fd0: 6494 8c02 696e 948c 0470 6174 6894 8c08  d...in...path...
-00004fe0: 7265 7175 6972 6564 9488 8c06 7363 6865  required....sche
-00004ff0: 6d61 947d 948c 0474 7970 6594 8c06 7374  ma.}...type...st
-00005000: 7269 6e67 9473 757d 9428 8c04 6e61 6d65  ring.su}.(..name
-00005010: 948c 0670 7265 7474 7994 8c02 696e 948c  ...pretty...in..
-00005020: 0571 7565 7279 948c 0673 6368 656d 6194  .query...schema.
-00005030: 7d94 288c 0474 7970 6594 8c07 626f 6f6c  }.(..type...bool
-00005040: 6561 6e94 8c07 6465 6661 756c 7494 8975  ean...default..u
-00005050: 7565 8c0b 7265 7175 6573 7442 6f64 7994  ue..requestBody.
-00005060: 7d94 288c 0763 6f6e 7465 6e74 947d 948c  }.(..content.}..
-00005070: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00005080: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-00005090: 0424 7265 6694 8c20 232f 636f 6d70 6f6e  .$ref.. #/compon
-000050a0: 656e 7473 2f73 6368 656d 6173 2f52 6571  ents/schemas/Req
-000050b0: 5368 6172 654a 6f62 9473 7373 8c08 7265  ShareJob.sss..re
-000050c0: 7175 6972 6564 9488 758c 0972 6573 706f  quired..u..respo
-000050d0: 6e73 6573 947d 9428 8c03 3230 3094 7d94  nses.}.(..200.}.
-000050e0: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-000050f0: 1a4a 6f62 2069 7320 7368 6172 6564 2073  .Job is shared s
-00005100: 7563 6573 7366 756c 6c79 2e94 8c07 636f  ucessfully....co
-00005110: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00005120: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00005130: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00005140: 2123 2f63 6f6d 706f 6e65 6e74 732f 7363  !#/components/sc
-00005150: 6865 6d61 732f 5265 7370 5368 6172 654a  hemas/RespShareJ
-00005160: 6f62 9473 7373 758c 0334 3030 947d 9428  ob.sssu..400.}.(
-00005170: 8c0b 6465 7363 7269 7074 696f 6e94 8c0c  ..description...
-00005180: 496e 7075 7420 6572 726f 722e 948c 0763  Input error....c
-00005190: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-000051a0: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-000051b0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-000051c0: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
-000051d0: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
-000051e0: 9473 7373 758c 0334 3031 947d 9428 8c0b  .sssu..401.}.(..
-000051f0: 6465 7363 7269 7074 696f 6e94 8c0f 4e6f  description...No
-00005200: 7420 6175 7468 6f72 697a 6564 2e94 8c07  t authorized....
-00005210: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00005220: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00005230: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00005240: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
-00005250: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
-00005260: 6394 7373 7375 8c03 3430 3394 7d94 288c  c.sssu..403.}.(.
-00005270: 0b64 6573 6372 6970 7469 6f6e 948c 0a46  .description...F
-00005280: 6f72 6269 6464 656e 2e94 8c07 636f 6e74  orbidden....cont
-00005290: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-000052a0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-000052b0: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-000052c0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-000052d0: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-000052e0: 7375 8c03 3530 3094 7d94 288c 0b64 6573  su..500.}.(..des
-000052f0: 6372 6970 7469 6f6e 948c 0d53 6572 7665  cription...Serve
-00005300: 7220 6572 726f 722e 948c 0763 6f6e 7465  r error....conte
+000029a0: 2062 7920 6974 7320 5555 4944 2e20 0a54   by its UUID. .T
+000029b0: 6865 206a 6f62 206d 7573 7420 6265 2069  he job must be i
+000029c0: 6e20 6120 7465 726d 696e 616c 2073 7461  n a terminal sta
+000029d0: 7465 2028 4649 4e49 5348 4544 206f 7220  te (FINISHED or 
+000029e0: 4641 494c 4544 206f 7220 4341 4e43 454c  FAILED or CANCEL
+000029f0: 4c45 4429 2e20 4279 2064 6566 6175 6c74  LED). By default
+00002a00: 2c20 616c 6c6f 7749 6652 756e 6e69 6e67  , allowIfRunning
+00002a10: 3d66 616c 7365 2e20 0a61 6c6c 6f77 4966  =false. .allowIf
+00002a20: 5275 6e6e 696e 673d 7472 7565 2061 6c6c  Running=true all
+00002a30: 6f77 7320 6a6f 6220 6f75 7470 7574 2064  ows job output d
+00002a40: 6f77 6e6c 6f61 6420 6576 656e 2069 6620  ownload even if 
+00002a50: 6a6f 6220 6973 206e 6f74 2069 6e20 7468  job is not in th
+00002a60: 6520 7465 726d 696e 616c 2073 7461 7465  e terminal state
+00002a70: 2e20 200a 0a54 6865 2063 616c 6c65 7220  .  ..The caller 
+00002a80: 6d75 7374 2062 6520 7468 6520 6a6f 6220  must be the job 
+00002a90: 6f77 6e65 722c 2063 7265 6174 6f72 206f  owner, creator o
+00002aa0: 7220 6120 7465 6e61 6e74 2061 646d 696e  r a tenant admin
+00002ab0: 6973 7472 6174 6f72 2e0a 5468 6520 5552  istrator..The UR
+00002ac0: 4c20 6d75 7374 2065 6e64 7320 7769 7468  L must ends with
+00002ad0: 2027 2f27 2065 7665 6e20 6966 2074 6865   '/' even if the
+00002ae0: 7265 2069 7320 6e6f 206f 7574 7075 7450  re is no outputP
+00002af0: 6174 6820 6973 2073 7065 6369 6669 6564  ath is specified
+00002b00: 2e20 0a6f 7574 7075 7450 6174 6820 6973  . .outputPath is
+00002b10: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
+00002b20: 206a 6f62 206f 7574 7075 7420 7061 7468   job output path
+00002b30: 2e20 948c 0b6f 7065 7261 7469 6f6e 4964  . ...operationId
+00002b40: 948c 1467 6574 4a6f 624f 7574 7075 7444  ...getJobOutputD
+00002b50: 6f77 6e6c 6f61 6494 8c0a 7061 7261 6d65  ownload...parame
+00002b60: 7465 7273 945d 9428 7d94 288c 046e 616d  ters.].(}.(..nam
+00002b70: 6594 8c07 6a6f 6255 7569 6494 8c02 696e  e...jobUuid...in
+00002b80: 948c 0470 6174 6894 8c08 7265 7175 6972  ...path...requir
+00002b90: 6564 9488 8c06 7363 6865 6d61 947d 948c  ed....schema.}..
+00002ba0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00002bb0: 757d 9428 8c04 6e61 6d65 948c 0a6f 7574  u}.(..name...out
+00002bc0: 7075 7450 6174 6894 8c02 696e 948c 0470  putPath...in...p
+00002bd0: 6174 6894 8c08 7265 7175 6972 6564 9488  ath...required..
+00002be0: 8c06 7363 6865 6d61 947d 9428 8c04 7479  ..schema.}.(..ty
+00002bf0: 7065 948c 0673 7472 696e 6794 8c07 6465  pe...string...de
+00002c00: 6661 756c 7494 8c00 9475 757d 9428 8c04  fault....uu}.(..
+00002c10: 6e61 6d65 948c 0863 6f6d 7072 6573 7394  name...compress.
+00002c20: 8c02 696e 948c 0571 7565 7279 948c 0673  ..in...query...s
+00002c30: 6368 656d 6194 7d94 288c 0474 7970 6594  chema.}.(..type.
+00002c40: 8c07 626f 6f6c 6561 6e94 8c07 6465 6661  ..boolean...defa
+00002c50: 756c 7494 8975 757d 9428 8c04 6e61 6d65  ult..uu}.(..name
+00002c60: 948c 0666 6f72 6d61 7494 8c02 696e 948c  ...format...in..
+00002c70: 0571 7565 7279 948c 0673 6368 656d 6194  .query...schema.
+00002c80: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
+00002c90: 6e67 948c 0764 6566 6175 6c74 948c 037a  ng...default...z
+00002ca0: 6970 9475 757d 9428 8c04 6e61 6d65 948c  ip.uu}.(..name..
+00002cb0: 0e61 6c6c 6f77 4966 5275 6e6e 696e 6794  .allowIfRunning.
+00002cc0: 8c02 696e 948c 0571 7565 7279 948c 0673  ..in...query...s
+00002cd0: 6368 656d 6194 7d94 288c 0474 7970 6594  chema.}.(..type.
+00002ce0: 8c07 626f 6f6c 6561 6e94 8c07 6465 6661  ..boolean...defa
+00002cf0: 756c 7494 8975 757d 9428 8c04 6e61 6d65  ult..uu}.(..name
+00002d00: 948c 0670 7265 7474 7994 8c02 696e 948c  ...pretty...in..
+00002d10: 0571 7565 7279 948c 0673 6368 656d 6194  .query...schema.
+00002d20: 7d94 288c 0474 7970 6594 8c07 626f 6f6c  }.(..type...bool
+00002d30: 6561 6e94 8c07 6465 6661 756c 7494 8975  ean...default..u
+00002d40: 7565 8c09 7265 7370 6f6e 7365 7394 7d94  ue..responses.}.
+00002d50: 288c 0332 3030 947d 9428 8c0b 6465 7363  (..200.}.(..desc
+00002d60: 7269 7074 696f 6e94 8c1e 4a6f 6227 7320  ription...Job's 
+00002d70: 6f75 7470 7574 2066 696c 6573 2064 6f77  output files dow
+00002d80: 6e6c 6f61 6465 642e 948c 0763 6f6e 7465  nloaded....conte
+00002d90: 6e74 947d 948c 1861 7070 6c69 6361 7469  nt.}...applicati
+00002da0: 6f6e 2f6f 6374 6574 2d73 7472 6561 6d94  on/octet-stream.
+00002db0: 7d94 8c06 7363 6865 6d61 947d 9428 8c04  }...schema.}.(..
+00002dc0: 7479 7065 948c 0673 7472 696e 6794 8c06  type...string...
+00002dd0: 666f 726d 6174 948c 0662 696e 6172 7994  format...binary.
+00002de0: 7573 7375 8c03 3430 3094 7d94 288c 0b64  ussu..400.}.(..d
+00002df0: 6573 6372 6970 7469 6f6e 948c 0c49 6e70  escription...Inp
+00002e00: 7574 2065 7272 6f72 2e94 8c07 636f 6e74  ut error....cont
+00002e10: 656e 7494 7d94 8c18 6170 706c 6963 6174  ent.}...applicat
+00002e20: 696f 6e2f 6f63 7465 742d 7374 7265 616d  ion/octet-stream
+00002e30: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00002e40: 2472 6566 948c 1e23 2f63 6f6d 706f 6e65  $ref...#/compone
+00002e50: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
+00002e60: 4261 7369 6394 7373 7375 8c03 3430 3194  Basic.sssu..401.
+00002e70: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00002e80: 948c 0f4e 6f74 2061 7574 686f 7269 7a65  ...Not authorize
+00002e90: 642e 948c 0763 6f6e 7465 6e74 947d 948c  d....content.}..
+00002ea0: 1861 7070 6c69 6361 7469 6f6e 2f6f 6374  .application/oct
+00002eb0: 6574 2d73 7472 6561 6d94 7d94 8c06 7363  et-stream.}...sc
+00002ec0: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
+00002ed0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00002ee0: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
+00002ef0: 7373 758c 0334 3033 947d 9428 8c0b 6465  ssu..403.}.(..de
+00002f00: 7363 7269 7074 696f 6e94 8c0a 466f 7262  scription...Forb
+00002f10: 6964 6465 6e2e 948c 0763 6f6e 7465 6e74  idden....content
+00002f20: 947d 948c 1861 7070 6c69 6361 7469 6f6e  .}...application
+00002f30: 2f6f 6374 6574 2d73 7472 6561 6d94 7d94  /octet-stream.}.
+00002f40: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00002f50: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00002f60: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
+00002f70: 6963 9473 7373 758c 0334 3034 947d 9428  ic.sssu..404.}.(
+00002f80: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
+00002f90: 4a6f 6220 6e6f 7420 666f 756e 642e 948c  Job not found...
+00002fa0: 0763 6f6e 7465 6e74 947d 948c 1861 7070  .content.}...app
+00002fb0: 6c69 6361 7469 6f6e 2f6f 6374 6574 2d73  lication/octet-s
+00002fc0: 7472 6561 6d94 7d94 8c06 7363 6865 6d61  tream.}...schema
+00002fd0: 947d 948c 0424 7265 6694 8c1d 232f 636f  .}...$ref...#/co
+00002fe0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00002ff0: 2f52 6573 704e 616d 6594 7373 7375 8c03  /RespName.sssu..
+00003000: 3530 3094 7d94 288c 0b64 6573 6372 6970  500.}.(..descrip
+00003010: 7469 6f6e 948c 0d53 6572 7665 7220 6572  tion...Server er
+00003020: 726f 722e 948c 0763 6f6e 7465 6e74 947d  ror....content.}
+00003030: 948c 1861 7070 6c69 6361 7469 6f6e 2f6f  ...application/o
+00003040: 6374 6574 2d73 7472 6561 6d94 7d94 8c06  ctet-stream.}...
+00003050: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
+00003060: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
+00003070: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
+00003080: 9473 7373 7575 8c08 7365 6375 7269 7479  .sssuu..security
+00003090: 945d 947d 948c 0854 6170 6973 4a57 5494  .].}...TapisJWT.
+000030a0: 5d94 7361 7573 8c28 2f6a 6f62 732f 7b6a  ].saus.(/jobs/{j
+000030b0: 6f62 5575 6964 7d2f 6f75 7470 7574 2f6c  obUuid}/output/l
+000030c0: 6973 742f 7b6f 7574 7075 7450 6174 687d  ist/{outputPath}
+000030d0: 947d 948c 0367 6574 947d 9428 8c04 7461  .}...get.}.(..ta
+000030e0: 6773 945d 948c 046a 6f62 7394 618c 0b64  gs.]...jobs.a..d
+000030f0: 6573 6372 6970 7469 6f6e 9458 cd01 0000  escription.X....
+00003100: 5265 7472 6965 7665 206a 6f62 2773 206f  Retrieve job's o
+00003110: 7574 7075 7420 6669 6c65 7320 6c69 7374  utput files list
+00003120: 2066 6f72 2070 7265 7669 6f75 736c 7920   for previously 
+00003130: 7375 626d 6974 7465 6420 6a6f 6220 6279  submitted job by
+00003140: 2069 7473 2055 5549 442e 200a 5468 6520   its UUID. .The 
+00003150: 6a6f 6220 6d75 7374 2062 6520 696e 2061  job must be in a
+00003160: 2074 6572 6d69 6e61 6c20 7374 6174 6520   terminal state 
+00003170: 2846 494e 4953 4845 4420 6f72 2046 4149  (FINISHED or FAI
+00003180: 4c45 4420 6f72 2043 414e 4345 4c4c 4544  LED or CANCELLED
+00003190: 292e 2042 7920 6465 6661 756c 742c 2061  ). By default, a
+000031a0: 6c6c 6f77 4966 5275 6e6e 696e 673d 6661  llowIfRunning=fa
+000031b0: 6c73 652e 200a 616c 6c6f 7749 6652 756e  lse. .allowIfRun
+000031c0: 6e69 6e67 3d74 7275 6520 616c 6c6f 7773  ning=true allows
+000031d0: 206a 6f62 206f 7574 7075 7420 6c69 7374   job output list
+000031e0: 696e 6720 6576 656e 2069 6620 6a6f 6220  ing even if job 
+000031f0: 6973 206e 6f74 2069 6e20 7468 6520 7465  is not in the te
+00003200: 726d 696e 616c 2073 7461 7465 2e20 200a  rminal state.  .
+00003210: 0a54 6865 2063 616c 6c65 7220 6d75 7374  .The caller must
+00003220: 2062 6520 7468 6520 6a6f 6220 6f77 6e65   be the job owne
+00003230: 722c 2063 7265 6174 6f72 206f 7220 6120  r, creator or a 
+00003240: 7465 6e61 6e74 2061 646d 696e 6973 7472  tenant administr
+00003250: 6174 6f72 2e0a 5468 6520 5552 4c20 6d75  ator..The URL mu
+00003260: 7374 2065 6e64 7320 7769 7468 2027 2f27  st ends with '/'
+00003270: 2065 7665 6e20 6966 2074 6865 7265 2069   even if there i
+00003280: 7320 6e6f 206f 7574 7075 7450 6174 6820  s no outputPath 
+00003290: 6973 2073 7065 6369 6669 6564 2e0a 6f75  is specified..ou
+000032a0: 7470 7574 5061 7468 2069 7320 7265 6c61  tputPath is rela
+000032b0: 7469 7665 2074 6f20 7468 6520 6a6f 6220  tive to the job 
+000032c0: 6f75 7470 7574 2070 6174 682e 2094 8c0b  output path. ...
+000032d0: 6f70 6572 6174 696f 6e49 6494 8c10 6765  operationId...ge
+000032e0: 744a 6f62 4f75 7470 7574 4c69 7374 948c  tJobOutputList..
+000032f0: 0a70 6172 616d 6574 6572 7394 5d94 287d  .parameters.].(}
+00003300: 9428 8c04 6e61 6d65 948c 076a 6f62 5575  .(..name...jobUu
+00003310: 6964 948c 0269 6e94 8c04 7061 7468 948c  id...in...path..
+00003320: 0872 6571 7569 7265 6494 888c 0673 6368  .required....sch
+00003330: 656d 6194 7d94 8c04 7479 7065 948c 0673  ema.}...type...s
+00003340: 7472 696e 6794 7375 7d94 288c 046e 616d  tring.su}.(..nam
+00003350: 6594 8c0a 6f75 7470 7574 5061 7468 948c  e...outputPath..
+00003360: 0269 6e94 8c04 7061 7468 948c 0872 6571  .in...path...req
+00003370: 7569 7265 6494 888c 0673 6368 656d 6194  uired....schema.
+00003380: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
+00003390: 6e67 948c 0764 6566 6175 6c74 946a dc03  ng...default.j..
+000033a0: 0000 7575 7d94 288c 046e 616d 6594 8c05  ..uu}.(..name...
+000033b0: 6c69 6d69 7494 8c02 696e 948c 0571 7565  limit...in...que
+000033c0: 7279 948c 0673 6368 656d 6194 7d94 288c  ry...schema.}.(.
+000033d0: 0474 7970 6594 8c07 696e 7465 6765 7294  .type...integer.
+000033e0: 8c06 666f 726d 6174 948c 0569 6e74 3332  ..format...int32
+000033f0: 9475 757d 9428 8c04 6e61 6d65 948c 0473  .uu}.(..name...s
+00003400: 6b69 7094 8c02 696e 948c 0571 7565 7279  kip...in...query
+00003410: 948c 0673 6368 656d 6194 7d94 288c 0474  ...schema.}.(..t
+00003420: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
+00003430: 666f 726d 6174 948c 0569 6e74 3332 9475  format...int32.u
+00003440: 757d 9428 8c04 6e61 6d65 948c 0e61 6c6c  u}.(..name...all
+00003450: 6f77 4966 5275 6e6e 696e 6794 8c02 696e  owIfRunning...in
+00003460: 948c 0571 7565 7279 948c 0673 6368 656d  ...query...schem
+00003470: 6194 7d94 288c 0474 7970 6594 8c07 626f  a.}.(..type...bo
+00003480: 6f6c 6561 6e94 8c07 6465 6661 756c 7494  olean...default.
+00003490: 8975 757d 9428 8c04 6e61 6d65 948c 0670  .uu}.(..name...p
+000034a0: 7265 7474 7994 8c02 696e 948c 0571 7565  retty...in...que
+000034b0: 7279 948c 0673 6368 656d 6194 7d94 288c  ry...schema.}.(.
+000034c0: 0474 7970 6594 8c07 626f 6f6c 6561 6e94  .type...boolean.
+000034d0: 8c07 6465 6661 756c 7494 8975 7565 8c09  ..default..uue..
+000034e0: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
+000034f0: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
+00003500: 696f 6e94 8c22 4a6f 6227 7320 6f75 7470  ion.."Job's outp
+00003510: 7574 2066 696c 6573 206c 6973 7420 7265  ut files list re
+00003520: 7472 6965 7665 642e 948c 0763 6f6e 7465  trieved....conte
+00003530: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00003540: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00003550: 6d61 947d 948c 0424 7265 6694 8c29 232f  ma.}...$ref..)#/
+00003560: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00003570: 6173 2f52 6573 7047 6574 4a6f 624f 7574  as/RespGetJobOut
+00003580: 7075 744c 6973 7494 7373 7375 8c03 3430  putList.sssu..40
+00003590: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
+000035a0: 6f6e 948c 0c49 6e70 7574 2065 7272 6f72  on...Input error
+000035b0: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
+000035c0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+000035d0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+000035e0: 2472 6566 948c 1e23 2f63 6f6d 706f 6e65  $ref...#/compone
+000035f0: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
+00003600: 4261 7369 6394 7373 7375 8c03 3430 3194  Basic.sssu..401.
+00003610: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00003620: 948c 0f4e 6f74 2061 7574 686f 7269 7a65  ...Not authorize
+00003630: 642e 948c 0763 6f6e 7465 6e74 947d 948c  d....content.}..
+00003640: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00003650: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00003660: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
+00003670: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+00003680: 7042 6173 6963 9473 7373 758c 0334 3033  pBasic.sssu..403
+00003690: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
+000036a0: 6e94 8c0a 466f 7262 6964 6465 6e2e 948c  n...Forbidden...
+000036b0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+000036c0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+000036d0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+000036e0: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
+000036f0: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
+00003700: 6963 9473 7373 758c 0334 3034 947d 9428  ic.sssu..404.}.(
+00003710: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
+00003720: 4a6f 6220 6e6f 7420 666f 756e 642e 948c  Job not found...
+00003730: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00003740: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00003750: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00003760: 6694 8c1d 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00003770: 2f73 6368 656d 6173 2f52 6573 704e 616d  /schemas/RespNam
+00003780: 6594 7373 7375 8c03 3530 3094 7d94 288c  e.sssu..500.}.(.
+00003790: 0b64 6573 6372 6970 7469 6f6e 948c 0d53  .description...S
+000037a0: 6572 7665 7220 6572 726f 722e 948c 0763  erver error....c
+000037b0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
+000037c0: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
+000037d0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
+000037e0: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
+000037f0: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
+00003800: 9473 7373 7575 8c08 7365 6375 7269 7479  .sssuu..security
+00003810: 945d 947d 948c 0854 6170 6973 4a57 5494  .].}...TapisJWT.
+00003820: 5d94 7361 7573 8c0c 2f6a 6f62 732f 7365  ].saus../jobs/se
+00003830: 6172 6368 947d 9428 8c03 6765 7494 7d94  arch.}.(..get.}.
+00003840: 288c 0474 6167 7394 5d94 8c04 6a6f 6273  (..tags.]...jobs
+00003850: 9461 8c0b 6465 7363 7269 7074 696f 6e94  .a..description.
+00003860: 8cf5 5265 7472 6965 7665 206c 6973 7420  ..Retrieve list 
+00003870: 6f66 206a 6f62 7320 666f 7220 7468 6520  of jobs for the 
+00003880: 7573 6572 2062 6173 6564 206f 6e20 7365  user based on se
+00003890: 6172 6368 2063 6f6e 6469 7469 6f6e 7320  arch conditions 
+000038a0: 696e 2074 6865 2071 7565 7279 2070 6172  in the query par
+000038b0: 616d 7465 7220 6f6e 2074 6865 2064 6564  amter on the ded
+000038c0: 6963 6174 6564 2073 6561 7263 6820 656e  icated search en
+000038d0: 642d 706f 696e 742e 0a0a 5468 6520 6361  d-point...The ca
+000038e0: 6c6c 6572 206d 7573 7420 6265 2074 6865  ller must be the
+000038f0: 206a 6f62 206f 776e 6572 2c20 6372 6561   job owner, crea
+00003900: 746f 7220 6f72 2061 2074 656e 616e 7420  tor or a tenant 
+00003910: 6164 6d69 6e69 7374 7261 746f 722e 200a  administrator. .
+00003920: 0a4c 6973 7420 6f66 204a 6f62 7320 7368  .List of Jobs sh
+00003930: 6172 6564 2077 6974 6820 7468 6520 7573  ared with the us
+00003940: 6572 2063 616e 2061 6c73 6f20 6265 2073  er can also be s
+00003950: 6561 7263 6865 6494 8c0b 6f70 6572 6174  earched...operat
+00003960: 696f 6e49 6494 8c10 6765 744a 6f62 5365  ionId...getJobSe
+00003970: 6172 6368 4c69 7374 948c 0a70 6172 616d  archList...param
+00003980: 6574 6572 7394 5d94 287d 9428 8c04 6e61  eters.].(}.(..na
+00003990: 6d65 948c 056c 696d 6974 948c 0269 6e94  me...limit...in.
+000039a0: 8c05 7175 6572 7994 8c06 7363 6865 6d61  ..query...schema
+000039b0: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
+000039c0: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
+000039d0: 696e 7433 3294 7575 7d94 288c 046e 616d  int32.uu}.(..nam
+000039e0: 6594 8c04 736b 6970 948c 0269 6e94 8c05  e...skip...in...
+000039f0: 7175 6572 7994 8c06 7363 6865 6d61 947d  query...schema.}
+00003a00: 9428 8c04 7479 7065 948c 0769 6e74 6567  .(..type...integ
+00003a10: 6572 948c 0666 6f72 6d61 7494 8c05 696e  er...format...in
+00003a20: 7433 3294 7575 7d94 288c 046e 616d 6594  t32.uu}.(..name.
+00003a30: 8c0a 7374 6172 7441 6674 6572 948c 0269  ..startAfter...i
+00003a40: 6e94 8c05 7175 6572 7994 8c06 7363 6865  n...query...sche
+00003a50: 6d61 947d 9428 8c04 7479 7065 948c 0769  ma.}.(..type...i
+00003a60: 6e74 6567 6572 948c 0666 6f72 6d61 7494  nteger...format.
+00003a70: 8c05 696e 7433 3294 7575 7d94 288c 046e  ..int32.uu}.(..n
+00003a80: 616d 6594 8c07 6f72 6465 7242 7994 8c02  ame...orderBy...
+00003a90: 696e 948c 0571 7565 7279 948c 0673 6368  in...query...sch
+00003aa0: 656d 6194 7d94 8c04 7479 7065 948c 0673  ema.}...type...s
+00003ab0: 7472 696e 6794 7375 7d94 288c 046e 616d  tring.su}.(..nam
+00003ac0: 6594 8c0c 636f 6d70 7574 6554 6f74 616c  e...computeTotal
+00003ad0: 948c 0269 6e94 8c05 7175 6572 7994 8c06  ...in...query...
+00003ae0: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
+00003af0: 8c07 626f 6f6c 6561 6e94 7375 7d94 288c  ..boolean.su}.(.
+00003b00: 046e 616d 6594 8c06 7365 6c65 6374 948c  .name...select..
+00003b10: 0269 6e94 8c05 7175 6572 7994 8c06 7363  .in...query...sc
+00003b20: 6865 6d61 947d 948c 0474 7970 6594 8c06  hema.}...type...
+00003b30: 7374 7269 6e67 9473 757d 9428 8c04 6e61  string.su}.(..na
+00003b40: 6d65 948c 086c 6973 7454 7970 6594 8c02  me...listType...
+00003b50: 696e 948c 0571 7565 7279 948c 0673 6368  in...query...sch
+00003b60: 656d 6194 7d94 288c 0474 7970 6594 8c06  ema.}.(..type...
+00003b70: 7374 7269 6e67 948c 0764 6566 6175 6c74  string...default
+00003b80: 948c 074d 595f 4a4f 4253 9475 757d 9428  ...MY_JOBS.uu}.(
+00003b90: 8c04 6e61 6d65 948c 0670 7265 7474 7994  ..name...pretty.
+00003ba0: 8c02 696e 948c 0571 7565 7279 948c 0673  ..in...query...s
+00003bb0: 6368 656d 6194 7d94 288c 0474 7970 6594  chema.}.(..type.
+00003bc0: 8c07 626f 6f6c 6561 6e94 8c07 6465 6661  ..boolean...defa
+00003bd0: 756c 7494 8975 7565 8c09 7265 7370 6f6e  ult..uue..respon
+00003be0: 7365 7394 7d94 288c 0332 3030 947d 9428  ses.}.(..200.}.(
+00003bf0: 8c0b 6465 7363 7269 7074 696f 6e94 8c1b  ..description...
+00003c00: 4a6f 6273 2053 6561 7263 6820 4c69 7374  Jobs Search List
+00003c10: 2072 6574 7269 6576 6564 2e94 8c07 636f   retrieved....co
+00003c20: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00003c30: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00003c40: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00003c50: 2f23 2f63 6f6d 706f 6e65 6e74 732f 7363  /#/components/sc
+00003c60: 6865 6d61 732f 5265 7370 4a6f 6253 6561  hemas/RespJobSea
+00003c70: 7263 6841 6c6c 4174 7472 6962 7574 6573  rchAllAttributes
+00003c80: 9473 7373 758c 0334 3030 947d 9428 8c0b  .sssu..400.}.(..
+00003c90: 6465 7363 7269 7074 696f 6e94 8c0c 496e  description...In
+00003ca0: 7075 7420 6572 726f 722e 948c 0763 6f6e  put error....con
+00003cb0: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00003cc0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00003cd0: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
+00003ce0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00003cf0: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
+00003d00: 7373 758c 0334 3031 947d 9428 8c0b 6465  ssu..401.}.(..de
+00003d10: 7363 7269 7074 696f 6e94 8c0f 4e6f 7420  scription...Not 
+00003d20: 6175 7468 6f72 697a 6564 2e94 8c07 636f  authorized....co
+00003d30: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00003d40: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00003d50: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00003d60: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
+00003d70: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
+00003d80: 7373 7375 8c03 3430 3394 7d94 288c 0b64  sssu..403.}.(..d
+00003d90: 6573 6372 6970 7469 6f6e 948c 0a46 6f72  escription...For
+00003da0: 6269 6464 656e 2e94 8c07 636f 6e74 656e  bidden....conten
+00003db0: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00003dc0: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00003dd0: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
+00003de0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00003df0: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
+00003e00: 8c03 3430 3494 7d94 288c 0b64 6573 6372  ..404.}.(..descr
+00003e10: 6970 7469 6f6e 948c 0f4a 6f62 7320 6e6f  iption...Jobs no
+00003e20: 7420 666f 756e 642e 948c 0763 6f6e 7465  t found....conte
+00003e30: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00003e40: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00003e50: 6d61 947d 948c 0424 7265 6694 8c1d 232f  ma.}...$ref...#/
+00003e60: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00003e70: 6173 2f52 6573 704e 616d 6594 7373 7375  as/RespName.sssu
+00003e80: 8c03 3530 3094 7d94 288c 0b64 6573 6372  ..500.}.(..descr
+00003e90: 6970 7469 6f6e 948c 0d53 6572 7665 7220  iption...Server 
+00003ea0: 6572 726f 722e 948c 0763 6f6e 7465 6e74  error....content
+00003eb0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+00003ec0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00003ed0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+00003ee0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00003ef0: 2f52 6573 7042 6173 6963 9473 7373 7575  /RespBasic.sssuu
+00003f00: 8c08 7365 6375 7269 7479 945d 947d 948c  ..security.].}..
+00003f10: 0854 6170 6973 4a57 5494 5d94 7361 758c  .TapisJWT.].sau.
+00003f20: 0470 6f73 7494 7d94 288c 0474 6167 7394  .post.}.(..tags.
+00003f30: 5d94 8c04 6a6f 6273 9461 8c0b 6465 7363  ]...jobs.a..desc
+00003f40: 7269 7074 696f 6e94 8ced 5265 7472 6965  ription...Retrie
+00003f50: 7665 206c 6973 7420 6f66 206a 6f62 7320  ve list of jobs 
+00003f60: 666f 7220 7468 6520 7573 6572 2062 6173  for the user bas
+00003f70: 6564 206f 6e20 7365 6172 6368 2063 6f6e  ed on search con
+00003f80: 6469 7469 6f6e 7320 696e 2074 6865 2072  ditions in the r
+00003f90: 6571 7565 7374 2062 6f64 7920 616e 6420  equest body and 
+00003fa0: 7061 6769 6e61 7469 6f6e 2069 6e66 6f72  pagination infor
+00003fb0: 6d61 7469 6f6e 2066 726f 6d20 7468 6520  mation from the 
+00003fc0: 7175 6572 7920 7061 7261 6d74 6572 206f  query paramter o
+00003fd0: 6e20 7468 6520 6465 6469 6361 7465 6420  n the dedicated 
+00003fe0: 7365 6172 6368 2065 6e64 2d70 6f69 6e74  search end-point
+00003ff0: 2e0a 0a54 6865 2063 616c 6c65 7220 6d75  ...The caller mu
+00004000: 7374 2062 6520 7468 6520 6a6f 6220 6f77  st be the job ow
+00004010: 6e65 722c 2063 7265 6174 6f72 206f 7220  ner, creator or 
+00004020: 6120 7465 6e61 6e74 2061 646d 696e 6973  a tenant adminis
+00004030: 7472 6174 6f72 2e94 8c0b 6f70 6572 6174  trator....operat
+00004040: 696f 6e49 6494 8c1c 6765 744a 6f62 5365  ionId...getJobSe
+00004050: 6172 6368 4c69 7374 4279 506f 7374 5371  archListByPostSq
+00004060: 6c53 7472 948c 0a70 6172 616d 6574 6572  lStr...parameter
+00004070: 7394 5d94 287d 9428 8c04 6e61 6d65 948c  s.].(}.(..name..
+00004080: 056c 696d 6974 948c 0269 6e94 8c05 7175  .limit...in...qu
+00004090: 6572 7994 8c06 7363 6865 6d61 947d 9428  ery...schema.}.(
+000040a0: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
+000040b0: 948c 0666 6f72 6d61 7494 8c05 696e 7433  ...format...int3
+000040c0: 3294 7575 7d94 288c 046e 616d 6594 8c04  2.uu}.(..name...
+000040d0: 736b 6970 948c 0269 6e94 8c05 7175 6572  skip...in...quer
+000040e0: 7994 8c06 7363 6865 6d61 947d 9428 8c04  y...schema.}.(..
+000040f0: 7479 7065 948c 0769 6e74 6567 6572 948c  type...integer..
+00004100: 0666 6f72 6d61 7494 8c05 696e 7433 3294  .format...int32.
+00004110: 7575 7d94 288c 046e 616d 6594 8c0a 7374  uu}.(..name...st
+00004120: 6172 7441 6674 6572 948c 0269 6e94 8c05  artAfter...in...
+00004130: 7175 6572 7994 8c06 7363 6865 6d61 947d  query...schema.}
+00004140: 9428 8c04 7479 7065 948c 0769 6e74 6567  .(..type...integ
+00004150: 6572 948c 0666 6f72 6d61 7494 8c05 696e  er...format...in
+00004160: 7433 3294 7575 7d94 288c 046e 616d 6594  t32.uu}.(..name.
+00004170: 8c07 6f72 6465 7242 7994 8c02 696e 948c  ..orderBy...in..
+00004180: 0571 7565 7279 948c 0673 6368 656d 6194  .query...schema.
+00004190: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+000041a0: 6794 7375 7d94 288c 046e 616d 6594 8c0c  g.su}.(..name...
+000041b0: 636f 6d70 7574 6554 6f74 616c 948c 0269  computeTotal...i
+000041c0: 6e94 8c05 7175 6572 7994 8c06 7363 6865  n...query...sche
+000041d0: 6d61 947d 948c 0474 7970 6594 8c07 626f  ma.}...type...bo
+000041e0: 6f6c 6561 6e94 7375 7d94 288c 046e 616d  olean.su}.(..nam
+000041f0: 6594 8c06 7365 6c65 6374 948c 0269 6e94  e...select...in.
+00004200: 8c05 7175 6572 7994 8c06 7363 6865 6d61  ..query...schema
+00004210: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00004220: 6e67 9473 757d 9428 8c04 6e61 6d65 948c  ng.su}.(..name..
+00004230: 086c 6973 7454 7970 6594 8c02 696e 948c  .listType...in..
+00004240: 0571 7565 7279 948c 0673 6368 656d 6194  .query...schema.
+00004250: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
+00004260: 6e67 948c 0764 6566 6175 6c74 948c 074d  ng...default...M
+00004270: 595f 4a4f 4253 9475 757d 9428 8c04 6e61  Y_JOBS.uu}.(..na
+00004280: 6d65 948c 0670 7265 7474 7994 8c02 696e  me...pretty...in
+00004290: 948c 0571 7565 7279 948c 0673 6368 656d  ...query...schem
+000042a0: 6194 7d94 288c 0474 7970 6594 8c07 626f  a.}.(..type...bo
+000042b0: 6f6c 6561 6e94 8c07 6465 6661 756c 7494  olean...default.
+000042c0: 8975 7565 8c0b 7265 7175 6573 7442 6f64  .uue..requestBod
+000042d0: 7994 7d94 8c07 636f 6e74 656e 7494 7d94  y.}...content.}.
+000042e0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+000042f0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00004300: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
+00004310: 7373 7373 8c09 7265 7370 6f6e 7365 7394  ssss..responses.
+00004320: 7d94 288c 0332 3030 947d 9428 8c0b 6465  }.(..200.}.(..de
+00004330: 7363 7269 7074 696f 6e94 8c1b 4a6f 6273  scription...Jobs
+00004340: 2053 6561 7263 6820 4c69 7374 2072 6574   Search List ret
+00004350: 7269 6576 6564 2e94 8c07 636f 6e74 656e  rieved....conten
+00004360: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00004370: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00004380: 6194 7d94 8c04 2472 6566 948c 2f23 2f63  a.}...$ref../#/c
+00004390: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+000043a0: 732f 5265 7370 4a6f 6253 6561 7263 6841  s/RespJobSearchA
+000043b0: 6c6c 4174 7472 6962 7574 6573 9473 7373  llAttributes.sss
+000043c0: 758c 0334 3030 947d 9428 8c0b 6465 7363  u..400.}.(..desc
+000043d0: 7269 7074 696f 6e94 8c0c 496e 7075 7420  ription...Input 
+000043e0: 6572 726f 722e 948c 0763 6f6e 7465 6e74  error....content
+000043f0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+00004400: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00004410: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+00004420: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00004430: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
+00004440: 0334 3031 947d 9428 8c0b 6465 7363 7269  .401.}.(..descri
+00004450: 7074 696f 6e94 8c0f 4e6f 7420 6175 7468  ption...Not auth
+00004460: 6f72 697a 6564 2e94 8c07 636f 6e74 656e  orized....conten
+00004470: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00004480: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00004490: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
+000044a0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+000044b0: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
+000044c0: 8c03 3430 3394 7d94 288c 0b64 6573 6372  ..403.}.(..descr
+000044d0: 6970 7469 6f6e 948c 0a46 6f72 6269 6464  iption...Forbidd
+000044e0: 656e 2e94 8c07 636f 6e74 656e 7494 7d94  en....content.}.
+000044f0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00004500: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00004510: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
+00004520: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+00004530: 7370 4261 7369 6394 7373 7375 8c03 3430  spBasic.sssu..40
+00004540: 3494 7d94 288c 0b64 6573 6372 6970 7469  4.}.(..descripti
+00004550: 6f6e 948c 0f4a 6f62 7320 6e6f 7420 666f  on...Jobs not fo
+00004560: 756e 642e 948c 0763 6f6e 7465 6e74 947d  und....content.}
+00004570: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
+00004580: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
+00004590: 948c 0424 7265 6694 8c1d 232f 636f 6d70  ...$ref...#/comp
+000045a0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
+000045b0: 6573 704e 616d 6594 7373 7375 8c03 3530  espName.sssu..50
+000045c0: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
+000045d0: 6f6e 948c 0d53 6572 7665 7220 6572 726f  on...Server erro
+000045e0: 722e 948c 0763 6f6e 7465 6e74 947d 948c  r....content.}..
+000045f0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00004600: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00004610: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
+00004620: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+00004630: 7042 6173 6963 9473 7373 7575 8c08 7365  pBasic.sssuu..se
+00004640: 6375 7269 7479 945d 947d 948c 0854 6170  curity.].}...Tap
+00004650: 6973 4a57 5494 5d94 7361 7575 8c1c 2f6a  isJWT.].sauu../j
+00004660: 6f62 732f 7b6a 6f62 5575 6964 7d2f 7368  obs/{jobUuid}/sh
+00004670: 6172 652f 7b75 7365 727d 947d 948c 0664  are/{user}.}...d
+00004680: 656c 6574 6594 7d94 288c 0474 6167 7394  elete.}.(..tags.
+00004690: 5d94 8c05 7368 6172 6594 618c 0b64 6573  ]...share.a..des
+000046a0: 6372 6970 7469 6f6e 948c 9144 656c 6574  cription...Delet
+000046b0: 6520 616c 6c20 7368 6172 6520 696e 666f  e all share info
+000046c0: 726d 6174 696f 6e20 6f66 2061 2070 7265  rmation of a pre
+000046d0: 7669 6f75 736c 7920 7368 6172 6564 206a  viously shared j
+000046e0: 6f62 2066 6f72 2061 2073 7065 6369 6669  ob for a specifi
+000046f0: 6320 7573 6572 0a0a 5468 6520 6361 6c6c  c user..The call
+00004700: 6572 206d 7573 7420 6265 2074 6865 206a  er must be the j
+00004710: 6f62 206f 776e 6572 2c20 6372 6561 746f  ob owner, creato
+00004720: 7220 6f72 2061 2074 656e 616e 7420 6164  r or a tenant ad
+00004730: 6d69 6e69 7374 7261 746f 722e 948c 0b6f  ministrator....o
+00004740: 7065 7261 7469 6f6e 4964 948c 0e64 656c  perationId...del
+00004750: 6574 654a 6f62 5368 6172 6594 8c0a 7061  eteJobShare...pa
+00004760: 7261 6d65 7465 7273 945d 9428 7d94 288c  rameters.].(}.(.
+00004770: 046e 616d 6594 8c07 6a6f 6255 7569 6494  .name...jobUuid.
+00004780: 8c02 696e 948c 0470 6174 6894 8c08 7265  ..in...path...re
+00004790: 7175 6972 6564 9488 8c06 7363 6865 6d61  quired....schema
+000047a0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+000047b0: 6e67 9473 757d 9428 8c04 6e61 6d65 948c  ng.su}.(..name..
+000047c0: 0475 7365 7294 8c02 696e 948c 0470 6174  .user...in...pat
+000047d0: 6894 8c08 7265 7175 6972 6564 9488 8c06  h...required....
+000047e0: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
+000047f0: 8c06 7374 7269 6e67 9473 757d 9428 8c04  ..string.su}.(..
+00004800: 6e61 6d65 948c 0670 7265 7474 7994 8c02  name...pretty...
+00004810: 696e 948c 0571 7565 7279 948c 0673 6368  in...query...sch
+00004820: 656d 6194 7d94 288c 0474 7970 6594 8c07  ema.}.(..type...
+00004830: 626f 6f6c 6561 6e94 8c07 6465 6661 756c  boolean...defaul
+00004840: 7494 8975 7565 8c09 7265 7370 6f6e 7365  t..uue..response
+00004850: 7394 7d94 288c 0332 3030 947d 9428 8c0b  s.}.(..200.}.(..
+00004860: 6465 7363 7269 7074 696f 6e94 8c34 4a6f  description..4Jo
+00004870: 6227 7320 7368 6172 6520 696e 666f 726d  b's share inform
+00004880: 6174 696f 6e20 6465 6c65 7465 6420 666f  ation deleted fo
+00004890: 7220 6120 7370 6563 6966 6963 2075 7365  r a specific use
+000048a0: 722e 948c 0763 6f6e 7465 6e74 947d 948c  r....content.}..
+000048b0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+000048c0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+000048d0: 0424 7265 6694 8c23 232f 636f 6d70 6f6e  .$ref..##/compon
+000048e0: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+000048f0: 7055 6e53 6861 7265 4a6f 6294 7373 7375  pUnShareJob.sssu
+00004900: 8c03 3430 3094 7d94 288c 0b64 6573 6372  ..400.}.(..descr
+00004910: 6970 7469 6f6e 948c 0c49 6e70 7574 2065  iption...Input e
+00004920: 7272 6f72 2e94 8c07 636f 6e74 656e 7494  rror....content.
+00004930: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00004940: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00004950: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
+00004960: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00004970: 5265 7370 4261 7369 6394 7373 7375 8c03  RespBasic.sssu..
+00004980: 3430 3194 7d94 288c 0b64 6573 6372 6970  401.}.(..descrip
+00004990: 7469 6f6e 948c 0f4e 6f74 2061 7574 686f  tion...Not autho
+000049a0: 7269 7a65 642e 948c 0763 6f6e 7465 6e74  rized....content
+000049b0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000049c0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+000049d0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+000049e0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+000049f0: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
+00004a00: 0334 3033 947d 9428 8c0b 6465 7363 7269  .403.}.(..descri
+00004a10: 7074 696f 6e94 8c0a 466f 7262 6964 6465  ption...Forbidde
+00004a20: 6e2e 948c 0763 6f6e 7465 6e74 947d 948c  n....content.}..
+00004a30: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00004a40: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00004a50: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
+00004a60: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+00004a70: 7042 6173 6963 9473 7373 758c 0334 3034  pBasic.sssu..404
+00004a80: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
+00004a90: 6e94 8c0e 4a6f 6220 6e6f 7420 666f 756e  n...Job not foun
+00004aa0: 642e 948c 0763 6f6e 7465 6e74 947d 948c  d....content.}..
+00004ab0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00004ac0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00004ad0: 0424 7265 6694 8c1d 232f 636f 6d70 6f6e  .$ref...#/compon
+00004ae0: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+00004af0: 704e 616d 6594 7373 7375 8c03 3530 3094  pName.sssu..500.
+00004b00: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00004b10: 948c 0d53 6572 7665 7220 6572 726f 722e  ...Server error.
+00004b20: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00004b30: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+00004b40: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+00004b50: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
+00004b60: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
+00004b70: 6173 6963 9473 7373 7575 8c08 7365 6375  asic.sssuu..secu
+00004b80: 7269 7479 945d 947d 948c 0854 6170 6973  rity.].}...Tapis
+00004b90: 4a57 5494 5d94 7361 7573 8c15 2f6a 6f62  JWT.].saus../job
+00004ba0: 732f 7b6a 6f62 5575 6964 7d2f 7368 6172  s/{jobUuid}/shar
+00004bb0: 6594 7d94 288c 0367 6574 947d 9428 8c04  e.}.(..get.}.(..
+00004bc0: 7461 6773 945d 948c 0573 6861 7265 9461  tags.]...share.a
+00004bd0: 8c0b 6465 7363 7269 7074 696f 6e94 8c76  ..description..v
+00004be0: 5265 7472 6965 7665 2073 6861 7265 2069  Retrieve share i
+00004bf0: 6e66 6f72 6d61 7469 6f6e 206f 6620 6120  nformation of a 
+00004c00: 6a6f 6220 6279 2069 7473 2055 5549 442e  job by its UUID.
+00004c10: 0a0a 5468 6520 6361 6c6c 6572 206d 7573  ..The caller mus
+00004c20: 7420 6265 2074 6865 206a 6f62 206f 776e  t be the job own
+00004c30: 6572 2c20 6372 6561 746f 7220 6f72 2061  er, creator or a
+00004c40: 2074 656e 616e 7420 6164 6d69 6e69 7374   tenant administ
+00004c50: 7261 746f 722e 948c 0b6f 7065 7261 7469  rator....operati
+00004c60: 6f6e 4964 948c 0b67 6574 4a6f 6253 6861  onId...getJobSha
+00004c70: 7265 948c 0a70 6172 616d 6574 6572 7394  re...parameters.
+00004c80: 5d94 287d 9428 8c04 6e61 6d65 948c 076a  ].(}.(..name...j
+00004c90: 6f62 5575 6964 948c 0269 6e94 8c04 7061  obUuid...in...pa
+00004ca0: 7468 948c 0872 6571 7569 7265 6494 888c  th...required...
+00004cb0: 0673 6368 656d 6194 7d94 8c04 7479 7065  .schema.}...type
+00004cc0: 948c 0673 7472 696e 6794 7375 7d94 288c  ...string.su}.(.
+00004cd0: 046e 616d 6594 8c05 6c69 6d69 7494 8c02  .name...limit...
+00004ce0: 696e 948c 0571 7565 7279 948c 0673 6368  in...query...sch
+00004cf0: 656d 6194 7d94 288c 0474 7970 6594 8c07  ema.}.(..type...
+00004d00: 696e 7465 6765 7294 8c06 666f 726d 6174  integer...format
+00004d10: 948c 0569 6e74 3332 9475 757d 9428 8c04  ...int32.uu}.(..
+00004d20: 6e61 6d65 948c 0473 6b69 7094 8c02 696e  name...skip...in
+00004d30: 948c 0571 7565 7279 948c 0673 6368 656d  ...query...schem
+00004d40: 6194 7d94 288c 0474 7970 6594 8c07 696e  a.}.(..type...in
+00004d50: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
+00004d60: 0569 6e74 3332 9475 757d 9428 8c04 6e61  .int32.uu}.(..na
+00004d70: 6d65 948c 0670 7265 7474 7994 8c02 696e  me...pretty...in
+00004d80: 948c 0571 7565 7279 948c 0673 6368 656d  ...query...schem
+00004d90: 6194 7d94 288c 0474 7970 6594 8c07 626f  a.}.(..type...bo
+00004da0: 6f6c 6561 6e94 8c07 6465 6661 756c 7494  olean...default.
+00004db0: 8975 7565 8c09 7265 7370 6f6e 7365 7394  .uue..responses.
+00004dc0: 7d94 288c 0332 3030 947d 9428 8c0b 6465  }.(..200.}.(..de
+00004dd0: 7363 7269 7074 696f 6e94 8c22 4a6f 6227  scription.."Job'
+00004de0: 7320 7368 6172 6520 696e 666f 726d 6174  s share informat
+00004df0: 696f 6e20 7265 7472 6965 7665 642e 948c  ion retrieved...
+00004e00: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00004e10: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00004e20: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00004e30: 6694 8c28 232f 636f 6d70 6f6e 656e 7473  f..(#/components
+00004e40: 2f73 6368 656d 6173 2f52 6573 7047 6574  /schemas/RespGet
+00004e50: 4a6f 6253 6861 7265 4c69 7374 9473 7373  JobShareList.sss
+00004e60: 758c 0334 3030 947d 9428 8c0b 6465 7363  u..400.}.(..desc
+00004e70: 7269 7074 696f 6e94 8c0c 496e 7075 7420  ription...Input 
+00004e80: 6572 726f 722e 948c 0763 6f6e 7465 6e74  error....content
+00004e90: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+00004ea0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00004eb0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+00004ec0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00004ed0: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
+00004ee0: 0334 3031 947d 9428 8c0b 6465 7363 7269  .401.}.(..descri
+00004ef0: 7074 696f 6e94 8c0f 4e6f 7420 6175 7468  ption...Not auth
+00004f00: 6f72 697a 6564 2e94 8c07 636f 6e74 656e  orized....conten
+00004f10: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00004f20: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00004f30: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
+00004f40: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00004f50: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
+00004f60: 8c03 3430 3394 7d94 288c 0b64 6573 6372  ..403.}.(..descr
+00004f70: 6970 7469 6f6e 948c 0a46 6f72 6269 6464  iption...Forbidd
+00004f80: 656e 2e94 8c07 636f 6e74 656e 7494 7d94  en....content.}.
+00004f90: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00004fa0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00004fb0: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
+00004fc0: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+00004fd0: 7370 4261 7369 6394 7373 7375 8c03 3430  spBasic.sssu..40
+00004fe0: 3494 7d94 288c 0b64 6573 6372 6970 7469  4.}.(..descripti
+00004ff0: 6f6e 948c 0e4a 6f62 206e 6f74 2066 6f75  on...Job not fou
+00005000: 6e64 2e94 8c07 636f 6e74 656e 7494 7d94  nd....content.}.
+00005010: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00005020: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00005030: 8c04 2472 6566 948c 1d23 2f63 6f6d 706f  ..$ref...#/compo
+00005040: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+00005050: 7370 4e61 6d65 9473 7373 758c 0335 3030  spName.sssu..500
+00005060: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
+00005070: 6e94 8c0d 5365 7276 6572 2065 7272 6f72  n...Server error
+00005080: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
+00005090: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+000050a0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+000050b0: 2472 6566 948c 1e23 2f63 6f6d 706f 6e65  $ref...#/compone
+000050c0: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
+000050d0: 4261 7369 6394 7373 7375 758c 0873 6563  Basic.sssuu..sec
+000050e0: 7572 6974 7994 5d94 7d94 8c08 5461 7069  urity.].}...Tapi
+000050f0: 734a 5754 945d 9473 6175 8c04 706f 7374  sJWT.].sau..post
+00005100: 947d 9428 8c04 7461 6773 945d 948c 0573  .}.(..tags.]...s
+00005110: 6861 7265 9461 8c0b 6465 7363 7269 7074  hare.a..descript
+00005120: 696f 6e94 8c6b 5368 6172 6520 6120 6a6f  ion..kShare a jo
+00005130: 6220 7769 7468 2061 2075 7365 7220 6f66  b with a user of
+00005140: 2074 6865 2074 656e 616e 742e 2054 6865   the tenant. The
+00005150: 2063 616c 6c65 7220 6d75 7374 2062 6520   caller must be 
+00005160: 7468 6520 6a6f 6220 6f77 6e65 722c 2063  the job owner, c
+00005170: 7265 6174 6f72 206f 7220 6120 7465 6e61  reator or a tena
+00005180: 6e74 2061 646d 696e 6973 7472 6174 6f72  nt administrator
+00005190: 2e94 8c0b 6f70 6572 6174 696f 6e49 6494  ....operationId.
+000051a0: 8c08 7368 6172 654a 6f62 948c 0a70 6172  ..shareJob...par
+000051b0: 616d 6574 6572 7394 5d94 287d 9428 8c04  ameters.].(}.(..
+000051c0: 6e61 6d65 948c 076a 6f62 5575 6964 948c  name...jobUuid..
+000051d0: 0269 6e94 8c04 7061 7468 948c 0872 6571  .in...path...req
+000051e0: 7569 7265 6494 888c 0673 6368 656d 6194  uired....schema.
+000051f0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00005200: 6794 7375 7d94 288c 046e 616d 6594 8c06  g.su}.(..name...
+00005210: 7072 6574 7479 948c 0269 6e94 8c05 7175  pretty...in...qu
+00005220: 6572 7994 8c06 7363 6865 6d61 947d 9428  ery...schema.}.(
+00005230: 8c04 7479 7065 948c 0762 6f6f 6c65 616e  ..type...boolean
+00005240: 948c 0764 6566 6175 6c74 9489 7575 658c  ...default..uue.
+00005250: 0b72 6571 7565 7374 426f 6479 947d 9428  .requestBody.}.(
+00005260: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00005270: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00005280: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00005290: 6566 948c 2023 2f63 6f6d 706f 6e65 6e74  ef.. #/component
+000052a0: 732f 7363 6865 6d61 732f 5265 7153 6861  s/schemas/ReqSha
+000052b0: 7265 4a6f 6294 7373 738c 0872 6571 7569  reJob.sss..requi
+000052c0: 7265 6494 8875 8c09 7265 7370 6f6e 7365  red..u..response
+000052d0: 7394 7d94 288c 0332 3030 947d 9428 8c0b  s.}.(..200.}.(..
+000052e0: 6465 7363 7269 7074 696f 6e94 8c1a 4a6f  description...Jo
+000052f0: 6220 6973 2073 6861 7265 6420 7375 6365  b is shared suce
+00005300: 7373 6675 6c6c 792e 948c 0763 6f6e 7465  ssfully....conte
 00005310: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
 00005320: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00005330: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
+00005330: 6d61 947d 948c 0424 7265 6694 8c21 232f  ma.}...$ref..!#/
 00005340: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00005350: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
-00005360: 7575 8c08 7365 6375 7269 7479 945d 947d  uu..security.].}
-00005370: 948c 0854 6170 6973 4a57 5494 5d94 7361  ...TapisJWT.].sa
-00005380: 7575 8c16 2f6a 6f62 732f 7b6a 6f62 5575  uu../jobs/{jobUu
-00005390: 6964 7d2f 7374 6174 7573 947d 948c 0367  id}/status.}...g
-000053a0: 6574 947d 9428 8c04 7461 6773 945d 948c  et.}.(..tags.]..
-000053b0: 046a 6f62 7394 618c 0b64 6573 6372 6970  .jobs.a..descrip
-000053c0: 7469 6f6e 948c 8052 6574 7269 6576 6520  tion...Retrieve 
-000053d0: 7374 6174 7573 206f 6620 6120 7072 6576  status of a prev
-000053e0: 696f 7573 6c79 2073 7562 6d69 7474 6564  iously submitted
-000053f0: 206a 6f62 2062 7920 6974 7320 5555 4944   job by its UUID
-00005400: 2e0a 0a54 6865 2063 616c 6c65 7220 6d75  ...The caller mu
-00005410: 7374 2062 6520 7468 6520 6a6f 6220 6f77  st be the job ow
-00005420: 6e65 722c 2063 7265 6174 6f72 206f 7220  ner, creator or 
-00005430: 6120 7465 6e61 6e74 2061 646d 696e 6973  a tenant adminis
-00005440: 7472 6174 6f72 2e94 8c0b 6f70 6572 6174  trator....operat
-00005450: 696f 6e49 6494 8c0c 6765 744a 6f62 5374  ionId...getJobSt
-00005460: 6174 7573 948c 0a70 6172 616d 6574 6572  atus...parameter
-00005470: 7394 5d94 287d 9428 8c04 6e61 6d65 948c  s.].(}.(..name..
-00005480: 076a 6f62 5575 6964 948c 0269 6e94 8c04  .jobUuid...in...
-00005490: 7061 7468 948c 0872 6571 7569 7265 6494  path...required.
-000054a0: 888c 0673 6368 656d 6194 7d94 8c04 7479  ...schema.}...ty
-000054b0: 7065 948c 0673 7472 696e 6794 7375 7d94  pe...string.su}.
-000054c0: 288c 046e 616d 6594 8c06 7072 6574 7479  (..name...pretty
-000054d0: 948c 0269 6e94 8c05 7175 6572 7994 8c06  ...in...query...
-000054e0: 7363 6865 6d61 947d 9428 8c04 7479 7065  schema.}.(..type
-000054f0: 948c 0762 6f6f 6c65 616e 948c 0764 6566  ...boolean...def
-00005500: 6175 6c74 9489 7575 658c 0972 6573 706f  ault..uue..respo
-00005510: 6e73 6573 947d 9428 8c03 3230 3094 7d94  nses.}.(..200.}.
-00005520: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-00005530: 154a 6f62 2073 7461 7475 7320 7265 7472  .Job status retr
-00005540: 6965 7665 642e 948c 0763 6f6e 7465 6e74  ieved....content
-00005550: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-00005560: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-00005570: 947d 948c 0424 7265 6694 8c25 232f 636f  .}...$ref..%#/co
-00005580: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00005590: 2f52 6573 7047 6574 4a6f 6253 7461 7475  /RespGetJobStatu
-000055a0: 7394 7373 7375 8c03 3430 3094 7d94 288c  s.sssu..400.}.(.
-000055b0: 0b64 6573 6372 6970 7469 6f6e 948c 0c49  .description...I
-000055c0: 6e70 7574 2065 7272 6f72 2e94 8c07 636f  nput error....co
-000055d0: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-000055e0: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-000055f0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00005600: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
-00005610: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
-00005620: 7373 7375 8c03 3430 3194 7d94 288c 0b64  sssu..401.}.(..d
-00005630: 6573 6372 6970 7469 6f6e 948c 0f4e 6f74  escription...Not
-00005640: 2061 7574 686f 7269 7a65 642e 948c 0763   authorized....c
-00005650: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00005660: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00005670: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00005680: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
-00005690: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
-000056a0: 9473 7373 758c 0334 3033 947d 9428 8c0b  .sssu..403.}.(..
-000056b0: 6465 7363 7269 7074 696f 6e94 8c0a 466f  description...Fo
-000056c0: 7262 6964 6465 6e2e 948c 0763 6f6e 7465  rbidden....conte
-000056d0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-000056e0: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-000056f0: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
-00005700: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00005710: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
-00005720: 758c 0334 3034 947d 9428 8c0b 6465 7363  u..404.}.(..desc
-00005730: 7269 7074 696f 6e94 8c0e 4a6f 6220 6e6f  ription...Job no
-00005740: 7420 666f 756e 642e 948c 0763 6f6e 7465  t found....conte
-00005750: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-00005760: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-00005770: 6d61 947d 948c 0424 7265 6694 8c1d 232f  ma.}...$ref...#/
-00005780: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00005790: 6173 2f52 6573 704e 616d 6594 7373 7375  as/RespName.sssu
-000057a0: 8c03 3530 3094 7d94 288c 0b64 6573 6372  ..500.}.(..descr
-000057b0: 6970 7469 6f6e 948c 0d53 6572 7665 7220  iption...Server 
-000057c0: 6572 726f 722e 948c 0763 6f6e 7465 6e74  error....content
-000057d0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-000057e0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-000057f0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
-00005800: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00005810: 2f52 6573 7042 6173 6963 9473 7373 7575  /RespBasic.sssuu
-00005820: 8c08 7365 6375 7269 7479 945d 947d 948c  ..security.].}..
-00005830: 0854 6170 6973 4a57 5494 5d94 7361 7573  .TapisJWT.].saus
-00005840: 8c20 2f6a 6f62 732f 7b6a 6f62 5575 6964  . /jobs/{jobUuid
-00005850: 7d2f 7265 7375 626d 6974 5f72 6571 7565  }/resubmit_reque
-00005860: 7374 947d 948c 0367 6574 947d 9428 8c04  st.}...get.}.(..
-00005870: 7461 6773 945d 948c 046a 6f62 7394 618c  tags.]...jobs.a.
-00005880: 0b64 6573 6372 6970 7469 6f6e 948c 3347  .description..3G
-00005890: 6574 2052 6573 7562 6d69 7420 7265 7175  et Resubmit requ
-000058a0: 6573 7420 666f 7220 6f66 2061 206a 6f62  est for of a job
-000058b0: 2069 6e20 4a53 4f4e 2066 6f72 6d61 742e   in JSON format.
-000058c0: 2020 948c 0b6f 7065 7261 7469 6f6e 4964    ...operationId
-000058d0: 948c 1667 6574 5265 7375 626d 6974 5265  ...getResubmitRe
-000058e0: 7175 6573 744a 736f 6e94 8c0a 7061 7261  questJson...para
-000058f0: 6d65 7465 7273 945d 9428 7d94 288c 046e  meters.].(}.(..n
-00005900: 616d 6594 8c07 6a6f 6255 7569 6494 8c02  ame...jobUuid...
-00005910: 696e 948c 0470 6174 6894 8c08 7265 7175  in...path...requ
-00005920: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
-00005930: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00005940: 9473 757d 9428 8c04 6e61 6d65 948c 0670  .su}.(..name...p
-00005950: 7265 7474 7994 8c02 696e 948c 0571 7565  retty...in...que
-00005960: 7279 948c 0673 6368 656d 6194 7d94 288c  ry...schema.}.(.
-00005970: 0474 7970 6594 8c07 626f 6f6c 6561 6e94  .type...boolean.
-00005980: 8c07 6465 6661 756c 7494 8975 7565 8c09  ..default..uue..
-00005990: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
+00005350: 6173 2f52 6573 7053 6861 7265 4a6f 6294  as/RespShareJob.
+00005360: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
+00005370: 6573 6372 6970 7469 6f6e 948c 0c49 6e70  escription...Inp
+00005380: 7574 2065 7272 6f72 2e94 8c07 636f 6e74  ut error....cont
+00005390: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+000053a0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+000053b0: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
+000053c0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+000053d0: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
+000053e0: 7375 8c03 3430 3194 7d94 288c 0b64 6573  su..401.}.(..des
+000053f0: 6372 6970 7469 6f6e 948c 0f4e 6f74 2061  cription...Not a
+00005400: 7574 686f 7269 7a65 642e 948c 0763 6f6e  uthorized....con
+00005410: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00005420: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00005430: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
+00005440: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00005450: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
+00005460: 7373 758c 0334 3033 947d 9428 8c0b 6465  ssu..403.}.(..de
+00005470: 7363 7269 7074 696f 6e94 8c0a 466f 7262  scription...Forb
+00005480: 6964 6465 6e2e 948c 0763 6f6e 7465 6e74  idden....content
+00005490: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000054a0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+000054b0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+000054c0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+000054d0: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
+000054e0: 0335 3030 947d 9428 8c0b 6465 7363 7269  .500.}.(..descri
+000054f0: 7074 696f 6e94 8c0d 5365 7276 6572 2065  ption...Server e
+00005500: 7272 6f72 2e94 8c07 636f 6e74 656e 7494  rror....content.
+00005510: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00005520: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00005530: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
+00005540: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00005550: 5265 7370 4261 7369 6394 7373 7375 758c  RespBasic.sssuu.
+00005560: 0873 6563 7572 6974 7994 5d94 7d94 8c08  .security.].}...
+00005570: 5461 7069 734a 5754 945d 9473 6175 758c  TapisJWT.].sauu.
+00005580: 162f 6a6f 6273 2f7b 6a6f 6255 7569 647d  ./jobs/{jobUuid}
+00005590: 2f73 7461 7475 7394 7d94 8c03 6765 7494  /status.}...get.
+000055a0: 7d94 288c 0474 6167 7394 5d94 8c04 6a6f  }.(..tags.]...jo
+000055b0: 6273 9461 8c0b 6465 7363 7269 7074 696f  bs.a..descriptio
+000055c0: 6e94 8c80 5265 7472 6965 7665 2073 7461  n...Retrieve sta
+000055d0: 7475 7320 6f66 2061 2070 7265 7669 6f75  tus of a previou
+000055e0: 736c 7920 7375 626d 6974 7465 6420 6a6f  sly submitted jo
+000055f0: 6220 6279 2069 7473 2055 5549 442e 0a0a  b by its UUID...
+00005600: 5468 6520 6361 6c6c 6572 206d 7573 7420  The caller must 
+00005610: 6265 2074 6865 206a 6f62 206f 776e 6572  be the job owner
+00005620: 2c20 6372 6561 746f 7220 6f72 2061 2074  , creator or a t
+00005630: 656e 616e 7420 6164 6d69 6e69 7374 7261  enant administra
+00005640: 746f 722e 948c 0b6f 7065 7261 7469 6f6e  tor....operation
+00005650: 4964 948c 0c67 6574 4a6f 6253 7461 7475  Id...getJobStatu
+00005660: 7394 8c0a 7061 7261 6d65 7465 7273 945d  s...parameters.]
+00005670: 9428 7d94 288c 046e 616d 6594 8c07 6a6f  .(}.(..name...jo
+00005680: 6255 7569 6494 8c02 696e 948c 0470 6174  bUuid...in...pat
+00005690: 6894 8c08 7265 7175 6972 6564 9488 8c06  h...required....
+000056a0: 7363 6865 6d61 947d 948c 0474 7970 6594  schema.}...type.
+000056b0: 8c06 7374 7269 6e67 9473 757d 9428 8c04  ..string.su}.(..
+000056c0: 6e61 6d65 948c 0670 7265 7474 7994 8c02  name...pretty...
+000056d0: 696e 948c 0571 7565 7279 948c 0673 6368  in...query...sch
+000056e0: 656d 6194 7d94 288c 0474 7970 6594 8c07  ema.}.(..type...
+000056f0: 626f 6f6c 6561 6e94 8c07 6465 6661 756c  boolean...defaul
+00005700: 7494 8975 7565 8c09 7265 7370 6f6e 7365  t..uue..response
+00005710: 7394 7d94 288c 0332 3030 947d 9428 8c0b  s.}.(..200.}.(..
+00005720: 6465 7363 7269 7074 696f 6e94 8c15 4a6f  description...Jo
+00005730: 6220 7374 6174 7573 2072 6574 7269 6576  b status retriev
+00005740: 6564 2e94 8c07 636f 6e74 656e 7494 7d94  ed....content.}.
+00005750: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+00005760: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+00005770: 8c04 2472 6566 948c 2523 2f63 6f6d 706f  ..$ref..%#/compo
+00005780: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+00005790: 7370 4765 744a 6f62 5374 6174 7573 9473  spGetJobStatus.s
+000057a0: 7373 758c 0334 3030 947d 9428 8c0b 6465  ssu..400.}.(..de
+000057b0: 7363 7269 7074 696f 6e94 8c0c 496e 7075  scription...Inpu
+000057c0: 7420 6572 726f 722e 948c 0763 6f6e 7465  t error....conte
+000057d0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+000057e0: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+000057f0: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
+00005800: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00005810: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
+00005820: 758c 0334 3031 947d 9428 8c0b 6465 7363  u..401.}.(..desc
+00005830: 7269 7074 696f 6e94 8c0f 4e6f 7420 6175  ription...Not au
+00005840: 7468 6f72 697a 6564 2e94 8c07 636f 6e74  thorized....cont
+00005850: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00005860: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00005870: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
+00005880: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00005890: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
+000058a0: 7375 8c03 3430 3394 7d94 288c 0b64 6573  su..403.}.(..des
+000058b0: 6372 6970 7469 6f6e 948c 0a46 6f72 6269  cription...Forbi
+000058c0: 6464 656e 2e94 8c07 636f 6e74 656e 7494  dden....content.
+000058d0: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+000058e0: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+000058f0: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
+00005900: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00005910: 5265 7370 4261 7369 6394 7373 7375 8c03  RespBasic.sssu..
+00005920: 3430 3494 7d94 288c 0b64 6573 6372 6970  404.}.(..descrip
+00005930: 7469 6f6e 948c 0e4a 6f62 206e 6f74 2066  tion...Job not f
+00005940: 6f75 6e64 2e94 8c07 636f 6e74 656e 7494  ound....content.
+00005950: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00005960: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00005970: 7d94 8c04 2472 6566 948c 1d23 2f63 6f6d  }...$ref...#/com
+00005980: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00005990: 5265 7370 4e61 6d65 9473 7373 758c 0335  RespName.sssu..5
 000059a0: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-000059b0: 696f 6e94 8c36 5265 7375 6d62 6974 2072  ion..6Resumbit r
-000059c0: 6571 7565 7374 2066 6f72 2074 6865 206a  equest for the j
-000059d0: 6f62 2069 7320 7265 7472 6965 7665 6420  ob is retrieved 
-000059e0: 7375 6365 7373 6675 6c6c 792e 948c 0763  sucessfully....c
-000059f0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00005a00: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00005a10: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00005a20: 8c24 232f 636f 6d70 6f6e 656e 7473 2f73  .$#/components/s
-00005a30: 6368 656d 6173 2f52 6573 7047 6574 5265  chemas/RespGetRe
-00005a40: 7375 626d 6974 9473 7373 758c 0334 3030  submit.sssu..400
-00005a50: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-00005a60: 6e94 8c0c 496e 7075 7420 6572 726f 722e  n...Input error.
-00005a70: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00005a80: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00005a90: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00005aa0: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
-00005ab0: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
-00005ac0: 6173 6963 9473 7373 758c 0334 3031 947d  asic.sssu..401.}
-00005ad0: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-00005ae0: 8c0f 4e6f 7420 6175 7468 6f72 697a 6564  ..Not authorized
-00005af0: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
-00005b00: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00005b10: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00005b20: 2472 6566 948c 1e23 2f63 6f6d 706f 6e65  $ref...#/compone
-00005b30: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
-00005b40: 4261 7369 6394 7373 7375 8c03 3430 3394  Basic.sssu..403.
-00005b50: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00005b60: 948c 0a46 6f72 6269 6464 656e 2e94 8c07  ...Forbidden....
-00005b70: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00005b80: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00005b90: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00005ba0: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
-00005bb0: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
-00005bc0: 6394 7373 7375 8c03 3530 3094 7d94 288c  c.sssu..500.}.(.
-00005bd0: 0b64 6573 6372 6970 7469 6f6e 948c 0d53  .description...S
-00005be0: 6572 7665 7220 6572 726f 722e 948c 0763  erver error....c
-00005bf0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00005c00: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00005c10: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00005c20: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
-00005c30: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
-00005c40: 9473 7373 7575 8c08 7365 6375 7269 7479  .sssuu..security
-00005c50: 945d 947d 948c 0854 6170 6973 4a57 5494  .].}...TapisJWT.
-00005c60: 5d94 7361 7573 8c18 2f6a 6f62 732f 7b6a  ].saus../jobs/{j
-00005c70: 6f62 5575 6964 7d2f 7265 7375 626d 6974  obUuid}/resubmit
-00005c80: 947d 948c 0470 6f73 7494 7d94 288c 0474  .}...post.}.(..t
-00005c90: 6167 7394 5d94 8c04 6a6f 6273 9461 8c0b  ags.]...jobs.a..
-00005ca0: 6465 7363 7269 7074 696f 6e94 58c6 0200  description.X...
-00005cb0: 0052 6573 7562 6d69 7420 6120 6a6f 6220  .Resubmit a job 
-00005cc0: 666f 7220 6578 6563 7574 696f 6e20 7573  for execution us
-00005cd0: 696e 6720 7468 6520 6a6f 6227 7320 6f72  ing the job's or
-00005ce0: 6967 696e 616c 2070 6172 616d 6574 6572  iginal parameter
-00005cf0: 732e 2020 5468 6520 6d61 696e 2070 6861  s.  The main pha
-00005d00: 7365 7320 6f66 206a 6f62 2065 7865 6375  ses of job execu
-00005d10: 7469 6f6e 2061 7265 3a0a 0a20 202d 2076  tion are:..  - v
-00005d20: 616c 6964 6174 6520 696e 7075 740a 2020  alidate input.  
-00005d30: 2d20 6368 6563 6b20 7265 736f 7572 6365  - check resource
-00005d40: 2061 7661 696c 6162 696c 6974 790a 2020   availability.  
-00005d50: 2d20 7374 6167 6520 696e 7075 7420 6669  - stage input fi
-00005d60: 6c65 730a 2020 2d20 7374 6167 6520 6170  les.  - stage ap
-00005d70: 706c 6963 6174 696f 6e20 636f 6465 0a20  plication code. 
-00005d80: 202d 206c 6175 6e63 6820 6170 706c 6963   - launch applic
-00005d90: 6174 696f 6e0a 2020 2d20 6d6f 6e69 746f  ation.  - monito
-00005da0: 7220 6170 706c 6963 6174 696f 6e0a 2020  r application.  
-00005db0: 2d20 6172 6368 6976 6520 6170 706c 6963  - archive applic
-00005dc0: 6174 696f 6e20 6f75 7470 7574 0a0a 5768  ation output..Wh
-00005dd0: 656e 2061 206a 6f62 2069 7320 7375 626d  en a job is subm
-00005de0: 6974 7465 6420 6974 7320 7265 7175 6573  itted its reques
-00005df0: 7420 7061 796c 6f61 6420 6973 2063 6170  t payload is cap
-00005e00: 7475 7265 6420 616e 6420 6176 6169 6c61  tured and availa
-00005e10: 626c 6520 666f 7220 7265 7375 626d 6973  ble for resubmis
-00005e20: 7369 6f6e 2075 7369 6e67 2074 6869 7320  sion using this 
-00005e30: 4150 492e 2054 6865 2072 6573 7562 6d69  API. The resubmi
-00005e40: 7474 6564 206a 6f62 2069 7320 6173 7369  tted job is assi
-00005e50: 676e 6564 2061 206e 6577 2055 5549 4420  gned a new UUID 
-00005e60: 616e 6420 646f 6573 206e 6f74 2072 6566  and does not ref
-00005e70: 6572 656e 6365 206f 7220 6861 7665 2061  erence or have a
-00005e80: 6e79 2073 7065 6369 616c 2061 6363 6573  ny special acces
-00005e90: 7320 746f 2074 6865 206f 7269 6769 6e61  s to the origina
-00005ea0: 6c20 6a6f 6227 7320 696e 666f 726d 6174  l job's informat
-00005eb0: 696f 6e20 6f6e 6365 2074 6865 206f 7267  ion once the org
-00005ec0: 696e 616c 206a 6f62 2773 2072 6571 7565  inal job's reque
-00005ed0: 7374 2069 7320 636f 7069 6564 2e20 5468  st is copied. Th
-00005ee0: 6520 7265 7375 626d 6974 7465 6420 6a6f  e resubmitted jo
-00005ef0: 6227 7320 6578 6563 7574 696f 6e20 6361  b's execution ca
-00005f00: 6e20 6469 6666 6572 2066 726f 6d20 7468  n differ from th
-00005f10: 6520 6f72 6967 696e 616c 206a 6f62 2773  e original job's
-00005f20: 2069 6620 7468 6520 6170 706c 6963 6174   if the applicat
-00005f30: 696f 6e2c 2073 7973 7465 6d20 6f72 206f  ion, system or o
-00005f40: 7468 6572 2061 7370 6563 7473 206f 6620  ther aspects of 
-00005f50: 7468 6520 6578 6563 7574 696f 6e20 656e  the execution en
-00005f60: 7669 726f 6e6d 656e 7420 6861 7665 2063  vironment have c
-00005f70: 6861 6e67 6564 2e94 8c0b 6f70 6572 6174  hanged....operat
-00005f80: 696f 6e49 6494 8c0b 7265 7375 626d 6974  ionId...resubmit
-00005f90: 4a6f 6294 8c0a 7061 7261 6d65 7465 7273  Job...parameters
-00005fa0: 945d 9428 7d94 288c 046e 616d 6594 8c07  .].(}.(..name...
-00005fb0: 6a6f 6255 7569 6494 8c02 696e 948c 0470  jobUuid...in...p
-00005fc0: 6174 6894 8c08 7265 7175 6972 6564 9488  ath...required..
-00005fd0: 8c06 7363 6865 6d61 947d 948c 0474 7970  ..schema.}...typ
-00005fe0: 6594 8c06 7374 7269 6e67 9473 757d 9428  e...string.su}.(
-00005ff0: 8c04 6e61 6d65 948c 0670 7265 7474 7994  ..name...pretty.
-00006000: 8c02 696e 948c 0571 7565 7279 948c 0673  ..in...query...s
-00006010: 6368 656d 6194 7d94 288c 0474 7970 6594  chema.}.(..type.
-00006020: 8c07 626f 6f6c 6561 6e94 8c07 6465 6661  ..boolean...defa
-00006030: 756c 7494 8975 7565 8c09 7265 7370 6f6e  ult..uue..respon
-00006040: 7365 7394 7d94 288c 0332 3030 947d 9428  ses.}.(..200.}.(
-00006050: 8c0b 6465 7363 7269 7074 696f 6e94 8c0c  ..description...
-00006060: 4a6f 6220 6372 6561 7465 642e 948c 0763  Job created....c
-00006070: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00006080: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00006090: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-000060a0: 8c22 232f 636f 6d70 6f6e 656e 7473 2f73  ."#/components/s
-000060b0: 6368 656d 6173 2f52 6573 7053 7562 6d69  chemas/RespSubmi
-000060c0: 744a 6f62 9473 7373 758c 0334 3030 947d  tJob.sssu..400.}
-000060d0: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-000060e0: 8c0c 496e 7075 7420 6572 726f 722e 948c  ..Input error...
-000060f0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00006100: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-00006110: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00006120: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
-00006130: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
-00006140: 6963 9473 7373 758c 0334 3031 947d 9428  ic.sssu..401.}.(
-00006150: 8c0b 6465 7363 7269 7074 696f 6e94 8c0f  ..description...
-00006160: 4e6f 7420 6175 7468 6f72 697a 6564 2e94  Not authorized..
-00006170: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
-00006180: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
-00006190: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-000061a0: 6566 948c 1e23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-000061b0: 732f 7363 6865 6d61 732f 5265 7370 4261  s/schemas/RespBa
-000061c0: 7369 6394 7373 7375 8c03 3430 3394 7d94  sic.sssu..403.}.
-000061d0: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
-000061e0: 0a46 6f72 6269 6464 656e 2e94 8c07 636f  .Forbidden....co
-000061f0: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
-00006200: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
-00006210: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
-00006220: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
-00006230: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
-00006240: 7373 7375 8c03 3530 3094 7d94 288c 0b64  sssu..500.}.(..d
-00006250: 6573 6372 6970 7469 6f6e 948c 0d53 6572  escription...Ser
-00006260: 7665 7220 6572 726f 722e 948c 0763 6f6e  ver error....con
-00006270: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00006280: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00006290: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
-000062a0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-000062b0: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
-000062c0: 7373 7575 8c08 7365 6375 7269 7479 945d  ssuu..security.]
-000062d0: 947d 948c 0854 6170 6973 4a57 5494 5d94  .}...TapisJWT.].
-000062e0: 7361 7573 8c19 2f6a 6f62 732f 7b6a 6f62  saus../jobs/{job
-000062f0: 5575 6964 7d2f 7365 6e64 4576 656e 7494  Uuid}/sendEvent.
-00006300: 7d94 8c04 706f 7374 947d 9428 8c04 7461  }...post.}.(..ta
-00006310: 6773 945d 948c 046a 6f62 7394 618c 0b64  gs.]...jobs.a..d
-00006320: 6573 6372 6970 7469 6f6e 9458 3102 0000  escription.X1...
-00006330: 5365 6e64 2061 2075 7365 7220 6576 656e  Send a user even
-00006340: 7420 746f 2061 6e20 6163 7469 7665 206a  t to an active j
-00006350: 6f62 2e20 5468 6520 6a6f 6220 6d75 7374  ob. The job must
-00006360: 2062 6520 696e 2074 6865 2073 616d 6520   be in the same 
-00006370: 7465 6e61 6e74 2061 7320 7468 6520 6361  tenant as the ca
-00006380: 6c6c 6572 2c20 6275 7420 6e6f 206f 7468  ller, but no oth
-00006390: 6572 2061 7574 686f 7269 7a61 7469 6f6e  er authorization
-000063a0: 2069 7320 6e65 6564 6564 2e20 4966 2074   is needed. If t
-000063b0: 6865 206a 6f62 2068 6173 2074 6572 6d69  he job has termi
-000063c0: 6e61 7465 6420 7468 6520 7265 7175 6573  nated the reques
-000063d0: 7420 7769 6c6c 2062 6520 7265 6a65 6374  t will be reject
-000063e0: 6564 2e20 5468 6520 6361 6c6c 6572 206d  ed. The caller m
-000063f0: 7573 7420 7370 6563 6966 7920 6120 7061  ust specify a pa
-00006400: 796c 6f61 6420 6f66 206e 6f6e 2d65 6d70  yload of non-emp
-00006410: 7479 2073 7472 696e 6720 6461 7461 2069  ty string data i
-00006420: 6e20 7468 6520 2a65 7665 6e74 4461 7461  n the *eventData
-00006430: 2a20 6669 656c 642e 2054 6865 202a 6576  * field. The *ev
-00006440: 656e 7444 6574 6169 6c2a 2066 6965 6c64  entDetail* field
-00006450: 2063 616e 2062 6520 7365 7420 746f 2066   can be set to f
-00006460: 7572 7468 6572 2071 7561 6c69 6679 2074  urther qualify t
-00006470: 6865 2074 7970 6520 6f66 2075 7365 7220  he type of user 
-00006480: 6576 656e 742c 2077 6869 6368 2069 7320  event, which is 
-00006490: 7573 6566 756c 2077 6865 6e20 6669 6c74  useful when filt
-000064a0: 6572 696e 6720 6576 656e 7473 2e20 4966  ering events. If
-000064b0: 206e 6f74 2070 726f 7669 6465 6420 7468   not provided th
-000064c0: 6520 2a65 7665 6e74 4465 7461 696c 2a20  e *eventDetail* 
-000064d0: 6465 6661 756c 7473 2074 6f20 2244 4546  defaults to "DEF
-000064e0: 4155 4c54 222e 0a0a 5375 6273 6372 6962  AULT"...Subscrib
-000064f0: 6572 7320 7468 6174 2072 6567 6973 7465  ers that registe
-00006500: 7220 696e 7465 7265 7374 2069 6e20 6576  r interest in ev
-00006510: 656e 7473 206f 6620 7479 7065 204a 4f42  ents of type JOB
-00006520: 5f55 5345 525f 4556 454e 5420 7769 6c6c  _USER_EVENT will
-00006530: 2072 6563 6569 7665 2061 206e 6f74 6966   receive a notif
-00006540: 6963 6174 696f 6e20 6173 2061 2072 6573  ication as a res
-00006550: 756c 7420 6f66 2074 6869 7320 6361 6c6c  ult of this call
-00006560: 2e94 8c0b 6f70 6572 6174 696f 6e49 6494  ....operationId.
-00006570: 8c09 7365 6e64 4576 656e 7494 8c0a 7061  ..sendEvent...pa
-00006580: 7261 6d65 7465 7273 945d 9428 7d94 288c  rameters.].(}.(.
-00006590: 046e 616d 6594 8c07 6a6f 6255 7569 6494  .name...jobUuid.
-000065a0: 8c02 696e 948c 0470 6174 6894 8c08 7265  ..in...path...re
-000065b0: 7175 6972 6564 9488 8c06 7363 6865 6d61  quired....schema
-000065c0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-000065d0: 6e67 9473 757d 9428 8c04 6e61 6d65 948c  ng.su}.(..name..
-000065e0: 0670 7265 7474 7994 8c02 696e 948c 0571  .pretty...in...q
-000065f0: 7565 7279 948c 0673 6368 656d 6194 7d94  uery...schema.}.
-00006600: 288c 0474 7970 6594 8c07 626f 6f6c 6561  (..type...boolea
-00006610: 6e94 8c07 6465 6661 756c 7494 8975 7565  n...default..uue
-00006620: 8c0b 7265 7175 6573 7442 6f64 7994 7d94  ..requestBody.}.
-00006630: 288c 0763 6f6e 7465 6e74 947d 948c 1061  (..content.}...a
-00006640: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00006650: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00006660: 7265 6694 8c21 232f 636f 6d70 6f6e 656e  ref..!#/componen
-00006670: 7473 2f73 6368 656d 6173 2f52 6571 5573  ts/schemas/ReqUs
-00006680: 6572 4576 656e 7494 7373 738c 0872 6571  erEvent.sss..req
-00006690: 7569 7265 6494 8875 8c09 7265 7370 6f6e  uired..u..respon
-000066a0: 7365 7394 7d94 288c 0332 3030 947d 9428  ses.}.(..200.}.(
-000066b0: 8c0b 6465 7363 7269 7074 696f 6e94 8c0e  ..description...
-000066c0: 4576 656e 7420 6372 6561 7465 642e 948c  Event created...
-000066d0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-000066e0: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-000066f0: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00006700: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
-00006710: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
-00006720: 6963 9473 7373 758c 0334 3030 947d 9428  ic.sssu..400.}.(
-00006730: 8c0b 6465 7363 7269 7074 696f 6e94 8c0c  ..description...
-00006740: 496e 7075 7420 6572 726f 722e 948c 0763  Input error....c
-00006750: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00006760: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00006770: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00006780: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
-00006790: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
-000067a0: 9473 7373 758c 0334 3031 947d 9428 8c0b  .sssu..401.}.(..
-000067b0: 6465 7363 7269 7074 696f 6e94 8c0f 4e6f  description...No
-000067c0: 7420 6175 7468 6f72 697a 6564 2e94 8c07  t authorized....
-000067d0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-000067e0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-000067f0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00006800: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
-00006810: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
-00006820: 6394 7373 7375 8c03 3430 3394 7d94 288c  c.sssu..403.}.(.
-00006830: 0b64 6573 6372 6970 7469 6f6e 948c 0a46  .description...F
-00006840: 6f72 6269 6464 656e 2e94 8c07 636f 6e74  orbidden....cont
-00006850: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00006860: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00006870: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-00006880: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00006890: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-000068a0: 7375 8c03 3530 3094 7d94 288c 0b64 6573  su..500.}.(..des
-000068b0: 6372 6970 7469 6f6e 948c 0d53 6572 7665  cription...Serve
-000068c0: 7220 6572 726f 722e 948c 0763 6f6e 7465  r error....conte
-000068d0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-000068e0: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-000068f0: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
-00006900: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-00006910: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
-00006920: 7575 8c08 7365 6375 7269 7479 945d 947d  uu..security.].}
-00006930: 948c 0854 6170 6973 4a57 5494 5d94 7361  ...TapisJWT.].sa
-00006940: 7573 8c0c 2f6a 6f62 732f 7375 626d 6974  us../jobs/submit
-00006950: 947d 948c 0470 6f73 7494 7d94 288c 0474  .}...post.}.(..t
-00006960: 6167 7394 5d94 8c04 6a6f 6273 9461 8c0b  ags.]...jobs.a..
-00006970: 6465 7363 7269 7074 696f 6e94 58ac 0300  description.X...
-00006980: 0053 7562 6d69 7420 6120 6a6f 6220 666f  .Submit a job fo
-00006990: 7220 6578 6563 7574 696f 6e2e 2020 5468  r execution.  Th
-000069a0: 6520 6d61 696e 2070 6861 7365 7320 6f66  e main phases of
-000069b0: 206a 6f62 2065 7865 6375 7469 6f6e 2061   job execution a
-000069c0: 7265 3a0a 0a20 202d 2076 616c 6964 6174  re:..  - validat
-000069d0: 6520 696e 7075 740a 2020 2d20 6368 6563  e input.  - chec
-000069e0: 6b20 7265 736f 7572 6365 2061 7661 696c  k resource avail
-000069f0: 6162 696c 6974 790a 2020 2d20 7374 6167  ability.  - stag
-00006a00: 6520 696e 7075 7420 6669 6c65 730a 2020  e input files.  
-00006a10: 2d20 7374 6167 6520 6170 706c 6963 6174  - stage applicat
-00006a20: 696f 6e20 636f 6465 0a20 202d 206c 6175  ion code.  - lau
-00006a30: 6e63 6820 6170 706c 6963 6174 696f 6e0a  nch application.
-00006a40: 2020 2d20 6d6f 6e69 746f 7220 6170 706c    - monitor appl
-00006a50: 6963 6174 696f 6e0a 2020 2d20 6172 6368  ication.  - arch
-00006a60: 6976 6520 6170 706c 6963 6174 696f 6e20  ive application 
-00006a70: 6f75 7470 7574 0a0a 4174 2061 206d 696e  output..At a min
-00006a80: 696d 756d 2c20 7468 6520 6a6f 6220 6e61  imum, the job na
-00006a90: 6d65 2c20 6170 706c 6963 6174 696f 6e20  me, application 
-00006aa0: 4944 2061 6e64 2061 7070 6c69 6361 7469  ID and applicati
-00006ab0: 6f6e 2076 6572 7369 6f6e 206d 7573 7420  on version must 
-00006ac0: 6265 2073 7065 6369 6669 6564 2069 6e20  be specified in 
-00006ad0: 7468 6520 7265 7175 6573 7420 7061 796c  the request payl
-00006ae0: 6f61 642e 2054 6865 206f 7074 696f 6e61  oad. The optiona
-00006af0: 6c20 7061 7261 6d65 7465 7273 2061 7661  l parameters ava
-00006b00: 696c 6162 6c65 2069 6e20 6120 6a6f 6220  ilable in a job 
-00006b10: 7265 7175 6573 7420 7072 6f76 6964 6520  request provide 
-00006b20: 6772 6561 7420 666c 6578 6962 696c 6974  great flexibilit
-00006b30: 7920 6275 7420 6d75 7374 2062 6520 636f  y but must be co
-00006b40: 6e73 6964 6572 6564 2069 6e20 7468 6520  nsidered in the 
-00006b50: 636f 6e74 6578 7420 6f66 2074 6865 2061  context of the a
-00006b60: 7070 6c69 6361 7469 6f6e 2061 6e64 2073  pplication and s
-00006b70: 7973 7465 6d20 6465 6669 6e69 7469 6f6e  ystem definition
-00006b80: 732e 2054 6865 2061 6374 7561 6c20 7661  s. The actual va
-00006b90: 6c75 6573 2075 7365 6420 6475 7269 6e67  lues used during
-00006ba0: 206a 6f62 2065 7865 6375 7469 6f6e 2061   job execution a
-00006bb0: 7265 2061 2063 6f6d 6269 6e61 7469 6f6e  re a combination
-00006bc0: 206f 6620 7468 6520 7661 6c75 6573 2069   of the values i
-00006bd0: 6e20 7468 6973 2072 6571 7565 7374 2061  n this request a
-00006be0: 6e64 2074 686f 7365 2073 7065 6369 6669  nd those specifi
-00006bf0: 6564 2069 6e20 7468 6520 6a6f 6227 7320  ed in the job's 
-00006c00: 6170 706c 6963 6174 696f 6e20 616e 6420  application and 
-00006c10: 7379 7374 656d 2064 6566 696e 6974 696f  system definitio
-00006c20: 6e73 2e20 4974 2773 206f 6674 656e 2064  ns. It's often d
-00006c30: 6573 6972 6162 6c65 2074 6f20 6b65 6570  esirable to keep
-00006c40: 2074 6865 2073 7562 6d69 7373 696f 6e20   the submission 
-00006c50: 7265 7175 6573 7420 7369 6d70 6c65 2062  request simple b
-00006c60: 7920 7370 6563 6966 7969 6e67 2063 6f6d  y specifying com
-00006c70: 6d6f 6e20 7661 6c75 6573 2069 6e20 7468  mon values in th
-00006c80: 6573 6520 6f74 6865 7220 7477 6f20 6465  ese other two de
-00006c90: 6669 6e69 7469 6f6e 732e 2053 6565 2074  finitions. See t
-00006ca0: 6865 205b 4a6f 6220 5375 626d 6973 7369  he [Job Submissi
-00006cb0: 6f6e 2052 6571 7565 7374 5d28 6874 7470  on Request](http
-00006cc0: 733a 2f2f 7461 7069 732e 7265 6164 7468  s://tapis.readth
-00006cd0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00006ce0: 7374 2f74 6563 686e 6963 616c 2f6a 6f62  st/technical/job
-00006cf0: 732e 6874 6d6c 2374 6865 2d6a 6f62 2d73  s.html#the-job-s
-00006d00: 7562 6d69 7373 696f 6e2d 7265 7175 6573  ubmission-reques
-00006d10: 7429 2064 6f63 756d 656e 7461 7469 6f6e  t) documentation
-00006d20: 2066 6f72 2064 6574 6169 6c73 2e94 8c0b   for details....
-00006d30: 6f70 6572 6174 696f 6e49 6494 8c09 7375  operationId...su
-00006d40: 626d 6974 4a6f 6294 8c0a 7061 7261 6d65  bmitJob...parame
-00006d50: 7465 7273 945d 947d 9428 8c04 6e61 6d65  ters.].}.(..name
-00006d60: 948c 0670 7265 7474 7994 8c02 696e 948c  ...pretty...in..
-00006d70: 0571 7565 7279 948c 0673 6368 656d 6194  .query...schema.
-00006d80: 7d94 288c 0474 7970 6594 8c07 626f 6f6c  }.(..type...bool
-00006d90: 6561 6e94 8c07 6465 6661 756c 7494 8975  ean...default..u
-00006da0: 7561 8c0b 7265 7175 6573 7442 6f64 7994  ua..requestBody.
-00006db0: 7d94 288c 0763 6f6e 7465 6e74 947d 948c  }.(..content.}..
-00006dc0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00006dd0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-00006de0: 0424 7265 6694 8c21 232f 636f 6d70 6f6e  .$ref..!#/compon
-00006df0: 656e 7473 2f73 6368 656d 6173 2f52 6571  ents/schemas/Req
-00006e00: 5375 626d 6974 4a6f 6294 7373 738c 0872  SubmitJob.sss..r
-00006e10: 6571 7569 7265 6494 8875 8c09 7265 7370  equired..u..resp
-00006e20: 6f6e 7365 7394 7d94 288c 0332 3030 947d  onses.}.(..200.}
-00006e30: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-00006e40: 8c0c 4a6f 6220 6372 6561 7465 642e 948c  ..Job created...
-00006e50: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
-00006e60: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
-00006e70: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
-00006e80: 6694 8c22 232f 636f 6d70 6f6e 656e 7473  f.."#/components
-00006e90: 2f73 6368 656d 6173 2f52 6573 7053 7562  /schemas/RespSub
-00006ea0: 6d69 744a 6f62 9473 7373 758c 0334 3030  mitJob.sssu..400
-00006eb0: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
-00006ec0: 6e94 8c0c 496e 7075 7420 6572 726f 722e  n...Input error.
-00006ed0: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00006ee0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00006ef0: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00006f00: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
-00006f10: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
-00006f20: 6173 6963 9473 7373 758c 0334 3031 947d  asic.sssu..401.}
-00006f30: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-00006f40: 8c0f 4e6f 7420 6175 7468 6f72 697a 6564  ..Not authorized
-00006f50: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
-00006f60: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00006f70: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
-00006f80: 2472 6566 948c 1e23 2f63 6f6d 706f 6e65  $ref...#/compone
-00006f90: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
-00006fa0: 4261 7369 6394 7373 7375 8c03 3430 3394  Basic.sssu..403.
-00006fb0: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
-00006fc0: 948c 0a46 6f72 6269 6464 656e 2e94 8c07  ...Forbidden....
-00006fd0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
-00006fe0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
-00006ff0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
-00007000: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
-00007010: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
-00007020: 6394 7373 7375 8c03 3530 3094 7d94 288c  c.sssu..500.}.(.
-00007030: 0b64 6573 6372 6970 7469 6f6e 948c 0d53  .description...S
-00007040: 6572 7665 7220 6572 726f 722e 948c 0763  erver error....c
-00007050: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00007060: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00007070: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-00007080: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
-00007090: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
-000070a0: 9473 7373 7575 8c08 7365 6375 7269 7479  .sssuu..security
-000070b0: 945d 947d 948c 0854 6170 6973 4a57 5494  .].}...TapisJWT.
-000070c0: 5d94 7361 7573 8c16 2f6a 6f62 732f 7375  ].saus../jobs/su
-000070d0: 6273 6372 6962 652f 7b75 7569 647d 947d  bscribe/{uuid}.}
-000070e0: 948c 0664 656c 6574 6594 7d94 288c 0474  ...delete.}.(..t
-000070f0: 6167 7394 5d94 8c0d 7375 6273 6372 6970  ags.]...subscrip
-00007100: 7469 6f6e 7394 618c 0b64 6573 6372 6970  tions.a..descrip
-00007110: 7469 6f6e 9458 fe01 0000 4465 7065 6e64  tion.X....Depend
-00007120: 696e 6720 6f6e 2074 6865 2055 5549 4420  ing on the UUID 
-00007130: 7072 6f76 6964 652c 2074 6869 7320 4150  provide, this AP
-00007140: 4920 6569 7468 6572 2064 656c 6574 6573  I either deletes
-00007150: 2061 2073 696e 676c 6520 7375 6273 6372   a single subscr
-00007160: 6970 7469 6f6e 2066 726f 6d20 6120 6a6f  iption from a jo
-00007170: 6220 6f72 2061 6c6c 2073 7562 7363 7269  b or all subscri
-00007180: 7074 696f 6e73 2066 726f 6d20 6120 6a6f  ptions from a jo
-00007190: 622e 2054 6f20 6465 6c65 7465 2073 696e  b. To delete sin
-000071a0: 676c 6520 7375 6273 6372 6970 7469 6f6e  gle subscription
-000071b0: 2c20 7072 6f76 6964 6520 7468 6520 5555  , provide the UU
-000071c0: 4944 206f 6620 7468 6174 2073 7562 7363  ID of that subsc
-000071d0: 7269 7074 696f 6e20 6173 206c 6973 7465  ription as liste
-000071e0: 6420 696e 2074 6865 2073 7562 7363 7269  d in the subscri
-000071f0: 7074 696f 6e20 7265 7472 6965 7661 6c20  ption retrieval 
-00007200: 7265 7375 6c74 2066 6f72 2074 6865 206a  result for the j
-00007210: 6f62 2e20 2054 6f20 6465 6c65 7465 2061  ob.  To delete a
-00007220: 6c6c 2061 206a 6f62 2773 2073 7562 7363  ll a job's subsc
-00007230: 7269 7074 696f 6e73 2c20 7370 6563 6966  riptions, specif
-00007240: 7920 7468 6520 6a6f 6220 5555 4944 2e0a  y the job UUID..
-00007250: 0a4c 696b 6520 616c 6c20 4a6f 6220 7375  .Like all Job su
-00007260: 6273 6372 6970 7469 6f6e 2041 5049 732c  bscription APIs,
-00007270: 206d 6f64 6966 6963 6174 696f 6e73 206f   modifications o
-00007280: 6e6c 7920 6166 6665 6374 2072 756e 6e69  nly affect runni
-00007290: 6e67 206a 6f62 7320 616e 6420 6e65 7665  ng jobs and neve
-000072a0: 7220 6368 616e 6765 2074 6865 2073 6176  r change the sav
-000072b0: 6564 206a 6f62 2064 6566 696e 6974 696f  ed job definitio
-000072c0: 6e2e 2041 7320 6120 636f 6e73 6571 7565  n. As a conseque
-000072d0: 6e63 652c 206a 6f62 2072 6573 7562 6d69  nce, job resubmi
-000072e0: 7373 696f 6e73 2061 7265 206e 6f74 2061  ssions are not a
-000072f0: 6666 6563 7465 6420 6279 2072 756e 7469  ffected by runti
-00007300: 6d65 2073 7562 7363 7269 7074 696f 6e20  me subscription 
-00007310: 6368 616e 6765 732e 948c 0b6f 7065 7261  changes....opera
-00007320: 7469 6f6e 4964 948c 1364 656c 6574 6553  tionId...deleteS
-00007330: 7562 7363 7269 7074 696f 6e73 948c 0a70  ubscriptions...p
-00007340: 6172 616d 6574 6572 7394 5d94 287d 9428  arameters.].(}.(
-00007350: 8c04 6e61 6d65 948c 0475 7569 6494 8c02  ..name...uuid...
-00007360: 696e 948c 0470 6174 6894 8c08 7265 7175  in...path...requ
-00007370: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
-00007380: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00007390: 9473 757d 9428 8c04 6e61 6d65 948c 0670  .su}.(..name...p
-000073a0: 7265 7474 7994 8c02 696e 948c 0571 7565  retty...in...que
-000073b0: 7279 948c 0673 6368 656d 6194 7d94 288c  ry...schema.}.(.
-000073c0: 0474 7970 6594 8c07 626f 6f6c 6561 6e94  .type...boolean.
-000073d0: 8c07 6465 6661 756c 7494 8975 7565 8c09  ..default..uue..
-000073e0: 7265 7370 6f6e 7365 7394 7d94 288c 0332  responses.}.(..2
-000073f0: 3030 947d 9428 8c0b 6465 7363 7269 7074  00.}.(..descript
-00007400: 696f 6e94 8c0c 4a6f 6220 6372 6561 7465  ion...Job create
-00007410: 642e 948c 0763 6f6e 7465 6e74 947d 948c  d....content.}..
-00007420: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
-00007430: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
-00007440: 0424 7265 6694 8c26 232f 636f 6d70 6f6e  .$ref..&#/compon
-00007450: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
-00007460: 756c 7443 6861 6e67 6543 6f75 6e74 9473  ultChangeCount.s
-00007470: 7373 758c 0334 3030 947d 9428 8c0b 6465  ssu..400.}.(..de
-00007480: 7363 7269 7074 696f 6e94 8c0c 496e 7075  scription...Inpu
-00007490: 7420 6572 726f 722e 948c 0763 6f6e 7465  t error....conte
-000074a0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
-000074b0: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
-000074c0: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
-000074d0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-000074e0: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
-000074f0: 758c 0334 3031 947d 9428 8c0b 6465 7363  u..401.}.(..desc
-00007500: 7269 7074 696f 6e94 8c0f 4e6f 7420 6175  ription...Not au
-00007510: 7468 6f72 697a 6564 2e94 8c07 636f 6e74  thorized....cont
-00007520: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-00007530: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-00007540: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-00007550: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00007560: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-00007570: 7375 8c03 3430 3394 7d94 288c 0b64 6573  su..403.}.(..des
-00007580: 6372 6970 7469 6f6e 948c 0a46 6f72 6269  cription...Forbi
-00007590: 6464 656e 2e94 8c07 636f 6e74 656e 7494  dden....content.
-000075a0: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-000075b0: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-000075c0: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
-000075d0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-000075e0: 5265 7370 4261 7369 6394 7373 7375 8c03  RespBasic.sssu..
-000075f0: 3530 3094 7d94 288c 0b64 6573 6372 6970  500.}.(..descrip
-00007600: 7469 6f6e 948c 0d53 6572 7665 7220 6572  tion...Server er
-00007610: 726f 722e 948c 0763 6f6e 7465 6e74 947d  ror....content.}
-00007620: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00007630: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00007640: 948c 0424 7265 6694 8c1e 232f 636f 6d70  ...$ref...#/comp
-00007650: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
-00007660: 6573 7042 6173 6963 9473 7373 7575 8c08  espBasic.sssuu..
-00007670: 7365 6375 7269 7479 945d 947d 948c 0854  security.].}...T
-00007680: 6170 6973 4a57 5494 5d94 7361 7573 8c19  apisJWT.].saus..
-00007690: 2f6a 6f62 732f 7375 6273 6372 6962 652f  /jobs/subscribe/
-000076a0: 7b6a 6f62 5575 6964 7d94 7d94 288c 0367  {jobUuid}.}.(..g
-000076b0: 6574 947d 9428 8c04 7461 6773 945d 948c  et.}.(..tags.]..
-000076c0: 0d73 7562 7363 7269 7074 696f 6e73 9461  .subscriptions.a
-000076d0: 8c0b 6465 7363 7269 7074 696f 6e94 5808  ..description.X.
-000076e0: 0100 0052 6574 7269 6576 6520 6120 6a6f  ...Retrieve a jo
-000076f0: 6227 7320 7375 6273 6372 6970 7469 6f6e  b's subscription
-00007700: 7320 666f 6d20 7468 6520 4e6f 7469 6669  s fom the Notifi
-00007710: 6361 7469 6f6e 7320 7365 7276 6963 652e  cations service.
-00007720: 2041 6674 6572 2073 7562 7363 7269 7074   After subscript
-00007730: 696f 6e73 2065 7870 6972 6520 6f72 2061  ions expire or a
-00007740: 7265 2064 656c 6574 6564 2062 7920 7573  re deleted by us
-00007750: 6572 2061 6374 696f 6e20 7468 6579 206d  er action they m
-00007760: 6179 206e 6f20 6c6f 6e67 6572 2062 6520  ay no longer be 
-00007770: 6c69 7374 6564 2069 6e20 4e6f 7469 6669  listed in Notifi
-00007780: 6361 7469 6f6e 2073 6572 7669 6365 2e20  cation service. 
-00007790: 546f 2069 6e73 7065 6374 2074 6865 2069  To inspect the i
-000077a0: 6e69 7469 616c 2073 6574 206f 6620 7375  nitial set of su
-000077b0: 6273 6372 6970 7469 6f6e 7320 6173 7369  bscriptions assi
-000077c0: 676e 6564 2074 6f20 6120 6a6f 622c 2072  gned to a job, r
-000077d0: 6574 7269 6576 6520 7468 6520 6a6f 6220  etrieve the job 
-000077e0: 6465 6669 6e69 7469 6f6e 2e94 8c0b 6f70  definition....op
-000077f0: 6572 6174 696f 6e49 6494 8c10 6765 7453  erationId...getS
-00007800: 7562 7363 7269 7074 696f 6e73 948c 0a70  ubscriptions...p
-00007810: 6172 616d 6574 6572 7394 5d94 287d 9428  arameters.].(}.(
-00007820: 8c04 6e61 6d65 948c 076a 6f62 5575 6964  ..name...jobUuid
-00007830: 948c 0269 6e94 8c04 7061 7468 948c 0872  ...in...path...r
-00007840: 6571 7569 7265 6494 888c 0673 6368 656d  equired....schem
-00007850: 6194 7d94 8c04 7479 7065 948c 0673 7472  a.}...type...str
-00007860: 696e 6794 7375 7d94 288c 046e 616d 6594  ing.su}.(..name.
-00007870: 8c05 6c69 6d69 7494 8c02 696e 948c 0571  ..limit...in...q
-00007880: 7565 7279 948c 0673 6368 656d 6194 7d94  uery...schema.}.
-00007890: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
-000078a0: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
-000078b0: 3332 948c 0764 6566 6175 6c74 944b 6475  32...default.Kdu
-000078c0: 757d 9428 8c04 6e61 6d65 948c 0473 6b69  u}.(..name...ski
-000078d0: 7094 8c02 696e 948c 0571 7565 7279 948c  p...in...query..
-000078e0: 0673 6368 656d 6194 7d94 288c 0474 7970  .schema.}.(..typ
-000078f0: 6594 8c07 696e 7465 6765 7294 8c06 666f  e...integer...fo
-00007900: 726d 6174 948c 0569 6e74 3332 948c 0764  rmat...int32...d
-00007910: 6566 6175 6c74 944b 0075 757d 9428 8c04  efault.K.uu}.(..
-00007920: 6e61 6d65 948c 0670 7265 7474 7994 8c02  name...pretty...
-00007930: 696e 948c 0571 7565 7279 948c 0673 6368  in...query...sch
-00007940: 656d 6194 7d94 288c 0474 7970 6594 8c07  ema.}.(..type...
-00007950: 626f 6f6c 6561 6e94 8c07 6465 6661 756c  boolean...defaul
-00007960: 7494 8975 7565 8c09 7265 7370 6f6e 7365  t..uue..response
-00007970: 7394 7d94 288c 0332 3030 947d 9428 8c0b  s.}.(..200.}.(..
-00007980: 6465 7363 7269 7074 696f 6e94 8c0c 4a6f  description...Jo
-00007990: 6220 6372 6561 7465 642e 948c 0763 6f6e  b created....con
-000079a0: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-000079b0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-000079c0: 6865 6d61 947d 948c 0424 7265 6694 8c29  hema.}...$ref..)
-000079d0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-000079e0: 656d 6173 2f52 6573 7047 6574 5375 6273  emas/RespGetSubs
-000079f0: 6372 6970 7469 6f6e 7394 7373 7375 8c03  criptions.sssu..
-00007a00: 3430 3094 7d94 288c 0b64 6573 6372 6970  400.}.(..descrip
-00007a10: 7469 6f6e 948c 0c49 6e70 7574 2065 7272  tion...Input err
-00007a20: 6f72 2e94 8c07 636f 6e74 656e 7494 7d94  or....content.}.
-00007a30: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
-00007a40: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
-00007a50: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
-00007a60: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
-00007a70: 7370 4261 7369 6394 7373 7375 8c03 3430  spBasic.sssu..40
-00007a80: 3194 7d94 288c 0b64 6573 6372 6970 7469  1.}.(..descripti
-00007a90: 6f6e 948c 0f4e 6f74 2061 7574 686f 7269  on...Not authori
-00007aa0: 7a65 642e 948c 0763 6f6e 7465 6e74 947d  zed....content.}
-00007ab0: 948c 1061 7070 6c69 6361 7469 6f6e 2f6a  ...application/j
-00007ac0: 736f 6e94 7d94 8c06 7363 6865 6d61 947d  son.}...schema.}
-00007ad0: 948c 0424 7265 6694 8c1e 232f 636f 6d70  ...$ref...#/comp
-00007ae0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
-00007af0: 6573 7042 6173 6963 9473 7373 758c 0334  espBasic.sssu..4
-00007b00: 3033 947d 9428 8c0b 6465 7363 7269 7074  03.}.(..descript
-00007b10: 696f 6e94 8c0a 466f 7262 6964 6465 6e2e  ion...Forbidden.
-00007b20: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
-00007b30: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
-00007b40: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
-00007b50: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
-00007b60: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
-00007b70: 6173 6963 9473 7373 758c 0335 3030 947d  asic.sssu..500.}
-00007b80: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
-00007b90: 8c0d 5365 7276 6572 2065 7272 6f72 2e94  ..Server error..
-00007ba0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
-00007bb0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
-00007bc0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
-00007bd0: 6566 948c 1e23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-00007be0: 732f 7363 6865 6d61 732f 5265 7370 4261  s/schemas/RespBa
-00007bf0: 7369 6394 7373 7375 758c 0873 6563 7572  sic.sssuu..secur
-00007c00: 6974 7994 5d94 7d94 8c08 5461 7069 734a  ity.].}...TapisJ
-00007c10: 5754 945d 9473 6175 8c04 706f 7374 947d  WT.].sau..post.}
-00007c20: 9428 8c04 7461 6773 945d 948c 0d73 7562  .(..tags.]...sub
-00007c30: 7363 7269 7074 696f 6e73 9461 8c0b 6465  scriptions.a..de
-00007c40: 7363 7269 7074 696f 6e94 584e 0300 0053  scription.XN...S
-00007c50: 7562 6372 6962 6520 746f 2061 2072 756e  ubcribe to a run
-00007c60: 6e69 6e67 206a 6f62 2069 6465 6e74 6966  ning job identif
-00007c70: 6965 6420 6279 2069 7427 7320 5555 4944  ied by it's UUID
-00007c80: 2e20 5468 6520 6361 6c6c 6572 206d 7573  . The caller mus
-00007c90: 7420 6265 2074 6865 206a 6f62 206f 776e  t be the job own
-00007ca0: 6572 206f 7220 6120 7465 6e61 6e74 2061  er or a tenant a
-00007cb0: 646d 696e 6973 7472 6174 6f72 2e0a 0a4c  dministrator...L
-00007cc0: 696b 6520 616c 6c20 4a6f 6220 7375 6273  ike all Job subs
-00007cd0: 6372 6970 7469 6f6e 2041 5049 732c 206d  cription APIs, m
-00007ce0: 6f64 6966 6963 6174 696f 6e73 206f 6e6c  odifications onl
-00007cf0: 7920 6166 6665 6374 2072 756e 6e69 6e67  y affect running
-00007d00: 206a 6f62 7320 616e 6420 6e65 7665 7220   jobs and never 
-00007d10: 6368 616e 6765 2074 6865 2073 6176 6564  change the saved
-00007d20: 206a 6f62 2064 6566 696e 6974 696f 6e2e   job definition.
-00007d30: 2041 7320 6120 636f 6e73 6571 7565 6e63   As a consequenc
-00007d40: 652c 206a 6f62 2072 6573 7562 6d69 7373  e, job resubmiss
-00007d50: 696f 6e73 2061 7265 206e 6f74 2061 6666  ions are not aff
-00007d60: 6563 7465 6420 6279 2072 756e 7469 6d65  ected by runtime
-00007d70: 2073 7562 7363 7269 7074 696f 6e20 6368   subscription ch
-00007d80: 616e 6765 732e 0a0a 5468 6520 6576 656e  anges...The even
-00007d90: 7473 2074 6f20 7768 6963 6820 6f6e 6520  ts to which one 
-00007da0: 6361 6e20 7375 6273 6372 6962 6520 6172  can subscribe ar
-00007db0: 653a 0a0a 2d20 4a4f 425f 4e45 575f 5354  e:..- JOB_NEW_ST
-00007dc0: 4154 5553 202d 2074 6865 206a 6f62 2068  ATUS - the job h
-00007dd0: 6173 2074 7261 6e73 6974 696f 6e65 6420  as transitioned 
-00007de0: 746f 2061 206e 6577 2073 7461 7475 730a  to a new status.
-00007df0: 2d20 4a4f 425f 494e 5055 545f 5452 414e  - JOB_INPUT_TRAN
-00007e00: 5341 4354 494f 4e5f 4944 202d 2061 2072  SACTION_ID - a r
-00007e10: 6571 7565 7374 2074 6f20 7374 6167 6520  equest to stage 
-00007e20: 6a6f 6220 696e 7075 7420 6669 6c65 7320  job input files 
-00007e30: 6861 7320 6265 656e 2073 7562 6d69 7474  has been submitt
-00007e40: 6564 0a2d 204a 4f42 5f41 5243 4849 5645  ed.- JOB_ARCHIVE
-00007e50: 5f54 5241 4e53 4143 5449 4f4e 5f49 4420  _TRANSACTION_ID 
-00007e60: 2d20 6120 7265 7175 6573 7420 746f 2061  - a request to a
-00007e70: 7263 6869 7665 206a 6f62 206f 7574 7075  rchive job outpu
-00007e80: 7420 6669 6c65 7320 6861 7320 6265 656e  t files has been
-00007e90: 2073 7562 6d69 7474 6564 0a2d 204a 4f42   submitted.- JOB
-00007ea0: 5f53 5542 5343 5249 5054 494f 4e20 2d20  _SUBSCRIPTION - 
-00007eb0: 6120 6368 616e 6765 2074 6f20 7468 6520  a change to the 
-00007ec0: 6a6f 6227 7320 7375 6273 6372 6970 7469  job's subscripti
-00007ed0: 6f6e 7320 6861 7320 6f63 6375 7272 6564  ons has occurred
-00007ee0: 0a2d 204a 4f42 5f53 4841 5245 5f45 5645  .- JOB_SHARE_EVE
-00007ef0: 4e54 202d 2061 206a 6f62 2072 6573 6f75  NT - a job resou
-00007f00: 7263 6520 6861 7320 6265 656e 2073 6861  rce has been sha
-00007f10: 7265 6420 6f72 2075 6e73 6861 7265 640a  red or unshared.
-00007f20: 2d20 4a4f 425f 4552 524f 525f 4d45 5353  - JOB_ERROR_MESS
-00007f30: 4147 4520 2d20 7468 6520 6a6f 6220 6578  AGE - the job ex
-00007f40: 7065 7269 656e 6365 6420 616e 2065 7272  perienced an err
-00007f50: 6f72 0a2d 204a 4f42 5f55 5345 525f 4556  or.- JOB_USER_EV
-00007f60: 454e 5420 2d20 7573 6572 2067 656e 6572  ENT - user gener
-00007f70: 6174 6564 2065 7665 6e74 730a 2d20 414c  ated events.- AL
-00007f80: 4c20 2d20 616c 6c20 6a6f 6220 6576 656e  L - all job even
-00007f90: 7420 6361 7465 676f 7269 6573 0a94 8c0b  t categories....
-00007fa0: 6f70 6572 6174 696f 6e49 6494 8c09 7375  operationId...su
-00007fb0: 6273 6372 6962 6594 8c0a 7061 7261 6d65  bscribe...parame
-00007fc0: 7465 7273 945d 9428 7d94 288c 046e 616d  ters.].(}.(..nam
-00007fd0: 6594 8c07 6a6f 6255 7569 6494 8c02 696e  e...jobUuid...in
-00007fe0: 948c 0470 6174 6894 8c08 7265 7175 6972  ...path...requir
-00007ff0: 6564 9488 8c06 7363 6865 6d61 947d 948c  ed....schema.}..
-00008000: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00008010: 757d 9428 8c04 6e61 6d65 948c 0670 7265  u}.(..name...pre
-00008020: 7474 7994 8c02 696e 948c 0571 7565 7279  tty...in...query
-00008030: 948c 0673 6368 656d 6194 7d94 288c 0474  ...schema.}.(..t
-00008040: 7970 6594 8c07 626f 6f6c 6561 6e94 8c07  ype...boolean...
-00008050: 6465 6661 756c 7494 8975 7565 8c0b 7265  default..uue..re
-00008060: 7175 6573 7442 6f64 7994 7d94 288c 0763  questBody.}.(..c
-00008070: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
-00008080: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
-00008090: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
-000080a0: 8c21 232f 636f 6d70 6f6e 656e 7473 2f73  .!#/components/s
-000080b0: 6368 656d 6173 2f52 6571 5375 6273 6372  chemas/ReqSubscr
-000080c0: 6962 6594 7373 738c 0872 6571 7569 7265  ibe.sss..require
-000080d0: 6494 8875 8c09 7265 7370 6f6e 7365 7394  d..u..responses.
-000080e0: 7d94 288c 0332 3030 947d 9428 8c0b 6465  }.(..200.}.(..de
-000080f0: 7363 7269 7074 696f 6e94 8c19 4a6f 6220  scription...Job 
-00008100: 7375 6273 6372 6970 7469 6f6e 2063 7265  subscription cre
-00008110: 6174 6564 2e94 8c07 636f 6e74 656e 7494  ated....content.
-00008120: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00008130: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00008140: 7d94 8c04 2472 6566 948c 2423 2f63 6f6d  }...$ref..$#/com
-00008150: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00008160: 5265 7370 5265 736f 7572 6365 5572 6c94  RespResourceUrl.
-00008170: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
-00008180: 6573 6372 6970 7469 6f6e 948c 0c49 6e70  escription...Inp
-00008190: 7574 2065 7272 6f72 2e94 8c07 636f 6e74  ut error....cont
-000081a0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
-000081b0: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
-000081c0: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
-000081d0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-000081e0: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
-000081f0: 7375 8c03 3430 3194 7d94 288c 0b64 6573  su..401.}.(..des
-00008200: 6372 6970 7469 6f6e 948c 0f4e 6f74 2061  cription...Not a
-00008210: 7574 686f 7269 7a65 642e 948c 0763 6f6e  uthorized....con
-00008220: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
-00008230: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
-00008240: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
-00008250: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-00008260: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
-00008270: 7373 758c 0334 3033 947d 9428 8c0b 6465  ssu..403.}.(..de
-00008280: 7363 7269 7074 696f 6e94 8c0a 466f 7262  scription...Forb
-00008290: 6964 6465 6e2e 948c 0763 6f6e 7465 6e74  idden....content
-000082a0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
-000082b0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
-000082c0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
-000082d0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-000082e0: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
-000082f0: 0335 3030 947d 9428 8c0b 6465 7363 7269  .500.}.(..descri
-00008300: 7074 696f 6e94 8c0d 5365 7276 6572 2065  ption...Server e
-00008310: 7272 6f72 2e94 8c07 636f 6e74 656e 7494  rror....content.
-00008320: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
-00008330: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
-00008340: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
-00008350: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-00008360: 5265 7370 4261 7369 6394 7373 7375 758c  RespBasic.sssuu.
-00008370: 0873 6563 7572 6974 7994 5d94 7d94 8c08  .security.].}...
-00008380: 5461 7069 734a 5754 945d 9473 6175 7575  TapisJWT.].sauuu
-00008390: 8c0a 636f 6d70 6f6e 656e 7473 947d 9428  ..components.}.(
-000083a0: 8c07 7363 6865 6d61 7394 7d94 288c 094a  ..schemas.}.(..J
-000083b0: 6f62 7350 726f 6265 947d 9428 8c04 7479  obsProbe.}.(..ty
-000083c0: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
-000083d0: 6f70 6572 7469 6573 947d 9428 8c08 6368  operties.}.(..ch
-000083e0: 6563 6b4e 756d 947d 9428 8c04 7479 7065  eckNum.}.(..type
-000083f0: 948c 0769 6e74 6567 6572 948c 0666 6f72  ...integer...for
-00008400: 6d61 7494 8c05 696e 7436 3494 758c 0e64  mat...int64.u..d
-00008410: 6174 6162 6173 6541 6363 6573 7394 7d94  atabaseAccess.}.
-00008420: 8c04 7479 7065 948c 0762 6f6f 6c65 616e  ..type...boolean
-00008430: 9473 8c0d 7465 6e61 6e74 7341 6363 6573  .s..tenantsAcces
-00008440: 7394 7d94 8c04 7479 7065 948c 0762 6f6f  s.}...type...boo
-00008450: 6c65 616e 9473 8c0b 7175 6575 6541 6363  lean.s..queueAcc
-00008460: 6573 7394 7d94 8c04 7479 7065 948c 0762  ess.}...type...b
-00008470: 6f6f 6c65 616e 9473 7575 8c09 5265 7370  oolean.suu..Resp
-00008480: 5072 6f62 6594 7d94 288c 0474 7970 6594  Probe.}.(..type.
-00008490: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
-000084a0: 7274 6965 7394 7d94 288c 0673 7461 7475  rties.}.(..statu
-000084b0: 7394 7d94 8c04 7479 7065 948c 0673 7472  s.}...type...str
-000084c0: 696e 6794 738c 076d 6573 7361 6765 947d  ing.s..message.}
-000084d0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-000084e0: 9473 8c07 7665 7273 696f 6e94 7d94 8c04  .s..version.}...
-000084f0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00008500: 0663 6f6d 6d69 7494 7d94 8c04 7479 7065  .commit.}...type
-00008510: 948c 0673 7472 696e 6794 738c 0562 7569  ...string.s..bui
-00008520: 6c64 947d 948c 0474 7970 6594 8c06 7374  ld.}...type...st
-00008530: 7269 6e67 9473 8c08 6d65 7461 6461 7461  ring.s..metadata
-00008540: 947d 948c 0424 7265 6694 8c23 232f 636f  .}...$ref..##/co
-00008550: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00008560: 2f52 6573 756c 744d 6574 6164 6174 6194  /ResultMetadata.
-00008570: 738c 0672 6573 756c 7494 7d94 8c04 2472  s..result.}...$r
-00008580: 6566 948c 1e23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-00008590: 732f 7363 6865 6d61 732f 4a6f 6273 5072  s/schemas/JobsPr
-000085a0: 6f62 6594 7375 758c 0e52 6573 756c 744d  obe.suu..ResultM
-000085b0: 6574 6164 6174 6194 7d94 8c04 7479 7065  etadata.}...type
-000085c0: 948c 066f 626a 6563 7494 738c 0952 6573  ...object.s..Res
-000085d0: 7042 6173 6963 947d 9428 8c04 7479 7065  pBasic.}.(..type
-000085e0: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
-000085f0: 6572 7469 6573 947d 9428 8c06 7374 6174  erties.}.(..stat
-00008600: 7573 947d 948c 0474 7970 6594 8c06 7374  us.}...type...st
-00008610: 7269 6e67 9473 8c07 6d65 7373 6167 6594  ring.s..message.
-00008620: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-00008630: 6794 738c 0776 6572 7369 6f6e 947d 948c  g.s..version.}..
-00008640: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00008650: 8c06 636f 6d6d 6974 947d 948c 0474 7970  ..commit.}...typ
-00008660: 6594 8c06 7374 7269 6e67 9473 8c05 6275  e...string.s..bu
-00008670: 696c 6494 7d94 8c04 7479 7065 948c 0673  ild.}...type...s
-00008680: 7472 696e 6794 738c 086d 6574 6164 6174  tring.s..metadat
-00008690: 6194 7d94 8c04 2472 6566 948c 2323 2f63  a.}...$ref..##/c
-000086a0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
-000086b0: 732f 5265 7375 6c74 4d65 7461 6461 7461  s/ResultMetadata
-000086c0: 9473 8c06 7265 7375 6c74 947d 948c 0474  .s..result.}...t
-000086d0: 7970 6594 8c06 6f62 6a65 6374 9473 7575  ype...object.suu
-000086e0: 8c0e 4a6f 6248 6964 6544 6973 706c 6179  ..JobHideDisplay
-000086f0: 947d 9428 8c04 7479 7065 948c 066f 626a  .}.(..type...obj
-00008700: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
-00008710: 947d 948c 076d 6573 7361 6765 947d 948c  .}...message.}..
-00008720: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00008730: 7375 8c0b 5265 7370 4869 6465 4a6f 6294  su..RespHideJob.
-00008740: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-00008750: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-00008760: 7d94 288c 0673 7461 7475 7394 7d94 8c04  }.(..status.}...
-00008770: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00008780: 076d 6573 7361 6765 947d 948c 0474 7970  .message.}...typ
-00008790: 6594 8c06 7374 7269 6e67 9473 8c07 7665  e...string.s..ve
-000087a0: 7273 696f 6e94 7d94 8c04 7479 7065 948c  rsion.}...type..
-000087b0: 0673 7472 696e 6794 738c 0663 6f6d 6d69  .string.s..commi
-000087c0: 7494 7d94 8c04 7479 7065 948c 0673 7472  t.}...type...str
-000087d0: 696e 6794 738c 0562 7569 6c64 947d 948c  ing.s..build.}..
-000087e0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-000087f0: 8c08 6d65 7461 6461 7461 947d 948c 0424  ..metadata.}...$
-00008800: 7265 6694 8c23 232f 636f 6d70 6f6e 656e  ref..##/componen
-00008810: 7473 2f73 6368 656d 6173 2f52 6573 756c  ts/schemas/Resul
-00008820: 744d 6574 6164 6174 6194 738c 0672 6573  tMetadata.s..res
-00008830: 756c 7494 7d94 8c04 2472 6566 948c 2323  ult.}...$ref..##
-00008840: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-00008850: 6d61 732f 4a6f 6248 6964 6544 6973 706c  mas/JobHideDispl
-00008860: 6179 9473 7575 8c08 5265 7370 4e61 6d65  ay.suu..RespName
-00008870: 947d 9428 8c04 7479 7065 948c 066f 626a  .}.(..type...obj
-00008880: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
-00008890: 947d 9428 8c06 7374 6174 7573 947d 948c  .}.(..status.}..
-000088a0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-000088b0: 8c07 6d65 7373 6167 6594 7d94 8c04 7479  ..message.}...ty
-000088c0: 7065 948c 0673 7472 696e 6794 738c 0776  pe...string.s..v
-000088d0: 6572 7369 6f6e 947d 948c 0474 7970 6594  ersion.}...type.
-000088e0: 8c06 7374 7269 6e67 9473 8c06 636f 6d6d  ..string.s..comm
-000088f0: 6974 947d 948c 0474 7970 6594 8c06 7374  it.}...type...st
-00008900: 7269 6e67 9473 8c05 6275 696c 6494 7d94  ring.s..build.}.
-00008910: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00008920: 738c 086d 6574 6164 6174 6194 7d94 8c04  s..metadata.}...
-00008930: 2472 6566 948c 2323 2f63 6f6d 706f 6e65  $ref..##/compone
-00008940: 6e74 732f 7363 6865 6d61 732f 5265 7375  nts/schemas/Resu
-00008950: 6c74 4d65 7461 6461 7461 9473 8c06 7265  ltMetadata.s..re
-00008960: 7375 6c74 947d 948c 0424 7265 6694 8c1f  sult.}...$ref...
-00008970: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
-00008980: 656d 6173 2f52 6573 756c 744e 616d 6594  emas/ResultName.
-00008990: 7375 758c 0a52 6573 756c 744e 616d 6594  suu..ResultName.
-000089a0: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-000089b0: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-000089c0: 7d94 8c04 6e61 6d65 947d 948c 0474 7970  }...name.}...typ
-000089d0: 6594 8c06 7374 7269 6e67 9473 7375 8c10  e...string.ssu..
-000089e0: 4a6f 6243 616e 6365 6c44 6973 706c 6179  JobCancelDisplay
-000089f0: 947d 9428 8c04 7479 7065 948c 066f 626a  .}.(..type...obj
-00008a00: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
-00008a10: 947d 948c 076d 6573 7361 6765 947d 948c  .}...message.}..
-00008a20: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00008a30: 7375 8c0d 5265 7370 4361 6e63 656c 4a6f  su..RespCancelJo
-00008a40: 6294 7d94 288c 0474 7970 6594 8c06 6f62  b.}.(..type...ob
-00008a50: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
-00008a60: 7394 7d94 288c 0673 7461 7475 7394 7d94  s.}.(..status.}.
-00008a70: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00008a80: 738c 076d 6573 7361 6765 947d 948c 0474  s..message.}...t
-00008a90: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
-00008aa0: 7665 7273 696f 6e94 7d94 8c04 7479 7065  version.}...type
-00008ab0: 948c 0673 7472 696e 6794 738c 0663 6f6d  ...string.s..com
-00008ac0: 6d69 7494 7d94 8c04 7479 7065 948c 0673  mit.}...type...s
-00008ad0: 7472 696e 6794 738c 0562 7569 6c64 947d  tring.s..build.}
-00008ae0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00008af0: 9473 8c08 6d65 7461 6461 7461 947d 948c  .s..metadata.}..
-00008b00: 0424 7265 6694 8c23 232f 636f 6d70 6f6e  .$ref..##/compon
-00008b10: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
-00008b20: 756c 744d 6574 6164 6174 6194 738c 0672  ultMetadata.s..r
-00008b30: 6573 756c 7494 7d94 8c04 2472 6566 948c  esult.}...$ref..
-00008b40: 2523 2f63 6f6d 706f 6e65 6e74 732f 7363  %#/components/sc
-00008b50: 6865 6d61 732f 4a6f 6243 616e 6365 6c44  hemas/JobCancelD
-00008b60: 6973 706c 6179 9473 7575 8c03 4a6f 6294  isplay.suu..Job.
-00008b70: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-00008b80: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-00008b90: 7d94 288c 0269 6494 7d94 288c 0474 7970  }.(..id.}.(..typ
-00008ba0: 6594 8c07 696e 7465 6765 7294 8c06 666f  e...integer...fo
-00008bb0: 726d 6174 948c 0569 6e74 3332 9475 8c04  rmat...int32.u..
-00008bc0: 6e61 6d65 947d 948c 0474 7970 6594 8c06  name.}...type...
-00008bd0: 7374 7269 6e67 9473 8c05 6f77 6e65 7294  string.s..owner.
-00008be0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-00008bf0: 6794 738c 0674 656e 616e 7494 7d94 8c04  g.s..tenant.}...
-00008c00: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00008c10: 0b64 6573 6372 6970 7469 6f6e 947d 948c  .description.}..
-00008c20: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00008c30: 8c06 7374 6174 7573 947d 9428 8c04 7479  ..status.}.(..ty
-00008c40: 7065 948c 0673 7472 696e 6794 8c04 656e  pe...string...en
-00008c50: 756d 945d 9428 8c07 5045 4e44 494e 4794  um.].(..PENDING.
-00008c60: 8c11 5052 4f43 4553 5349 4e47 5f49 4e50  ..PROCESSING_INP
-00008c70: 5554 5394 8c0e 5354 4147 494e 475f 494e  UTS...STAGING_IN
-00008c80: 5055 5453 948c 0b53 5441 4749 4e47 5f4a  PUTS...STAGING_J
-00008c90: 4f42 948c 0e53 5542 4d49 5454 494e 475f  OB...SUBMITTING_
-00008ca0: 4a4f 4294 8c06 5155 4555 4544 948c 0752  JOB...QUEUED...R
-00008cb0: 554e 4e49 4e47 948c 0941 5243 4849 5649  UNNING...ARCHIVI
-00008cc0: 4e47 948c 0742 4c4f 434b 4544 948c 0650  NG...BLOCKED...P
-00008cd0: 4155 5345 4494 8c08 4649 4e49 5348 4544  AUSED...FINISHED
-00008ce0: 948c 0943 414e 4345 4c4c 4544 948c 0646  ...CANCELLED...F
-00008cf0: 4149 4c45 4494 6575 8c0b 6c61 7374 4d65  AILED.eu..lastMe
-00008d00: 7373 6167 6594 7d94 8c04 7479 7065 948c  ssage.}...type..
-00008d10: 0673 7472 696e 6794 738c 0763 7265 6174  .string.s..creat
-00008d20: 6564 947d 948c 0474 7970 6594 8c06 7374  ed.}...type...st
-00008d30: 7269 6e67 9473 8c05 656e 6465 6494 7d94  ring.s..ended.}.
-00008d40: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00008d50: 738c 0b6c 6173 7455 7064 6174 6564 947d  s..lastUpdated.}
-00008d60: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00008d70: 9473 8c04 7575 6964 947d 948c 0474 7970  .s..uuid.}...typ
-00008d80: 6594 8c06 7374 7269 6e67 9473 8c05 6170  e...string.s..ap
-00008d90: 7049 6494 7d94 8c04 7479 7065 948c 0673  pId.}...type...s
-00008da0: 7472 696e 6794 738c 0a61 7070 5665 7273  tring.s..appVers
-00008db0: 696f 6e94 7d94 8c04 7479 7065 948c 0673  ion.}...type...s
-00008dc0: 7472 696e 6794 738c 1161 7263 6869 7665  tring.s..archive
-00008dd0: 4f6e 4170 7045 7272 6f72 947d 948c 0474  OnAppError.}...t
-00008de0: 7970 6594 8c07 626f 6f6c 6561 6e94 738c  ype...boolean.s.
-00008df0: 1164 796e 616d 6963 4578 6563 5379 7374  .dynamicExecSyst
-00008e00: 656d 947d 948c 0474 7970 6594 8c07 626f  em.}...type...bo
-00008e10: 6f6c 6561 6e94 738c 0c65 7865 6353 7973  olean.s..execSys
-00008e20: 7465 6d49 6494 7d94 8c04 7479 7065 948c  temId.}...type..
-00008e30: 0673 7472 696e 6794 738c 1165 7865 6353  .string.s..execS
-00008e40: 7973 7465 6d45 7865 6344 6972 947d 948c  ystemExecDir.}..
-00008e50: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00008e60: 8c12 6578 6563 5379 7374 656d 496e 7075  ..execSystemInpu
-00008e70: 7444 6972 947d 948c 0474 7970 6594 8c06  tDir.}...type...
-00008e80: 7374 7269 6e67 9473 8c13 6578 6563 5379  string.s..execSy
-00008e90: 7374 656d 4f75 7470 7574 4469 7294 7d94  stemOutputDir.}.
-00008ea0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00008eb0: 738c 1665 7865 6353 7973 7465 6d4c 6f67  s..execSystemLog
-00008ec0: 6963 616c 5175 6575 6594 7d94 8c04 7479  icalQueue.}...ty
-00008ed0: 7065 948c 0673 7472 696e 6794 738c 0f61  pe...string.s..a
-00008ee0: 7263 6869 7665 5379 7374 656d 4964 947d  rchiveSystemId.}
-00008ef0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00008f00: 9473 8c10 6172 6368 6976 6553 7973 7465  .s..archiveSyste
-00008f10: 6d44 6972 947d 948c 0474 7970 6594 8c06  mDir.}...type...
-00008f20: 7374 7269 6e67 9473 8c0b 6474 6e53 7973  string.s..dtnSys
-00008f30: 7465 6d49 6494 7d94 8c04 7479 7065 948c  temId.}...type..
-00008f40: 0673 7472 696e 6794 738c 1264 746e 4d6f  .string.s..dtnMo
-00008f50: 756e 7453 6f75 7263 6550 6174 6894 7d94  untSourcePath.}.
-00008f60: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00008f70: 738c 0d64 746e 4d6f 756e 7450 6f69 6e74  s..dtnMountPoint
-00008f80: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00008f90: 6e67 9473 8c09 6e6f 6465 436f 756e 7494  ng.s..nodeCount.
-00008fa0: 7d94 288c 0474 7970 6594 8c07 696e 7465  }.(..type...inte
-00008fb0: 6765 7294 8c06 666f 726d 6174 948c 0569  ger...format...i
-00008fc0: 6e74 3332 9475 8c0c 636f 7265 7350 6572  nt32.u..coresPer
-00008fd0: 4e6f 6465 947d 9428 8c04 7479 7065 948c  Node.}.(..type..
-00008fe0: 0769 6e74 6567 6572 948c 0666 6f72 6d61  .integer...forma
-00008ff0: 7494 8c05 696e 7433 3294 758c 086d 656d  t...int32.u..mem
-00009000: 6f72 794d 4294 7d94 288c 0474 7970 6594  oryMB.}.(..type.
-00009010: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
-00009020: 6174 948c 0569 6e74 3332 9475 8c0a 6d61  at...int32.u..ma
-00009030: 784d 696e 7574 6573 947d 9428 8c04 7479  xMinutes.}.(..ty
-00009040: 7065 948c 0769 6e74 6567 6572 948c 0666  pe...integer...f
-00009050: 6f72 6d61 7494 8c05 696e 7433 3294 758c  ormat...int32.u.
-00009060: 0a66 696c 6549 6e70 7574 7394 7d94 8c04  .fileInputs.}...
-00009070: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00009080: 0c70 6172 616d 6574 6572 5365 7494 7d94  .parameterSet.}.
-00009090: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-000090a0: 738c 1565 7865 6353 7973 7465 6d43 6f6e  s..execSystemCon
-000090b0: 7374 7261 696e 7473 947d 948c 0474 7970  straints.}...typ
-000090c0: 6594 8c06 7374 7269 6e67 9473 8c0d 7375  e...string.s..su
-000090d0: 6273 6372 6970 7469 6f6e 7394 7d94 8c04  bscriptions.}...
-000090e0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-000090f0: 0c62 6c6f 636b 6564 436f 756e 7494 7d94  .blockedCount.}.
-00009100: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
-00009110: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
-00009120: 3332 9475 8c0b 7265 6d6f 7465 4a6f 6249  32.u..remoteJobI
-00009130: 6494 7d94 8c04 7479 7065 948c 0673 7472  d.}...type...str
-00009140: 696e 6794 738c 0c72 656d 6f74 654a 6f62  ing.s..remoteJob
-00009150: 4964 3294 7d94 8c04 7479 7065 948c 0673  Id2.}...type...s
-00009160: 7472 696e 6794 738c 0d72 656d 6f74 654f  tring.s..remoteO
-00009170: 7574 636f 6d65 947d 9428 8c04 7479 7065  utcome.}.(..type
-00009180: 948c 0673 7472 696e 6794 8c04 656e 756d  ...string...enum
-00009190: 945d 9428 8c08 4649 4e49 5348 4544 948c  .].(..FINISHED..
-000091a0: 0646 4149 4c45 4494 8c13 4641 494c 4544  .FAILED...FAILED
-000091b0: 5f53 4b49 505f 4152 4348 4956 4594 6575  _SKIP_ARCHIVE.eu
-000091c0: 8c10 7265 6d6f 7465 5265 7375 6c74 496e  ..remoteResultIn
-000091d0: 666f 947d 948c 0474 7970 6594 8c06 7374  fo.}...type...st
-000091e0: 7269 6e67 9473 8c0b 7265 6d6f 7465 5175  ring.s..remoteQu
-000091f0: 6575 6594 7d94 8c04 7479 7065 948c 0673  eue.}...type...s
-00009200: 7472 696e 6794 738c 0f72 656d 6f74 6553  tring.s..remoteS
-00009210: 7562 6d69 7474 6564 947d 948c 0474 7970  ubmitted.}...typ
-00009220: 6594 8c06 7374 7269 6e67 9473 8c0d 7265  e...string.s..re
-00009230: 6d6f 7465 5374 6172 7465 6494 7d94 8c04  moteStarted.}...
-00009240: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00009250: 0b72 656d 6f74 6545 6e64 6564 947d 948c  .remoteEnded.}..
-00009260: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00009270: 8c13 7265 6d6f 7465 5375 626d 6974 5265  ..remoteSubmitRe
-00009280: 7472 6965 7394 7d94 288c 0474 7970 6594  tries.}.(..type.
-00009290: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
-000092a0: 6174 948c 0569 6e74 3332 9475 8c13 7265  at...int32.u..re
-000092b0: 6d6f 7465 4368 6563 6b73 5375 6363 6573  moteChecksSucces
-000092c0: 7394 7d94 288c 0474 7970 6594 8c07 696e  s.}.(..type...in
-000092d0: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
-000092e0: 0569 6e74 3332 9475 8c12 7265 6d6f 7465  .int32.u..remote
-000092f0: 4368 6563 6b73 4661 696c 6564 947d 9428  ChecksFailed.}.(
-00009300: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
-00009310: 948c 0666 6f72 6d61 7494 8c05 696e 7433  ...format...int3
-00009320: 3294 758c 1572 656d 6f74 654c 6173 7453  2.u..remoteLastS
-00009330: 7461 7475 7343 6865 636b 947d 948c 0474  tatusCheck.}...t
-00009340: 7970 6594 8c06 7374 7269 6e67 9473 8c12  ype...string.s..
-00009350: 696e 7075 7454 7261 6e73 6163 7469 6f6e  inputTransaction
-00009360: 4964 947d 948c 0474 7970 6594 8c06 7374  Id.}...type...st
-00009370: 7269 6e67 9473 8c12 696e 7075 7443 6f72  ring.s..inputCor
-00009380: 7265 6c61 7469 6f6e 4964 947d 948c 0474  relationId.}...t
-00009390: 7970 6594 8c06 7374 7269 6e67 9473 8c14  ype...string.s..
-000093a0: 6172 6368 6976 6554 7261 6e73 6163 7469  archiveTransacti
-000093b0: 6f6e 4964 947d 948c 0474 7970 6594 8c06  onId.}...type...
-000093c0: 7374 7269 6e67 9473 8c14 6172 6368 6976  string.s..archiv
-000093d0: 6543 6f72 7265 6c61 7469 6f6e 4964 947d  eCorrelationId.}
-000093e0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-000093f0: 9473 8c0a 7461 7069 7351 7565 7565 947d  .s..tapisQueue.}
-00009400: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00009410: 9473 8c07 7669 7369 626c 6594 7d94 8c04  .s..visible.}...
-00009420: 7479 7065 948c 0762 6f6f 6c65 616e 9473  type...boolean.s
-00009430: 8c09 6372 6561 7465 6462 7994 7d94 8c04  ..createdby.}...
-00009440: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00009450: 0f63 7265 6174 6564 6279 5465 6e61 6e74  .createdbyTenant
-00009460: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00009470: 6e67 9473 8c04 7461 6773 947d 9428 8c04  ng.s..tags.}.(..
-00009480: 7479 7065 948c 0561 7272 6179 948c 0569  type...array...i
-00009490: 7465 6d73 947d 948c 0474 7970 6594 8c06  tems.}...type...
-000094a0: 7374 7269 6e67 9473 758c 076a 6f62 5479  string.su..jobTy
-000094b0: 7065 947d 9428 8c04 7479 7065 948c 0673  pe.}.(..type...s
-000094c0: 7472 696e 6794 8c04 656e 756d 945d 9428  tring...enum.].(
-000094d0: 8c04 464f 524b 948c 0542 4154 4348 9465  ..FORK...BATCH.e
-000094e0: 758c 066d 7069 436d 6494 7d94 8c04 7479  u..mpiCmd.}...ty
-000094f0: 7065 948c 0673 7472 696e 6794 738c 0963  pe...string.s..c
-00009500: 6d64 5072 6566 6978 947d 948c 0474 7970  mdPrefix.}...typ
-00009510: 6594 8c06 7374 7269 6e67 9473 8c0c 7368  e...string.s..sh
-00009520: 6172 6564 4170 7043 7478 947d 948c 0474  aredAppCtx.}...t
-00009530: 7970 6594 8c07 626f 6f6c 6561 6e94 738c  ype...boolean.s.
-00009540: 1373 6861 7265 6441 7070 4374 7841 7474  .sharedAppCtxAtt
-00009550: 7269 6273 947d 9428 8c04 7479 7065 948c  ribs.}.(..type..
-00009560: 0561 7272 6179 948c 0569 7465 6d73 947d  .array...items.}
-00009570: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
-00009580: 6794 8c04 656e 756d 945d 9428 8c12 5341  g...enum.].(..SA
-00009590: 435f 4558 4543 5f53 5953 5445 4d5f 4944  C_EXEC_SYSTEM_ID
-000095a0: 948c 1853 4143 5f45 5845 435f 5359 5354  ...SAC_EXEC_SYST
-000095b0: 454d 5f45 5845 435f 4449 5294 8c19 5341  EM_EXEC_DIR...SA
-000095c0: 435f 4558 4543 5f53 5953 5445 4d5f 494e  C_EXEC_SYSTEM_IN
-000095d0: 5055 545f 4449 5294 8c1a 5341 435f 4558  PUT_DIR...SAC_EX
-000095e0: 4543 5f53 5953 5445 4d5f 4f55 5450 5554  EC_SYSTEM_OUTPUT
-000095f0: 5f44 4952 948c 1553 4143 5f41 5243 4849  _DIR...SAC_ARCHI
-00009600: 5645 5f53 5953 5445 4d5f 4944 948c 1653  VE_SYSTEM_ID...S
-00009610: 4143 5f41 5243 4849 5645 5f53 5953 5445  AC_ARCHIVE_SYSTE
-00009620: 4d5f 4449 5294 6575 758c 056e 6f74 6573  M_DIR.euu..notes
-00009630: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00009640: 6e67 9473 8c03 6d70 6994 7d94 8c04 7479  ng.s..mpi.}...ty
-00009650: 7065 948c 0762 6f6f 6c65 616e 9473 7575  pe...boolean.suu
-00009660: 8c0a 5265 7370 4765 744a 6f62 947d 9428  ..RespGetJob.}.(
-00009670: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
-00009680: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
-00009690: 8c06 7374 6174 7573 947d 948c 0474 7970  ..status.}...typ
-000096a0: 6594 8c06 7374 7269 6e67 9473 8c07 6d65  e...string.s..me
-000096b0: 7373 6167 6594 7d94 8c04 7479 7065 948c  ssage.}...type..
-000096c0: 0673 7472 696e 6794 738c 0776 6572 7369  .string.s..versi
-000096d0: 6f6e 947d 948c 0474 7970 6594 8c06 7374  on.}...type...st
-000096e0: 7269 6e67 9473 8c06 636f 6d6d 6974 947d  ring.s..commit.}
-000096f0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00009700: 9473 8c05 6275 696c 6494 7d94 8c04 7479  .s..build.}...ty
-00009710: 7065 948c 0673 7472 696e 6794 738c 086d  pe...string.s..m
-00009720: 6574 6164 6174 6194 7d94 8c04 2472 6566  etadata.}...$ref
-00009730: 948c 2323 2f63 6f6d 706f 6e65 6e74 732f  ..##/components/
-00009740: 7363 6865 6d61 732f 5265 7375 6c74 4d65  schemas/ResultMe
-00009750: 7461 6461 7461 9473 8c06 7265 7375 6c74  tadata.s..result
-00009760: 947d 948c 0424 7265 6694 8c18 232f 636f  .}...$ref...#/co
-00009770: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-00009780: 2f4a 6f62 9473 7575 8c14 4a6f 6248 6973  /Job.suu..JobHis
-00009790: 746f 7279 4469 7370 6c61 7944 544f 947d  toryDisplayDTO.}
-000097a0: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
-000097b0: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
-000097c0: 9428 8c05 6576 656e 7494 7d94 8c04 7479  .(..event.}...ty
-000097d0: 7065 948c 0673 7472 696e 6794 738c 0763  pe...string.s..c
-000097e0: 7265 6174 6564 947d 9428 8c04 7479 7065  reated.}.(..type
-000097f0: 948c 0673 7472 696e 6794 8c06 666f 726d  ...string...form
-00009800: 6174 948c 0964 6174 652d 7469 6d65 9475  at...date-time.u
-00009810: 8c0b 6576 656e 7444 6574 6169 6c94 7d94  ..eventDetail.}.
-00009820: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00009830: 738c 0b64 6573 6372 6970 7469 6f6e 947d  s..description.}
-00009840: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00009850: 9473 8c10 7472 616e 7366 6572 5461 736b  .s..transferTask
-00009860: 5575 6964 947d 948c 0474 7970 6594 8c06  Uuid.}...type...
-00009870: 7374 7269 6e67 9473 7575 8c0e 5265 7370  string.suu..Resp
-00009880: 4a6f 6248 6973 746f 7279 947d 9428 8c04  JobHistory.}.(..
-00009890: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
-000098a0: 7072 6f70 6572 7469 6573 947d 9428 8c06  properties.}.(..
-000098b0: 7374 6174 7573 947d 948c 0474 7970 6594  status.}...type.
-000098c0: 8c06 7374 7269 6e67 9473 8c07 6d65 7373  ..string.s..mess
-000098d0: 6167 6594 7d94 8c04 7479 7065 948c 0673  age.}...type...s
-000098e0: 7472 696e 6794 738c 0776 6572 7369 6f6e  tring.s..version
-000098f0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00009900: 6e67 9473 8c06 636f 6d6d 6974 947d 948c  ng.s..commit.}..
-00009910: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-00009920: 8c05 6275 696c 6494 7d94 8c04 7479 7065  ..build.}...type
-00009930: 948c 0673 7472 696e 6794 738c 086d 6574  ...string.s..met
-00009940: 6164 6174 6194 7d94 8c04 2472 6566 948c  adata.}...$ref..
-00009950: 2323 2f63 6f6d 706f 6e65 6e74 732f 7363  ##/components/sc
-00009960: 6865 6d61 732f 5265 7375 6c74 4d65 7461  hemas/ResultMeta
-00009970: 6461 7461 9473 8c06 7265 7375 6c74 947d  data.s..result.}
-00009980: 9428 8c04 7479 7065 948c 0561 7272 6179  .(..type...array
-00009990: 948c 0569 7465 6d73 947d 948c 0424 7265  ...items.}...$re
-000099a0: 6694 8c29 232f 636f 6d70 6f6e 656e 7473  f..)#/components
-000099b0: 2f73 6368 656d 6173 2f4a 6f62 4869 7374  /schemas/JobHist
-000099c0: 6f72 7944 6973 706c 6179 4454 4f94 7375  oryDisplayDTO.su
-000099d0: 7575 8c0a 4a6f 624c 6973 7444 544f 947d  uu..JobListDTO.}
-000099e0: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
-000099f0: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
-00009a00: 9428 8c04 7575 6964 947d 948c 0474 7970  .(..uuid.}...typ
-00009a10: 6594 8c06 7374 7269 6e67 9473 8c04 6e61  e...string.s..na
-00009a20: 6d65 947d 948c 0474 7970 6594 8c06 7374  me.}...type...st
-00009a30: 7269 6e67 9473 8c05 6f77 6e65 7294 7d94  ring.s..owner.}.
-00009a40: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00009a50: 738c 0561 7070 4964 947d 948c 0474 7970  s..appId.}...typ
-00009a60: 6594 8c06 7374 7269 6e67 9473 8c07 6372  e...string.s..cr
-00009a70: 6561 7465 6494 7d94 288c 0474 7970 6594  eated.}.(..type.
-00009a80: 8c06 7374 7269 6e67 948c 0666 6f72 6d61  ..string...forma
-00009a90: 7494 8c09 6461 7465 2d74 696d 6594 758c  t...date-time.u.
-00009aa0: 0673 7461 7475 7394 7d94 288c 0474 7970  .status.}.(..typ
-00009ab0: 6594 8c06 7374 7269 6e67 948c 0465 6e75  e...string...enu
-00009ac0: 6d94 5d94 288c 0750 454e 4449 4e47 948c  m.].(..PENDING..
-00009ad0: 1150 524f 4345 5353 494e 475f 494e 5055  .PROCESSING_INPU
-00009ae0: 5453 948c 0e53 5441 4749 4e47 5f49 4e50  TS...STAGING_INP
-00009af0: 5554 5394 8c0b 5354 4147 494e 475f 4a4f  UTS...STAGING_JO
-00009b00: 4294 8c0e 5355 424d 4954 5449 4e47 5f4a  B...SUBMITTING_J
-00009b10: 4f42 948c 0651 5545 5545 4494 8c07 5255  OB...QUEUED...RU
-00009b20: 4e4e 494e 4794 8c09 4152 4348 4956 494e  NNING...ARCHIVIN
-00009b30: 4794 8c07 424c 4f43 4b45 4494 8c06 5041  G...BLOCKED...PA
-00009b40: 5553 4544 948c 0846 494e 4953 4845 4494  USED...FINISHED.
-00009b50: 8c09 4341 4e43 454c 4c45 4494 8c06 4641  ..CANCELLED...FA
-00009b60: 494c 4544 9465 758c 0d72 656d 6f74 6553  ILED.eu..remoteS
-00009b70: 7461 7274 6564 947d 9428 8c04 7479 7065  tarted.}.(..type
-00009b80: 948c 0673 7472 696e 6794 8c06 666f 726d  ...string...form
-00009b90: 6174 948c 0964 6174 652d 7469 6d65 9475  at...date-time.u
-00009ba0: 8c05 656e 6465 6494 7d94 288c 0474 7970  ..ended.}.(..typ
-00009bb0: 6594 8c06 7374 7269 6e67 948c 0666 6f72  e...string...for
-00009bc0: 6d61 7494 8c09 6461 7465 2d74 696d 6594  mat...date-time.
-00009bd0: 758c 0674 656e 616e 7494 7d94 8c04 7479  u..tenant.}...ty
-00009be0: 7065 948c 0673 7472 696e 6794 738c 0c65  pe...string.s..e
-00009bf0: 7865 6353 7973 7465 6d49 6494 7d94 8c04  xecSystemId.}...
-00009c00: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-00009c10: 0f61 7263 6869 7665 5379 7374 656d 4964  .archiveSystemId
-00009c20: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00009c30: 6e67 9473 8c0a 6170 7056 6572 7369 6f6e  ng.s..appVersion
-00009c40: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-00009c50: 6e67 9473 8c0b 6c61 7374 5570 6461 7465  ng.s..lastUpdate
-00009c60: 6494 7d94 288c 0474 7970 6594 8c06 7374  d.}.(..type...st
-00009c70: 7269 6e67 948c 0666 6f72 6d61 7494 8c09  ring...format...
-00009c80: 6461 7465 2d74 696d 6594 7575 758c 0e52  date-time.uuu..R
-00009c90: 6573 7047 6574 4a6f 624c 6973 7494 7d94  espGetJobList.}.
-00009ca0: 288c 0474 7970 6594 8c06 6f62 6a65 6374  (..type...object
-00009cb0: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
-00009cc0: 288c 0673 7461 7475 7394 7d94 8c04 7479  (..status.}...ty
-00009cd0: 7065 948c 0673 7472 696e 6794 738c 076d  pe...string.s..m
-00009ce0: 6573 7361 6765 947d 948c 0474 7970 6594  essage.}...type.
-00009cf0: 8c06 7374 7269 6e67 9473 8c07 7665 7273  ..string.s..vers
-00009d00: 696f 6e94 7d94 8c04 7479 7065 948c 0673  ion.}...type...s
-00009d10: 7472 696e 6794 738c 0663 6f6d 6d69 7494  tring.s..commit.
-00009d20: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-00009d30: 6794 738c 0562 7569 6c64 947d 948c 0474  g.s..build.}...t
-00009d40: 7970 6594 8c06 7374 7269 6e67 9473 8c08  ype...string.s..
-00009d50: 6d65 7461 6461 7461 947d 948c 0424 7265  metadata.}...$re
-00009d60: 6694 8c23 232f 636f 6d70 6f6e 656e 7473  f..##/components
-00009d70: 2f73 6368 656d 6173 2f52 6573 756c 744d  /schemas/ResultM
-00009d80: 6574 6164 6174 6194 738c 0672 6573 756c  etadata.s..resul
-00009d90: 7494 7d94 288c 0474 7970 6594 8c05 6172  t.}.(..type...ar
-00009da0: 7261 7994 8c05 6974 656d 7394 7d94 8c04  ray...items.}...
-00009db0: 2472 6566 948c 1f23 2f63 6f6d 706f 6e65  $ref...#/compone
-00009dc0: 6e74 732f 7363 6865 6d61 732f 4a6f 624c  nts/schemas/JobL
-00009dd0: 6973 7444 544f 9473 7575 758c 0846 696c  istDTO.suuu..Fil
-00009de0: 6549 6e66 6f94 7d94 288c 0474 7970 6594  eInfo.}.(..type.
-00009df0: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
-00009e00: 7274 6965 7394 7d94 288c 086d 696d 6554  rties.}.(..mimeT
-00009e10: 7970 6594 7d94 8c04 7479 7065 948c 0673  ype.}...type...s
-00009e20: 7472 696e 6794 738c 0474 7970 6594 7d94  tring.s..type.}.
-00009e30: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-00009e40: 738c 056f 776e 6572 947d 948c 0474 7970  s..owner.}...typ
-00009e50: 6594 8c06 7374 7269 6e67 9473 8c05 6772  e...string.s..gr
-00009e60: 6f75 7094 7d94 8c04 7479 7065 948c 0673  oup.}...type...s
-00009e70: 7472 696e 6794 738c 116e 6174 6976 6550  tring.s..nativeP
-00009e80: 6572 6d69 7373 696f 6e73 947d 948c 0474  ermissions.}...t
-00009e90: 7970 6594 8c06 7374 7269 6e67 9473 8c03  ype...string.s..
-00009ea0: 7572 6c94 7d94 8c04 7479 7065 948c 0673  url.}...type...s
-00009eb0: 7472 696e 6794 738c 0c6c 6173 744d 6f64  tring.s..lastMod
-00009ec0: 6966 6965 6494 7d94 288c 0474 7970 6594  ified.}.(..type.
-00009ed0: 8c06 7374 7269 6e67 948c 0666 6f72 6d61  ..string...forma
-00009ee0: 7494 8c09 6461 7465 2d74 696d 6594 758c  t...date-time.u.
-00009ef0: 046e 616d 6594 7d94 8c04 7479 7065 948c  .name.}...type..
-00009f00: 0673 7472 696e 6794 738c 0470 6174 6894  .string.s..path.
-00009f10: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-00009f20: 6794 738c 0473 697a 6594 7d94 288c 0474  g.s..size.}.(..t
-00009f30: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
-00009f40: 666f 726d 6174 948c 0569 6e74 3634 9475  format...int64.u
-00009f50: 7575 8c14 5265 7370 4765 744a 6f62 4f75  uu..RespGetJobOu
-00009f60: 7470 7574 4c69 7374 947d 9428 8c04 7479  tputList.}.(..ty
-00009f70: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
-00009f80: 6f70 6572 7469 6573 947d 9428 8c06 7374  operties.}.(..st
-00009f90: 6174 7573 947d 948c 0474 7970 6594 8c06  atus.}...type...
-00009fa0: 7374 7269 6e67 9473 8c07 6d65 7373 6167  string.s..messag
-00009fb0: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
-00009fc0: 696e 6794 738c 0776 6572 7369 6f6e 947d  ing.s..version.}
-00009fd0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-00009fe0: 9473 8c06 636f 6d6d 6974 947d 948c 0474  .s..commit.}...t
-00009ff0: 7970 6594 8c06 7374 7269 6e67 9473 8c05  ype...string.s..
-0000a000: 6275 696c 6494 7d94 8c04 7479 7065 948c  build.}...type..
-0000a010: 0673 7472 696e 6794 738c 086d 6574 6164  .string.s..metad
-0000a020: 6174 6194 7d94 8c04 2472 6566 948c 2323  ata.}...$ref..##
-0000a030: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0000a040: 6d61 732f 5265 7375 6c74 4d65 7461 6461  mas/ResultMetada
-0000a050: 7461 9473 8c06 7265 7375 6c74 947d 9428  ta.s..result.}.(
-0000a060: 8c04 7479 7065 948c 0561 7272 6179 948c  ..type...array..
-0000a070: 0569 7465 6d73 947d 948c 0424 7265 6694  .items.}...$ref.
-0000a080: 8c1d 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
-0000a090: 6368 656d 6173 2f46 696c 6549 6e66 6f94  chemas/FileInfo.
-0000a0a0: 7375 7575 8c1a 5265 7370 4a6f 6253 6561  suuu..RespJobSea
-0000a0b0: 7263 6841 6c6c 4174 7472 6962 7574 6573  rchAllAttributes
-0000a0c0: 947d 9428 8c04 7479 7065 948c 066f 626a  .}.(..type...obj
-0000a0d0: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
-0000a0e0: 947d 9428 8c06 7374 6174 7573 947d 948c  .}.(..status.}..
-0000a0f0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000a100: 8c07 6d65 7373 6167 6594 7d94 8c04 7479  ..message.}...ty
-0000a110: 7065 948c 0673 7472 696e 6794 738c 0776  pe...string.s..v
-0000a120: 6572 7369 6f6e 947d 948c 0474 7970 6594  ersion.}...type.
-0000a130: 8c06 7374 7269 6e67 9473 8c06 636f 6d6d  ..string.s..comm
-0000a140: 6974 947d 948c 0474 7970 6594 8c06 7374  it.}...type...st
-0000a150: 7269 6e67 9473 8c05 6275 696c 6494 7d94  ring.s..build.}.
-0000a160: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000a170: 738c 086d 6574 6164 6174 6194 7d94 8c04  s..metadata.}...
-0000a180: 2472 6566 948c 2323 2f63 6f6d 706f 6e65  $ref..##/compone
-0000a190: 6e74 732f 7363 6865 6d61 732f 5265 7375  nts/schemas/Resu
-0000a1a0: 6c74 4d65 7461 6461 7461 9473 8c06 7265  ltMetadata.s..re
-0000a1b0: 7375 6c74 947d 9428 8c04 7479 7065 948c  sult.}.(..type..
-0000a1c0: 0561 7272 6179 948c 0569 7465 6d73 947d  .array...items.}
-0000a1d0: 948c 0424 7265 6694 8c18 232f 636f 6d70  ...$ref...#/comp
-0000a1e0: 6f6e 656e 7473 2f73 6368 656d 6173 2f4a  onents/schemas/J
-0000a1f0: 6f62 9473 7575 758c 114a 6f62 556e 5368  ob.suuu..JobUnSh
-0000a200: 6172 6544 6973 706c 6179 947d 9428 8c04  areDisplay.}.(..
-0000a210: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
-0000a220: 7072 6f70 6572 7469 6573 947d 948c 076d  properties.}...m
-0000a230: 6573 7361 6765 947d 948c 0474 7970 6594  essage.}...type.
-0000a240: 8c06 7374 7269 6e67 9473 7375 8c0e 5265  ..string.ssu..Re
-0000a250: 7370 556e 5368 6172 654a 6f62 947d 9428  spUnShareJob.}.(
-0000a260: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
-0000a270: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
-0000a280: 8c06 7374 6174 7573 947d 948c 0474 7970  ..status.}...typ
-0000a290: 6594 8c06 7374 7269 6e67 9473 8c07 6d65  e...string.s..me
-0000a2a0: 7373 6167 6594 7d94 8c04 7479 7065 948c  ssage.}...type..
-0000a2b0: 0673 7472 696e 6794 738c 0776 6572 7369  .string.s..versi
-0000a2c0: 6f6e 947d 948c 0474 7970 6594 8c06 7374  on.}...type...st
-0000a2d0: 7269 6e67 9473 8c06 636f 6d6d 6974 947d  ring.s..commit.}
-0000a2e0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000a2f0: 9473 8c05 6275 696c 6494 7d94 8c04 7479  .s..build.}...ty
-0000a300: 7065 948c 0673 7472 696e 6794 738c 086d  pe...string.s..m
-0000a310: 6574 6164 6174 6194 7d94 8c04 2472 6566  etadata.}...$ref
-0000a320: 948c 2323 2f63 6f6d 706f 6e65 6e74 732f  ..##/components/
-0000a330: 7363 6865 6d61 732f 5265 7375 6c74 4d65  schemas/ResultMe
-0000a340: 7461 6461 7461 9473 8c06 7265 7375 6c74  tadata.s..result
-0000a350: 947d 948c 0424 7265 6694 8c26 232f 636f  .}...$ref..&#/co
-0000a360: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-0000a370: 2f4a 6f62 556e 5368 6172 6544 6973 706c  /JobUnShareDispl
-0000a380: 6179 9473 7575 8c0f 4a6f 6253 6861 7265  ay.suu..JobShare
-0000a390: 4c69 7374 4454 4f94 7d94 288c 0474 7970  ListDTO.}.(..typ
-0000a3a0: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
-0000a3b0: 7065 7274 6965 7394 7d94 288c 0674 656e  perties.}.(..ten
-0000a3c0: 616e 7494 7d94 8c04 7479 7065 948c 0673  ant.}...type...s
-0000a3d0: 7472 696e 6794 738c 0963 7265 6174 6564  tring.s..created
-0000a3e0: 6279 947d 948c 0474 7970 6594 8c06 7374  by.}...type...st
-0000a3f0: 7269 6e67 9473 8c07 6a6f 6255 7569 6494  ring.s..jobUuid.
-0000a400: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000a410: 6794 738c 0767 7261 6e74 6565 947d 948c  g.s..grantee.}..
-0000a420: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000a430: 8c0b 6a6f 6252 6573 6f75 7263 6594 7d94  ..jobResource.}.
-0000a440: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000a450: 738c 0d6a 6f62 5065 726d 6973 7369 6f6e  s..jobPermission
-0000a460: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000a470: 6e67 9473 8c07 6372 6561 7465 6494 7d94  ng.s..created.}.
-0000a480: 288c 0474 7970 6594 8c06 7374 7269 6e67  (..type...string
-0000a490: 948c 0666 6f72 6d61 7494 8c09 6461 7465  ...format...date
-0000a4a0: 2d74 696d 6594 7575 758c 1352 6573 7047  -time.uuu..RespG
-0000a4b0: 6574 4a6f 6253 6861 7265 4c69 7374 947d  etJobShareList.}
-0000a4c0: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
-0000a4d0: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
-0000a4e0: 9428 8c06 7374 6174 7573 947d 948c 0474  .(..status.}...t
-0000a4f0: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
-0000a500: 6d65 7373 6167 6594 7d94 8c04 7479 7065  message.}...type
-0000a510: 948c 0673 7472 696e 6794 738c 0776 6572  ...string.s..ver
-0000a520: 7369 6f6e 947d 948c 0474 7970 6594 8c06  sion.}...type...
-0000a530: 7374 7269 6e67 9473 8c06 636f 6d6d 6974  string.s..commit
-0000a540: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000a550: 6e67 9473 8c05 6275 696c 6494 7d94 8c04  ng.s..build.}...
-0000a560: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000a570: 086d 6574 6164 6174 6194 7d94 8c04 2472  .metadata.}...$r
-0000a580: 6566 948c 2323 2f63 6f6d 706f 6e65 6e74  ef..##/component
-0000a590: 732f 7363 6865 6d61 732f 5265 7375 6c74  s/schemas/Result
-0000a5a0: 4d65 7461 6461 7461 9473 8c06 7265 7375  Metadata.s..resu
-0000a5b0: 6c74 947d 9428 8c04 7479 7065 948c 0561  lt.}.(..type...a
-0000a5c0: 7272 6179 948c 0569 7465 6d73 947d 948c  rray...items.}..
-0000a5d0: 0424 7265 6694 8c24 232f 636f 6d70 6f6e  .$ref..$#/compon
-0000a5e0: 656e 7473 2f73 6368 656d 6173 2f4a 6f62  ents/schemas/Job
-0000a5f0: 5368 6172 654c 6973 7444 544f 9473 7575  ShareListDTO.suu
-0000a600: 758c 0f4a 6f62 5368 6172 6544 6973 706c  u..JobShareDispl
-0000a610: 6179 947d 9428 8c04 7479 7065 948c 066f  ay.}.(..type...o
-0000a620: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
-0000a630: 6573 947d 948c 076d 6573 7361 6765 947d  es.}...message.}
-0000a640: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000a650: 9473 7375 8c0c 5265 7370 5368 6172 654a  .ssu..RespShareJ
-0000a660: 6f62 947d 9428 8c04 7479 7065 948c 066f  ob.}.(..type...o
-0000a670: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
-0000a680: 6573 947d 9428 8c06 7374 6174 7573 947d  es.}.(..status.}
-0000a690: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000a6a0: 9473 8c07 6d65 7373 6167 6594 7d94 8c04  .s..message.}...
-0000a6b0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000a6c0: 0776 6572 7369 6f6e 947d 948c 0474 7970  .version.}...typ
-0000a6d0: 6594 8c06 7374 7269 6e67 9473 8c06 636f  e...string.s..co
-0000a6e0: 6d6d 6974 947d 948c 0474 7970 6594 8c06  mmit.}...type...
-0000a6f0: 7374 7269 6e67 9473 8c05 6275 696c 6494  string.s..build.
-0000a700: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000a710: 6794 738c 086d 6574 6164 6174 6194 7d94  g.s..metadata.}.
-0000a720: 8c04 2472 6566 948c 2323 2f63 6f6d 706f  ..$ref..##/compo
-0000a730: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
-0000a740: 7375 6c74 4d65 7461 6461 7461 9473 8c06  sultMetadata.s..
-0000a750: 7265 7375 6c74 947d 948c 0424 7265 6694  result.}...$ref.
-0000a760: 8c24 232f 636f 6d70 6f6e 656e 7473 2f73  .$#/components/s
-0000a770: 6368 656d 6173 2f4a 6f62 5368 6172 6544  chemas/JobShareD
-0000a780: 6973 706c 6179 9473 7575 8c0b 5265 7153  isplay.suu..ReqS
-0000a790: 6861 7265 4a6f 6294 7d94 288c 0474 7970  hareJob.}.(..typ
-0000a7a0: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
-0000a7b0: 7065 7274 6965 7394 7d94 288c 0767 7261  perties.}.(..gra
-0000a7c0: 6e74 6565 947d 948c 0474 7970 6594 8c06  ntee.}...type...
-0000a7d0: 7374 7269 6e67 9473 8c0b 6a6f 6252 6573  string.s..jobRes
-0000a7e0: 6f75 7263 6594 7d94 288c 0474 7970 6594  ource.}.(..type.
-0000a7f0: 8c05 6172 7261 7994 8c05 6974 656d 7394  ..array...items.
-0000a800: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
-0000a810: 6e67 948c 0465 6e75 6d94 5d94 288c 0b4a  ng...enum.].(..J
-0000a820: 4f42 5f48 4953 544f 5259 948c 144a 4f42  OB_HISTORY...JOB
-0000a830: 5f52 4553 5542 4d49 545f 5245 5155 4553  _RESUBMIT_REQUES
-0000a840: 5494 8c0a 4a4f 425f 4f55 5450 5554 948c  T...JOB_OUTPUT..
-0000a850: 094a 4f42 5f49 4e50 5554 9465 7575 8c0d  .JOB_INPUT.euu..
-0000a860: 6a6f 6250 6572 6d69 7373 696f 6e94 7d94  jobPermission.}.
-0000a870: 288c 0474 7970 6594 8c06 7374 7269 6e67  (..type...string
-0000a880: 948c 0465 6e75 6d94 5d94 8c04 5245 4144  ...enum.]...READ
-0000a890: 9461 7575 758c 104a 6f62 5374 6174 7573  .auuu..JobStatus
-0000a8a0: 4469 7370 6c61 7994 7d94 288c 0474 7970  Display.}.(..typ
-0000a8b0: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
-0000a8c0: 7065 7274 6965 7394 7d94 8c06 7374 6174  perties.}...stat
-0000a8d0: 7573 947d 948c 0474 7970 6594 8c06 7374  us.}...type...st
-0000a8e0: 7269 6e67 9473 7375 8c10 5265 7370 4765  ring.ssu..RespGe
-0000a8f0: 744a 6f62 5374 6174 7573 947d 9428 8c04  tJobStatus.}.(..
-0000a900: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
-0000a910: 7072 6f70 6572 7469 6573 947d 9428 8c06  properties.}.(..
-0000a920: 7374 6174 7573 947d 948c 0474 7970 6594  status.}...type.
-0000a930: 8c06 7374 7269 6e67 9473 8c07 6d65 7373  ..string.s..mess
-0000a940: 6167 6594 7d94 8c04 7479 7065 948c 0673  age.}...type...s
-0000a950: 7472 696e 6794 738c 0776 6572 7369 6f6e  tring.s..version
-0000a960: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000a970: 6e67 9473 8c06 636f 6d6d 6974 947d 948c  ng.s..commit.}..
-0000a980: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000a990: 8c05 6275 696c 6494 7d94 8c04 7479 7065  ..build.}...type
-0000a9a0: 948c 0673 7472 696e 6794 738c 086d 6574  ...string.s..met
-0000a9b0: 6164 6174 6194 7d94 8c04 2472 6566 948c  adata.}...$ref..
-0000a9c0: 2323 2f63 6f6d 706f 6e65 6e74 732f 7363  ##/components/sc
-0000a9d0: 6865 6d61 732f 5265 7375 6c74 4d65 7461  hemas/ResultMeta
-0000a9e0: 6461 7461 9473 8c06 7265 7375 6c74 947d  data.s..result.}
-0000a9f0: 948c 0424 7265 6694 8c25 232f 636f 6d70  ...$ref..%#/comp
-0000aa00: 6f6e 656e 7473 2f73 6368 656d 6173 2f4a  onents/schemas/J
-0000aa10: 6f62 5374 6174 7573 4469 7370 6c61 7994  obStatusDisplay.
-0000aa20: 7375 758c 1449 6e63 6c75 6465 4578 636c  suu..IncludeExcl
-0000aa30: 7564 6546 696c 7465 7294 7d94 288c 0474  udeFilter.}.(..t
-0000aa40: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
-0000aa50: 726f 7065 7274 6965 7394 7d94 288c 0869  roperties.}.(..i
-0000aa60: 6e63 6c75 6465 7394 7d94 288c 0474 7970  ncludes.}.(..typ
-0000aa70: 6594 8c05 6172 7261 7994 8c05 6974 656d  e...array...item
-0000aa80: 7394 7d94 8c04 7479 7065 948c 0673 7472  s.}...type...str
-0000aa90: 696e 6794 7375 8c08 6578 636c 7564 6573  ing.su..excludes
-0000aaa0: 947d 9428 8c04 7479 7065 948c 0561 7272  .}.(..type...arr
-0000aab0: 6179 948c 0569 7465 6d73 947d 948c 0474  ay...items.}...t
-0000aac0: 7970 6594 8c06 7374 7269 6e67 9473 758c  ype...string.su.
-0000aad0: 1269 6e63 6c75 6465 4c61 756e 6368 4669  .includeLaunchFi
-0000aae0: 6c65 7394 7d94 8c04 7479 7065 948c 0762  les.}...type...b
-0000aaf0: 6f6f 6c65 616e 9473 7575 8c0a 4a6f 6241  oolean.suu..JobA
-0000ab00: 7267 5370 6563 947d 9428 8c04 7479 7065  rgSpec.}.(..type
-0000ab10: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
-0000ab20: 6572 7469 6573 947d 9428 8c04 6e61 6d65  erties.}.(..name
-0000ab30: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000ab40: 6e67 9473 8c0b 6465 7363 7269 7074 696f  ng.s..descriptio
-0000ab50: 6e94 7d94 8c04 7479 7065 948c 0673 7472  n.}...type...str
-0000ab60: 696e 6794 738c 0769 6e63 6c75 6465 947d  ing.s..include.}
-0000ab70: 948c 0474 7970 6594 8c07 626f 6f6c 6561  ...type...boolea
-0000ab80: 6e94 738c 0361 7267 947d 948c 0474 7970  n.s..arg.}...typ
-0000ab90: 6594 8c06 7374 7269 6e67 9473 8c05 6e6f  e...string.s..no
-0000aba0: 7465 7394 7d94 8c04 7479 7065 948c 066f  tes.}...type...o
-0000abb0: 626a 6563 7494 7375 758c 0c4a 6f62 4669  bject.suu..JobFi
-0000abc0: 6c65 496e 7075 7494 7d94 288c 0474 7970  leInput.}.(..typ
-0000abd0: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
-0000abe0: 7065 7274 6965 7394 7d94 288c 046e 616d  perties.}.(..nam
-0000abf0: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
-0000ac00: 696e 6794 738c 0b64 6573 6372 6970 7469  ing.s..descripti
-0000ac10: 6f6e 947d 948c 0474 7970 6594 8c06 7374  on.}...type...st
-0000ac20: 7269 6e67 9473 8c0e 6175 746f 4d6f 756e  ring.s..autoMoun
-0000ac30: 744c 6f63 616c 947d 948c 0474 7970 6594  tLocal.}...type.
-0000ac40: 8c07 626f 6f6c 6561 6e94 738c 0973 6f75  ..boolean.s..sou
-0000ac50: 7263 6555 726c 947d 948c 0474 7970 6594  rceUrl.}...type.
-0000ac60: 8c06 7374 7269 6e67 9473 8c0a 7461 7267  ..string.s..targ
-0000ac70: 6574 5061 7468 947d 948c 0474 7970 6594  etPath.}...type.
-0000ac80: 8c06 7374 7269 6e67 9473 7575 8c11 4a6f  ..string.suu..Jo
-0000ac90: 6246 696c 6549 6e70 7574 4172 7261 7994  bFileInputArray.
-0000aca0: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-0000acb0: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-0000acc0: 7d94 288c 046e 616d 6594 7d94 8c04 7479  }.(..name.}...ty
-0000acd0: 7065 948c 0673 7472 696e 6794 738c 0b64  pe...string.s..d
-0000ace0: 6573 6372 6970 7469 6f6e 947d 948c 0474  escription.}...t
-0000acf0: 7970 6594 8c06 7374 7269 6e67 9473 8c0a  ype...string.s..
-0000ad00: 736f 7572 6365 5572 6c73 947d 9428 8c04  sourceUrls.}.(..
-0000ad10: 7479 7065 948c 0561 7272 6179 948c 0569  type...array...i
-0000ad20: 7465 6d73 947d 948c 0474 7970 6594 8c06  tems.}...type...
-0000ad30: 7374 7269 6e67 9473 758c 0974 6172 6765  string.su..targe
-0000ad40: 7444 6972 947d 948c 0474 7970 6594 8c06  tDir.}...type...
-0000ad50: 7374 7269 6e67 9473 7575 8c0f 4a6f 6250  string.suu..JobP
-0000ad60: 6172 616d 6574 6572 5365 7494 7d94 288c  arameterSet.}.(.
-0000ad70: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
-0000ad80: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
-0000ad90: 0761 7070 4172 6773 947d 9428 8c04 7479  .appArgs.}.(..ty
-0000ada0: 7065 948c 0561 7272 6179 948c 0569 7465  pe...array...ite
-0000adb0: 6d73 947d 948c 0424 7265 6694 8c1f 232f  ms.}...$ref...#/
-0000adc0: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
-0000add0: 6173 2f4a 6f62 4172 6753 7065 6394 7375  as/JobArgSpec.su
-0000ade0: 8c0d 636f 6e74 6169 6e65 7241 7267 7394  ..containerArgs.
-0000adf0: 7d94 288c 0474 7970 6594 8c05 6172 7261  }.(..type...arra
-0000ae00: 7994 8c05 6974 656d 7394 7d94 8c04 2472  y...items.}...$r
-0000ae10: 6566 948c 1f23 2f63 6f6d 706f 6e65 6e74  ef...#/component
-0000ae20: 732f 7363 6865 6d61 732f 4a6f 6241 7267  s/schemas/JobArg
-0000ae30: 5370 6563 9473 758c 1073 6368 6564 756c  Spec.su..schedul
-0000ae40: 6572 4f70 7469 6f6e 7394 7d94 288c 0474  erOptions.}.(..t
-0000ae50: 7970 6594 8c05 6172 7261 7994 8c05 6974  ype...array...it
-0000ae60: 656d 7394 7d94 8c04 2472 6566 948c 1f23  ems.}...$ref...#
-0000ae70: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0000ae80: 6d61 732f 4a6f 6241 7267 5370 6563 9473  mas/JobArgSpec.s
-0000ae90: 758c 0c65 6e76 5661 7269 6162 6c65 7394  u..envVariables.
-0000aea0: 7d94 288c 0474 7970 6594 8c05 6172 7261  }.(..type...arra
-0000aeb0: 7994 8c05 6974 656d 7394 7d94 8c04 2472  y...items.}...$r
-0000aec0: 6566 948c 2123 2f63 6f6d 706f 6e65 6e74  ef..!#/component
-0000aed0: 732f 7363 6865 6d61 732f 4b65 7956 616c  s/schemas/KeyVal
-0000aee0: 7565 5061 6972 9473 758c 0d61 7263 6869  uePair.su..archi
-0000aef0: 7665 4669 6c74 6572 947d 948c 0424 7265  veFilter.}...$re
-0000af00: 6694 8c29 232f 636f 6d70 6f6e 656e 7473  f..)#/components
-0000af10: 2f73 6368 656d 6173 2f49 6e63 6c75 6465  /schemas/Include
-0000af20: 4578 636c 7564 6546 696c 7465 7294 7375  ExcludeFilter.su
-0000af30: 758c 0c4b 6579 5661 6c75 6550 6169 7294  u..KeyValuePair.
-0000af40: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-0000af50: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-0000af60: 7d94 288c 036b 6579 947d 948c 0474 7970  }.(..key.}...typ
-0000af70: 6594 8c06 7374 7269 6e67 9473 8c05 7661  e...string.s..va
-0000af80: 6c75 6594 7d94 8c04 7479 7065 948c 0673  lue.}...type...s
-0000af90: 7472 696e 6794 738c 0b64 6573 6372 6970  tring.s..descrip
-0000afa0: 7469 6f6e 947d 948c 0474 7970 6594 8c06  tion.}...type...
-0000afb0: 7374 7269 6e67 9473 7575 8c13 4e6f 7469  string.suu..Noti
-0000afc0: 6644 656c 6976 6572 7954 6172 6765 7494  fDeliveryTarget.
-0000afd0: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-0000afe0: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-0000aff0: 7d94 288c 0e64 656c 6976 6572 794d 6574  }.(..deliveryMet
-0000b000: 686f 6494 7d94 288c 0474 7970 6594 8c06  hod.}.(..type...
-0000b010: 7374 7269 6e67 948c 0465 6e75 6d94 5d94  string...enum.].
-0000b020: 288c 0757 4542 484f 4f4b 948c 0545 4d41  (..WEBHOOK...EMA
-0000b030: 494c 948c 0551 5545 5545 948c 0541 4354  IL...QUEUE...ACT
-0000b040: 4f52 9465 758c 0f64 656c 6976 6572 7941  OR.eu..deliveryA
-0000b050: 6464 7265 7373 947d 948c 0474 7970 6594  ddress.}...type.
-0000b060: 8c06 7374 7269 6e67 9473 7575 8c0c 5265  ..string.suu..Re
-0000b070: 7153 7562 6d69 744a 6f62 947d 9428 8c08  qSubmitJob.}.(..
-0000b080: 7265 7175 6972 6564 945d 9428 8c05 6170  required.].(..ap
-0000b090: 7049 6494 8c0a 6170 7056 6572 7369 6f6e  pId...appVersion
-0000b0a0: 948c 046e 616d 6594 658c 0474 7970 6594  ...name.e..type.
-0000b0b0: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
-0000b0c0: 7274 6965 7394 7d94 288c 046e 616d 6594  rties.}.(..name.
-0000b0d0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000b0e0: 6794 738c 056f 776e 6572 947d 948c 0474  g.s..owner.}...t
-0000b0f0: 7970 6594 8c06 7374 7269 6e67 9473 8c06  ype...string.s..
-0000b100: 7465 6e61 6e74 947d 948c 0474 7970 6594  tenant.}...type.
-0000b110: 8c06 7374 7269 6e67 9473 8c0b 6465 7363  ..string.s..desc
-0000b120: 7269 7074 696f 6e94 7d94 8c04 7479 7065  ription.}...type
-0000b130: 948c 0673 7472 696e 6794 738c 0561 7070  ...string.s..app
-0000b140: 4964 947d 948c 0474 7970 6594 8c06 7374  Id.}...type...st
-0000b150: 7269 6e67 9473 8c0a 6170 7056 6572 7369  ring.s..appVersi
-0000b160: 6f6e 947d 948c 0474 7970 6594 8c06 7374  on.}...type...st
-0000b170: 7269 6e67 9473 8c07 6a6f 6254 7970 6594  ring.s..jobType.
+000059b0: 696f 6e94 8c0d 5365 7276 6572 2065 7272  ion...Server err
+000059c0: 6f72 2e94 8c07 636f 6e74 656e 7494 7d94  or....content.}.
+000059d0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+000059e0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+000059f0: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
+00005a00: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+00005a10: 7370 4261 7369 6394 7373 7375 758c 0873  spBasic.sssuu..s
+00005a20: 6563 7572 6974 7994 5d94 7d94 8c08 5461  ecurity.].}...Ta
+00005a30: 7069 734a 5754 945d 9473 6175 738c 202f  pisJWT.].saus. /
+00005a40: 6a6f 6273 2f7b 6a6f 6255 7569 647d 2f72  jobs/{jobUuid}/r
+00005a50: 6573 7562 6d69 745f 7265 7175 6573 7494  esubmit_request.
+00005a60: 7d94 8c03 6765 7494 7d94 288c 0474 6167  }...get.}.(..tag
+00005a70: 7394 5d94 8c04 6a6f 6273 9461 8c0b 6465  s.]...jobs.a..de
+00005a80: 7363 7269 7074 696f 6e94 8c33 4765 7420  scription..3Get 
+00005a90: 5265 7375 626d 6974 2072 6571 7565 7374  Resubmit request
+00005aa0: 2066 6f72 206f 6620 6120 6a6f 6220 696e   for of a job in
+00005ab0: 204a 534f 4e20 666f 726d 6174 2e20 2094   JSON format.  .
+00005ac0: 8c0b 6f70 6572 6174 696f 6e49 6494 8c16  ..operationId...
+00005ad0: 6765 7452 6573 7562 6d69 7452 6571 7565  getResubmitReque
+00005ae0: 7374 4a73 6f6e 948c 0a70 6172 616d 6574  stJson...paramet
+00005af0: 6572 7394 5d94 287d 9428 8c04 6e61 6d65  ers.].(}.(..name
+00005b00: 948c 076a 6f62 5575 6964 948c 0269 6e94  ...jobUuid...in.
+00005b10: 8c04 7061 7468 948c 0872 6571 7569 7265  ..path...require
+00005b20: 6494 888c 0673 6368 656d 6194 7d94 8c04  d....schema.}...
+00005b30: 7479 7065 948c 0673 7472 696e 6794 7375  type...string.su
+00005b40: 7d94 288c 046e 616d 6594 8c06 7072 6574  }.(..name...pret
+00005b50: 7479 948c 0269 6e94 8c05 7175 6572 7994  ty...in...query.
+00005b60: 8c06 7363 6865 6d61 947d 9428 8c04 7479  ..schema.}.(..ty
+00005b70: 7065 948c 0762 6f6f 6c65 616e 948c 0764  pe...boolean...d
+00005b80: 6566 6175 6c74 9489 7575 658c 0972 6573  efault..uue..res
+00005b90: 706f 6e73 6573 947d 9428 8c03 3230 3094  ponses.}.(..200.
+00005ba0: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00005bb0: 948c 3652 6573 756d 6269 7420 7265 7175  ..6Resumbit requ
+00005bc0: 6573 7420 666f 7220 7468 6520 6a6f 6220  est for the job 
+00005bd0: 6973 2072 6574 7269 6576 6564 2073 7563  is retrieved suc
+00005be0: 6573 7366 756c 6c79 2e94 8c07 636f 6e74  essfully....cont
+00005bf0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00005c00: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00005c10: 656d 6194 7d94 8c04 2472 6566 948c 2423  ema.}...$ref..$#
+00005c20: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00005c30: 6d61 732f 5265 7370 4765 7452 6573 7562  mas/RespGetResub
+00005c40: 6d69 7494 7373 7375 8c03 3430 3094 7d94  mit.sssu..400.}.
+00005c50: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+00005c60: 0c49 6e70 7574 2065 7272 6f72 2e94 8c07  .Input error....
+00005c70: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00005c80: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00005c90: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00005ca0: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
+00005cb0: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
+00005cc0: 6394 7373 7375 8c03 3430 3194 7d94 288c  c.sssu..401.}.(.
+00005cd0: 0b64 6573 6372 6970 7469 6f6e 948c 0f4e  .description...N
+00005ce0: 6f74 2061 7574 686f 7269 7a65 642e 948c  ot authorized...
+00005cf0: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00005d00: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00005d10: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00005d20: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00005d30: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
+00005d40: 6963 9473 7373 758c 0334 3033 947d 9428  ic.sssu..403.}.(
+00005d50: 8c0b 6465 7363 7269 7074 696f 6e94 8c0a  ..description...
+00005d60: 466f 7262 6964 6465 6e2e 948c 0763 6f6e  Forbidden....con
+00005d70: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+00005d80: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+00005d90: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
+00005da0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00005db0: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
+00005dc0: 7373 758c 0335 3030 947d 9428 8c0b 6465  ssu..500.}.(..de
+00005dd0: 7363 7269 7074 696f 6e94 8c0d 5365 7276  scription...Serv
+00005de0: 6572 2065 7272 6f72 2e94 8c07 636f 6e74  er error....cont
+00005df0: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00005e00: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00005e10: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
+00005e20: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00005e30: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
+00005e40: 7375 758c 0873 6563 7572 6974 7994 5d94  suu..security.].
+00005e50: 7d94 8c08 5461 7069 734a 5754 945d 9473  }...TapisJWT.].s
+00005e60: 6175 738c 182f 6a6f 6273 2f7b 6a6f 6255  aus../jobs/{jobU
+00005e70: 7569 647d 2f72 6573 7562 6d69 7494 7d94  uid}/resubmit.}.
+00005e80: 8c04 706f 7374 947d 9428 8c04 7461 6773  ..post.}.(..tags
+00005e90: 945d 948c 046a 6f62 7394 618c 0b64 6573  .]...jobs.a..des
+00005ea0: 6372 6970 7469 6f6e 9458 c602 0000 5265  cription.X....Re
+00005eb0: 7375 626d 6974 2061 206a 6f62 2066 6f72  submit a job for
+00005ec0: 2065 7865 6375 7469 6f6e 2075 7369 6e67   execution using
+00005ed0: 2074 6865 206a 6f62 2773 206f 7269 6769   the job's origi
+00005ee0: 6e61 6c20 7061 7261 6d65 7465 7273 2e20  nal parameters. 
+00005ef0: 2054 6865 206d 6169 6e20 7068 6173 6573   The main phases
+00005f00: 206f 6620 6a6f 6220 6578 6563 7574 696f   of job executio
+00005f10: 6e20 6172 653a 0a0a 2020 2d20 7661 6c69  n are:..  - vali
+00005f20: 6461 7465 2069 6e70 7574 0a20 202d 2063  date input.  - c
+00005f30: 6865 636b 2072 6573 6f75 7263 6520 6176  heck resource av
+00005f40: 6169 6c61 6269 6c69 7479 0a20 202d 2073  ailability.  - s
+00005f50: 7461 6765 2069 6e70 7574 2066 696c 6573  tage input files
+00005f60: 0a20 202d 2073 7461 6765 2061 7070 6c69  .  - stage appli
+00005f70: 6361 7469 6f6e 2063 6f64 650a 2020 2d20  cation code.  - 
+00005f80: 6c61 756e 6368 2061 7070 6c69 6361 7469  launch applicati
+00005f90: 6f6e 0a20 202d 206d 6f6e 6974 6f72 2061  on.  - monitor a
+00005fa0: 7070 6c69 6361 7469 6f6e 0a20 202d 2061  pplication.  - a
+00005fb0: 7263 6869 7665 2061 7070 6c69 6361 7469  rchive applicati
+00005fc0: 6f6e 206f 7574 7075 740a 0a57 6865 6e20  on output..When 
+00005fd0: 6120 6a6f 6220 6973 2073 7562 6d69 7474  a job is submitt
+00005fe0: 6564 2069 7473 2072 6571 7565 7374 2070  ed its request p
+00005ff0: 6179 6c6f 6164 2069 7320 6361 7074 7572  ayload is captur
+00006000: 6564 2061 6e64 2061 7661 696c 6162 6c65  ed and available
+00006010: 2066 6f72 2072 6573 7562 6d69 7373 696f   for resubmissio
+00006020: 6e20 7573 696e 6720 7468 6973 2041 5049  n using this API
+00006030: 2e20 5468 6520 7265 7375 626d 6974 7465  . The resubmitte
+00006040: 6420 6a6f 6220 6973 2061 7373 6967 6e65  d job is assigne
+00006050: 6420 6120 6e65 7720 5555 4944 2061 6e64  d a new UUID and
+00006060: 2064 6f65 7320 6e6f 7420 7265 6665 7265   does not refere
+00006070: 6e63 6520 6f72 2068 6176 6520 616e 7920  nce or have any 
+00006080: 7370 6563 6961 6c20 6163 6365 7373 2074  special access t
+00006090: 6f20 7468 6520 6f72 6967 696e 616c 206a  o the original j
+000060a0: 6f62 2773 2069 6e66 6f72 6d61 7469 6f6e  ob's information
+000060b0: 206f 6e63 6520 7468 6520 6f72 6769 6e61   once the orgina
+000060c0: 6c20 6a6f 6227 7320 7265 7175 6573 7420  l job's request 
+000060d0: 6973 2063 6f70 6965 642e 2054 6865 2072  is copied. The r
+000060e0: 6573 7562 6d69 7474 6564 206a 6f62 2773  esubmitted job's
+000060f0: 2065 7865 6375 7469 6f6e 2063 616e 2064   execution can d
+00006100: 6966 6665 7220 6672 6f6d 2074 6865 206f  iffer from the o
+00006110: 7269 6769 6e61 6c20 6a6f 6227 7320 6966  riginal job's if
+00006120: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
+00006130: 2c20 7379 7374 656d 206f 7220 6f74 6865  , system or othe
+00006140: 7220 6173 7065 6374 7320 6f66 2074 6865  r aspects of the
+00006150: 2065 7865 6375 7469 6f6e 2065 6e76 6972   execution envir
+00006160: 6f6e 6d65 6e74 2068 6176 6520 6368 616e  onment have chan
+00006170: 6765 642e 948c 0b6f 7065 7261 7469 6f6e  ged....operation
+00006180: 4964 948c 0b72 6573 7562 6d69 744a 6f62  Id...resubmitJob
+00006190: 948c 0a70 6172 616d 6574 6572 7394 5d94  ...parameters.].
+000061a0: 287d 9428 8c04 6e61 6d65 948c 076a 6f62  (}.(..name...job
+000061b0: 5575 6964 948c 0269 6e94 8c04 7061 7468  Uuid...in...path
+000061c0: 948c 0872 6571 7569 7265 6494 888c 0673  ...required....s
+000061d0: 6368 656d 6194 7d94 8c04 7479 7065 948c  chema.}...type..
+000061e0: 0673 7472 696e 6794 7375 7d94 288c 046e  .string.su}.(..n
+000061f0: 616d 6594 8c06 7072 6574 7479 948c 0269  ame...pretty...i
+00006200: 6e94 8c05 7175 6572 7994 8c06 7363 6865  n...query...sche
+00006210: 6d61 947d 9428 8c04 7479 7065 948c 0762  ma.}.(..type...b
+00006220: 6f6f 6c65 616e 948c 0764 6566 6175 6c74  oolean...default
+00006230: 9489 7575 658c 0972 6573 706f 6e73 6573  ..uue..responses
+00006240: 947d 9428 8c03 3230 3094 7d94 288c 0b64  .}.(..200.}.(..d
+00006250: 6573 6372 6970 7469 6f6e 948c 0c4a 6f62  escription...Job
+00006260: 2063 7265 6174 6564 2e94 8c07 636f 6e74   created....cont
+00006270: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00006280: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00006290: 656d 6194 7d94 8c04 2472 6566 948c 2223  ema.}...$ref.."#
+000062a0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+000062b0: 6d61 732f 5265 7370 5375 626d 6974 4a6f  mas/RespSubmitJo
+000062c0: 6294 7373 7375 8c03 3430 3094 7d94 288c  b.sssu..400.}.(.
+000062d0: 0b64 6573 6372 6970 7469 6f6e 948c 0c49  .description...I
+000062e0: 6e70 7574 2065 7272 6f72 2e94 8c07 636f  nput error....co
+000062f0: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00006300: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00006310: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00006320: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
+00006330: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
+00006340: 7373 7375 8c03 3430 3194 7d94 288c 0b64  sssu..401.}.(..d
+00006350: 6573 6372 6970 7469 6f6e 948c 0f4e 6f74  escription...Not
+00006360: 2061 7574 686f 7269 7a65 642e 948c 0763   authorized....c
+00006370: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
+00006380: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
+00006390: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
+000063a0: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
+000063b0: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
+000063c0: 9473 7373 758c 0334 3033 947d 9428 8c0b  .sssu..403.}.(..
+000063d0: 6465 7363 7269 7074 696f 6e94 8c0a 466f  description...Fo
+000063e0: 7262 6964 6465 6e2e 948c 0763 6f6e 7465  rbidden....conte
+000063f0: 6e74 947d 948c 1061 7070 6c69 6361 7469  nt.}...applicati
+00006400: 6f6e 2f6a 736f 6e94 7d94 8c06 7363 6865  on/json.}...sche
+00006410: 6d61 947d 948c 0424 7265 6694 8c1e 232f  ma.}...$ref...#/
+00006420: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00006430: 6173 2f52 6573 7042 6173 6963 9473 7373  as/RespBasic.sss
+00006440: 758c 0335 3030 947d 9428 8c0b 6465 7363  u..500.}.(..desc
+00006450: 7269 7074 696f 6e94 8c0d 5365 7276 6572  ription...Server
+00006460: 2065 7272 6f72 2e94 8c07 636f 6e74 656e   error....conten
+00006470: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00006480: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00006490: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
+000064a0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+000064b0: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
+000064c0: 758c 0873 6563 7572 6974 7994 5d94 7d94  u..security.].}.
+000064d0: 8c08 5461 7069 734a 5754 945d 9473 6175  ..TapisJWT.].sau
+000064e0: 738c 192f 6a6f 6273 2f7b 6a6f 6255 7569  s../jobs/{jobUui
+000064f0: 647d 2f73 656e 6445 7665 6e74 947d 948c  d}/sendEvent.}..
+00006500: 0470 6f73 7494 7d94 288c 0474 6167 7394  .post.}.(..tags.
+00006510: 5d94 8c04 6a6f 6273 9461 8c0b 6465 7363  ]...jobs.a..desc
+00006520: 7269 7074 696f 6e94 5831 0200 0053 656e  ription.X1...Sen
+00006530: 6420 6120 7573 6572 2065 7665 6e74 2074  d a user event t
+00006540: 6f20 616e 2061 6374 6976 6520 6a6f 622e  o an active job.
+00006550: 2054 6865 206a 6f62 206d 7573 7420 6265   The job must be
+00006560: 2069 6e20 7468 6520 7361 6d65 2074 656e   in the same ten
+00006570: 616e 7420 6173 2074 6865 2063 616c 6c65  ant as the calle
+00006580: 722c 2062 7574 206e 6f20 6f74 6865 7220  r, but no other 
+00006590: 6175 7468 6f72 697a 6174 696f 6e20 6973  authorization is
+000065a0: 206e 6565 6465 642e 2049 6620 7468 6520   needed. If the 
+000065b0: 6a6f 6220 6861 7320 7465 726d 696e 6174  job has terminat
+000065c0: 6564 2074 6865 2072 6571 7565 7374 2077  ed the request w
+000065d0: 696c 6c20 6265 2072 656a 6563 7465 642e  ill be rejected.
+000065e0: 2054 6865 2063 616c 6c65 7220 6d75 7374   The caller must
+000065f0: 2073 7065 6369 6679 2061 2070 6179 6c6f   specify a paylo
+00006600: 6164 206f 6620 6e6f 6e2d 656d 7074 7920  ad of non-empty 
+00006610: 7374 7269 6e67 2064 6174 6120 696e 2074  string data in t
+00006620: 6865 202a 6576 656e 7444 6174 612a 2066  he *eventData* f
+00006630: 6965 6c64 2e20 5468 6520 2a65 7665 6e74  ield. The *event
+00006640: 4465 7461 696c 2a20 6669 656c 6420 6361  Detail* field ca
+00006650: 6e20 6265 2073 6574 2074 6f20 6675 7274  n be set to furt
+00006660: 6865 7220 7175 616c 6966 7920 7468 6520  her qualify the 
+00006670: 7479 7065 206f 6620 7573 6572 2065 7665  type of user eve
+00006680: 6e74 2c20 7768 6963 6820 6973 2075 7365  nt, which is use
+00006690: 6675 6c20 7768 656e 2066 696c 7465 7269  ful when filteri
+000066a0: 6e67 2065 7665 6e74 732e 2049 6620 6e6f  ng events. If no
+000066b0: 7420 7072 6f76 6964 6564 2074 6865 202a  t provided the *
+000066c0: 6576 656e 7444 6574 6169 6c2a 2064 6566  eventDetail* def
+000066d0: 6175 6c74 7320 746f 2022 4445 4641 554c  aults to "DEFAUL
+000066e0: 5422 2e0a 0a53 7562 7363 7269 6265 7273  T"...Subscribers
+000066f0: 2074 6861 7420 7265 6769 7374 6572 2069   that register i
+00006700: 6e74 6572 6573 7420 696e 2065 7665 6e74  nterest in event
+00006710: 7320 6f66 2074 7970 6520 4a4f 425f 5553  s of type JOB_US
+00006720: 4552 5f45 5645 4e54 2077 696c 6c20 7265  ER_EVENT will re
+00006730: 6365 6976 6520 6120 6e6f 7469 6669 6361  ceive a notifica
+00006740: 7469 6f6e 2061 7320 6120 7265 7375 6c74  tion as a result
+00006750: 206f 6620 7468 6973 2063 616c 6c2e 948c   of this call...
+00006760: 0b6f 7065 7261 7469 6f6e 4964 948c 0973  .operationId...s
+00006770: 656e 6445 7665 6e74 948c 0a70 6172 616d  endEvent...param
+00006780: 6574 6572 7394 5d94 287d 9428 8c04 6e61  eters.].(}.(..na
+00006790: 6d65 948c 076a 6f62 5575 6964 948c 0269  me...jobUuid...i
+000067a0: 6e94 8c04 7061 7468 948c 0872 6571 7569  n...path...requi
+000067b0: 7265 6494 888c 0673 6368 656d 6194 7d94  red....schema.}.
+000067c0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+000067d0: 7375 7d94 288c 046e 616d 6594 8c06 7072  su}.(..name...pr
+000067e0: 6574 7479 948c 0269 6e94 8c05 7175 6572  etty...in...quer
+000067f0: 7994 8c06 7363 6865 6d61 947d 9428 8c04  y...schema.}.(..
+00006800: 7479 7065 948c 0762 6f6f 6c65 616e 948c  type...boolean..
+00006810: 0764 6566 6175 6c74 9489 7575 658c 0b72  .default..uue..r
+00006820: 6571 7565 7374 426f 6479 947d 9428 8c07  equestBody.}.(..
+00006830: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00006840: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00006850: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00006860: 948c 2123 2f63 6f6d 706f 6e65 6e74 732f  ..!#/components/
+00006870: 7363 6865 6d61 732f 5265 7155 7365 7245  schemas/ReqUserE
+00006880: 7665 6e74 9473 7373 8c08 7265 7175 6972  vent.sss..requir
+00006890: 6564 9488 758c 0972 6573 706f 6e73 6573  ed..u..responses
+000068a0: 947d 9428 8c03 3230 3094 7d94 288c 0b64  .}.(..200.}.(..d
+000068b0: 6573 6372 6970 7469 6f6e 948c 0e45 7665  escription...Eve
+000068c0: 6e74 2063 7265 6174 6564 2e94 8c07 636f  nt created....co
+000068d0: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+000068e0: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+000068f0: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00006900: 1e23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
+00006910: 6865 6d61 732f 5265 7370 4261 7369 6394  hemas/RespBasic.
+00006920: 7373 7375 8c03 3430 3094 7d94 288c 0b64  sssu..400.}.(..d
+00006930: 6573 6372 6970 7469 6f6e 948c 0c49 6e70  escription...Inp
+00006940: 7574 2065 7272 6f72 2e94 8c07 636f 6e74  ut error....cont
+00006950: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00006960: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00006970: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
+00006980: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00006990: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
+000069a0: 7375 8c03 3430 3194 7d94 288c 0b64 6573  su..401.}.(..des
+000069b0: 6372 6970 7469 6f6e 948c 0f4e 6f74 2061  cription...Not a
+000069c0: 7574 686f 7269 7a65 642e 948c 0763 6f6e  uthorized....con
+000069d0: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+000069e0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+000069f0: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
+00006a00: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00006a10: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
+00006a20: 7373 758c 0334 3033 947d 9428 8c0b 6465  ssu..403.}.(..de
+00006a30: 7363 7269 7074 696f 6e94 8c0a 466f 7262  scription...Forb
+00006a40: 6964 6465 6e2e 948c 0763 6f6e 7465 6e74  idden....content
+00006a50: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+00006a60: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00006a70: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+00006a80: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00006a90: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
+00006aa0: 0335 3030 947d 9428 8c0b 6465 7363 7269  .500.}.(..descri
+00006ab0: 7074 696f 6e94 8c0d 5365 7276 6572 2065  ption...Server e
+00006ac0: 7272 6f72 2e94 8c07 636f 6e74 656e 7494  rror....content.
+00006ad0: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+00006ae0: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+00006af0: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
+00006b00: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+00006b10: 5265 7370 4261 7369 6394 7373 7375 758c  RespBasic.sssuu.
+00006b20: 0873 6563 7572 6974 7994 5d94 7d94 8c08  .security.].}...
+00006b30: 5461 7069 734a 5754 945d 9473 6175 738c  TapisJWT.].saus.
+00006b40: 0c2f 6a6f 6273 2f73 7562 6d69 7494 7d94  ./jobs/submit.}.
+00006b50: 8c04 706f 7374 947d 9428 8c04 7461 6773  ..post.}.(..tags
+00006b60: 945d 948c 046a 6f62 7394 618c 0b64 6573  .]...jobs.a..des
+00006b70: 6372 6970 7469 6f6e 9458 ac03 0000 5375  cription.X....Su
+00006b80: 626d 6974 2061 206a 6f62 2066 6f72 2065  bmit a job for e
+00006b90: 7865 6375 7469 6f6e 2e20 2054 6865 206d  xecution.  The m
+00006ba0: 6169 6e20 7068 6173 6573 206f 6620 6a6f  ain phases of jo
+00006bb0: 6220 6578 6563 7574 696f 6e20 6172 653a  b execution are:
+00006bc0: 0a0a 2020 2d20 7661 6c69 6461 7465 2069  ..  - validate i
+00006bd0: 6e70 7574 0a20 202d 2063 6865 636b 2072  nput.  - check r
+00006be0: 6573 6f75 7263 6520 6176 6169 6c61 6269  esource availabi
+00006bf0: 6c69 7479 0a20 202d 2073 7461 6765 2069  lity.  - stage i
+00006c00: 6e70 7574 2066 696c 6573 0a20 202d 2073  nput files.  - s
+00006c10: 7461 6765 2061 7070 6c69 6361 7469 6f6e  tage application
+00006c20: 2063 6f64 650a 2020 2d20 6c61 756e 6368   code.  - launch
+00006c30: 2061 7070 6c69 6361 7469 6f6e 0a20 202d   application.  -
+00006c40: 206d 6f6e 6974 6f72 2061 7070 6c69 6361   monitor applica
+00006c50: 7469 6f6e 0a20 202d 2061 7263 6869 7665  tion.  - archive
+00006c60: 2061 7070 6c69 6361 7469 6f6e 206f 7574   application out
+00006c70: 7075 740a 0a41 7420 6120 6d69 6e69 6d75  put..At a minimu
+00006c80: 6d2c 2074 6865 206a 6f62 206e 616d 652c  m, the job name,
+00006c90: 2061 7070 6c69 6361 7469 6f6e 2049 4420   application ID 
+00006ca0: 616e 6420 6170 706c 6963 6174 696f 6e20  and application 
+00006cb0: 7665 7273 696f 6e20 6d75 7374 2062 6520  version must be 
+00006cc0: 7370 6563 6966 6965 6420 696e 2074 6865  specified in the
+00006cd0: 2072 6571 7565 7374 2070 6179 6c6f 6164   request payload
+00006ce0: 2e20 5468 6520 6f70 7469 6f6e 616c 2070  . The optional p
+00006cf0: 6172 616d 6574 6572 7320 6176 6169 6c61  arameters availa
+00006d00: 626c 6520 696e 2061 206a 6f62 2072 6571  ble in a job req
+00006d10: 7565 7374 2070 726f 7669 6465 2067 7265  uest provide gre
+00006d20: 6174 2066 6c65 7869 6269 6c69 7479 2062  at flexibility b
+00006d30: 7574 206d 7573 7420 6265 2063 6f6e 7369  ut must be consi
+00006d40: 6465 7265 6420 696e 2074 6865 2063 6f6e  dered in the con
+00006d50: 7465 7874 206f 6620 7468 6520 6170 706c  text of the appl
+00006d60: 6963 6174 696f 6e20 616e 6420 7379 7374  ication and syst
+00006d70: 656d 2064 6566 696e 6974 696f 6e73 2e20  em definitions. 
+00006d80: 5468 6520 6163 7475 616c 2076 616c 7565  The actual value
+00006d90: 7320 7573 6564 2064 7572 696e 6720 6a6f  s used during jo
+00006da0: 6220 6578 6563 7574 696f 6e20 6172 6520  b execution are 
+00006db0: 6120 636f 6d62 696e 6174 696f 6e20 6f66  a combination of
+00006dc0: 2074 6865 2076 616c 7565 7320 696e 2074   the values in t
+00006dd0: 6869 7320 7265 7175 6573 7420 616e 6420  his request and 
+00006de0: 7468 6f73 6520 7370 6563 6966 6965 6420  those specified 
+00006df0: 696e 2074 6865 206a 6f62 2773 2061 7070  in the job's app
+00006e00: 6c69 6361 7469 6f6e 2061 6e64 2073 7973  lication and sys
+00006e10: 7465 6d20 6465 6669 6e69 7469 6f6e 732e  tem definitions.
+00006e20: 2049 7427 7320 6f66 7465 6e20 6465 7369   It's often desi
+00006e30: 7261 626c 6520 746f 206b 6565 7020 7468  rable to keep th
+00006e40: 6520 7375 626d 6973 7369 6f6e 2072 6571  e submission req
+00006e50: 7565 7374 2073 696d 706c 6520 6279 2073  uest simple by s
+00006e60: 7065 6369 6679 696e 6720 636f 6d6d 6f6e  pecifying common
+00006e70: 2076 616c 7565 7320 696e 2074 6865 7365   values in these
+00006e80: 206f 7468 6572 2074 776f 2064 6566 696e   other two defin
+00006e90: 6974 696f 6e73 2e20 5365 6520 7468 6520  itions. See the 
+00006ea0: 5b4a 6f62 2053 7562 6d69 7373 696f 6e20  [Job Submission 
+00006eb0: 5265 7175 6573 745d 2868 7474 7073 3a2f  Request](https:/
+00006ec0: 2f74 6170 6973 2e72 6561 6474 6865 646f  /tapis.readthedo
+00006ed0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00006ee0: 7465 6368 6e69 6361 6c2f 6a6f 6273 2e68  technical/jobs.h
+00006ef0: 746d 6c23 7468 652d 6a6f 622d 7375 626d  tml#the-job-subm
+00006f00: 6973 7369 6f6e 2d72 6571 7565 7374 2920  ission-request) 
+00006f10: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
+00006f20: 7220 6465 7461 696c 732e 948c 0b6f 7065  r details....ope
+00006f30: 7261 7469 6f6e 4964 948c 0973 7562 6d69  rationId...submi
+00006f40: 744a 6f62 948c 0a70 6172 616d 6574 6572  tJob...parameter
+00006f50: 7394 5d94 7d94 288c 046e 616d 6594 8c06  s.].}.(..name...
+00006f60: 7072 6574 7479 948c 0269 6e94 8c05 7175  pretty...in...qu
+00006f70: 6572 7994 8c06 7363 6865 6d61 947d 9428  ery...schema.}.(
+00006f80: 8c04 7479 7065 948c 0762 6f6f 6c65 616e  ..type...boolean
+00006f90: 948c 0764 6566 6175 6c74 9489 7575 618c  ...default..uua.
+00006fa0: 0b72 6571 7565 7374 426f 6479 947d 9428  .requestBody.}.(
+00006fb0: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00006fc0: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00006fd0: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00006fe0: 6566 948c 2123 2f63 6f6d 706f 6e65 6e74  ef..!#/component
+00006ff0: 732f 7363 6865 6d61 732f 5265 7153 7562  s/schemas/ReqSub
+00007000: 6d69 744a 6f62 9473 7373 8c08 7265 7175  mitJob.sss..requ
+00007010: 6972 6564 9488 758c 0972 6573 706f 6e73  ired..u..respons
+00007020: 6573 947d 9428 8c03 3230 3094 7d94 288c  es.}.(..200.}.(.
+00007030: 0b64 6573 6372 6970 7469 6f6e 948c 0c4a  .description...J
+00007040: 6f62 2063 7265 6174 6564 2e94 8c07 636f  ob created....co
+00007050: 6e74 656e 7494 7d94 8c10 6170 706c 6963  ntent.}...applic
+00007060: 6174 696f 6e2f 6a73 6f6e 947d 948c 0673  ation/json.}...s
+00007070: 6368 656d 6194 7d94 8c04 2472 6566 948c  chema.}...$ref..
+00007080: 2223 2f63 6f6d 706f 6e65 6e74 732f 7363  "#/components/sc
+00007090: 6865 6d61 732f 5265 7370 5375 626d 6974  hemas/RespSubmit
+000070a0: 4a6f 6294 7373 7375 8c03 3430 3094 7d94  Job.sssu..400.}.
+000070b0: 288c 0b64 6573 6372 6970 7469 6f6e 948c  (..description..
+000070c0: 0c49 6e70 7574 2065 7272 6f72 2e94 8c07  .Input error....
+000070d0: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+000070e0: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+000070f0: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00007100: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
+00007110: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
+00007120: 6394 7373 7375 8c03 3430 3194 7d94 288c  c.sssu..401.}.(.
+00007130: 0b64 6573 6372 6970 7469 6f6e 948c 0f4e  .description...N
+00007140: 6f74 2061 7574 686f 7269 7a65 642e 948c  ot authorized...
+00007150: 0763 6f6e 7465 6e74 947d 948c 1061 7070  .content.}...app
+00007160: 6c69 6361 7469 6f6e 2f6a 736f 6e94 7d94  lication/json.}.
+00007170: 8c06 7363 6865 6d61 947d 948c 0424 7265  ..schema.}...$re
+00007180: 6694 8c1e 232f 636f 6d70 6f6e 656e 7473  f...#/components
+00007190: 2f73 6368 656d 6173 2f52 6573 7042 6173  /schemas/RespBas
+000071a0: 6963 9473 7373 758c 0334 3033 947d 9428  ic.sssu..403.}.(
+000071b0: 8c0b 6465 7363 7269 7074 696f 6e94 8c0a  ..description...
+000071c0: 466f 7262 6964 6465 6e2e 948c 0763 6f6e  Forbidden....con
+000071d0: 7465 6e74 947d 948c 1061 7070 6c69 6361  tent.}...applica
+000071e0: 7469 6f6e 2f6a 736f 6e94 7d94 8c06 7363  tion/json.}...sc
+000071f0: 6865 6d61 947d 948c 0424 7265 6694 8c1e  hema.}...$ref...
+00007200: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00007210: 656d 6173 2f52 6573 7042 6173 6963 9473  emas/RespBasic.s
+00007220: 7373 758c 0335 3030 947d 9428 8c0b 6465  ssu..500.}.(..de
+00007230: 7363 7269 7074 696f 6e94 8c0d 5365 7276  scription...Serv
+00007240: 6572 2065 7272 6f72 2e94 8c07 636f 6e74  er error....cont
+00007250: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00007260: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00007270: 656d 6194 7d94 8c04 2472 6566 948c 1e23  ema.}...$ref...#
+00007280: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00007290: 6d61 732f 5265 7370 4261 7369 6394 7373  mas/RespBasic.ss
+000072a0: 7375 758c 0873 6563 7572 6974 7994 5d94  suu..security.].
+000072b0: 7d94 8c08 5461 7069 734a 5754 945d 9473  }...TapisJWT.].s
+000072c0: 6175 738c 162f 6a6f 6273 2f73 7562 7363  aus../jobs/subsc
+000072d0: 7269 6265 2f7b 7575 6964 7d94 7d94 8c06  ribe/{uuid}.}...
+000072e0: 6465 6c65 7465 947d 9428 8c04 7461 6773  delete.}.(..tags
+000072f0: 945d 948c 0d73 7562 7363 7269 7074 696f  .]...subscriptio
+00007300: 6e73 9461 8c0b 6465 7363 7269 7074 696f  ns.a..descriptio
+00007310: 6e94 58fe 0100 0044 6570 656e 6469 6e67  n.X....Depending
+00007320: 206f 6e20 7468 6520 5555 4944 2070 726f   on the UUID pro
+00007330: 7669 6465 2c20 7468 6973 2041 5049 2065  vide, this API e
+00007340: 6974 6865 7220 6465 6c65 7465 7320 6120  ither deletes a 
+00007350: 7369 6e67 6c65 2073 7562 7363 7269 7074  single subscript
+00007360: 696f 6e20 6672 6f6d 2061 206a 6f62 206f  ion from a job o
+00007370: 7220 616c 6c20 7375 6273 6372 6970 7469  r all subscripti
+00007380: 6f6e 7320 6672 6f6d 2061 206a 6f62 2e20  ons from a job. 
+00007390: 546f 2064 656c 6574 6520 7369 6e67 6c65  To delete single
+000073a0: 2073 7562 7363 7269 7074 696f 6e2c 2070   subscription, p
+000073b0: 726f 7669 6465 2074 6865 2055 5549 4420  rovide the UUID 
+000073c0: 6f66 2074 6861 7420 7375 6273 6372 6970  of that subscrip
+000073d0: 7469 6f6e 2061 7320 6c69 7374 6564 2069  tion as listed i
+000073e0: 6e20 7468 6520 7375 6273 6372 6970 7469  n the subscripti
+000073f0: 6f6e 2072 6574 7269 6576 616c 2072 6573  on retrieval res
+00007400: 756c 7420 666f 7220 7468 6520 6a6f 622e  ult for the job.
+00007410: 2020 546f 2064 656c 6574 6520 616c 6c20    To delete all 
+00007420: 6120 6a6f 6227 7320 7375 6273 6372 6970  a job's subscrip
+00007430: 7469 6f6e 732c 2073 7065 6369 6679 2074  tions, specify t
+00007440: 6865 206a 6f62 2055 5549 442e 0a0a 4c69  he job UUID...Li
+00007450: 6b65 2061 6c6c 204a 6f62 2073 7562 7363  ke all Job subsc
+00007460: 7269 7074 696f 6e20 4150 4973 2c20 6d6f  ription APIs, mo
+00007470: 6469 6669 6361 7469 6f6e 7320 6f6e 6c79  difications only
+00007480: 2061 6666 6563 7420 7275 6e6e 696e 6720   affect running 
+00007490: 6a6f 6273 2061 6e64 206e 6576 6572 2063  jobs and never c
+000074a0: 6861 6e67 6520 7468 6520 7361 7665 6420  hange the saved 
+000074b0: 6a6f 6220 6465 6669 6e69 7469 6f6e 2e20  job definition. 
+000074c0: 4173 2061 2063 6f6e 7365 7175 656e 6365  As a consequence
+000074d0: 2c20 6a6f 6220 7265 7375 626d 6973 7369  , job resubmissi
+000074e0: 6f6e 7320 6172 6520 6e6f 7420 6166 6665  ons are not affe
+000074f0: 6374 6564 2062 7920 7275 6e74 696d 6520  cted by runtime 
+00007500: 7375 6273 6372 6970 7469 6f6e 2063 6861  subscription cha
+00007510: 6e67 6573 2e94 8c0b 6f70 6572 6174 696f  nges....operatio
+00007520: 6e49 6494 8c13 6465 6c65 7465 5375 6273  nId...deleteSubs
+00007530: 6372 6970 7469 6f6e 7394 8c0a 7061 7261  criptions...para
+00007540: 6d65 7465 7273 945d 9428 7d94 288c 046e  meters.].(}.(..n
+00007550: 616d 6594 8c04 7575 6964 948c 0269 6e94  ame...uuid...in.
+00007560: 8c04 7061 7468 948c 0872 6571 7569 7265  ..path...require
+00007570: 6494 888c 0673 6368 656d 6194 7d94 8c04  d....schema.}...
+00007580: 7479 7065 948c 0673 7472 696e 6794 7375  type...string.su
+00007590: 7d94 288c 046e 616d 6594 8c06 7072 6574  }.(..name...pret
+000075a0: 7479 948c 0269 6e94 8c05 7175 6572 7994  ty...in...query.
+000075b0: 8c06 7363 6865 6d61 947d 9428 8c04 7479  ..schema.}.(..ty
+000075c0: 7065 948c 0762 6f6f 6c65 616e 948c 0764  pe...boolean...d
+000075d0: 6566 6175 6c74 9489 7575 658c 0972 6573  efault..uue..res
+000075e0: 706f 6e73 6573 947d 9428 8c03 3230 3094  ponses.}.(..200.
+000075f0: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00007600: 948c 0c4a 6f62 2063 7265 6174 6564 2e94  ...Job created..
+00007610: 8c07 636f 6e74 656e 7494 7d94 8c10 6170  ..content.}...ap
+00007620: 706c 6963 6174 696f 6e2f 6a73 6f6e 947d  plication/json.}
+00007630: 948c 0673 6368 656d 6194 7d94 8c04 2472  ...schema.}...$r
+00007640: 6566 948c 2623 2f63 6f6d 706f 6e65 6e74  ef..&#/component
+00007650: 732f 7363 6865 6d61 732f 5265 7375 6c74  s/schemas/Result
+00007660: 4368 616e 6765 436f 756e 7494 7373 7375  ChangeCount.sssu
+00007670: 8c03 3430 3094 7d94 288c 0b64 6573 6372  ..400.}.(..descr
+00007680: 6970 7469 6f6e 948c 0c49 6e70 7574 2065  iption...Input e
+00007690: 7272 6f72 2e94 8c07 636f 6e74 656e 7494  rror....content.
+000076a0: 7d94 8c10 6170 706c 6963 6174 696f 6e2f  }...application/
+000076b0: 6a73 6f6e 947d 948c 0673 6368 656d 6194  json.}...schema.
+000076c0: 7d94 8c04 2472 6566 948c 1e23 2f63 6f6d  }...$ref...#/com
+000076d0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+000076e0: 5265 7370 4261 7369 6394 7373 7375 8c03  RespBasic.sssu..
+000076f0: 3430 3194 7d94 288c 0b64 6573 6372 6970  401.}.(..descrip
+00007700: 7469 6f6e 948c 0f4e 6f74 2061 7574 686f  tion...Not autho
+00007710: 7269 7a65 642e 948c 0763 6f6e 7465 6e74  rized....content
+00007720: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+00007730: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+00007740: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+00007750: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00007760: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
+00007770: 0334 3033 947d 9428 8c0b 6465 7363 7269  .403.}.(..descri
+00007780: 7074 696f 6e94 8c0a 466f 7262 6964 6465  ption...Forbidde
+00007790: 6e2e 948c 0763 6f6e 7465 6e74 947d 948c  n....content.}..
+000077a0: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+000077b0: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+000077c0: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
+000077d0: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+000077e0: 7042 6173 6963 9473 7373 758c 0335 3030  pBasic.sssu..500
+000077f0: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
+00007800: 6e94 8c0d 5365 7276 6572 2065 7272 6f72  n...Server error
+00007810: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
+00007820: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00007830: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00007840: 2472 6566 948c 1e23 2f63 6f6d 706f 6e65  $ref...#/compone
+00007850: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
+00007860: 4261 7369 6394 7373 7375 758c 0873 6563  Basic.sssuu..sec
+00007870: 7572 6974 7994 5d94 7d94 8c08 5461 7069  urity.].}...Tapi
+00007880: 734a 5754 945d 9473 6175 738c 192f 6a6f  sJWT.].saus../jo
+00007890: 6273 2f73 7562 7363 7269 6265 2f7b 6a6f  bs/subscribe/{jo
+000078a0: 6255 7569 647d 947d 9428 8c03 6765 7494  bUuid}.}.(..get.
+000078b0: 7d94 288c 0474 6167 7394 5d94 8c0d 7375  }.(..tags.]...su
+000078c0: 6273 6372 6970 7469 6f6e 7394 618c 0b64  bscriptions.a..d
+000078d0: 6573 6372 6970 7469 6f6e 9458 0801 0000  escription.X....
+000078e0: 5265 7472 6965 7665 2061 206a 6f62 2773  Retrieve a job's
+000078f0: 2073 7562 7363 7269 7074 696f 6e73 2066   subscriptions f
+00007900: 6f6d 2074 6865 204e 6f74 6966 6963 6174  om the Notificat
+00007910: 696f 6e73 2073 6572 7669 6365 2e20 4166  ions service. Af
+00007920: 7465 7220 7375 6273 6372 6970 7469 6f6e  ter subscription
+00007930: 7320 6578 7069 7265 206f 7220 6172 6520  s expire or are 
+00007940: 6465 6c65 7465 6420 6279 2075 7365 7220  deleted by user 
+00007950: 6163 7469 6f6e 2074 6865 7920 6d61 7920  action they may 
+00007960: 6e6f 206c 6f6e 6765 7220 6265 206c 6973  no longer be lis
+00007970: 7465 6420 696e 204e 6f74 6966 6963 6174  ted in Notificat
+00007980: 696f 6e20 7365 7276 6963 652e 2054 6f20  ion service. To 
+00007990: 696e 7370 6563 7420 7468 6520 696e 6974  inspect the init
+000079a0: 6961 6c20 7365 7420 6f66 2073 7562 7363  ial set of subsc
+000079b0: 7269 7074 696f 6e73 2061 7373 6967 6e65  riptions assigne
+000079c0: 6420 746f 2061 206a 6f62 2c20 7265 7472  d to a job, retr
+000079d0: 6965 7665 2074 6865 206a 6f62 2064 6566  ieve the job def
+000079e0: 696e 6974 696f 6e2e 948c 0b6f 7065 7261  inition....opera
+000079f0: 7469 6f6e 4964 948c 1067 6574 5375 6273  tionId...getSubs
+00007a00: 6372 6970 7469 6f6e 7394 8c0a 7061 7261  criptions...para
+00007a10: 6d65 7465 7273 945d 9428 7d94 288c 046e  meters.].(}.(..n
+00007a20: 616d 6594 8c07 6a6f 6255 7569 6494 8c02  ame...jobUuid...
+00007a30: 696e 948c 0470 6174 6894 8c08 7265 7175  in...path...requ
+00007a40: 6972 6564 9488 8c06 7363 6865 6d61 947d  ired....schema.}
+00007a50: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+00007a60: 9473 757d 9428 8c04 6e61 6d65 948c 056c  .su}.(..name...l
+00007a70: 696d 6974 948c 0269 6e94 8c05 7175 6572  imit...in...quer
+00007a80: 7994 8c06 7363 6865 6d61 947d 9428 8c04  y...schema.}.(..
+00007a90: 7479 7065 948c 0769 6e74 6567 6572 948c  type...integer..
+00007aa0: 0666 6f72 6d61 7494 8c05 696e 7433 3294  .format...int32.
+00007ab0: 8c07 6465 6661 756c 7494 4b64 7575 7d94  ..default.Kduu}.
+00007ac0: 288c 046e 616d 6594 8c04 736b 6970 948c  (..name...skip..
+00007ad0: 0269 6e94 8c05 7175 6572 7994 8c06 7363  .in...query...sc
+00007ae0: 6865 6d61 947d 9428 8c04 7479 7065 948c  hema.}.(..type..
+00007af0: 0769 6e74 6567 6572 948c 0666 6f72 6d61  .integer...forma
+00007b00: 7494 8c05 696e 7433 3294 8c07 6465 6661  t...int32...defa
+00007b10: 756c 7494 4b00 7575 7d94 288c 046e 616d  ult.K.uu}.(..nam
+00007b20: 6594 8c06 7072 6574 7479 948c 0269 6e94  e...pretty...in.
+00007b30: 8c05 7175 6572 7994 8c06 7363 6865 6d61  ..query...schema
+00007b40: 947d 9428 8c04 7479 7065 948c 0762 6f6f  .}.(..type...boo
+00007b50: 6c65 616e 948c 0764 6566 6175 6c74 9489  lean...default..
+00007b60: 7575 658c 0972 6573 706f 6e73 6573 947d  uue..responses.}
+00007b70: 9428 8c03 3230 3094 7d94 288c 0b64 6573  .(..200.}.(..des
+00007b80: 6372 6970 7469 6f6e 948c 0c4a 6f62 2063  cription...Job c
+00007b90: 7265 6174 6564 2e94 8c07 636f 6e74 656e  reated....conten
+00007ba0: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00007bb0: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00007bc0: 6194 7d94 8c04 2472 6566 948c 2923 2f63  a.}...$ref..)#/c
+00007bd0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00007be0: 732f 5265 7370 4765 7453 7562 7363 7269  s/RespGetSubscri
+00007bf0: 7074 696f 6e73 9473 7373 758c 0334 3030  ptions.sssu..400
+00007c00: 947d 9428 8c0b 6465 7363 7269 7074 696f  .}.(..descriptio
+00007c10: 6e94 8c0c 496e 7075 7420 6572 726f 722e  n...Input error.
+00007c20: 948c 0763 6f6e 7465 6e74 947d 948c 1061  ...content.}...a
+00007c30: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e94  pplication/json.
+00007c40: 7d94 8c06 7363 6865 6d61 947d 948c 0424  }...schema.}...$
+00007c50: 7265 6694 8c1e 232f 636f 6d70 6f6e 656e  ref...#/componen
+00007c60: 7473 2f73 6368 656d 6173 2f52 6573 7042  ts/schemas/RespB
+00007c70: 6173 6963 9473 7373 758c 0334 3031 947d  asic.sssu..401.}
+00007c80: 9428 8c0b 6465 7363 7269 7074 696f 6e94  .(..description.
+00007c90: 8c0f 4e6f 7420 6175 7468 6f72 697a 6564  ..Not authorized
+00007ca0: 2e94 8c07 636f 6e74 656e 7494 7d94 8c10  ....content.}...
+00007cb0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00007cc0: 947d 948c 0673 6368 656d 6194 7d94 8c04  .}...schema.}...
+00007cd0: 2472 6566 948c 1e23 2f63 6f6d 706f 6e65  $ref...#/compone
+00007ce0: 6e74 732f 7363 6865 6d61 732f 5265 7370  nts/schemas/Resp
+00007cf0: 4261 7369 6394 7373 7375 8c03 3430 3394  Basic.sssu..403.
+00007d00: 7d94 288c 0b64 6573 6372 6970 7469 6f6e  }.(..description
+00007d10: 948c 0a46 6f72 6269 6464 656e 2e94 8c07  ...Forbidden....
+00007d20: 636f 6e74 656e 7494 7d94 8c10 6170 706c  content.}...appl
+00007d30: 6963 6174 696f 6e2f 6a73 6f6e 947d 948c  ication/json.}..
+00007d40: 0673 6368 656d 6194 7d94 8c04 2472 6566  .schema.}...$ref
+00007d50: 948c 1e23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
+00007d60: 7363 6865 6d61 732f 5265 7370 4261 7369  schemas/RespBasi
+00007d70: 6394 7373 7375 8c03 3530 3094 7d94 288c  c.sssu..500.}.(.
+00007d80: 0b64 6573 6372 6970 7469 6f6e 948c 0d53  .description...S
+00007d90: 6572 7665 7220 6572 726f 722e 948c 0763  erver error....c
+00007da0: 6f6e 7465 6e74 947d 948c 1061 7070 6c69  ontent.}...appli
+00007db0: 6361 7469 6f6e 2f6a 736f 6e94 7d94 8c06  cation/json.}...
+00007dc0: 7363 6865 6d61 947d 948c 0424 7265 6694  schema.}...$ref.
+00007dd0: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
+00007de0: 6368 656d 6173 2f52 6573 7042 6173 6963  chemas/RespBasic
+00007df0: 9473 7373 7575 8c08 7365 6375 7269 7479  .sssuu..security
+00007e00: 945d 947d 948c 0854 6170 6973 4a57 5494  .].}...TapisJWT.
+00007e10: 5d94 7361 758c 0470 6f73 7494 7d94 288c  ].sau..post.}.(.
+00007e20: 0474 6167 7394 5d94 8c0d 7375 6273 6372  .tags.]...subscr
+00007e30: 6970 7469 6f6e 7394 618c 0b64 6573 6372  iptions.a..descr
+00007e40: 6970 7469 6f6e 9458 4e03 0000 5375 6263  iption.XN...Subc
+00007e50: 7269 6265 2074 6f20 6120 7275 6e6e 696e  ribe to a runnin
+00007e60: 6720 6a6f 6220 6964 656e 7469 6669 6564  g job identified
+00007e70: 2062 7920 6974 2773 2055 5549 442e 2054   by it's UUID. T
+00007e80: 6865 2063 616c 6c65 7220 6d75 7374 2062  he caller must b
+00007e90: 6520 7468 6520 6a6f 6220 6f77 6e65 7220  e the job owner 
+00007ea0: 6f72 2061 2074 656e 616e 7420 6164 6d69  or a tenant admi
+00007eb0: 6e69 7374 7261 746f 722e 0a0a 4c69 6b65  nistrator...Like
+00007ec0: 2061 6c6c 204a 6f62 2073 7562 7363 7269   all Job subscri
+00007ed0: 7074 696f 6e20 4150 4973 2c20 6d6f 6469  ption APIs, modi
+00007ee0: 6669 6361 7469 6f6e 7320 6f6e 6c79 2061  fications only a
+00007ef0: 6666 6563 7420 7275 6e6e 696e 6720 6a6f  ffect running jo
+00007f00: 6273 2061 6e64 206e 6576 6572 2063 6861  bs and never cha
+00007f10: 6e67 6520 7468 6520 7361 7665 6420 6a6f  nge the saved jo
+00007f20: 6220 6465 6669 6e69 7469 6f6e 2e20 4173  b definition. As
+00007f30: 2061 2063 6f6e 7365 7175 656e 6365 2c20   a consequence, 
+00007f40: 6a6f 6220 7265 7375 626d 6973 7369 6f6e  job resubmission
+00007f50: 7320 6172 6520 6e6f 7420 6166 6665 6374  s are not affect
+00007f60: 6564 2062 7920 7275 6e74 696d 6520 7375  ed by runtime su
+00007f70: 6273 6372 6970 7469 6f6e 2063 6861 6e67  bscription chang
+00007f80: 6573 2e0a 0a54 6865 2065 7665 6e74 7320  es...The events 
+00007f90: 746f 2077 6869 6368 206f 6e65 2063 616e  to which one can
+00007fa0: 2073 7562 7363 7269 6265 2061 7265 3a0a   subscribe are:.
+00007fb0: 0a2d 204a 4f42 5f4e 4557 5f53 5441 5455  .- JOB_NEW_STATU
+00007fc0: 5320 2d20 7468 6520 6a6f 6220 6861 7320  S - the job has 
+00007fd0: 7472 616e 7369 7469 6f6e 6564 2074 6f20  transitioned to 
+00007fe0: 6120 6e65 7720 7374 6174 7573 0a2d 204a  a new status.- J
+00007ff0: 4f42 5f49 4e50 5554 5f54 5241 4e53 4143  OB_INPUT_TRANSAC
+00008000: 5449 4f4e 5f49 4420 2d20 6120 7265 7175  TION_ID - a requ
+00008010: 6573 7420 746f 2073 7461 6765 206a 6f62  est to stage job
+00008020: 2069 6e70 7574 2066 696c 6573 2068 6173   input files has
+00008030: 2062 6565 6e20 7375 626d 6974 7465 640a   been submitted.
+00008040: 2d20 4a4f 425f 4152 4348 4956 455f 5452  - JOB_ARCHIVE_TR
+00008050: 414e 5341 4354 494f 4e5f 4944 202d 2061  ANSACTION_ID - a
+00008060: 2072 6571 7565 7374 2074 6f20 6172 6368   request to arch
+00008070: 6976 6520 6a6f 6220 6f75 7470 7574 2066  ive job output f
+00008080: 696c 6573 2068 6173 2062 6565 6e20 7375  iles has been su
+00008090: 626d 6974 7465 640a 2d20 4a4f 425f 5355  bmitted.- JOB_SU
+000080a0: 4253 4352 4950 5449 4f4e 202d 2061 2063  BSCRIPTION - a c
+000080b0: 6861 6e67 6520 746f 2074 6865 206a 6f62  hange to the job
+000080c0: 2773 2073 7562 7363 7269 7074 696f 6e73  's subscriptions
+000080d0: 2068 6173 206f 6363 7572 7265 640a 2d20   has occurred.- 
+000080e0: 4a4f 425f 5348 4152 455f 4556 454e 5420  JOB_SHARE_EVENT 
+000080f0: 2d20 6120 6a6f 6220 7265 736f 7572 6365  - a job resource
+00008100: 2068 6173 2062 6565 6e20 7368 6172 6564   has been shared
+00008110: 206f 7220 756e 7368 6172 6564 0a2d 204a   or unshared.- J
+00008120: 4f42 5f45 5252 4f52 5f4d 4553 5341 4745  OB_ERROR_MESSAGE
+00008130: 202d 2074 6865 206a 6f62 2065 7870 6572   - the job exper
+00008140: 6965 6e63 6564 2061 6e20 6572 726f 720a  ienced an error.
+00008150: 2d20 4a4f 425f 5553 4552 5f45 5645 4e54  - JOB_USER_EVENT
+00008160: 202d 2075 7365 7220 6765 6e65 7261 7465   - user generate
+00008170: 6420 6576 656e 7473 0a2d 2041 4c4c 202d  d events.- ALL -
+00008180: 2061 6c6c 206a 6f62 2065 7665 6e74 2063   all job event c
+00008190: 6174 6567 6f72 6965 730a 948c 0b6f 7065  ategories....ope
+000081a0: 7261 7469 6f6e 4964 948c 0973 7562 7363  rationId...subsc
+000081b0: 7269 6265 948c 0a70 6172 616d 6574 6572  ribe...parameter
+000081c0: 7394 5d94 287d 9428 8c04 6e61 6d65 948c  s.].(}.(..name..
+000081d0: 076a 6f62 5575 6964 948c 0269 6e94 8c04  .jobUuid...in...
+000081e0: 7061 7468 948c 0872 6571 7569 7265 6494  path...required.
+000081f0: 888c 0673 6368 656d 6194 7d94 8c04 7479  ...schema.}...ty
+00008200: 7065 948c 0673 7472 696e 6794 7375 7d94  pe...string.su}.
+00008210: 288c 046e 616d 6594 8c06 7072 6574 7479  (..name...pretty
+00008220: 948c 0269 6e94 8c05 7175 6572 7994 8c06  ...in...query...
+00008230: 7363 6865 6d61 947d 9428 8c04 7479 7065  schema.}.(..type
+00008240: 948c 0762 6f6f 6c65 616e 948c 0764 6566  ...boolean...def
+00008250: 6175 6c74 9489 7575 658c 0b72 6571 7565  ault..uue..reque
+00008260: 7374 426f 6479 947d 9428 8c07 636f 6e74  stBody.}.(..cont
+00008270: 656e 7494 7d94 8c10 6170 706c 6963 6174  ent.}...applicat
+00008280: 696f 6e2f 6a73 6f6e 947d 948c 0673 6368  ion/json.}...sch
+00008290: 656d 6194 7d94 8c04 2472 6566 948c 2123  ema.}...$ref..!#
+000082a0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+000082b0: 6d61 732f 5265 7153 7562 7363 7269 6265  mas/ReqSubscribe
+000082c0: 9473 7373 8c08 7265 7175 6972 6564 9488  .sss..required..
+000082d0: 758c 0972 6573 706f 6e73 6573 947d 9428  u..responses.}.(
+000082e0: 8c03 3230 3094 7d94 288c 0b64 6573 6372  ..200.}.(..descr
+000082f0: 6970 7469 6f6e 948c 194a 6f62 2073 7562  iption...Job sub
+00008300: 7363 7269 7074 696f 6e20 6372 6561 7465  scription create
+00008310: 642e 948c 0763 6f6e 7465 6e74 947d 948c  d....content.}..
+00008320: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00008330: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00008340: 0424 7265 6694 8c24 232f 636f 6d70 6f6e  .$ref..$#/compon
+00008350: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+00008360: 7052 6573 6f75 7263 6555 726c 9473 7373  pResourceUrl.sss
+00008370: 758c 0334 3030 947d 9428 8c0b 6465 7363  u..400.}.(..desc
+00008380: 7269 7074 696f 6e94 8c0c 496e 7075 7420  ription...Input 
+00008390: 6572 726f 722e 948c 0763 6f6e 7465 6e74  error....content
+000083a0: 947d 948c 1061 7070 6c69 6361 7469 6f6e  .}...application
+000083b0: 2f6a 736f 6e94 7d94 8c06 7363 6865 6d61  /json.}...schema
+000083c0: 947d 948c 0424 7265 6694 8c1e 232f 636f  .}...$ref...#/co
+000083d0: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+000083e0: 2f52 6573 7042 6173 6963 9473 7373 758c  /RespBasic.sssu.
+000083f0: 0334 3031 947d 9428 8c0b 6465 7363 7269  .401.}.(..descri
+00008400: 7074 696f 6e94 8c0f 4e6f 7420 6175 7468  ption...Not auth
+00008410: 6f72 697a 6564 2e94 8c07 636f 6e74 656e  orized....conten
+00008420: 7494 7d94 8c10 6170 706c 6963 6174 696f  t.}...applicatio
+00008430: 6e2f 6a73 6f6e 947d 948c 0673 6368 656d  n/json.}...schem
+00008440: 6194 7d94 8c04 2472 6566 948c 1e23 2f63  a.}...$ref...#/c
+00008450: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00008460: 732f 5265 7370 4261 7369 6394 7373 7375  s/RespBasic.sssu
+00008470: 8c03 3430 3394 7d94 288c 0b64 6573 6372  ..403.}.(..descr
+00008480: 6970 7469 6f6e 948c 0a46 6f72 6269 6464  iption...Forbidd
+00008490: 656e 2e94 8c07 636f 6e74 656e 7494 7d94  en....content.}.
+000084a0: 8c10 6170 706c 6963 6174 696f 6e2f 6a73  ..application/js
+000084b0: 6f6e 947d 948c 0673 6368 656d 6194 7d94  on.}...schema.}.
+000084c0: 8c04 2472 6566 948c 1e23 2f63 6f6d 706f  ..$ref...#/compo
+000084d0: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+000084e0: 7370 4261 7369 6394 7373 7375 8c03 3530  spBasic.sssu..50
+000084f0: 3094 7d94 288c 0b64 6573 6372 6970 7469  0.}.(..descripti
+00008500: 6f6e 948c 0d53 6572 7665 7220 6572 726f  on...Server erro
+00008510: 722e 948c 0763 6f6e 7465 6e74 947d 948c  r....content.}..
+00008520: 1061 7070 6c69 6361 7469 6f6e 2f6a 736f  .application/jso
+00008530: 6e94 7d94 8c06 7363 6865 6d61 947d 948c  n.}...schema.}..
+00008540: 0424 7265 6694 8c1e 232f 636f 6d70 6f6e  .$ref...#/compon
+00008550: 656e 7473 2f73 6368 656d 6173 2f52 6573  ents/schemas/Res
+00008560: 7042 6173 6963 9473 7373 7575 8c08 7365  pBasic.sssuu..se
+00008570: 6375 7269 7479 945d 947d 948c 0854 6170  curity.].}...Tap
+00008580: 6973 4a57 5494 5d94 7361 7575 758c 0a63  isJWT.].sauuu..c
+00008590: 6f6d 706f 6e65 6e74 7394 7d94 288c 0773  omponents.}.(..s
+000085a0: 6368 656d 6173 947d 9428 8c09 4a6f 6273  chemas.}.(..Jobs
+000085b0: 5072 6f62 6594 7d94 288c 0474 7970 6594  Probe.}.(..type.
+000085c0: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
+000085d0: 7274 6965 7394 7d94 288c 0863 6865 636b  rties.}.(..check
+000085e0: 4e75 6d94 7d94 288c 0474 7970 6594 8c07  Num.}.(..type...
+000085f0: 696e 7465 6765 7294 8c06 666f 726d 6174  integer...format
+00008600: 948c 0569 6e74 3634 9475 8c0e 6461 7461  ...int64.u..data
+00008610: 6261 7365 4163 6365 7373 947d 948c 0474  baseAccess.}...t
+00008620: 7970 6594 8c07 626f 6f6c 6561 6e94 738c  ype...boolean.s.
+00008630: 0d74 656e 616e 7473 4163 6365 7373 947d  .tenantsAccess.}
+00008640: 948c 0474 7970 6594 8c07 626f 6f6c 6561  ...type...boolea
+00008650: 6e94 738c 0b71 7565 7565 4163 6365 7373  n.s..queueAccess
+00008660: 947d 948c 0474 7970 6594 8c07 626f 6f6c  .}...type...bool
+00008670: 6561 6e94 7375 758c 0952 6573 7050 726f  ean.suu..RespPro
+00008680: 6265 947d 9428 8c04 7479 7065 948c 066f  be.}.(..type...o
+00008690: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
+000086a0: 6573 947d 9428 8c06 7374 6174 7573 947d  es.}.(..status.}
+000086b0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+000086c0: 9473 8c07 6d65 7373 6167 6594 7d94 8c04  .s..message.}...
+000086d0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+000086e0: 0776 6572 7369 6f6e 947d 948c 0474 7970  .version.}...typ
+000086f0: 6594 8c06 7374 7269 6e67 9473 8c06 636f  e...string.s..co
+00008700: 6d6d 6974 947d 948c 0474 7970 6594 8c06  mmit.}...type...
+00008710: 7374 7269 6e67 9473 8c05 6275 696c 6494  string.s..build.
+00008720: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00008730: 6794 738c 086d 6574 6164 6174 6194 7d94  g.s..metadata.}.
+00008740: 8c04 2472 6566 948c 2323 2f63 6f6d 706f  ..$ref..##/compo
+00008750: 6e65 6e74 732f 7363 6865 6d61 732f 5265  nents/schemas/Re
+00008760: 7375 6c74 4d65 7461 6461 7461 9473 8c06  sultMetadata.s..
+00008770: 7265 7375 6c74 947d 948c 0424 7265 6694  result.}...$ref.
+00008780: 8c1e 232f 636f 6d70 6f6e 656e 7473 2f73  ..#/components/s
+00008790: 6368 656d 6173 2f4a 6f62 7350 726f 6265  chemas/JobsProbe
+000087a0: 9473 7575 8c0e 5265 7375 6c74 4d65 7461  .suu..ResultMeta
+000087b0: 6461 7461 947d 948c 0474 7970 6594 8c06  data.}...type...
+000087c0: 6f62 6a65 6374 9473 8c09 5265 7370 4261  object.s..RespBa
+000087d0: 7369 6394 7d94 288c 0474 7970 6594 8c06  sic.}.(..type...
+000087e0: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
+000087f0: 6965 7394 7d94 288c 0673 7461 7475 7394  ies.}.(..status.
+00008800: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00008810: 6794 738c 076d 6573 7361 6765 947d 948c  g.s..message.}..
+00008820: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00008830: 8c07 7665 7273 696f 6e94 7d94 8c04 7479  ..version.}...ty
+00008840: 7065 948c 0673 7472 696e 6794 738c 0663  pe...string.s..c
+00008850: 6f6d 6d69 7494 7d94 8c04 7479 7065 948c  ommit.}...type..
+00008860: 0673 7472 696e 6794 738c 0562 7569 6c64  .string.s..build
+00008870: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00008880: 6e67 9473 8c08 6d65 7461 6461 7461 947d  ng.s..metadata.}
+00008890: 948c 0424 7265 6694 8c23 232f 636f 6d70  ...$ref..##/comp
+000088a0: 6f6e 656e 7473 2f73 6368 656d 6173 2f52  onents/schemas/R
+000088b0: 6573 756c 744d 6574 6164 6174 6194 738c  esultMetadata.s.
+000088c0: 0672 6573 756c 7494 7d94 8c04 7479 7065  .result.}...type
+000088d0: 948c 066f 626a 6563 7494 7375 758c 0e4a  ...object.suu..J
+000088e0: 6f62 4869 6465 4469 7370 6c61 7994 7d94  obHideDisplay.}.
+000088f0: 288c 0474 7970 6594 8c06 6f62 6a65 6374  (..type...object
+00008900: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
+00008910: 8c07 6d65 7373 6167 6594 7d94 8c04 7479  ..message.}...ty
+00008920: 7065 948c 0673 7472 696e 6794 7373 758c  pe...string.ssu.
+00008930: 0b52 6573 7048 6964 654a 6f62 947d 9428  .RespHideJob.}.(
+00008940: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
+00008950: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
+00008960: 8c06 7374 6174 7573 947d 948c 0474 7970  ..status.}...typ
+00008970: 6594 8c06 7374 7269 6e67 9473 8c07 6d65  e...string.s..me
+00008980: 7373 6167 6594 7d94 8c04 7479 7065 948c  ssage.}...type..
+00008990: 0673 7472 696e 6794 738c 0776 6572 7369  .string.s..versi
+000089a0: 6f6e 947d 948c 0474 7970 6594 8c06 7374  on.}...type...st
+000089b0: 7269 6e67 9473 8c06 636f 6d6d 6974 947d  ring.s..commit.}
+000089c0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+000089d0: 9473 8c05 6275 696c 6494 7d94 8c04 7479  .s..build.}...ty
+000089e0: 7065 948c 0673 7472 696e 6794 738c 086d  pe...string.s..m
+000089f0: 6574 6164 6174 6194 7d94 8c04 2472 6566  etadata.}...$ref
+00008a00: 948c 2323 2f63 6f6d 706f 6e65 6e74 732f  ..##/components/
+00008a10: 7363 6865 6d61 732f 5265 7375 6c74 4d65  schemas/ResultMe
+00008a20: 7461 6461 7461 9473 8c06 7265 7375 6c74  tadata.s..result
+00008a30: 947d 948c 0424 7265 6694 8c23 232f 636f  .}...$ref..##/co
+00008a40: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
+00008a50: 2f4a 6f62 4869 6465 4469 7370 6c61 7994  /JobHideDisplay.
+00008a60: 7375 758c 0852 6573 704e 616d 6594 7d94  suu..RespName.}.
+00008a70: 288c 0474 7970 6594 8c06 6f62 6a65 6374  (..type...object
+00008a80: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
+00008a90: 288c 0673 7461 7475 7394 7d94 8c04 7479  (..status.}...ty
+00008aa0: 7065 948c 0673 7472 696e 6794 738c 076d  pe...string.s..m
+00008ab0: 6573 7361 6765 947d 948c 0474 7970 6594  essage.}...type.
+00008ac0: 8c06 7374 7269 6e67 9473 8c07 7665 7273  ..string.s..vers
+00008ad0: 696f 6e94 7d94 8c04 7479 7065 948c 0673  ion.}...type...s
+00008ae0: 7472 696e 6794 738c 0663 6f6d 6d69 7494  tring.s..commit.
+00008af0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00008b00: 6794 738c 0562 7569 6c64 947d 948c 0474  g.s..build.}...t
+00008b10: 7970 6594 8c06 7374 7269 6e67 9473 8c08  ype...string.s..
+00008b20: 6d65 7461 6461 7461 947d 948c 0424 7265  metadata.}...$re
+00008b30: 6694 8c23 232f 636f 6d70 6f6e 656e 7473  f..##/components
+00008b40: 2f73 6368 656d 6173 2f52 6573 756c 744d  /schemas/ResultM
+00008b50: 6574 6164 6174 6194 738c 0672 6573 756c  etadata.s..resul
+00008b60: 7494 7d94 8c04 2472 6566 948c 1f23 2f63  t.}...$ref...#/c
+00008b70: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00008b80: 732f 5265 7375 6c74 4e61 6d65 9473 7575  s/ResultName.suu
+00008b90: 8c0a 5265 7375 6c74 4e61 6d65 947d 9428  ..ResultName.}.(
+00008ba0: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
+00008bb0: 8c0a 7072 6f70 6572 7469 6573 947d 948c  ..properties.}..
+00008bc0: 046e 616d 6594 7d94 8c04 7479 7065 948c  .name.}...type..
+00008bd0: 0673 7472 696e 6794 7373 758c 104a 6f62  .string.ssu..Job
+00008be0: 4361 6e63 656c 4469 7370 6c61 7994 7d94  CancelDisplay.}.
+00008bf0: 288c 0474 7970 6594 8c06 6f62 6a65 6374  (..type...object
+00008c00: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
+00008c10: 8c07 6d65 7373 6167 6594 7d94 8c04 7479  ..message.}...ty
+00008c20: 7065 948c 0673 7472 696e 6794 7373 758c  pe...string.ssu.
+00008c30: 0d52 6573 7043 616e 6365 6c4a 6f62 947d  .RespCancelJob.}
+00008c40: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
+00008c50: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
+00008c60: 9428 8c06 7374 6174 7573 947d 948c 0474  .(..status.}...t
+00008c70: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
+00008c80: 6d65 7373 6167 6594 7d94 8c04 7479 7065  message.}...type
+00008c90: 948c 0673 7472 696e 6794 738c 0776 6572  ...string.s..ver
+00008ca0: 7369 6f6e 947d 948c 0474 7970 6594 8c06  sion.}...type...
+00008cb0: 7374 7269 6e67 9473 8c06 636f 6d6d 6974  string.s..commit
+00008cc0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00008cd0: 6e67 9473 8c05 6275 696c 6494 7d94 8c04  ng.s..build.}...
+00008ce0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+00008cf0: 086d 6574 6164 6174 6194 7d94 8c04 2472  .metadata.}...$r
+00008d00: 6566 948c 2323 2f63 6f6d 706f 6e65 6e74  ef..##/component
+00008d10: 732f 7363 6865 6d61 732f 5265 7375 6c74  s/schemas/Result
+00008d20: 4d65 7461 6461 7461 9473 8c06 7265 7375  Metadata.s..resu
+00008d30: 6c74 947d 948c 0424 7265 6694 8c25 232f  lt.}...$ref..%#/
+00008d40: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+00008d50: 6173 2f4a 6f62 4361 6e63 656c 4469 7370  as/JobCancelDisp
+00008d60: 6c61 7994 7375 758c 034a 6f62 947d 9428  lay.suu..Job.}.(
+00008d70: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
+00008d80: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
+00008d90: 8c02 6964 947d 9428 8c04 7479 7065 948c  ..id.}.(..type..
+00008da0: 0769 6e74 6567 6572 948c 0666 6f72 6d61  .integer...forma
+00008db0: 7494 8c05 696e 7433 3294 758c 046e 616d  t...int32.u..nam
+00008dc0: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+00008dd0: 696e 6794 738c 056f 776e 6572 947d 948c  ing.s..owner.}..
+00008de0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00008df0: 8c06 7465 6e61 6e74 947d 948c 0474 7970  ..tenant.}...typ
+00008e00: 6594 8c06 7374 7269 6e67 9473 8c0b 6465  e...string.s..de
+00008e10: 7363 7269 7074 696f 6e94 7d94 8c04 7479  scription.}...ty
+00008e20: 7065 948c 0673 7472 696e 6794 738c 0673  pe...string.s..s
+00008e30: 7461 7475 7394 7d94 288c 0474 7970 6594  tatus.}.(..type.
+00008e40: 8c06 7374 7269 6e67 948c 0465 6e75 6d94  ..string...enum.
+00008e50: 5d94 288c 0750 454e 4449 4e47 948c 1150  ].(..PENDING...P
+00008e60: 524f 4345 5353 494e 475f 494e 5055 5453  ROCESSING_INPUTS
+00008e70: 948c 0e53 5441 4749 4e47 5f49 4e50 5554  ...STAGING_INPUT
+00008e80: 5394 8c0b 5354 4147 494e 475f 4a4f 4294  S...STAGING_JOB.
+00008e90: 8c0e 5355 424d 4954 5449 4e47 5f4a 4f42  ..SUBMITTING_JOB
+00008ea0: 948c 0651 5545 5545 4494 8c07 5255 4e4e  ...QUEUED...RUNN
+00008eb0: 494e 4794 8c09 4152 4348 4956 494e 4794  ING...ARCHIVING.
+00008ec0: 8c07 424c 4f43 4b45 4494 8c06 5041 5553  ..BLOCKED...PAUS
+00008ed0: 4544 948c 0846 494e 4953 4845 4494 8c09  ED...FINISHED...
+00008ee0: 4341 4e43 454c 4c45 4494 8c06 4641 494c  CANCELLED...FAIL
+00008ef0: 4544 9465 758c 0b6c 6173 744d 6573 7361  ED.eu..lastMessa
+00008f00: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
+00008f10: 7269 6e67 9473 8c07 6372 6561 7465 6494  ring.s..created.
+00008f20: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00008f30: 6794 738c 0565 6e64 6564 947d 948c 0474  g.s..ended.}...t
+00008f40: 7970 6594 8c06 7374 7269 6e67 9473 8c0b  ype...string.s..
+00008f50: 6c61 7374 5570 6461 7465 6494 7d94 8c04  lastUpdated.}...
+00008f60: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+00008f70: 0475 7569 6494 7d94 8c04 7479 7065 948c  .uuid.}...type..
+00008f80: 0673 7472 696e 6794 738c 0561 7070 4964  .string.s..appId
+00008f90: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00008fa0: 6e67 9473 8c0a 6170 7056 6572 7369 6f6e  ng.s..appVersion
+00008fb0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00008fc0: 6e67 9473 8c11 6172 6368 6976 654f 6e41  ng.s..archiveOnA
+00008fd0: 7070 4572 726f 7294 7d94 8c04 7479 7065  ppError.}...type
+00008fe0: 948c 0762 6f6f 6c65 616e 9473 8c11 6479  ...boolean.s..dy
+00008ff0: 6e61 6d69 6345 7865 6353 7973 7465 6d94  namicExecSystem.
+00009000: 7d94 8c04 7479 7065 948c 0762 6f6f 6c65  }...type...boole
+00009010: 616e 9473 8c0c 6578 6563 5379 7374 656d  an.s..execSystem
+00009020: 4964 947d 948c 0474 7970 6594 8c06 7374  Id.}...type...st
+00009030: 7269 6e67 9473 8c11 6578 6563 5379 7374  ring.s..execSyst
+00009040: 656d 4578 6563 4469 7294 7d94 8c04 7479  emExecDir.}...ty
+00009050: 7065 948c 0673 7472 696e 6794 738c 1265  pe...string.s..e
+00009060: 7865 6353 7973 7465 6d49 6e70 7574 4469  xecSystemInputDi
+00009070: 7294 7d94 8c04 7479 7065 948c 0673 7472  r.}...type...str
+00009080: 696e 6794 738c 1365 7865 6353 7973 7465  ing.s..execSyste
+00009090: 6d4f 7574 7075 7444 6972 947d 948c 0474  mOutputDir.}...t
+000090a0: 7970 6594 8c06 7374 7269 6e67 9473 8c16  ype...string.s..
+000090b0: 6578 6563 5379 7374 656d 4c6f 6769 6361  execSystemLogica
+000090c0: 6c51 7565 7565 947d 948c 0474 7970 6594  lQueue.}...type.
+000090d0: 8c06 7374 7269 6e67 9473 8c0f 6172 6368  ..string.s..arch
+000090e0: 6976 6553 7973 7465 6d49 6494 7d94 8c04  iveSystemId.}...
+000090f0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+00009100: 1061 7263 6869 7665 5379 7374 656d 4469  .archiveSystemDi
+00009110: 7294 7d94 8c04 7479 7065 948c 0673 7472  r.}...type...str
+00009120: 696e 6794 738c 0b64 746e 5379 7374 656d  ing.s..dtnSystem
+00009130: 4964 947d 948c 0474 7970 6594 8c06 7374  Id.}...type...st
+00009140: 7269 6e67 9473 8c12 6474 6e4d 6f75 6e74  ring.s..dtnMount
+00009150: 536f 7572 6365 5061 7468 947d 948c 0474  SourcePath.}...t
+00009160: 7970 6594 8c06 7374 7269 6e67 9473 8c0d  ype...string.s..
+00009170: 6474 6e4d 6f75 6e74 506f 696e 7494 7d94  dtnMountPoint.}.
+00009180: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+00009190: 738c 096e 6f64 6543 6f75 6e74 947d 9428  s..nodeCount.}.(
+000091a0: 8c04 7479 7065 948c 0769 6e74 6567 6572  ..type...integer
+000091b0: 948c 0666 6f72 6d61 7494 8c05 696e 7433  ...format...int3
+000091c0: 3294 758c 0c63 6f72 6573 5065 724e 6f64  2.u..coresPerNod
+000091d0: 6594 7d94 288c 0474 7970 6594 8c07 696e  e.}.(..type...in
+000091e0: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
+000091f0: 0569 6e74 3332 9475 8c08 6d65 6d6f 7279  .int32.u..memory
+00009200: 4d42 947d 9428 8c04 7479 7065 948c 0769  MB.}.(..type...i
+00009210: 6e74 6567 6572 948c 0666 6f72 6d61 7494  nteger...format.
+00009220: 8c05 696e 7433 3294 758c 0a6d 6178 4d69  ..int32.u..maxMi
+00009230: 6e75 7465 7394 7d94 288c 0474 7970 6594  nutes.}.(..type.
+00009240: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
+00009250: 6174 948c 0569 6e74 3332 9475 8c0a 6669  at...int32.u..fi
+00009260: 6c65 496e 7075 7473 947d 948c 0474 7970  leInputs.}...typ
+00009270: 6594 8c06 7374 7269 6e67 9473 8c0c 7061  e...string.s..pa
+00009280: 7261 6d65 7465 7253 6574 947d 948c 0474  rameterSet.}...t
+00009290: 7970 6594 8c06 7374 7269 6e67 9473 8c15  ype...string.s..
+000092a0: 6578 6563 5379 7374 656d 436f 6e73 7472  execSystemConstr
+000092b0: 6169 6e74 7394 7d94 8c04 7479 7065 948c  aints.}...type..
+000092c0: 0673 7472 696e 6794 738c 0d73 7562 7363  .string.s..subsc
+000092d0: 7269 7074 696f 6e73 947d 948c 0474 7970  riptions.}...typ
+000092e0: 6594 8c06 7374 7269 6e67 9473 8c0c 626c  e...string.s..bl
+000092f0: 6f63 6b65 6443 6f75 6e74 947d 9428 8c04  ockedCount.}.(..
+00009300: 7479 7065 948c 0769 6e74 6567 6572 948c  type...integer..
+00009310: 0666 6f72 6d61 7494 8c05 696e 7433 3294  .format...int32.
+00009320: 758c 0b72 656d 6f74 654a 6f62 4964 947d  u..remoteJobId.}
+00009330: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+00009340: 9473 8c0c 7265 6d6f 7465 4a6f 6249 6432  .s..remoteJobId2
+00009350: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00009360: 6e67 9473 8c0d 7265 6d6f 7465 4f75 7463  ng.s..remoteOutc
+00009370: 6f6d 6594 7d94 288c 0474 7970 6594 8c06  ome.}.(..type...
+00009380: 7374 7269 6e67 948c 0465 6e75 6d94 5d94  string...enum.].
+00009390: 288c 0846 494e 4953 4845 4494 8c06 4641  (..FINISHED...FA
+000093a0: 494c 4544 948c 1346 4149 4c45 445f 534b  ILED...FAILED_SK
+000093b0: 4950 5f41 5243 4849 5645 9465 758c 1072  IP_ARCHIVE.eu..r
+000093c0: 656d 6f74 6552 6573 756c 7449 6e66 6f94  emoteResultInfo.
+000093d0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+000093e0: 6794 738c 0b72 656d 6f74 6551 7565 7565  g.s..remoteQueue
+000093f0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00009400: 6e67 9473 8c0f 7265 6d6f 7465 5375 626d  ng.s..remoteSubm
+00009410: 6974 7465 6494 7d94 8c04 7479 7065 948c  itted.}...type..
+00009420: 0673 7472 696e 6794 738c 0d72 656d 6f74  .string.s..remot
+00009430: 6553 7461 7274 6564 947d 948c 0474 7970  eStarted.}...typ
+00009440: 6594 8c06 7374 7269 6e67 9473 8c0b 7265  e...string.s..re
+00009450: 6d6f 7465 456e 6465 6494 7d94 8c04 7479  moteEnded.}...ty
+00009460: 7065 948c 0673 7472 696e 6794 738c 1372  pe...string.s..r
+00009470: 656d 6f74 6553 7562 6d69 7452 6574 7269  emoteSubmitRetri
+00009480: 6573 947d 9428 8c04 7479 7065 948c 0769  es.}.(..type...i
+00009490: 6e74 6567 6572 948c 0666 6f72 6d61 7494  nteger...format.
+000094a0: 8c05 696e 7433 3294 758c 1372 656d 6f74  ..int32.u..remot
+000094b0: 6543 6865 636b 7353 7563 6365 7373 947d  eChecksSuccess.}
+000094c0: 9428 8c04 7479 7065 948c 0769 6e74 6567  .(..type...integ
+000094d0: 6572 948c 0666 6f72 6d61 7494 8c05 696e  er...format...in
+000094e0: 7433 3294 758c 1272 656d 6f74 6543 6865  t32.u..remoteChe
+000094f0: 636b 7346 6169 6c65 6494 7d94 288c 0474  cksFailed.}.(..t
+00009500: 7970 6594 8c07 696e 7465 6765 7294 8c06  ype...integer...
+00009510: 666f 726d 6174 948c 0569 6e74 3332 9475  format...int32.u
+00009520: 8c15 7265 6d6f 7465 4c61 7374 5374 6174  ..remoteLastStat
+00009530: 7573 4368 6563 6b94 7d94 8c04 7479 7065  usCheck.}...type
+00009540: 948c 0673 7472 696e 6794 738c 1269 6e70  ...string.s..inp
+00009550: 7574 5472 616e 7361 6374 696f 6e49 6494  utTransactionId.
+00009560: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00009570: 6794 738c 1269 6e70 7574 436f 7272 656c  g.s..inputCorrel
+00009580: 6174 696f 6e49 6494 7d94 8c04 7479 7065  ationId.}...type
+00009590: 948c 0673 7472 696e 6794 738c 1461 7263  ...string.s..arc
+000095a0: 6869 7665 5472 616e 7361 6374 696f 6e49  hiveTransactionI
+000095b0: 6494 7d94 8c04 7479 7065 948c 0673 7472  d.}...type...str
+000095c0: 696e 6794 738c 1461 7263 6869 7665 436f  ing.s..archiveCo
+000095d0: 7272 656c 6174 696f 6e49 6494 7d94 8c04  rrelationId.}...
+000095e0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+000095f0: 0a74 6170 6973 5175 6575 6594 7d94 8c04  .tapisQueue.}...
+00009600: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+00009610: 0776 6973 6962 6c65 947d 948c 0474 7970  .visible.}...typ
+00009620: 6594 8c07 626f 6f6c 6561 6e94 738c 0963  e...boolean.s..c
+00009630: 7265 6174 6564 6279 947d 948c 0474 7970  reatedby.}...typ
+00009640: 6594 8c06 7374 7269 6e67 9473 8c0f 6372  e...string.s..cr
+00009650: 6561 7465 6462 7954 656e 616e 7494 7d94  eatedbyTenant.}.
+00009660: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+00009670: 738c 0474 6167 7394 7d94 288c 0474 7970  s..tags.}.(..typ
+00009680: 6594 8c05 6172 7261 7994 8c05 6974 656d  e...array...item
+00009690: 7394 7d94 8c04 7479 7065 948c 0673 7472  s.}...type...str
+000096a0: 696e 6794 7375 8c07 6a6f 6254 7970 6594  ing.su..jobType.
+000096b0: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
+000096c0: 6e67 948c 0465 6e75 6d94 5d94 288c 0446  ng...enum.].(..F
+000096d0: 4f52 4b94 8c05 4241 5443 4894 6575 8c06  ORK...BATCH.eu..
+000096e0: 6d70 6943 6d64 947d 948c 0474 7970 6594  mpiCmd.}...type.
+000096f0: 8c06 7374 7269 6e67 9473 8c09 636d 6450  ..string.s..cmdP
+00009700: 7265 6669 7894 7d94 8c04 7479 7065 948c  refix.}...type..
+00009710: 0673 7472 696e 6794 738c 0c73 6861 7265  .string.s..share
+00009720: 6441 7070 4374 7894 7d94 8c04 7479 7065  dAppCtx.}...type
+00009730: 948c 0673 7472 696e 6794 738c 1373 6861  ...string.s..sha
+00009740: 7265 6441 7070 4374 7841 7474 7269 6273  redAppCtxAttribs
+00009750: 947d 9428 8c04 7479 7065 948c 0561 7272  .}.(..type...arr
+00009760: 6179 948c 0569 7465 6d73 947d 9428 8c04  ay...items.}.(..
+00009770: 7479 7065 948c 0673 7472 696e 6794 8c04  type...string...
+00009780: 656e 756d 945d 9428 8c12 5341 435f 4558  enum.].(..SAC_EX
+00009790: 4543 5f53 5953 5445 4d5f 4944 948c 1853  EC_SYSTEM_ID...S
+000097a0: 4143 5f45 5845 435f 5359 5354 454d 5f45  AC_EXEC_SYSTEM_E
+000097b0: 5845 435f 4449 5294 8c19 5341 435f 4558  XEC_DIR...SAC_EX
+000097c0: 4543 5f53 5953 5445 4d5f 494e 5055 545f  EC_SYSTEM_INPUT_
+000097d0: 4449 5294 8c1a 5341 435f 4558 4543 5f53  DIR...SAC_EXEC_S
+000097e0: 5953 5445 4d5f 4f55 5450 5554 5f44 4952  YSTEM_OUTPUT_DIR
+000097f0: 948c 1553 4143 5f41 5243 4849 5645 5f53  ...SAC_ARCHIVE_S
+00009800: 5953 5445 4d5f 4944 948c 1653 4143 5f41  YSTEM_ID...SAC_A
+00009810: 5243 4849 5645 5f53 5953 5445 4d5f 4449  RCHIVE_SYSTEM_DI
+00009820: 5294 6575 758c 056e 6f74 6573 947d 948c  R.euu..notes.}..
+00009830: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00009840: 8c03 6d70 6994 7d94 8c04 7479 7065 948c  ..mpi.}...type..
+00009850: 0762 6f6f 6c65 616e 9473 7575 8c0a 5265  .boolean.suu..Re
+00009860: 7370 4765 744a 6f62 947d 9428 8c04 7479  spGetJob.}.(..ty
+00009870: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
+00009880: 6f70 6572 7469 6573 947d 9428 8c06 7374  operties.}.(..st
+00009890: 6174 7573 947d 948c 0474 7970 6594 8c06  atus.}...type...
+000098a0: 7374 7269 6e67 9473 8c07 6d65 7373 6167  string.s..messag
+000098b0: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+000098c0: 696e 6794 738c 0776 6572 7369 6f6e 947d  ing.s..version.}
+000098d0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+000098e0: 9473 8c06 636f 6d6d 6974 947d 948c 0474  .s..commit.}...t
+000098f0: 7970 6594 8c06 7374 7269 6e67 9473 8c05  ype...string.s..
+00009900: 6275 696c 6494 7d94 8c04 7479 7065 948c  build.}...type..
+00009910: 0673 7472 696e 6794 738c 086d 6574 6164  .string.s..metad
+00009920: 6174 6194 7d94 8c04 2472 6566 948c 2323  ata.}...$ref..##
+00009930: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+00009940: 6d61 732f 5265 7375 6c74 4d65 7461 6461  mas/ResultMetada
+00009950: 7461 9473 8c06 7265 7375 6c74 947d 948c  ta.s..result.}..
+00009960: 0424 7265 6694 8c18 232f 636f 6d70 6f6e  .$ref...#/compon
+00009970: 656e 7473 2f73 6368 656d 6173 2f4a 6f62  ents/schemas/Job
+00009980: 9473 7575 8c14 4a6f 6248 6973 746f 7279  .suu..JobHistory
+00009990: 4469 7370 6c61 7944 544f 947d 9428 8c04  DisplayDTO.}.(..
+000099a0: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
+000099b0: 7072 6f70 6572 7469 6573 947d 9428 8c05  properties.}.(..
+000099c0: 6576 656e 7494 7d94 8c04 7479 7065 948c  event.}...type..
+000099d0: 0673 7472 696e 6794 738c 0763 7265 6174  .string.s..creat
+000099e0: 6564 947d 9428 8c04 7479 7065 948c 0673  ed.}.(..type...s
+000099f0: 7472 696e 6794 8c06 666f 726d 6174 948c  tring...format..
+00009a00: 0964 6174 652d 7469 6d65 9475 8c0b 6576  .date-time.u..ev
+00009a10: 656e 7444 6574 6169 6c94 7d94 8c04 7479  entDetail.}...ty
+00009a20: 7065 948c 0673 7472 696e 6794 738c 0b64  pe...string.s..d
+00009a30: 6573 6372 6970 7469 6f6e 947d 948c 0474  escription.}...t
+00009a40: 7970 6594 8c06 7374 7269 6e67 9473 8c10  ype...string.s..
+00009a50: 7472 616e 7366 6572 5461 736b 5575 6964  transferTaskUuid
+00009a60: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+00009a70: 6e67 9473 7575 8c0e 5265 7370 4a6f 6248  ng.suu..RespJobH
+00009a80: 6973 746f 7279 947d 9428 8c04 7479 7065  istory.}.(..type
+00009a90: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
+00009aa0: 6572 7469 6573 947d 9428 8c06 7374 6174  erties.}.(..stat
+00009ab0: 7573 947d 948c 0474 7970 6594 8c06 7374  us.}...type...st
+00009ac0: 7269 6e67 9473 8c07 6d65 7373 6167 6594  ring.s..message.
+00009ad0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00009ae0: 6794 738c 0776 6572 7369 6f6e 947d 948c  g.s..version.}..
+00009af0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00009b00: 8c06 636f 6d6d 6974 947d 948c 0474 7970  ..commit.}...typ
+00009b10: 6594 8c06 7374 7269 6e67 9473 8c05 6275  e...string.s..bu
+00009b20: 696c 6494 7d94 8c04 7479 7065 948c 0673  ild.}...type...s
+00009b30: 7472 696e 6794 738c 086d 6574 6164 6174  tring.s..metadat
+00009b40: 6194 7d94 8c04 2472 6566 948c 2323 2f63  a.}...$ref..##/c
+00009b50: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+00009b60: 732f 5265 7375 6c74 4d65 7461 6461 7461  s/ResultMetadata
+00009b70: 9473 8c06 7265 7375 6c74 947d 9428 8c04  .s..result.}.(..
+00009b80: 7479 7065 948c 0561 7272 6179 948c 0569  type...array...i
+00009b90: 7465 6d73 947d 948c 0424 7265 6694 8c29  tems.}...$ref..)
+00009ba0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00009bb0: 656d 6173 2f4a 6f62 4869 7374 6f72 7944  emas/JobHistoryD
+00009bc0: 6973 706c 6179 4454 4f94 7375 7575 8c0a  isplayDTO.suuu..
+00009bd0: 4a6f 624c 6973 7444 544f 947d 9428 8c04  JobListDTO.}.(..
+00009be0: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
+00009bf0: 7072 6f70 6572 7469 6573 947d 9428 8c04  properties.}.(..
+00009c00: 7575 6964 947d 948c 0474 7970 6594 8c06  uuid.}...type...
+00009c10: 7374 7269 6e67 9473 8c04 6e61 6d65 947d  string.s..name.}
+00009c20: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+00009c30: 9473 8c05 6f77 6e65 7294 7d94 8c04 7479  .s..owner.}...ty
+00009c40: 7065 948c 0673 7472 696e 6794 738c 0561  pe...string.s..a
+00009c50: 7070 4964 947d 948c 0474 7970 6594 8c06  ppId.}...type...
+00009c60: 7374 7269 6e67 9473 8c07 6372 6561 7465  string.s..create
+00009c70: 6494 7d94 288c 0474 7970 6594 8c06 7374  d.}.(..type...st
+00009c80: 7269 6e67 948c 0666 6f72 6d61 7494 8c09  ring...format...
+00009c90: 6461 7465 2d74 696d 6594 758c 0673 7461  date-time.u..sta
+00009ca0: 7475 7394 7d94 288c 0474 7970 6594 8c06  tus.}.(..type...
+00009cb0: 7374 7269 6e67 948c 0465 6e75 6d94 5d94  string...enum.].
+00009cc0: 288c 0750 454e 4449 4e47 948c 1150 524f  (..PENDING...PRO
+00009cd0: 4345 5353 494e 475f 494e 5055 5453 948c  CESSING_INPUTS..
+00009ce0: 0e53 5441 4749 4e47 5f49 4e50 5554 5394  .STAGING_INPUTS.
+00009cf0: 8c0b 5354 4147 494e 475f 4a4f 4294 8c0e  ..STAGING_JOB...
+00009d00: 5355 424d 4954 5449 4e47 5f4a 4f42 948c  SUBMITTING_JOB..
+00009d10: 0651 5545 5545 4494 8c07 5255 4e4e 494e  .QUEUED...RUNNIN
+00009d20: 4794 8c09 4152 4348 4956 494e 4794 8c07  G...ARCHIVING...
+00009d30: 424c 4f43 4b45 4494 8c06 5041 5553 4544  BLOCKED...PAUSED
+00009d40: 948c 0846 494e 4953 4845 4494 8c09 4341  ...FINISHED...CA
+00009d50: 4e43 454c 4c45 4494 8c06 4641 494c 4544  NCELLED...FAILED
+00009d60: 9465 758c 0d72 656d 6f74 6553 7461 7274  .eu..remoteStart
+00009d70: 6564 947d 9428 8c04 7479 7065 948c 0673  ed.}.(..type...s
+00009d80: 7472 696e 6794 8c06 666f 726d 6174 948c  tring...format..
+00009d90: 0964 6174 652d 7469 6d65 9475 8c05 656e  .date-time.u..en
+00009da0: 6465 6494 7d94 288c 0474 7970 6594 8c06  ded.}.(..type...
+00009db0: 7374 7269 6e67 948c 0666 6f72 6d61 7494  string...format.
+00009dc0: 8c09 6461 7465 2d74 696d 6594 758c 0674  ..date-time.u..t
+00009dd0: 656e 616e 7494 7d94 8c04 7479 7065 948c  enant.}...type..
+00009de0: 0673 7472 696e 6794 738c 0c65 7865 6353  .string.s..execS
+00009df0: 7973 7465 6d49 6494 7d94 8c04 7479 7065  ystemId.}...type
+00009e00: 948c 0673 7472 696e 6794 738c 0f61 7263  ...string.s..arc
+00009e10: 6869 7665 5379 7374 656d 4964 947d 948c  hiveSystemId.}..
+00009e20: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00009e30: 8c0a 6170 7056 6572 7369 6f6e 947d 948c  ..appVersion.}..
+00009e40: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+00009e50: 8c0b 6c61 7374 5570 6461 7465 6494 7d94  ..lastUpdated.}.
+00009e60: 288c 0474 7970 6594 8c06 7374 7269 6e67  (..type...string
+00009e70: 948c 0666 6f72 6d61 7494 8c09 6461 7465  ...format...date
+00009e80: 2d74 696d 6594 7575 758c 0e52 6573 7047  -time.uuu..RespG
+00009e90: 6574 4a6f 624c 6973 7494 7d94 288c 0474  etJobList.}.(..t
+00009ea0: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
+00009eb0: 726f 7065 7274 6965 7394 7d94 288c 0673  roperties.}.(..s
+00009ec0: 7461 7475 7394 7d94 8c04 7479 7065 948c  tatus.}...type..
+00009ed0: 0673 7472 696e 6794 738c 076d 6573 7361  .string.s..messa
+00009ee0: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
+00009ef0: 7269 6e67 9473 8c07 7665 7273 696f 6e94  ring.s..version.
+00009f00: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+00009f10: 6794 738c 0663 6f6d 6d69 7494 7d94 8c04  g.s..commit.}...
+00009f20: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+00009f30: 0562 7569 6c64 947d 948c 0474 7970 6594  .build.}...type.
+00009f40: 8c06 7374 7269 6e67 9473 8c08 6d65 7461  ..string.s..meta
+00009f50: 6461 7461 947d 948c 0424 7265 6694 8c23  data.}...$ref..#
+00009f60: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+00009f70: 656d 6173 2f52 6573 756c 744d 6574 6164  emas/ResultMetad
+00009f80: 6174 6194 738c 0672 6573 756c 7494 7d94  ata.s..result.}.
+00009f90: 288c 0474 7970 6594 8c05 6172 7261 7994  (..type...array.
+00009fa0: 8c05 6974 656d 7394 7d94 8c04 2472 6566  ..items.}...$ref
+00009fb0: 948c 1f23 2f63 6f6d 706f 6e65 6e74 732f  ...#/components/
+00009fc0: 7363 6865 6d61 732f 4a6f 624c 6973 7444  schemas/JobListD
+00009fd0: 544f 9473 7575 758c 0846 696c 6549 6e66  TO.suuu..FileInf
+00009fe0: 6f94 7d94 288c 0474 7970 6594 8c06 6f62  o.}.(..type...ob
+00009ff0: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
+0000a000: 7394 7d94 288c 086d 696d 6554 7970 6594  s.}.(..mimeType.
+0000a010: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000a020: 6794 738c 0474 7970 6594 7d94 8c04 7479  g.s..type.}...ty
+0000a030: 7065 948c 0673 7472 696e 6794 738c 056f  pe...string.s..o
+0000a040: 776e 6572 947d 948c 0474 7970 6594 8c06  wner.}...type...
+0000a050: 7374 7269 6e67 9473 8c05 6772 6f75 7094  string.s..group.
+0000a060: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000a070: 6794 738c 116e 6174 6976 6550 6572 6d69  g.s..nativePermi
+0000a080: 7373 696f 6e73 947d 948c 0474 7970 6594  ssions.}...type.
+0000a090: 8c06 7374 7269 6e67 9473 8c03 7572 6c94  ..string.s..url.
+0000a0a0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000a0b0: 6794 738c 0c6c 6173 744d 6f64 6966 6965  g.s..lastModifie
+0000a0c0: 6494 7d94 288c 0474 7970 6594 8c06 7374  d.}.(..type...st
+0000a0d0: 7269 6e67 948c 0666 6f72 6d61 7494 8c09  ring...format...
+0000a0e0: 6461 7465 2d74 696d 6594 758c 046e 616d  date-time.u..nam
+0000a0f0: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+0000a100: 696e 6794 738c 0470 6174 6894 7d94 8c04  ing.s..path.}...
+0000a110: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000a120: 0473 697a 6594 7d94 288c 0474 7970 6594  .size.}.(..type.
+0000a130: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
+0000a140: 6174 948c 0569 6e74 3634 9475 7575 8c14  at...int64.uuu..
+0000a150: 5265 7370 4765 744a 6f62 4f75 7470 7574  RespGetJobOutput
+0000a160: 4c69 7374 947d 9428 8c04 7479 7065 948c  List.}.(..type..
+0000a170: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
+0000a180: 7469 6573 947d 9428 8c06 7374 6174 7573  ties.}.(..status
+0000a190: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000a1a0: 6e67 9473 8c07 6d65 7373 6167 6594 7d94  ng.s..message.}.
+0000a1b0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000a1c0: 738c 0776 6572 7369 6f6e 947d 948c 0474  s..version.}...t
+0000a1d0: 7970 6594 8c06 7374 7269 6e67 9473 8c06  ype...string.s..
+0000a1e0: 636f 6d6d 6974 947d 948c 0474 7970 6594  commit.}...type.
+0000a1f0: 8c06 7374 7269 6e67 9473 8c05 6275 696c  ..string.s..buil
+0000a200: 6494 7d94 8c04 7479 7065 948c 0673 7472  d.}...type...str
+0000a210: 696e 6794 738c 086d 6574 6164 6174 6194  ing.s..metadata.
+0000a220: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
+0000a230: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+0000a240: 5265 7375 6c74 4d65 7461 6461 7461 9473  ResultMetadata.s
+0000a250: 8c06 7265 7375 6c74 947d 9428 8c04 7479  ..result.}.(..ty
+0000a260: 7065 948c 0561 7272 6179 948c 0569 7465  pe...array...ite
+0000a270: 6d73 947d 948c 0424 7265 6694 8c1d 232f  ms.}...$ref...#/
+0000a280: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+0000a290: 6173 2f46 696c 6549 6e66 6f94 7375 7575  as/FileInfo.suuu
+0000a2a0: 8c1a 5265 7370 4a6f 6253 6561 7263 6841  ..RespJobSearchA
+0000a2b0: 6c6c 4174 7472 6962 7574 6573 947d 9428  llAttributes.}.(
+0000a2c0: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
+0000a2d0: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
+0000a2e0: 8c06 7374 6174 7573 947d 948c 0474 7970  ..status.}...typ
+0000a2f0: 6594 8c06 7374 7269 6e67 9473 8c07 6d65  e...string.s..me
+0000a300: 7373 6167 6594 7d94 8c04 7479 7065 948c  ssage.}...type..
+0000a310: 0673 7472 696e 6794 738c 0776 6572 7369  .string.s..versi
+0000a320: 6f6e 947d 948c 0474 7970 6594 8c06 7374  on.}...type...st
+0000a330: 7269 6e67 9473 8c06 636f 6d6d 6974 947d  ring.s..commit.}
+0000a340: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000a350: 9473 8c05 6275 696c 6494 7d94 8c04 7479  .s..build.}...ty
+0000a360: 7065 948c 0673 7472 696e 6794 738c 086d  pe...string.s..m
+0000a370: 6574 6164 6174 6194 7d94 8c04 2472 6566  etadata.}...$ref
+0000a380: 948c 2323 2f63 6f6d 706f 6e65 6e74 732f  ..##/components/
+0000a390: 7363 6865 6d61 732f 5265 7375 6c74 4d65  schemas/ResultMe
+0000a3a0: 7461 6461 7461 9473 8c06 7265 7375 6c74  tadata.s..result
+0000a3b0: 947d 9428 8c04 7479 7065 948c 0561 7272  .}.(..type...arr
+0000a3c0: 6179 948c 0569 7465 6d73 947d 948c 0424  ay...items.}...$
+0000a3d0: 7265 6694 8c18 232f 636f 6d70 6f6e 656e  ref...#/componen
+0000a3e0: 7473 2f73 6368 656d 6173 2f4a 6f62 9473  ts/schemas/Job.s
+0000a3f0: 7575 758c 114a 6f62 556e 5368 6172 6544  uuu..JobUnShareD
+0000a400: 6973 706c 6179 947d 9428 8c04 7479 7065  isplay.}.(..type
+0000a410: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
+0000a420: 6572 7469 6573 947d 948c 076d 6573 7361  erties.}...messa
+0000a430: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
+0000a440: 7269 6e67 9473 7375 8c0e 5265 7370 556e  ring.ssu..RespUn
+0000a450: 5368 6172 654a 6f62 947d 9428 8c04 7479  ShareJob.}.(..ty
+0000a460: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
+0000a470: 6f70 6572 7469 6573 947d 9428 8c06 7374  operties.}.(..st
+0000a480: 6174 7573 947d 948c 0474 7970 6594 8c06  atus.}...type...
+0000a490: 7374 7269 6e67 9473 8c07 6d65 7373 6167  string.s..messag
+0000a4a0: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+0000a4b0: 696e 6794 738c 0776 6572 7369 6f6e 947d  ing.s..version.}
+0000a4c0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000a4d0: 9473 8c06 636f 6d6d 6974 947d 948c 0474  .s..commit.}...t
+0000a4e0: 7970 6594 8c06 7374 7269 6e67 9473 8c05  ype...string.s..
+0000a4f0: 6275 696c 6494 7d94 8c04 7479 7065 948c  build.}...type..
+0000a500: 0673 7472 696e 6794 738c 086d 6574 6164  .string.s..metad
+0000a510: 6174 6194 7d94 8c04 2472 6566 948c 2323  ata.}...$ref..##
+0000a520: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+0000a530: 6d61 732f 5265 7375 6c74 4d65 7461 6461  mas/ResultMetada
+0000a540: 7461 9473 8c06 7265 7375 6c74 947d 948c  ta.s..result.}..
+0000a550: 0424 7265 6694 8c26 232f 636f 6d70 6f6e  .$ref..&#/compon
+0000a560: 656e 7473 2f73 6368 656d 6173 2f4a 6f62  ents/schemas/Job
+0000a570: 556e 5368 6172 6544 6973 706c 6179 9473  UnShareDisplay.s
+0000a580: 7575 8c0f 4a6f 6253 6861 7265 4c69 7374  uu..JobShareList
+0000a590: 4454 4f94 7d94 288c 0474 7970 6594 8c06  DTO.}.(..type...
+0000a5a0: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
+0000a5b0: 6965 7394 7d94 288c 0674 656e 616e 7494  ies.}.(..tenant.
+0000a5c0: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000a5d0: 6794 738c 0963 7265 6174 6564 6279 947d  g.s..createdby.}
+0000a5e0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000a5f0: 9473 8c07 6a6f 6255 7569 6494 7d94 8c04  .s..jobUuid.}...
+0000a600: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000a610: 0767 7261 6e74 6565 947d 948c 0474 7970  .grantee.}...typ
+0000a620: 6594 8c06 7374 7269 6e67 9473 8c0b 6a6f  e...string.s..jo
+0000a630: 6252 6573 6f75 7263 6594 7d94 8c04 7479  bResource.}...ty
+0000a640: 7065 948c 0673 7472 696e 6794 738c 0d6a  pe...string.s..j
+0000a650: 6f62 5065 726d 6973 7369 6f6e 947d 948c  obPermission.}..
+0000a660: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000a670: 8c07 6372 6561 7465 6494 7d94 288c 0474  ..created.}.(..t
+0000a680: 7970 6594 8c06 7374 7269 6e67 948c 0666  ype...string...f
+0000a690: 6f72 6d61 7494 8c09 6461 7465 2d74 696d  ormat...date-tim
+0000a6a0: 6594 7575 758c 1352 6573 7047 6574 4a6f  e.uuu..RespGetJo
+0000a6b0: 6253 6861 7265 4c69 7374 947d 9428 8c04  bShareList.}.(..
+0000a6c0: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
+0000a6d0: 7072 6f70 6572 7469 6573 947d 9428 8c06  properties.}.(..
+0000a6e0: 7374 6174 7573 947d 948c 0474 7970 6594  status.}...type.
+0000a6f0: 8c06 7374 7269 6e67 9473 8c07 6d65 7373  ..string.s..mess
+0000a700: 6167 6594 7d94 8c04 7479 7065 948c 0673  age.}...type...s
+0000a710: 7472 696e 6794 738c 0776 6572 7369 6f6e  tring.s..version
+0000a720: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000a730: 6e67 9473 8c06 636f 6d6d 6974 947d 948c  ng.s..commit.}..
+0000a740: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000a750: 8c05 6275 696c 6494 7d94 8c04 7479 7065  ..build.}...type
+0000a760: 948c 0673 7472 696e 6794 738c 086d 6574  ...string.s..met
+0000a770: 6164 6174 6194 7d94 8c04 2472 6566 948c  adata.}...$ref..
+0000a780: 2323 2f63 6f6d 706f 6e65 6e74 732f 7363  ##/components/sc
+0000a790: 6865 6d61 732f 5265 7375 6c74 4d65 7461  hemas/ResultMeta
+0000a7a0: 6461 7461 9473 8c06 7265 7375 6c74 947d  data.s..result.}
+0000a7b0: 9428 8c04 7479 7065 948c 0561 7272 6179  .(..type...array
+0000a7c0: 948c 0569 7465 6d73 947d 948c 0424 7265  ...items.}...$re
+0000a7d0: 6694 8c24 232f 636f 6d70 6f6e 656e 7473  f..$#/components
+0000a7e0: 2f73 6368 656d 6173 2f4a 6f62 5368 6172  /schemas/JobShar
+0000a7f0: 654c 6973 7444 544f 9473 7575 758c 0f4a  eListDTO.suuu..J
+0000a800: 6f62 5368 6172 6544 6973 706c 6179 947d  obShareDisplay.}
+0000a810: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
+0000a820: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
+0000a830: 948c 076d 6573 7361 6765 947d 948c 0474  ...message.}...t
+0000a840: 7970 6594 8c06 7374 7269 6e67 9473 7375  ype...string.ssu
+0000a850: 8c0c 5265 7370 5368 6172 654a 6f62 947d  ..RespShareJob.}
+0000a860: 9428 8c04 7479 7065 948c 066f 626a 6563  .(..type...objec
+0000a870: 7494 8c0a 7072 6f70 6572 7469 6573 947d  t...properties.}
+0000a880: 9428 8c06 7374 6174 7573 947d 948c 0474  .(..status.}...t
+0000a890: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
+0000a8a0: 6d65 7373 6167 6594 7d94 8c04 7479 7065  message.}...type
+0000a8b0: 948c 0673 7472 696e 6794 738c 0776 6572  ...string.s..ver
+0000a8c0: 7369 6f6e 947d 948c 0474 7970 6594 8c06  sion.}...type...
+0000a8d0: 7374 7269 6e67 9473 8c06 636f 6d6d 6974  string.s..commit
+0000a8e0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000a8f0: 6e67 9473 8c05 6275 696c 6494 7d94 8c04  ng.s..build.}...
+0000a900: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000a910: 086d 6574 6164 6174 6194 7d94 8c04 2472  .metadata.}...$r
+0000a920: 6566 948c 2323 2f63 6f6d 706f 6e65 6e74  ef..##/component
+0000a930: 732f 7363 6865 6d61 732f 5265 7375 6c74  s/schemas/Result
+0000a940: 4d65 7461 6461 7461 9473 8c06 7265 7375  Metadata.s..resu
+0000a950: 6c74 947d 948c 0424 7265 6694 8c24 232f  lt.}...$ref..$#/
+0000a960: 636f 6d70 6f6e 656e 7473 2f73 6368 656d  components/schem
+0000a970: 6173 2f4a 6f62 5368 6172 6544 6973 706c  as/JobShareDispl
+0000a980: 6179 9473 7575 8c0b 5265 7153 6861 7265  ay.suu..ReqShare
+0000a990: 4a6f 6294 7d94 288c 0474 7970 6594 8c06  Job.}.(..type...
+0000a9a0: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
+0000a9b0: 6965 7394 7d94 288c 0767 7261 6e74 6565  ies.}.(..grantee
+0000a9c0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000a9d0: 6e67 9473 8c0b 6a6f 6252 6573 6f75 7263  ng.s..jobResourc
+0000a9e0: 6594 7d94 288c 0474 7970 6594 8c05 6172  e.}.(..type...ar
+0000a9f0: 7261 7994 8c05 6974 656d 7394 7d94 288c  ray...items.}.(.
+0000aa00: 0474 7970 6594 8c06 7374 7269 6e67 948c  .type...string..
+0000aa10: 0465 6e75 6d94 5d94 288c 0b4a 4f42 5f48  .enum.].(..JOB_H
+0000aa20: 4953 544f 5259 948c 144a 4f42 5f52 4553  ISTORY...JOB_RES
+0000aa30: 5542 4d49 545f 5245 5155 4553 5494 8c0a  UBMIT_REQUEST...
+0000aa40: 4a4f 425f 4f55 5450 5554 948c 094a 4f42  JOB_OUTPUT...JOB
+0000aa50: 5f49 4e50 5554 9465 7575 8c0d 6a6f 6250  _INPUT.euu..jobP
+0000aa60: 6572 6d69 7373 696f 6e94 7d94 288c 0474  ermission.}.(..t
+0000aa70: 7970 6594 8c06 7374 7269 6e67 948c 0465  ype...string...e
+0000aa80: 6e75 6d94 5d94 8c04 5245 4144 9461 7575  num.]...READ.auu
+0000aa90: 758c 104a 6f62 5374 6174 7573 4469 7370  u..JobStatusDisp
+0000aaa0: 6c61 7994 7d94 288c 0474 7970 6594 8c06  lay.}.(..type...
+0000aab0: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
+0000aac0: 6965 7394 7d94 8c06 7374 6174 7573 947d  ies.}...status.}
+0000aad0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000aae0: 9473 7375 8c10 5265 7370 4765 744a 6f62  .ssu..RespGetJob
+0000aaf0: 5374 6174 7573 947d 9428 8c04 7479 7065  Status.}.(..type
+0000ab00: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
+0000ab10: 6572 7469 6573 947d 9428 8c06 7374 6174  erties.}.(..stat
+0000ab20: 7573 947d 948c 0474 7970 6594 8c06 7374  us.}...type...st
+0000ab30: 7269 6e67 9473 8c07 6d65 7373 6167 6594  ring.s..message.
+0000ab40: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000ab50: 6794 738c 0776 6572 7369 6f6e 947d 948c  g.s..version.}..
+0000ab60: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000ab70: 8c06 636f 6d6d 6974 947d 948c 0474 7970  ..commit.}...typ
+0000ab80: 6594 8c06 7374 7269 6e67 9473 8c05 6275  e...string.s..bu
+0000ab90: 696c 6494 7d94 8c04 7479 7065 948c 0673  ild.}...type...s
+0000aba0: 7472 696e 6794 738c 086d 6574 6164 6174  tring.s..metadat
+0000abb0: 6194 7d94 8c04 2472 6566 948c 2323 2f63  a.}...$ref..##/c
+0000abc0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+0000abd0: 732f 5265 7375 6c74 4d65 7461 6461 7461  s/ResultMetadata
+0000abe0: 9473 8c06 7265 7375 6c74 947d 948c 0424  .s..result.}...$
+0000abf0: 7265 6694 8c25 232f 636f 6d70 6f6e 656e  ref..%#/componen
+0000ac00: 7473 2f73 6368 656d 6173 2f4a 6f62 5374  ts/schemas/JobSt
+0000ac10: 6174 7573 4469 7370 6c61 7994 7375 758c  atusDisplay.suu.
+0000ac20: 1449 6e63 6c75 6465 4578 636c 7564 6546  .IncludeExcludeF
+0000ac30: 696c 7465 7294 7d94 288c 0474 7970 6594  ilter.}.(..type.
+0000ac40: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
+0000ac50: 7274 6965 7394 7d94 288c 0869 6e63 6c75  rties.}.(..inclu
+0000ac60: 6465 7394 7d94 288c 0474 7970 6594 8c05  des.}.(..type...
+0000ac70: 6172 7261 7994 8c05 6974 656d 7394 7d94  array...items.}.
+0000ac80: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000ac90: 7375 8c08 6578 636c 7564 6573 947d 9428  su..excludes.}.(
+0000aca0: 8c04 7479 7065 948c 0561 7272 6179 948c  ..type...array..
+0000acb0: 0569 7465 6d73 947d 948c 0474 7970 6594  .items.}...type.
+0000acc0: 8c06 7374 7269 6e67 9473 758c 1269 6e63  ..string.su..inc
+0000acd0: 6c75 6465 4c61 756e 6368 4669 6c65 7394  ludeLaunchFiles.
+0000ace0: 7d94 8c04 7479 7065 948c 0762 6f6f 6c65  }...type...boole
+0000acf0: 616e 9473 7575 8c0a 4a6f 6241 7267 5370  an.suu..JobArgSp
+0000ad00: 6563 947d 9428 8c04 7479 7065 948c 066f  ec.}.(..type...o
+0000ad10: 626a 6563 7494 8c0a 7072 6f70 6572 7469  bject...properti
+0000ad20: 6573 947d 9428 8c04 6e61 6d65 947d 948c  es.}.(..name.}..
+0000ad30: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000ad40: 8c0b 6465 7363 7269 7074 696f 6e94 7d94  ..description.}.
+0000ad50: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000ad60: 738c 0769 6e63 6c75 6465 947d 948c 0474  s..include.}...t
+0000ad70: 7970 6594 8c07 626f 6f6c 6561 6e94 738c  ype...boolean.s.
+0000ad80: 0361 7267 947d 948c 0474 7970 6594 8c06  .arg.}...type...
+0000ad90: 7374 7269 6e67 9473 8c05 6e6f 7465 7394  string.s..notes.
+0000ada0: 7d94 8c04 7479 7065 948c 066f 626a 6563  }...type...objec
+0000adb0: 7494 7375 758c 0c4a 6f62 4669 6c65 496e  t.suu..JobFileIn
+0000adc0: 7075 7494 7d94 288c 0474 7970 6594 8c06  put.}.(..type...
+0000add0: 6f62 6a65 6374 948c 0a70 726f 7065 7274  object...propert
+0000ade0: 6965 7394 7d94 288c 046e 616d 6594 7d94  ies.}.(..name.}.
+0000adf0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000ae00: 738c 0b64 6573 6372 6970 7469 6f6e 947d  s..description.}
+0000ae10: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000ae20: 9473 8c0e 6175 746f 4d6f 756e 744c 6f63  .s..autoMountLoc
+0000ae30: 616c 947d 948c 0474 7970 6594 8c07 626f  al.}...type...bo
+0000ae40: 6f6c 6561 6e94 738c 0973 6f75 7263 6555  olean.s..sourceU
+0000ae50: 726c 947d 948c 0474 7970 6594 8c06 7374  rl.}...type...st
+0000ae60: 7269 6e67 9473 8c0a 7461 7267 6574 5061  ring.s..targetPa
+0000ae70: 7468 947d 948c 0474 7970 6594 8c06 7374  th.}...type...st
+0000ae80: 7269 6e67 9473 7575 8c11 4a6f 6246 696c  ring.suu..JobFil
+0000ae90: 6549 6e70 7574 4172 7261 7994 7d94 288c  eInputArray.}.(.
+0000aea0: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
+0000aeb0: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
+0000aec0: 046e 616d 6594 7d94 8c04 7479 7065 948c  .name.}...type..
+0000aed0: 0673 7472 696e 6794 738c 0b64 6573 6372  .string.s..descr
+0000aee0: 6970 7469 6f6e 947d 948c 0474 7970 6594  iption.}...type.
+0000aef0: 8c06 7374 7269 6e67 9473 8c0a 736f 7572  ..string.s..sour
+0000af00: 6365 5572 6c73 947d 9428 8c04 7479 7065  ceUrls.}.(..type
+0000af10: 948c 0561 7272 6179 948c 0569 7465 6d73  ...array...items
+0000af20: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000af30: 6e67 9473 758c 0974 6172 6765 7444 6972  ng.su..targetDir
+0000af40: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000af50: 6e67 9473 7575 8c0f 4a6f 6250 6172 616d  ng.suu..JobParam
+0000af60: 6574 6572 5365 7494 7d94 288c 0474 7970  eterSet.}.(..typ
+0000af70: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
+0000af80: 7065 7274 6965 7394 7d94 288c 0761 7070  perties.}.(..app
+0000af90: 4172 6773 947d 9428 8c04 7479 7065 948c  Args.}.(..type..
+0000afa0: 0561 7272 6179 948c 0569 7465 6d73 947d  .array...items.}
+0000afb0: 948c 0424 7265 6694 8c1f 232f 636f 6d70  ...$ref...#/comp
+0000afc0: 6f6e 656e 7473 2f73 6368 656d 6173 2f4a  onents/schemas/J
+0000afd0: 6f62 4172 6753 7065 6394 7375 8c0d 636f  obArgSpec.su..co
+0000afe0: 6e74 6169 6e65 7241 7267 7394 7d94 288c  ntainerArgs.}.(.
+0000aff0: 0474 7970 6594 8c05 6172 7261 7994 8c05  .type...array...
+0000b000: 6974 656d 7394 7d94 8c04 2472 6566 948c  items.}...$ref..
+0000b010: 1f23 2f63 6f6d 706f 6e65 6e74 732f 7363  .#/components/sc
+0000b020: 6865 6d61 732f 4a6f 6241 7267 5370 6563  hemas/JobArgSpec
+0000b030: 9473 758c 1073 6368 6564 756c 6572 4f70  .su..schedulerOp
+0000b040: 7469 6f6e 7394 7d94 288c 0474 7970 6594  tions.}.(..type.
+0000b050: 8c05 6172 7261 7994 8c05 6974 656d 7394  ..array...items.
+0000b060: 7d94 8c04 2472 6566 948c 1f23 2f63 6f6d  }...$ref...#/com
+0000b070: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+0000b080: 4a6f 6241 7267 5370 6563 9473 758c 0c65  JobArgSpec.su..e
+0000b090: 6e76 5661 7269 6162 6c65 7394 7d94 288c  nvVariables.}.(.
+0000b0a0: 0474 7970 6594 8c05 6172 7261 7994 8c05  .type...array...
+0000b0b0: 6974 656d 7394 7d94 8c04 2472 6566 948c  items.}...$ref..
+0000b0c0: 2123 2f63 6f6d 706f 6e65 6e74 732f 7363  !#/components/sc
+0000b0d0: 6865 6d61 732f 4b65 7956 616c 7565 5061  hemas/KeyValuePa
+0000b0e0: 6972 9473 758c 0d61 7263 6869 7665 4669  ir.su..archiveFi
+0000b0f0: 6c74 6572 947d 948c 0424 7265 6694 8c29  lter.}...$ref..)
+0000b100: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0000b110: 656d 6173 2f49 6e63 6c75 6465 4578 636c  emas/IncludeExcl
+0000b120: 7564 6546 696c 7465 7294 7375 758c 0c4b  udeFilter.suu..K
+0000b130: 6579 5661 6c75 6550 6169 7294 7d94 288c  eyValuePair.}.(.
+0000b140: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
+0000b150: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
+0000b160: 036b 6579 947d 948c 0474 7970 6594 8c06  .key.}...type...
+0000b170: 7374 7269 6e67 9473 8c05 7661 6c75 6594  string.s..value.
 0000b180: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000b190: 6794 738c 1161 7263 6869 7665 4f6e 4170  g.s..archiveOnAp
-0000b1a0: 7045 7272 6f72 947d 948c 0474 7970 6594  pError.}...type.
-0000b1b0: 8c07 626f 6f6c 6561 6e94 738c 1164 796e  ..boolean.s..dyn
-0000b1c0: 616d 6963 4578 6563 5379 7374 656d 947d  amicExecSystem.}
-0000b1d0: 948c 0474 7970 6594 8c07 626f 6f6c 6561  ...type...boolea
-0000b1e0: 6e94 738c 0c65 7865 6353 7973 7465 6d49  n.s..execSystemI
-0000b1f0: 6494 7d94 8c04 7479 7065 948c 0673 7472  d.}...type...str
-0000b200: 696e 6794 738c 1165 7865 6353 7973 7465  ing.s..execSyste
-0000b210: 6d45 7865 6344 6972 947d 948c 0474 7970  mExecDir.}...typ
-0000b220: 6594 8c06 7374 7269 6e67 9473 8c12 6578  e...string.s..ex
-0000b230: 6563 5379 7374 656d 496e 7075 7444 6972  ecSystemInputDir
-0000b240: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000b250: 6e67 9473 8c13 6578 6563 5379 7374 656d  ng.s..execSystem
-0000b260: 4f75 7470 7574 4469 7294 7d94 8c04 7479  OutputDir.}...ty
-0000b270: 7065 948c 0673 7472 696e 6794 738c 1665  pe...string.s..e
-0000b280: 7865 6353 7973 7465 6d4c 6f67 6963 616c  xecSystemLogical
-0000b290: 5175 6575 6594 7d94 8c04 7479 7065 948c  Queue.}...type..
-0000b2a0: 0673 7472 696e 6794 738c 0f61 7263 6869  .string.s..archi
-0000b2b0: 7665 5379 7374 656d 4964 947d 948c 0474  veSystemId.}...t
-0000b2c0: 7970 6594 8c06 7374 7269 6e67 9473 8c10  ype...string.s..
-0000b2d0: 6172 6368 6976 6553 7973 7465 6d44 6972  archiveSystemDir
-0000b2e0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000b2f0: 6e67 9473 8c09 6e6f 6465 436f 756e 7494  ng.s..nodeCount.
-0000b300: 7d94 288c 0474 7970 6594 8c07 696e 7465  }.(..type...inte
-0000b310: 6765 7294 8c06 666f 726d 6174 948c 0569  ger...format...i
-0000b320: 6e74 3332 9475 8c0c 636f 7265 7350 6572  nt32.u..coresPer
-0000b330: 4e6f 6465 947d 9428 8c04 7479 7065 948c  Node.}.(..type..
-0000b340: 0769 6e74 6567 6572 948c 0666 6f72 6d61  .integer...forma
-0000b350: 7494 8c05 696e 7433 3294 758c 086d 656d  t...int32.u..mem
-0000b360: 6f72 794d 4294 7d94 288c 0474 7970 6594  oryMB.}.(..type.
-0000b370: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
-0000b380: 6174 948c 0569 6e74 3332 9475 8c0a 6d61  at...int32.u..ma
-0000b390: 784d 696e 7574 6573 947d 9428 8c04 7479  xMinutes.}.(..ty
-0000b3a0: 7065 948c 0769 6e74 6567 6572 948c 0666  pe...integer...f
-0000b3b0: 6f72 6d61 7494 8c05 696e 7433 3294 758c  ormat...int32.u.
-0000b3c0: 0a66 696c 6549 6e70 7574 7394 7d94 288c  .fileInputs.}.(.
-0000b3d0: 0474 7970 6594 8c05 6172 7261 7994 8c05  .type...array...
-0000b3e0: 6974 656d 7394 7d94 8c04 2472 6566 948c  items.}...$ref..
-0000b3f0: 2123 2f63 6f6d 706f 6e65 6e74 732f 7363  !#/components/sc
-0000b400: 6865 6d61 732f 4a6f 6246 696c 6549 6e70  hemas/JobFileInp
-0000b410: 7574 9473 758c 0f66 696c 6549 6e70 7574  ut.su..fileInput
-0000b420: 4172 7261 7973 947d 9428 8c04 7479 7065  Arrays.}.(..type
-0000b430: 948c 0561 7272 6179 948c 0569 7465 6d73  ...array...items
-0000b440: 947d 948c 0424 7265 6694 8c26 232f 636f  .}...$ref..&#/co
-0000b450: 6d70 6f6e 656e 7473 2f73 6368 656d 6173  mponents/schemas
-0000b460: 2f4a 6f62 4669 6c65 496e 7075 7441 7272  /JobFileInputArr
-0000b470: 6179 9473 758c 0c70 6172 616d 6574 6572  ay.su..parameter
-0000b480: 5365 7494 7d94 8c04 2472 6566 948c 2423  Set.}...$ref..$#
-0000b490: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0000b4a0: 6d61 732f 4a6f 6250 6172 616d 6574 6572  mas/JobParameter
-0000b4b0: 5365 7494 738c 1565 7865 6353 7973 7465  Set.s..execSyste
-0000b4c0: 6d43 6f6e 7374 7261 696e 7473 947d 9428  mConstraints.}.(
-0000b4d0: 8c04 7479 7065 948c 0561 7272 6179 948c  ..type...array..
-0000b4e0: 0569 7465 6d73 947d 948c 0474 7970 6594  .items.}...type.
-0000b4f0: 8c06 7374 7269 6e67 9473 758c 0474 6167  ..string.su..tag
-0000b500: 7394 7d94 288c 0474 7970 6594 8c05 6172  s.}.(..type...ar
-0000b510: 7261 7994 8c05 6974 656d 7394 7d94 8c04  ray...items.}...
-0000b520: 7479 7065 948c 0673 7472 696e 6794 7375  type...string.su
-0000b530: 8c0d 7375 6273 6372 6970 7469 6f6e 7394  ..subscriptions.
-0000b540: 7d94 288c 0474 7970 6594 8c05 6172 7261  }.(..type...arra
-0000b550: 7994 8c05 6974 656d 7394 7d94 8c04 2472  y...items.}...$r
-0000b560: 6566 948c 2123 2f63 6f6d 706f 6e65 6e74  ef..!#/component
-0000b570: 732f 7363 6865 6d61 732f 5265 7153 7562  s/schemas/ReqSub
-0000b580: 7363 7269 6265 9473 758c 0569 734d 7069  scribe.su..isMpi
-0000b590: 947d 948c 0474 7970 6594 8c07 626f 6f6c  .}...type...bool
-0000b5a0: 6561 6e94 738c 066d 7069 436d 6494 7d94  ean.s..mpiCmd.}.
-0000b5b0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000b5c0: 738c 0963 6d64 5072 6566 6978 947d 948c  s..cmdPrefix.}..
-0000b5d0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000b5e0: 8c05 6e6f 7465 7394 7d94 8c04 7479 7065  ..notes.}...type
-0000b5f0: 948c 066f 626a 6563 7494 7375 758c 0c52  ...object.suu..R
-0000b600: 6571 5375 6273 6372 6962 6594 7d94 288c  eqSubscribe.}.(.
-0000b610: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
-0000b620: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
-0000b630: 0b64 6573 6372 6970 7469 6f6e 947d 948c  .description.}..
-0000b640: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000b650: 8c07 656e 6162 6c65 6494 7d94 8c04 7479  ..enabled.}...ty
-0000b660: 7065 948c 0762 6f6f 6c65 616e 9473 8c13  pe...boolean.s..
-0000b670: 6576 656e 7443 6174 6567 6f72 7946 696c  eventCategoryFil
-0000b680: 7465 7294 7d94 288c 0474 7970 6594 8c06  ter.}.(..type...
-0000b690: 7374 7269 6e67 948c 0465 6e75 6d94 5d94  string...enum.].
-0000b6a0: 288c 0e4a 4f42 5f4e 4557 5f53 5441 5455  (..JOB_NEW_STATU
-0000b6b0: 5394 8c18 4a4f 425f 494e 5055 545f 5452  S...JOB_INPUT_TR
-0000b6c0: 414e 5341 4354 494f 4e5f 4944 948c 1a4a  ANSACTION_ID...J
-0000b6d0: 4f42 5f41 5243 4849 5645 5f54 5241 4e53  OB_ARCHIVE_TRANS
-0000b6e0: 4143 5449 4f4e 5f49 4494 8c10 4a4f 425f  ACTION_ID...JOB_
-0000b6f0: 5355 4253 4352 4950 5449 4f4e 948c 0f4a  SUBSCRIPTION...J
-0000b700: 4f42 5f53 4841 5245 5f45 5645 4e54 948c  OB_SHARE_EVENT..
-0000b710: 114a 4f42 5f45 5252 4f52 5f4d 4553 5341  .JOB_ERROR_MESSA
-0000b720: 4745 948c 0e4a 4f42 5f55 5345 525f 4556  GE...JOB_USER_EV
-0000b730: 454e 5494 8c03 414c 4c94 6575 8c0f 6465  ENT...ALL.eu..de
-0000b740: 6c69 7665 7279 5461 7267 6574 7394 7d94  liveryTargets.}.
-0000b750: 288c 0474 7970 6594 8c05 6172 7261 7994  (..type...array.
-0000b760: 8c05 6974 656d 7394 7d94 8c04 2472 6566  ..items.}...$ref
-0000b770: 948c 2823 2f63 6f6d 706f 6e65 6e74 732f  ..(#/components/
-0000b780: 7363 6865 6d61 732f 4e6f 7469 6644 656c  schemas/NotifDel
-0000b790: 6976 6572 7954 6172 6765 7494 7375 8c0a  iveryTarget.su..
-0000b7a0: 7474 6c6d 696e 7574 6573 947d 9428 8c04  ttlminutes.}.(..
-0000b7b0: 7479 7065 948c 0769 6e74 6567 6572 948c  type...integer..
-0000b7c0: 0666 6f72 6d61 7494 8c05 696e 7433 3294  .format...int32.
-0000b7d0: 7575 758c 0f52 6573 7047 6574 5265 7375  uuu..RespGetResu
-0000b7e0: 626d 6974 947d 9428 8c04 7479 7065 948c  bmit.}.(..type..
-0000b7f0: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
-0000b800: 7469 6573 947d 9428 8c06 7374 6174 7573  ties.}.(..status
-0000b810: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
-0000b820: 6e67 9473 8c07 6d65 7373 6167 6594 7d94  ng.s..message.}.
-0000b830: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
-0000b840: 738c 0776 6572 7369 6f6e 947d 948c 0474  s..version.}...t
-0000b850: 7970 6594 8c06 7374 7269 6e67 9473 8c06  ype...string.s..
-0000b860: 636f 6d6d 6974 947d 948c 0474 7970 6594  commit.}...type.
-0000b870: 8c06 7374 7269 6e67 9473 8c05 6275 696c  ..string.s..buil
-0000b880: 6494 7d94 8c04 7479 7065 948c 0673 7472  d.}...type...str
-0000b890: 696e 6794 738c 086d 6574 6164 6174 6194  ing.s..metadata.
-0000b8a0: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
-0000b8b0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
-0000b8c0: 5265 7375 6c74 4d65 7461 6461 7461 9473  ResultMetadata.s
-0000b8d0: 8c06 7265 7375 6c74 947d 948c 0424 7265  ..result.}...$re
-0000b8e0: 6694 8c21 232f 636f 6d70 6f6e 656e 7473  f..!#/components
-0000b8f0: 2f73 6368 656d 6173 2f52 6571 5375 626d  /schemas/ReqSubm
-0000b900: 6974 4a6f 6294 7375 758c 0d52 6573 7053  itJob.suu..RespS
-0000b910: 7562 6d69 744a 6f62 947d 9428 8c04 7479  ubmitJob.}.(..ty
-0000b920: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
-0000b930: 6f70 6572 7469 6573 947d 9428 8c06 7374  operties.}.(..st
-0000b940: 6174 7573 947d 948c 0474 7970 6594 8c06  atus.}...type...
-0000b950: 7374 7269 6e67 9473 8c07 6d65 7373 6167  string.s..messag
-0000b960: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
-0000b970: 696e 6794 738c 0776 6572 7369 6f6e 947d  ing.s..version.}
-0000b980: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000b990: 9473 8c06 636f 6d6d 6974 947d 948c 0474  .s..commit.}...t
-0000b9a0: 7970 6594 8c06 7374 7269 6e67 9473 8c05  ype...string.s..
-0000b9b0: 6275 696c 6494 7d94 8c04 7479 7065 948c  build.}...type..
-0000b9c0: 0673 7472 696e 6794 738c 086d 6574 6164  .string.s..metad
-0000b9d0: 6174 6194 7d94 8c04 2472 6566 948c 2323  ata.}...$ref..##
-0000b9e0: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0000b9f0: 6d61 732f 5265 7375 6c74 4d65 7461 6461  mas/ResultMetada
-0000ba00: 7461 9473 8c06 7265 7375 6c74 947d 948c  ta.s..result.}..
-0000ba10: 0424 7265 6694 8c18 232f 636f 6d70 6f6e  .$ref...#/compon
-0000ba20: 656e 7473 2f73 6368 656d 6173 2f4a 6f62  ents/schemas/Job
-0000ba30: 9473 7575 8c0c 5265 7155 7365 7245 7665  .suu..ReqUserEve
-0000ba40: 6e74 947d 9428 8c08 7265 7175 6972 6564  nt.}.(..required
-0000ba50: 945d 948c 0965 7665 6e74 4461 7461 9461  .]...eventData.a
-0000ba60: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
-0000ba70: 8c0a 7072 6f70 6572 7469 6573 947d 9428  ..properties.}.(
-0000ba80: 8c09 6576 656e 7444 6174 6194 7d94 8c04  ..eventData.}...
-0000ba90: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000baa0: 0b65 7665 6e74 4465 7461 696c 947d 948c  .eventDetail.}..
-0000bab0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000bac0: 7575 8c11 5265 7375 6c74 4368 616e 6765  uu..ResultChange
-0000bad0: 436f 756e 7494 7d94 288c 0474 7970 6594  Count.}.(..type.
-0000bae0: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
-0000baf0: 7274 6965 7394 7d94 8c07 6368 616e 6765  rties.}...change
-0000bb00: 7394 7d94 288c 0474 7970 6594 8c07 696e  s.}.(..type...in
-0000bb10: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
-0000bb20: 0569 6e74 3332 9475 7375 8c0e 4465 6c69  .int32.usu..Deli
-0000bb30: 7665 7279 5461 7267 6574 947d 9428 8c04  veryTarget.}.(..
-0000bb40: 7479 7065 948c 066f 626a 6563 7494 8c0a  type...object...
-0000bb50: 7072 6f70 6572 7469 6573 947d 9428 8c0e  properties.}.(..
-0000bb60: 6465 6c69 7665 7279 4d65 7468 6f64 947d  deliveryMethod.}
-0000bb70: 9428 8c04 7479 7065 948c 0673 7472 696e  .(..type...strin
-0000bb80: 6794 8c04 656e 756d 945d 9428 8c07 5745  g...enum.].(..WE
-0000bb90: 4248 4f4f 4b94 8c05 454d 4149 4c94 6575  BHOOK...EMAIL.eu
-0000bba0: 8c0f 6465 6c69 7665 7279 4164 6472 6573  ..deliveryAddres
-0000bbb0: 7394 7d94 8c04 7479 7065 948c 0673 7472  s.}...type...str
-0000bbc0: 696e 6794 7375 758c 1452 6573 7047 6574  ing.suu..RespGet
-0000bbd0: 5375 6273 6372 6970 7469 6f6e 7394 7d94  Subscriptions.}.
-0000bbe0: 288c 0474 7970 6594 8c06 6f62 6a65 6374  (..type...object
-0000bbf0: 948c 0a70 726f 7065 7274 6965 7394 7d94  ...properties.}.
-0000bc00: 288c 0673 7461 7475 7394 7d94 8c04 7479  (..status.}...ty
-0000bc10: 7065 948c 0673 7472 696e 6794 738c 076d  pe...string.s..m
-0000bc20: 6573 7361 6765 947d 948c 0474 7970 6594  essage.}...type.
-0000bc30: 8c06 7374 7269 6e67 9473 8c07 7665 7273  ..string.s..vers
-0000bc40: 696f 6e94 7d94 8c04 7479 7065 948c 0673  ion.}...type...s
-0000bc50: 7472 696e 6794 738c 0663 6f6d 6d69 7494  tring.s..commit.
-0000bc60: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
-0000bc70: 6794 738c 0562 7569 6c64 947d 948c 0474  g.s..build.}...t
-0000bc80: 7970 6594 8c06 7374 7269 6e67 9473 8c08  ype...string.s..
-0000bc90: 6d65 7461 6461 7461 947d 948c 0424 7265  metadata.}...$re
-0000bca0: 6694 8c23 232f 636f 6d70 6f6e 656e 7473  f..##/components
-0000bcb0: 2f73 6368 656d 6173 2f52 6573 756c 744d  /schemas/ResultM
-0000bcc0: 6574 6164 6174 6194 738c 0672 6573 756c  etadata.s..resul
-0000bcd0: 7494 7d94 288c 0474 7970 6594 8c05 6172  t.}.(..type...ar
-0000bce0: 7261 7994 8c05 6974 656d 7394 7d94 8c04  ray...items.}...
-0000bcf0: 2472 6566 948c 2623 2f63 6f6d 706f 6e65  $ref..&#/compone
-0000bd00: 6e74 732f 7363 6865 6d61 732f 5461 7069  nts/schemas/Tapi
-0000bd10: 7353 7562 7363 7269 7074 696f 6e94 7375  sSubscription.su
-0000bd20: 7575 8c11 5461 7069 7353 7562 7363 7269  uu..TapisSubscri
-0000bd30: 7074 696f 6e94 7d94 288c 0474 7970 6594  ption.}.(..type.
-0000bd40: 8c06 6f62 6a65 6374 948c 0a70 726f 7065  ..object...prope
-0000bd50: 7274 6965 7394 7d94 288c 0674 656e 616e  rties.}.(..tenan
-0000bd60: 7494 7d94 8c04 7479 7065 948c 0673 7472  t.}...type...str
-0000bd70: 696e 6794 738c 046e 616d 6594 7d94 8c04  ing.s..name.}...
-0000bd80: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000bd90: 0b64 6573 6372 6970 7469 6f6e 947d 948c  .description.}..
-0000bda0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000bdb0: 8c05 6f77 6e65 7294 7d94 8c04 7479 7065  ..owner.}...type
-0000bdc0: 948c 0673 7472 696e 6794 738c 0765 6e61  ...string.s..ena
-0000bdd0: 626c 6564 947d 948c 0474 7970 6594 8c07  bled.}...type...
-0000bde0: 626f 6f6c 6561 6e94 738c 0a74 7970 6546  boolean.s..typeF
-0000bdf0: 696c 7465 7294 7d94 8c04 7479 7065 948c  ilter.}...type..
-0000be00: 0673 7472 696e 6794 738c 0d73 7562 6a65  .string.s..subje
-0000be10: 6374 4669 6c74 6572 947d 948c 0474 7970  ctFilter.}...typ
-0000be20: 6594 8c06 7374 7269 6e67 9473 8c0f 6465  e...string.s..de
-0000be30: 6c69 7665 7279 5461 7267 6574 7394 7d94  liveryTargets.}.
-0000be40: 288c 0474 7970 6594 8c05 6172 7261 7994  (..type...array.
-0000be50: 8c05 6974 656d 7394 7d94 8c04 2472 6566  ..items.}...$ref
-0000be60: 948c 2323 2f63 6f6d 706f 6e65 6e74 732f  ..##/components/
-0000be70: 7363 6865 6d61 732f 4465 6c69 7665 7279  schemas/Delivery
-0000be80: 5461 7267 6574 9473 758c 0a74 746c 4d69  Target.su..ttlMi
-0000be90: 6e75 7465 7394 7d94 288c 0474 7970 6594  nutes.}.(..type.
-0000bea0: 8c07 696e 7465 6765 7294 8c06 666f 726d  ..integer...form
-0000beb0: 6174 948c 0569 6e74 3332 9475 8c04 7575  at...int32.u..uu
-0000bec0: 6964 947d 948c 0474 7970 6594 8c06 7374  id.}...type...st
-0000bed0: 7269 6e67 9473 8c06 6578 7069 7279 947d  ring.s..expiry.}
-0000bee0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
-0000bef0: 9473 8c07 6372 6561 7465 6494 7d94 8c04  .s..created.}...
-0000bf00: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000bf10: 0775 7064 6174 6564 947d 948c 0474 7970  .updated.}...typ
-0000bf20: 6594 8c06 7374 7269 6e67 9473 7575 8c0f  e...string.suu..
-0000bf30: 5265 7370 5265 736f 7572 6365 5572 6c94  RespResourceUrl.
-0000bf40: 7d94 288c 0474 7970 6594 8c06 6f62 6a65  }.(..type...obje
-0000bf50: 6374 948c 0a70 726f 7065 7274 6965 7394  ct...properties.
-0000bf60: 7d94 288c 0673 7461 7475 7394 7d94 8c04  }.(..status.}...
-0000bf70: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
-0000bf80: 076d 6573 7361 6765 947d 948c 0474 7970  .message.}...typ
-0000bf90: 6594 8c06 7374 7269 6e67 9473 8c07 7665  e...string.s..ve
-0000bfa0: 7273 696f 6e94 7d94 8c04 7479 7065 948c  rsion.}...type..
-0000bfb0: 0673 7472 696e 6794 738c 0663 6f6d 6d69  .string.s..commi
-0000bfc0: 7494 7d94 8c04 7479 7065 948c 0673 7472  t.}...type...str
-0000bfd0: 696e 6794 738c 0562 7569 6c64 947d 948c  ing.s..build.}..
-0000bfe0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
-0000bff0: 8c08 6d65 7461 6461 7461 947d 948c 0424  ..metadata.}...$
-0000c000: 7265 6694 8c23 232f 636f 6d70 6f6e 656e  ref..##/componen
-0000c010: 7473 2f73 6368 656d 6173 2f52 6573 756c  ts/schemas/Resul
-0000c020: 744d 6574 6164 6174 6194 738c 0672 6573  tMetadata.s..res
-0000c030: 756c 7494 7d94 8c04 2472 6566 948c 2623  ult.}...$ref..&#
-0000c040: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
-0000c050: 6d61 732f 5265 7375 6c74 5265 736f 7572  mas/ResultResour
-0000c060: 6365 5572 6c94 7375 758c 1152 6573 756c  ceUrl.suu..Resul
-0000c070: 7452 6573 6f75 7263 6555 726c 947d 9428  tResourceUrl.}.(
-0000c080: 8c04 7479 7065 948c 066f 626a 6563 7494  ..type...object.
-0000c090: 8c0a 7072 6f70 6572 7469 6573 947d 948c  ..properties.}..
-0000c0a0: 0375 726c 947d 948c 0474 7970 6594 8c06  .url.}...type...
-0000c0b0: 7374 7269 6e67 9473 7375 758c 0f73 6563  string.ssuu..sec
-0000c0c0: 7572 6974 7953 6368 656d 6573 947d 948c  uritySchemes.}..
-0000c0d0: 0854 6170 6973 4a57 5494 7d94 288c 0474  .TapisJWT.}.(..t
-0000c0e0: 7970 6594 8c06 6170 694b 6579 948c 0b64  ype...apiKey...d
-0000c0f0: 6573 6372 6970 7469 6f6e 948c 2554 6170  escription..%Tap
-0000c100: 6973 2073 6967 6e65 6420 4a57 5420 746f  is signed JWT to
-0000c110: 6b65 6e20 6175 7468 656e 7469 6361 7469  ken authenticati
-0000c120: 6f6e 948c 046e 616d 6594 8c0d 582d 5461  on...name...X-Ta
-0000c130: 7069 732d 546f 6b65 6e94 8c02 696e 948c  pis-Token...in..
-0000c140: 0668 6561 6465 7294 7573 7575 2e         .header.usuu.
+0000b190: 6794 738c 0b64 6573 6372 6970 7469 6f6e  g.s..description
+0000b1a0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000b1b0: 6e67 9473 7575 8c13 4e6f 7469 6644 656c  ng.suu..NotifDel
+0000b1c0: 6976 6572 7954 6172 6765 7494 7d94 288c  iveryTarget.}.(.
+0000b1d0: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
+0000b1e0: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
+0000b1f0: 0e64 656c 6976 6572 794d 6574 686f 6494  .deliveryMethod.
+0000b200: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
+0000b210: 6e67 948c 0465 6e75 6d94 5d94 288c 0757  ng...enum.].(..W
+0000b220: 4542 484f 4f4b 948c 0545 4d41 494c 948c  EBHOOK...EMAIL..
+0000b230: 0551 5545 5545 948c 0541 4354 4f52 9465  .QUEUE...ACTOR.e
+0000b240: 758c 0f64 656c 6976 6572 7941 6464 7265  u..deliveryAddre
+0000b250: 7373 947d 948c 0474 7970 6594 8c06 7374  ss.}...type...st
+0000b260: 7269 6e67 9473 7575 8c0c 5265 7153 7562  ring.suu..ReqSub
+0000b270: 6d69 744a 6f62 947d 9428 8c08 7265 7175  mitJob.}.(..requ
+0000b280: 6972 6564 945d 9428 8c05 6170 7049 6494  ired.].(..appId.
+0000b290: 8c0a 6170 7056 6572 7369 6f6e 948c 046e  ..appVersion...n
+0000b2a0: 616d 6594 658c 0474 7970 6594 8c06 6f62  ame.e..type...ob
+0000b2b0: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
+0000b2c0: 7394 7d94 288c 046e 616d 6594 7d94 8c04  s.}.(..name.}...
+0000b2d0: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000b2e0: 056f 776e 6572 947d 948c 0474 7970 6594  .owner.}...type.
+0000b2f0: 8c06 7374 7269 6e67 9473 8c06 7465 6e61  ..string.s..tena
+0000b300: 6e74 947d 948c 0474 7970 6594 8c06 7374  nt.}...type...st
+0000b310: 7269 6e67 9473 8c0b 6465 7363 7269 7074  ring.s..descript
+0000b320: 696f 6e94 7d94 8c04 7479 7065 948c 0673  ion.}...type...s
+0000b330: 7472 696e 6794 738c 0561 7070 4964 947d  tring.s..appId.}
+0000b340: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000b350: 9473 8c0a 6170 7056 6572 7369 6f6e 947d  .s..appVersion.}
+0000b360: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000b370: 9473 8c07 6a6f 6254 7970 6594 7d94 8c04  .s..jobType.}...
+0000b380: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000b390: 1161 7263 6869 7665 4f6e 4170 7045 7272  .archiveOnAppErr
+0000b3a0: 6f72 947d 948c 0474 7970 6594 8c07 626f  or.}...type...bo
+0000b3b0: 6f6c 6561 6e94 738c 1164 796e 616d 6963  olean.s..dynamic
+0000b3c0: 4578 6563 5379 7374 656d 947d 948c 0474  ExecSystem.}...t
+0000b3d0: 7970 6594 8c07 626f 6f6c 6561 6e94 738c  ype...boolean.s.
+0000b3e0: 0c65 7865 6353 7973 7465 6d49 6494 7d94  .execSystemId.}.
+0000b3f0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000b400: 738c 1165 7865 6353 7973 7465 6d45 7865  s..execSystemExe
+0000b410: 6344 6972 947d 948c 0474 7970 6594 8c06  cDir.}...type...
+0000b420: 7374 7269 6e67 9473 8c12 6578 6563 5379  string.s..execSy
+0000b430: 7374 656d 496e 7075 7444 6972 947d 948c  stemInputDir.}..
+0000b440: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000b450: 8c13 6578 6563 5379 7374 656d 4f75 7470  ..execSystemOutp
+0000b460: 7574 4469 7294 7d94 8c04 7479 7065 948c  utDir.}...type..
+0000b470: 0673 7472 696e 6794 738c 1665 7865 6353  .string.s..execS
+0000b480: 7973 7465 6d4c 6f67 6963 616c 5175 6575  ystemLogicalQueu
+0000b490: 6594 7d94 8c04 7479 7065 948c 0673 7472  e.}...type...str
+0000b4a0: 696e 6794 738c 0f61 7263 6869 7665 5379  ing.s..archiveSy
+0000b4b0: 7374 656d 4964 947d 948c 0474 7970 6594  stemId.}...type.
+0000b4c0: 8c06 7374 7269 6e67 9473 8c10 6172 6368  ..string.s..arch
+0000b4d0: 6976 6553 7973 7465 6d44 6972 947d 948c  iveSystemDir.}..
+0000b4e0: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000b4f0: 8c09 6e6f 6465 436f 756e 7494 7d94 288c  ..nodeCount.}.(.
+0000b500: 0474 7970 6594 8c07 696e 7465 6765 7294  .type...integer.
+0000b510: 8c06 666f 726d 6174 948c 0569 6e74 3332  ..format...int32
+0000b520: 9475 8c0c 636f 7265 7350 6572 4e6f 6465  .u..coresPerNode
+0000b530: 947d 9428 8c04 7479 7065 948c 0769 6e74  .}.(..type...int
+0000b540: 6567 6572 948c 0666 6f72 6d61 7494 8c05  eger...format...
+0000b550: 696e 7433 3294 758c 086d 656d 6f72 794d  int32.u..memoryM
+0000b560: 4294 7d94 288c 0474 7970 6594 8c07 696e  B.}.(..type...in
+0000b570: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
+0000b580: 0569 6e74 3332 9475 8c0a 6d61 784d 696e  .int32.u..maxMin
+0000b590: 7574 6573 947d 9428 8c04 7479 7065 948c  utes.}.(..type..
+0000b5a0: 0769 6e74 6567 6572 948c 0666 6f72 6d61  .integer...forma
+0000b5b0: 7494 8c05 696e 7433 3294 758c 0a66 696c  t...int32.u..fil
+0000b5c0: 6549 6e70 7574 7394 7d94 288c 0474 7970  eInputs.}.(..typ
+0000b5d0: 6594 8c05 6172 7261 7994 8c05 6974 656d  e...array...item
+0000b5e0: 7394 7d94 8c04 2472 6566 948c 2123 2f63  s.}...$ref..!#/c
+0000b5f0: 6f6d 706f 6e65 6e74 732f 7363 6865 6d61  omponents/schema
+0000b600: 732f 4a6f 6246 696c 6549 6e70 7574 9473  s/JobFileInput.s
+0000b610: 758c 0f66 696c 6549 6e70 7574 4172 7261  u..fileInputArra
+0000b620: 7973 947d 9428 8c04 7479 7065 948c 0561  ys.}.(..type...a
+0000b630: 7272 6179 948c 0569 7465 6d73 947d 948c  rray...items.}..
+0000b640: 0424 7265 6694 8c26 232f 636f 6d70 6f6e  .$ref..&#/compon
+0000b650: 656e 7473 2f73 6368 656d 6173 2f4a 6f62  ents/schemas/Job
+0000b660: 4669 6c65 496e 7075 7441 7272 6179 9473  FileInputArray.s
+0000b670: 758c 0c70 6172 616d 6574 6572 5365 7494  u..parameterSet.
+0000b680: 7d94 8c04 2472 6566 948c 2423 2f63 6f6d  }...$ref..$#/com
+0000b690: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+0000b6a0: 4a6f 6250 6172 616d 6574 6572 5365 7494  JobParameterSet.
+0000b6b0: 738c 1565 7865 6353 7973 7465 6d43 6f6e  s..execSystemCon
+0000b6c0: 7374 7261 696e 7473 947d 9428 8c04 7479  straints.}.(..ty
+0000b6d0: 7065 948c 0561 7272 6179 948c 0569 7465  pe...array...ite
+0000b6e0: 6d73 947d 948c 0474 7970 6594 8c06 7374  ms.}...type...st
+0000b6f0: 7269 6e67 9473 758c 0474 6167 7394 7d94  ring.su..tags.}.
+0000b700: 288c 0474 7970 6594 8c05 6172 7261 7994  (..type...array.
+0000b710: 8c05 6974 656d 7394 7d94 8c04 7479 7065  ..items.}...type
+0000b720: 948c 0673 7472 696e 6794 7375 8c0d 7375  ...string.su..su
+0000b730: 6273 6372 6970 7469 6f6e 7394 7d94 288c  bscriptions.}.(.
+0000b740: 0474 7970 6594 8c05 6172 7261 7994 8c05  .type...array...
+0000b750: 6974 656d 7394 7d94 8c04 2472 6566 948c  items.}...$ref..
+0000b760: 2123 2f63 6f6d 706f 6e65 6e74 732f 7363  !#/components/sc
+0000b770: 6865 6d61 732f 5265 7153 7562 7363 7269  hemas/ReqSubscri
+0000b780: 6265 9473 758c 0569 734d 7069 947d 948c  be.su..isMpi.}..
+0000b790: 0474 7970 6594 8c07 626f 6f6c 6561 6e94  .type...boolean.
+0000b7a0: 738c 066d 7069 436d 6494 7d94 8c04 7479  s..mpiCmd.}...ty
+0000b7b0: 7065 948c 0673 7472 696e 6794 738c 0963  pe...string.s..c
+0000b7c0: 6d64 5072 6566 6978 947d 948c 0474 7970  mdPrefix.}...typ
+0000b7d0: 6594 8c06 7374 7269 6e67 9473 8c05 6e6f  e...string.s..no
+0000b7e0: 7465 7394 7d94 8c04 7479 7065 948c 066f  tes.}...type...o
+0000b7f0: 626a 6563 7494 7375 758c 0c52 6571 5375  bject.suu..ReqSu
+0000b800: 6273 6372 6962 6594 7d94 288c 0474 7970  bscribe.}.(..typ
+0000b810: 6594 8c06 6f62 6a65 6374 948c 0a70 726f  e...object...pro
+0000b820: 7065 7274 6965 7394 7d94 288c 0b64 6573  perties.}.(..des
+0000b830: 6372 6970 7469 6f6e 947d 948c 0474 7970  cription.}...typ
+0000b840: 6594 8c06 7374 7269 6e67 9473 8c07 656e  e...string.s..en
+0000b850: 6162 6c65 6494 7d94 8c04 7479 7065 948c  abled.}...type..
+0000b860: 0762 6f6f 6c65 616e 9473 8c13 6576 656e  .boolean.s..even
+0000b870: 7443 6174 6567 6f72 7946 696c 7465 7294  tCategoryFilter.
+0000b880: 7d94 288c 0474 7970 6594 8c06 7374 7269  }.(..type...stri
+0000b890: 6e67 948c 0465 6e75 6d94 5d94 288c 0e4a  ng...enum.].(..J
+0000b8a0: 4f42 5f4e 4557 5f53 5441 5455 5394 8c18  OB_NEW_STATUS...
+0000b8b0: 4a4f 425f 494e 5055 545f 5452 414e 5341  JOB_INPUT_TRANSA
+0000b8c0: 4354 494f 4e5f 4944 948c 1a4a 4f42 5f41  CTION_ID...JOB_A
+0000b8d0: 5243 4849 5645 5f54 5241 4e53 4143 5449  RCHIVE_TRANSACTI
+0000b8e0: 4f4e 5f49 4494 8c10 4a4f 425f 5355 4253  ON_ID...JOB_SUBS
+0000b8f0: 4352 4950 5449 4f4e 948c 0f4a 4f42 5f53  CRIPTION...JOB_S
+0000b900: 4841 5245 5f45 5645 4e54 948c 114a 4f42  HARE_EVENT...JOB
+0000b910: 5f45 5252 4f52 5f4d 4553 5341 4745 948c  _ERROR_MESSAGE..
+0000b920: 0e4a 4f42 5f55 5345 525f 4556 454e 5494  .JOB_USER_EVENT.
+0000b930: 8c03 414c 4c94 6575 8c0f 6465 6c69 7665  ..ALL.eu..delive
+0000b940: 7279 5461 7267 6574 7394 7d94 288c 0474  ryTargets.}.(..t
+0000b950: 7970 6594 8c05 6172 7261 7994 8c05 6974  ype...array...it
+0000b960: 656d 7394 7d94 8c04 2472 6566 948c 2823  ems.}...$ref..(#
+0000b970: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+0000b980: 6d61 732f 4e6f 7469 6644 656c 6976 6572  mas/NotifDeliver
+0000b990: 7954 6172 6765 7494 7375 8c0a 7474 6c6d  yTarget.su..ttlm
+0000b9a0: 696e 7574 6573 947d 9428 8c04 7479 7065  inutes.}.(..type
+0000b9b0: 948c 0769 6e74 6567 6572 948c 0666 6f72  ...integer...for
+0000b9c0: 6d61 7494 8c05 696e 7433 3294 7575 758c  mat...int32.uuu.
+0000b9d0: 0f52 6573 7047 6574 5265 7375 626d 6974  .RespGetResubmit
+0000b9e0: 947d 9428 8c04 7479 7065 948c 066f 626a  .}.(..type...obj
+0000b9f0: 6563 7494 8c0a 7072 6f70 6572 7469 6573  ect...properties
+0000ba00: 947d 9428 8c06 7374 6174 7573 947d 948c  .}.(..status.}..
+0000ba10: 0474 7970 6594 8c06 7374 7269 6e67 9473  .type...string.s
+0000ba20: 8c07 6d65 7373 6167 6594 7d94 8c04 7479  ..message.}...ty
+0000ba30: 7065 948c 0673 7472 696e 6794 738c 0776  pe...string.s..v
+0000ba40: 6572 7369 6f6e 947d 948c 0474 7970 6594  ersion.}...type.
+0000ba50: 8c06 7374 7269 6e67 9473 8c06 636f 6d6d  ..string.s..comm
+0000ba60: 6974 947d 948c 0474 7970 6594 8c06 7374  it.}...type...st
+0000ba70: 7269 6e67 9473 8c05 6275 696c 6494 7d94  ring.s..build.}.
+0000ba80: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000ba90: 738c 086d 6574 6164 6174 6194 7d94 8c04  s..metadata.}...
+0000baa0: 2472 6566 948c 2323 2f63 6f6d 706f 6e65  $ref..##/compone
+0000bab0: 6e74 732f 7363 6865 6d61 732f 5265 7375  nts/schemas/Resu
+0000bac0: 6c74 4d65 7461 6461 7461 9473 8c06 7265  ltMetadata.s..re
+0000bad0: 7375 6c74 947d 948c 0424 7265 6694 8c21  sult.}...$ref..!
+0000bae0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0000baf0: 656d 6173 2f52 6571 5375 626d 6974 4a6f  emas/ReqSubmitJo
+0000bb00: 6294 7375 758c 0d52 6573 7053 7562 6d69  b.suu..RespSubmi
+0000bb10: 744a 6f62 947d 9428 8c04 7479 7065 948c  tJob.}.(..type..
+0000bb20: 066f 626a 6563 7494 8c0a 7072 6f70 6572  .object...proper
+0000bb30: 7469 6573 947d 9428 8c06 7374 6174 7573  ties.}.(..status
+0000bb40: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000bb50: 6e67 9473 8c07 6d65 7373 6167 6594 7d94  ng.s..message.}.
+0000bb60: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000bb70: 738c 0776 6572 7369 6f6e 947d 948c 0474  s..version.}...t
+0000bb80: 7970 6594 8c06 7374 7269 6e67 9473 8c06  ype...string.s..
+0000bb90: 636f 6d6d 6974 947d 948c 0474 7970 6594  commit.}...type.
+0000bba0: 8c06 7374 7269 6e67 9473 8c05 6275 696c  ..string.s..buil
+0000bbb0: 6494 7d94 8c04 7479 7065 948c 0673 7472  d.}...type...str
+0000bbc0: 696e 6794 738c 086d 6574 6164 6174 6194  ing.s..metadata.
+0000bbd0: 7d94 8c04 2472 6566 948c 2323 2f63 6f6d  }...$ref..##/com
+0000bbe0: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+0000bbf0: 5265 7375 6c74 4d65 7461 6461 7461 9473  ResultMetadata.s
+0000bc00: 8c06 7265 7375 6c74 947d 948c 0424 7265  ..result.}...$re
+0000bc10: 6694 8c18 232f 636f 6d70 6f6e 656e 7473  f...#/components
+0000bc20: 2f73 6368 656d 6173 2f4a 6f62 9473 7575  /schemas/Job.suu
+0000bc30: 8c0c 5265 7155 7365 7245 7665 6e74 947d  ..ReqUserEvent.}
+0000bc40: 9428 8c08 7265 7175 6972 6564 945d 948c  .(..required.]..
+0000bc50: 0965 7665 6e74 4461 7461 9461 8c04 7479  .eventData.a..ty
+0000bc60: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
+0000bc70: 6f70 6572 7469 6573 947d 9428 8c09 6576  operties.}.(..ev
+0000bc80: 656e 7444 6174 6194 7d94 8c04 7479 7065  entData.}...type
+0000bc90: 948c 0673 7472 696e 6794 738c 0b65 7665  ...string.s..eve
+0000bca0: 6e74 4465 7461 696c 947d 948c 0474 7970  ntDetail.}...typ
+0000bcb0: 6594 8c06 7374 7269 6e67 9473 7575 8c11  e...string.suu..
+0000bcc0: 5265 7375 6c74 4368 616e 6765 436f 756e  ResultChangeCoun
+0000bcd0: 7494 7d94 288c 0474 7970 6594 8c06 6f62  t.}.(..type...ob
+0000bce0: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
+0000bcf0: 7394 7d94 8c07 6368 616e 6765 7394 7d94  s.}...changes.}.
+0000bd00: 288c 0474 7970 6594 8c07 696e 7465 6765  (..type...intege
+0000bd10: 7294 8c06 666f 726d 6174 948c 0569 6e74  r...format...int
+0000bd20: 3332 9475 7375 8c0e 4465 6c69 7665 7279  32.usu..Delivery
+0000bd30: 5461 7267 6574 947d 9428 8c04 7479 7065  Target.}.(..type
+0000bd40: 948c 066f 626a 6563 7494 8c0a 7072 6f70  ...object...prop
+0000bd50: 6572 7469 6573 947d 9428 8c0e 6465 6c69  erties.}.(..deli
+0000bd60: 7665 7279 4d65 7468 6f64 947d 9428 8c04  veryMethod.}.(..
+0000bd70: 7479 7065 948c 0673 7472 696e 6794 8c04  type...string...
+0000bd80: 656e 756d 945d 9428 8c07 5745 4248 4f4f  enum.].(..WEBHOO
+0000bd90: 4b94 8c05 454d 4149 4c94 6575 8c0f 6465  K...EMAIL.eu..de
+0000bda0: 6c69 7665 7279 4164 6472 6573 7394 7d94  liveryAddress.}.
+0000bdb0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000bdc0: 7375 758c 1452 6573 7047 6574 5375 6273  suu..RespGetSubs
+0000bdd0: 6372 6970 7469 6f6e 7394 7d94 288c 0474  criptions.}.(..t
+0000bde0: 7970 6594 8c06 6f62 6a65 6374 948c 0a70  ype...object...p
+0000bdf0: 726f 7065 7274 6965 7394 7d94 288c 0673  roperties.}.(..s
+0000be00: 7461 7475 7394 7d94 8c04 7479 7065 948c  tatus.}...type..
+0000be10: 0673 7472 696e 6794 738c 076d 6573 7361  .string.s..messa
+0000be20: 6765 947d 948c 0474 7970 6594 8c06 7374  ge.}...type...st
+0000be30: 7269 6e67 9473 8c07 7665 7273 696f 6e94  ring.s..version.
+0000be40: 7d94 8c04 7479 7065 948c 0673 7472 696e  }...type...strin
+0000be50: 6794 738c 0663 6f6d 6d69 7494 7d94 8c04  g.s..commit.}...
+0000be60: 7479 7065 948c 0673 7472 696e 6794 738c  type...string.s.
+0000be70: 0562 7569 6c64 947d 948c 0474 7970 6594  .build.}...type.
+0000be80: 8c06 7374 7269 6e67 9473 8c08 6d65 7461  ..string.s..meta
+0000be90: 6461 7461 947d 948c 0424 7265 6694 8c23  data.}...$ref..#
+0000bea0: 232f 636f 6d70 6f6e 656e 7473 2f73 6368  #/components/sch
+0000beb0: 656d 6173 2f52 6573 756c 744d 6574 6164  emas/ResultMetad
+0000bec0: 6174 6194 738c 0672 6573 756c 7494 7d94  ata.s..result.}.
+0000bed0: 288c 0474 7970 6594 8c05 6172 7261 7994  (..type...array.
+0000bee0: 8c05 6974 656d 7394 7d94 8c04 2472 6566  ..items.}...$ref
+0000bef0: 948c 2623 2f63 6f6d 706f 6e65 6e74 732f  ..&#/components/
+0000bf00: 7363 6865 6d61 732f 5461 7069 7353 7562  schemas/TapisSub
+0000bf10: 7363 7269 7074 696f 6e94 7375 7575 8c11  scription.suuu..
+0000bf20: 5461 7069 7353 7562 7363 7269 7074 696f  TapisSubscriptio
+0000bf30: 6e94 7d94 288c 0474 7970 6594 8c06 6f62  n.}.(..type...ob
+0000bf40: 6a65 6374 948c 0a70 726f 7065 7274 6965  ject...propertie
+0000bf50: 7394 7d94 288c 0674 656e 616e 7494 7d94  s.}.(..tenant.}.
+0000bf60: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000bf70: 738c 046e 616d 6594 7d94 8c04 7479 7065  s..name.}...type
+0000bf80: 948c 0673 7472 696e 6794 738c 0b64 6573  ...string.s..des
+0000bf90: 6372 6970 7469 6f6e 947d 948c 0474 7970  cription.}...typ
+0000bfa0: 6594 8c06 7374 7269 6e67 9473 8c05 6f77  e...string.s..ow
+0000bfb0: 6e65 7294 7d94 8c04 7479 7065 948c 0673  ner.}...type...s
+0000bfc0: 7472 696e 6794 738c 0765 6e61 626c 6564  tring.s..enabled
+0000bfd0: 947d 948c 0474 7970 6594 8c07 626f 6f6c  .}...type...bool
+0000bfe0: 6561 6e94 738c 0a74 7970 6546 696c 7465  ean.s..typeFilte
+0000bff0: 7294 7d94 8c04 7479 7065 948c 0673 7472  r.}...type...str
+0000c000: 696e 6794 738c 0d73 7562 6a65 6374 4669  ing.s..subjectFi
+0000c010: 6c74 6572 947d 948c 0474 7970 6594 8c06  lter.}...type...
+0000c020: 7374 7269 6e67 9473 8c0f 6465 6c69 7665  string.s..delive
+0000c030: 7279 5461 7267 6574 7394 7d94 288c 0474  ryTargets.}.(..t
+0000c040: 7970 6594 8c05 6172 7261 7994 8c05 6974  ype...array...it
+0000c050: 656d 7394 7d94 8c04 2472 6566 948c 2323  ems.}...$ref..##
+0000c060: 2f63 6f6d 706f 6e65 6e74 732f 7363 6865  /components/sche
+0000c070: 6d61 732f 4465 6c69 7665 7279 5461 7267  mas/DeliveryTarg
+0000c080: 6574 9473 758c 0a74 746c 4d69 6e75 7465  et.su..ttlMinute
+0000c090: 7394 7d94 288c 0474 7970 6594 8c07 696e  s.}.(..type...in
+0000c0a0: 7465 6765 7294 8c06 666f 726d 6174 948c  teger...format..
+0000c0b0: 0569 6e74 3332 9475 8c04 7575 6964 947d  .int32.u..uuid.}
+0000c0c0: 948c 0474 7970 6594 8c06 7374 7269 6e67  ...type...string
+0000c0d0: 9473 8c06 6578 7069 7279 947d 948c 0474  .s..expiry.}...t
+0000c0e0: 7970 6594 8c06 7374 7269 6e67 9473 8c07  ype...string.s..
+0000c0f0: 6372 6561 7465 6494 7d94 8c04 7479 7065  created.}...type
+0000c100: 948c 0673 7472 696e 6794 738c 0775 7064  ...string.s..upd
+0000c110: 6174 6564 947d 948c 0474 7970 6594 8c06  ated.}...type...
+0000c120: 7374 7269 6e67 9473 7575 8c0f 5265 7370  string.suu..Resp
+0000c130: 5265 736f 7572 6365 5572 6c94 7d94 288c  ResourceUrl.}.(.
+0000c140: 0474 7970 6594 8c06 6f62 6a65 6374 948c  .type...object..
+0000c150: 0a70 726f 7065 7274 6965 7394 7d94 288c  .properties.}.(.
+0000c160: 0673 7461 7475 7394 7d94 8c04 7479 7065  .status.}...type
+0000c170: 948c 0673 7472 696e 6794 738c 076d 6573  ...string.s..mes
+0000c180: 7361 6765 947d 948c 0474 7970 6594 8c06  sage.}...type...
+0000c190: 7374 7269 6e67 9473 8c07 7665 7273 696f  string.s..versio
+0000c1a0: 6e94 7d94 8c04 7479 7065 948c 0673 7472  n.}...type...str
+0000c1b0: 696e 6794 738c 0663 6f6d 6d69 7494 7d94  ing.s..commit.}.
+0000c1c0: 8c04 7479 7065 948c 0673 7472 696e 6794  ..type...string.
+0000c1d0: 738c 0562 7569 6c64 947d 948c 0474 7970  s..build.}...typ
+0000c1e0: 6594 8c06 7374 7269 6e67 9473 8c08 6d65  e...string.s..me
+0000c1f0: 7461 6461 7461 947d 948c 0424 7265 6694  tadata.}...$ref.
+0000c200: 8c23 232f 636f 6d70 6f6e 656e 7473 2f73  .##/components/s
+0000c210: 6368 656d 6173 2f52 6573 756c 744d 6574  chemas/ResultMet
+0000c220: 6164 6174 6194 738c 0672 6573 756c 7494  adata.s..result.
+0000c230: 7d94 8c04 2472 6566 948c 2623 2f63 6f6d  }...$ref..&#/com
+0000c240: 706f 6e65 6e74 732f 7363 6865 6d61 732f  ponents/schemas/
+0000c250: 5265 7375 6c74 5265 736f 7572 6365 5572  ResultResourceUr
+0000c260: 6c94 7375 758c 1152 6573 756c 7452 6573  l.suu..ResultRes
+0000c270: 6f75 7263 6555 726c 947d 9428 8c04 7479  ourceUrl.}.(..ty
+0000c280: 7065 948c 066f 626a 6563 7494 8c0a 7072  pe...object...pr
+0000c290: 6f70 6572 7469 6573 947d 948c 0375 726c  operties.}...url
+0000c2a0: 947d 948c 0474 7970 6594 8c06 7374 7269  .}...type...stri
+0000c2b0: 6e67 9473 7375 758c 0f73 6563 7572 6974  ng.ssuu..securit
+0000c2c0: 7953 6368 656d 6573 947d 948c 0854 6170  ySchemes.}...Tap
+0000c2d0: 6973 4a57 5494 7d94 288c 0474 7970 6594  isJWT.}.(..type.
+0000c2e0: 8c06 6170 694b 6579 948c 0b64 6573 6372  ..apiKey...descr
+0000c2f0: 6970 7469 6f6e 948c 2554 6170 6973 2073  iption..%Tapis s
+0000c300: 6967 6e65 6420 4a57 5420 746f 6b65 6e20  igned JWT token 
+0000c310: 6175 7468 656e 7469 6361 7469 6f6e 948c  authentication..
+0000c320: 046e 616d 6594 8c0d 582d 5461 7069 732d  .name...X-Tapis-
+0000c330: 546f 6b65 6e94 8c02 696e 948c 0668 6561  Token...in...hea
+0000c340: 6465 7294 7573 7575 2e                   der.usuu.
```

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/specs/tapis-project-tapis-client-java-dev-jobs-client-src-main-resources-jobsapi.pickle` & `tapipy-1.3.4/tapipy/specs/tapis-project-tapis-client-java-dev-jobs-client-src-main-resources-jobsapi.pickle`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/tapipy/tapis.py` & `tapipy-1.3.4/tapipy/tapis.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.3.3/setup.py` & `tapipy-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'requests>=2.20.0,<3.0.0',
  'setuptools>=21.0.0',
  'six>=1.10,<2.0',
  'urllib3>=1.26.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'tapipy',
-    'version': '1.3.3',
+    'version': '1.3.4',
     'description': 'Python lib for interacting with an instance of the Tapis API Framework',
     'long_description': '# tapipy - Tapis V3 Python SDK\n\nPython library for interacting with an instance of the Tapis API Framework.\n\nThe library is automatically generated by referencing the OpenAPI spec files which  a `Tapis` object built from the OpenAPI spec files from TACC\'s Tapis services. With this functionality a user is able to authorize itself with the `Tapis` object and have a \'live\' library in order to interact with Tapis services.\n\n## Development\n\nThis project is under active development, exploring different approaches to SDK generation.\n\n## Installation\nTapipy is packaged on [pypi](https://pypi.org/project/tapipy/) and can be installed with pip.\n\n```\npip install tapipy\n```\n\n\n## Usage\nTapipy\'s Tapis object first must be initialized in order to be used.\nA basic example of logging in with a user account is below.\n\n```\n# Import the Tapis object\nfrom tapipy.tapis import Tapis\n\n# Log into you the Tapis service by providing user/pass and the base url of your tenant. For example, to interact with the tacc tenant --\nt = Tapis(base_url=\'https://tacc.tapis.io\',\n          username=\'myuser\',\n          password=\'mypass\')\n\t  \n# Get tokens that will be used for authentication function calls\nt.get_tokens()\n```\n\nNow you have a Tapis object that is authenticated and able to call Tapis service endpoints. It\'s useful to know that the Tapis object will automatically refresh it\'s token if it is deemed appropriate, so the object should stay in the good graces of Tapis indefinitely.\n\nNow in order to use the Tapis object you can reference the [Tapis Framework](https://tapis-project.github.io/live-docs/) to browse all functions. For example, if I wanted to use the SK service in order to check if a user has a specific role I would find the function on the site (which is just a better way to look at the json specs).\n\nWith the site I can see that I need to use my Tapis object, initialized as `t`, access `sk`, and then use the `hasRole` function with the required inputs as follows.\n```\nt.sk.hasRole(tenant=\'dev\', user=\'_testuser\', roleName=\'Do you have this role?\')\n```\n\n### Special Query Parameters and Headers\nFor the most part, arguments that can or should be passed to a Tapis endpoint are described in the OpenAPI \ndefinition files and recognized automatically by `tapipy`. However, due to limitations in what can be expressed\nin OpenAPI, there are some paramaters that are not defined in the definition files; for example, the search\nparameters for various endpoints.\n\nTo accommodate these cases, `tapipy` recognizes two special keyword arguments to all of its methods that\ncorrespond to Tapis API calls (i.e., all of its "operations"). They are:\n\n  * `_tapis_headers` -- dictionary-like object of header names (keys) and vales.\n  * `_tapis_query_parameters` -- dictionary-like object of query parameter names (keys) and values.\n\nUse the above two special arguments for passing headers (respectively, query parameters) that are not specified\nin the OpenAPI definition of an endpoint.\n\nFor example, I can issue a search using the following syntax:\n\n```\nt.jobs.getJobSearchList(limit=5, orderBy=\'lastUpdated(desc),name(asc)\', _tapis_query_parameters={\'key\': \'value\'})\n```\n\n# Development Docs\n## Running the tests\n\nTests resources are contained within the `test` directory. `Dockerfile-tests` is at root.\n1. Build the test docker image: `docker build -t tapis/tapipy-tests -f Dockerfile-tests .`\n2. Run these tests using the built docker image: `docker run -it --rm -e username=<dev_user> -e password=<dev_pass> tapis/tapipy-tests`\n\n\n## Important Parameters to Know\n\nThe `tapipy` package allows for spec file customization in Tapis object initialization:\n* resource_set: str \n\t* Determines which set of resource to use, master or dev, defaults to master.\n\t* Important to note that if a custom_spec_dictionary is used, it is appended to this resource_set.\n\t\t* For example, you would set master and then specify a custom specs that will be added on.\n* custom_spec_dict: {resource_name: str, resource_url: str}\n\t* Allows users to modify the base resource set urls.\n\t\t* e.g. I can specify actor as a resource name and change the url.\n\t* Also allows users to add new resources to the set.\n\t\t* e.g. I can add a new resource named "test" with a  custom url.\n\t\t* Important that know that any new specs will be downloaded and added to the cache\n\t\t\t* No need to specify download_latest_specs or update spec files.\n\t* ALLOWS LOCAL RESOURCES!\n\t\t* Specify an absolute path in the dict with `local:` prefixing it and tapipy will load in a local OpenAPI v3 yml spec file.\n\t\t* `custom_spec_dict={\'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'}`\n* download_latest_specs: bool\n\t* Allows users to re-download all specs regardless on if they already exist in the cache. Defaulted to False\n\t* This will happen every time the Tapis object is initialized, it\'s a tad slower, and can cause live updates to specs.\n\t\t* As such, be warned. There are functions to update spec files below.\n* spec_dir: str\n\t* Allows users to specify folder to save specs to. Defaults to none which uses Tapipy\'s package folder.\n\t* If you are updating specs it\'s wise to use a different folder in order to not modify the base specs.\n\nThe following is an example of some custom parameter setting. As you can see, the abaco resource will now use the spec at `URL#1`, overwriting the resource definition in the master resource set, it\'ll download it if it doesn\'t exist. The same for the longhorn resource. This means that the Tapis object will now have access to all specs in master like normal, but with a modified abaco and with a new longhorn resource. All of these are stored at the new spec_dir because I don\'t want to accidentally overwrite any base specs if I call `update_spec_cache()` later (talked about in the next section).\n```\nfrom tapipy.tapis import Tapis\n\nt = Tapis(base_url=\'https://admin.develop.tapis.io\',\n          tenant_id=\'admin\',\n          username=\'username\',\n          account_type=\'user\',\n          password=\'password\',\n          resource_set=\'admin\',\n          custom_spec_dict={\'abaco\': \'URL#1\',\n                            \'longhorn\': \'URL#2\'},\n                            \'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'},\n          spec_dir=\'/home/username/tapipy_specs\')\nt.get_tokens()\n```\n\n## Update Specs Files\n\nThe Tapipy package now uses a cache to organize spec dictionaries as pickled files and has the ability to accept custom spec files. By default Tapipy keeps a set of base spec files in the `%tapipy%/specs` folder. These specs are pre-pickled at package creation time.\n\nIn order to update all default spec files a user can use the `update_spec_cache()` function. Said function\'s definition is below. If no resources are provided the function will download all default spec urls in the RESOURCES object in `%tapipy%/tapipy/tapis.py` file.\n```\nResources = Dict[ResourceName, ResourceUrl]\nupdate_spec_cache(resources: Resources = None, spec_dir: str = None)\n```\nUsers are able to specify custom resources to download by providing their own resource dictionary. For example, providing `{\'actors\': \'URLToMyActorDictionary\'}` would update that spec.\n\nUsers can also specify here where to update the spec with the `spec_dir` variable.\n\nThe Tapis object itself also has a `update_spec_cache()` function that takes the Tapis parameters given at startup and updates the spec cache. Meaning that if the Tapis object was given a custom dictionary, the `update_spec_cache()` function would update it without the need for setting parameters.\n```\nt.update_spec_cache()\n```\n\n## Build instructions\n\nBuilding is done with poetry as follows:\n```\npip install poetry\npoetry install\n```\nThis installs `tapipy` to a virtual environment. Run a shell in this environment with:\n```\npoetry shell\n```\n\nTo install locally (not in a virtual environment):\n```\npip install poetry\npoetry build\ncd dists\npip install *.whl\n```\n\n## PyPi Push Instructions\n\n```\npoetry build\npoetry publish\n```\n\n## Archive Usage\nTODO - provide working examples, e.g., \n```\nimport tapipy\nt = tapipy.Tapis(base_url=\'http://localhost:5001\')\nreq = t.tokens.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\nt.tokens.create_token(req)\n\nimport openapi_client\nconfiguration = openapi_client.Configuration()\nconfiguration.host = \'http://localhost:5001\'\napi_instance = openapi_client.TokensApi(openapi_client.ApiClient(configuration))\n\nnew_token = openapi_client.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\n\nresp = api_instance.create_token(new_token)\njwt = resp.get(\'result\').get(\'access_token\').get(\'access_token\')\n```\n',
     'author': 'Joe Stubbs',
     'author_email': 'jstubbs@tacc.utexas.edu',
     'maintainer': 'Joe Stubbs',
     'maintainer_email': 'jstubbs@tacc.utexas.edu',
     'url': 'https://github.com/tapis-project/tapipy',
```

### Comparing `tapipy-1.3.3/PKG-INFO` & `tapipy-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapipy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python lib for interacting with an instance of the Tapis API Framework
 Home-page: https://github.com/tapis-project/tapipy
 License: BSD-4-Clause
 Author: Joe Stubbs
 Author-email: jstubbs@tacc.utexas.edu
 Maintainer: Joe Stubbs
 Maintainer-email: jstubbs@tacc.utexas.edu
```

