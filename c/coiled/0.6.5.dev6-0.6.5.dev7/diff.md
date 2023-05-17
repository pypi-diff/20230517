# Comparing `tmp/coiled-0.6.5.dev6.tar.gz` & `tmp/coiled-0.6.5.dev7.tar.gz`

## Comparing `coiled-0.6.5.dev6.tar` & `coiled-0.6.5.dev7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_version.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/analytics.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/context.py
--rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/exceptions.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/magic.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/software.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/types.py
--rw-r--r--   0        0        0    49062 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/websockets.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    86022 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    60139 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/pyproject.toml
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.5.dev6/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_version.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/analytics.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/coiled.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/context.py
+-rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/exceptions.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/magic.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/software.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/types.py
+-rw-r--r--   0        0        0    49062 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/websockets.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    86022 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    60907 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/login.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/pyproject.toml
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/PKG-INFO
```

### Comparing `coiled-0.6.5.dev6/coiled/__init__.py` & `coiled-0.6.5.dev7/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/analytics.py` & `coiled-0.6.5.dev7/coiled/analytics.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,38 +86,44 @@
     >>> coiled.analytics.list_clusters()  # doctest: +SKIP
     >>> coiled.analytics.list_clusters(since="30 days", user="alice")  # doctest: +SKIP
     """
     with coiled.Cloud() as c:
         return c.list_dask_scheduler(account=account, since=since, user=user)
 
 
-def list_computations(cluster_id: int, account: Optional[str] = None):
+def list_computations(
+    cluster_id: Optional[int] = None, scheduler_id: Optional[int] = None, account: Optional[str] = None
+):
     """List computations associated to a cluster
 
+    You need to specify either cluster_id or scheduler_id.
+
     Parameters
     ----------
-    cluster_id:
-        The identifier of the cluster that you want to select
+    cluster_id (optional):
+        The identifier of the Coiled cluster that you want to select
+    scheduler_id (optional):
+        The identifier of the (Coiled or non-Coiled) scheduler analytics that you want to select
     account:
         The account whose clusters you want to list
         You must be a member of this account
         Your default account will be used if none is provided
 
     Examples
     --------
     >>> import coiled.analytics
     >>> clusters = coiled.analytics.list_clusters()  # doctest: +SKIP
-    >>> coiled.analytics.list_computations(clusters[0]["id"])  # doctest: +SKIP
+    >>> coiled.analytics.list_computations(scheduler_id=clusters[0]["id"])  # doctest: +SKIP
 
     See Also
     --------
     list_clusters
     """
     with coiled.Cloud() as c:
-        return c.list_computations(cluster_id, account=account)
+        return c.list_computations(cluster_id=cluster_id, scheduler_id=scheduler_id, account=account)
 
 
 def list_events(cluster_id: int, account: Optional[str] = None):
     """List events associated to a cluster
 
     Parameters
     ----------
@@ -192,17 +198,17 @@
         The amount of time to go back in history to list clusters.
         Defaults to seven days.  Leave as ``None`` to collect all history.
         Accepts any value parseable by dask.utils.parse_timedelta
     user (optional):
         Optionally filter on username
         Providing ``None`` selects all users
     cluster_id (optional):
-        The identifier of the cluster that you want to select
+        The identifier of the Coiled cluster that you want to select
     scheduler_id (optional):
-        The identifier of the scheduler analytics that you want to select
+        The identifier of the (Coiled or non-Coiled) scheduler analytics that you want to select
 
     Examples
     --------
     >>> import coiled.analytics
     >>> coiled.analytics.list_exceptions()  # doctest: +SKIP
     >>> coiled.analytics.list_exceptions(since="30 days", user="alice")  # doctest: +SKIP
     """
```

### Comparing `coiled-0.6.5.dev6/coiled/cluster.py` & `coiled-0.6.5.dev7/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/coiled.yaml` & `coiled-0.6.5.dev7/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/context.py` & `coiled-0.6.5.dev7/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/core.py` & `coiled-0.6.5.dev7/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/exceptions.py` & `coiled-0.6.5.dev7/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/magic.py` & `coiled-0.6.5.dev7/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/scan.py` & `coiled-0.6.5.dev7/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/software.py` & `coiled-0.6.5.dev7/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/types.py` & `coiled-0.6.5.dev7/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/utils.py` & `coiled-0.6.5.dev7/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/websockets.py` & `coiled-0.6.5.dev7/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/_beta/cluster.py` & `coiled-0.6.5.dev7/coiled/_beta/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/_beta/core.py` & `coiled-0.6.5.dev7/coiled/_beta/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,47 +336,74 @@
         self,
         account: Optional[str] = None,
         since: Optional[str] = "7 days",
         user: Optional[str] = "",
     ) -> Union[list, Awaitable[list]]:
         return self._sync(self._list_dask_scheduler, account, since=since, user=user)
 
-    async def _list_computations(self, cluster_id: int, account: Optional[str] = None):
-        return await self._depaginate_list(self._list_computations_page, cluster_id=cluster_id, account=account)
+    async def _list_computations(
+        self, cluster_id: Optional[int] = None, scheduler_id: Optional[int] = None, account: Optional[str] = None
+    ):
+        return await self._depaginate_list(
+            self._list_computations_page, cluster_id=cluster_id, scheduler_id=scheduler_id, account=account
+        )
 
     async def _list_computations_page(
         self,
         page: int,
-        cluster_id: int,
+        cluster_id: Optional[int] = None,
+        scheduler_id: Optional[int] = None,
         account: Optional[str] = None,
     ) -> Tuple[list, bool]:
         page_size = 100
         account = account or self.default_account
+
+        if not scheduler_id and not cluster_id:
+            raise ValueError("either cluster_id or scheduler_id must be specified")
+
+        api = (
+            f"/api/v2/analytics/{account}/{scheduler_id}/computations/list"
+            if scheduler_id
+            else f"/api/v2/analytics/{account}/cluster/{cluster_id}/computations/list"
+        )
+
         response = await self._do_request(
             "GET",
-            self.server + f"/api/v2/analytics/{account}/{cluster_id}/computations/list",
+            self.server + api,
             params={"limit": page_size, "offset": page_size * page},
         )
         if response.status >= 400:
             await handle_api_exception(response)
 
         results = await response.json()
         has_more_pages = len(results) > 0
         return results, has_more_pages
 
     @overload
-    def list_computations(self: Cloud[Sync], cluster_id: int, account: Optional[str] = None) -> list:
+    def list_computations(
+        self: Cloud[Sync],
+        cluster_id: Optional[int] = None,
+        scheduler_id: Optional[int] = None,
+        account: Optional[str] = None,
+    ) -> list:
         ...
 
     @overload
-    def list_computations(self: Cloud[Async], cluster_id: int, account: Optional[str] = None) -> Awaitable[list]:
+    def list_computations(
+        self: Cloud[Async],
+        cluster_id: Optional[int] = None,
+        scheduler_id: Optional[int] = None,
+        account: Optional[str] = None,
+    ) -> Awaitable[list]:
         ...
 
-    def list_computations(self, cluster_id: int, account: Optional[str] = None) -> Union[list, Awaitable[list]]:
-        return self._sync(self._list_computations, cluster_id, account)
+    def list_computations(
+        self, cluster_id: Optional[int] = None, scheduler_id: Optional[int] = None, account: Optional[str] = None
+    ) -> Union[list, Awaitable[list]]:
+        return self._sync(self._list_computations, cluster_id=cluster_id, scheduler_id=scheduler_id, account=account)
 
     @overload
     def list_exceptions(
         self,
         cluster_id: Optional[int] = None,
         scheduler_id: Optional[int] = None,
         account: Optional[str] = None,
```

### Comparing `coiled-0.6.5.dev6/coiled/_beta/cwi_log_link.py` & `coiled-0.6.5.dev7/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/_beta/states.py` & `coiled-0.6.5.dev7/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/_beta/widgets/__init__.py` & `coiled-0.6.5.dev7/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/_beta/widgets/rich.py` & `coiled-0.6.5.dev7/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/_beta/widgets/util.py` & `coiled-0.6.5.dev7/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/config.py` & `coiled-0.6.5.dev7/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/core.py` & `coiled-0.6.5.dev7/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/curl.py` & `coiled-0.6.5.dev7/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/env.py` & `coiled-0.6.5.dev7/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/login.py` & `coiled-0.6.5.dev7/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/package_sync.py` & `coiled-0.6.5.dev7/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/utils.py` & `coiled-0.6.5.dev7/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/cluster/__init__.py` & `coiled-0.6.5.dev7/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/cluster/better_logs.py` & `coiled-0.6.5.dev7/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/cluster/logs.py` & `coiled-0.6.5.dev7/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/cluster/ssh.py` & `coiled-0.6.5.dev7/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/notebook/__init__.py` & `coiled-0.6.5.dev7/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/notebook/notebook.py` & `coiled-0.6.5.dev7/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/setup/__init__.py` & `coiled-0.6.5.dev7/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/setup/amp.py` & `coiled-0.6.5.dev7/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/setup/aws.py` & `coiled-0.6.5.dev7/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/setup/entry.py` & `coiled-0.6.5.dev7/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/setup/gcp.py` & `coiled-0.6.5.dev7/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/cli/setup/prometheus.py` & `coiled-0.6.5.dev7/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/coiled/v2/__init__.py` & `coiled-0.6.5.dev7/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/LICENSE` & `coiled-0.6.5.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/README.md` & `coiled-0.6.5.dev7/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/pyproject.toml` & `coiled-0.6.5.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev6/PKG-INFO` & `coiled-0.6.5.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.5.dev6
+Version: 0.6.5.dev7
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.6.5.dev6 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.6.5.dev7 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
```

