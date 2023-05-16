# Comparing `tmp/openimis-be-tools-1.5.0.tar.gz` & `tmp/openimis-be-tools-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-tools-1.5.0.tar", last modified: Fri Nov 11 09:46:11 2022, max compression
+gzip compressed data, was "openimis-be-tools-1.5.1.tar", last modified: Tue May 16 22:29:01 2023, max compression
```

## Comparing `openimis-be-tools-1.5.0.tar` & `openimis-be-tools-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:46:11.054205 openimis-be-tools-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-11-11 09:46:11.054205 openimis-be-tools-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:46:11.050205 openimis-be-tools-1.5.0/openimis_be_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-11-11 09:46:10.000000 openimis-be-tools-1.5.0/openimis_be_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-11-11 09:46:11.000000 openimis-be-tools-1.5.0/openimis_be_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 09:46:10.000000 openimis-be-tools-1.5.0/openimis_be_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-11 09:46:10.000000 openimis-be-tools-1.5.0/openimis_be_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-11 09:46:10.000000 openimis-be-tools-1.5.0/openimis_be_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 09:46:11.054205 openimis-be-tools-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-11-11 09:46:10.000000 openimis-be-tools-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:46:11.050205 openimis-be-tools-1.5.0/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:46:11.054205 openimis-be-tools-1.5.0/tools/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/migrations/0002_extract_file_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/migrations/0003_auto_20211220_0920.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/migrations/0004_registers_right_for_scheme_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4446 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)    45619 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:46:11.054205 openimis-be-tools-1.5.0/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13168 2022-11-11 09:46:00.000000 openimis-be-tools-1.5.0/tools/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:29:01.196760 openimis-be-tools-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-16 22:29:01.196760 openimis-be-tools-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:29:01.184759 openimis-be-tools-1.5.1/openimis_be_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-16 22:29:01.000000 openimis-be-tools-1.5.1/openimis_be_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-16 22:29:01.000000 openimis-be-tools-1.5.1/openimis_be_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:29:01.000000 openimis-be-tools-1.5.1/openimis_be_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 22:29:01.000000 openimis-be-tools-1.5.1/openimis_be_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 22:29:01.000000 openimis-be-tools-1.5.1/openimis_be_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:29:01.196760 openimis-be-tools-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-16 22:28:59.000000 openimis-be-tools-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:29:01.188759 openimis-be-tools-1.5.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:29:01.192760 openimis-be-tools-1.5.1/tools/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/migrations/0002_extract_file_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/migrations/0003_auto_20211220_0920.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/migrations/0004_registers_right_for_scheme_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/migrations/0005_items_services_rights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/migrations/0006_update_django_scheme_with_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/migrations/0007_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73009 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:29:01.196760 openimis-be-tools-1.5.1/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/tests/test_upload_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58395 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/tests/test_upload_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22549 2023-05-16 22:28:43.000000 openimis-be-tools-1.5.1/tools/views.py
```

### Comparing `openimis-be-tools-1.5.0/LICENSE.md` & `openimis-be-tools-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.5.0/PKG-INFO` & `openimis-be-tools-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-tools
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Tools reference module.
 Home-page: https://openimis.org/
 Author: Bluesquare
 Author-email: developers@bluesquare.org
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-tools-1.5.0/README.md` & `openimis-be-tools-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.5.0/openimis_be_tools.egg-info/PKG-INFO` & `openimis-be-tools-1.5.1/openimis_be_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-tools
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Tools reference module.
 Home-page: https://openimis.org/
 Author: Bluesquare
 Author-email: developers@bluesquare.org
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-tools-1.5.0/openimis_be_tools.egg-info/SOURCES.txt` & `openimis-be-tools-1.5.1/openimis_be_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,25 @@
 openimis_be_tools.egg-info/requires.txt
 openimis_be_tools.egg-info/top_level.txt
 tools/__init__.py
 tools/admin.py
 tools/apps.py
 tools/constants.py
 tools/models.py
+tools/resources.py
 tools/serializers.py
 tools/services.py
 tools/urls.py
 tools/utils.py
 tools/views.py
 tools/migrations/0001_initial.py
 tools/migrations/0002_extract_file_field.py
 tools/migrations/0003_auto_20211220_0920.py
 tools/migrations/0004_registers_right_for_scheme_admin.py
+tools/migrations/0005_items_services_rights.py
+tools/migrations/0006_update_django_scheme_with_missing_fields.py
+tools/migrations/0007_set_managed_to_true.py
 tools/migrations/__init__.py
 tools/tests/__init__.py
-tools/tests/test_services.py
+tools/tests/test_services.py
+tools/tests/test_upload_items.py
+tools/tests/test_upload_services.py
```

### Comparing `openimis-be-tools-1.5.0/setup.py` & `openimis-be-tools-1.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="openimis-be-tools",
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license="GNU AGPL v3",
     description="The openIMIS Backend Tools reference module.",
     # long_description=README,
     url="https://openimis.org/",
     author="Bluesquare",
@@ -23,14 +23,16 @@
         "django-db-signals",
         "djangorestframework",
         "djangorestframework-xml",
         "simplejson",
         "pyminizip",
         "pyzipper",
         "defusedxml",
+        "tablib",
+        "django-import-export",
     ],
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 2.1",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
```

### Comparing `openimis-be-tools-1.5.0/tools/apps.py` & `openimis-be-tools-1.5.1/tools/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from django.conf import settings
 
 DEFAULT_CFG = {
     "registers_perms": ["131000"],
     "registers_diagnoses_perms": ["131000", "131002", "131001"],
     "registers_health_facilities_perms": ["131000", "131004", "131003"],
     "registers_locations_perms": ["131000", "131006", "131005"],
+    "registers_items_perms": ["131000", "131008", "131007"],
+    "registers_services_perms": ["131000", "131010", "131009"],
     "extracts_master_data_perms": [],
     "extracts_officer_feedbacks_perms": [],
     "extracts_officer_renewals_perms": [],
     "extracts_phone_extract_perms": [],
     "extracts_upload_claims_perms": [],
     "master_data_password": None,
 }
@@ -18,14 +20,16 @@
 class ToolsConfig(AppConfig):
     name = "tools"
 
     registers_perms = []
     registers_diagnoses_perms = []
     registers_health_facilities_perms = []
     registers_locations_perms = []
+    registers_items_perms = []
+    registers_services_perms = []
 
     extracts_master_data_perms = []
     extracts_officer_feedbacks_perms = []
     extracts_officer_renewals_perms = []
     extracts_phone_extract_perms = []
     extracts_upload_claims_perms = []
 
@@ -33,14 +37,16 @@
 
     def _configure_permissions(self, cfg):
         ToolsConfig.registers_perms = cfg["registers_perms"]
         ToolsConfig.registers_diagnoses_perms = cfg["registers_diagnoses_perms"]
         ToolsConfig.registers_health_facilities_perms = cfg[
             "registers_health_facilities_perms"
         ]
+        ToolsConfig.registers_items_perms = cfg["registers_items_perms"]
+        ToolsConfig.registers_services_perms = cfg["registers_services_perms"]
         ToolsConfig.registers_locations_perms = cfg["registers_locations_perms"]
         ToolsConfig.extracts_master_data_perms = cfg["extracts_master_data_perms"]
         ToolsConfig.extracts_phone_extract_perms = cfg["extracts_phone_extract_perms"]
         ToolsConfig.extracts_upload_claims_perms = cfg["extracts_upload_claims_perms"]
 
         ToolsConfig.extracts_officer_feedbacks_perms = cfg[
             "extracts_officer_feedbacks_perms"
```

### Comparing `openimis-be-tools-1.5.0/tools/migrations/0001_initial.py` & `openimis-be-tools-1.5.1/tools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.5.0/tools/migrations/0002_extract_file_field.py` & `openimis-be-tools-1.5.1/tools/migrations/0002_extract_file_field.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.5.0/tools/migrations/0003_auto_20211220_0920.py` & `openimis-be-tools-1.5.1/tools/migrations/0003_auto_20211220_0920.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.5.0/tools/models.py` & `openimis-be-tools-1.5.1/tools/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,9 +40,9 @@
         null=False,
         default=0,
     )
     audit_user_id = models.IntegerField(db_column="AuditUserID")
     stored_file = models.FileField(upload_to="extracts/%Y/%m/", db_column="ExtractFile")
 
     class Meta:
-        managed = False
+        managed = True
         db_table = "tblExtracts"
```

### Comparing `openimis-be-tools-1.5.0/tools/urls.py` & `openimis-be-tools-1.5.1/tools/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 urlpatterns = [
     path("registers/download_locations", views.download_locations),
     path("registers/upload_locations", views.upload_locations),
     path("registers/download_healthfacilities", views.download_health_facilities),
     path("registers/upload_healthfacilities", views.upload_health_facilities),
     path("registers/download_diagnoses", views.download_diagnoses),
     path("registers/upload_diagnoses", views.upload_diagnoses),
+    path("registers/download_items", views.download_items),
+    path("registers/upload_items", views.upload_items),
+    path("registers/download_services", views.download_services),
+    path("registers/upload_services", views.upload_services),
+    path("exports/items", views.export_items),
+    path("imports/items", views.import_items),
+    path("exports/services", views.export_services),
+    path("imports/services", views.import_services),
     path("extracts/download_master_data", csrf_exempt(views.download_master_data)),
     path("extracts/download_phone_extract", views.download_phone_extract),
     path("extracts/download_renewals", csrf_exempt(views.download_renewals)),
     path("extracts/download_feedbacks", csrf_exempt(views.download_feedbacks)),
     path("extracts/upload_claims", csrf_exempt(views.upload_claims)),
     path("extracts/upload_enrollments", csrf_exempt(views.upload_enrollments)),
     path("extracts/upload_renewals", csrf_exempt(views.upload_renewals)),
```

### Comparing `openimis-be-tools-1.5.0/tools/utils.py` & `openimis-be-tools-1.5.1/tools/utils.py`

 * *Files identical despite different names*

