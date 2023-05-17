# Comparing `tmp/databricks-sdk-0.1.6.tar.gz` & `tmp/databricks-sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-sdk-0.1.6.tar", last modified: Wed May 10 18:14:10 2023, max compression
+gzip compressed data, was "databricks-sdk-0.1.7.tar", last modified: Wed May 17 15:59:05 2023, max compression
```

## Comparing `databricks-sdk-0.1.6.tar` & `databricks-sdk-0.1.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:14:10.470137 databricks-sdk-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-10 18:14:10.470137 databricks-sdk-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28605 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:14:10.458137 databricks-sdk-0.1.6/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:14:10.462137 databricks-sdk-0.1.6/databricks/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12817 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    34351 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/dbconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/dbutils.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:14:10.462137 databricks-sdk-0.1.6/databricks/sdk/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/mixins/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/mixins/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:14:10.462137 databricks-sdk-0.1.6/databricks/sdk/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/runtime/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:14:10.466137 databricks-sdk-0.1.6/databricks/sdk/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/_internal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30457 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/billing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   157480 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/catalog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   188918 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/compute.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14727 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    68249 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/iam.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    99652 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113286 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/ml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19395 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/oauth2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51501 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/pipelines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    87514 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/provisioning.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24891 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/serving.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33670 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44357 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/sharing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   140031 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/sql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43457 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/service/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/databricks/sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:14:10.470137 databricks-sdk-0.1.6/databricks_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-05-10 18:14:10.000000 databricks-sdk-0.1.6/databricks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-10 18:14:10.000000 databricks-sdk-0.1.6/databricks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:14:10.000000 databricks-sdk-0.1.6/databricks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-10 18:14:10.000000 databricks-sdk-0.1.6/databricks_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 18:14:10.000000 databricks-sdk-0.1.6/databricks_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-10 18:14:10.470137 databricks-sdk-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-10 18:13:54.000000 databricks-sdk-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:59:05.263213 databricks-sdk-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    29730 2023-05-17 15:59:05.263213 databricks-sdk-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28754 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:59:05.259213 databricks-sdk-0.1.7/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:59:05.263213 databricks-sdk-0.1.7/databricks/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12817 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/dbconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/dbutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:59:05.263213 databricks-sdk-0.1.7/databricks/sdk/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/mixins/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/mixins/dbfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:59:05.263213 databricks-sdk-0.1.7/databricks/sdk/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/runtime/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:59:05.263213 databricks-sdk-0.1.7/databricks/sdk/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/_internal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30457 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/billing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   157480 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/catalog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   188918 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/compute.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14727 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68249 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/iam.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99652 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113286 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/ml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19395 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/oauth2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51501 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/pipelines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87514 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/provisioning.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24891 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/serving.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33670 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44357 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/sharing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   140031 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/sql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43457 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/service/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/databricks/sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:59:05.263213 databricks-sdk-0.1.7/databricks_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29730 2023-05-17 15:59:05.000000 databricks-sdk-0.1.7/databricks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-17 15:59:05.000000 databricks-sdk-0.1.7/databricks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:59:05.000000 databricks-sdk-0.1.7/databricks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 15:59:05.000000 databricks-sdk-0.1.7/databricks_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 15:59:05.000000 databricks-sdk-0.1.7/databricks_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-17 15:59:05.267213 databricks-sdk-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-17 15:58:55.000000 databricks-sdk-0.1.7/setup.py
```

### Comparing `databricks-sdk-0.1.6/LICENSE` & `databricks-sdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/NOTICE` & `databricks-sdk-0.1.7/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/PKG-INFO` & `databricks-sdk-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Databricks SDK for Python (Experimental)
 Home-page: https://github.com/databricks/databricks-sdk-py
 Author: Serge Smertin
 Author-email: serge.smertin@databricks.com
 License: UNKNOWN
 Keywords: databricks sdk
 Platform: UNKNOWN
@@ -23,25 +23,26 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 # Databricks SDK for Python
 
-**Stability**: [Experimental](https://docs.databricks.com/release-notes/release-types.html)
+**Stability**: [Experimental](https://docs.databricks.com/release-notes/release-types.html) 
+| Code [examples](https://github.com/databricks/databricks-sdk-py/tree/main/examples) 
+| See also the [SDK for Go](https://github.com/databricks/databricks-sdk-go) 
+| See also the [Terraform Provider](https://github.com/databricks/terraform-provider-databricks)
+| See also cloud-specific docs ([AWS](https://docs.databricks.com/dev-tools/sdk-python.html), 
+   [Azure](https://learn.microsoft.com/en-us/azure/databricks/dev-tools/sdk-python), 
+   [GCP](https://docs.gcp.databricks.com/dev-tools/sdk-python.html)) 
 
 The Databricks SDK for Python includes functionality to accelerate development with [Python](https://www.python.org/) for the Databricks Lakehouse.
 It covers all public [Databricks REST API](https://docs.databricks.com/dev-tools/api/index.html) operations.
 The SDK's internal HTTP client is robust and handles failures on different levels by performing intelligent retries.
 
-For additional and cloud-specific documentation, you can consult the following pages:
-- [AWS Documentation](https://docs.databricks.com/dev-tools/sdk-python.html)
-- [Azure Documentation](https://learn.microsoft.com/en-us/azure/databricks/dev-tools/sdk-python)
-- [GCP Documentation](https://docs.gcp.databricks.com/dev-tools/sdk-python.html)
-
 ## Contents
 
 - [Getting started](#getting-started)
 - [Authentication](#authentication)
 - [Code examples](#code-examples)
 - [Long-running operations](#long-running-operations)
 - [Paginated responses](#paginated-responses)
@@ -391,49 +392,52 @@
 PKCE state verification. Application developers are expected to persist `RefreshableCredentials` in the webapp session
 and restore it via `RefreshableCredentials.from_dict(oauth_client, session['creds'])` helpers.
 
 Works for both AWS and Azure. Not supported for GCP at the moment.
 
 ```python
 from databricks.sdk.oauth import OAuthClient
+
 oauth_client = OAuthClient(host='<workspace-url>',
                            client_id='<oauth client ID>',
                            redirect_url=f'http://host.domain/callback',
                            scopes=['clusters'])
 
 import secrets
 from flask import Flask, render_template_string, request, redirect, url_for, session
 
 APP_NAME = 'flask-demo'
 app = Flask(APP_NAME)
 app.secret_key = secrets.token_urlsafe(32)
 
+
 @app.route('/callback')
 def callback():
-    from databricks.sdk.oauth import Consent
-    consent = Consent.from_dict(oauth_client, session['consent'])
-    session['creds'] = consent.exchange_callback_parameters(request.args).as_dict()
-    return redirect(url_for('index'))
+   from databricks.sdk.oauth import Consent
+   consent = Consent.from_dict(oauth_client, session['consent'])
+   session['creds'] = consent.exchange_callback_parameters(request.args).as_dict()
+   return redirect(url_for('index'))
+
 
 @app.route('/')
 def index():
-    if 'creds' not in session:
-        consent = oauth_client.initiate_consent()
-        session['consent'] = consent.as_dict()
-        return redirect(consent.auth_url)
-
-    from databricks.sdk import WorkspaceClient
-    from databricks.sdk.oauth import RefreshableCredentials
-
-    credentials_provider = RefreshableCredentials.from_dict(oauth_client, session['creds'])
-    workspace_client = WorkspaceClient(host=oauth_client.host,
-                                       product=APP_NAME,
-                                       credentials_provider=credentials_provider)
+   if 'creds' not in session:
+      consent = oauth_client.initiate_consent()
+      session['consent'] = consent.as_dict()
+      return redirect(consent.auth_url)
+
+   from databricks.sdk import WorkspaceClient
+   from databricks.sdk.oauth import SessionCredentials
+
+   credentials_provider = SessionCredentials.from_dict(oauth_client, session['creds'])
+   workspace_client = WorkspaceClient(host=oauth_client.host,
+                                      product=APP_NAME,
+                                      credentials_provider=credentials_provider)
 
-    return render_template_string('...', w=workspace_client)
+   return render_template_string('...', w=workspace_client)
 ```
 
 ### SSO for local scripts on development machines
 
 For applications, that do run on developer workstations, Databricks SDK for Python provides `auth_type='external-browser'`
 utility, that opens up a browser for a user to go through SSO flow. Azure support is still in the early experimental
 stage.
```

### Comparing `databricks-sdk-0.1.6/README.md` & `databricks-sdk-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Databricks SDK for Python
 
-**Stability**: [Experimental](https://docs.databricks.com/release-notes/release-types.html)
+**Stability**: [Experimental](https://docs.databricks.com/release-notes/release-types.html) 
+| Code [examples](https://github.com/databricks/databricks-sdk-py/tree/main/examples) 
+| See also the [SDK for Go](https://github.com/databricks/databricks-sdk-go) 
+| See also the [Terraform Provider](https://github.com/databricks/terraform-provider-databricks)
+| See also cloud-specific docs ([AWS](https://docs.databricks.com/dev-tools/sdk-python.html), 
+   [Azure](https://learn.microsoft.com/en-us/azure/databricks/dev-tools/sdk-python), 
+   [GCP](https://docs.gcp.databricks.com/dev-tools/sdk-python.html)) 
 
 The Databricks SDK for Python includes functionality to accelerate development with [Python](https://www.python.org/) for the Databricks Lakehouse.
 It covers all public [Databricks REST API](https://docs.databricks.com/dev-tools/api/index.html) operations.
 The SDK's internal HTTP client is robust and handles failures on different levels by performing intelligent retries.
 
-For additional and cloud-specific documentation, you can consult the following pages:
-- [AWS Documentation](https://docs.databricks.com/dev-tools/sdk-python.html)
-- [Azure Documentation](https://learn.microsoft.com/en-us/azure/databricks/dev-tools/sdk-python)
-- [GCP Documentation](https://docs.gcp.databricks.com/dev-tools/sdk-python.html)
-
 ## Contents
 
 - [Getting started](#getting-started)
 - [Authentication](#authentication)
 - [Code examples](#code-examples)
 - [Long-running operations](#long-running-operations)
 - [Paginated responses](#paginated-responses)
@@ -364,49 +365,52 @@
 PKCE state verification. Application developers are expected to persist `RefreshableCredentials` in the webapp session
 and restore it via `RefreshableCredentials.from_dict(oauth_client, session['creds'])` helpers.
 
 Works for both AWS and Azure. Not supported for GCP at the moment.
 
 ```python
 from databricks.sdk.oauth import OAuthClient
+
 oauth_client = OAuthClient(host='<workspace-url>',
                            client_id='<oauth client ID>',
                            redirect_url=f'http://host.domain/callback',
                            scopes=['clusters'])
 
 import secrets
 from flask import Flask, render_template_string, request, redirect, url_for, session
 
 APP_NAME = 'flask-demo'
 app = Flask(APP_NAME)
 app.secret_key = secrets.token_urlsafe(32)
 
+
 @app.route('/callback')
 def callback():
-    from databricks.sdk.oauth import Consent
-    consent = Consent.from_dict(oauth_client, session['consent'])
-    session['creds'] = consent.exchange_callback_parameters(request.args).as_dict()
-    return redirect(url_for('index'))
+   from databricks.sdk.oauth import Consent
+   consent = Consent.from_dict(oauth_client, session['consent'])
+   session['creds'] = consent.exchange_callback_parameters(request.args).as_dict()
+   return redirect(url_for('index'))
+
 
 @app.route('/')
 def index():
-    if 'creds' not in session:
-        consent = oauth_client.initiate_consent()
-        session['consent'] = consent.as_dict()
-        return redirect(consent.auth_url)
-
-    from databricks.sdk import WorkspaceClient
-    from databricks.sdk.oauth import RefreshableCredentials
-
-    credentials_provider = RefreshableCredentials.from_dict(oauth_client, session['creds'])
-    workspace_client = WorkspaceClient(host=oauth_client.host,
-                                       product=APP_NAME,
-                                       credentials_provider=credentials_provider)
+   if 'creds' not in session:
+      consent = oauth_client.initiate_consent()
+      session['consent'] = consent.as_dict()
+      return redirect(consent.auth_url)
+
+   from databricks.sdk import WorkspaceClient
+   from databricks.sdk.oauth import SessionCredentials
+
+   credentials_provider = SessionCredentials.from_dict(oauth_client, session['creds'])
+   workspace_client = WorkspaceClient(host=oauth_client.host,
+                                      product=APP_NAME,
+                                      credentials_provider=credentials_provider)
 
-    return render_template_string('...', w=workspace_client)
+   return render_template_string('...', w=workspace_client)
 ```
 
 ### SSO for local scripts on development machines
 
 For applications, that do run on developer workstations, Databricks SDK for Python provides `auth_type='external-browser'`
 utility, that opens up a browser for a user to go through SSO flow. Azure support is still in the early experimental
 stage.
```

### Comparing `databricks-sdk-0.1.6/databricks/sdk/__init__.py` & `databricks-sdk-0.1.7/databricks/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/azure.py` & `databricks-sdk-0.1.7/databricks/sdk/azure.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/core.py` & `databricks-sdk-0.1.7/databricks/sdk/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 import json
 import logging
 import os
 import pathlib
 import platform
 import re
 import subprocess
+import sys
 import urllib.parse
 from datetime import datetime
 from json import JSONDecodeError
 from typing import Callable, Dict, Iterable, List, Optional
 
 import requests
 import requests.auth
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from .azure import ARM_DATABRICKS_RESOURCE_ID, ENVIRONMENTS, AzureEnvironment
 from .oauth import (ClientCredentials, OAuthClient, OidcEndpoints, Refreshable,
-                    Token, TokenSource)
+                    Token, TokenCache, TokenSource)
 from .version import __version__
 
 __all__ = ['Config', 'DatabricksError']
 
 logger = logging.getLogger('databricks.sdk')
 
 HeaderFactory = Callable[[], Dict[str, str]]
@@ -83,14 +84,25 @@
 
     def inner() -> Dict[str, str]:
         return static_credentials
 
     return inner
 
 
+@credentials_provider('runtime', [])
+def runtime_native_auth(cfg: 'Config') -> Optional[HeaderFactory]:
+    from databricks.sdk.runtime import init_runtime_native_auth
+    try:
+        host, inner = init_runtime_native_auth()
+        cfg.host = host
+        return inner
+    except NotImplementedError:
+        return None
+
+
 @credentials_provider('oauth-m2m', ['is_aws', 'host', 'client_id', 'client_secret'])
 def oauth_service_principal(cfg: 'Config') -> Optional[HeaderFactory]:
     """ Adds refreshed Databricks machine-to-machine OAuth Bearer token to every request,
     if /oidc/.well-known/oauth-authorization-server is available on the given host. """
     # TODO: change to use cfg.oidc_endpoints (and add cache there)
     # TODO: Azure returns 404 for UC workspace after redirecting to
     # https://login.microsoftonline.com/{cfg.azure_tenant_id}/.well-known/oauth-authorization-server
@@ -125,18 +137,28 @@
         client_id = '6128a518-99a9-425b-8333-4cc94f04cacd'
     else:
         raise ValueError(f'local browser SSO is not supported')
     oauth_client = OAuthClient(host=cfg.host,
                                client_id=client_id,
                                redirect_url='http://localhost:8020',
                                client_secret=cfg.client_secret)
-    consent = oauth_client.initiate_consent()
-    if not consent:
-        return None
-    credentials = consent.launch_external_browser()
+
+    # Load cached credentials from disk if they exist.
+    # Note that these are local to the Python SDK and not reused by other SDKs.
+    token_cache = TokenCache(oauth_client)
+    credentials = token_cache.load()
+    if credentials:
+        # Force a refresh in case the loaded credentials are expired.
+        credentials.token()
+    else:
+        consent = oauth_client.initiate_consent()
+        if not consent:
+            return None
+        credentials = consent.launch_external_browser()
+    token_cache.save(credentials)
     return credentials(cfg)
 
 
 def _ensure_host_present(cfg: 'Config', token_source_for: Callable[[str], TokenSource]):
     """ Resolves Azure Databricks workspace URL from ARM Resource ID """
     if cfg.host:
         return
@@ -199,15 +221,18 @@
             except ValueError as e:
                 last_e = e
         if last_e:
             raise last_e
 
     def refresh(self) -> Token:
         try:
-            out = subprocess.check_output(self._cmd, stderr=subprocess.STDOUT)
+            is_windows = sys.platform.startswith('win')
+            # windows requires shell=True to be able to execute 'az login' or other commands
+            # cannot use shell=True all the time, as it breaks macOS
+            out = subprocess.check_output(self._cmd, stderr=subprocess.STDOUT, shell=is_windows)
             it = json.loads(out.decode())
             expires_on = self._parse_expiry(it[self._expiry_field])
             return Token(access_token=it[self._access_token_field],
                          token_type=it[self._token_type_field],
                          expiry=expires_on)
         except ValueError as e:
             raise ValueError(f"cannot unmarshal CLI result: {e}")
@@ -295,15 +320,15 @@
 
     def auth_type(self) -> str:
         return self._auth_type
 
     def __call__(self, cfg: 'Config') -> HeaderFactory:
         auth_providers = [
             pat_auth, basic_auth, oauth_service_principal, azure_service_principal, azure_cli,
-            external_browser, bricks_cli
+            external_browser, bricks_cli, runtime_native_auth
         ]
         for provider in auth_providers:
             auth_type = provider.auth_type()
             if cfg.auth_type and auth_type != cfg.auth_type:
                 # ignore other auth types if one is explicitly enforced
                 logger.debug(f"Ignoring {auth_type} auth, because {cfg.auth_type} is preferred")
                 continue
@@ -703,33 +728,34 @@
             message = f"{scimType} {message}".strip(" ")
             error_code = f"SCIM_{status}"
         super().__init__(message if message else error)
         self.error_code = error_code
         self.kwargs = kwargs
 
 
-class ApiClient(requests.Session):
+class ApiClient:
     _cfg: Config
 
     def __init__(self, cfg: Config = None):
-        super().__init__()
         self._cfg = Config() if not cfg else cfg
+        self._debug_truncate_bytes = cfg.debug_truncate_bytes if cfg.debug_truncate_bytes else 96
+        self._user_agent_base = cfg.user_agent
+
         retry_strategy = Retry(
             total=6,
             backoff_factor=1,
             status_forcelist=[429],
             allowed_methods={"POST"} | set(Retry.DEFAULT_ALLOWED_METHODS),
             respect_retry_after_header=True,
             raise_on_status=False, # return original response when retries have been exhausted
         )
-        self._debug_truncate_bytes = cfg.debug_truncate_bytes if cfg.debug_truncate_bytes else 96
-        self._user_agent_base = cfg.user_agent
-        self.auth = self._authenticate
 
-        self.mount("https://", HTTPAdapter(max_retries=retry_strategy))
+        self._session = requests.Session()
+        self._session.auth = self._authenticate
+        self._session.mount("https://", HTTPAdapter(max_retries=retry_strategy))
 
     @property
     def account_id(self) -> str:
         return self._cfg.account_id
 
     @property
     def is_account_client(self) -> bool:
@@ -739,15 +765,19 @@
         headers = self._cfg.authenticate()
         for k, v in headers.items():
             r.headers[k] = v
         return r
 
     def do(self, method: str, path: str, query: dict = None, body: dict = None) -> dict:
         headers = {'Accept': 'application/json', 'User-Agent': self._user_agent_base}
-        response = self.request(method, f"{self._cfg.host}{path}", params=query, json=body, headers=headers)
+        response = self._session.request(method,
+                                         f"{self._cfg.host}{path}",
+                                         params=query,
+                                         json=body,
+                                         headers=headers)
         try:
             self._record_request_log(response)
             if not response.ok:
                 # TODO: experiment with traceback pruning for better readability
                 # See https://stackoverflow.com/a/58821552/277035
                 payload = response.json()
                 raise self._make_nicer_error(status_code=response.status_code, **payload) from None
```

### Comparing `databricks-sdk-0.1.6/databricks/sdk/dbconnect.py` & `databricks-sdk-0.1.7/databricks/sdk/dbconnect.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/dbutils.py` & `databricks-sdk-0.1.7/databricks/sdk/dbutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import base64
 import json
+import logging
 import threading
 import typing
 from collections import namedtuple
 
-from .core import ApiClient, Config
+from .core import ApiClient, Config, DatabricksError
 from .mixins import compute as compute_ext
 from .mixins import dbfs as dbfs_ext
 from .service import compute, workspace
 
+_LOG = logging.getLogger('databricks.sdk')
+
 
 class FileInfo(namedtuple('FileInfo', ['path', 'name', 'size', "modificationTime"])):
     pass
 
 
 class MountInfo(namedtuple('MountInfo', ['mountPoint', 'source', 'encryptionType'])):
     pass
@@ -73,46 +76,50 @@
     def rm(self, dir: str, recurse: bool = False) -> bool:
         """Removes a file or directory """
         self._dbfs.delete(dir, recursive=recurse)
         return True
 
     def mount(self,
               source: str,
-              mountPoint: str,
-              encryptionType: str = "",
-              owner: str = "",
-              extraConfigs: 'typing.Dict[str, str]' = None,
-              ) -> bool:
+              mount_point: str,
+              encryption_type: str = None,
+              owner: str = None,
+              extra_configs: 'typing.Dict[str, str]' = None) -> bool:
         """Mounts the given source directory into DBFS at the given mount point"""
         fs = self._proxy_factory('fs')
-        return fs.mount(source=source,
-                        mountPoint=mountPoint,
-                        encryptionType=encryptionType,
-                        owner=owner,
-                        extraConfigs=extraConfigs)
+        kwargs = {}
+        if encryption_type:
+            kwargs['encryption_type'] = encryption_type
+        if owner:
+            kwargs['owner'] = owner
+        if extra_configs:
+            kwargs['extra_configs'] = extra_configs
+        return fs.mount(source, mount_point, **kwargs)
 
-    def unmount(self, mountPoint: str) -> bool:
+    def unmount(self, mount_point: str) -> bool:
         """Deletes a DBFS mount point"""
         fs = self._proxy_factory('fs')
-        return fs.unmount(mountPoint)
+        return fs.unmount(mount_point)
 
     def updateMount(self,
                     source: str,
-                    mountPoint: str,
-                    encryptionType: str = "",
-                    owner: str = "",
-                    extraConfigs: 'typing.Dict[str, str]' = None,
-                    ) -> bool:
+                    mount_point: str,
+                    encryption_type: str = None,
+                    owner: str = None,
+                    extra_configs: 'typing.Dict[str, str]' = None) -> bool:
         """ Similar to mount(), but updates an existing mount point (if present) instead of creating a new one """
         fs = self._proxy_factory('fs')
-        return fs.updateMount(source=source,
-                              mountPoint=mountPoint,
-                              encryptionType=encryptionType,
-                              owner=owner,
-                              extraConfigs=extraConfigs)
+        kwargs = {}
+        if encryption_type:
+            kwargs['encryption_type'] = encryption_type
+        if owner:
+            kwargs['owner'] = owner
+        if extra_configs:
+            kwargs['extra_configs'] = extra_configs
+        return fs.updateMount(source, mount_point, **kwargs)
 
     def mounts(self) -> typing.List[MountInfo]:
         """ Displays information about what is mounted within DBFS """
         result = []
         fs = self._proxy_factory('fs')
         for info in fs.mounts():
             result.append(MountInfo(info[0], info[1], info[2]))
@@ -210,36 +217,87 @@
         return _ProxyCall(command_execution=self._commands,
                           cluster_id=self._cluster_id,
                           context_factory=self._context_factory,
                           util=self._name,
                           method=method)
 
 
+import html
+import re
+
+
 class _ProxyCall:
 
     def __init__(self, *, command_execution: compute.CommandExecutionAPI,
                  context_factory: typing.Callable[[], compute.ContextStatusResponse], cluster_id: str,
                  util: str, method: str):
         self._commands = command_execution
         self._cluster_id = cluster_id
         self._context_factory = context_factory
         self._util = util
         self._method = method
 
+    _out_re = re.compile(r'Out\[[\d\s]+]:\s')
+    _tag_re = re.compile(r'<[^>]*>')
+    _exception_re = re.compile(r'.*Exception:\s+(.*)')
+    _execution_error_re = re.compile(
+        r'ExecutionError: ([\s\S]*)\n(StatusCode=[0-9]*)\n(StatusDescription=.*)\n')
+    _error_message_re = re.compile(r'ErrorMessage=(.+)\n')
+    _ascii_escape_re = re.compile(r'(\x9B|\x1B\[)[0-?]*[ -/]*[@-~]')
+
+    def _is_failed(self, results: compute.Results) -> bool:
+        return results.result_type == compute.ResultType.error
+
+    def _text(self, results: compute.Results) -> str:
+        if results.result_type != compute.ResultType.text:
+            return ''
+        return self._out_re.sub("", str(results.data))
+
+    def _raise_if_failed(self, results: compute.Results):
+        if not self._is_failed(results):
+            return
+        raise DatabricksError(self._error_from_results(results))
+
+    def _error_from_results(self, results: compute.Results):
+        if not self._is_failed(results):
+            return
+        if results.cause:
+            _LOG.debug(f'{self._ascii_escape_re.sub("", results.cause)}')
+
+        summary = self._tag_re.sub("", results.summary)
+        summary = html.unescape(summary)
+
+        exception_matches = self._exception_re.findall(summary)
+        if len(exception_matches) == 1:
+            summary = exception_matches[0].replace("; nested exception is:", "")
+            summary = summary.rstrip(" ")
+            return summary
+
+        execution_error_matches = self._execution_error_re.findall(results.cause)
+        if len(execution_error_matches) == 1:
+            return "\n".join(execution_error_matches[0])
+
+        error_message_matches = self._error_message_re.findall(results.cause)
+        if len(error_message_matches) == 1:
+            return error_message_matches[0]
+
+        return summary
+
     def __call__(self, *args, **kwargs):
         raw = json.dumps((args, kwargs))
         code = f'''
         import json
         (args, kwargs) = json.loads('{raw}')
         result = dbutils.{self._util}.{self._method}(*args, **kwargs)
         dbutils.notebook.exit(json.dumps(result))
         '''
         ctx = self._context_factory()
         result = self._commands.execute(cluster_id=self._cluster_id,
                                         language=compute.Language.python,
                                         context_id=ctx.id,
                                         command=code).result()
         if result.status == compute.CommandStatus.Finished:
+            self._raise_if_failed(result.results)
             raw = result.results.data
             return json.loads(raw)
         else:
             raise Exception(result.results.summary)
```

### Comparing `databricks-sdk-0.1.6/databricks/sdk/mixins/compute.py` & `databricks-sdk-0.1.7/databricks/sdk/mixins/compute.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/mixins/dbfs.py` & `databricks-sdk-0.1.7/databricks/sdk/mixins/dbfs.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/oauth.py` & `databricks-sdk-0.1.7/databricks/sdk/oauth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 import base64
 import functools
 import hashlib
+import json
 import logging
+import os
 import secrets
 import threading
 import urllib.parse
 import webbrowser
 from abc import abstractmethod
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from http.server import BaseHTTPRequestHandler, HTTPServer
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 import requests
 import requests.auth
 
 # Error code for PKCE flow in Azure Active Directory, that gets additional retry.
 # See https://stackoverflow.com/a/75466778/277035 for more info
 NO_ORIGIN_FOR_SPA_CLIENT_ERROR = 'AADSTS9002327'
 
 logger = logging.getLogger(__name__)
 
 
+class IgnoreNetrcAuth(requests.auth.AuthBase):
+    """This auth method is a no-op.
+
+    We use it to force requestslib to not use .netrc to write auth headers
+    when making .post() requests to the oauth token endpoints, since these
+    don't require authentication.
+
+    In cases where .netrc is outdated or corrupt, these requests will fail.
+
+    See issue #121
+    """
+
+    def __call__(self, r):
+        return r
+
+
 @dataclass
 class OidcEndpoints:
     authorization_endpoint: str # ../v1/authorize
     token_endpoint: str # ../v1/token
 
 
 @dataclass
@@ -81,14 +99,16 @@
     logger.debug(f'Retrieving token for {client_id}')
     if use_params:
         if client_id: params["client_id"] = client_id
         if client_secret: params["client_secret"] = client_secret
     auth = None
     if use_header:
         auth = requests.auth.HTTPBasicAuth(client_id, client_secret)
+    else:
+        auth = IgnoreNetrcAuth()
     resp = requests.post(token_url, params, auth=auth, headers=headers)
     if not resp.ok:
         if resp.headers['Content-Type'].startswith('application/json'):
             err = resp.json()
             code = err.get('errorCode', err.get('error', 'unknown'))
             summary = err.get('errorSummary', err.get('error_description', 'unknown'))
             summary = summary.replace("\r\n", ' ')
@@ -153,26 +173,26 @@
         self.send_response(200)
         self.send_header('Content-type', 'text/html')
         self.end_headers()
         # TODO: show better message
         self.wfile.write(b'You can close this tab.')
 
 
-class RefreshableCredentials(Refreshable):
+class SessionCredentials(Refreshable):
 
     def __init__(self, client: 'OAuthClient', token: Token):
         self._client = client
         super().__init__(token)
 
     def as_dict(self) -> dict:
         return {'token': self._token.as_dict()}
 
     @staticmethod
-    def from_dict(client: 'OAuthClient', raw: dict) -> 'RefreshableCredentials':
-        return RefreshableCredentials(client=client, token=Token.from_dict(raw['token']))
+    def from_dict(client: 'OAuthClient', raw: dict) -> 'SessionCredentials':
+        return SessionCredentials(client=client, token=Token.from_dict(raw['token']))
 
     def auth_type(self):
         """Implementing CredentialsProvider protocol"""
         # TODO: distinguish between Databricks IDP and Azure AD
         return 'oauth'
 
     def __call__(self, *args, **kwargs):
@@ -213,15 +233,15 @@
     def as_dict(self) -> dict:
         return {'state': self._state, 'verifier': self._verifier}
 
     @staticmethod
     def from_dict(client: 'OAuthClient', raw: dict) -> 'Consent':
         return Consent(client, raw['state'], raw['verifier'])
 
-    def launch_external_browser(self) -> RefreshableCredentials:
+    def launch_external_browser(self) -> SessionCredentials:
         redirect_url = urllib.parse.urlparse(self._client.redirect_url)
         if redirect_url.hostname not in ('localhost', '127.0.0.1'):
             raise ValueError(f'cannot listen on {redirect_url.hostname}')
         feedback = []
         logger.info(f'Opening {self.auth_url} in a browser')
         webbrowser.open_new(self.auth_url)
         port = redirect_url.port
@@ -230,22 +250,22 @@
             logger.info(f'Waiting for redirect to http://localhost:{port}')
             httpd.handle_request()
         if not feedback:
             raise ValueError('No data received in callback')
         query = feedback.pop()
         return self.exchange_callback_parameters(query)
 
-    def exchange_callback_parameters(self, query: Dict[str, str]) -> RefreshableCredentials:
+    def exchange_callback_parameters(self, query: Dict[str, str]) -> SessionCredentials:
         if 'error' in query:
             raise ValueError('{error}: {error_description}'.format(**query))
         if 'code' not in query or 'state' not in query:
             raise ValueError('No code returned in callback')
         return self.exchange(query['code'], query['state'])
 
-    def exchange(self, code: str, state: str) -> RefreshableCredentials:
+    def exchange(self, code: str, state: str) -> SessionCredentials:
         if self._state != state:
             raise ValueError('state mismatch')
         params = {
             'redirect_uri': self._client.redirect_url,
             'grant_type': 'authorization_code',
             'code_verifier': self._verifier,
             'code': code
@@ -255,15 +275,15 @@
             try:
                 token = retrieve_token(client_id=self._client.client_id,
                                        client_secret=self._client.client_secret,
                                        token_url=self._client.token_url,
                                        params=params,
                                        headers=headers,
                                        use_params=True)
-                return RefreshableCredentials(self._client, token)
+                return SessionCredentials(self._client, token)
             except ValueError as e:
                 if NO_ORIGIN_FOR_SPA_CLIENT_ERROR in str(e):
                     # Retry in cases of 'Single-Page Application' client-type with
                     # 'Origin' header equal to client's redirect URL.
                     headers['Origin'] = self._client.redirect_url
                     msg = f'Retrying OAuth token exchange with {self._client.redirect_url} origin'
                     logger.debug(msg)
@@ -380,7 +400,45 @@
                 params[k] = v
         return retrieve_token(self.client_id,
                               self.client_secret,
                               self.token_url,
                               params,
                               use_params=self.use_params,
                               use_header=self.use_header)
+
+
+class TokenCache():
+    BASE_PATH = "~/.config/databricks-sdk-py/oauth"
+
+    def __init__(self, client: OAuthClient) -> None:
+        self.client = client
+
+    @property
+    def filename(self) -> str:
+        # Include host, client_id, and scopes in the cache filename to make it unique.
+        hash = hashlib.sha256()
+        for chunk in [self.client.host, self.client.client_id, ",".join(self.client._scopes), ]:
+            hash.update(chunk.encode('utf-8'))
+        return os.path.expanduser(os.path.join(self.__class__.BASE_PATH, hash.hexdigest() + ".json"))
+
+    def load(self) -> Optional[SessionCredentials]:
+        """
+        Load credentials from cache file. Return None if the cache file does not exist or is invalid.
+        """
+        if not os.path.exists(self.filename):
+            return None
+
+        try:
+            with open(self.filename, 'r') as f:
+                raw = json.load(f)
+                return SessionCredentials.from_dict(self.client, raw)
+        except Exception:
+            return None
+
+    def save(self, credentials: SessionCredentials) -> None:
+        """
+        Save credentials to cache file.
+        """
+        os.makedirs(os.path.dirname(self.filename), exist_ok=True)
+        with open(self.filename, 'w') as f:
+            json.dump(credentials.as_dict(), f)
+        os.chmod(self.filename, 0o600)
```

### Comparing `databricks-sdk-0.1.6/databricks/sdk/runtime/stub.py` & `databricks-sdk-0.1.7/databricks/sdk/runtime/stub.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/_internal.py` & `databricks-sdk-0.1.7/databricks/sdk/service/_internal.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/billing.py` & `databricks-sdk-0.1.7/databricks/sdk/service/billing.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/catalog.py` & `databricks-sdk-0.1.7/databricks/sdk/service/catalog.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/compute.py` & `databricks-sdk-0.1.7/databricks/sdk/service/compute.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/files.py` & `databricks-sdk-0.1.7/databricks/sdk/service/files.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/iam.py` & `databricks-sdk-0.1.7/databricks/sdk/service/iam.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/jobs.py` & `databricks-sdk-0.1.7/databricks/sdk/service/jobs.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/ml.py` & `databricks-sdk-0.1.7/databricks/sdk/service/ml.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/oauth2.py` & `databricks-sdk-0.1.7/databricks/sdk/service/oauth2.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/pipelines.py` & `databricks-sdk-0.1.7/databricks/sdk/service/pipelines.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/provisioning.py` & `databricks-sdk-0.1.7/databricks/sdk/service/provisioning.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/serving.py` & `databricks-sdk-0.1.7/databricks/sdk/service/serving.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/settings.py` & `databricks-sdk-0.1.7/databricks/sdk/service/settings.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/sharing.py` & `databricks-sdk-0.1.7/databricks/sdk/service/sharing.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/sql.py` & `databricks-sdk-0.1.7/databricks/sdk/service/sql.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks/sdk/service/workspace.py` & `databricks-sdk-0.1.7/databricks/sdk/service/workspace.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/databricks_sdk.egg-info/PKG-INFO` & `databricks-sdk-0.1.7/databricks_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Databricks SDK for Python (Experimental)
 Home-page: https://github.com/databricks/databricks-sdk-py
 Author: Serge Smertin
 Author-email: serge.smertin@databricks.com
 License: UNKNOWN
 Keywords: databricks sdk
 Platform: UNKNOWN
@@ -23,25 +23,26 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 # Databricks SDK for Python
 
-**Stability**: [Experimental](https://docs.databricks.com/release-notes/release-types.html)
+**Stability**: [Experimental](https://docs.databricks.com/release-notes/release-types.html) 
+| Code [examples](https://github.com/databricks/databricks-sdk-py/tree/main/examples) 
+| See also the [SDK for Go](https://github.com/databricks/databricks-sdk-go) 
+| See also the [Terraform Provider](https://github.com/databricks/terraform-provider-databricks)
+| See also cloud-specific docs ([AWS](https://docs.databricks.com/dev-tools/sdk-python.html), 
+   [Azure](https://learn.microsoft.com/en-us/azure/databricks/dev-tools/sdk-python), 
+   [GCP](https://docs.gcp.databricks.com/dev-tools/sdk-python.html)) 
 
 The Databricks SDK for Python includes functionality to accelerate development with [Python](https://www.python.org/) for the Databricks Lakehouse.
 It covers all public [Databricks REST API](https://docs.databricks.com/dev-tools/api/index.html) operations.
 The SDK's internal HTTP client is robust and handles failures on different levels by performing intelligent retries.
 
-For additional and cloud-specific documentation, you can consult the following pages:
-- [AWS Documentation](https://docs.databricks.com/dev-tools/sdk-python.html)
-- [Azure Documentation](https://learn.microsoft.com/en-us/azure/databricks/dev-tools/sdk-python)
-- [GCP Documentation](https://docs.gcp.databricks.com/dev-tools/sdk-python.html)
-
 ## Contents
 
 - [Getting started](#getting-started)
 - [Authentication](#authentication)
 - [Code examples](#code-examples)
 - [Long-running operations](#long-running-operations)
 - [Paginated responses](#paginated-responses)
@@ -391,49 +392,52 @@
 PKCE state verification. Application developers are expected to persist `RefreshableCredentials` in the webapp session
 and restore it via `RefreshableCredentials.from_dict(oauth_client, session['creds'])` helpers.
 
 Works for both AWS and Azure. Not supported for GCP at the moment.
 
 ```python
 from databricks.sdk.oauth import OAuthClient
+
 oauth_client = OAuthClient(host='<workspace-url>',
                            client_id='<oauth client ID>',
                            redirect_url=f'http://host.domain/callback',
                            scopes=['clusters'])
 
 import secrets
 from flask import Flask, render_template_string, request, redirect, url_for, session
 
 APP_NAME = 'flask-demo'
 app = Flask(APP_NAME)
 app.secret_key = secrets.token_urlsafe(32)
 
+
 @app.route('/callback')
 def callback():
-    from databricks.sdk.oauth import Consent
-    consent = Consent.from_dict(oauth_client, session['consent'])
-    session['creds'] = consent.exchange_callback_parameters(request.args).as_dict()
-    return redirect(url_for('index'))
+   from databricks.sdk.oauth import Consent
+   consent = Consent.from_dict(oauth_client, session['consent'])
+   session['creds'] = consent.exchange_callback_parameters(request.args).as_dict()
+   return redirect(url_for('index'))
+
 
 @app.route('/')
 def index():
-    if 'creds' not in session:
-        consent = oauth_client.initiate_consent()
-        session['consent'] = consent.as_dict()
-        return redirect(consent.auth_url)
-
-    from databricks.sdk import WorkspaceClient
-    from databricks.sdk.oauth import RefreshableCredentials
-
-    credentials_provider = RefreshableCredentials.from_dict(oauth_client, session['creds'])
-    workspace_client = WorkspaceClient(host=oauth_client.host,
-                                       product=APP_NAME,
-                                       credentials_provider=credentials_provider)
+   if 'creds' not in session:
+      consent = oauth_client.initiate_consent()
+      session['consent'] = consent.as_dict()
+      return redirect(consent.auth_url)
+
+   from databricks.sdk import WorkspaceClient
+   from databricks.sdk.oauth import SessionCredentials
+
+   credentials_provider = SessionCredentials.from_dict(oauth_client, session['creds'])
+   workspace_client = WorkspaceClient(host=oauth_client.host,
+                                      product=APP_NAME,
+                                      credentials_provider=credentials_provider)
 
-    return render_template_string('...', w=workspace_client)
+   return render_template_string('...', w=workspace_client)
 ```
 
 ### SSO for local scripts on development machines
 
 For applications, that do run on developer workstations, Databricks SDK for Python provides `auth_type='external-browser'`
 utility, that opens up a browser for a user to go through SSO flow. Azure support is still in the early experimental
 stage.
```

### Comparing `databricks-sdk-0.1.6/databricks_sdk.egg-info/SOURCES.txt` & `databricks-sdk-0.1.7/databricks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/setup.cfg` & `databricks-sdk-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.1.6/setup.py` & `databricks-sdk-0.1.7/setup.py`

 * *Files identical despite different names*

