# Comparing `tmp/django-beam-1.3.3.tar.gz` & `tmp/django-beam-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-beam-1.3.3.tar", last modified: Thu Apr 27 07:27:42 2023, max compression
+gzip compressed data, was "django-beam-1.4.0.tar", last modified: Wed May 17 08:51:14 2023, max compression
```

## Comparing `django-beam-1.3.3.tar` & `django-beam-1.4.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.862520 django-beam-1.3.3/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.3.3/LICENSE
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.3.3/MANIFEST.in
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-04-27 07:27:42.862623 django-beam-1.3.3/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.3.3/README.md
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-04-27 07:27:42.863952 django-beam-1.3.3/setup.cfg
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.3.3/setup.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.841917 django-beam-1.3.3/src/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.845881 django-beam-1.3.3/src/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/components.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.846087 django-beam-1.3.3/src/beam/contrib/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.846789 django-beam-1.3.3/src/beam/contrib/auth/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/apps.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/forms.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.840465 django-beam-1.3.3/src/beam/contrib/auth/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.848244 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/logged_out.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/login.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_change_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_change_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_complete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_email.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/auth/views.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.848406 django-beam-1.3.3/src/beam/contrib/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/autocomplete_light/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.840674 django-beam-1.3.3/src/beam/contrib/autocomplete_light/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.848560 django-beam-1.3.3/src/beam/contrib/autocomplete_light/static/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-04-27 06:36:15.000000 django-beam-1.3.3/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.849330 django-beam-1.3.3/src/beam/contrib/reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/reversion/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/reversion/apps.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.840873 django-beam-1.3.3/src/beam/contrib/reversion/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.849753 django-beam-1.3.3/src/beam/contrib/reversion/templates/beam_reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/reversion/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/contrib/reversion/viewsets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/layouts.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.841004 django-beam-1.3.3/src/beam/locale/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.841058 django-beam-1.3.3/src/beam/locale/de/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.849918 django-beam-1.3.3/src/beam/locale/de/LC_MESSAGES/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/registry.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.850198 django-beam-1.3.3/src/beam/templatetags/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/templatetags/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8414 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/templatetags/beam_tags.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.850357 django-beam-1.3.3/src/beam/themes/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.850547 django-beam-1.3.3/src/beam/themes/bootstrap4/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.841425 django-beam-1.3.3/src/beam/themes/bootstrap4/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.841615 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.850722 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/css/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.852042 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/actions.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1328 2023-04-27 07:25:44.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/add_related.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/inlines.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    82676 2023-04-27 07:24:58.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.841760 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.854698 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3352 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/base.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/create.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1668 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/dashboard.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2444 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/delete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8134 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/list.html
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.857934 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1756 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1954 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4380 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1289 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      553 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6084 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3061 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-04-27 07:20:15.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4586 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2072 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4788 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4968 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/update.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/themes/bootstrap4/widgets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/types.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-04-27 06:10:00.000000 django-beam-1.3.3/src/beam/viewsets.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.858567 django-beam-1.3.3/src/django_beam.egg-info/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-04-27 07:27:42.000000 django-beam-1.3.3/src/django_beam.egg-info/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-04-27 07:27:42.000000 django-beam-1.3.3/src/django_beam.egg-info/SOURCES.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-04-27 07:27:42.000000 django-beam-1.3.3/src/django_beam.egg-info/dependency_links.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-04-27 07:27:42.000000 django-beam-1.3.3/src/django_beam.egg-info/requires.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-04-27 07:27:42.000000 django-beam-1.3.3/src/django_beam.egg-info/top_level.txt
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:27:42.862361 django-beam-1.3.3/tests/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.3.3/tests/test_actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.3.3/tests/test_components.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.3.3/tests/test_contrib_auth.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.3.3/tests/test_contrib_autocomplete.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.3.3/tests/test_contrib_reversion.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.3.3/tests/test_inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.3.3/tests/test_layouts.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.3.3/tests/test_registry.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2352 2023-01-11 09:59:58.000000 django-beam-1.3.3/tests/test_tags.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.3.3/tests/test_urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.3.3/tests/test_utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    31258 2023-03-30 10:35:40.000000 django-beam-1.3.3/tests/test_views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.3.3/tests/test_viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.664585 django-beam-1.4.0/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.4.0/LICENSE
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.4.0/MANIFEST.in
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-05-17 08:51:14.664677 django-beam-1.4.0/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.4.0/README.md
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-05-17 08:51:14.665074 django-beam-1.4.0/setup.cfg
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.4.0/setup.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644819 django-beam-1.4.0/src/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.648121 django-beam-1.4.0/src/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/components.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.648272 django-beam-1.4.0/src/beam/contrib/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.649167 django-beam-1.4.0/src/beam/contrib/auth/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/apps.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/forms.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.643530 django-beam-1.4.0/src/beam/contrib/auth/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.650959 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/logged_out.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/login.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_change_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_change_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_complete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_email.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/views.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.651150 django-beam-1.4.0/src/beam/contrib/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/autocomplete_light/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.643729 django-beam-1.4.0/src/beam/contrib/autocomplete_light/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.651347 django-beam-1.4.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.651984 django-beam-1.4.0/src/beam/contrib/reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/apps.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.643915 django-beam-1.4.0/src/beam/contrib/reversion/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.652332 django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/viewsets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/layouts.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644036 django-beam-1.4.0/src/beam/locale/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644087 django-beam-1.4.0/src/beam/locale/de/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.652499 django-beam-1.4.0/src/beam/locale/de/LC_MESSAGES/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/registry.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.652806 django-beam-1.4.0/src/beam/templatetags/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/templatetags/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8705 2023-05-17 08:50:04.000000 django-beam-1.4.0/src/beam/templatetags/beam_tags.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.653098 django-beam-1.4.0/src/beam/themes/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.653338 django-beam-1.4.0/src/beam/themes/bootstrap4/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644411 django-beam-1.4.0/src/beam/themes/bootstrap4/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644533 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.653555 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/css/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.654692 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/actions.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1328 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/add_related.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/inlines.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    82676 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644667 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.656670 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3374 2023-05-17 08:50:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/base.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/create.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1668 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/dashboard.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2444 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/delete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8134 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/list.html
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.659600 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1756 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1954 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4380 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1289 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      553 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6084 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3061 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4586 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2072 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4826 2023-05-17 08:50:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4968 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/update.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/widgets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/types.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-05-17 08:50:04.000000 django-beam-1.4.0/src/beam/utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.660361 django-beam-1.4.0/src/django_beam.egg-info/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/requires.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/top_level.txt
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.664416 django-beam-1.4.0/tests/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.4.0/tests/test_components.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.4.0/tests/test_contrib_auth.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_contrib_autocomplete.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.4.0/tests/test_contrib_reversion.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_layouts.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_registry.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-05-17 08:50:04.000000 django-beam-1.4.0/tests/test_tags.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.4.0/tests/test_urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.4.0/tests/test_utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    31258 2023-03-30 10:35:40.000000 django-beam-1.4.0/tests/test_views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_viewsets.py
```

### Comparing `django-beam-1.3.3/LICENSE` & `django-beam-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/PKG-INFO` & `django-beam-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.3.3
+Version: 1.4.0
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.3.3.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.4.0.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-beam-1.3.3/README.md` & `django-beam-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/setup.cfg` & `django-beam-1.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = django-beam
-version = 1.3.3
+version = 1.4.0
 description = A crud library for python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/django-beam/django-beam
-download_url = https://github.com/django-beam/django-beam/archive/1.3.3.tar.gz
+download_url = https://github.com/django-beam/django-beam/archive/1.4.0.tar.gz
 author = Raphael Kimmig
 author_email = raphael@ampad.de
 keywords = 
 license = BSD 3-Clause License
 classifiers = 
 	Framework :: Django
 	Programming Language :: Python :: 3
```

### Comparing `django-beam-1.3.3/src/beam/actions.py` & `django-beam-1.4.0/src/beam/actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/components.py` & `django-beam-1.4.0/src/beam/components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/auth/forms.py` & `django-beam-1.4.0/src/beam/contrib/auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/auth/templates/registration/login.html` & `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_change_form.html` & `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_confirm.html` & `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_done.html` & `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_email.html` & `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/auth/templates/registration/password_reset_form.html` & `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/auth/views.py` & `django-beam-1.4.0/src/beam/contrib/auth/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/autocomplete_light/__init__.py` & `django-beam-1.4.0/src/beam/contrib/autocomplete_light/__init__.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css` & `django-beam-1.4.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html` & `django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/reversion/templates/beam_reversion/version_list.html` & `django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/version_list.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/reversion/views.py` & `django-beam-1.4.0/src/beam/contrib/reversion/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/contrib/reversion/viewsets.py` & `django-beam-1.4.0/src/beam/contrib/reversion/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/inlines.py` & `django-beam-1.4.0/src/beam/inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/layouts.py` & `django-beam-1.4.0/src/beam/layouts.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/locale/de/LC_MESSAGES/django.mo` & `django-beam-1.4.0/src/beam/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/registry.py` & `django-beam-1.4.0/src/beam/registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/templatetags/beam_tags.py` & `django-beam-1.4.0/src/beam/templatetags/beam_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,19 +179,19 @@
 def any_filter(iterable):
     if not iterable:
         return False
     return any(iterable)
 
 
 @register.simple_tag(takes_context=True)
-def render_navigation(context):
+def get_apps_for_navigation(context):
     request = context.get("request", None)
     user = request.user if request else None
 
-    grouped = []
+    apps_with_entries = []
     for app_label, viewsets_dict in default_registry.items():
         entries = []
         for viewset in viewsets_dict.values():
             entry = navigation_component_entry(
                 viewset().links.get("list"), user=user, request=request
             )
             if entry:
@@ -201,18 +201,29 @@
             continue
 
         group = {
             "app_label": app_label,
             "app_config": apps.get_app_config(app_label),
             "entries": entries,
         }
-        grouped.append(group)
-    navigation_template = get_template("beam/partials/navigation.html")
+        apps_with_entries.append(group)
+    return apps_with_entries
+
+
+@register.simple_tag(takes_context=True)
+def render_navigation(context):
+    """
+    Render the navigation template with the apps.
+
+    Deprecated: use get_apps_for_navigation instead.
+    """
+    apps = get_apps_for_navigation(context)
     request = context.get("request", None)
-    return navigation_template.render({"apps": grouped, "request": request})
+    navigation_template = get_template("beam/partials/navigation.html")
+    return navigation_template.render({"apps": apps, "request": request})
 
 
 @register.simple_tag()
 def fields_to_layout(fields):
     return [[fields]]
```

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css` & `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/actions.js` & `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/actions.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/add_related.js` & `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/add_related.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js` & `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/inlines.js` & `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/inlines.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js` & `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/base.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 <body class="beam {% if popup %}popup {% endif %}{% block body_classes %}{% endblock %}">
 
     {% block layout %}
 
         {% block navigation %}
-            {% render_navigation %}
+            {% include "beam/partials/navigation.html" %}
         {% endblock %}
 
         {% block messages_container %}
             {% if messages %}
                 <div class="container">
                     {% block messages %}
                         {% include "beam/partials/messages.html" %}
```

#### html2text {}

```diff
@@ -4,16 +4,17 @@
 {% block meta %}
 
  {% block extra_meta %}{% endblock %} {% endblock %}
 {% block styles %} {% block bootstrap_styles %}
 
  {% endblock %} {% block extra_styles %}{% endblock %} {% endblock %} {% block
 extra_head %}{% endblock %}
-{% block layout %} {% block navigation %} {% render_navigation %} {% endblock
-%} {% block messages_container %} {% if messages %}
+{% block layout %} {% block navigation %} {% include "beam/partials/
+navigation.html" %} {% endblock %} {% block messages_container %} {% if
+messages %}
 {% block messages %} {% include "beam/partials/messages.html" %} {% endblock %}
 {% endif %} {% endblock %} {% block content_container %}
 {% block content %}{% endblock %}
 {% endblock %} {% endblock %} {% block scripts %}  {% block jquery %}
  {% endblock %} {% block bootstrap_scripts %}
  {% endblock %} {% block beam_scripts %}
 s/sortable.min.js" %}">
```

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/dashboard.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/delete.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/delete.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/detail.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/form.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/list.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/list.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/actions.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/actions.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/filters.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/filters.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/layout.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/layout.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/links.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/messages.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/messages.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% load i18n %}
 {% load beam_tags %}
 
 {% block navigation_container %}
+{% get_apps_for_navigation as apps %}
 <nav class="navbar navbar-expand-md navbar-light shadow-sm border-bottom bg-light mb-3">
     <div class="container">
     {% block navigation %}
 
         {% block navbar_brand %}
             {% url "dashboard" as dashboard_url %}
             <a class="navbar-brand" href="{{ dashboard_url|default:'/' }}">
```

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/templates/beam/update.html` & `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/update.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/themes/bootstrap4/widgets.py` & `django-beam-1.4.0/src/beam/themes/bootstrap4/widgets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/urls.py` & `django-beam-1.4.0/src/beam/urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/utils.py` & `django-beam-1.4.0/src/beam/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     return user.has_perm(permission)
 
 
 def navigation_component_entry(
     component=None, user=None, request=None
 ) -> Optional[Tuple[str, str]]:
     """
-    Get an optional tuple (label, url) for a given compoment to use in render_navigation
+    Get an optional tuple (label, url) for a given component to use in render_navigation
     """
     if not component:
         return None
 
     if not component.has_perm(user=user, obj=None, request=request):
         return None
```

### Comparing `django-beam-1.3.3/src/beam/views.py` & `django-beam-1.4.0/src/beam/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/beam/viewsets.py` & `django-beam-1.4.0/src/beam/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/src/django_beam.egg-info/PKG-INFO` & `django-beam-1.4.0/src/django_beam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.3.3
+Version: 1.4.0
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.3.3.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.4.0.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-beam-1.3.3/src/django_beam.egg-info/SOURCES.txt` & `django-beam-1.4.0/src/django_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_actions.py` & `django-beam-1.4.0/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_components.py` & `django-beam-1.4.0/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_contrib_auth.py` & `django-beam-1.4.0/tests/test_contrib_auth.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_contrib_autocomplete.py` & `django-beam-1.4.0/tests/test_contrib_autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_contrib_reversion.py` & `django-beam-1.4.0/tests/test_contrib_reversion.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_inlines.py` & `django-beam-1.4.0/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_registry.py` & `django-beam-1.4.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_tags.py` & `django-beam-1.4.0/tests/test_tags.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from django.template import RequestContext
 from django.test import RequestFactory, TestCase
 from django.urls import NoReverseMatch
 from test_views import user_with_perms
 from testapp.models import Dragonfly
 from testapp.views import DragonflyViewSet
 
 from beam.templatetags.beam_tags import (
     _add_params_to_url_if_new,
+    get_apps_for_navigation,
     get_visible_links,
     preserve_query_string,
 )
 
 
 class TagsTest(TestCase):
     def test_preserve_query_string_preserves_query_string(self):
@@ -59,7 +61,28 @@
             links=DragonflyViewSet().links,
             link_layout=["detail", "update", "create"],
             obj=Dragonfly(pk=123),
         )
         self.assertEqual(
             {component.name for component, url in links}, {"create", "detail"}
         )
+
+    def test_apps_for_navigation(self):
+        request = RequestFactory().get("/")
+        request.user = user_with_perms(
+            ["testapp.view_dragonfly", "testapp.view_sighting"]
+        )
+        context = RequestContext(request, {"request": request})
+        apps = get_apps_for_navigation(context=context)
+        self.assertEqual(len(apps), 1)
+        self.assertEqual(apps[0]["app_label"], "testapp")
+        self.assertEqual(
+            apps[0]["entries"],
+            [("dragonflys", "/dragonfly/"), ("sightings", "/sighting/")],
+        )
+
+    def test_apps_for_navigation_require_permission(self):
+        request = RequestFactory().get("/")
+        request.user = user_with_perms([])
+        context = RequestContext(request, {"request": request})
+        apps = get_apps_for_navigation(context=context)
+        self.assertEqual(apps, [])
```

### Comparing `django-beam-1.3.3/tests/test_urls.py` & `django-beam-1.4.0/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_utils.py` & `django-beam-1.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_views.py` & `django-beam-1.4.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.3/tests/test_viewsets.py` & `django-beam-1.4.0/tests/test_viewsets.py`

 * *Files identical despite different names*

