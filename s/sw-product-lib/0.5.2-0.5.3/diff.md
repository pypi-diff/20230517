# Comparing `tmp/sw_product_lib-0.5.2.tar.gz` & `tmp/sw_product_lib-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_product_lib-0.5.2.tar", max compression
+gzip compressed data, was "sw_product_lib-0.5.3.tar", max compression
```

## Comparing `sw_product_lib-0.5.2.tar` & `sw_product_lib-0.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1134 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       87 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/sw_product_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/sw_product_lib/client/__init__.py
--rw-r--r--   0        0        0    10691 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/sw_product_lib/client/backend.py
--rw-r--r--   0        0        0     3885 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/sw_product_lib/client/billing.py
--rw-r--r--   0        0        0    19698 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/sw_product_lib/client/job.py
--rw-r--r--   0        0        0     8702 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/sw_product_lib/client/resource.py
--rw-r--r--   0        0        0      331 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/sw_product_lib/platform/gql.py
--rw-r--r--   0        0        0    19163 2023-03-03 23:18:51.270074 sw_product_lib-0.5.2/sw_product_lib/service.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 sw_product_lib-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1134 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/sw_product_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/sw_product_lib/client/__init__.py
+-rw-r--r--   0        0        0    10691 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/sw_product_lib/client/backend.py
+-rw-r--r--   0        0        0     3885 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/sw_product_lib/client/billing.py
+-rw-r--r--   0        0        0    19698 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/sw_product_lib/client/job.py
+-rw-r--r--   0        0        0     8702 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/sw_product_lib/client/resource.py
+-rw-r--r--   0        0        0      331 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/sw_product_lib/platform/gql.py
+-rw-r--r--   0        0        0    19264 2023-03-07 15:47:27.241407 sw_product_lib-0.5.3/sw_product_lib/service.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 sw_product_lib-0.5.3/PKG-INFO
```

### Comparing `sw_product_lib-0.5.2/pyproject.toml` & `sw_product_lib-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 per-file-ignores = [
     "__init__.py:F401",
     "./docs/*:E402"
 ]
 
 [tool.poetry]
 name = "sw-product-lib"
-version = "0.5.2"
+version = "0.5.3"
 description = "Python library for Strangeworks products to interact with the Strangeworks Platform"
 authors = ["Strangeworks Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^12.4.4"
```

### Comparing `sw_product_lib-0.5.2/sw_product_lib/client/backend.py` & `sw_product_lib-0.5.3/sw_product_lib/client/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.5.2/sw_product_lib/client/billing.py` & `sw_product_lib-0.5.3/sw_product_lib/client/billing.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.5.2/sw_product_lib/client/job.py` & `sw_product_lib-0.5.3/sw_product_lib/client/job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.5.2/sw_product_lib/client/resource.py` & `sw_product_lib-0.5.3/sw_product_lib/client/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.5.2/sw_product_lib/service.py` & `sw_product_lib-0.5.3/sw_product_lib/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,19 @@
         )
 
 
 DEFAULT_PLATFORM_BASE_URL = "https://api.strangeworks.com"
 api_key = os.getenv("PRODUCT_LIB_API_KEY")
 base_url = os.getenv("PRODUCT_LIB_BASE_URL", DEFAULT_PLATFORM_BASE_URL)
 
-_api = ProductAPI(api_key=api_key, base_url=base_url) if api_key and base_url else None
+
+def _api():
+    return (
+        ProductAPI(api_key=api_key, base_url=base_url) if api_key and base_url else None
+    )
 
 
 def create_job(
     ctx: RequestContext,
     parent_job_slug: Optional[str] = None,
     external_identifier: Optional[str] = None,
     status: str = "CREATED",
@@ -113,15 +117,15 @@
         status of job that was initiated on an  external (non-Strangeworks) system.
     job_data_schema: Optional[str]
         link to the json schema describing job output.
     job_data: Optional[str]
         job output.
     """
     return job.create(
-        api=ctx.api or _api,
+        api=ctx.api or _api(),
         resource_slug=ctx.resource_slug,
         workspace_member_slug=ctx.workspace_member_slug,
         parent_job_slug=parent_job_slug,
         external_identifier=external_identifier,
         status=status,
         remote_status=remote_status,
         job_data_schema=job_data_schema,
@@ -159,15 +163,15 @@
         status of job that was initiated on an  external (non-Strangeworks) system.
     job_data_schema: Optional[str]
         link to the json schema describing job output.
     job_data: Optional[str]
         job output.
     """
     return job.update(
-        api=ctx.api or _api,
+        api=ctx.api or _api(),
         resource_slug=ctx.resource_slug,
         job_slug=job_slug,
         parent_job_slug=parent_job_slug,
         external_identifier=external_identifier,
         status=status,
         remote_status=remote_status,
         job_data_schema=job_data_schema,
@@ -188,15 +192,15 @@
         contains key-values specific to the current request.
     job_slug: str
       slug of the job that needs values updated.
     tags: List[str]
         list of tags to apply to the job
     """
     return job.add_tags(
-        api=ctx.api or _api,
+        api=ctx.api or _api(),
         resource_slug=ctx.resource_slug,
         job_slug=job_slug,
         tags=tags,
     )
 
 
 def create_billing_transaction(
@@ -218,15 +222,15 @@
         numerical amount. can be negative.
     unit: str
         describes the unit for the amount. for example, USD for currency.
     description: str
         a brief description that can be seen by the user.
     """
     return billing.create_transaction(
-        api=ctx.api or _api,
+        api=ctx.api or _api(),
         resource_slug=ctx.resource_slug,
         job_slug=job_slug,
         amount=amount,
         unit=unit,
         description=description,
     )
 
@@ -244,15 +248,15 @@
             used to map workspace and user.
     amount: float
         numerical amount to indicate cost (negative amount) or credit(positive amount)
     unit: str
         unit for the amount
     """
     return billing.request_approval(
-        api=ctx.api or _api,
+        api=ctx.api or _api(),
         resource_slug=ctx.resource_slug,
         workspace_member_slug=ctx.workspace_member_slug,
         amount=amount,
         currency=unit,
     )
 
 
@@ -263,15 +267,18 @@
     from the request context object passed in.
 
     Parameters:
     ctx: RequestContext
         contains key-values specific to the current request.
 
     """
-    return resource.get(api=_api, resource_slug=ctx.resource_slug)
+    return resource.get(
+        api=ctx.api or _api(),
+        resource_slug=ctx.resource_slug,
+    )
 
 
 def upload_job_file(
     ctx: RequestContext,
     job_slug: str,
     name: Optional[str],
     path: str,
@@ -321,15 +328,15 @@
     ------
     File
         Object with information about the file that was uploaded.
 
     raises StrangeworksError if any issues arise while attempting to upload the file.
     """
     f, signedUrl = job.upload_file(
-        api=ctx.api or _api,
+        api=ctx.api or _api(),
         resource_slug=ctx.resource_slug,
         job_slug=job_slug,
         file_path=path,
         file_name=name,
         override_existing=overwrite,
         json_schema=json_schema,
         is_hidden=is_hidden,
@@ -364,15 +371,15 @@
         job_slug identifies the job which is fetched.
 
     Returns
     -------
     Job
         A Job object identified by the slug.
     """
-    return job.get(api=ctx.api or _api, resource_slug=ctx.resource_slug, id=job_slug)
+    return job.get(api=ctx.api or _api(), resource_slug=ctx.resource_slug, id=job_slug)
 
 
 def get_job_by_external_identifier(
     ctx: RequestContext, external_identifier: str
 ) -> Optional[Job]:
     """Get the job identified by external_identifier.
     Parameters
@@ -383,15 +390,15 @@
         external_identifier identifies the job which is fetched.
     Returns
     -------
     Optional[Job]
         A Job object identified by the product identifier or None.
     """
     return job.get_by_external_identifier(
-        api=ctx.api or _api,
+        api=ctx.api or _api(),
         id=external_identifier,
     )
 
 
 def get_jobs_by_statuses(
     ctx: RequestContext, statuses: List[JobStatus]
 ) -> Optional[Dict[JobStatus, List[Job]]]:
@@ -408,15 +415,15 @@
     ----------
     A dictionary where the jobs are grouped by statuses.
     The keys in the dictionary are the statuses.
     Each status has their list of jobs.
 
     Optional[Dict[JobStatus, List[Job]]]
     """
-    return job.get_by_statuses(api=ctx.api or _api, statuses=statuses)
+    return job.get_by_statuses(api=ctx.api or _api(), statuses=statuses)
 
 
 def get_backends(
     ctx: RequestContext,
     product_slugs: Optional[List[str]] = None,
     backend_type_slugs: Optional[List[str]] = None,
     backend_statuses: Optional[List[str]] = None,
@@ -444,15 +451,15 @@
 
     Returns
     -------
     List[Backend]
         The list of backend filtered by the params
     """
     return backend.get_backends(
-        api=ctx.api or _api,
+        api=ctx.api or _api(),
         product_slugs=product_slugs,
         backend_type_slugs=backend_type_slugs,
         backend_statuses=backend_statuses,
         backend_tags=backend_tags,
     )
 
 
@@ -475,15 +482,15 @@
 
     Returns
     -------
     List[Backend]
         The list of backend filtered by the params
     """
     return backend.get_product_backends(
-        api=ctx.api or _api, status=status, remote_backend_id=remote_backend_id
+        api=ctx.api or _api(), status=status, remote_backend_id=remote_backend_id
     )
 
 
 def create_backends(
     ctx: RequestContext, backends: List[backend.Backend]
 ) -> List[backend.Backend]:
     """Create backends specified by the payload
@@ -496,15 +503,15 @@
         backends to create
 
     Returns
     -------
     List[Backend]
         The list of backends created
     """
-    return backend.backend_create(api=ctx.api or _api, payload=backends)
+    return backend.backend_create(api=ctx.api or _api(), payload=backends)
 
 
 def delete_backend(ctx: RequestContext, backend_slug: str) -> None:
     """Delete backend by slug
 
     Parameters
     ----------
@@ -513,15 +520,15 @@
     backend_slug: str
         backend to delete
 
     Returns
     -------
     None
     """
-    return backend.backend_delete(api=ctx.api or _api, backend_slug=backend_slug)
+    return backend.backend_delete(api=ctx.api or _api(), backend_slug=backend_slug)
 
 
 def update_backends(
     ctx: RequestContext, backends: List[backend.BackendUpdateInput]
 ) -> List[backend.Backend]:
     """Update backends specified by the payload
     Overwites all write-able fields, so must include
@@ -535,15 +542,15 @@
         backend update input for each backend to update
 
     Returns
     -------
     List[Backend]
         The list of backends updated
     """
-    return backend.backend_update(api=ctx.api or _api, backend_update_input=backends)
+    return backend.backend_update(api=ctx.api or _api(), backend_update_input=backends)
 
 
 def add_backend_types(
     ctx: RequestContext, backend_slug: str, types: List[backend.BackendTypeInput]
 ):
     """Add backend types to a certain backend.
     Strangeworks defines certain types a backend can adhere to.
@@ -558,15 +565,15 @@
     backend_slug: str
         backend slug that identifies the backend which you will add types to
     types: List[backend.BackendTypeInput]
         the many types you are registering to this backend.
 
     """
     backend.backend_add_types(
-        api=ctx.api or _api, backend_slug=backend_slug, backend_types=types
+        api=ctx.api or _api(), backend_slug=backend_slug, backend_types=types
     )
 
 
 def remove_backend_types(ctx: RequestContext, backend_slug: str, types: List[str]):
     """Remove backend types from a certain backend.
     Strangeworks defines certain types a backend can adhere to.
     This un-registers the specified backend with the many types provided.
@@ -580,15 +587,15 @@
     backend_slug: str
         backend slug that identifies the backend which you will add types to
     types: List[str]
         the many types you are un-registering from this backend.
 
     """
     backend.backend_remove_types(
-        api=ctx.api or _api, backend_slug=backend_slug, backend_types=types
+        api=ctx.api or _api(), backend_slug=backend_slug, backend_types=types
     )
 
 
 @deprecated(
     reason=(
         "This function is deprecated and will be removed. Use auth.get_token instead."
     )
```

### Comparing `sw_product_lib-0.5.2/PKG-INFO` & `sw_product_lib-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw-product-lib
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python library for Strangeworks products to interact with the Strangeworks Platform
 License: Apache-2.0
 Author: Strangeworks Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

