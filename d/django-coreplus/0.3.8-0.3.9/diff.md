# Comparing `tmp/django-coreplus-0.3.8.tar.gz` & `tmp/django-coreplus-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-coreplus-0.3.8.tar", last modified: Thu May 11 11:25:31 2023, max compression
+gzip compressed data, was "django-coreplus-0.3.9.tar", last modified: Wed May 17 06:31:59 2023, max compression
```

## Comparing `django-coreplus-0.3.8.tar` & `django-coreplus-0.3.9.tar`

### file list

```diff
@@ -1,492 +1,494 @@
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4229 2023-05-11 11:25:11.000000 django-coreplus-0.3.8/CHANGELOG.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/LICENSE
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      141 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/MANIFEST.in
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3670 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/PKG-INFO
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2429 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/README.md
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      110 2023-05-11 11:24:37.000000 django-coreplus-0.3.8/coreplus/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       77 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      440 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    10774 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/base.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      890 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/filters.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1402 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2602 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2379 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/mixins.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    10056 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/sites.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/static/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/static/coreplus_admin/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/static/coreplus_admin/js/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    37296 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/static/coreplus_admin/js/alpine.min.js
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    34881 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/static/coreplus_admin/js/htmx.min.js
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    89501 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/static/coreplus_admin/js/jquery.min.js
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2881 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/base.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/confirmation.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3051 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/form_view.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      942 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/inspect.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1590 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/inspect_object_tools.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      130 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/object_buttons.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      338 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/print.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/print_cover.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/print_footer.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/admin/templates/admin/print_header.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/ads/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/ads/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/ads/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/ads/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/ads/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/ads/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/ads/api/v1/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       55 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/ads/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/ads/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1882 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      182 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/consts.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/api/endpoints/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/endpoints/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      237 2022-12-28 08:58:55.000000 django-coreplus-0.3.8/coreplus/api/endpoints/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      585 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/endpoints/v1.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      599 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/endpoints/v2.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2377 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/helpers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/api/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/api/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/api/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      562 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      910 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      275 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/schemas.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/api/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/api/templates/drf_spectacular/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1069 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/templates/drf_spectacular/redoc.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      231 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      418 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/api/views.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6886 2022-12-28 08:58:55.000000 django-coreplus-0.3.8/coreplus/configs.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    13235 2023-03-07 09:24:58.000000 django-coreplus-0.3.8/coreplus/contacts/abstracts.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      298 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      193 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      452 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      496 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/gis.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2934 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/inlines.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3484 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6069 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/management/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/management/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/management/commands/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/management/commands/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2280 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/management/commands/populate_countries.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/contacts/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    24385 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6351 2022-12-13 04:40:56.000000 django-coreplus-0.3.8/coreplus/contacts/migrations/0002_alter_billingaddress_address_and_more.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1106 2023-03-07 09:24:58.000000 django-coreplus-0.3.8/coreplus/contacts/migrations/0003_billingaddress_district_deliverableaddress_district_and_more.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3644 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/contacts/models.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/discuss/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      245 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      243 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/discuss/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/discuss/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1288 2022-12-28 08:58:55.000000 django-coreplus-0.3.8/coreplus/discuss/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      194 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4367 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      448 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/discuss/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/discuss/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/discuss/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1034 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1623 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/discuss/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4163 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      591 2023-01-30 02:56:44.000000 django-coreplus-0.3.8/coreplus/discuss/migrations/0002_alter_discuss_flag.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3597 2023-03-14 07:44:17.000000 django-coreplus-0.3.8/coreplus/discuss/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/discuss/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/docs/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       57 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      269 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/docs/management/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/management/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/docs/management/commands/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/management/commands/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      467 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/management/commands/build_docs.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/docs/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/docs/templates/docs/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      468 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/templates/docs/_base_one.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      581 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/templates/docs/_base_two.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      505 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/templates/docs/index.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/docs/tests/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/tests/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2022 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/tests/runtests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/docs/tests/test_docs/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        2 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/tests/test_docs/index.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/docs/tests/test_docs/sub_dir/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        2 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/tests/test_docs/sub_dir/index.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3898 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/tests/test_views.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      345 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/tests/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      419 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3537 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/docs/views.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/heralds/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       78 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      521 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/heralds/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/heralds/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2150 2023-03-07 09:24:58.000000 django-coreplus-0.3.8/coreplus/heralds/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      214 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     8624 2023-03-07 09:24:58.000000 django-coreplus-0.3.8/coreplus/heralds/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      444 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/heralds/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/heralds/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/heralds/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1142 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1851 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      323 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/managers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/heralds/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5041 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      441 2023-03-07 09:24:58.000000 django-coreplus-0.3.8/coreplus/heralds/migrations/0002_alter_directmessage_content.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/heralds/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2406 2023-03-07 09:24:58.000000 django-coreplus-0.3.8/coreplus/heralds/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1216 2022-12-13 05:03:37.000000 django-coreplus-0.3.8/coreplus/heralds/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/hooks/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      753 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       28 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1069 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/admin.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      438 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2249 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/core.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/hooks/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/hooks/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/hooks/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      395 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      658 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/hooks/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/hooks/templates/admin/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/hooks/templates/admin/coreplus_hooks/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      677 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/templates/admin/coreplus_hooks/hooks_registry.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      240 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/hooks/urls.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      683 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/markdown/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      106 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3313 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      280 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1529 2023-04-13 03:30:17.000000 django-coreplus-0.3.8/coreplus/markdown/bleaching.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/markdown/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/markdown/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/markdown/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      562 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      910 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/markdown/plugins/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/plugins/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      951 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/plugins/gist.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      614 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/plugins/linkify.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1837 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/plugins/twitter.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1430 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/plugins/youtube.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      112 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/renderer.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      953 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/markdown/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/media/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       68 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/media/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/media/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3960 2023-01-09 06:47:42.000000 django-coreplus-0.3.8/coreplus/media/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      333 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4386 2023-01-09 06:47:42.000000 django-coreplus-0.3.8/coreplus/media/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      439 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      766 2023-01-09 06:47:42.000000 django-coreplus-0.3.8/coreplus/media/helpers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/media/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/media/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/media/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2051 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2976 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/media/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5350 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4011 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      434 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/media/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/navigators/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2099 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      361 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/admin.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      606 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/navigators/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/navigators/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/navigators/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1377 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2174 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/navigators/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4224 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5698 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/models.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/navigators/templatetags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/templatetags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      567 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/templatetags/navigators_tags.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/navigators/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/notices/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       61 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1030 2023-01-26 04:08:06.000000 django-coreplus-0.3.8/coreplus/notices/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/notices/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/notices/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1217 2023-01-24 06:23:58.000000 django-coreplus-0.3.8/coreplus/notices/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      622 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2037 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      276 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/notices/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/notices/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/notices/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1290 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2077 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/notices/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3941 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2805 2023-01-26 04:08:06.000000 django-coreplus-0.3.8/coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     9231 2023-05-11 11:16:28.000000 django-coreplus-0.3.8/coreplus/notices/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      211 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/signals.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      325 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/tasks.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/notices/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/notices/templates/notices/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       79 2023-01-26 04:08:06.000000 django-coreplus-0.3.8/coreplus/notices/templates/notices/email_broadcast.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      392 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/notices/urls.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/numerators/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       87 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      290 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/numerators/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/api/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/api/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/api/views.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/api/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      452 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/numerators/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/numerators/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/numerators/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      746 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1346 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/numerators/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2052 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5998 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/numerators/models.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/profanity/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       81 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      166 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3380 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/extras.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/profanity/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/migrations/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/profanity/templatetags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/templatetags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      264 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/templatetags/profanity.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      402 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      257 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/validators.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3583 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/profanity/wordlist.txt
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/qrcodes/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       79 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/qrcodes/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/qrcodes/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       41 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/qrcodes/admin.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      155 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/qrcodes/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4184 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/qrcodes/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/qrcodes/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/reactions/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      115 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      628 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/reactions/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/reactions/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1332 2023-03-07 09:24:58.000000 django-coreplus-0.3.8/coreplus/reactions/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      517 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/reactions/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/reactions/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/reactions/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3073 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/reactions/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     8838 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    15907 2023-03-17 05:46:47.000000 django-coreplus-0.3.8/coreplus/reactions/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/reactions/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/search/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       73 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/search/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/search/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      444 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/search/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/search/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/search/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      637 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1005 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/search/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/search/templates/search/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       94 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/templates/search/algolia_search.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1724 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/templates/search/search.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      413 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/templates/search/search_form.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/search/templatetags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/templatetags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      674 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/templatetags/search_tags.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      131 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2350 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/search/views.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       94 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1273 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/api/v1/views.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      477 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2395 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/contexts.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/settings/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/settings/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      918 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1985 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1716 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3441 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1283 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/permissions.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2254 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/registries.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/settings/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/templates/admin/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      173 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/templates/admin/base.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/templates/admin/settings/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/templates/admin/settings/.gitinclude
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2461 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/templates/admin/settings/edit.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/templates/simpel_settings/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/templates/simpel_settings/.gitinclude
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/settings/templatetags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/templatetags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1629 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/templatetags/settings_tags.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       68 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      438 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3650 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/settings/views.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/shorts/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       63 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       63 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/shorts/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/shorts/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      412 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      197 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1491 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      505 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/shorts/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/coreplus/shorts/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/shorts/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      399 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      663 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      136 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/managers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/shorts/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2354 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1362 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      125 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      692 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/utils.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      625 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/shorts/views.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/spams/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       83 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      150 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1018 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/extras.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      101 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/spams.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/spams/static/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)   311221 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/static/model_and_vectorizer_with_pickle(en).pkl
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)   253954 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/static/model_and_vectorizer_with_pickle(id).pkl
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      951 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      223 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/spams/validators.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/tags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       72 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      706 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/tags/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       34 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/api/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      420 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/api/extensions.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/tags/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      524 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      300 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      907 2023-04-13 04:22:09.000000 django-coreplus-0.3.8/coreplus/tags/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      146 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      131 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/managers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/tags/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4657 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      450 2023-03-28 02:54:06.000000 django-coreplus-0.3.8/coreplus/tags/migrations/0002_category_category_id.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      480 2023-04-13 09:52:56.000000 django-coreplus-0.3.8/coreplus/tags/migrations/0003_alter_category_category_id.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3576 2023-04-13 09:52:26.000000 django-coreplus-0.3.8/coreplus/tags/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      826 2023-04-13 03:50:58.000000 django-coreplus-0.3.8/coreplus/tags/resources.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/tags/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      117 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/urls.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/utils/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      997 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/avatars.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      823 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/contenttypes.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3995 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/currencies.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3901 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/decorators.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/utils/forms/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/forms/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      996 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/forms/fields.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3122 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/loading.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/coreplus/utils/models/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    11822 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/actions.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5723 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/choices.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    17271 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/fields.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    14099 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/managers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     7742 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2308 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/paranoid.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1117 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/signals.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    14851 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/models/tracker.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2593 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/slugs.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4505 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/utils/validators.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1471 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/coreplus/version.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/django_coreplus.egg-info/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3670 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/django_coreplus.egg-info/PKG-INFO
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    12071 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/django_coreplus.egg-info/SOURCES.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        1 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/django_coreplus.egg-info/dependency_links.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        1 2022-12-13 05:23:51.000000 django-coreplus-0.3.8/django_coreplus.egg-info/not-zip-safe
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      433 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/django_coreplus.egg-info/requires.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        9 2023-05-11 11:25:30.000000 django-coreplus-0.3.8/django_coreplus.egg-info/top_level.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2123 2023-05-11 11:25:31.000000 django-coreplus-0.3.8/setup.cfg
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       61 2022-12-05 03:07:46.000000 django-coreplus-0.3.8/setup.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.517824 django-coreplus-0.3.9/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4229 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/CHANGELOG.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/LICENSE
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      141 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/MANIFEST.in
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3670 2023-05-17 06:31:59.517824 django-coreplus-0.3.9/PKG-INFO
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2429 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/README.md
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.447824 django-coreplus-0.3.9/coreplus/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      110 2023-05-17 06:29:23.000000 django-coreplus-0.3.9/coreplus/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.447824 django-coreplus-0.3.9/coreplus/admin/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       77 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      440 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    10774 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/base.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      890 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/filters.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/admin/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/admin/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.447824 django-coreplus-0.3.9/coreplus/admin/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1402 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2602 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2379 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/mixins.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    10056 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/sites.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/admin/static/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/admin/static/coreplus_admin/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.447824 django-coreplus-0.3.9/coreplus/admin/static/coreplus_admin/js/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    37296 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/static/coreplus_admin/js/alpine.min.js
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    34881 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/static/coreplus_admin/js/htmx.min.js
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    89501 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/static/coreplus_admin/js/jquery.min.js
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/admin/templates/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.447824 django-coreplus-0.3.9/coreplus/admin/templates/admin/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2881 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/base.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/confirmation.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3051 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/form_view.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      942 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/inspect.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1590 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/inspect_object_tools.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      130 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/object_buttons.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      338 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/print.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/print_cover.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/print_footer.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/admin/templates/admin/print_header.html
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.447824 django-coreplus-0.3.9/coreplus/ads/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/ads/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.447824 django-coreplus-0.3.9/coreplus/ads/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/ads/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.447824 django-coreplus-0.3.9/coreplus/ads/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/ads/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/ads/api/v1/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       55 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/ads/api/v1/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/ads/tests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1882 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      182 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/consts.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/api/endpoints/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/endpoints/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      237 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/api/endpoints/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      585 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/endpoints/v1.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      599 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/endpoints/v2.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2377 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/helpers.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/api/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/api/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/api/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      562 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      910 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      275 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/schemas.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/api/templates/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/api/templates/drf_spectacular/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1069 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/templates/drf_spectacular/redoc.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      231 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      418 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/api/views.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     6886 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/configs.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/contacts/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    13235 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/contacts/abstracts.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      298 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/contacts/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/contacts/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      193 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      452 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      496 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/gis.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2934 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/inlines.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/contacts/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/contacts/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/contacts/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3484 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     6069 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/contacts/management/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/management/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/contacts/management/commands/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/management/commands/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2280 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/management/commands/populate_countries.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/contacts/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    24385 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     6351 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/contacts/migrations/0002_alter_billingaddress_address_and_more.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1106 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/contacts/migrations/0003_billingaddress_district_deliverableaddress_district_and_more.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3644 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/contacts/models.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/discuss/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      245 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      243 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/discuss/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/discuss/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1288 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/discuss/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      194 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/api/v1/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4367 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/api/v1/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      448 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/discuss/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/discuss/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/discuss/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1034 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1623 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/discuss/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4163 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      591 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/discuss/migrations/0002_alter_discuss_flag.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3597 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/discuss/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/discuss/tests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/docs/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       57 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      269 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.457824 django-coreplus-0.3.9/coreplus/docs/management/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/management/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/docs/management/commands/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/management/commands/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      467 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/management/commands/build_docs.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.417824 django-coreplus-0.3.9/coreplus/docs/templates/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/docs/templates/docs/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      468 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/templates/docs/_base_one.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      581 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/templates/docs/_base_two.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      505 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/templates/docs/index.html
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/docs/tests/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/tests/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2022 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/tests/runtests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/docs/tests/test_docs/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        2 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/tests/test_docs/index.html
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/docs/tests/test_docs/sub_dir/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        2 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/tests/test_docs/sub_dir/index.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3898 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/tests/test_views.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      345 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/tests/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      419 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3537 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/docs/views.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/heralds/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       78 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      521 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/heralds/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/heralds/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2150 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/heralds/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      214 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/api/v1/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     8624 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/heralds/api/v1/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      444 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/heralds/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/heralds/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/heralds/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1142 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1851 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      323 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/managers.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/heralds/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     5041 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      441 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/heralds/migrations/0002_alter_directmessage_content.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2406 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/heralds/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1216 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/heralds/tests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/hooks/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      753 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       28 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1069 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/admin.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      438 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2249 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/core.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/hooks/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/hooks/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/hooks/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      395 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      658 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/hooks/templates/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/hooks/templates/admin/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/hooks/templates/admin/coreplus_hooks/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      677 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/templates/admin/coreplus_hooks/hooks_registry.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      240 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/hooks/urls.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.467824 django-coreplus-0.3.9/coreplus/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      683 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/markdown/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      106 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3313 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      280 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1529 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/markdown/bleaching.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/markdown/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/markdown/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/markdown/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      562 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      910 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/markdown/plugins/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/plugins/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      951 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/plugins/gist.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      614 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/plugins/linkify.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1837 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/plugins/twitter.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1430 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/plugins/youtube.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      112 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/renderer.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      953 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/markdown/tests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/media/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       68 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/media/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/media/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3960 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/media/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      333 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/api/v1/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4386 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/media/api/v1/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      439 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      766 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/media/helpers.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/media/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/media/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/media/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2051 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2976 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/media/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     5350 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4011 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      434 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/media/tests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/navigators/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2099 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      361 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/admin.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      606 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/navigators/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/navigators/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/navigators/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1377 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2174 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/navigators/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4224 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     5698 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/models.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/navigators/templatetags/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/templatetags/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      567 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/templatetags/navigators_tags.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/navigators/tests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/notices/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       61 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1376 2023-05-17 06:07:33.000000 django-coreplus-0.3.9/coreplus/notices/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/notices/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.477824 django-coreplus-0.3.9/coreplus/notices/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1861 2023-05-17 06:16:19.000000 django-coreplus-0.3.9/coreplus/notices/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      719 2023-05-17 06:19:48.000000 django-coreplus-0.3.9/coreplus/notices/api/v1/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2339 2023-05-17 06:16:55.000000 django-coreplus-0.3.9/coreplus/notices/api/v1/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      276 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/notices/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.427824 django-coreplus-0.3.9/coreplus/notices/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/notices/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1290 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2077 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/notices/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3941 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2805 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3403 2023-05-17 04:54:52.000000 django-coreplus-0.3.9/coreplus/notices/migrations/0003_firebasedevice.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      368 2023-05-17 06:27:18.000000 django-coreplus-0.3.9/coreplus/notices/migrations/0004_alter_firebasedevice_options.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    10486 2023-05-17 06:21:32.000000 django-coreplus-0.3.9/coreplus/notices/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      211 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/signals.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      325 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/tasks.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/notices/templates/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/notices/templates/notices/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       79 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/notices/templates/notices/email_broadcast.txt
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      392 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/notices/urls.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/numerators/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       87 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      290 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/numerators/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/api/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/api/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/api/views.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/api/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      452 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/numerators/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/numerators/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/numerators/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      746 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1346 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/numerators/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2052 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     5998 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/numerators/models.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/profanity/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       81 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      166 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3380 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/extras.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/profanity/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/migrations/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/profanity/templatetags/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/templatetags/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      264 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/templatetags/profanity.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      402 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      257 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/validators.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3583 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/profanity/wordlist.txt
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/qrcodes/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       79 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/qrcodes/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/qrcodes/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       41 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/qrcodes/admin.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      155 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/qrcodes/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4184 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/qrcodes/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/qrcodes/tests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/reactions/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      115 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      628 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/reactions/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/reactions/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1332 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/reactions/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      517 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/reactions/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/reactions/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.487824 django-coreplus-0.3.9/coreplus/reactions/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3073 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/reactions/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     8838 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    15907 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/reactions/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/reactions/tests.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/search/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       73 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/search/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/search/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/api/v1/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      444 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/search/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/search/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/search/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      637 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1005 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/search/templates/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/search/templates/search/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       94 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/templates/search/algolia_search.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1724 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/templates/search/search.html
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      413 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/templates/search/search_form.html
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/search/templatetags/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/templatetags/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      674 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/templatetags/search_tags.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      131 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2350 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/search/views.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       94 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1273 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/api/v1/views.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/api/v1/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      477 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2395 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/contexts.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/settings/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/settings/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      918 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1985 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1716 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3441 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1283 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/permissions.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2254 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/registries.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/settings/templates/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/templates/admin/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      173 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/templates/admin/base.html
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/templates/admin/settings/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/templates/admin/settings/.gitinclude
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2461 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/templates/admin/settings/edit.html
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/templates/simpel_settings/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/templates/simpel_settings/.gitinclude
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.497824 django-coreplus-0.3.9/coreplus/settings/templatetags/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/templatetags/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1629 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/templatetags/settings_tags.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       68 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      438 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3650 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/settings/views.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/shorts/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       63 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       63 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/shorts/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/api/__init__.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/shorts/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      412 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      197 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/api/v1/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1491 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/api/v1/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      505 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/apps.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/shorts/locale/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.437824 django-coreplus-0.3.9/coreplus/shorts/locale/id/
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/shorts/locale/id/LC_MESSAGES/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      399 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      663 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      136 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/managers.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/shorts/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2354 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1362 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      125 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      692 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/utils.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      625 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/shorts/views.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/spams/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       83 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      150 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1018 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/extras.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      101 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/spams.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/spams/static/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)   311221 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/static/model_and_vectorizer_with_pickle(en).pkl
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)   253954 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/static/model_and_vectorizer_with_pickle(id).pkl
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      951 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      223 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/spams/validators.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/tags/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       72 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/README.md
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      706 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/admin.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/tags/api/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       34 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/api/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      420 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/api/extensions.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/tags/api/v1/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/api/v1/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      524 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/api/v1/serializers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      300 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/api/v1/urls.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      907 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/tags/api/v1/viewsets.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      146 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/apps.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      131 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/managers.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/tags/migrations/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4657 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/migrations/0001_initial.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      450 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/tags/migrations/0002_category_category_id.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      480 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/tags/migrations/0003_alter_category_category_id.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/migrations/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3576 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/tags/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      826 2023-05-17 03:50:45.000000 django-coreplus-0.3.9/coreplus/tags/resources.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/tags/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      117 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/urls.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.507824 django-coreplus-0.3.9/coreplus/utils/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      997 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/avatars.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      823 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/contenttypes.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3995 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/currencies.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3901 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/decorators.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.517824 django-coreplus-0.3.9/coreplus/utils/forms/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/forms/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      996 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/forms/fields.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3122 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/loading.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.517824 django-coreplus-0.3.9/coreplus/utils/models/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/__init__.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    11822 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/actions.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     5723 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/choices.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    17271 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/fields.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    14099 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/managers.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     7742 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/models.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2308 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/paranoid.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1117 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/signals.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    14851 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/models/tracker.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2593 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/slugs.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/tests.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     4505 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/utils/validators.py
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     1471 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/coreplus/version.py
+drwxr-xr-x   0 rizkisasri  (1000) rizkisasri  (1000)        0 2023-05-17 06:31:59.517824 django-coreplus-0.3.9/django_coreplus.egg-info/
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     3670 2023-05-17 06:31:59.000000 django-coreplus-0.3.9/django_coreplus.egg-info/PKG-INFO
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)    12187 2023-05-17 06:31:59.000000 django-coreplus-0.3.9/django_coreplus.egg-info/SOURCES.txt
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        1 2023-05-17 06:31:59.000000 django-coreplus-0.3.9/django_coreplus.egg-info/dependency_links.txt
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        1 2023-05-17 06:30:11.000000 django-coreplus-0.3.9/django_coreplus.egg-info/not-zip-safe
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)      433 2023-05-17 06:31:59.000000 django-coreplus-0.3.9/django_coreplus.egg-info/requires.txt
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)        9 2023-05-17 06:31:59.000000 django-coreplus-0.3.9/django_coreplus.egg-info/top_level.txt
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)     2123 2023-05-17 06:31:59.517824 django-coreplus-0.3.9/setup.cfg
+-rw-r--r--   0 rizkisasri  (1000) rizkisasri  (1000)       61 2023-05-17 03:46:21.000000 django-coreplus-0.3.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-coreplus-0.3.8/CHANGELOG.md` & `django-coreplus-0.3.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/PKG-INFO` & `django-coreplus-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-coreplus
-Version: 0.3.8
+Version: 0.3.9
 Summary: Django functional modules
 Home-page: https://gitlab.com/zeroplus/django/django-coreplus
 Author: Zero Plus
 Author-email: sasri.works@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/zeroplus/django/django-coreplus/-/wikis/
 Project-URL: Source, https://gitlab.com/zeroplus/django/django-coreplus
```

### Comparing `django-coreplus-0.3.8/README.md` & `django-coreplus-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/base.py` & `django-coreplus-0.3.9/coreplus/admin/base.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/filters.py` & `django-coreplus-0.3.9/coreplus/admin/filters.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/admin/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/admin/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/mixins.py` & `django-coreplus-0.3.9/coreplus/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/sites.py` & `django-coreplus-0.3.9/coreplus/admin/sites.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/static/coreplus_admin/js/alpine.min.js` & `django-coreplus-0.3.9/coreplus/admin/static/coreplus_admin/js/alpine.min.js`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/static/coreplus_admin/js/htmx.min.js` & `django-coreplus-0.3.9/coreplus/admin/static/coreplus_admin/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/static/coreplus_admin/js/jquery.min.js` & `django-coreplus-0.3.9/coreplus/admin/static/coreplus_admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/templates/admin/base.html` & `django-coreplus-0.3.9/coreplus/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/templates/admin/form_view.html` & `django-coreplus-0.3.9/coreplus/admin/templates/admin/form_view.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/templates/admin/inspect.html` & `django-coreplus-0.3.9/coreplus/admin/templates/admin/inspect.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/admin/templates/admin/inspect_object_tools.html` & `django-coreplus-0.3.9/coreplus/admin/templates/admin/inspect_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/api/README.md` & `django-coreplus-0.3.9/coreplus/api/README.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/api/endpoints/v1.py` & `django-coreplus-0.3.9/coreplus/api/endpoints/v1.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/api/endpoints/v2.py` & `django-coreplus-0.3.9/coreplus/api/endpoints/v2.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/api/helpers.py` & `django-coreplus-0.3.9/coreplus/api/helpers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/api/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/api/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/api/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/api/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/api/templates/drf_spectacular/redoc.html` & `django-coreplus-0.3.9/coreplus/api/templates/drf_spectacular/redoc.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/configs.py` & `django-coreplus-0.3.9/coreplus/configs.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/abstracts.py` & `django-coreplus-0.3.9/coreplus/contacts/abstracts.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/inlines.py` & `django-coreplus-0.3.9/coreplus/contacts/inlines.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/contacts/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/contacts/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/management/commands/populate_countries.py` & `django-coreplus-0.3.9/coreplus/contacts/management/commands/populate_countries.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/contacts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/migrations/0002_alter_billingaddress_address_and_more.py` & `django-coreplus-0.3.9/coreplus/contacts/migrations/0002_alter_billingaddress_address_and_more.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/migrations/0003_billingaddress_district_deliverableaddress_district_and_more.py` & `django-coreplus-0.3.9/coreplus/contacts/migrations/0003_billingaddress_district_deliverableaddress_district_and_more.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/contacts/models.py` & `django-coreplus-0.3.9/coreplus/contacts/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/discuss/api/v1/serializers.py` & `django-coreplus-0.3.9/coreplus/discuss/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/discuss/api/v1/viewsets.py` & `django-coreplus-0.3.9/coreplus/discuss/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/discuss/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/discuss/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/discuss/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/discuss/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/discuss/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/discuss/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/discuss/migrations/0002_alter_discuss_flag.py` & `django-coreplus-0.3.9/coreplus/discuss/migrations/0002_alter_discuss_flag.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/discuss/models.py` & `django-coreplus-0.3.9/coreplus/discuss/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/docs/templates/docs/_base_two.html` & `django-coreplus-0.3.9/coreplus/docs/templates/docs/_base_two.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/docs/tests/runtests.py` & `django-coreplus-0.3.9/coreplus/docs/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/docs/tests/test_views.py` & `django-coreplus-0.3.9/coreplus/docs/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/docs/views.py` & `django-coreplus-0.3.9/coreplus/docs/views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/heralds/admin.py` & `django-coreplus-0.3.9/coreplus/heralds/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/heralds/api/v1/serializers.py` & `django-coreplus-0.3.9/coreplus/heralds/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/heralds/api/v1/viewsets.py` & `django-coreplus-0.3.9/coreplus/heralds/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/heralds/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/heralds/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/heralds/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/heralds/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/heralds/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/heralds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/heralds/models.py` & `django-coreplus-0.3.9/coreplus/heralds/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/heralds/tests.py` & `django-coreplus-0.3.9/coreplus/heralds/tests.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/hooks/README.md` & `django-coreplus-0.3.9/coreplus/hooks/README.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/hooks/admin.py` & `django-coreplus-0.3.9/coreplus/hooks/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/hooks/core.py` & `django-coreplus-0.3.9/coreplus/hooks/core.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/hooks/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/hooks/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/hooks/templates/admin/coreplus_hooks/hooks_registry.html` & `django-coreplus-0.3.9/coreplus/hooks/templates/admin/coreplus_hooks/hooks_registry.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/__init__.py` & `django-coreplus-0.3.9/coreplus/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/bleaching.py` & `django-coreplus-0.3.9/coreplus/markdown/bleaching.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/markdown/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/markdown/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/plugins/gist.py` & `django-coreplus-0.3.9/coreplus/markdown/plugins/gist.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/plugins/linkify.py` & `django-coreplus-0.3.9/coreplus/markdown/plugins/linkify.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/plugins/twitter.py` & `django-coreplus-0.3.9/coreplus/markdown/plugins/twitter.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/plugins/youtube.py` & `django-coreplus-0.3.9/coreplus/markdown/plugins/youtube.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/markdown/tests.py` & `django-coreplus-0.3.9/coreplus/markdown/tests.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/media/api/v1/serializers.py` & `django-coreplus-0.3.9/coreplus/media/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/media/api/v1/viewsets.py` & `django-coreplus-0.3.9/coreplus/media/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/media/helpers.py` & `django-coreplus-0.3.9/coreplus/media/helpers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/media/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/media/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/media/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/media/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/media/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/media/models.py` & `django-coreplus-0.3.9/coreplus/media/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/navigators/README.md` & `django-coreplus-0.3.9/coreplus/navigators/README.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/navigators/apps.py` & `django-coreplus-0.3.9/coreplus/navigators/apps.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/navigators/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/navigators/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/navigators/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/navigators/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/navigators/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/navigators/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/navigators/models.py` & `django-coreplus-0.3.9/coreplus/navigators/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/navigators/templatetags/navigators_tags.py` & `django-coreplus-0.3.9/coreplus/navigators/templatetags/navigators_tags.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/notices/admin.py` & `django-coreplus-0.3.9/coreplus/notices/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 from django.contrib import admin, messages
+
 # from django.http.response import HttpResponseRedirect
 # from django.shortcuts import get_object_or_404
 # from django.urls import re_path
+from push_notifications.admin import DeviceAdmin
 from django.utils.translation import gettext_lazy as _
 
-from .models import Broadcast
+from .models import Broadcast, FirebaseDevice
+
+
+@admin.register(FirebaseDevice)
+class FirebaseDeviceAdmin(DeviceAdmin):
+    list_display = (
+        "__str__",
+        "device_id",
+        "user",
+        "active",
+        "date_created",
+        "cloud_message_type",
+    )
+    list_filter = ("active", "cloud_message_type")
 
 
 @admin.register(Broadcast)
 class BroadcastModelAdmin(admin.ModelAdmin):
     menu_order = 9
     model = Broadcast
     menu_label = _("Broadcasts")
```

### Comparing `django-coreplus-0.3.8/coreplus/notices/api/v1/viewsets.py` & `django-coreplus-0.3.9/coreplus/notices/api/v1/viewsets.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 from django.shortcuts import get_object_or_404
 from drf_spectacular.utils import extend_schema
 from notifications.models import Notification
 from rest_framework.decorators import action
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.viewsets import ReadOnlyModelViewSet, mixins
+from ...models import FirebaseDevice
+from .serializers import NotificationSerializer, FirebaseDeviceSerializer
+from push_notifications.api.rest_framework import DeviceViewSetMixin, ModelViewSet
 
-from .serializers import NotificationSerializer
+
+class FirebaseDeviceViewSet(DeviceViewSetMixin, ModelViewSet):
+    queryset = FirebaseDevice.objects.all()
+    serializer_class = FirebaseDeviceSerializer
 
 
 class NotificationViewSet(mixins.DestroyModelMixin, ReadOnlyModelViewSet):
     queryset = Notification.objects.all()
     permission_classes = [IsAuthenticated]
     serializer_class = NotificationSerializer
```

### Comparing `django-coreplus-0.3.8/coreplus/notices/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/notices/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/notices/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/notices/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/notices/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/notices/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py` & `django-coreplus-0.3.9/coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/notices/models.py` & `django-coreplus-0.3.9/coreplus/notices/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 from django.core.mail import send_mass_mail
 from django.db import models
 from django.db.models.query import QuerySet
 from django.template.loader import render_to_string
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _  # NOQA
 
-from push_notifications.gcm import GCMDevice
+from push_notifications.models import (
+    Device,
+    SETTINGS,
+    CLOUD_MESSAGE_TYPES,
+    GCMDeviceManager,
+)
 from swapper import load_model
 
 from .signals import bulk_notify, firebase_push_notify
 
 User = get_user_model()
 
 
@@ -44,14 +49,57 @@
         verbose_name = _("Notification Preference")
         verbose_name_plural = _("Notification Preferences")
 
     def __str__(self):
         return f"{self.user}"
 
 
+class FirebaseDevice(Device):
+    device_id = models.CharField(
+        verbose_name=_("Device ID"),
+        blank=True,
+        null=True,
+        db_index=True,
+        max_length=255,
+        help_text=_("Device ID"),
+    )
+    registration_id = models.TextField(
+        verbose_name=_("Registration ID"), unique=SETTINGS["UNIQUE_REG_ID"]
+    )
+    cloud_message_type = models.CharField(
+        verbose_name=_("Cloud Message Type"),
+        max_length=3,
+        choices=CLOUD_MESSAGE_TYPES,
+        default="GCM",
+        help_text=_("You should choose FCM or GCM"),
+    )
+    objects = GCMDeviceManager()
+
+    class Meta:
+        verbose_name = _("Firebase device")
+
+    def send_message(self, message, **kwargs):
+        from push_notifications.gcm import send_message as gcm_send_message
+
+        data = kwargs.pop("extra", {})
+        if message is not None:
+            data["message"] = message
+
+        return gcm_send_message(
+            self.registration_id,
+            data,
+            self.cloud_message_type,
+            application_id=self.application_id,
+            **kwargs,
+        )
+
+    def save(self, *args, **kwargs) -> None:
+        return super().save(*args, **kwargs)
+
+
 class Broadcast(models.Model):
     EMAIL = "email"
     NOTIFICATION = "notification"
     ANDROID_NOTIFICATION = "android_notification"
     APPLE_NOTIFICATION = "apple_notification"
     ALL_MEDIA = "all"
 
@@ -297,18 +345,17 @@
     return results
 
 
 def firebase_notification_handler(recipients, title, message, **kwargs):
     kwargs.pop("signal", None)
     kwargs.pop("sender", None)
     recipient_ids = [user.id for user in recipients]
-    gcm_devices = GCMDevice.objects.filter(user_id__in=recipient_ids, active=True)
-    print(gcm_devices)
+    fcm_devices = FirebaseDevice.objects.filter(user_id__in=recipient_ids, active=True)
     try:
-        gcm_devices.send_message(message, title=title, extra=kwargs)
+        fcm_devices.send_message(message, title=title, extra=kwargs)
     except Exception as err:
         print(err)
 
 
 # Connect the signal
 bulk_notify.connect(
     bulk_notification_handler, dispatch_uid="notifications.models.notification"
```

### Comparing `django-coreplus-0.3.8/coreplus/numerators/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/numerators/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/numerators/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/numerators/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/numerators/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/numerators/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/numerators/models.py` & `django-coreplus-0.3.9/coreplus/numerators/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/profanity/extras.py` & `django-coreplus-0.3.9/coreplus/profanity/extras.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/profanity/wordlist.txt` & `django-coreplus-0.3.9/coreplus/profanity/wordlist.txt`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/qrcodes/models.py` & `django-coreplus-0.3.9/coreplus/qrcodes/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/reactions/admin.py` & `django-coreplus-0.3.9/coreplus/reactions/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/reactions/api/v1/serializers.py` & `django-coreplus-0.3.9/coreplus/reactions/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/reactions/apps.py` & `django-coreplus-0.3.9/coreplus/reactions/apps.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/reactions/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/reactions/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/reactions/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/reactions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/reactions/models.py` & `django-coreplus-0.3.9/coreplus/reactions/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/search/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/search/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/search/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/search/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/search/templates/search/search.html` & `django-coreplus-0.3.9/coreplus/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/search/templatetags/search_tags.py` & `django-coreplus-0.3.9/coreplus/search/templatetags/search_tags.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/search/views.py` & `django-coreplus-0.3.9/coreplus/search/views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/admin.py` & `django-coreplus-0.3.9/coreplus/settings/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/contexts.py` & `django-coreplus-0.3.9/coreplus/settings/contexts.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.9/coreplus/settings/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/settings/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/models.py` & `django-coreplus-0.3.9/coreplus/settings/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/permissions.py` & `django-coreplus-0.3.9/coreplus/settings/permissions.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/registries.py` & `django-coreplus-0.3.9/coreplus/settings/registries.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/templates/admin/settings/edit.html` & `django-coreplus-0.3.9/coreplus/settings/templates/admin/settings/edit.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/templatetags/settings_tags.py` & `django-coreplus-0.3.9/coreplus/settings/templatetags/settings_tags.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/settings/views.py` & `django-coreplus-0.3.9/coreplus/settings/views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/shorts/api/v1/viewsets.py` & `django-coreplus-0.3.9/coreplus/shorts/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/shorts/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.9/coreplus/shorts/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/shorts/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/shorts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/shorts/models.py` & `django-coreplus-0.3.9/coreplus/shorts/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/shorts/utils.py` & `django-coreplus-0.3.9/coreplus/shorts/utils.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/shorts/views.py` & `django-coreplus-0.3.9/coreplus/shorts/views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/spams/extras.py` & `django-coreplus-0.3.9/coreplus/spams/extras.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/spams/static/model_and_vectorizer_with_pickle(en).pkl` & `django-coreplus-0.3.9/coreplus/spams/static/model_and_vectorizer_with_pickle(en).pkl`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/spams/static/model_and_vectorizer_with_pickle(id).pkl` & `django-coreplus-0.3.9/coreplus/spams/static/model_and_vectorizer_with_pickle(id).pkl`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/spams/tests.py` & `django-coreplus-0.3.9/coreplus/spams/tests.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/tags/admin.py` & `django-coreplus-0.3.9/coreplus/tags/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/tags/api/v1/serializers.py` & `django-coreplus-0.3.9/coreplus/tags/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/tags/api/v1/viewsets.py` & `django-coreplus-0.3.9/coreplus/tags/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/tags/migrations/0001_initial.py` & `django-coreplus-0.3.9/coreplus/tags/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/tags/models.py` & `django-coreplus-0.3.9/coreplus/tags/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/tags/resources.py` & `django-coreplus-0.3.9/coreplus/tags/resources.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/avatars.py` & `django-coreplus-0.3.9/coreplus/utils/avatars.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/contenttypes.py` & `django-coreplus-0.3.9/coreplus/utils/contenttypes.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/currencies.py` & `django-coreplus-0.3.9/coreplus/utils/currencies.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/decorators.py` & `django-coreplus-0.3.9/coreplus/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/forms/fields.py` & `django-coreplus-0.3.9/coreplus/utils/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/loading.py` & `django-coreplus-0.3.9/coreplus/utils/loading.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/models/actions.py` & `django-coreplus-0.3.9/coreplus/utils/models/actions.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/models/choices.py` & `django-coreplus-0.3.9/coreplus/utils/models/choices.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/models/fields.py` & `django-coreplus-0.3.9/coreplus/utils/models/fields.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/models/managers.py` & `django-coreplus-0.3.9/coreplus/utils/models/managers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/models/models.py` & `django-coreplus-0.3.9/coreplus/utils/models/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/models/paranoid.py` & `django-coreplus-0.3.9/coreplus/utils/models/paranoid.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/models/signals.py` & `django-coreplus-0.3.9/coreplus/utils/models/signals.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/models/tracker.py` & `django-coreplus-0.3.9/coreplus/utils/models/tracker.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/slugs.py` & `django-coreplus-0.3.9/coreplus/utils/slugs.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/utils/validators.py` & `django-coreplus-0.3.9/coreplus/utils/validators.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/coreplus/version.py` & `django-coreplus-0.3.9/coreplus/version.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.8/django_coreplus.egg-info/PKG-INFO` & `django-coreplus-0.3.9/django_coreplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-coreplus
-Version: 0.3.8
+Version: 0.3.9
 Summary: Django functional modules
 Home-page: https://gitlab.com/zeroplus/django/django-coreplus
 Author: Zero Plus
 Author-email: sasri.works@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/zeroplus/django/django-coreplus/-/wikis/
 Project-URL: Source, https://gitlab.com/zeroplus/django/django-coreplus
```

### Comparing `django-coreplus-0.3.8/django_coreplus.egg-info/SOURCES.txt` & `django-coreplus-0.3.9/django_coreplus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,16 @@
 coreplus/notices/api/v1/serializers.py
 coreplus/notices/api/v1/urls.py
 coreplus/notices/api/v1/viewsets.py
 coreplus/notices/locale/id/LC_MESSAGES/django.mo
 coreplus/notices/locale/id/LC_MESSAGES/django.po
 coreplus/notices/migrations/0001_initial.py
 coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py
+coreplus/notices/migrations/0003_firebasedevice.py
+coreplus/notices/migrations/0004_alter_firebasedevice_options.py
 coreplus/notices/migrations/__init__.py
 coreplus/notices/templates/notices/email_broadcast.txt
 coreplus/numerators/README.md
 coreplus/numerators/__init__.py
 coreplus/numerators/admin.py
 coreplus/numerators/apps.py
 coreplus/numerators/models.py
```

### Comparing `django-coreplus-0.3.8/setup.cfg` & `django-coreplus-0.3.9/setup.cfg`

 * *Files identical despite different names*

