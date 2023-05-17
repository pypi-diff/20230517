# Comparing `tmp/pGerrit-0.1.4.tar.gz` & `tmp/pGerrit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pGerrit-0.1.4.tar", last modified: Fri Mar 31 12:52:54 2023, max compression
+gzip compressed data, was "pGerrit-0.1.5.tar", last modified: Wed May 17 11:51:53 2023, max compression
```

## Comparing `pGerrit-0.1.4.tar` & `pGerrit-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-03-31 12:52:54.086437 pGerrit-0.1.4/
--rw-rw-r--   0 cy        (1000) cy        (1000)      891 2023-03-31 12:52:54.086437 pGerrit-0.1.4/PKG-INFO
--rw-rw-r--   0 cy        (1000) cy        (1000)     3256 2023-03-31 08:22:30.000000 pGerrit-0.1.4/README.md
-drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-03-31 12:52:54.086437 pGerrit-0.1.4/pGerrit/
--rw-rw-r--   0 cy        (1000) cy        (1000)     1477 2023-03-31 12:44:06.000000 pGerrit-0.1.4/pGerrit/Access.py
--rw-rw-r--   0 cy        (1000) cy        (1000)       21 2023-03-31 12:50:33.000000 pGerrit-0.1.4/pGerrit/__init__.py
--rw-rw-r--   0 cy        (1000) cy        (1000)    32093 2023-03-31 12:44:06.000000 pGerrit-0.1.4/pGerrit/change.py
--rw-rw-r--   0 cy        (1000) cy        (1000)     3581 2023-03-31 12:44:06.000000 pGerrit-0.1.4/pGerrit/client.py
--rw-rw-r--   0 cy        (1000) cy        (1000)      130 2023-03-29 03:40:33.000000 pGerrit-0.1.4/pGerrit/exception.py
--rw-rw-r--   0 cy        (1000) cy        (1000)      586 2023-03-29 03:40:33.000000 pGerrit-0.1.4/pGerrit/queryMeta.py
--rw-rw-r--   0 cy        (1000) cy        (1000)     3529 2023-03-29 03:40:33.000000 pGerrit-0.1.4/pGerrit/restAPIwrapper.py
--rw-rw-r--   0 cy        (1000) cy        (1000)      772 2023-03-31 11:18:07.000000 pGerrit-0.1.4/pGerrit/utils.py
-drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-03-31 12:52:54.086437 pGerrit-0.1.4/pGerrit.egg-info/
--rw-rw-r--   0 cy        (1000) cy        (1000)      891 2023-03-31 12:52:54.000000 pGerrit-0.1.4/pGerrit.egg-info/PKG-INFO
--rw-rw-r--   0 cy        (1000) cy        (1000)      373 2023-03-31 12:52:54.000000 pGerrit-0.1.4/pGerrit.egg-info/SOURCES.txt
--rw-rw-r--   0 cy        (1000) cy        (1000)        1 2023-03-31 12:52:54.000000 pGerrit-0.1.4/pGerrit.egg-info/dependency_links.txt
--rw-rw-r--   0 cy        (1000) cy        (1000)       24 2023-03-31 12:52:54.000000 pGerrit-0.1.4/pGerrit.egg-info/requires.txt
--rw-rw-r--   0 cy        (1000) cy        (1000)       14 2023-03-31 12:52:54.000000 pGerrit-0.1.4/pGerrit.egg-info/top_level.txt
--rw-rw-r--   0 cy        (1000) cy        (1000)      847 2023-03-31 12:52:54.086437 pGerrit-0.1.4/setup.cfg
--rw-rw-r--   0 cy        (1000) cy        (1000)       68 2023-03-31 11:18:07.000000 pGerrit-0.1.4/setup.py
-drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-03-31 12:52:54.086437 pGerrit-0.1.4/tests/
--rw-rw-r--   0 cy        (1000) cy        (1000)        0 2023-03-29 03:40:33.000000 pGerrit-0.1.4/tests/__init__.py
--rw-rw-r--   0 cy        (1000) cy        (1000)    10149 2023-03-29 03:40:33.000000 pGerrit-0.1.4/tests/test.py
+drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-05-17 11:51:53.325699 pGerrit-0.1.5/
+-rw-rw-r--   0 cy        (1000) cy        (1000)      891 2023-05-17 11:51:53.325699 pGerrit-0.1.5/PKG-INFO
+-rw-rw-r--   0 cy        (1000) cy        (1000)     3288 2023-05-17 06:38:32.000000 pGerrit-0.1.5/README.md
+drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-05-17 11:51:53.325699 pGerrit-0.1.5/pGerrit/
+-rw-rw-r--   0 cy        (1000) cy        (1000)     1431 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/Access.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)      987 2023-04-04 12:31:47.000000 pGerrit-0.1.5/pGerrit/ApprovalInfo.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)       21 2023-05-17 11:48:49.000000 pGerrit-0.1.5/pGerrit/__init__.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)    35397 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/change.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)     4033 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/client.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)     2292 2023-05-17 11:48:26.000000 pGerrit-0.1.5/pGerrit/project.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)     3859 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/queryDescriptor.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)     3778 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/restAPIwrapper.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)      772 2023-03-31 11:18:07.000000 pGerrit-0.1.5/pGerrit/utils.py
+drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-05-17 11:51:53.325699 pGerrit-0.1.5/pGerrit.egg-info/
+-rw-rw-r--   0 cy        (1000) cy        (1000)      891 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/PKG-INFO
+-rw-rw-r--   0 cy        (1000) cy        (1000)      401 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 cy        (1000) cy        (1000)        1 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 cy        (1000) cy        (1000)       24 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/requires.txt
+-rw-rw-r--   0 cy        (1000) cy        (1000)       14 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/top_level.txt
+-rw-rw-r--   0 cy        (1000) cy        (1000)      847 2023-05-17 11:51:53.325699 pGerrit-0.1.5/setup.cfg
+-rw-rw-r--   0 cy        (1000) cy        (1000)       68 2023-03-31 11:18:07.000000 pGerrit-0.1.5/setup.py
+drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-05-17 11:51:53.325699 pGerrit-0.1.5/tests/
+-rw-rw-r--   0 cy        (1000) cy        (1000)        0 2023-03-29 03:40:33.000000 pGerrit-0.1.5/tests/__init__.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)    13790 2023-05-17 06:38:32.000000 pGerrit-0.1.5/tests/test.py
```

### Comparing `pGerrit-0.1.4/PKG-INFO` & `pGerrit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pGerrit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A well designed base on decorator pattern library to access Google Gerrit REST API
 Home-page: UNKNOWN
 Author: CY
 Author-email: 17103513@qq.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/demonguy/pGerrit
 Project-URL: Tracker, https://github.com/demonguy/pGerrit/issues
```

### Comparing `pGerrit-0.1.4/README.md` & `pGerrit-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 <!-- RTD-IGNORE -->
 Complete project documentation can be found at [here](https://pgerrit.readthedocs.io/en/latest/).
 <!-- END-RTD-IGNORE -->
 
 ## Features
 * 🍰 **Clear design:** Every REST API endpoint is a class. Every entity of the endpoint is an object
 * 🚀 **Easy of use** You can access the state of entity by access the property of the object
-* ⚙️ **Easy to contribute** Add a new REST API is pretty easy by using decorator.
+* ⚙️ **PyCharm Autocomplete Support** Adapted for PyCharm's auto-completion. Next step we will support response autocomplete
 
 ## Quickstart
 
 ### Installation
 ```bash
 pip install pGerrit
 ```
@@ -70,8 +70,8 @@
 ```
 
 ## Next Steps
 To find out more about what you can do with pGerrit, see:
 
 * [Quick Start](https://pgerrit.readthedocs.io/en/latest/user/quickstart/)
 * [Advanced Usage](https://pgerrit.readthedocs.io/en/latest/user/advanced/)
-* [API Reference](https://pgerrit.readthedocs.io/end/latest/reference.html)
+* [API Reference](https://pgerrit.readthedocs.io/en/latest/api/)
```

### Comparing `pGerrit-0.1.4/pGerrit/Access.py` & `pGerrit-0.1.5/pGerrit/project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,58 @@
 from pGerrit.restAPIwrapper import GerritRest
 from pGerrit.client import GerritClient
 from pGerrit.utils import urljoin, urlformat
-from pGerrit.queryMeta import QueryMeta
 
-class GerritAccess(GerritClient, metaclass=QueryMeta):
-    """Class maps /access/ endpoint of Gerrit REST API
+class GerritProject(GerritClient):
+    """Class maps /projects/ endpoint of Gerrit REST API
 
-    :return: An instance of GerritAccess.
-    :rtype: pGerrit.GerritAccess
+    :return: An instance of GerritProject.
+    :rtype: pGerrit.project.GerritProject
 
     You won't need to instantiate this Class directly.
-    Use ``pGerrit.GerritClient.access``
+    Use ``pGerrit.GerritClient.project``
     """
-    _endpoint = "/a/access/{}"
+    _endpoint = "/a/projects/{}"
+    _args = ["pj"]
 
-    def __init__(self, host, auth=None, verify=True, adapter=None, cache=True, cache_expire=3):
+    def __init__(self, host, project, auth=None, verify=True, adapter=None, cache=True, cache_expire=3):
         """See class docstring."""
         super().__init__(host, auth=auth, verify=verify, adapter=adapter, cache=cache, cache_expire=cache_expire)
+        self.pj = project
 
+        self.args = [host, project]
+        self.kwargs = {"auth": auth, "verify": verify, "adapter":adapter, "cache":cache, "cache_expire":cache_expire}
+
+    @classmethod
     @GerritRest.get()
-    def query(self, *args, **kwargs):
-        """Performs a GET request to query for access rights from the Gerrit API.
+    def query(cls, *args, **kwargs):
+        """Performs a GET request to query for projects from the Gerrit API.
 
-        **API URL**: `/a/access/ <https://gerrit-review.googlesource.com/Documentation/rest-api-access.html#list-access>`__
+        **API URL**: `/a/projects/ <https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#list-projects>`__
 
-        **Input type**: `QueryOptions <https://gerrit-review.googlesource.com/Documentation/rest-api-access.html#list-access>`__
+        **Input type**: `QueryOptions <https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#list-projects>`__
 
-        **Return type**: Dict[`str`, `ProjectAccessInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-access.html#project-access-info>`__]
+        **Return type**: `ProjectInfo  <https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-info>`__
 
         Usage::
 
-            access_rights = gerrit_access.query(**{"project": "All-Projects"})
+            project.query(
+                query="name:test"
+            )
+        """
+        return urljoin(cls.host, urlformat(GerritProject._endpoint, ""))
+    
+    @GerritRest.get()
+    @GerritRest.url_wrapper()
+    def access(self, *args, **kwargs):
+        """Performs a GET request to list access rights for project from the Gerrit API.
+
+        **API URL**: `/a/projects/ <https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#get-access>`__
 
+        **Input type**: `QueryOptions <https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#get-access>`__
+
+        **Return type**: `ProjectAccessInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-access.html#project-access-info>`__
+
+        Usage::
+            project.access()
         """
-        return urljoin(self.host, urlformat(GerritAccess._endpoint, ""))
+        pass
```

### Comparing `pGerrit-0.1.4/pGerrit/change.py` & `pGerrit-0.1.5/pGerrit/change.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from pGerrit.restAPIwrapper import GerritRest
 from pGerrit.client import GerritClient
 from pGerrit.utils import urljoin, urlformat
-from pGerrit.queryMeta import QueryMeta
 
-class GerritChange(GerritClient, metaclass=QueryMeta):
+class GerritChange(GerritClient):
     """Class maps /changes/ endpoint of Gerrit REST API
 
     :return: An instance of GerritChange.
     :rtype: pGerrit.change.GerritChange
 
     You won't need to instantiate this Class directly.
     Use ``pGerrit.GerritClient.change``
     """
     _endpoint = "/a/changes/{}"
     _args = ["id"]
 
-    def __init__(self, host, gerritID=None, auth=None, verify=True, adapter=None, cache=True, cache_expire=3):
+    def __init__(self, host, gerritID, auth=None, verify=True, adapter=None, cache=True, cache_expire=3):
         """See class docstring."""
         super().__init__(host, auth=auth, verify=verify, adapter=adapter, cache=cache, cache_expire=cache_expire)
         self.id = gerritID
 
+        self.args = [host, gerritID]
+        self.kwargs = {"auth": auth, "verify": verify, "adapter":adapter, "cache":cache, "cache_expire":cache_expire}
+
+    @classmethod
     @GerritRest.get()
-    def query(self, *args, **kwargs):
+    def query(cls, *args, **kwargs):
         """Performs a GET request to query for changes from the Gerrit API.
 
         **API URL**: `/a/changes/ <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#list-changes>`__
 
         **Input type**: `QueryOptions <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#list-changes>`__
 
         **Return type**: List[`ChangeInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#change-info>`__]
@@ -39,15 +42,15 @@
                     "o": [
                         "CURRENT_REVISION",
                         "CURRENT_COMMIT"
                     ]
                 }
             )
         """
-        return urljoin(self.host, urlformat(GerritChange._endpoint, ""))
+        return urljoin(cls.host, urlformat(GerritChange._endpoint, ""))
 
     @GerritRest.get()
     def info(self, *args, **kwargs):
         """Performs a GET request to retrieve information about a change.
 
         **API URL**: `/a/changes/{change_id} <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#get-change>`__
 
@@ -58,28 +61,14 @@
         Usage::
 
             change.info(**{o":["CURRENT_REVISION", "CURRENT_COMMIT"]})
 
         """
         return urljoin(self.host, urlformat(GerritChange._endpoint, self.id))
 
-    def is_merge(self):
-        """Checks if the change is a merge change.
-
-        Usage::
-
-            is_merge_change = change.is_merge()
-
-        """
-        revision = self.current_revision()
-        if len(revision.commit().parents) == 2:
-            return True
-        else:
-            return False
-
     @GerritRest.get()
     @GerritRest.url_wrapper()
     def detail(self, *args, **kwargs):
         """Performs a GET request to retrieve detailed information about a change.
 
         **API URL**: `/a/changes/{change_id}/detail <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#get-change-detail>`__
 
@@ -126,14 +115,32 @@
         Usage::
 
             change.set_topic({"topic": "new-topic"})
 
         """
         pass
 
+    @GerritRest.delete
+    @GerritRest.url_wrapper("topic")
+    def delete_topic(self, *args, **kwargs):
+        """Performs a PUT request to set the topic of a change.
+
+        **API URL**: `/a/changes/{change_id}/topic <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#set-topic>`__
+
+        **Input type**: None
+
+        **Return type**: None
+
+        Usage::
+
+            change.delete_topic()
+
+        """
+        pass
+
     @GerritRest.get()
     @GerritRest.url_wrapper()
     def submitted_together(self, *args, **kwargs):
         """Performs a GET request to retrieve the list of changes that would be submitted together with a change.
 
         **API URL**: `/a/changes/{change_id}/submitted_together <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#submitted-together>`__
 
@@ -236,231 +243,348 @@
             change.check()
 
         """
         pass
 
     @GerritRest.get()
     @GerritRest.url_wrapper()
-    def edit(self, *args, **kwargs):
-        """Performs a GET request to retrieve information about the change edit.
+    def hashtags(self, *args, **kwargs):
+        """Performs a GET request to retrieve the hashtags associated with a change.
 
-        **API URL**: `/a/changes/{change_id}/edit <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#edit-endpoints>`__
+        **API URL**: `/a/changes/{change_id}/hashtags <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#get-hashtags>`__
 
         **Input type**: None
 
-        **Return type**: `EditInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#edit-info>`__
+        **Return type**: List[str]
 
         Usage::
 
-            change.edit()
+            change.hashtags()
 
         """
         pass
 
-    @GerritRest.get()
-    @GerritRest.url_wrapper()
-    def reviewers(self, *args, **kwargs):
-        """Performs a GET request to retrieve the list of reviewers for a change.
+    @GerritRest.post
+    @GerritRest.url_wrapper("hashtags")
+    def set_hashtags(self, payload=None, *args, **kwargs):
+        """Performs a POST request to add or remove hashtags from a change.
 
-        **API URL**: `/a/changes/{change_id}/reviewers <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#list-reviewers>`__
+        **API URL**: `/a/changes/{change_id}/hashtags <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#set-hashtags>`__
 
-        **Input type**: None
+        **Input type**: `HashtagsInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#hashtags-input>`__
 
-        **Return type**: List[`ReviewerInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#reviewer-info>`__]
+        **Return type**: List[str]
 
         Usage::
 
-            change.reviewers()
+            change.set_hashtags(payload={"add":["tag1"], "remove":["tag2"]})
 
         """
         pass
 
     @GerritRest.post
-    @GerritRest.url_wrapper("reviewers")
-    def add_reviewer(self, *args, **kwargs):
-        """Performs a POST request to add a reviewer to a change.
+    @GerritRest.url_wrapper()
+    def rebase(self, payload=None, headers=None):
+        """Performs a POST request to rebase a change.
 
-        **API URL**: `/a/changes/{change_id}/reviewers <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#add-reviewer>`__
+        **API URL**: `/a/changes/{change_id}/rebase <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#rebase-change>`__
 
-        **Input type**: `ReviewerInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#reviewer-input>`__
+        **Input type**: `RebaseInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#rebase-input>`__ (optional)
 
-        **Return type**: `ReviewerResult <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#reviewer-result>`__
+        **Return type**: `ChangeInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#change-info>`__
 
         Usage::
 
-            change.add_reviewer({"reviewer": "example@example.com"})
+            change.rebase()
 
         """
         pass
 
-    @GerritRest.get()
-    @GerritRest.url_wrapper()
-    def hashtags(self, *args, **kwargs):
-        """Performs a GET request to retrieve the hashtags associated with a change.
+    @GerritRest.delete
+    @GerritRest.url_wrapper("")
+    def delete_change(self, payload=None, headers=None):
+        """Performs a DELETE request to delete a change.
 
-        **API URL**: `/a/changes/{change_id}/hashtags <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#get-hashtags>`__
+        **API URL**: `/a/changes/{change_id} <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-change>`__
 
         **Input type**: None
 
-        **Return type**: List[str]
+        **Return type**: None
 
         Usage::
 
-            change.hashtags()
+            change.delete_change()
 
         """
         pass
 
-    @GerritRest.post
-    @GerritRest.url_wrapper("hashtags")
-    def set_hashtags(self, *args, **kwargs):
-        """Performs a POST request to add or remove hashtags from a change.
+    def is_merge(self):
+        """Checks if the change is a merge change.
 
-        **API URL**: `/a/changes/{change_id}/hashtags <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#set-hashtags>`__
+        Usage::
 
-        **Input type**: `HashtagsInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#hashtags-input>`__
+            is_merge_change = change.is_merge()
 
-        **Return type**: List[str]
+        """
+        revision = self.current_revision()
+        if len(revision.commit().parents) == 2:
+            return True
+        else:
+            return False
+
+
+    def revision(self, revisionID):
+        """Creates a GerritChangeRevision object for a specific revision of the change.
+
+        :param revisionID: The `revision ID <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#ids>`__ (commit SHA1 or numeric ID)
 
         Usage::
 
-            change.set_hashtags(add=["tag1"], remove=["tag2"])
+            change_revision = change.revision(revisionID)
 
         """
-        pass
+        return GerritChangeRevision(self.host, self.id, revisionID, auth=self.session.auth, verify=self.verify, adapter=self.adapter, cache=self.cache, cache_expire=self.cache_expire)
 
-    @GerritRest.get()
-    @GerritRest.url_wrapper()
-    def suggest_reviewers(self, *args, **kwargs):
-        """Performs a GET request to retrieve a list of suggested reviewers for a change.
+    def current_revision(self):
+        """Creates a GerritChangeRevision object for the current revision of the change.
 
-        **API URL**: `/a/changes/{change_id}/suggest_reviewers <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#suggest-reviewers>`__
+        Usage::
 
-        **Input type**: `SuggestReviewersOptions <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#suggest-reviewers>`__
+            current_revision = change.current_revision()
 
-        **Return type**: List[`SuggestedReviewerInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#suggested-reviewer-info>`__]
+        """
+        return GerritChangeRevision(self.host, self.id, "current", auth=self.session.auth, verify=self.verify, adapter=self.adapter, cache=self.cache, cache_expire=self.cache_expire)
+
+    @property
+    def edit(self):
+        """Provides an instance of GerritChangeEditQueryDescriptor for the given Gerrit client configuration.
+
+        :return: An instance of GerritChangeEditQueryDescriptor.
+        :rtype: pGerrit.queryDescriptor.GerritChangeEditQueryDescriptor
 
         Usage::
 
-            change.suggest_reviewers(q="john")
+            change = GerritChange(...)
+            edit_info = change.edit.info()
+            edited_content = change.edit("COMMIT_MSG").edit_retrieve()
 
         """
-        pass
+        from pGerrit.queryDescriptor import GerritChangeEditQueryDescriptor
+        return GerritChangeEditQueryDescriptor(self)
 
-    @GerritRest.post
-    @GerritRest.url_wrapper()
-    def rebase(self, payload=None, headers=None):
-        """Performs a POST request to rebase a change.
+    @property
+    def reviewer(self):
+        """Provides an instance of GerritChangeReviewerQueryDescriptor for the given Gerrit client configuration.
 
-        **API URL**: `/a/changes/{change_id}/rebase <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#rebase-change>`__
+        :return: An instance of GerritChangeReviewerQueryDescriptor.
+        :rtype: pGerrit.queryDescriptor.GerritChangeReviewerQueryDescriptor
 
-        **Input type**: `RebaseInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#rebase-input>`__ (optional)
+        Usage::
 
-        **Return type**: `ChangeInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#change-info>`__
+            change = GerritChange(...)
+            reviewers = change.reviewer.query()
+            suggested_reviewers = change.reviewer.suggest_reviewers(q="john")
+            result = change.reviewer.add_reviewer({"reviewer": "example@example.com"})
+
+        """
+        from pGerrit.queryDescriptor import GerritChangeReviewerQueryDescriptor
+        return GerritChangeReviewerQueryDescriptor(self)
+
+class GerritChangeEdit(GerritChange):
+    """Class maps /a/changes/{change_id}/edit endpoint of Gerrit REST API
+
+    :return: An instance of GerritChangeEdit.
+    :rtype: pGerrit.change.GerritChangeEdit
+
+    You won't need to instantiate this Class directly.
+    Use ``pGerrit.change.GerritChange.revision``
+    """
+    _endpoint = "/a/changes/{}/edit/{}"
+    _args = ["id", "fileID"]
+
+    def __init__(self, host, gerritID, fileID, auth=None, verify=True, adapter=None, cache=True, cache_expire=3):
+        """See class docstring."""
+        super().__init__(host, gerritID, auth=auth, verify=verify, adapter=adapter, cache=cache, cache_expire=cache_expire)
+        self.fileID = fileID
+
+    @classmethod
+    @GerritRest.get()
+    def info(self, *args, **kwargs):
+        """Performs a GET request to retrieve information about the change edit.
+
+        **API URL**: `/a/changes/{change_id}/edit <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#edit-endpoints>`__
+
+        **Input type**: None
+
+        **Return type**: `EditInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#edit-info>`__
 
         Usage::
 
-            change.rebase()
+            edit.info()
 
         """
-        pass
+        return urljoin(self.host, urlformat(GerritChangeEdit._endpoint, self.id, ""))
 
+    @classmethod
     @GerritRest.post
     @GerritRest.url_wrapper("edit:publish")
     def edit_publish(self, payload=None, headers=None):
         """Performs a POST request to publish a change edit.
 
-        **API URL**: `/a/changes/{change_id}/edit:publish <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#publish-edit>`__
+        **API URL**: `/a/changes/{change_id}/edit/edit:publish <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#publish-edit>`__
 
         **Input type**: `PublishChangeEditInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#publish-change-edit-input>`__ (optional)
 
         **Return type**: None
 
         Usage::
 
-            change.edit_publish()
+            edit.edit_publish()
 
         """
         pass
 
+    @classmethod
     @GerritRest.post
     @GerritRest.url_wrapper("edit")
     def edit_restore(self, payload=None, headers=None):
         """Performs a POST request to restore a change edit.
 
         **API URL**: `/a/changes/{change_id}/edit <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#post-edit>`__
 
         **Input type**: `ChangeEditInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#change-edit-input>`__
         
         **Return type**: None
 
         Usage::
 
-            change.edit_restore({"restore_path": "foo"})
+            edit.edit_restore({"restore_path": "foo"})
 
         """
         pass
 
+    @classmethod
     @GerritRest.delete
     @GerritRest.url_wrapper("edit")
-    def edit_delete(self, payload=None, headers=None):
+    def edit_delete(self, headers=None):
         """Performs a DELETE request to delete a change edit.
 
         **API URL**: `/a/changes/{change_id}/edit <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-edit>`__
 
         **Input type**: None
 
         **Return type**: None
 
         Usage::
 
-            change.edit_delete()
+            edit.edit_delete()
 
         """
         pass
 
-    @GerritRest.delete
-    @GerritRest.url_wrapper("")
-    def delete_change(self, payload=None, headers=None):
-        """Performs a DELETE request to delete a change.
+    @GerritRest.put
+    @GerritRest.url_wrapper()
+    def edit_file(self, payload, headers=None):
+        """Performs a PUT request to edit a specific file in a change revision.
 
-        **API URL**: `/a/changes/{change_id} <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-change>`__
+        **API URL**: `/a/changes/{change_id}/edit/{file_id} <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#edit-file>`__
 
-        **Input type**: None
+        **Input type**: str
 
         **Return type**: None
 
         Usage::
 
-            change.delete_change()
+            edit_file.edit(payload='new_file_content')
 
         """
         pass
 
-    def revision(self, revisionID):
-        """Creates a GerritChangeRevision object for a specific revision of the change.
+    @GerritRest.get()
+    @GerritRest.url_wrapper()
+    def edit_retrieve(self, headers=None):
+        """Performs a GET request to retrieve the content of a specific file in a change revision after editing.
 
-        :param revisionID: The `revision ID <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#ids>`__ (commit SHA1 or numeric ID)
+        **API URL**: `/a/changes/{change_id}/edit/{file_id} <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#get-edit>`__
+
+        **Input type**: None
+
+        **Return type**: str
 
         Usage::
 
-            change_revision = change.revision(revisionID)
+            edited_content = edit_file.edit_retrieve()
 
         """
-        return GerritChangeRevision(self.host, self.id, revisionID, auth=self.session.auth, verify=self.verify, adapter=self.adapter, cache=self.cache, cache_expire=self.cache_expire)
+        pass
 
-    def current_revision(self):
-        """Creates a GerritChangeRevision object for the current revision of the change.
+class GerritChangeReviewer(GerritChange):
+    """Class maps /a/changes/{change_id}/reviewers/{account_id} endpoint of Gerrit REST API
+
+    :return: An instance of GerritChangeReviewer.
+    :rtype: pGerrit.change.GerritChangeReviewer
+
+    You won't need to instantiate this Class directly.
+    Use ``pGerrit.change.GerritChange.reviewer``
+    """
+    _endpoint = "/a/changes/{}/reviewers/{}"
+    _args = ["id", "account_id"]
+
+    def __init__(self, host, gerritID, account_id, auth=None, verify=True, adapter=None, cache=True, cache_expire=3):
+        """See class docstring."""
+        super().__init__(host, gerritID, auth=auth, verify=verify, adapter=adapter, cache=cache, cache_expire=cache_expire)
+        self.account_id = account_id
+
+    @classmethod
+    @GerritRest.get()
+    def query(self, *args, **kwargs):
+        """Performs a GET request to retrieve information about the change edit.
+
+        **API URL**: `/a/changes/{change_id}/reviewers/ <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#list-reviewers>`__
+
+        **Input type**: None
+        """
+        return urljoin(self.host, urlformat(GerritChangeReviewer._endpoint, self.id, ""))
+
+    @classmethod
+    @GerritRest.get()
+    def suggest_reviewers(self, *args, **kwargs):
+        """Performs a GET request to retrieve a list of suggested reviewers for a change.
+
+        **API URL**: `/a/changes/{change_id}/suggest_reviewers <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#suggest-reviewers>`__
+
+        **Input type**: `SuggestReviewersOptions <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#suggest-reviewers>`__
+
+        **Return type**: List[`SuggestedReviewerInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#suggested-reviewer-info>`__]
 
         Usage::
 
-            current_revision = change.current_revision()
+            reviewer.suggest_reviewers(q="john")
 
         """
-        return GerritChangeRevision(self.host, self.id, "current", auth=self.session.auth, verify=self.verify, adapter=self.adapter, cache=self.cache, cache_expire=self.cache_expire)
+        return urljoin(self.host, urlformat("/a/changes/{}/suggest_reviewers", self.id, "suggest_reviewers"))
+
+    @classmethod
+    @GerritRest.post
+    def add_reviewer(self, payload=None, *args, **kwargs):
+        """Performs a POST request to add a reviewer to a change.
+
+        **API URL**: `/a/changes/{change_id}/reviewers <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#add-reviewer>`__
+
+        **Input type**: `ReviewerInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#reviewer-input>`__
+
+        **Return type**: `ReviewerResult <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#reviewer-result>`__
+
+        Usage::
+
+            reviewer.add_reviewer({"reviewer": "example@example.com"})
+
+        """
+        return urljoin(self.host, urlformat(self._endpoint, self.id, ""))
+
 
 class GerritChangeRevision(GerritChange):
     """Class maps /a/changes/{change_id}/revisions/{revision_id} endpoint of Gerrit REST API
 
     :return: An instance of GerritChangeRevision.
     :rtype: pGerrit.change.GerritChangeRevision
 
@@ -702,15 +826,15 @@
         Usage::
 
             file_instance = revision.file(fileID)
 
         """
         return GerritChangeRevisionFile(self.host, self.id, self.revisionID, fileID, auth=self.session.auth, verify=self.verify, adapter=self.adapter, cache=self.cache, cache_expire=self.cache_expire)
 
-    def reviwer(self, accountID):
+    def reviewer(self, accountID):
         """Get the GerritChangeRevisionReviewer instance for a specific reviewer of the change revision.
 
         :arg str accountID: The ID of the reviewer.
 
         :return: A GerritChangeRevisionReviewer instance for the specified reviewer.
         :rtype: pGerrit.change.GerritChangeRevisionReviewer
 
@@ -888,44 +1012,7 @@
 
             history_log = revision_file.get_history_log(commit='commit_hash')
 
         """
         project = self.info().project
         commit = commit or self.commit().commit
         return urljoin(self.host, "a/plugins", "gitiles", project, "+log", commit, self.fileID)
-
-    @GerritRest.put
-    def edit(self, payload, headers=None):
-        """Edit a specific file in a change revision.
-
-        :param payload: The file content to be updated.
-        :type payload: str
-        :param headers: (optional) Additional headers to send with the request.
-        :type headers: dict
-
-        :return: The URL for the edited file.
-        :rtype: str
-
-        Usage::
-
-            edit_url = revision_file.edit(payload='new_file_content')
-
-        """
-        return urljoin(self.host, "/a/changes/", self.id, "/edit/", urlformat("{}", self.fileID))
-
-    @GerritRest.get()
-    def edit_retrieve(self, headers=None):
-        """Retrieve the content of a specific file in a change revision after editing.
-
-        :param headers: (optional) Additional headers to send with the request.
-        :type headers: dict
-
-        :return: The content of the specified file in the change revision after editing.
-        :rtype: str
-
-        Usage::
-
-            edited_content = revision_file.edit_retrieve()
-
-        """
-        return urljoin(self.host, "/a/changes/", self.id, "/edit/", urlformat("{}", self.fileID))
-
```

### Comparing `pGerrit-0.1.4/pGerrit/client.py` & `pGerrit-0.1.5/pGerrit/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,49 +46,64 @@
         self.adapter = adapter
         self.cache = cache
         self.cache_expire = cache_expire
 
         if auth:
             self.session.auth = auth
 
-        self.kwargs = {"auth": auth, "verify": verify, "adapter":adapter}
+        self.args = [host]
+        self.kwargs = {"auth": auth, "verify": verify, "adapter":adapter, "cache":cache, "cache_expire":cache_expire}
 
         if not self.host.endswith("/"):
             self.host += "/"
 
     def __del__(self):
         self.session.close()
 
     @property
     def change(self):
         """Provides an instance of GerritChange for the given Gerrit client configuration.
 
         :param str id: the Change-id of Gerrit
 
-        :return: An instance of GerritChange.
-        :rtype: pGerrit.change.GerritChange
+        :return: An instance of GerritChangeQueryDescriptor.
+        :rtype: pGerrit.queryDescriptor.GerritChangeQueryDescriptor
 
         Usage::
 
             gerrit_client = GerritClient(...)
             changes = gerrit_client.change.query(...)
-            change = gerrit_client.change(12345)
-
-        Notice that GerritChange class use QueryMeta as metaclass to make query as classmethod
+            change = gerrit_client.change(12345).detail()
         """
-        from pGerrit.change import GerritChange
-        return GerritChange(self.host, gerritID=None, auth=self.session.auth, verify=self.verify, adapter=self.adapter, cache=self.cache, cache_expire=self.cache_expire)
+        from pGerrit.queryDescriptor import GerritChangeQueryDescriptor
+        return GerritChangeQueryDescriptor(self)
 
     @property
     def access(self):
         """Provides an instance of GerritAccess for the given Gerrit client configuration.
 
-        :return: An instance of GerritAccess.
-        :rtype: pGerrit.Access.GerritAccess
+        :return: An instance of GerritAccessQueryDescriptor.
+        :rtype: pGerrit.queryDescriptor.GerritAccessQueryDescriptor
 
         Usage::
 
             gerrit_client = GerritClient(...)
             access = gerrit_client.access.query(...)
         """
-        from pGerrit.Access import GerritAccess
-        return GerritAccess(self.host, auth=self.session.auth, verify=self.verify, adapter=self.adapter, cache=self.cache, cache_expire=self.cache_expire)
+        from pGerrit.queryDescriptor import GerritAccessQueryDescriptor
+        return GerritAccessQueryDescriptor(self)
+
+    @property
+    def project(self):
+        """Provides an instance of GerritProject for the given Gerrit client configuration.
+
+        :return: An instance of GerritProjectQueryDescriptor.
+        :rtype: pGerrit.queryDescriptor.GerritProjectQueryDescriptor
+
+        Usage::
+
+            gerrit_client = GerritClient(...)
+            projects = gerrit_client.project.query(...)
+            project = gerrit_client.project("test")
+        """
+        from pGerrit.queryDescriptor import GerritProjectQueryDescriptor
+        return GerritProjectQueryDescriptor(self)
```

### Comparing `pGerrit-0.1.4/pGerrit/restAPIwrapper.py` & `pGerrit-0.1.5/pGerrit/restAPIwrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 from functools import wraps
-import requests
 from types import SimpleNamespace
 from pGerrit.utils import urljoin, urlformat
-from pGerrit.exception import GerritError
 import json
-
+from typing import Callable
 
 class GerritRest(object):
     """
     docstring for RestAPI
     """
-    def get(raw=False):
+    def get(raw=False) -> Callable:
         def dec_get(func):
             @wraps(func)
             def decorator_get(self, headers={"Accept":"application/json"}, *args, **kwargs):
                 if raw:
                     headers = None
                 url = func(self, headers=headers, *args, **kwargs)
                 url = url if self.session.auth else url.replace("/a/", "/")
                 res = self.session.get(url, headers=headers, verify=self.kwargs["verify"], params=kwargs)
                 res._content = res._content.replace(b")]}'\n", b"")
-                if res.status_code != 200:
-                    raise GerritError(res.status_code, res.content)
+                res.raise_for_status()
 
                 if raw:
                     return res
+                elif res.content == b'':
+                    return res.content
                 else:
                     return res.json(object_hook=lambda d: SimpleNamespace(**d))
             return decorator_get
         return dec_get
 
-    def put(func):
+    def put(func) -> Callable:
         @wraps(func)
         def decorator_put(self, payload=None, headers={"content-type":"application/json"}, *args, **kwargs):
             url = func(self, payload, headers=headers, *args, **kwargs)
             url = url if self.session.auth else url.replace("/a/", "/")
             res = self.session.put(url, payload, headers=headers, verify=self.kwargs["verify"], params=kwargs)
+            res.raise_for_status()
             # res._content = res._content.replace(b")]}'\n", b"")
             # des.resultType
             return res
         return decorator_put
 
-    def post(func):
+    def post(func) -> Callable:
         @wraps(func)
         def decorator_post(self, payload=None, headers={"content-type":"application/json"}, *args, **kwargs):
             url = func(self, payload, headers=headers, *args, **kwargs)
             url = url if self.session.auth else url.replace("/a/", "/")
             res = self.session.post(url, json.dumps(payload), headers=headers, verify=self.kwargs["verify"], params=kwargs)
+            res.raise_for_status()         
             # res._content = res._content.replace(b")]}'\n", b"")
             # des.resultType
             return res
         return decorator_post
 
-    def delete(func):
+    def delete(func) -> Callable:
         @wraps(func)
         def decorator_delete(self, headers={"Accept":"application/json"}, *args, **kwargs):
             url = func(self, headers=headers, *args, **kwargs)
             url = url if self.session.auth else url.replace("/a/", "/")
             res = self.session.delete(url, headers=headers, verify=self.kwargs["verify"], params=kwargs)
+            res.raise_for_status()
             # res._content = res._content.replace(b")]}'\n", b"")
             # des.resultType
             return res
         return decorator_delete
 
-    def url_wrapper(end=None):
+    def url_wrapper(end=None) -> Callable:
         def wrapper(func):
             @wraps(func)
             def decorator_url(self, *args, **kwargs):
-                from pGerrit.change import GerritChange, GerritChangeRevision, GerritChangeRevisionFile
+                from pGerrit.change import GerritChange, GerritChangeRevision, GerritChangeRevisionFile, GerritChangeEdit, GerritChangeReviewer
+                from pGerrit.project import GerritProject
                 name = end if end != None else func.__name__
                 # find the class defined the method
                 cls_d = eval(func.__qualname__.split(".")[-2])
                 # extend all arguments which need to be inserted into endpoint
                 args = []
                 for arg_name in cls_d._args:
                     args.append(getattr(self, arg_name))
```

### Comparing `pGerrit-0.1.4/pGerrit/utils.py` & `pGerrit-0.1.5/pGerrit/utils.py`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.4/pGerrit.egg-info/PKG-INFO` & `pGerrit-0.1.5/pGerrit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pGerrit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A well designed base on decorator pattern library to access Google Gerrit REST API
 Home-page: UNKNOWN
 Author: CY
 Author-email: 17103513@qq.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/demonguy/pGerrit
 Project-URL: Tracker, https://github.com/demonguy/pGerrit/issues
```

### Comparing `pGerrit-0.1.4/setup.cfg` & `pGerrit-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.4/tests/test.py` & `pGerrit-0.1.5/tests/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 import os
 import requests
 
 import unittest
 from pGerrit.client import GerritClient
-from pGerrit.change import GerritChange, GerritChangeRevision, GerritChangeRevisionFile
+from pGerrit.change import GerritChange, GerritChangeRevision, GerritChangeRevisionFile, GerritChangeEdit, GerritChangeReviewer
+from pGerrit.queryDescriptor import GerritChangeEditQueryDescriptor, GerritChangeReviewerQueryDescriptor
 from pGerrit.utils import urljoin
 from requests.auth import HTTPBasicAuth
 from pGerrit.utils import urljoin
 from types import SimpleNamespace
 
 import requests_cache
 requests_cache.disabled()
@@ -36,139 +37,221 @@
 
 g_host =  os.environ.get("GERRIT_HOST")
 assert g_host is not None
 
 g_id = os.environ.get("GERRIT_CHANGE_NUMBER")
 assert g_id is not None
 
+g_file_id = "COMMIT_MSG"
+
+g_pj = os.environ.get("GERRIT_PROJECT_NAME")
+assert g_pj is not None
+
 
 class TestChange(unittest.TestCase):
     """docstring for TestGerrit"""
     def setUp(self):
         requests.packages.urllib3.disable_warnings()
         self.auth = HTTPBasicAuth(g_username, g_password)
         self.client = GerritClient(g_host, auth=self.auth, verify=False, cache=False)
         self.change = self.client.change(g_id)
 
     def tearDown(self):
         pass
 
-    def testChangeDetail(self):
-        detail = self.change.detail(o=["ALL_COMMITS", "CURRENT_REVISION"])
-        self.assertIsInstance(detail, SimpleNamespace)
-        self.assertEqual(detail.branch, "master")
+    def testChangeQuery(self):
+        results = self.client.change.query(q=g_id)
+        self.assertIsInstance(results, list)
+        for result in results:
+            self.assertIsInstance(result, SimpleNamespace)
 
     def testChangeInfo(self):
         info = self.change.info(o=["ALL_COMMITS", "CURRENT_REVISION"])
         self.assertIsInstance(info, SimpleNamespace)
         self.assertEqual(info.branch, "master")
 
-    def testChangeIsMerge(self):
-        self.assertTrue(self.change.is_merge())
-
-    def testChangeCurrentRevision(self):
-        revision = self.change.current_revision()
-        self.assertIsInstance(revision, GerritChangeRevision)
-
-    def testChangeRevision(self):
-        revision = self.change.revision("current")
-        self.assertIsInstance(revision, GerritChangeRevision)
-
-    def testChangeQuery(self):
-        results = self.client.change.query(q=g_id)
-        self.assertIsInstance(results, list)
-        for result in results:
-            self.assertIsInstance(result, SimpleNamespace)
+    def testChangeDetail(self):
+        detail = self.change.detail(o=["ALL_COMMITS", "CURRENT_REVISION"])
+        self.assertIsInstance(detail, SimpleNamespace)
+        self.assertEqual(detail.branch, "master")
 
     def testChangeTopic(self):
         topic = self.change.topic()
         self.assertIsInstance(topic, str)
 
     def testSetChangeTopic(self):
         target_topic = "test_set_topic"
         self.change.set_topic(target_topic)
         topic = self.change.topic()
         self.assertEqual(topic, target_topic)
 
+    def testDeleteChangeTopic(self):
+        self.change.delete_topic()
+        topic = self.change.topic()
+        self.assertEqual(topic, "")
+
     def testChangeSubmitted_together(self):
         submitted_together = self.change.submitted_together()
         self.assertIsInstance(submitted_together, list)
 
     def testChange_in(self):
-        _in = self.change._in()
+        _in = self.change.in_()
         self.assertIsInstance(_in, SimpleNamespace)
 
     def testChangeComments(self):
         comments = self.change.comments()
         self.assertIsInstance(comments, SimpleNamespace)
 
+    def testChangeRobotComments(self):
+        robot_comments = self.change.robotcomments()
+        if len(vars(robot_comments)) == 0:
+            return
+
+        self.assertIsInstance(robot_comments, dict)
+        for key, value in robot_comments.items():
+            self.assertIsInstance(key, str)
+            self.assertIsInstance(value, list)
+            for comment in value:
+                self.assertIsInstance(comment, SimpleNamespace)
+
     def testChangeDrafts(self):
         drafts = self.change.drafts()
         self.assertIsInstance(drafts, SimpleNamespace)
 
     def testChangeCheck(self):
         check = self.change.check()
         self.assertIsInstance(check, SimpleNamespace)
 
+    def testChangeHashtags(self):
+        hashtags = self.change.hashtags()
+        if isinstance(hashtags, SimpleNamespace) and len(vars(hashtags)) == 0:
+            return
+
+        self.assertIsInstance(hashtags, list)
+        for hashtag in hashtags:
+            self.assertIsInstance(hashtag, str)
+
+    def testSetChangeHashtag(self):
+        target_hashtags = ["test1", "test2"]
+        self.change.set_hashtags(payload={"add":target_hashtags})
+        hashtags = self.change.hashtags()
+        self.change.set_hashtags(payload={"remove":target_hashtags})
+        self.assertEqual(set(hashtags), set(target_hashtags))
+
     @unittest.skip("This change cannot be rebased, so skip")
     def testChangeRebase(self):
         rebase = self.change.rebase()
         # self.assertIsInstance(edit, SimpleNamespace)
 
-    @unittest.skip("Edit will return empty unless the change is in the edit status")
-    def testChangeEdit(self):
-        edit = self.change.edit()
-        self.assertIsInstance(edit, SimpleNamespace)
+    def testChangeIsMerge(self):
+        self.assertTrue(self.change.is_merge())
 
-    @unittest.skip("Edit will return empty unless the change is in the edit status")
-    def testChangeEditPublish(self):
-        edit = self.change.edit_publish()
-        self.assertIsInstance(edit, SimpleNamespace)
-
-    @unittest.skip("Edit will return empty unless the change is in the edit status")
-    def testChangeEditDelete(self):
-        edit = self.change.edit_delete()
-        self.assertIsInstance(edit, SimpleNamespace)
-
-    def testChangeReviewers(self):
-        reviewers = self.change.reviewers()
-        self.assertIsInstance(reviewers[0], SimpleNamespace)
-
-    def testChangeAddReviewers(self):
-        payload = {"reviewer":g_username}
-        res = self.change.add_reviewer(payload=payload)
-        self.assertEqual(res.status_code, 200)
+    def testChangeCurrentRevision(self):
+        revision = self.change.current_revision()
+        self.assertIsInstance(revision, GerritChangeRevision)
 
-    def testChangeSuggest_reviewers(self):
-        suggest_reviewers = self.change.suggest_reviewers()
-        self.assertIsInstance(suggest_reviewers[0], SimpleNamespace)
+    def testChangeRevision(self):
+        revision = self.change.revision("current")
+        self.assertIsInstance(revision, GerritChangeRevision)
+
+    def testChangeEdit(self):
+        edit = self.change.edit
+        self.assertIsInstance(edit, GerritChangeEditQueryDescriptor)
+
+    def testChangeReviewer(self):
+        reviewer = self.change.reviewer
+        self.assertIsInstance(reviewer, GerritChangeReviewerQueryDescriptor)
 
 class TestChangeRevisionReviewer(unittest.TestCase):
     """docstring for Test"""
     def setUp(self):
         requests.packages.urllib3.disable_warnings()
         self.auth = HTTPBasicAuth(g_username, g_password)
         self.client = GerritClient(g_host, auth=self.auth, verify=False)
         self.change = self.client.change(g_id)
         self.revision = self.change.revision("1")
         self.current = self.change.current_revision()
-        self.reviewer = self.current.reviwer("")
+        self.reviewer = self.current.reviewer("")
 
     def tearDown(self):
         pass
 
-    def testRevisionReviwerList(self):
+    def testRevisionReviewerList(self):
         files = self.reviewer.list()
         self.assertIsInstance(files, list)
 
     @unittest.skip("Delete vote can only delete others vote, so cannot be idempotent")
-    def testRevisionReviwerDeleteVote(self):
+    def testRevisionReviewerDeleteVote(self):
         files = self.reviewer.delete_vote()
         self.assertIsInstance(files, SimpleNamespace)
 
+class TestGerritChangeReviewer(unittest.TestCase):
+
+    def setUp(self):
+        requests.packages.urllib3.disable_warnings()
+        self.auth = HTTPBasicAuth(g_username, g_password)
+        self.client = GerritClient(g_host, auth=self.auth, verify=False)
+        self.change = self.client.change(g_id)
+        self.revision = self.change.revision("1")
+        self.current = self.change.current_revision()
+        self.reviewer = self.change.reviewer
+
+    def test_query(self):
+        reviewers = self.reviewer.query()
+        if isinstance(reviewers, SimpleNamespace) and len(vars(reviewers)) == 0:
+            return
+
+        self.assertIsInstance(reviewers, list)
+        for reviewer in reviewers:
+            self.assertIsInstance(reviewer, SimpleNamespace)
+
+    def test_suggest_reviewers(self):
+        suggested_reviewers = self.reviewer.suggest_reviewers(q="john")
+        self.assertIsInstance(suggested_reviewers, list)
+
+    @unittest.skip
+    def test_add_reviewer(self):
+        response = self.gerrit_reviewer.add_reviewer({"reviewer": "example@example.com"})
+        self.assertIsNotNone(response)
+
+class TestGerritChangeEdit(unittest.TestCase):
+
+    def setUp(self):
+        requests.packages.urllib3.disable_warnings()
+        self.auth = HTTPBasicAuth(g_username, g_password)
+        self.client = GerritClient(g_host, auth=self.auth, verify=False)
+        self.change = self.client.change(g_id)
+        self.edit = self.change.edit(g_file_id)
+
+    def test_info(self):
+        info = self.change.edit.info()
+        self.assertIsNotNone(info)
+
+    @unittest.skip
+    def test_edit_publish(self):
+        # Create an edit before trying to publish
+        self.edit.edit_file(payload='new_file_content')
+        self.edit.edit_publish()
+
+    @unittest.skip
+    def test_edit_restore(self):
+        # Create an edit before trying to restore
+        self.edit.edit_file(payload='new_file_content')
+        self.edit.edit_restore({"restore_path": "foo"})
+
+    @unittest.skip
+    def test_edit_delete(self):
+        # Create an edit before trying to delete
+        self.edit.edit_file(payload='new_file_content')
+        self.edit.edit_delete()
+
+    @unittest.skip
+    def test_edit_file(self):
+        self.edit.edit_file(payload='new_file_content')
+
 class TestChangeRevision(unittest.TestCase):
     """docstring for Test"""
     def setUp(self):
         requests.packages.urllib3.disable_warnings()
         self.auth = HTTPBasicAuth(g_username, g_password)
         self.client = GerritClient(g_host, auth=self.auth, verify=False)
         self.change = self.client.change(g_id)
@@ -281,7 +364,30 @@
     def tearDown(self):
         pass
 
     def testAccessQuery(self):
         access = self.client.access.query(project="All-Projects")
         self.assertIsInstance(access, SimpleNamespace)
 
+class TestProject(unittest.TestCase):
+    """docstring for TestGerrit"""
+    def setUp(self):
+        requests.packages.urllib3.disable_warnings()
+        self.auth = HTTPBasicAuth(g_username, g_password)
+        self.client = GerritClient(g_host, auth=self.auth, verify=False)
+        self.project = self.client.project(g_pj)
+
+    def tearDown(self):
+        pass
+
+    def testProjectQuery(self):
+        results = self.client.project.query(query=g_pj)
+        self.assertIsInstance(results, list)
+        for result in results:
+            self.assertIsInstance(result, SimpleNamespace)
+
+    def testProjectAccess(self):
+        access = self.project.access()
+        self.assertIsInstance(access, SimpleNamespace)
+
+if __name__ == "__main__":
+    unittest.main()
```

