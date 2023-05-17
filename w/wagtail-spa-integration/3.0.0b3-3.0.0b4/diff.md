# Comparing `tmp/wagtail_spa_integration-3.0.0b3.tar.gz` & `tmp/wagtail_spa_integration-3.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_spa_integration-3.0.0b3.tar", max compression
+gzip compressed data, was "wagtail_spa_integration-3.0.0b4.tar", max compression
```

## Comparing `wagtail_spa_integration-3.0.0b3.tar` & `wagtail_spa_integration-3.0.0b4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      740 2023-03-10 16:29:44.029017 wagtail_spa_integration-3.0.0b3/LICENSE
--rw-r--r--   0        0        0      946 2023-03-10 16:29:44.030017 wagtail_spa_integration-3.0.0b3/pyproject.toml
--rw-r--r--   0        0        0       83 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/__init__.py
--rw-r--r--   0        0        0      221 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/apps.py
--rw-r--r--   0        0        0     1260 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/headless_preview_api.py
--rw-r--r--   0        0        0      253 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/serializers.py
--rw-r--r--   0        0        0      423 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/templates/wagtailadmin/pages/_preview_button_on_edit.html
--rw-r--r--   0        0        0        0 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/templatetags/__init__.py
--rw-r--r--   0        0        0      335 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/templatetags/wagtail_spa_integration_tags.py
--rw-r--r--   0        0        0     7981 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/tests.py
--rw-r--r--   0        0        0      500 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/utils.py
--rw-r--r--   0        0        0     8648 2023-03-10 16:29:44.031017 wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/views.py
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 wagtail_spa_integration-3.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0      740 2023-03-13 19:14:33.245788 wagtail_spa_integration-3.0.0b4/LICENSE
+-rw-r--r--   0        0        0      946 2023-03-13 19:14:33.246789 wagtail_spa_integration-3.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/__init__.py
+-rw-r--r--   0        0        0      221 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/apps.py
+-rw-r--r--   0        0        0      289 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/filters.py
+-rw-r--r--   0        0        0     1260 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/headless_preview_api.py
+-rw-r--r--   0        0        0      333 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/serializers.py
+-rw-r--r--   0        0        0      423 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/templates/wagtailadmin/pages/_preview_button_on_edit.html
+-rw-r--r--   0        0        0        0 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/templatetags/__init__.py
+-rw-r--r--   0        0        0      335 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/templatetags/wagtail_spa_integration_tags.py
+-rw-r--r--   0        0        0     9000 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/tests.py
+-rw-r--r--   0        0        0      500 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/utils.py
+-rw-r--r--   0        0        0     9063 2023-03-13 19:14:33.247789 wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/views.py
+-rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 wagtail_spa_integration-3.0.0b4/PKG-INFO
```

### Comparing `wagtail_spa_integration-3.0.0b3/LICENSE` & `wagtail_spa_integration-3.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_spa_integration-3.0.0b3/pyproject.toml` & `wagtail_spa_integration-3.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtail-spa-integration"
-version = "3.0.0b3"
+version = "3.0.0b4"
 description = "Tools for using Wagtail API with JavaScript single page apps"
 authors = ["thelabnyc <thelabdev@thelabnyc.com>"]
 license = "ISC"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     'Environment :: Web Environment',
     'Framework :: Django',
```

### Comparing `wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/headless_preview_api.py` & `wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/headless_preview_api.py`

 * *Files identical despite different names*

### Comparing `wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/tests.py` & `wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -165,31 +165,55 @@
         }
         res = self.client.get(url, params)
 
         self.assertEqual(res.status_code, 404)
 
     def test_sitemap_with_site(self):
         home = Page.objects.last()
-        site2_hostname = "http://example.com"
-        site2 = Site.objects.create(root_page=home, hostname=site2_hostname)
-        params = {"site": site2.id}
+        site_hostname = "http://example.com"
+        site = Site.objects.create(root_page=home, hostname=site_hostname)
+        params = {"site": site.hostname}
         request = RequestFactory().get("sitemap.xml", params)
         res = sitemap(request)
         res.render()
-        self.assertContains(res, site2_hostname)
+        self.assertContains(res, site_hostname)
 
     def test_redirect_viewset(self):
+        home = Page.objects.last()
+        site_hostname = "http://example.com"
+        site = Site.objects.create(root_page=home, hostname=site_hostname)
         params = {"old_path": "/lol/"}
         request = APIRequestFactory().get("", params)
         redirect_list = RedirectViewSet.as_view({"get": "list"})
-        Redirect.objects.create(old_path="/lol/", redirect_link="https://example.com")
-        Redirect.objects.create(old_path="/test/", redirect_link="https://no.com")
+        Redirect.objects.create(
+            old_path="/lol/", redirect_link="https://example.com", site=site
+        )
+        Redirect.objects.create(
+            old_path="/test/", redirect_link="https://no.com", site=site
+        )
         response = redirect_list(request)
         self.assertContains(response, "example.com")
         self.assertNotContains(response, "no.com")
+        self.assertEqual(response.data[0]["site"], site_hostname)
+
+    def test_redirect_viewset_by_site_filter(self):
+        home = Page.objects.last()
+        site_hostname = "http://example.com"
+        site_hostname2 = "http://foo.com"
+        site = Site.objects.create(root_page=home, hostname=site_hostname)
+        site2 = Site.objects.create(root_page=home, hostname=site_hostname2)
+        Redirect.objects.create(site=site)
+        Redirect.objects.create(site=site2)
+
+        params = {"site": site_hostname}
+        request = APIRequestFactory().get("", params)
+        redirect_list = RedirectViewSet.as_view({"get": "list"})
+        response = redirect_list(request)
+        self.assertEqual(len(response.data), 1)
+        self.assertEqual(response.data[0]["site"], site_hostname)
 
     def test_exclude_type(self):
         home = Page.objects.last()
         foo = FooPage(title="foo")
         home.add_child(instance=foo)
         params = {"exclude_type": "sandbox.FooPage"}
         request = APIRequestFactory().get("", params)
```

### Comparing `wagtail_spa_integration-3.0.0b3/wagtail_spa_integration/views.py` & `wagtail_spa_integration-3.0.0b4/wagtail_spa_integration/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from wagtail.api.v2.views import PagesAPIViewSet
 from wagtail.api.v2.utils import BadRequestError, page_models_from_string
 from wagtail.contrib.sitemaps.views import sitemap as wagtail_sitemap
 from wagtail.contrib.redirects.models import Redirect
 from wagtail.models import Site, Page, Revision
 from rest_framework import viewsets, permissions
 from rest_framework.response import Response
+from .filters import RedirectFilter
 from .serializers import RedirectSerializer
 from .utils import exclude_page_type, hash_draft_code
 
 
 class SPAExtendedPagesAPIEndpoint(PagesAPIViewSet):
     """
     Wagtail preview doesn't work with a JS client
@@ -112,14 +113,15 @@
         This can be useful with node, which has complications when handling redirects in a
         different manner than a web browser.
         """
         has_draft_param = bool(request.GET.get("draft"))
         queryset = self.get_queryset(include_drafts=has_draft_param)
 
         if has_draft_param:
+            self.set_request_site()
             # We have to reimplement some of wagtail's logic to include unpublished pages
             if not hasattr(self.request, "_wagtail_site"):
                 raise BadRequestError("Site not found")
             root_page = self.request._wagtail_site.root_page.specific
             path = request.GET["html_path"]
             path_components = [component for component in path.split("/") if component]
             obj = self.route(root_page, request, path_components)
@@ -149,23 +151,33 @@
             queryset = super().get_queryset()
             queryset = self.exclude_page_types(queryset)
             if self.check_valid_draft_code():
                 # We can't remove from a queryset
                 queryset = queryset.include_drafts_instead_of_live_public()
             return queryset
         """
+        self.set_request_site()
         queryset = super().get_queryset()
         if include_drafts or self.kwargs.get("is_draft_code_valid"):
             queryset = queryset | Page.objects.filter(live=False)
         else:
             queryset = queryset.public()
 
         queryset = self.exclude_page_types(queryset)
         return queryset
 
+    def set_request_site(self):
+        site_hostname = self.request.GET.get("site", None)
+        if site_hostname:
+            try:
+                site = Site.objects.get(hostname=site_hostname)
+                self.request._wagtail_site = site
+            except Site.DoesNotExist:
+                pass
+
     def exclude_page_types(self, queryset):
         exclude_type = self.request.GET.get("exclude_type", None)
         if exclude_type is not None:
             try:
                 models = page_models_from_string(exclude_type)
             except (LookupError, ValueError):
                 raise BadRequestError("type doesn't exist")
@@ -186,30 +198,30 @@
 
 
 class RedirectViewSet(viewsets.ReadOnlyModelViewSet):
     queryset = Redirect.objects.all()
     serializer_class = RedirectSerializer
     permission_classes = [permissions.AllowAny]
     filter_backends = (filters.DjangoFilterBackend,)
-    filterset_fields = ("old_path", "site")
+    filterset_class = RedirectFilter
     model = Redirect
 
     @classmethod
     def get_urlpatterns(cls):
         """
         This returns a list of URL patterns for the endpoint
         """
         return [
             url(r"^$", cls.as_view({"get": "list"})),
         ]
 
 
 def sitemap(request, sitemaps=None, **kwargs):
-    """Extended wagtail sitemap view. Adds `site` query parameter to site site ID"""
-    site_id = request.GET.get("site", None)
-    if site_id:
+    """Extended wagtail sitemap view. Adds `site` query parameter to site hostname"""
+    hostname = request.GET.get("site", None)
+    if hostname:
         try:
-            request._wagtail_site = Site.objects.get(id=site_id)
+            request._wagtail_site = Site.objects.get(hostname=hostname)
         except Site.DoesNotExist:
             pass
 
     return wagtail_sitemap(request, sitemaps=sitemaps, **kwargs)
```

### Comparing `wagtail_spa_integration-3.0.0b3/PKG-INFO` & `wagtail_spa_integration-3.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-spa-integration
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Tools for using Wagtail API with JavaScript single page apps
 License: ISC
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

