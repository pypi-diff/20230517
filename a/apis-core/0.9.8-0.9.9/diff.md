# Comparing `tmp/apis-core-0.9.8.tar.gz` & `tmp/apis-core-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apis-core-0.9.8.tar", last modified: Mon Dec 17 19:15:24 2018, max compression
+gzip compressed data, was "dist/apis-core-0.9.9.tar", last modified: Tue Dec 18 13:59:55 2018, max compression
```

## Comparing `apis-core-0.9.8.tar` & `apis-core-0.9.9.tar`

### file list

```diff
@@ -1,251 +1,252 @@
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4239 2018-12-07 10:25:34.000000 apis-core-0.9.8/README.rst
--rwxrwxrwx   0 sennierer  (1000) sennierer  (1000)      418 2018-11-20 12:29:27.000000 apis-core-0.9.8/MANIFEST.in
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6128 2018-12-17 19:15:24.000000 apis-core-0.9.8/PKG-INFO
--rwxr-xr-x   0 sennierer  (1000) sennierer  (1000)     2544 2018-12-17 19:15:03.000000 apis-core-0.9.8/setup.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core.egg-info/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      410 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core.egg-info/requires.txt
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      399 2018-12-17 15:45:44.000000 apis-core-0.9.8/apis_core.egg-info/bower.json
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6128 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core.egg-info/PKG-INFO
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        1 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core.egg-info/dependency_links.txt
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       10 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core.egg-info/top_level.txt
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    11983 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core.egg-info/SOURCES.txt
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_vocabularies/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_vocabularies/migrations/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13191 2018-10-03 13:10:44.000000 apis-core-0.9.8/apis_core/apis_vocabularies/migrations/0001_initial.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_vocabularies/migrations/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      348 2018-10-03 13:43:41.000000 apis-core-0.9.8/apis_core/apis_vocabularies/urls.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       63 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_vocabularies/views.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5642 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_vocabularies/api_views.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2561 2018-11-09 09:17:27.000000 apis-core-0.9.8/apis_core/apis_vocabularies/admin.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      104 2018-10-02 14:27:49.000000 apis-core-0.9.8/apis_core/apis_vocabularies/apps.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_vocabularies/tests.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_vocabularies/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5022 2018-11-20 15:47:57.000000 apis-core-0.9.8/apis_core/apis_vocabularies/serializers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     9977 2018-10-03 10:13:44.000000 apis-core-0.9.8/apis_core/apis_vocabularies/models.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     7383 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/urls.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/templates/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/templates/apis_templates/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      584 2018-10-05 12:53:27.000000 apis-core-0.9.8/apis_core/templates/apis_templates/_ajax_form.html
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/templates/apis_templates/registration/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      985 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/templates/apis_templates/registration/registration_closed.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1242 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/templates/apis_templates/registration/registration_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      574 2018-10-05 12:53:27.000000 apis-core-0.9.8/apis_core/templates/apis_templates/_ajax_form_generic.html
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      575 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/vocabs_base2.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      340 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/AddRelation.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      411 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/openskos.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1967 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/stanbol.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      410 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/vocabs_base.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      304 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/Ort.html
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_entities/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_entities/migrations/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3544 2018-10-03 13:10:44.000000 apis-core-0.9.8/apis_core/apis_entities/migrations/0001_initial.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_entities/migrations/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3284 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_entities/tables.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     7040 2018-10-04 07:57:47.000000 apis-core-0.9.8/apis_core/apis_entities/test_parsers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1506 2018-11-19 14:12:16.000000 apis-core-0.9.8/apis_core/apis_entities/fields.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    14205 2018-12-11 10:04:21.000000 apis-core-0.9.8/apis_core/apis_entities/forms.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1007 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_entities/test_forms.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1039 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_entities/test_api.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2816 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_entities/urls.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    21215 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_entities/views.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    14384 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_entities/api_views.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_entities/templates/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      909 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/institution_list.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    20039 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_create.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1036 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/confirm_delete.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      976 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_create_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      974 2018-12-07 12:16:24.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/work_create_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      328 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/place_list_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      332 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_list_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6838 2018-12-17 15:35:42.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/apis_templatetag.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    11606 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_create_new.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13269 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/place_create.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     9573 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/network_institution.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      974 2018-12-07 15:58:51.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/event_create_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2345 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/place_list.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      328 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/event_list_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6676 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/place_create_generic.html
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/detail_views/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1429 2018-12-08 15:43:11.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/detail_views/person_detail_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    11705 2018-12-08 15:43:11.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/detail_views/entity_detail_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    21363 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/institution_create.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      456 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/compare_base.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2996 2018-12-07 10:35:51.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/institution_create_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      352 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/institution_list_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    27549 2018-12-17 12:56:59.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/generic_network_visualization.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     9822 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/generic_list.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      279 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/apis_create_entities.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      324 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/work_list_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13624 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/entity_create_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      902 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_list.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3675 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/map_list.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     9417 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/network.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      152 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_entities/admin.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5469 2018-11-21 10:17:39.000000 apis-core-0.9.8/apis_core/apis_entities/serializers_generic.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5225 2018-10-22 13:10:24.000000 apis-core-0.9.8/apis_core/apis_entities/test_models.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       96 2018-10-02 13:50:04.000000 apis-core-0.9.8/apis_core/apis_entities/apps.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_entities/tests.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_entities/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2176 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_entities/api_renderers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2112 2018-10-02 13:51:30.000000 apis-core-0.9.8/apis_core/apis_entities/autocomplete_light_registry.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     8847 2018-11-09 09:17:27.000000 apis-core-0.9.8/apis_core/apis_entities/filters.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    10640 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_entities/views2.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6788 2018-12-07 12:04:12.000000 apis-core-0.9.8/apis_core/apis_entities/serializers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     8461 2018-12-07 12:04:32.000000 apis-core-0.9.8/apis_core/apis_entities/models.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    15587 2018-10-11 13:05:41.000000 apis-core-0.9.8/apis_core/apis_entities/autocomplete3.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      734 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_entities/custom_authentication.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1254 2018-11-09 16:21:07.000000 apis-core-0.9.8/apis_core/apis_entities/api_urls.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_entities/custom_autocompletes.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5167 2018-12-07 10:25:34.000000 apis-core-0.9.8/apis_core/apis_entities/detail_views.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/helper_functions/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5921 2018-10-02 14:18:48.000000 apis-core-0.9.8/apis_core/helper_functions/stanbolQueries.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2686 2018-10-02 14:16:12.000000 apis-core-0.9.8/apis_core/helper_functions/dl_models.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/helper_functions/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5238 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/helper_functions/highlighter.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     7458 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/helper_functions/inter_annotator_agreement.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    15882 2018-12-17 14:28:26.000000 apis-core-0.9.8/apis_core/helper_functions/RDFparsers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      789 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/helper_functions/utils.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/__init__.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_tei/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      249 2018-11-13 09:29:20.000000 apis-core-0.9.8/apis_core/apis_tei/tei_urls.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      805 2018-11-13 09:29:20.000000 apis-core-0.9.8/apis_core/apis_tei/partials.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    10567 2018-12-07 10:25:34.000000 apis-core-0.9.8/apis_core/apis_tei/tei.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-13 09:29:20.000000 apis-core-0.9.8/apis_core/apis_tei/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1350 2018-11-13 09:29:20.000000 apis-core-0.9.8/apis_core/apis_tei/tei_ac.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/default_settings/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    15423 2018-06-22 07:05:40.000000 apis-core-0.9.8/apis_core/default_settings/NER_settings.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-20 11:42:03.000000 apis-core-0.9.8/apis_core/default_settings/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    14388 2018-11-09 09:17:27.000000 apis-core-0.9.8/apis_core/default_settings/RDF_settings.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/context_processors/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1191 2018-11-09 09:17:27.000000 apis-core-0.9.8/apis_core/context_processors/custom_context_processors.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-20 11:42:31.000000 apis-core-0.9.8/apis_core/context_processors/__init__.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_labels/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_labels/migrations/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      734 2018-10-03 13:10:44.000000 apis-core-0.9.8/apis_core/apis_labels/migrations/0001_initial.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      834 2018-10-03 13:10:44.000000 apis-core-0.9.8/apis_core/apis_labels/migrations/0002_auto_20181003_1310.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_labels/migrations/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      927 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_labels/forms.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      400 2018-10-02 14:20:20.000000 apis-core-0.9.8/apis_core/apis_labels/urls.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1453 2018-10-03 09:55:50.000000 apis-core-0.9.8/apis_core/apis_labels/views.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_labels/templates/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_labels/templates/apis_labels/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      286 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_labels/templates/apis_labels/label_al.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1184 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_labels/templates/apis_labels/label_create.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      793 2018-10-23 10:41:18.000000 apis-core-0.9.8/apis_core/apis_labels/templates/apis_labels/labels_list.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      118 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_labels/admin.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       92 2018-10-02 14:19:11.000000 apis-core-0.9.8/apis_core/apis_labels/apps.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_labels/tests.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_labels/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1315 2018-10-03 09:52:32.000000 apis-core-0.9.8/apis_core/apis_labels/autocomplete_light_registry.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      333 2018-11-20 15:45:11.000000 apis-core-0.9.8/apis_core/apis_labels/serializers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1316 2018-10-03 13:02:31.000000 apis-core-0.9.8/apis_core/apis_labels/models.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_relations/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_relations/migrations/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13489 2018-10-03 13:10:44.000000 apis-core-0.9.8/apis_core/apis_relations/migrations/0001_initial.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_relations/migrations/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      814 2018-11-21 15:43:59.000000 apis-core-0.9.8/apis_core/apis_relations/migrations/0002_auto_20181121_1543.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6260 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_relations/tables.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3513 2018-10-03 13:41:59.000000 apis-core-0.9.8/apis_core/apis_relations/forms.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_relations/rel_tables.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      648 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_relations/urls.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    11434 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_relations/views.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4958 2018-10-03 13:07:33.000000 apis-core-0.9.8/apis_core/apis_relations/api_views.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_relations/templates/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      244 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_placeWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      145 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_workWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      244 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_eventWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      141 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_persPers_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      250 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_instWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      139 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_persPlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      137 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_eventWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      149 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_persPers_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      584 2018-10-05 12:53:27.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      131 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_persPlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      209 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_tables_default.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      129 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_placeWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      131 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_persEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      147 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      145 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_persInst_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      136 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_instPlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      137 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_placeWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      138 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_placeEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      238 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_generic_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      265 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_persPerson_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      139 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_persEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      138 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_persWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      245 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_placeEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      159 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_instInst_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      245 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_persWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      432 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_generic_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      251 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_instPlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      144 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_instPlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      143 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_instWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      263 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_placePlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      131 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_persLabel_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      147 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_placePlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      139 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_placePlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      147 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_eventEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      275 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_instInst_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      129 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_eventWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      136 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_instEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      252 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_persInstitution_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      130 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_placeEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      246 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_persPlace_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      130 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_persWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      576 2018-10-05 12:53:27.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/_ajax_form_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      135 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_instWork_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      246 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_persEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      182 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_generic_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      238 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_Uri_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      151 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_instInst_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      251 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/delete_button_instEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      137 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/edit_button_persInst_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4977 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/relations_detail_generic.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      144 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/rev_button_instEvent_ajax_form.html
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      131 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/admin.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       98 2018-10-02 14:22:46.000000 apis-core-0.9.8/apis_core/apis_relations/apps.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_relations/templatetags/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-20 12:30:09.000000 apis-core-0.9.8/apis_core/apis_relations/templatetags/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      467 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/templatetags/apis_helpers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/tests.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     7537 2018-10-03 13:41:35.000000 apis-core-0.9.8/apis_core/apis_relations/autocomplete_light_registry.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1840 2018-11-09 09:17:27.000000 apis-core-0.9.8/apis_core/apis_relations/rel_views.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      853 2018-11-01 13:14:44.000000 apis-core-0.9.8/apis_core/apis_relations/rel_forms.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2504 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_relations/serializers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    28392 2018-11-09 15:43:35.000000 apis-core-0.9.8/apis_core/apis_relations/models.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13006 2018-12-11 10:16:04.000000 apis-core-0.9.8/apis_core/apis_relations/forms2.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    76967 2018-10-02 14:25:07.000000 apis-core-0.9.8/apis_core/apis_relations/forms_backup.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_metainfo/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_metainfo/migrations/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4303 2018-10-03 13:10:44.000000 apis-core-0.9.8/apis_core/apis_metainfo/migrations/0001_initial.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2141 2018-10-03 13:10:44.000000 apis-core-0.9.8/apis_core/apis_metainfo/migrations/0002_auto_20181003_1310.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.8/apis_core/apis_metainfo/migrations/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       63 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_metainfo/views.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      945 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_metainfo/api_views.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_metainfo/templates/
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_metainfo/templates/apis_metainfo/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1656 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_metainfo/templates/apis_metainfo/TEI_renderer.xml
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      200 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_metainfo/admin.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2002 2018-10-22 14:52:25.000000 apis-core-0.9.8/apis_core/apis_metainfo/test_models.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       96 2018-10-02 14:21:10.000000 apis-core-0.9.8/apis_core/apis_metainfo/apps.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_metainfo/tests.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_metainfo/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      798 2018-10-03 09:56:33.000000 apis-core-0.9.8/apis_core/apis_metainfo/api_renderers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2495 2018-12-07 12:04:12.000000 apis-core-0.9.8/apis_core/apis_metainfo/serializers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)    16898 2018-12-17 14:04:39.000000 apis-core-0.9.8/apis_core/apis_metainfo/models.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      501 2018-10-02 12:27:59.000000 apis-core-0.9.8/apis_core/apis_metainfo/validators.py
-drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-17 19:15:24.000000 apis-core-0.9.8/apis_core/apis_vis/
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      727 2018-12-17 13:34:18.000000 apis-core-0.9.8/apis_core/apis_vis/urls.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4942 2018-12-17 13:34:18.000000 apis-core-0.9.8/apis_core/apis_vis/views.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1316 2018-12-17 13:41:01.000000 apis-core-0.9.8/apis_core/apis_vis/api_views.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       91 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_vis/apps.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_vis/__init__.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2255 2018-12-17 13:54:33.000000 apis-core-0.9.8/apis_core/apis_vis/serializers.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)      280 2018-12-10 17:53:56.000000 apis-core-0.9.8/apis_core/apis_vis/utils.py
--rw-r--r--   0 sennierer  (1000) sennierer  (1000)       38 2018-12-17 19:15:24.000000 apis-core-0.9.8/setup.cfg
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4239 2018-12-07 10:25:34.000000 apis-core-0.9.9/README.rst
+-rwxrwxrwx   0 sennierer  (1000) sennierer  (1000)      418 2018-11-20 12:29:27.000000 apis-core-0.9.9/MANIFEST.in
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6128 2018-12-18 13:59:55.000000 apis-core-0.9.9/PKG-INFO
+-rwxr-xr-x   0 sennierer  (1000) sennierer  (1000)     2544 2018-12-18 13:59:48.000000 apis-core-0.9.9/setup.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core.egg-info/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      410 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core.egg-info/requires.txt
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      399 2018-12-18 13:56:35.000000 apis-core-0.9.9/apis_core.egg-info/bower.json
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6128 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core.egg-info/PKG-INFO
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        1 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core.egg-info/dependency_links.txt
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       10 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core.egg-info/top_level.txt
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    12070 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core.egg-info/SOURCES.txt
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_vocabularies/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_vocabularies/migrations/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13191 2018-10-03 13:10:44.000000 apis-core-0.9.9/apis_core/apis_vocabularies/migrations/0001_initial.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_vocabularies/migrations/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      348 2018-10-03 13:43:41.000000 apis-core-0.9.9/apis_core/apis_vocabularies/urls.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       63 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_vocabularies/views.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5642 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_vocabularies/api_views.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2561 2018-11-09 09:17:27.000000 apis-core-0.9.9/apis_core/apis_vocabularies/admin.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      104 2018-10-02 14:27:49.000000 apis-core-0.9.9/apis_core/apis_vocabularies/apps.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_vocabularies/tests.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_vocabularies/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5022 2018-11-20 15:47:57.000000 apis-core-0.9.9/apis_core/apis_vocabularies/serializers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     9977 2018-10-03 10:13:44.000000 apis-core-0.9.9/apis_core/apis_vocabularies/models.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     7383 2018-12-10 17:53:56.000000 apis-core-0.9.9/apis_core/urls.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/templates/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/templates/apis_templates/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      584 2018-10-05 12:53:27.000000 apis-core-0.9.9/apis_core/templates/apis_templates/_ajax_form.html
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/templates/apis_templates/registration/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      985 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/templates/apis_templates/registration/registration_closed.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1242 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/templates/apis_templates/registration/registration_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      574 2018-10-05 12:53:27.000000 apis-core-0.9.9/apis_core/templates/apis_templates/_ajax_form_generic.html
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      575 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/vocabs_base2.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      340 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/AddRelation.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      411 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/openskos.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1967 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/stanbol.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      410 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/vocabs_base.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      304 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/Ort.html
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_entities/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_entities/migrations/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3544 2018-10-03 13:10:44.000000 apis-core-0.9.9/apis_core/apis_entities/migrations/0001_initial.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_entities/migrations/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3284 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_entities/tables.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     7040 2018-10-04 07:57:47.000000 apis-core-0.9.9/apis_core/apis_entities/test_parsers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2245 2018-12-18 11:54:35.000000 apis-core-0.9.9/apis_core/apis_entities/fields.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    14209 2018-12-18 11:29:23.000000 apis-core-0.9.9/apis_core/apis_entities/forms.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1007 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_entities/test_forms.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1039 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_entities/test_api.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2816 2018-12-10 17:53:56.000000 apis-core-0.9.9/apis_core/apis_entities/urls.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    21215 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_entities/views.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    14384 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_entities/api_views.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_entities/templates/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      909 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/institution_list.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    20039 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_create.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1036 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/confirm_delete.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      976 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_create_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      974 2018-12-07 12:16:24.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/work_create_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      328 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/place_list_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      332 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_list_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6838 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/apis_templatetag.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    11606 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_create_new.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13269 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/place_create.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     9573 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/network_institution.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      974 2018-12-07 15:58:51.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/event_create_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2345 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/place_list.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      328 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/event_list_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6676 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/place_create_generic.html
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/detail_views/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1429 2018-12-08 15:43:11.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/detail_views/person_detail_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    11705 2018-12-08 15:43:11.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/detail_views/entity_detail_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    21363 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/institution_create.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      456 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/compare_base.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2996 2018-12-07 10:35:51.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/institution_create_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    22625 2018-12-18 10:22:52.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/generic_network_visualization_bak.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      352 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/institution_list_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    27779 2018-12-18 10:25:25.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/generic_network_visualization.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     9822 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/generic_list.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      279 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/apis_create_entities.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      324 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/work_list_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13624 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/entity_create_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      902 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_list.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3675 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/map_list.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     9417 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/network.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      152 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_entities/admin.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5469 2018-11-21 10:17:39.000000 apis-core-0.9.9/apis_core/apis_entities/serializers_generic.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5225 2018-10-22 13:10:24.000000 apis-core-0.9.9/apis_core/apis_entities/test_models.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       96 2018-10-02 13:50:04.000000 apis-core-0.9.9/apis_core/apis_entities/apps.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_entities/tests.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_entities/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2176 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_entities/api_renderers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2112 2018-10-02 13:51:30.000000 apis-core-0.9.9/apis_core/apis_entities/autocomplete_light_registry.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     8847 2018-11-09 09:17:27.000000 apis-core-0.9.9/apis_core/apis_entities/filters.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    10640 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_entities/views2.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6788 2018-12-07 12:04:12.000000 apis-core-0.9.9/apis_core/apis_entities/serializers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     8461 2018-12-07 12:04:32.000000 apis-core-0.9.9/apis_core/apis_entities/models.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    15587 2018-10-11 13:05:41.000000 apis-core-0.9.9/apis_core/apis_entities/autocomplete3.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      734 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_entities/custom_authentication.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1254 2018-11-09 16:21:07.000000 apis-core-0.9.9/apis_core/apis_entities/api_urls.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_entities/custom_autocompletes.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5167 2018-12-07 10:25:34.000000 apis-core-0.9.9/apis_core/apis_entities/detail_views.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/helper_functions/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5921 2018-10-02 14:18:48.000000 apis-core-0.9.9/apis_core/helper_functions/stanbolQueries.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2686 2018-10-02 14:16:12.000000 apis-core-0.9.9/apis_core/helper_functions/dl_models.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/helper_functions/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     5238 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/helper_functions/highlighter.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     7458 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/helper_functions/inter_annotator_agreement.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    15882 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/helper_functions/RDFparsers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      789 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/helper_functions/utils.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/__init__.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_tei/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      249 2018-11-13 09:29:20.000000 apis-core-0.9.9/apis_core/apis_tei/tei_urls.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      805 2018-11-13 09:29:20.000000 apis-core-0.9.9/apis_core/apis_tei/partials.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    10567 2018-12-07 10:25:34.000000 apis-core-0.9.9/apis_core/apis_tei/tei.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-13 09:29:20.000000 apis-core-0.9.9/apis_core/apis_tei/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1350 2018-11-13 09:29:20.000000 apis-core-0.9.9/apis_core/apis_tei/tei_ac.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/default_settings/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    15423 2018-06-22 07:05:40.000000 apis-core-0.9.9/apis_core/default_settings/NER_settings.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-20 11:42:03.000000 apis-core-0.9.9/apis_core/default_settings/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    14388 2018-11-09 09:17:27.000000 apis-core-0.9.9/apis_core/default_settings/RDF_settings.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/context_processors/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1191 2018-11-09 09:17:27.000000 apis-core-0.9.9/apis_core/context_processors/custom_context_processors.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-20 11:42:31.000000 apis-core-0.9.9/apis_core/context_processors/__init__.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_labels/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_labels/migrations/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      734 2018-10-03 13:10:44.000000 apis-core-0.9.9/apis_core/apis_labels/migrations/0001_initial.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      834 2018-10-03 13:10:44.000000 apis-core-0.9.9/apis_core/apis_labels/migrations/0002_auto_20181003_1310.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_labels/migrations/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      927 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_labels/forms.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      400 2018-10-02 14:20:20.000000 apis-core-0.9.9/apis_core/apis_labels/urls.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1453 2018-10-03 09:55:50.000000 apis-core-0.9.9/apis_core/apis_labels/views.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_labels/templates/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_labels/templates/apis_labels/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      286 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_labels/templates/apis_labels/label_al.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1184 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_labels/templates/apis_labels/label_create.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      793 2018-10-23 10:41:18.000000 apis-core-0.9.9/apis_core/apis_labels/templates/apis_labels/labels_list.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      118 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_labels/admin.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       92 2018-10-02 14:19:11.000000 apis-core-0.9.9/apis_core/apis_labels/apps.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_labels/tests.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_labels/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1315 2018-10-03 09:52:32.000000 apis-core-0.9.9/apis_core/apis_labels/autocomplete_light_registry.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      333 2018-11-20 15:45:11.000000 apis-core-0.9.9/apis_core/apis_labels/serializers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1316 2018-10-03 13:02:31.000000 apis-core-0.9.9/apis_core/apis_labels/models.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_relations/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_relations/migrations/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13489 2018-10-03 13:10:44.000000 apis-core-0.9.9/apis_core/apis_relations/migrations/0001_initial.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_relations/migrations/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      814 2018-11-21 15:43:59.000000 apis-core-0.9.9/apis_core/apis_relations/migrations/0002_auto_20181121_1543.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6260 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_relations/tables.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3513 2018-10-03 13:41:59.000000 apis-core-0.9.9/apis_core/apis_relations/forms.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_relations/rel_tables.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      648 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_relations/urls.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    11434 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_relations/views.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4958 2018-10-03 13:07:33.000000 apis-core-0.9.9/apis_core/apis_relations/api_views.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_relations/templates/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      244 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_placeWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      145 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_workWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      244 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_eventWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      141 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_persPers_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      250 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_instWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      139 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_persPlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      137 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_eventWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      149 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_persPers_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      584 2018-10-05 12:53:27.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      131 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_persPlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      209 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_tables_default.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      129 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_placeWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      131 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_persEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      147 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      145 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_persInst_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      136 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_instPlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      137 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_placeWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      138 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_placeEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      238 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_generic_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      265 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_persPerson_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      139 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_persEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      138 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_persWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      245 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_placeEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      159 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_instInst_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      245 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_persWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      432 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_generic_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      251 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_instPlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      144 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_instPlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      143 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_instWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      263 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_placePlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      131 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_persLabel_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      147 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_placePlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      139 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_placePlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      147 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_eventEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      275 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_instInst_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      129 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_eventWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      136 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_instEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      252 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_persInstitution_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      130 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_placeEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      246 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_persPlace_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      130 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_persWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      576 2018-10-05 12:53:27.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/_ajax_form_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      135 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_instWork_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      246 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_persEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      182 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_generic_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      238 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_Uri_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      151 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_instInst_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      251 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/delete_button_instEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      137 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/edit_button_persInst_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4977 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/relations_detail_generic.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      144 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/rev_button_instEvent_ajax_form.html
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      131 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/admin.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       98 2018-10-02 14:22:46.000000 apis-core-0.9.9/apis_core/apis_relations/apps.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_relations/templatetags/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-11-20 12:30:09.000000 apis-core-0.9.9/apis_core/apis_relations/templatetags/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      467 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/templatetags/apis_helpers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/tests.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     7537 2018-10-03 13:41:35.000000 apis-core-0.9.9/apis_core/apis_relations/autocomplete_light_registry.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1840 2018-11-09 09:17:27.000000 apis-core-0.9.9/apis_core/apis_relations/rel_views.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      853 2018-11-01 13:14:44.000000 apis-core-0.9.9/apis_core/apis_relations/rel_forms.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2504 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_relations/serializers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    28392 2018-11-09 15:43:35.000000 apis-core-0.9.9/apis_core/apis_relations/models.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    13006 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_relations/forms2.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    76967 2018-10-02 14:25:07.000000 apis-core-0.9.9/apis_core/apis_relations/forms_backup.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_metainfo/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_metainfo/migrations/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     4303 2018-10-03 13:10:44.000000 apis-core-0.9.9/apis_core/apis_metainfo/migrations/0001_initial.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2141 2018-10-03 13:10:44.000000 apis-core-0.9.9/apis_core/apis_metainfo/migrations/0002_auto_20181003_1310.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-05 10:54:37.000000 apis-core-0.9.9/apis_core/apis_metainfo/migrations/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       63 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_metainfo/views.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      945 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_metainfo/api_views.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_metainfo/templates/
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_metainfo/templates/apis_metainfo/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1656 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_metainfo/templates/apis_metainfo/TEI_renderer.xml
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      200 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_metainfo/admin.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2002 2018-10-22 14:52:25.000000 apis-core-0.9.9/apis_core/apis_metainfo/test_models.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       96 2018-10-02 14:21:10.000000 apis-core-0.9.9/apis_core/apis_metainfo/apps.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       60 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_metainfo/tests.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_metainfo/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      798 2018-10-03 09:56:33.000000 apis-core-0.9.9/apis_core/apis_metainfo/api_renderers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     2495 2018-12-07 12:04:12.000000 apis-core-0.9.9/apis_core/apis_metainfo/serializers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)    16898 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_metainfo/models.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      501 2018-10-02 12:27:59.000000 apis-core-0.9.9/apis_core/apis_metainfo/validators.py
+drwxr-xr-x   0 sennierer  (1000) sennierer  (1000)        0 2018-12-18 13:59:55.000000 apis-core-0.9.9/apis_core/apis_vis/
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      894 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_vis/urls.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     6064 2018-12-18 10:22:52.000000 apis-core-0.9.9/apis_core/apis_vis/views.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     1160 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_vis/api_views.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       91 2018-12-10 17:53:56.000000 apis-core-0.9.9/apis_core/apis_vis/apps.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)        0 2018-12-10 17:53:56.000000 apis-core-0.9.9/apis_core/apis_vis/__init__.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)     3646 2018-12-18 10:23:25.000000 apis-core-0.9.9/apis_core/apis_vis/serializers.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)      280 2018-12-10 17:53:56.000000 apis-core-0.9.9/apis_core/apis_vis/utils.py
+-rw-r--r--   0 sennierer  (1000) sennierer  (1000)       38 2018-12-18 13:59:55.000000 apis-core-0.9.9/setup.cfg
```

### Comparing `apis-core-0.9.8/README.rst` & `apis-core-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/PKG-INFO` & `apis-core-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: apis-core
-Version: 0.9.8
+Version: 0.9.9
 Summary: APIS core package. Includes entities, relations, vocabularies,    labels and the helper scripts for RDF parsing.
 Home-page: https://www.apis.acdh.oeaw.ac.at/
 Author: Matthias Schlögl, Peter Andorfer
 Author-email: matthias.schloegl@oeaw.ac.at, peter.andorfer@oeaw.ac.at
 License: MIT License
 Description: Readme
         ======
```

### Comparing `apis-core-0.9.8/setup.py` & `apis-core-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "resolutions": {
         "jquery": "1.9.1 - 3"
       }
 }
 
 setup(
     name='apis-core',
-    version='0.9.8',
+    version='0.9.9',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',  # example license
     description='APIS core package. Includes entities, relations, vocabularies,\
     labels and the helper scripts for RDF parsing.',
     long_description=README,
     url='https://www.apis.acdh.oeaw.ac.at/',
```

### Comparing `apis-core-0.9.8/apis_core.egg-info/PKG-INFO` & `apis-core-0.9.9/apis_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: apis-core
-Version: 0.9.8
+Version: 0.9.9
 Summary: APIS core package. Includes entities, relations, vocabularies,    labels and the helper scripts for RDF parsing.
 Home-page: https://www.apis.acdh.oeaw.ac.at/
 Author: Matthias Schlögl, Peter Andorfer
 Author-email: matthias.schloegl@oeaw.ac.at, peter.andorfer@oeaw.ac.at
 License: MIT License
 Description: Readme
         ======
```

### Comparing `apis-core-0.9.8/apis_core.egg-info/SOURCES.txt` & `apis-core-0.9.9/apis_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 apis_core/apis_entities/templates/apis_entities/compare_base.html
 apis_core/apis_entities/templates/apis_entities/confirm_delete.html
 apis_core/apis_entities/templates/apis_entities/entity_create_generic.html
 apis_core/apis_entities/templates/apis_entities/event_create_generic.html
 apis_core/apis_entities/templates/apis_entities/event_list_generic.html
 apis_core/apis_entities/templates/apis_entities/generic_list.html
 apis_core/apis_entities/templates/apis_entities/generic_network_visualization.html
+apis_core/apis_entities/templates/apis_entities/generic_network_visualization_bak.html
 apis_core/apis_entities/templates/apis_entities/institution_create.html
 apis_core/apis_entities/templates/apis_entities/institution_create_generic.html
 apis_core/apis_entities/templates/apis_entities/institution_list.html
 apis_core/apis_entities/templates/apis_entities/institution_list_generic.html
 apis_core/apis_entities/templates/apis_entities/map_list.html
 apis_core/apis_entities/templates/apis_entities/network.html
 apis_core/apis_entities/templates/apis_entities/network_institution.html
```

### Comparing `apis-core-0.9.8/apis_core/apis_vocabularies/migrations/0001_initial.py` & `apis-core-0.9.9/apis_core/apis_vocabularies/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_vocabularies/api_views.py` & `apis-core-0.9.9/apis_core/apis_vocabularies/api_views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_vocabularies/admin.py` & `apis-core-0.9.9/apis_core/apis_vocabularies/admin.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_vocabularies/serializers.py` & `apis-core-0.9.9/apis_core/apis_vocabularies/serializers.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_vocabularies/models.py` & `apis-core-0.9.9/apis_core/apis_vocabularies/models.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/urls.py` & `apis-core-0.9.9/apis_core/urls.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/templates/apis_templates/_ajax_form.html` & `apis-core-0.9.9/apis_core/templates/apis_templates/_ajax_form.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/templates/apis_templates/registration/registration_closed.html` & `apis-core-0.9.9/apis_core/templates/apis_templates/registration/registration_closed.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/templates/apis_templates/registration/registration_form.html` & `apis-core-0.9.9/apis_core/templates/apis_templates/registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/templates/apis_templates/_ajax_form_generic.html` & `apis-core-0.9.9/apis_core/templates/apis_templates/_ajax_form_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/vocabs_base2.html` & `apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/vocabs_base2.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/templates/apis_templates/autocomplete/stanbol.html` & `apis-core-0.9.9/apis_core/templates/apis_templates/autocomplete/stanbol.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/migrations/0001_initial.py` & `apis-core-0.9.9/apis_core/apis_entities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/tables.py` & `apis-core-0.9.9/apis_core/apis_entities/tables.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/test_parsers.py` & `apis-core-0.9.9/apis_core/apis_entities/test_parsers.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/fields.py` & `apis-core-0.9.9/apis_core/apis_entities/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,23 +10,38 @@
 # "Rewrite" select2 widgets from Django Autocomplete Light so
 # that they don't use Django's admin-provided jQuery, which
 # causes errors with jQuery provided by us.
 class Select2WidgetMixin(DALSelect2WidgetMixin):
     @property
     def media(self):
         m = super().media
-        js = list(m._js) 
+        js = list(m._js)
+        css = list(m._css['screen'])
         try:
             js.remove('admin/js/vendor/jquery/jquery.js')
             js.remove('autocomplete_light/jquery.post-setup.js')
             #js.remove('admin/js/vendor/jquery/jquery.min.js')
         except ValueError:
             print('Error')
             pass
-        return forms.Media(css=m._css, js=js)
+        try:
+            print(js)
+            print(m._css['screen'])
+            js.remove('admin/js/vendor/select2/select2.full.js')
+            js.remove('admin/js/vendor/select2/i18n/en.js')
+            #js.remove('autocomplete_light/select2.js')
+            js.append('https://cdnjs.cloudflare.com/ajax/libs/select2/4.0.5/js/select2.full.min.js')
+            css.remove('admin/css/vendor/select2/select2.css')
+            css.remove('admin/css/autocomplete.css')
+            css.remove('autocomplete_light/select2.css')
+            css.insert(0, 'https://cdnjs.cloudflare.com/ajax/libs/select2/4.0.5/css/select2.min.css')
+        except:
+            print('didnt work')
+        print(js)
+        return forms.Media(css={'screen': css}, js=js)
 
 
 class Select2(Select2WidgetMixin, DALSelect2):
     pass
 
 
 class Select2Multiple(Select2WidgetMixin, DALSelect2Multiple):
```

### Comparing `apis-core-0.9.8/apis_core/apis_entities/forms.py` & `apis-core-0.9.9/apis_core/apis_entities/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from dal import autocomplete
-from .fields import ListSelect2
+from .fields import ListSelect2, Select2Multiple
 from django import forms
 from django.urls import reverse_lazy
 from crispy_forms.helper import FormHelper
 from crispy_forms.layout import Submit
 from crispy_forms.layout import Layout
 from crispy_forms.bootstrap import Accordion, AccordionGroup
 from django.forms import ModelMultipleChoiceField
@@ -67,15 +67,15 @@
                     if ContentType.objects.get(app_label__in=[
                         'apis_entities',
                         'apis_metainfo',
                         'apis_relations',
                         'apis_vocabularies',
                         'apis_labels'
                     ], model=v_name_p.lower()).app_label.lower() == 'apis_vocabularies':
-                        self.fields[f].widget = autocomplete.Select2Multiple(
+                        self.fields[f].widget = Select2Multiple(
                             url=reverse(
                                 'apis:apis_vocabularies:generic_vocabularies_autocomplete',
                                 kwargs={
                                     'vocab': v_name_p.lower(),
                                     'direct': 'normal'
                                     }
                                 ),
```

### Comparing `apis-core-0.9.8/apis_core/apis_entities/test_forms.py` & `apis-core-0.9.9/apis_core/apis_entities/test_forms.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/test_api.py` & `apis-core-0.9.9/apis_core/apis_entities/test_api.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/urls.py` & `apis-core-0.9.9/apis_core/apis_entities/urls.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/views.py` & `apis-core-0.9.9/apis_core/apis_entities/views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/api_views.py` & `apis-core-0.9.9/apis_core/apis_entities/api_views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/institution_list.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/institution_list.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_create.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_create.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/confirm_delete.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_create_generic.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_create_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/work_create_generic.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/work_create_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/apis_templatetag.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/apis_templatetag.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_create_new.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_create_new.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/place_create.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/place_create.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/network_institution.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/network_institution.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/event_create_generic.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/event_create_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/place_list.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/place_list.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/place_create_generic.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/place_create_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/detail_views/person_detail_generic.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/detail_views/person_detail_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/detail_views/entity_detail_generic.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/detail_views/entity_detail_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/institution_create.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/institution_create.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/institution_create_generic.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/institution_create_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/generic_network_visualization.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/generic_network_visualization.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 {% extends "webpage/base.html" %}
 {% load static %}
 {% load crispy_forms_tags %}
 {% block scriptHeader %}
 {{ block.super }}
+
 <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-slider/10.2.1/bootstrap-slider.min.js" integrity="sha256-rjNVc4p9W5ytzudhfdvmen38QnQTPHD6izDAF9nA95w=" crossorigin="anonymous"></script>
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-slider/10.2.1/css/bootstrap-slider.css" integrity="sha256-fyvdwFZ10EzDoLhbbG8gpn2ll8lqkABsEbGWrG18WOU=" crossorigin="anonymous" />
 <script src="{% static 'webpage/libraries/linkurious.js/src/sigma.core.js' %}"></script>
 <script src="{% static 'webpage/libraries/linkurious.js/src/conrad.js' %}"></script>
 <script src="{% static 'webpage/libraries/linkurious.js/src/utils/sigma.utils.js' %}"></script>
 <script src="{% static 'webpage/libraries/linkurious.js/src/utils/sigma.polyfills.js' %}"></script>
 <script src="{% static 'webpage/libraries/linkurious.js/src/sigma.settings.js' %}"></script>
@@ -70,15 +71,15 @@
    	width: 100%;
 	height: 100%;
    }
 div.col-md-9 {
 	height: 100%;
 }
       #graph-container {
-      
+
       min-height: 900px;
       width:100%;
       height:100%;
       margin:auto;
     }
 
     ul.dropdown-menu {
@@ -175,80 +176,83 @@
     #filter_network option, #filter_network label {
     text-transform:capitalize;
 }
 
     </style>
 {% endblock %}
 {% block content %}
-<div class="panel panel-default panel-fixed">
-<div class="panel-heading"><h2>Network Visualization</h2></div>
-<div class="panel-body">
-    <div class="row">
-        <div class="col-md-3">
-            <div id="filter-container">
-                {% crispy form %}
-            </div>
-	    <hr/>
-	    <div id="interaction-form">
-		    <input id="label-threshold" data-slider-id='threhSlider' type="text" data-slider-min="1" data-slider-max="30" data-slider-step="1" data-slider-value="8"/>
-		    <button type="submit" class="btn btn-default" id="toggle-force-link">Start Forcelink</button>
-	    </div>
-            <hr/>
-            <div id="export-form">
-                <form class="form-inline" id="create-file-form">
-                    <div class="form-group">
-                        <label for="select-format">Format</label>
-                        <select class="form-control" id="select-format">
-                            <option>Json</option>
-                            <option>Graphml</option>
-                        </select>
-                    </div>
-                    <div class="form-group">
-                        <div class="checkbox">
-                        <label>
-                        <input type="checkbox" id="choice-download"> Download?
-                        </label>
+<div class="container-fluid">
+    <div class="card">
+        <div class="card-heading">
+            <h2>Network Visualization</h2>
+        </div>
+        <div class="card-body">
+        <div class="row">
+            <div class="col-md-3">
+                <div id="filter-container">
+                    {% crispy form %}
+                </div>
+    	    <hr/>
+    	    <div id="interaction-form">
+    		    <input id="label-threshold" data-slider-id='threhSlider' type="text" data-slider-min="1" data-slider-max="30" data-slider-step="1" data-slider-value="8"/>
+    		    <button type="submit" class="btn btn-default" id="toggle-force-link">Start Forcelink</button>
+    	    </div>
+                <hr/>
+                <div id="export-form">
+                    <form class="form-inline" id="create-file-form">
+                        <div class="form-group">
+                            <label for="select-format">Format</label>
+                            <select class="form-control" id="select-format">
+                                <option>Json</option>
+                                <option>Graphml</option>
+                            </select>
                         </div>
-                    </div>
-                    <div class="form-group">
-                        <button type="submit" class="btn btn-default" id="create-button">Create</button>
-                    </div>
-                </form>
-            </div>
-        <hr/>
-      </div>
-
-        <div class="col-md-9">
-		<div id="graph-container"><div id="filter_network">
-                    <div class="panel panel-default">
-                        <div class="panel-heading" role="tab" id="headingNetworkFilter">
-                          <h4 class="panel-title">
-                            <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseNetworkFilter" aria-expanded="false" aria-controls="collapseNetworkFilter">
-                                Filter
-                            </a>
-                          </h4>
+                        <div class="form-group">
+                            <div class="checkbox">
+                            <label>
+                            <input type="checkbox" id="choice-download"> Download?
+                            </label>
+                            </div>
                         </div>
-                        <div id="collapseNetworkFilter" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingNetworkFilter">
-                          <div class="panel-body">
-                            
-				<form class="form" id="filter2-form">
-					
-				    <div class="form-group">
-					<label for="filter3-label">Name contains</label>
-					<input class="form-control" id="filter3-label">
-				    </div>
-				</form>
-                          </div>
+                        <div class="form-group">
+                            <button type="submit" class="btn btn-default" id="create-button">Create</button>
                         </div>
-                      </div>
-			</div></div>
+                    </form>
+                </div>
+            <hr/>
+          </div>
+
+            <div class="col-md-9">
+    		<div id="graph-container"><div id="filter_network">
+                        <div class="panel panel-default">
+                            <div class="panel-heading" role="tab" id="headingNetworkFilter">
+                              <h4 class="panel-title">
+                                <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseNetworkFilter" aria-expanded="false" aria-controls="collapseNetworkFilter">
+                                    Filter
+                                </a>
+                              </h4>
+                            </div>
+                            <div id="collapseNetworkFilter" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingNetworkFilter">
+                              <div class="panel-body">
+
+    				<form class="form" id="filter2-form">
+
+    				    <div class="form-group">
+    					<label for="filter3-label">Name contains</label>
+    					<input class="form-control" id="filter3-label">
+    				    </div>
+    				</form>
+                              </div>
+                            </div>
+                          </div>
+    			</div></div>
+            </div>
         </div>
     </div>
-</div>
-</div>
+</div></div>
 {% endblock %}
 
 {% block scripts %}
 {{block.super}}
 <script type="text/javascript">
 	$("#interaction-form").on( "click", "#toggle-force-link", function(e) {
 		e.preventDefault();
@@ -266,15 +270,15 @@
 	console.log("click worked");
 	var filters = new Object();
 	for (var f in $.ApisNet.filter.list_node_filters) {
 		filters[f] = $('#filter2-'+f).val()
 	}
 	console.log(filters);
         $.ApisNet.instance.graph.nodes().forEach(function (n) {
-		var test = false;	
+		var test = false;
 		var label_contains = $('#filter3-label').val()
 		if (label_contains != null) {
 			if (n.label.includes(label_contains)) {
 			test = true;
 			} else {
 			test = false;
 			return;
@@ -293,29 +297,29 @@
 					if (filters[f2].includes(d[f2][i])){
 					test2 = true
 					}
 				}
 				} else {
 					if (filters[f2].includes(d[f2])){
 					test2 = true
-					}	
+					}
 				}
 				if (test2){
 				test = true
 				} else {
 				test = false;
 				break;
 				}
 			}
 		}
 		if (test) {
 		n.color = '#f4e242';
 		$.ApisNet.selected_nodes.push(n);
 		}
-	
+
 	}
 )
 
      $.ApisNet.instance.refresh();
 })
 function download_network_data(formData) {
     $.ajax({
@@ -360,15 +364,15 @@
 			      $.ApisNet.filter.list_node_filters[key].values.push(n.data[key]);
 				      $.ApisNet.filter.list_node_filters[key].select2.push({id: n.data[key], text: n.data[key]})}}
 			      } else if (key == 'type') {
 			      if (!$.ApisNet.filter.list_node_filters[key].values.includes(n[key])) {
 			      $.ApisNet.filter.list_node_filters[key].values.push(n[key]);
 				      $.ApisNet.filter.list_node_filters[key].select2.push({id: n[key], text: n[key]})
 			      };
-			      
+
 			      }
 
 			      };
 
   });
        if (typeof $.ApisNet.form_data_load !== 'undefined'){
            if ($.ApisNet.form_data_load.length > 0) {
@@ -376,15 +380,15 @@
                download_network_data(form);
            }
        }
 
      $.ApisNet.instance.refresh();
      sigma.layouts.startForceLink($.ApisNet.instance);
 		  for (var key in $.ApisNet.filter.list_node_filters) {
-		  
+
 		$("#filter2-"+key).select2({
 		data: $.ApisNet.filter.list_node_filters[key].select2
 		})
 		  }
           }
 
     })
@@ -674,8 +678,7 @@
         });
     //$('#id_search_target-autocomplete').yourlabsAutocomplete('destroy');
     //$('#id_search_target-autocomplete').yourlabsAutocomplete({'url': new_val_target, 'minimumCharacters': 2});
 })
 })
 </script>
 {% endblock %}
-
```

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/generic_list.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/generic_list.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/entity_create_generic.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/entity_create_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/person_list.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/person_list.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/map_list.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/map_list.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/templates/apis_entities/network.html` & `apis-core-0.9.9/apis_core/apis_entities/templates/apis_entities/network.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/serializers_generic.py` & `apis-core-0.9.9/apis_core/apis_entities/serializers_generic.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/test_models.py` & `apis-core-0.9.9/apis_core/apis_entities/test_models.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/api_renderers.py` & `apis-core-0.9.9/apis_core/apis_entities/api_renderers.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/autocomplete_light_registry.py` & `apis-core-0.9.9/apis_core/apis_entities/autocomplete_light_registry.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/filters.py` & `apis-core-0.9.9/apis_core/apis_entities/filters.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/views2.py` & `apis-core-0.9.9/apis_core/apis_entities/views2.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/serializers.py` & `apis-core-0.9.9/apis_core/apis_entities/serializers.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/models.py` & `apis-core-0.9.9/apis_core/apis_entities/models.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/autocomplete3.py` & `apis-core-0.9.9/apis_core/apis_entities/autocomplete3.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/custom_authentication.py` & `apis-core-0.9.9/apis_core/apis_entities/custom_authentication.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/api_urls.py` & `apis-core-0.9.9/apis_core/apis_entities/api_urls.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_entities/detail_views.py` & `apis-core-0.9.9/apis_core/apis_entities/detail_views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/helper_functions/stanbolQueries.py` & `apis-core-0.9.9/apis_core/helper_functions/stanbolQueries.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/helper_functions/dl_models.py` & `apis-core-0.9.9/apis_core/helper_functions/dl_models.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/helper_functions/highlighter.py` & `apis-core-0.9.9/apis_core/helper_functions/highlighter.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/helper_functions/inter_annotator_agreement.py` & `apis-core-0.9.9/apis_core/helper_functions/inter_annotator_agreement.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/helper_functions/RDFparsers.py` & `apis-core-0.9.9/apis_core/helper_functions/RDFparsers.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/helper_functions/utils.py` & `apis-core-0.9.9/apis_core/helper_functions/utils.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_tei/partials.py` & `apis-core-0.9.9/apis_core/apis_tei/partials.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_tei/tei.py` & `apis-core-0.9.9/apis_core/apis_tei/tei.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_tei/tei_ac.py` & `apis-core-0.9.9/apis_core/apis_tei/tei_ac.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/default_settings/NER_settings.py` & `apis-core-0.9.9/apis_core/default_settings/NER_settings.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/default_settings/RDF_settings.py` & `apis-core-0.9.9/apis_core/default_settings/RDF_settings.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/context_processors/custom_context_processors.py` & `apis-core-0.9.9/apis_core/context_processors/custom_context_processors.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_labels/migrations/0001_initial.py` & `apis-core-0.9.9/apis_core/apis_labels/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_labels/migrations/0002_auto_20181003_1310.py` & `apis-core-0.9.9/apis_core/apis_labels/migrations/0002_auto_20181003_1310.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_labels/forms.py` & `apis-core-0.9.9/apis_core/apis_labels/forms.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_labels/views.py` & `apis-core-0.9.9/apis_core/apis_labels/views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_labels/templates/apis_labels/label_create.html` & `apis-core-0.9.9/apis_core/apis_labels/templates/apis_labels/label_create.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_labels/templates/apis_labels/labels_list.html` & `apis-core-0.9.9/apis_core/apis_labels/templates/apis_labels/labels_list.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_labels/autocomplete_light_registry.py` & `apis-core-0.9.9/apis_core/apis_labels/autocomplete_light_registry.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_labels/models.py` & `apis-core-0.9.9/apis_core/apis_labels/models.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/migrations/0001_initial.py` & `apis-core-0.9.9/apis_core/apis_relations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/migrations/0002_auto_20181121_1543.py` & `apis-core-0.9.9/apis_core/apis_relations/migrations/0002_auto_20181121_1543.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/tables.py` & `apis-core-0.9.9/apis_core/apis_relations/tables.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/forms.py` & `apis-core-0.9.9/apis_core/apis_relations/forms.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/urls.py` & `apis-core-0.9.9/apis_core/apis_relations/urls.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/views.py` & `apis-core-0.9.9/apis_core/apis_relations/views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/api_views.py` & `apis-core-0.9.9/apis_core/apis_relations/api_views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/_ajax_form.html` & `apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/_ajax_form.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/_ajax_form_generic.html` & `apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/_ajax_form_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/templates/apis_relations/relations_detail_generic.html` & `apis-core-0.9.9/apis_core/apis_relations/templates/apis_relations/relations_detail_generic.html`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/autocomplete_light_registry.py` & `apis-core-0.9.9/apis_core/apis_relations/autocomplete_light_registry.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/rel_views.py` & `apis-core-0.9.9/apis_core/apis_relations/rel_views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/rel_forms.py` & `apis-core-0.9.9/apis_core/apis_relations/rel_forms.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/serializers.py` & `apis-core-0.9.9/apis_core/apis_relations/serializers.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/models.py` & `apis-core-0.9.9/apis_core/apis_relations/models.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/forms2.py` & `apis-core-0.9.9/apis_core/apis_relations/forms2.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_relations/forms_backup.py` & `apis-core-0.9.9/apis_core/apis_relations/forms_backup.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_metainfo/migrations/0001_initial.py` & `apis-core-0.9.9/apis_core/apis_metainfo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_metainfo/migrations/0002_auto_20181003_1310.py` & `apis-core-0.9.9/apis_core/apis_metainfo/migrations/0002_auto_20181003_1310.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_metainfo/api_views.py` & `apis-core-0.9.9/apis_core/apis_metainfo/api_views.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_metainfo/templates/apis_metainfo/TEI_renderer.xml` & `apis-core-0.9.9/apis_core/apis_metainfo/templates/apis_metainfo/TEI_renderer.xml`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_metainfo/test_models.py` & `apis-core-0.9.9/apis_core/apis_metainfo/test_models.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_metainfo/api_renderers.py` & `apis-core-0.9.9/apis_core/apis_metainfo/api_renderers.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_metainfo/serializers.py` & `apis-core-0.9.9/apis_core/apis_metainfo/serializers.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_metainfo/models.py` & `apis-core-0.9.9/apis_core/apis_metainfo/models.py`

 * *Files identical despite different names*

### Comparing `apis-core-0.9.8/apis_core/apis_vis/views.py` & `apis-core-0.9.9/apis_core/apis_vis/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,51 @@
 import pandas as pd
 from collections import Counter
 from django.http import JsonResponse
 from django.views.generic import TemplateView
 from django.conf import settings
 from django.db.models import Avg
 
-from apis_core.apis_relations.models import PersonPlace, PersonInstitution
+from apis_core.apis_relations.models import *
 
 from . utils import calculate_age
 
 
+def get_inst_range_data(request):
+    df = pd.DataFrame(list(InstitutionInstitution.objects.filter(
+        relation_type__name="ist Teil von").distinct().values_list(
+        'related_institutionA__name',
+        'related_institutionA__start_date__year',
+        'related_institutionA__end_date__year',
+        'related_institutionB__name'
+        )
+    ), columns=['name', 'start_year', 'end_year', 'teil von']).fillna(2018)
+    df.sort_values('start_year')
+
+    data = {
+        "items": "some",
+        "title": "{}".format('Kommissionen'),
+        "subtitle": "Person Institution relation type {}".format('some type'),
+        "legendy": "legendy",
+        "legendx": "legendx",
+        "categories": "sorted(dates)",
+        "measuredObject": "{}".format("Persons average Age"),
+        "ymin": 0,
+        "x_axis": df['name'].values.tolist(),
+        "payload": [
+            {
+                'name': 'Kommissionen',
+                'data': df[['start_year', 'end_year']].values.tolist()
+            }
+        ]
+    }
+
+    return JsonResponse(data, safe=False)
+
+
 def get_average_members_data(request):
     rel_type = request.GET.get('rel-type')
     rel_inst = request.GET.get('rel-inst')
     start_year = request.GET.get('start-year')
     end_year = request.GET.get('start-year')
     per_inst = PersonInstitution.objects.filter(related_institution_id__in=[3, 2])
     if rel_type:
@@ -132,7 +164,11 @@
 
 class AvgAge(TemplateView):
     template_name = "apis_vis/avgage.html"
 
 
 class MembersAmountPerYear(TemplateView):
     template_name = "apis_vis/avgmemperyear.html"
+
+
+class InstRange(TemplateView):
+    template_name = "apis_vis/inst_range.html"
```

### Comparing `apis-core-0.9.8/apis_core/apis_vis/api_views.py` & `apis-core-0.9.9/apis_core/apis_vis/api_views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from django.contrib.contenttypes.models import ContentType
 from rest_framework.generics import ListAPIView
-from .serializers import VisAgeSerializer
+from .serializers import *
 from apis_core.apis_relations.models import PersonInstitution
 from django_filters.rest_framework import DjangoFilterBackend
-from rest_framework import  filters
+from rest_framework import filters
 
 
 class GetVisJson(ListAPIView):
 
     filter_backends = (DjangoFilterBackend, filters.SearchFilter)
     depth = 2
-    filter_fields = ('related_institution__name', 'related_person__name', 'relation_type__name', 'related_person__collection__name', 'related_institution_id')
-    search_fields = ('related_institution__name', 'related_person__name' )
+    # TODO: add a generic filter thing
+
     def get_serializer(self, instance=None, data=None, many=False, partial=False):
         vis = self.request.query_params.get('vis', None)
-        if vis == 'average_age':
+        if vis == 'av-age':
             return VisAgeSerializer(self.get_queryset(), many=False)
+        elif vis == 'avg-relations':
+            return AvRelations(self.get_queryset(), many=False)
         else:
             return None
 
-    def get_queryset(self):
-        queryset = PersonInstitution.objects.all()
-        start_date = self.request.query_params.get('end_date', None)
-        end_date = self.request.query_params.get('start_date', None)
-        if start_date is not None:
-            queryset = queryset.filter(start_date__lt=start_date)
-        if end_date is not None:
-            queryset = queryset.filter(end_date__gt=end_date)
+    def get_queryset(self, **kwargs):
+        relation = self.kwargs['relation'].lower()
+        relation_model = ContentType.objects.get(
+            app_label='apis_relations', model=relation).model_class()
+        print("from get_queryset {}".format(relation))
+        queryset = relation_model.objects.all()
         return queryset
```

