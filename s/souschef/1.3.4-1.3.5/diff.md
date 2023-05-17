# Comparing `tmp/souschef-1.3.4.tar.gz` & `tmp/souschef-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/souschef-1.3.4.tar", last modified: Fri Mar 12 20:48:44 2021, max compression
+gzip compressed data, was "dist/souschef-1.3.5.tar", last modified: Fri Apr  2 20:32:13 2021, max compression
```

## Comparing `souschef-1.3.4.tar` & `souschef-1.3.5.tar`

### file list

```diff
@@ -1,424 +1,428 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/
--rw-r--r--   0 root         (0) root         (0)     5729 2021-03-02 23:43:41.000000 souschef-1.3.4/INSTALL.md
--rw-r--r--   0 root         (0) root         (0)    33893 2020-11-20 01:08:04.000000 souschef-1.3.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      230 2021-01-23 15:51:37.000000 souschef-1.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2522 2021-03-12 20:48:44.000000 souschef-1.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1366 2021-01-22 18:52:15.000000 souschef-1.3.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1409 2021-01-23 16:03:53.000000 souschef-1.3.4/UPDATE.md
--rw-r--r--   0 root         (0) root         (0)      114 2021-03-12 20:48:44.000000 souschef-1.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1781 2021-03-12 20:47:40.000000 souschef-1.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/
--rw-r--r--   0 root         (0) root         (0)    32621 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/admin.py
--rw-r--r--   0 root         (0) root         (0)       89 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/apps.py
--rw-r--r--   0 root         (0) root         (0)      358 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/billing/migrations/
--rw-r--r--   0 root         (0) root         (0)      983 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      494 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/migrations/0002_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)      435 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/migrations/0003_auto_20161122_0515.py
--rw-r--r--   0 root         (0) root         (0)      439 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/migrations/0004_auto_20201030_1540.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5339 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/billing/templates/
--rw-r--r--   0 root         (0) root         (0)       42 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/base_billing.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/billing/templates/billing/
--rw-r--r--   0 root         (0) root         (0)     4897 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/billing/add.html
--rw-r--r--   0 root         (0) root         (0)      863 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/billing/billing_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     3310 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/billing/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/billing/templates/billing/partials/
--rw-r--r--   0 root         (0) root         (0)      531 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/billing/partials/statistics.html
--rw-r--r--   0 root         (0) root         (0)     5148 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/billing/partials/summary.html
--rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/billing/print_summary.html
--rw-r--r--   0 root         (0) root         (0)      822 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/billing/view.html
--rw-r--r--   0 root         (0) root         (0)     3398 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/templates/billing/view_orders.html
--rw-r--r--   0 root         (0) root         (0)     8493 2020-12-19 18:25:21.000000 souschef-1.3.4/souschef/billing/tests.py
--rw-r--r--   0 root         (0) root         (0)      718 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/urls.py
--rw-r--r--   0 root         (0) root         (0)    11692 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/billing/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/configsamples/
--rw-r--r--   0 root         (0) root         (0)      809 2021-03-02 23:43:41.000000 souschef-1.3.4/souschef/configsamples/nginx.conf
--rw-r--r--   0 root         (0) root         (0)      409 2020-12-19 18:25:21.000000 souschef-1.3.4/souschef/configsamples/souschef.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/cronscripts/
--rwxr-xr-x   0 root         (0) root         (0)      469 2021-01-23 16:08:34.000000 souschef-1.3.4/souschef/cronscripts/souschef_daily.sh
--rw-r--r--   0 root         (0) root         (0)      361 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/dataexec.py
--rw-r--r--   0 root         (0) root         (0)    81444 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/dataload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/datamigration/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/__init__.py
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/admin.py
--rw-r--r--   0 root         (0) root         (0)      101 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/datamigration/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:34.000000 souschef-1.3.4/souschef/datamigration/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/datamigration/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:11.000000 souschef-1.3.4/souschef/datamigration/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2178 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/management/commands/importaddresses.py
--rw-r--r--   0 root         (0) root         (0)     3174 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/management/commands/importclients.py
--rw-r--r--   0 root         (0) root         (0)     3106 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/management/commands/importcontactaddresses.py
--rw-r--r--   0 root         (0) root         (0)     3956 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/management/commands/importmeals.py
--rw-r--r--   0 root         (0) root         (0)     2593 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/management/commands/importorders.py
--rw-r--r--   0 root         (0) root         (0)     3306 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/management/commands/importrelationships.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/datamigration/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       58 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/models.py
--rw-r--r--   0 root         (0) root         (0)     9202 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/tests.py
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/datamigration/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/delivery/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/admin.py
--rwxr-xr-x   0 root         (0) root         (0)       91 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/apps.py
--rw-r--r--   0 root         (0) root         (0)      906 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/filters.py
--rw-r--r--   0 root         (0) root         (0)     1406 2021-03-12 20:47:33.000000 souschef-1.3.4/souschef/delivery/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/delivery/migrations/
--rw-r--r--   0 root         (0) root         (0)      582 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/migrations/0001_fix004a.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      218 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/delivery/templates/
--rw-r--r--   0 root         (0) root         (0)    11997 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/templates/edit_delivery_of_today.html
--rw-r--r--   0 root         (0) root         (0)     3511 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/templates/ingredients.html
--rw-r--r--   0 root         (0) root         (0)     4057 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/templates/kitchen_count.html
--rw-r--r--   0 root         (0) root         (0)     1183 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/templates/kitchen_count_steps.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/delivery/templates/partials/
--rw-r--r--   0 root         (0) root         (0)     3436 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/templates/partials/generated_orders.html
--rw-r--r--   0 root         (0) root         (0)     4349 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/templates/review_orders.html
--rw-r--r--   0 root         (0) root         (0)     3362 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/templates/route_sheet.html
--rw-r--r--   0 root         (0) root         (0)     4993 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/templates/routes.html
--rwxr-xr-x   0 root         (0) root         (0)    47234 2020-12-19 16:05:35.000000 souschef-1.3.4/souschef/delivery/tests.py
--rw-r--r--   0 root         (0) root         (0)     2978 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/tsp.py
--rw-r--r--   0 root         (0) root         (0)     1497 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/delivery/urls.py
--rwxr-xr-x   0 root         (0) root         (0)    70753 2021-03-12 20:47:33.000000 souschef-1.3.4/souschef/delivery/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:40.000000 souschef-1.3.4/souschef/frontend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/frontend/images/
--rw-r--r--   0 root         (0) root         (0)   292180 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/frontend/images/bg1.jpg
--rw-r--r--   0 root         (0) root         (0)    21988 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/frontend/images/jenny.jpg
--rw-r--r--   0 root         (0) root         (0)    28209 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/frontend/images/joe.jpg
--rw-r--r--   0 root         (0) root         (0)    23839 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/frontend/images/katrina.jpg
--rwxr-xr-x   0 root         (0) root         (0)      261 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/meal/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3639 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/apps.py
--rw-r--r--   0 root         (0) root         (0)     2290 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/meal/migrations/
--rw-r--r--   0 root         (0) root         (0)     4610 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/0002_ingredient_ingredient_group.py
--rw-r--r--   0 root         (0) root         (0)      857 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/0003_fix224a.py
--rw-r--r--   0 root         (0) root         (0)      475 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/0004_fix004d.py
--rw-r--r--   0 root         (0) root         (0)     1601 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/0005_fix241b.py
--rw-r--r--   0 root         (0) root         (0)      688 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/0006_auto_20160826_0007.py
--rw-r--r--   0 root         (0) root         (0)     1055 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/0007_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)      714 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/0008_auto_20180704_1613.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8381 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/models.py
--rw-r--r--   0 root         (0) root         (0)      200 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/settings.py
--rw-r--r--   0 root         (0) root         (0)     8022 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/tests.py
--rw-r--r--   0 root         (0) root         (0)       70 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/urls.py
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/meal/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2375 2021-03-05 21:55:29.000000 souschef-1.3.4/souschef/member/admin.py
--rw-r--r--   0 root         (0) root         (0)      122 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/apps.py
--rw-r--r--   0 root         (0) root         (0)     4590 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/factories.py
--rw-r--r--   0 root         (0) root         (0)    21109 2021-03-12 15:24:10.000000 souschef-1.3.4/souschef/member/forms.py
--rw-r--r--   0 root         (0) root         (0)      294 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/formsets.py
--rw-r--r--   0 root         (0) root         (0)     1073 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/formsfield.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:56.000000 souschef-1.3.4/souschef/member/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:35:45.000000 souschef-1.3.4/souschef/member/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      607 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/management/commands/createclients.py
--rw-r--r--   0 root         (0) root         (0)      406 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/management/commands/createnotes.py
--rw-r--r--   0 root         (0) root         (0)     1643 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/management/commands/processscheduledstatuschange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/migrations/
--rw-r--r--   0 root         (0) root         (0)     9199 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      559 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0002_auto_20160605_1609.py
--rw-r--r--   0 root         (0) root         (0)     1536 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0003_auto_20160615_2100.py
--rw-r--r--   0 root         (0) root         (0)     3288 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0004_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      565 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0005_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      479 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0006_client_meal_default_week.py
--rw-r--r--   0 root         (0) root         (0)      883 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0007_auto_20160726_1703.py
--rw-r--r--   0 root         (0) root         (0)      565 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0008_auto_20160727_2251.py
--rw-r--r--   0 root         (0) root         (0)      888 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0009_auto_20160728_1443.py
--rw-r--r--   0 root         (0) root         (0)      558 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0010_auto_20160803_2052.py
--rw-r--r--   0 root         (0) root         (0)      492 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0011_client_delivery_note.py
--rw-r--r--   0 root         (0) root         (0)     1788 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0012_clientscheduledstatus.py
--rw-r--r--   0 root         (0) root         (0)      756 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0013_auto_20160820_2322.py
--rw-r--r--   0 root         (0) root         (0)     1606 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0014_auto_20160826_0007.py
--rw-r--r--   0 root         (0) root         (0)      490 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0015_route_client_id_sequence.py
--rw-r--r--   0 root         (0) root         (0)      533 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0016_auto_20160912_1509.py
--rw-r--r--   0 root         (0) root         (0)      640 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0017_auto_20161020_2039.py
--rw-r--r--   0 root         (0) root         (0)      543 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0018_auto_20161110_2352.py
--rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0019_auto_20161111_1750.py
--rw-r--r--   0 root         (0) root         (0)      456 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0020_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)      481 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0021_auto_20161125_2055.py
--rw-r--r--   0 root         (0) root         (0)      592 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0022_auto_20161215_1936.py
--rw-r--r--   0 root         (0) root         (0)      885 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0023_auto_20161220_1401.py
--rw-r--r--   0 root         (0) root         (0)     2661 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0024_auto_20161227_1819.py
--rw-r--r--   0 root         (0) root         (0)      579 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0025_route_vehicle.py
--rw-r--r--   0 root         (0) root         (0)     3345 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0026_change_to_emergency_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1121 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0027_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)     1883 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py
--rw-r--r--   0 root         (0) root         (0)     1742 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0029_member_address_fk_to_1to1.py
--rw-r--r--   0 root         (0) root         (0)     1913 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0030_route_deliveryhistory.py
--rw-r--r--   0 root         (0) root         (0)      801 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0031_client_option_allow_reverse_relation.py
--rw-r--r--   0 root         (0) root         (0)     6237 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0032_relationship.py
--rw-r--r--   0 root         (0) root         (0)      828 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0033_auto_20170801_1607.py
--rw-r--r--   0 root         (0) root         (0)      619 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/0034_auto_20170816_0850.py
--rw-r--r--   0 root         (0) root         (0)      677 2021-02-12 02:15:29.000000 souschef-1.3.4/souschef/member/migrations/0035_auto_20210115_1155.py
--rw-r--r--   0 root         (0) root         (0)     1134 2021-03-02 23:43:41.000000 souschef-1.3.4/souschef/member/migrations/0036_member_addresses.py
--rw-r--r--   0 root         (0) root         (0)      574 2021-03-05 16:07:55.000000 souschef-1.3.4/souschef/member/migrations/0037_one_address_per_member.py
--rw-r--r--   0 root         (0) root         (0)      666 2021-03-05 16:07:55.000000 souschef-1.3.4/souschef/member/migrations/0038_member_verbose_names.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29003 2021-03-12 20:47:33.000000 souschef-1.3.4/souschef/member/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/signals/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/signals/__init__.py
--rw-r--r--   0 root         (0) root         (0)      400 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/signals/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:40.000000 souschef-1.3.4/souschef/member/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/templates/client/
--rw-r--r--   0 root         (0) root         (0)     3988 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/templates/client/create/
--rw-r--r--   0 root         (0) root         (0)     3868 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/create/form.html
--rw-r--r--   0 root         (0) root         (0)     1038 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/create/steps.html
--rw-r--r--   0 root         (0) root         (0)     5918 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/templates/client/partials/
--rw-r--r--   0 root         (0) root         (0)     1030 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/birthdays.html
--rw-r--r--   0 root         (0) root         (0)     1391 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/filters.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/templates/client/partials/forms/
--rw-r--r--   0 root         (0) root         (0)     2386 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/forms/address_information.html
--rw-r--r--   0 root         (0) root         (0)     2100 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/forms/basic_information.html
--rw-r--r--   0 root         (0) root         (0)     1467 2021-03-12 15:24:10.000000 souschef-1.3.4/souschef/member/templates/client/partials/forms/dietary_restriction.html
--rw-r--r--   0 root         (0) root         (0)     1293 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/forms/meal_defaults.html
--rw-r--r--   0 root         (0) root         (0)     2480 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/forms/payment_information.html
--rw-r--r--   0 root         (0) root         (0)     4373 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/forms/relationship_form.html
--rw-r--r--   0 root         (0) root         (0)      549 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/forms/relationships.html
--rw-r--r--   0 root         (0) root         (0)     1386 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/partials/menu.html
--rw-r--r--   0 root         (0) root         (0)     2017 2021-03-12 20:47:33.000000 souschef-1.3.4/souschef/member/templates/client/partials/order_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/templates/client/update/
--rw-r--r--   0 root         (0) root         (0)     3033 2021-03-12 15:24:10.000000 souschef-1.3.4/souschef/member/templates/client/update/base.html
--rw-r--r--   0 root         (0) root         (0)     2153 2021-03-12 20:47:33.000000 souschef-1.3.4/souschef/member/templates/client/update/status.html
--rw-r--r--   0 root         (0) root         (0)      291 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/update/step.html
--rw-r--r--   0 root         (0) root         (0)      149 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/update/steps.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/templates/client/view/
--rw-r--r--   0 root         (0) root         (0)      188 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/address.html
--rw-r--r--   0 root         (0) root         (0)     4633 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/allergies.html
--rw-r--r--   0 root         (0) root         (0)     1731 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/delete_status_confirmation.html
--rw-r--r--   0 root         (0) root         (0)     4471 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/information.html
--rw-r--r--   0 root         (0) root         (0)     2716 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/notes.html
--rw-r--r--   0 root         (0) root         (0)      637 2021-03-05 21:39:33.000000 souschef-1.3.4/souschef/member/templates/client/view/orders.html
--rw-r--r--   0 root         (0) root         (0)     1825 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/payment.html
--rw-r--r--   0 root         (0) root         (0)     1649 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/referent.html
--rw-r--r--   0 root         (0) root         (0)     2204 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/status.html
--rw-r--r--   0 root         (0) root         (0)     1622 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/client/view/summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/member/templates/route/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/route/delivered_route_detail.html
--rw-r--r--   0 root         (0) root         (0)     5832 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/route/delivery_history_detail.html
--rw-r--r--   0 root         (0) root         (0)     6159 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/route/detail.html
--rw-r--r--   0 root         (0) root         (0)     9150 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/route/edit.html
--rw-r--r--   0 root         (0) root         (0)     1875 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/templates/route/list.html
--rw-r--r--   0 root         (0) root         (0)   164454 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/tests.py
--rw-r--r--   0 root         (0) root         (0)     5326 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/member/urls.py
--rw-r--r--   0 root         (0) root         (0)    56544 2021-03-12 20:47:33.000000 souschef-1.3.4/souschef/member/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:42.000000 souschef-1.3.4/souschef/note/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/__init__.py
--rw-r--r--   0 root         (0) root         (0)      185 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/apps.py
--rw-r--r--   0 root         (0) root         (0)      781 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/factories.py
--rw-r--r--   0 root         (0) root         (0)      916 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/note/migrations/
--rw-r--r--   0 root         (0) root         (0)     1526 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      593 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0002_auto_20160818_2104.py
--rw-r--r--   0 root         (0) root         (0)      516 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0003_auto_20160819_2037.py
--rw-r--r--   0 root         (0) root         (0)     1006 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0004_notepriority.py
--rw-r--r--   0 root         (0) root         (0)     1256 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0005_note_priority_old_data_migration.py
--rw-r--r--   0 root         (0) root         (0)      546 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0006_change_priority_field.py
--rw-r--r--   0 root         (0) root         (0)     1323 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0007_notecategory.py
--rw-r--r--   0 root         (0) root         (0)     1009 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0008_auto_20170116_1441.py
--rw-r--r--   0 root         (0) root         (0)      836 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0009_auto_20170116_1543.py
--rw-r--r--   0 root         (0) root         (0)     1147 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0010_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)      862 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/0011_auto_20170419_1109.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3569 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/note/templates/
--rw-r--r--   0 root         (0) root         (0)     2186 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/templates/notes_add.html
--rw-r--r--   0 root         (0) root         (0)     4080 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/templates/notes_client_list.html
--rw-r--r--   0 root         (0) root         (0)     5732 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/templates/notes_list.html
--rw-r--r--   0 root         (0) root         (0)     9140 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/tests.py
--rw-r--r--   0 root         (0) root         (0)      609 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/urls.py
--rw-r--r--   0 root         (0) root         (0)     4803 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/note/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)      122 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/admin.py
--rw-r--r--   0 root         (0) root         (0)       99 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/notification/migrations/
--rw-r--r--   0 root         (0) root         (0)      980 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      606 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/models.py
--rw-r--r--   0 root         (0) root         (0)       61 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/tests.py
--rw-r--r--   0 root         (0) root         (0)       78 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/urls.py
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/notification/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/order/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1081 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/admin.py
--rw-r--r--   0 root         (0) root         (0)       85 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/apps.py
--rw-r--r--   0 root         (0) root         (0)     1536 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/factories.py
--rw-r--r--   0 root         (0) root         (0)     5536 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/order/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:21:15.000000 souschef-1.3.4/souschef/order/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/order/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:52.000000 souschef-1.3.4/souschef/order/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      445 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/management/commands/createorders.py
--rw-r--r--   0 root         (0) root         (0)     1769 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/management/commands/generateorders.py
--rw-r--r--   0 root         (0) root         (0)     1338 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/management/commands/setordersdelivered.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/order/migrations/
--rw-r--r--   0 root         (0) root         (0)     2602 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      567 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0002_auto_20160614_1736.py
--rw-r--r--   0 root         (0) root         (0)      583 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0003_auto_20160615_1504.py
--rw-r--r--   0 root         (0) root         (0)      939 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0004_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      700 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0005_fix241b.py
--rw-r--r--   0 root         (0) root         (0)      564 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0006_auto_20160803_2217.py
--rw-r--r--   0 root         (0) root         (0)      396 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0007_remove_order_item_component.py
--rw-r--r--   0 root         (0) root         (0)      603 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0008_auto_20160912_1509.py
--rw-r--r--   0 root         (0) root         (0)      799 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0009_auto_20161012_1919.py
--rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0010_auto_20161012_1921.py
--rw-r--r--   0 root         (0) root         (0)     1854 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0011_auto_20161014_1901.py
--rw-r--r--   0 root         (0) root         (0)      448 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0012_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)     1309 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0013_orderstatuschange.py
--rw-r--r--   0 root         (0) root         (0)     1007 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0014_auto_20161209_2045.py
--rw-r--r--   0 root         (0) root         (0)      548 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0015_auto_20170410_1029.py
--rw-r--r--   0 root         (0) root         (0)      739 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/0016_auto_20180704_1613.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1388 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/mixins.py
--rw-r--r--   0 root         (0) root         (0)    46177 2021-03-12 15:24:10.000000 souschef-1.3.4/souschef/order/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/order/templates/
--rw-r--r--   0 root         (0) root         (0)     5283 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/_form.html
--rw-r--r--   0 root         (0) root         (0)     1098 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/_order_info.html
--rw-r--r--   0 root         (0) root         (0)       92 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/base_order.html
--rw-r--r--   0 root         (0) root         (0)     1227 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/create.html
--rw-r--r--   0 root         (0) root         (0)     3647 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/order/templates/order/
--rw-r--r--   0 root         (0) root         (0)     9056 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/order/create_batch.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/order/templates/order/partials/
--rw-r--r--   0 root         (0) root         (0)     1308 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/order/partials/filters.html
--rw-r--r--   0 root         (0) root         (0)      801 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/order_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     2315 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/order_update_status.html
--rw-r--r--   0 root         (0) root         (0)     2023 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/update.html
--rw-r--r--   0 root         (0) root         (0)     3097 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/templates/view.html
--rw-r--r--   0 root         (0) root         (0)    65628 2020-12-18 17:45:24.000000 souschef-1.3.4/souschef/order/tests.py
--rw-r--r--   0 root         (0) root         (0)     1062 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/order/urls.py
--rw-r--r--   0 root         (0) root         (0)    14232 2020-12-18 18:15:58.000000 souschef-1.3.4/souschef/order/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/page/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/__init__.py
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/admin.py
--rw-r--r--   0 root         (0) root         (0)      124 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/page/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:40.000000 souschef-1.3.4/souschef/page/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/page/templates/pages/
--rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/templates/pages/card.html
--rw-r--r--   0 root         (0) root         (0)     7007 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/templates/pages/home.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/page/templates/registration/
--rw-r--r--   0 root         (0) root         (0)     1634 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/templates/registration/login.html
--rw-r--r--   0 root         (0) root         (0)    10266 2020-12-18 17:45:24.000000 souschef-1.3.4/souschef/page/tests.py
--rw-r--r--   0 root         (0) root         (0)      508 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/page/urls.py
--rw-r--r--   0 root         (0) root         (0)     4507 2020-12-11 20:17:31.000000 souschef-1.3.4/souschef/page/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/pycrons/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-12 02:23:19.000000 souschef-1.3.4/souschef/pycrons/__init__.py
--rw-r--r--   0 root         (0) root         (0)      429 2021-02-12 02:23:19.000000 souschef-1.3.4/souschef/pycrons/cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/sous_chef/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef/sous_chef/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:43.000000 souschef-1.3.4/souschef/sous_chef/assets/css/
--rw-r--r--   0 root         (0) root         (0)   654912 2021-03-12 20:48:32.000000 souschef-1.3.4/souschef/sous_chef/assets/css/main.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/
--rw-r--r--   0 root         (0) root         (0)    98640 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.eot
--rw-r--r--   0 root         (0) root         (0)   507628 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.svg
--rw-r--r--   0 root         (0) root         (0)    98404 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    63728 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.woff
--rw-r--r--   0 root         (0) root         (0)    54488 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.woff2
--rw-r--r--   0 root         (0) root         (0)   106004 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.eot
--rw-r--r--   0 root         (0) root         (0)    93888 2021-03-12 20:48:28.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.otf
--rw-r--r--   0 root         (0) root         (0)   390837 2021-03-12 20:48:28.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.svg
--rw-r--r--   0 root         (0) root         (0)   105784 2021-03-12 20:48:32.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.ttf
--rw-r--r--   0 root         (0) root         (0)    50524 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.woff
--rw-r--r--   0 root         (0) root         (0)    40148 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.woff2
--rw-r--r--   0 root         (0) root         (0)    31156 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.eot
--rw-r--r--   0 root         (0) root         (0)   107201 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.svg
--rw-r--r--   0 root         (0) root         (0)    30928 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    14712 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.woff
--rw-r--r--   0 root         (0) root         (0)    12240 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/assets/images/
--rw-r--r--   0 root         (0) root         (0)   258972 2021-03-12 20:48:35.000000 souschef-1.3.4/souschef/sous_chef/assets/images/bg1.jpg
--rw-r--r--   0 root         (0) root         (0)    11449 2021-03-12 20:48:35.000000 souschef-1.3.4/souschef/sous_chef/assets/images/demo.png
--rw-r--r--   0 root         (0) root         (0)      608 2021-03-12 20:48:36.000000 souschef-1.3.4/souschef/sous_chef/assets/images/favicon.png
--rw-r--r--   0 root         (0) root         (0)    28123 2021-03-12 20:48:28.000000 souschef-1.3.4/souschef/sous_chef/assets/images/flags.png
--rw-r--r--   0 root         (0) root         (0)      490 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/geocoder.png
--rw-r--r--   0 root         (0) root         (0)     1374 2021-03-12 20:48:35.000000 souschef-1.3.4/souschef/sous_chef/assets/images/glyph-marker-icon.png
--rw-r--r--   0 root         (0) root         (0)     1287 2021-03-12 20:48:35.000000 souschef-1.3.4/souschef/sous_chef/assets/images/glyph-marker-icon.svg
--rw-r--r--   0 root         (0) root         (0)    21977 2021-03-12 20:48:36.000000 souschef-1.3.4/souschef/sous_chef/assets/images/jenny.jpg
--rw-r--r--   0 root         (0) root         (0)    26952 2021-03-12 20:48:36.000000 souschef-1.3.4/souschef/sous_chef/assets/images/joe.jpg
--rw-r--r--   0 root         (0) root         (0)    23839 2021-03-12 20:48:36.000000 souschef-1.3.4/souschef/sous_chef/assets/images/katrina.jpg
--rw-r--r--   0 root         (0) root         (0)     2306 2021-03-12 20:48:32.000000 souschef-1.3.4/souschef/sous_chef/assets/images/leaflet.routing.icons.png
--rw-r--r--   0 root         (0) root         (0)     4060 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/leaflet.routing.icons.svg
--rw-r--r--   0 root         (0) root         (0)     6363 2021-03-12 20:48:36.000000 souschef-1.3.4/souschef/sous_chef/assets/images/logo-souschef-coul.png
--rw-r--r--   0 root         (0) root         (0)     6033 2021-03-12 20:48:36.000000 souschef-1.3.4/souschef/sous_chef/assets/images/logo-souschef-nb.png
--rw-r--r--   0 root         (0) root         (0)      891 2021-03-12 20:48:36.000000 souschef-1.3.4/souschef/sous_chef/assets/images/logo.png
--rw-r--r--   0 root         (0) root         (0)    14323 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/markers-matte.png
--rw-r--r--   0 root         (0) root         (0)    30194 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/markers-matte@2x.png
--rw-r--r--   0 root         (0) root         (0)     7946 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/markers-plain.png
--rw-r--r--   0 root         (0) root         (0)      535 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/markers-shadow.png
--rw-r--r--   0 root         (0) root         (0)     1134 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/markers-shadow@2x.png
--rw-r--r--   0 root         (0) root         (0)    36367 2021-03-12 20:48:34.000000 souschef-1.3.4/souschef/sous_chef/assets/images/markers-soft.png
--rw-r--r--   0 root         (0) root         (0)   146362 2021-03-12 20:48:35.000000 souschef-1.3.4/souschef/sous_chef/assets/images/markers-soft@2x.png
--rw-r--r--   0 root         (0) root         (0)      454 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/routing-icon.png
--rw-r--r--   0 root         (0) root         (0)     4831 2021-03-12 20:48:33.000000 souschef-1.3.4/souschef/sous_chef/assets/images/throbber.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/assets/js/
--rw-r--r--   0 root         (0) root         (0)  1031323 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/js/leaflet.js
--rw-r--r--   0 root         (0) root         (0)   627692 2021-03-12 20:48:28.000000 souschef-1.3.4/souschef/sous_chef/assets/js/leaflet.min.js
--rw-r--r--   0 root         (0) root         (0)    22295 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/js/multidatespicker.js
--rw-r--r--   0 root         (0) root         (0)    10453 2021-03-12 20:48:25.000000 souschef-1.3.4/souschef/sous_chef/assets/js/multidatespicker.min.js
--rw-r--r--   0 root         (0) root         (0)  1110220 2021-03-12 20:48:28.000000 souschef-1.3.4/souschef/sous_chef/assets/js/sous-chef.js
--rw-r--r--   0 root         (0) root         (0)   398649 2021-03-12 20:48:31.000000 souschef-1.3.4/souschef/sous_chef/assets/js/sous-chef.min.js
--rw-r--r--   0 root         (0) root         (0)     1436 2020-12-18 20:03:32.000000 souschef-1.3.4/souschef/sous_chef/context_processors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/formats/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/formats/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/formats/en/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/formats/en/__init__.py
--rw-r--r--   0 root         (0) root         (0)      186 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/formats/en/formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/formats/fr/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/formats/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/formats/fr/formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/management/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/management/commands/makemessages.py
--rw-r--r--   0 root         (0) root         (0)      536 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/rules.py
--rw-r--r--   0 root         (0) root         (0)     7517 2021-02-12 02:23:19.000000 souschef-1.3.4/souschef/sous_chef/settings.py
--rw-r--r--   0 root         (0) root         (0)      227 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/settings_test.py
--rw-r--r--   0 root         (0) root         (0)       59 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/settings_test_fr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/templates/
--rw-r--r--   0 root         (0) root         (0)      611 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templates/404.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/templates/avatar/
--rw-r--r--   0 root         (0) root         (0)     1870 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templates/avatar/change.html
--rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templates/avatar/confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     3461 2021-01-15 15:45:00.000000 souschef-1.3.4/souschef/sous_chef/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/templates/dashboard/
--rw-r--r--   0 root         (0) root         (0)      771 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templates/dashboard/statistics.html
--rw-r--r--   0 root         (0) root         (0)     1271 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templates/splash.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/templates/system/
--rw-r--r--   0 root         (0) root         (0)      219 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templates/system/_button_export.html
--rw-r--r--   0 root         (0) root         (0)      209 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templates/system/breadcrumb.html
--rw-r--r--   0 root         (0) root         (0)     2905 2021-03-02 23:43:41.000000 souschef-1.3.4/souschef/sous_chef/templates/system/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:44.000000 souschef-1.3.4/souschef/sous_chef/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      319 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/templatetags/sous_chef_extras.py
--rw-r--r--   0 root         (0) root         (0)     3100 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/tests.py
--rw-r--r--   0 root         (0) root         (0)     2062 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/urls.py
--rw-r--r--   0 root         (0) root         (0)      395 2020-11-06 14:25:57.000000 souschef-1.3.4/souschef/sous_chef/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-12 20:48:41.000000 souschef-1.3.4/souschef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2522 2021-03-12 20:48:39.000000 souschef-1.3.4/souschef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15173 2021-03-12 20:48:40.000000 souschef-1.3.4/souschef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-12 20:48:39.000000 souschef-1.3.4/souschef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      462 2021-03-12 20:48:39.000000 souschef-1.3.4/souschef.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-03-12 20:48:39.000000 souschef-1.3.4/souschef.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)     5729 2021-03-02 23:43:41.000000 souschef-1.3.5/INSTALL.md
+-rw-r--r--   0 root         (0) root         (0)    33893 2020-11-20 01:08:04.000000 souschef-1.3.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      230 2021-01-23 15:51:37.000000 souschef-1.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2522 2021-04-02 20:32:13.000000 souschef-1.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1366 2021-01-22 18:52:15.000000 souschef-1.3.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1409 2021-01-23 16:03:53.000000 souschef-1.3.5/UPDATE.md
+-rw-r--r--   0 root         (0) root         (0)      114 2021-04-02 20:32:13.000000 souschef-1.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1781 2021-04-02 20:30:51.000000 souschef-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:09.000000 souschef-1.3.5/souschef/
+-rw-r--r--   0 root         (0) root         (0)    32621 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      314 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/admin.py
+-rw-r--r--   0 root         (0) root         (0)       89 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/apps.py
+-rw-r--r--   0 root         (0) root         (0)      358 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/billing/migrations/
+-rw-r--r--   0 root         (0) root         (0)      983 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      494 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/migrations/0002_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)      435 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/migrations/0003_auto_20161122_0515.py
+-rw-r--r--   0 root         (0) root         (0)      439 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/migrations/0004_auto_20201030_1540.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/billing/templates/
+-rw-r--r--   0 root         (0) root         (0)       42 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/templates/base_billing.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/billing/templates/billing/
+-rw-r--r--   0 root         (0) root         (0)     4897 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/templates/billing/add.html
+-rw-r--r--   0 root         (0) root         (0)      863 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/templates/billing/billing_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     3310 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/templates/billing/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/billing/templates/billing/partials/
+-rw-r--r--   0 root         (0) root         (0)      531 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/templates/billing/partials/statistics.html
+-rw-r--r--   0 root         (0) root         (0)     5148 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/templates/billing/partials/summary.html
+-rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/templates/billing/print_summary.html
+-rw-r--r--   0 root         (0) root         (0)      822 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/templates/billing/view.html
+-rw-r--r--   0 root         (0) root         (0)     3407 2021-03-19 15:14:11.000000 souschef-1.3.5/souschef/billing/templates/billing/view_orders.html
+-rw-r--r--   0 root         (0) root         (0)     8493 2020-12-19 18:25:21.000000 souschef-1.3.5/souschef/billing/tests.py
+-rw-r--r--   0 root         (0) root         (0)      718 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/urls.py
+-rw-r--r--   0 root         (0) root         (0)    11692 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/billing/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/configsamples/
+-rw-r--r--   0 root         (0) root         (0)      809 2021-03-02 23:43:41.000000 souschef-1.3.5/souschef/configsamples/nginx.conf
+-rw-r--r--   0 root         (0) root         (0)      409 2020-12-19 18:25:21.000000 souschef-1.3.5/souschef/configsamples/souschef.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/cronscripts/
+-rwxr-xr-x   0 root         (0) root         (0)      469 2021-01-23 16:08:34.000000 souschef-1.3.5/souschef/cronscripts/souschef_daily.sh
+-rw-r--r--   0 root         (0) root         (0)      361 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/dataexec.py
+-rw-r--r--   0 root         (0) root         (0)    81444 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/dataload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/datamigration/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/admin.py
+-rw-r--r--   0 root         (0) root         (0)      101 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/datamigration/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:34.000000 souschef-1.3.5/souschef/datamigration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/datamigration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:11.000000 souschef-1.3.5/souschef/datamigration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/management/commands/importaddresses.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/management/commands/importclients.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/management/commands/importcontactaddresses.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/management/commands/importmeals.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/management/commands/importorders.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/management/commands/importrelationships.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/datamigration/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       58 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/models.py
+-rw-r--r--   0 root         (0) root         (0)     9202 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/tests.py
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/datamigration/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/delivery/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/admin.py
+-rwxr-xr-x   0 root         (0) root         (0)       91 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/apps.py
+-rw-r--r--   0 root         (0) root         (0)      906 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2021-03-19 15:07:36.000000 souschef-1.3.5/souschef/delivery/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/delivery/migrations/
+-rw-r--r--   0 root         (0) root         (0)      582 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/migrations/0001_fix004a.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/migrations/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      218 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/delivery/templates/
+-rw-r--r--   0 root         (0) root         (0)    12093 2021-03-19 19:46:01.000000 souschef-1.3.5/souschef/delivery/templates/edit_delivery_of_today.html
+-rw-r--r--   0 root         (0) root         (0)     3511 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/templates/ingredients.html
+-rw-r--r--   0 root         (0) root         (0)     4057 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/templates/kitchen_count.html
+-rw-r--r--   0 root         (0) root         (0)     1183 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/templates/kitchen_count_steps.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/delivery/templates/partials/
+-rw-r--r--   0 root         (0) root         (0)     2622 2021-03-20 15:32:41.000000 souschef-1.3.5/souschef/delivery/templates/partials/generated_orders.html
+-rw-r--r--   0 root         (0) root         (0)     1737 2021-03-19 19:57:48.000000 souschef-1.3.5/souschef/delivery/templates/partials/generated_orders_order_row_content.html
+-rw-r--r--   0 root         (0) root         (0)     1085 2021-03-19 15:56:24.000000 souschef-1.3.5/souschef/delivery/templates/partials/generated_orders_table_head.html
+-rw-r--r--   0 root         (0) root         (0)     4403 2021-03-20 15:19:06.000000 souschef-1.3.5/souschef/delivery/templates/review_orders.html
+-rw-r--r--   0 root         (0) root         (0)     3362 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/templates/route_sheet.html
+-rw-r--r--   0 root         (0) root         (0)     4993 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/templates/routes.html
+-rwxr-xr-x   0 root         (0) root         (0)    47234 2020-12-19 16:05:35.000000 souschef-1.3.5/souschef/delivery/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/tsp.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/delivery/urls.py
+-rwxr-xr-x   0 root         (0) root         (0)    71958 2021-03-20 15:14:08.000000 souschef-1.3.5/souschef/delivery/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:09.000000 souschef-1.3.5/souschef/frontend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/frontend/images/
+-rw-r--r--   0 root         (0) root         (0)   292180 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/frontend/images/bg1.jpg
+-rw-r--r--   0 root         (0) root         (0)    21988 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/frontend/images/jenny.jpg
+-rw-r--r--   0 root         (0) root         (0)    28209 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/frontend/images/joe.jpg
+-rw-r--r--   0 root         (0) root         (0)    23839 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/frontend/images/katrina.jpg
+-rwxr-xr-x   0 root         (0) root         (0)      261 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/meal/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/meal/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4610 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/0002_ingredient_ingredient_group.py
+-rw-r--r--   0 root         (0) root         (0)      857 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/0003_fix224a.py
+-rw-r--r--   0 root         (0) root         (0)      475 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/0004_fix004d.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/0005_fix241b.py
+-rw-r--r--   0 root         (0) root         (0)      688 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/0006_auto_20160826_0007.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/0007_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)      714 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/0008_auto_20180704_1613.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8381 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/models.py
+-rw-r--r--   0 root         (0) root         (0)      200 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/settings.py
+-rw-r--r--   0 root         (0) root         (0)     8022 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/tests.py
+-rw-r--r--   0 root         (0) root         (0)       70 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/urls.py
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/meal/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef/member/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2021-03-05 21:55:29.000000 souschef-1.3.5/souschef/member/admin.py
+-rw-r--r--   0 root         (0) root         (0)      122 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/apps.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/factories.py
+-rw-r--r--   0 root         (0) root         (0)    21109 2021-03-12 15:24:10.000000 souschef-1.3.5/souschef/member/forms.py
+-rw-r--r--   0 root         (0) root         (0)      294 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/formsets.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/formsfield.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:56.000000 souschef-1.3.5/souschef/member/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:35:45.000000 souschef-1.3.5/souschef/member/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      607 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/management/commands/createclients.py
+-rw-r--r--   0 root         (0) root         (0)      406 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/management/commands/createnotes.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/management/commands/processscheduledstatuschange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/migrations/
+-rw-r--r--   0 root         (0) root         (0)     9199 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      559 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0002_auto_20160605_1609.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0003_auto_20160615_2100.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0004_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      565 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0005_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      479 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0006_client_meal_default_week.py
+-rw-r--r--   0 root         (0) root         (0)      883 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0007_auto_20160726_1703.py
+-rw-r--r--   0 root         (0) root         (0)      565 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0008_auto_20160727_2251.py
+-rw-r--r--   0 root         (0) root         (0)      888 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0009_auto_20160728_1443.py
+-rw-r--r--   0 root         (0) root         (0)      558 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0010_auto_20160803_2052.py
+-rw-r--r--   0 root         (0) root         (0)      492 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0011_client_delivery_note.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0012_clientscheduledstatus.py
+-rw-r--r--   0 root         (0) root         (0)      756 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0013_auto_20160820_2322.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0014_auto_20160826_0007.py
+-rw-r--r--   0 root         (0) root         (0)      490 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0015_route_client_id_sequence.py
+-rw-r--r--   0 root         (0) root         (0)      533 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0016_auto_20160912_1509.py
+-rw-r--r--   0 root         (0) root         (0)      640 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0017_auto_20161020_2039.py
+-rw-r--r--   0 root         (0) root         (0)      543 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0018_auto_20161110_2352.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0019_auto_20161111_1750.py
+-rw-r--r--   0 root         (0) root         (0)      456 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0020_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)      481 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0021_auto_20161125_2055.py
+-rw-r--r--   0 root         (0) root         (0)      592 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0022_auto_20161215_1936.py
+-rw-r--r--   0 root         (0) root         (0)      885 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0023_auto_20161220_1401.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0024_auto_20161227_1819.py
+-rw-r--r--   0 root         (0) root         (0)      579 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0025_route_vehicle.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0026_change_to_emergency_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0027_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0029_member_address_fk_to_1to1.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0030_route_deliveryhistory.py
+-rw-r--r--   0 root         (0) root         (0)      801 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0031_client_option_allow_reverse_relation.py
+-rw-r--r--   0 root         (0) root         (0)     6237 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0032_relationship.py
+-rw-r--r--   0 root         (0) root         (0)      828 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0033_auto_20170801_1607.py
+-rw-r--r--   0 root         (0) root         (0)      619 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/0034_auto_20170816_0850.py
+-rw-r--r--   0 root         (0) root         (0)      677 2021-02-12 02:15:29.000000 souschef-1.3.5/souschef/member/migrations/0035_auto_20210115_1155.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2021-03-02 23:43:41.000000 souschef-1.3.5/souschef/member/migrations/0036_member_addresses.py
+-rw-r--r--   0 root         (0) root         (0)      574 2021-03-05 16:07:55.000000 souschef-1.3.5/souschef/member/migrations/0037_one_address_per_member.py
+-rw-r--r--   0 root         (0) root         (0)      666 2021-03-05 16:07:55.000000 souschef-1.3.5/souschef/member/migrations/0038_member_verbose_names.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29546 2021-03-19 20:02:11.000000 souschef-1.3.5/souschef/member/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/signals/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/signals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      400 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/signals/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:09.000000 souschef-1.3.5/souschef/member/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/templates/client/
+-rw-r--r--   0 root         (0) root         (0)     3988 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/templates/client/create/
+-rw-r--r--   0 root         (0) root         (0)     3868 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/create/form.html
+-rw-r--r--   0 root         (0) root         (0)     1038 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/create/steps.html
+-rw-r--r--   0 root         (0) root         (0)     5918 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/templates/client/partials/
+-rw-r--r--   0 root         (0) root         (0)     1030 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/birthdays.html
+-rw-r--r--   0 root         (0) root         (0)     1391 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/filters.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/templates/client/partials/forms/
+-rw-r--r--   0 root         (0) root         (0)     2386 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/forms/address_information.html
+-rw-r--r--   0 root         (0) root         (0)     2100 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/forms/basic_information.html
+-rw-r--r--   0 root         (0) root         (0)     1467 2021-03-12 15:24:10.000000 souschef-1.3.5/souschef/member/templates/client/partials/forms/dietary_restriction.html
+-rw-r--r--   0 root         (0) root         (0)     1293 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/forms/meal_defaults.html
+-rw-r--r--   0 root         (0) root         (0)     2480 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/forms/payment_information.html
+-rw-r--r--   0 root         (0) root         (0)     4373 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/forms/relationship_form.html
+-rw-r--r--   0 root         (0) root         (0)      549 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/forms/relationships.html
+-rw-r--r--   0 root         (0) root         (0)     1386 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/partials/menu.html
+-rw-r--r--   0 root         (0) root         (0)     2017 2021-03-12 21:55:40.000000 souschef-1.3.5/souschef/member/templates/client/partials/order_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/templates/client/update/
+-rw-r--r--   0 root         (0) root         (0)     3033 2021-03-12 15:24:10.000000 souschef-1.3.5/souschef/member/templates/client/update/base.html
+-rw-r--r--   0 root         (0) root         (0)     2153 2021-03-12 21:55:40.000000 souschef-1.3.5/souschef/member/templates/client/update/status.html
+-rw-r--r--   0 root         (0) root         (0)      291 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/update/step.html
+-rw-r--r--   0 root         (0) root         (0)      149 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/update/steps.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/templates/client/view/
+-rw-r--r--   0 root         (0) root         (0)      188 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/address.html
+-rw-r--r--   0 root         (0) root         (0)     4633 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/allergies.html
+-rw-r--r--   0 root         (0) root         (0)     1731 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/delete_status_confirmation.html
+-rw-r--r--   0 root         (0) root         (0)     4471 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/information.html
+-rw-r--r--   0 root         (0) root         (0)     2716 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/notes.html
+-rw-r--r--   0 root         (0) root         (0)      637 2021-03-05 21:39:33.000000 souschef-1.3.5/souschef/member/templates/client/view/orders.html
+-rw-r--r--   0 root         (0) root         (0)     1825 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/payment.html
+-rw-r--r--   0 root         (0) root         (0)     1649 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/referent.html
+-rw-r--r--   0 root         (0) root         (0)     2204 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/status.html
+-rw-r--r--   0 root         (0) root         (0)     1622 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/client/view/summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/member/templates/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/route/delivered_route_detail.html
+-rw-r--r--   0 root         (0) root         (0)     5832 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/route/delivery_history_detail.html
+-rw-r--r--   0 root         (0) root         (0)     6159 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/route/detail.html
+-rw-r--r--   0 root         (0) root         (0)     9150 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/route/edit.html
+-rw-r--r--   0 root         (0) root         (0)     1875 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/templates/route/list.html
+-rw-r--r--   0 root         (0) root         (0)   164454 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/tests.py
+-rw-r--r--   0 root         (0) root         (0)     5326 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/member/urls.py
+-rw-r--r--   0 root         (0) root         (0)    56544 2021-03-12 21:55:40.000000 souschef-1.3.5/souschef/member/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:11.000000 souschef-1.3.5/souschef/note/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      185 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/apps.py
+-rw-r--r--   0 root         (0) root         (0)      781 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/factories.py
+-rw-r--r--   0 root         (0) root         (0)      916 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/note/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1526 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      593 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0002_auto_20160818_2104.py
+-rw-r--r--   0 root         (0) root         (0)      516 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0003_auto_20160819_2037.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0004_notepriority.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0005_note_priority_old_data_migration.py
+-rw-r--r--   0 root         (0) root         (0)      546 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0006_change_priority_field.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0007_notecategory.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0008_auto_20170116_1441.py
+-rw-r--r--   0 root         (0) root         (0)      836 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0009_auto_20170116_1543.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0010_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)      862 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/0011_auto_20170419_1109.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/note/templates/
+-rw-r--r--   0 root         (0) root         (0)     2186 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/templates/notes_add.html
+-rw-r--r--   0 root         (0) root         (0)     4080 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/templates/notes_client_list.html
+-rw-r--r--   0 root         (0) root         (0)     5732 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/templates/notes_list.html
+-rw-r--r--   0 root         (0) root         (0)     9140 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/tests.py
+-rw-r--r--   0 root         (0) root         (0)      609 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/urls.py
+-rw-r--r--   0 root         (0) root         (0)     4803 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/note/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      122 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/admin.py
+-rw-r--r--   0 root         (0) root         (0)       99 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/notification/migrations/
+-rw-r--r--   0 root         (0) root         (0)      980 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      606 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/models.py
+-rw-r--r--   0 root         (0) root         (0)       61 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/tests.py
+-rw-r--r--   0 root         (0) root         (0)       78 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/urls.py
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/notification/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/order/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/admin.py
+-rw-r--r--   0 root         (0) root         (0)       85 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/factories.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2021-04-02 19:08:09.000000 souschef-1.3.5/souschef/order/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/order/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:21:15.000000 souschef-1.3.5/souschef/order/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/order/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:52.000000 souschef-1.3.5/souschef/order/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      445 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/management/commands/createorders.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/management/commands/generateorders.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/management/commands/setordersdelivered.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/order/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2602 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      567 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0002_auto_20160614_1736.py
+-rw-r--r--   0 root         (0) root         (0)      583 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0003_auto_20160615_1504.py
+-rw-r--r--   0 root         (0) root         (0)      939 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0004_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      700 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0005_fix241b.py
+-rw-r--r--   0 root         (0) root         (0)      564 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0006_auto_20160803_2217.py
+-rw-r--r--   0 root         (0) root         (0)      396 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0007_remove_order_item_component.py
+-rw-r--r--   0 root         (0) root         (0)      603 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0008_auto_20160912_1509.py
+-rw-r--r--   0 root         (0) root         (0)      799 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0009_auto_20161012_1919.py
+-rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0010_auto_20161012_1921.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0011_auto_20161014_1901.py
+-rw-r--r--   0 root         (0) root         (0)      448 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0012_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0013_orderstatuschange.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0014_auto_20161209_2045.py
+-rw-r--r--   0 root         (0) root         (0)      548 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0015_auto_20170410_1029.py
+-rw-r--r--   0 root         (0) root         (0)      739 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/0016_auto_20180704_1613.py
+-rw-r--r--   0 root         (0) root         (0)      528 2021-04-02 19:33:53.000000 souschef-1.3.5/souschef/order/migrations/0017_total_quantity_not_nullable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    46640 2021-04-02 19:45:10.000000 souschef-1.3.5/souschef/order/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/order/templates/
+-rw-r--r--   0 root         (0) root         (0)     5283 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/templates/_form.html
+-rw-r--r--   0 root         (0) root         (0)     1098 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/templates/_order_info.html
+-rw-r--r--   0 root         (0) root         (0)       92 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/templates/base_order.html
+-rw-r--r--   0 root         (0) root         (0)     1227 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/templates/create.html
+-rw-r--r--   0 root         (0) root         (0)     4421 2021-03-26 14:22:55.000000 souschef-1.3.5/souschef/order/templates/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/order/templates/order/
+-rw-r--r--   0 root         (0) root         (0)     9056 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/templates/order/create_batch.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/order/templates/order/partials/
+-rw-r--r--   0 root         (0) root         (0)     1308 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/order/templates/order/partials/filters.html
+-rw-r--r--   0 root         (0) root         (0)       15 2021-03-26 16:39:12.000000 souschef-1.3.5/souschef/order/templates/order/partials/order_history.html
+-rw-r--r--   0 root         (0) root         (0)     1069 2021-03-19 18:13:43.000000 souschef-1.3.5/souschef/order/templates/order_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     2315 2021-03-26 15:05:24.000000 souschef-1.3.5/souschef/order/templates/order_update_status.html
+-rw-r--r--   0 root         (0) root         (0)     2023 2021-03-26 14:34:44.000000 souschef-1.3.5/souschef/order/templates/update.html
+-rw-r--r--   0 root         (0) root         (0)     3240 2021-04-02 19:14:01.000000 souschef-1.3.5/souschef/order/templates/view.html
+-rw-r--r--   0 root         (0) root         (0)    65866 2021-04-02 19:51:50.000000 souschef-1.3.5/souschef/order/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2021-03-19 18:05:32.000000 souschef-1.3.5/souschef/order/urls.py
+-rw-r--r--   0 root         (0) root         (0)    14673 2021-03-26 14:26:51.000000 souschef-1.3.5/souschef/order/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/page/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/admin.py
+-rw-r--r--   0 root         (0) root         (0)      124 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/page/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:09.000000 souschef-1.3.5/souschef/page/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/page/templates/pages/
+-rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/templates/pages/card.html
+-rw-r--r--   0 root         (0) root         (0)     7007 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/templates/pages/home.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/page/templates/registration/
+-rw-r--r--   0 root         (0) root         (0)     1634 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/templates/registration/login.html
+-rw-r--r--   0 root         (0) root         (0)    10266 2020-12-18 17:45:24.000000 souschef-1.3.5/souschef/page/tests.py
+-rw-r--r--   0 root         (0) root         (0)      508 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/page/urls.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2020-12-11 20:17:31.000000 souschef-1.3.5/souschef/page/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/pycrons/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-02-12 02:23:19.000000 souschef-1.3.5/souschef/pycrons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      429 2021-02-12 02:23:19.000000 souschef-1.3.5/souschef/pycrons/cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/sous_chef/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:09.000000 souschef-1.3.5/souschef/sous_chef/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:12.000000 souschef-1.3.5/souschef/sous_chef/assets/css/
+-rw-r--r--   0 root         (0) root         (0)   655022 2021-04-02 20:32:01.000000 souschef-1.3.5/souschef/sous_chef/assets/css/main.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/
+-rw-r--r--   0 root         (0) root         (0)    98640 2021-04-02 20:31:54.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   507628 2021-04-02 20:31:54.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    98404 2021-04-02 20:31:54.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    63728 2021-04-02 20:31:54.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.woff
+-rw-r--r--   0 root         (0) root         (0)    54488 2021-04-02 20:31:54.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.woff2
+-rw-r--r--   0 root         (0) root         (0)   106004 2021-04-02 20:31:55.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.eot
+-rw-r--r--   0 root         (0) root         (0)    93888 2021-04-02 20:31:57.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.otf
+-rw-r--r--   0 root         (0) root         (0)   390837 2021-04-02 20:31:57.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.svg
+-rw-r--r--   0 root         (0) root         (0)   105784 2021-04-02 20:32:01.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    50524 2021-04-02 20:32:01.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.woff
+-rw-r--r--   0 root         (0) root         (0)    40148 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.woff2
+-rw-r--r--   0 root         (0) root         (0)    31156 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   107201 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    30928 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    14712 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.woff
+-rw-r--r--   0 root         (0) root         (0)    12240 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/assets/images/
+-rw-r--r--   0 root         (0) root         (0)   258972 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/bg1.jpg
+-rw-r--r--   0 root         (0) root         (0)    11449 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/demo.png
+-rw-r--r--   0 root         (0) root         (0)      608 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/favicon.png
+-rw-r--r--   0 root         (0) root         (0)    28123 2021-04-02 20:31:57.000000 souschef-1.3.5/souschef/sous_chef/assets/images/flags.png
+-rw-r--r--   0 root         (0) root         (0)      490 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/geocoder.png
+-rw-r--r--   0 root         (0) root         (0)     1374 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/glyph-marker-icon.png
+-rw-r--r--   0 root         (0) root         (0)     1287 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/glyph-marker-icon.svg
+-rw-r--r--   0 root         (0) root         (0)    21977 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/jenny.jpg
+-rw-r--r--   0 root         (0) root         (0)    26952 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/joe.jpg
+-rw-r--r--   0 root         (0) root         (0)    23839 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/katrina.jpg
+-rw-r--r--   0 root         (0) root         (0)     2306 2021-04-02 20:32:01.000000 souschef-1.3.5/souschef/sous_chef/assets/images/leaflet.routing.icons.png
+-rw-r--r--   0 root         (0) root         (0)     4060 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/leaflet.routing.icons.svg
+-rw-r--r--   0 root         (0) root         (0)     6363 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/logo-souschef-coul.png
+-rw-r--r--   0 root         (0) root         (0)     6033 2021-04-02 20:32:05.000000 souschef-1.3.5/souschef/sous_chef/assets/images/logo-souschef-nb.png
+-rw-r--r--   0 root         (0) root         (0)      891 2021-04-02 20:32:05.000000 souschef-1.3.5/souschef/sous_chef/assets/images/logo.png
+-rw-r--r--   0 root         (0) root         (0)    14323 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/markers-matte.png
+-rw-r--r--   0 root         (0) root         (0)    30194 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/markers-matte@2x.png
+-rw-r--r--   0 root         (0) root         (0)     7946 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/markers-plain.png
+-rw-r--r--   0 root         (0) root         (0)      535 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/markers-shadow.png
+-rw-r--r--   0 root         (0) root         (0)     1134 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/markers-shadow@2x.png
+-rw-r--r--   0 root         (0) root         (0)    36367 2021-04-02 20:32:03.000000 souschef-1.3.5/souschef/sous_chef/assets/images/markers-soft.png
+-rw-r--r--   0 root         (0) root         (0)   146362 2021-04-02 20:32:04.000000 souschef-1.3.5/souschef/sous_chef/assets/images/markers-soft@2x.png
+-rw-r--r--   0 root         (0) root         (0)      454 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/routing-icon.png
+-rw-r--r--   0 root         (0) root         (0)     4831 2021-04-02 20:32:02.000000 souschef-1.3.5/souschef/sous_chef/assets/images/throbber.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/assets/js/
+-rw-r--r--   0 root         (0) root         (0)  1031323 2021-04-02 20:31:55.000000 souschef-1.3.5/souschef/sous_chef/assets/js/leaflet.js
+-rw-r--r--   0 root         (0) root         (0)   627692 2021-04-02 20:31:57.000000 souschef-1.3.5/souschef/sous_chef/assets/js/leaflet.min.js
+-rw-r--r--   0 root         (0) root         (0)    22295 2021-04-02 20:31:54.000000 souschef-1.3.5/souschef/sous_chef/assets/js/multidatespicker.js
+-rw-r--r--   0 root         (0) root         (0)    10453 2021-04-02 20:31:54.000000 souschef-1.3.5/souschef/sous_chef/assets/js/multidatespicker.min.js
+-rw-r--r--   0 root         (0) root         (0)  1110276 2021-04-02 20:31:57.000000 souschef-1.3.5/souschef/sous_chef/assets/js/sous-chef.js
+-rw-r--r--   0 root         (0) root         (0)   398796 2021-04-02 20:32:01.000000 souschef-1.3.5/souschef/sous_chef/assets/js/sous-chef.min.js
+-rw-r--r--   0 root         (0) root         (0)     1436 2020-12-18 20:03:32.000000 souschef-1.3.5/souschef/sous_chef/context_processors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/formats/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/formats/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/formats/en/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/formats/en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      186 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/formats/en/formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/formats/fr/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/formats/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/formats/fr/formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/management/commands/makemessages.py
+-rw-r--r--   0 root         (0) root         (0)      536 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/rules.py
+-rw-r--r--   0 root         (0) root         (0)     7517 2021-02-12 02:23:19.000000 souschef-1.3.5/souschef/sous_chef/settings.py
+-rw-r--r--   0 root         (0) root         (0)      227 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/settings_test.py
+-rw-r--r--   0 root         (0) root         (0)       59 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/settings_test_fr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/templates/
+-rw-r--r--   0 root         (0) root         (0)      611 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templates/404.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/templates/avatar/
+-rw-r--r--   0 root         (0) root         (0)     1870 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templates/avatar/change.html
+-rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templates/avatar/confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     3467 2021-03-26 14:29:59.000000 souschef-1.3.5/souschef/sous_chef/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/templates/dashboard/
+-rw-r--r--   0 root         (0) root         (0)      771 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templates/dashboard/statistics.html
+-rw-r--r--   0 root         (0) root         (0)     1271 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templates/splash.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/templates/system/
+-rw-r--r--   0 root         (0) root         (0)      219 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templates/system/_button_export.html
+-rw-r--r--   0 root         (0) root         (0)      209 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templates/system/breadcrumb.html
+-rw-r--r--   0 root         (0) root         (0)     2905 2021-03-02 23:43:41.000000 souschef-1.3.5/souschef/sous_chef/templates/system/menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:13.000000 souschef-1.3.5/souschef/sous_chef/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      319 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/templatetags/sous_chef_extras.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/urls.py
+-rw-r--r--   0 root         (0) root         (0)      395 2020-11-06 14:25:57.000000 souschef-1.3.5/souschef/sous_chef/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-02 20:32:10.000000 souschef-1.3.5/souschef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2522 2021-04-02 20:32:08.000000 souschef-1.3.5/souschef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15441 2021-04-02 20:32:09.000000 souschef-1.3.5/souschef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-02 20:32:08.000000 souschef-1.3.5/souschef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      462 2021-04-02 20:32:08.000000 souschef-1.3.5/souschef.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2021-04-02 20:32:08.000000 souschef-1.3.5/souschef.egg-info/top_level.txt
```

### Comparing `souschef-1.3.4/INSTALL.md` & `souschef-1.3.5/INSTALL.md`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/LICENSE.txt` & `souschef-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/PKG-INFO` & `souschef-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souschef
-Version: 1.3.4
+Version: 1.3.5
 Summary: Webapp used to manage orders for meals-on-wheel delivery
 Home-page: https://github.com/pypa/sous-chef
 Author: Santropol Roulant and Savoir Faire Linux
 Author-email: info@santropolroulant.org
 License: AGPL-3.0
 Description: # Sous-Chef
```

### Comparing `souschef-1.3.4/README.md` & `souschef-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/UPDATE.md` & `souschef-1.3.5/UPDATE.md`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/setup.py` & `souschef-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="souschef",
-    version="1.3.4",
+    version="1.3.5",
     license="AGPL-3.0",
     author="Santropol Roulant and Savoir Faire Linux",
     author_email="info@santropolroulant.org",
     description="Webapp used to manage orders for meals-on-wheel delivery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sous-chef",
```

### Comparing `souschef-1.3.4/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg` & `souschef-1.3.5/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/migrations/0001_initial.py` & `souschef-1.3.5/souschef/billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/models.py` & `souschef-1.3.5/souschef/billing/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/templates/billing/add.html` & `souschef-1.3.5/souschef/billing/templates/billing/add.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/templates/billing/billing_confirm_delete.html` & `souschef-1.3.5/souschef/billing/templates/billing/billing_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/templates/billing/list.html` & `souschef-1.3.5/souschef/billing/templates/billing/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/templates/billing/partials/statistics.html` & `souschef-1.3.5/souschef/billing/templates/billing/partials/statistics.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/templates/billing/partials/summary.html` & `souschef-1.3.5/souschef/billing/templates/billing/partials/summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/templates/billing/print_summary.html` & `souschef-1.3.5/souschef/billing/templates/billing/print_summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/templates/billing/view.html` & `souschef-1.3.5/souschef/billing/templates/billing/view.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/templates/billing/view_orders.html` & `souschef-1.3.5/souschef/billing/templates/billing/view_orders.html`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     </th>
     <th class="">{% trans 'Actions' %}</th>
   </thead>
   <tbody>
     {% for order in orders %}
     <tr>
       <td><i class="hashtag icon"></i>{{order.id}}</td>
-      <td><a href="{% url 'member:client_information' pk=order.client.id %}">{{order.client}}
+      <td><a href="{% url 'member:client_information' pk=order.client.id %}">{{order.client}}</a></td>
       <td>{{order.delivery_date}}</td>
       <td class="center aligned">{{order.get_status_display}}</td>
       <td class="center aligned"><i class="dollar icon"></i>{{order.price}}</td>
       <td>
         <a class="ui basic icon button"  href="{% url 'order:view' pk=order.id %}"><i class="icon unhide"></i></a>
       </td>
     </tr>
```

### Comparing `souschef-1.3.4/souschef/billing/tests.py` & `souschef-1.3.5/souschef/billing/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/urls.py` & `souschef-1.3.5/souschef/billing/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/billing/views.py` & `souschef-1.3.5/souschef/billing/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/configsamples/nginx.conf` & `souschef-1.3.5/souschef/configsamples/nginx.conf`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/dataload.py` & `souschef-1.3.5/souschef/dataload.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/datamigration/management/commands/importaddresses.py` & `souschef-1.3.5/souschef/datamigration/management/commands/importaddresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/datamigration/management/commands/importclients.py` & `souschef-1.3.5/souschef/datamigration/management/commands/importclients.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/datamigration/management/commands/importcontactaddresses.py` & `souschef-1.3.5/souschef/datamigration/management/commands/importcontactaddresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/datamigration/management/commands/importmeals.py` & `souschef-1.3.5/souschef/datamigration/management/commands/importmeals.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/datamigration/management/commands/importorders.py` & `souschef-1.3.5/souschef/datamigration/management/commands/importorders.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/datamigration/management/commands/importrelationships.py` & `souschef-1.3.5/souschef/datamigration/management/commands/importrelationships.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/datamigration/tests.py` & `souschef-1.3.5/souschef/datamigration/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/filters.py` & `souschef-1.3.5/souschef/delivery/filters.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/forms.py` & `souschef-1.3.5/souschef/delivery/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/migrations/0001_fix004a.py` & `souschef-1.3.5/souschef/delivery/migrations/0001_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/templates/edit_delivery_of_today.html` & `souschef-1.3.5/souschef/delivery/templates/edit_delivery_of_today.html`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,18 @@
             <th>{% trans 'View order' %}</th>
             <th>{% trans 'Address' %}</th>
             <th>{% trans 'Status' %}<i class="help-text question grey icon link" data-content="{% trans 'Configured, edited or unconfigured.' %}"></i></th>
           </tr>
         </thead>
         <tbody id="clients-on-delivery-history">
           {% for client in clients_on_delivery_history %}
-          <tr data-latitude="{{ client.member.address.latitude|unlocalize }}" data-longitude="{{ client.member.address.longitude|unlocalize }}" data-id="{{ client.pk }}">
+          <tr data-latitude="{{ client.member.address.latitude|unlocalize }}"
+              data-longitude="{{ client.member.address.longitude|unlocalize }}"
+              data-id="{{ client.pk }}"
+              {% if client.status != 'A' %}class="error"{% endif %}>
             <td data-property="delivery_sequence">{{ forloop.counter }}</td>
             <td data-property="name"><a href="{% url 'member:client_information' pk=client.pk %}" title="{% trans "Access the client's file" %}">{{ client.member.firstname }} {{ client.member.lastname }}</a></td>
             <td>{{ client.get_status_display }}</td>
             <td>{{ client.get_delivery_type_display }}</td>
             <td>
               {% if client.order_of_the_day %}
               <a href="{% url 'order:view' client.order_of_the_day.pk %}" title="{% trans "View the order" %}">{% trans 'Order #' %}{{ client.order_of_the_day.pk }}</a>
```

### Comparing `souschef-1.3.4/souschef/delivery/templates/ingredients.html` & `souschef-1.3.5/souschef/delivery/templates/ingredients.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/templates/kitchen_count.html` & `souschef-1.3.5/souschef/delivery/templates/kitchen_count.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/templates/kitchen_count_steps.html` & `souschef-1.3.5/souschef/delivery/templates/kitchen_count_steps.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/templates/partials/generated_orders.html` & `souschef-1.3.5/souschef/member/templates/client/partials/order_list.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,41 @@
-<!-- Load internationalisation utils-->
 {% load i18n %}
-{% load static %}
-{% load rules %}
 
-{% has_perm 'sous_chef.edit' request.user as can_edit_data %}
-<table id="generated-orders" class="ui very basic stripped compact celled table">
-  <thead>
-    <th class="">{% trans 'Order' %}
-            <i class="help-text question grey icon link" data-content="{% trans 'A unique identifier for the order.' %}"></i>
-    </th>
-    <th class="">{% trans 'Client' %}
-        <i class="help-text question grey icon link" data-content="{% trans 'Quickly access the client file.' %}"></i>
-    </th>
-    <th class="">{% trans 'Delivery Date' %}
-        <i class="help-text question grey icon link" data-content="{% trans 'The delivery date planned for the order.' %}"></i>
-    </th>
-    <th class="">{% trans 'Route' %}
-        <i class="help-text question grey icon link" data-content="{% trans 'The delivery route.' %}"></i>
-    </th>
-    <th class="center aligned">{% trans 'Status' %}
-        <i class="help-text question grey icon link" data-content="{% trans 'Display only Ordered orders.' %}"></i>
-    </th>
-    <th class="center aligned">{% trans 'Amount' %}
-        <i class="help-text question grey icon link" data-content="{% trans 'Total amount in $CAD.' %}"></i>
-    </th>
-    <th class=""></th>
-  </thead>
-  <tbody>
-    {% for order in orders %}
-      {% if order.status == 'O' %}
-      <tr {% if not order.client.is_geolocalized or not order.client.route %}class="error"{% endif %}>
-        <td class="center aligned"><strong><i class="hashtag icon"></i>{{order.id}}</strong></td>
-        <td><a href="{% url 'member:client_information' pk=order.client.id %}">{{order.client.member}}</a>
-        </td>
-        <td>{{order.delivery_date}}</td>
-        <td>
-          {% if order.client.route %}
-            {{order.client.route}}
-            {% if not order.client.is_geolocalized %}
-            <a href="{% url 'member:member_update_address_information' pk=order.client.id %}?next={% url 'delivery:order' %}" title="{% trans 'Please fix geolocalization. Otherwise this client will be excluded in the next steps.' %}"><i class="warning sign red icon"></i></a>
-            {% endif %}
-          {% else %}
-            <a href="{% url 'member:member_update_address_information' pk=order.client.id %}?next={% url 'delivery:order' %}" title="{% trans 'Please fix delivery route. Otherwise this client will be excluded in the next steps.' %}"><i class="warning sign red icon"></i></a>
-          {% endif %}
-        </td>
-        <td class="center aligned">{{order.get_status_display}}</td>
-        <td class="center aligned"><i class="dollar icon"></i>{{order.price}}</td>
-        <td>
-            <a class="ui basic icon button" title="{% trans 'Review or change the status of the order.' %}"  href="{% url 'order:view' pk=order.id %}"><i class="icon unhide"></i></a>
-            {% if can_edit_data %}
-              <a class="ui basic icon button" title="{% trans 'Change the details of the order.' %}" href="{% url 'order:update' pk=order.id %}"><i class="icon edit"></i></a>
-              <a class="ui basic icon order cancel button" title="{% trans 'Cancel the order.' %}" data-url="{% url 'order:update_status' pk=order.id %}"><i class="icon ban"></i></a>
-            {% endif %}
-        </td>
-      </tr>
-      {% endif %}
-    {% endfor %}
-  </tbody>
-</table>
+<table class="ui very basic stripped celled table">
+    <thead>
+        <th class="sorted descending">{% trans 'Order' %}
+                <i class="help-text question grey icon link" data-content="{% trans 'A unique identifier for the order.' %}"></i>
+        </th>
+        <th class="">{% trans 'Delivery Date' %}
+            <i class="help-text question grey icon link" data-content="{% trans 'The delivery date planned for the order.' %}"></i>
+        </th>
+        <th class="center aligned">{% trans 'Status' %}
+            <i class="help-text question grey icon link" data-content="{% trans 'The order status' %}"></i>
+        </th>
+        <th class="">{% trans 'Amount' %}
+            <i class="help-text question grey icon link" data-content="{% trans 'Total amount in $CAD.' %}"></i>
+        </th>
+        {% if show_actions_column %}
+        <th class="">{% trans 'Actions' %}</th>
+        {% endif %}
+      </thead>
+    </thead>
+    <tbody>
+        {% for order in orders %}
+            <tr>
+                <td><strong><i class="hashtag icon"></i>{{order.id}}</strong></td>
+                <td>{{order.delivery_date}}</td>
+                <td class="center aligned">{{order.get_status_display}}</td>
+                <td><i class="dollar icon"></i>{{order.price}}</td>
+                {% if show_actions_column %}
+                <td>
+                    <a class="ui basic icon button"  href="{% url 'order:view' pk=order.id %}"><i class="icon unhide"></i></a>
+                    {% if can_edit_data %}<a class="ui basic icon button"  href="{% url 'order:update' pk=order.id %}"><i class="icon edit"></i></a>{% endif %}
+                    {% if can_edit_data %}<a class="ui basic icon button order-delete" href="#" data-order-id="{{order.id}}"><i class="icon trash"></i></a>{% endif %}
+                </td>
+                {% endif %}
+            </tr>
+            {% if can_edit_data %}{% include "order_confirm_delete.html" %}{% endif %}
+        {% endfor %}
+    </tbody>
 
-{% if can_edit_data %}
-  <div class="ui modal status"></div>
-{% endif %}
+</table>
```

#### html2text {}

```diff
@@ -1,4 +1,7 @@
- {% load i18n %} {% load static %} {% load rules %} {% has_perm
-'sous_chef.edit' request.user as can_edit_data %}
-{% if can_edit_data %}
-{% endif %}
+{% load i18n %}
+                                                                               {% if
+                                                                              can_edit_data
+{           {                      {                           {              %}{% endif %}
+{order.id}} {order.delivery_date}} {order.get_status_display}} {order.price}} {% if
+                                                                              can_edit_data
+                                                                              %}{% endif %}
```

### Comparing `souschef-1.3.4/souschef/delivery/templates/review_orders.html` & `souschef-1.3.5/souschef/delivery/templates/review_orders.html`

 * *Files 2% similar despite different names*

```diff
@@ -57,34 +57,34 @@
     {% if can_edit_data %}
     <div class="sixteen wide center aligned column">
         <div class="ui row">
             <div class="ui labeled button" tabindex="0">
                 <div class="ui pink big button orders" data-url="{% url 'delivery:refresh_orders'%}">
                     <i class="refresh icon"></i> {% trans 'Generate orders' %}
                 </div>
-                {% with count=orders.count %}
+                {% with count=nb_of_ordered_orders %}
                 <a class="ui basic left pointing pink label orders-count" data-order-count={{count}}>
                   {# Translators: This text is displayed in the kitchen count -> step 1: order review -> pink button #}
                   {% blocktrans trimmed %}
-                    {{ count }} today
+                    <span>{{ count }}</span>&nbsp;today
                   {% endblocktrans %}
                 </a>
                 {% endwith %}
             </div>
         </div>
     </div>
     {% endif %}
 
     <h4 class="ui horizontal divider header">
         <i class="unhide icon"></i>
         {% trans 'Review' %}
     </h4>
 
     <div class="sixteen wide column">
-        <form action="" method="get" class="ui form">
+        <form action="" method="get" class="ui form review-orders-client-search">
             <div class="inline fields">
                 <div class="field">
                     <label for="{{ filter.form.client_name.auto_id }}">{% trans 'Client name' %}</label>
                     <div class="field">
                         <div class="ui large left icon input">
                             <i class="users icon"></i>
                             {{ filter.form.client_name }}
```

#### html2text {}

```diff
@@ -14,17 +14,17 @@
 orders button to manually run the script. {% endblocktrans %}
 
 {% trans 'Geolocation' %}
 {% trans 'Highlighted orders are not properly geolocated. Edit the client
 information to fix it.' %}
 {% if can_edit_data %}
  {% trans 'Generate orders' %}
-{% with count=orders.count %} {# Translators: This text is displayed in the
-kitchen count -> step 1: order review -> pink button #} {% blocktrans trimmed
-%} {{ count }} today {% endblocktrans %} {% endwith %}
+{% with count=nb_of_ordered_orders %} {# Translators: This text is displayed in
+the kitchen count -> step 1: order review -> pink button #} {% blocktrans
+trimmed %} {{ count }} today {% endblocktrans %} {% endwith %}
 {% endif %}
  {% trans 'Review' %}
 {% trans 'Client name' %}
  {{ filter.form.client_name }}
 {%_trans_'Reset'_%} {% trans 'Search' %}
 {% include 'partials/generated_orders.html' %}
 {% if can_edit_data %}
```

### Comparing `souschef-1.3.4/souschef/delivery/templates/route_sheet.html` & `souschef-1.3.5/souschef/delivery/templates/route_sheet.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/templates/routes.html` & `souschef-1.3.5/souschef/delivery/templates/routes.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/tests.py` & `souschef-1.3.5/souschef/delivery/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/tsp.py` & `souschef-1.3.5/souschef/delivery/tsp.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/urls.py` & `souschef-1.3.5/souschef/delivery/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/delivery/views.py` & `souschef-1.3.5/souschef/delivery/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,57 +45,92 @@
     COMPONENT_GROUP_CHOICES_MAIN_DISH,
     COMPONENT_GROUP_CHOICES_SIDES,
     Component,
     Menu, Menu_component,
     Component_ingredient)
 from souschef.member.models import Client, Route, DeliveryHistory
 from souschef.order.models import (
-    Order, component_group_sorting, SIZE_CHOICES_REGULAR, SIZE_CHOICES_LARGE)
+    component_group_sorting,
+    ORDER_STATUS_CANCELLED,
+    ORDER_STATUS_ORDERED,
+    Order,
+    SIZE_CHOICES_LARGE,
+    SIZE_CHOICES_REGULAR,
+)
 from .filters import KitchenCountOrderFilter
 from .forms import DishIngredientsForm
 from . import tsp
 
 
 LOGO_IMAGE = os.path.join(settings.BASE_DIR, "160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg")
 DELIVERY_STARTING_POINT_LAT_LONG = (45.516564, -73.575145)  # Santropol Roulant
 
 
-class Orderlist(LoginRequiredMixin, PermissionRequiredMixin, FilterView):
-    # Display all the order on a given day
-    context_object_name = 'orders'
-    filterset_class = KitchenCountOrderFilter
-    model = Order
-    permission_required = 'sous_chef.read'
-    template_name = 'review_orders.html'
-
-    def get_queryset(self):
-        queryset = Order.objects.get_shippable_orders().order_by(
+def get_orders_for_kitchen_count(order_statuses):
+    return Order.objects.get_orders(order_statuses=order_statuses).order_by(
             'client__route__pk', 'pk'
         ).prefetch_related('orders').select_related(
             'client__member',
             'client__route',
             'client__member__address'
         ).only(
             'delivery_date',
             'status',
             'client__member__firstname',
             'client__member__lastname',
             'client__route__name',
             'client__member__address__latitude',
             'client__member__address__longitude'
         )
-        return queryset
+
+
+def get_number_of_orders_in_status(orders, status):
+    return len([o for o in orders if o.status == status])
+
+
+def get_has_orders_in_status(orders, status):
+    return get_number_of_orders_in_status(orders, status) > 0
+
+
+def get_kitchen_count_context():
+    orders = get_orders_for_kitchen_count((ORDER_STATUS_ORDERED, ORDER_STATUS_CANCELLED))
+    return {
+        'orders': orders,
+        'has_ordered_orders': get_has_orders_in_status(orders, ORDER_STATUS_ORDERED),
+        'has_cancelled_orders': get_has_orders_in_status(orders, ORDER_STATUS_CANCELLED),
+        'nb_of_ordered_orders': get_number_of_orders_in_status(orders, ORDER_STATUS_ORDERED),
+    }
+
+
+class Orderlist(LoginRequiredMixin, PermissionRequiredMixin, FilterView):
+    # Display all the order on a given day
+    context_object_name = 'orders'
+    filterset_class = KitchenCountOrderFilter
+    model = Order
+    permission_required = 'sous_chef.read'
+    template_name = 'review_orders.html'
+
+    def get_queryset(self):
+        return get_orders_for_kitchen_count((ORDER_STATUS_ORDERED, ORDER_STATUS_CANCELLED))
 
     def get_context_data(self, **kwargs):
         context = super(Orderlist, self).get_context_data(**kwargs)
         context['orders_refresh_date'] = None
         if LogEntry.objects.exists():
             log = LogEntry.objects.latest('action_time')
             context['orders_refresh_date'] = log
 
+        # See also get_kitchen_count_context, used for the "Generate orders" button.
+        context['has_ordered_orders'] = get_has_orders_in_status(
+            context['orders'], ORDER_STATUS_ORDERED)
+        context['has_cancelled_orders'] = get_has_orders_in_status(
+            context['orders'], ORDER_STATUS_CANCELLED)
+        context['nb_of_ordered_orders'] = get_number_of_orders_in_status(
+            context['orders'], ORDER_STATUS_ORDERED)
+        print(context)
         return context
 
 
 class MealInformation(
         LoginRequiredMixin, PermissionRequiredMixin, generic.View):
     # Choose today's main dish and its ingredients
     permission_required = 'sous_chef.read'
@@ -1693,20 +1728,16 @@
 class RefreshOrderView(
         LoginRequiredMixin, PermissionRequiredMixin, generic.View):
     permission_required = 'sous_chef.edit'
 
     def get(self, request):
         delivery_date = date.today()
         clients = Client.ongoing.all()
-        orders = Order.objects.auto_create_orders(delivery_date, clients)
+        Order.objects.auto_create_orders(delivery_date, clients)
         LogEntry.objects.log_action(
             user_id=1, content_type_id=1,
             object_id="", object_repr="Generation of orders for " + str(
                 datetime.datetime.now().strftime('%m %d %Y %H:%M')),
             action_flag=ADDITION,
         )
-        orders.sort(key=lambda o: (
-            o.client.route.pk if o.client.route is not None else -1,
-            o.pk
-        ))
-        context = {'orders': orders}
+        context = get_kitchen_count_context()
         return render(request, 'partials/generated_orders.html', context)
```

### Comparing `souschef-1.3.4/souschef/frontend/images/bg1.jpg` & `souschef-1.3.5/souschef/frontend/images/bg1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/frontend/images/jenny.jpg` & `souschef-1.3.5/souschef/frontend/images/jenny.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/frontend/images/joe.jpg` & `souschef-1.3.5/souschef/frontend/images/joe.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/frontend/images/katrina.jpg` & `souschef-1.3.5/souschef/frontend/images/katrina.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/admin.py` & `souschef-1.3.5/souschef/meal/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/factories.py` & `souschef-1.3.5/souschef/meal/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/migrations/0001_fix161f.py` & `souschef-1.3.5/souschef/meal/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/migrations/0002_ingredient_ingredient_group.py` & `souschef-1.3.5/souschef/meal/migrations/0002_ingredient_ingredient_group.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/migrations/0003_fix224a.py` & `souschef-1.3.5/souschef/meal/migrations/0003_fix224a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/migrations/0005_fix241b.py` & `souschef-1.3.5/souschef/meal/migrations/0005_fix241b.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/migrations/0006_auto_20160826_0007.py` & `souschef-1.3.5/souschef/meal/migrations/0006_auto_20160826_0007.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/migrations/0007_auto_20170313_1442.py` & `souschef-1.3.5/souschef/meal/migrations/0007_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/migrations/0008_auto_20180704_1613.py` & `souschef-1.3.5/souschef/meal/migrations/0008_auto_20180704_1613.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/models.py` & `souschef-1.3.5/souschef/meal/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/meal/tests.py` & `souschef-1.3.5/souschef/meal/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/admin.py` & `souschef-1.3.5/souschef/member/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/factories.py` & `souschef-1.3.5/souschef/member/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/forms.py` & `souschef-1.3.5/souschef/member/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/formsfield.py` & `souschef-1.3.5/souschef/member/formsfield.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/management/commands/createclients.py` & `souschef-1.3.5/souschef/member/management/commands/createclients.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/management/commands/processscheduledstatuschange.py` & `souschef-1.3.5/souschef/member/management/commands/processscheduledstatuschange.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0001_fix161f.py` & `souschef-1.3.5/souschef/member/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0002_auto_20160605_1609.py` & `souschef-1.3.5/souschef/member/migrations/0002_auto_20160605_1609.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0003_auto_20160615_2100.py` & `souschef-1.3.5/souschef/member/migrations/0003_auto_20160615_2100.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0004_fix004a.py` & `souschef-1.3.5/souschef/member/migrations/0004_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0005_fix004a.py` & `souschef-1.3.5/souschef/member/migrations/0005_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0007_auto_20160726_1703.py` & `souschef-1.3.5/souschef/member/migrations/0007_auto_20160726_1703.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0008_auto_20160727_2251.py` & `souschef-1.3.5/souschef/member/migrations/0008_auto_20160727_2251.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0009_auto_20160728_1443.py` & `souschef-1.3.5/souschef/member/migrations/0009_auto_20160728_1443.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0010_auto_20160803_2052.py` & `souschef-1.3.5/souschef/member/migrations/0010_auto_20160803_2052.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0012_clientscheduledstatus.py` & `souschef-1.3.5/souschef/member/migrations/0012_clientscheduledstatus.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0013_auto_20160820_2322.py` & `souschef-1.3.5/souschef/member/migrations/0013_auto_20160820_2322.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0014_auto_20160826_0007.py` & `souschef-1.3.5/souschef/member/migrations/0014_auto_20160826_0007.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0016_auto_20160912_1509.py` & `souschef-1.3.5/souschef/member/migrations/0016_auto_20160912_1509.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0017_auto_20161020_2039.py` & `souschef-1.3.5/souschef/member/migrations/0017_auto_20161020_2039.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0018_auto_20161110_2352.py` & `souschef-1.3.5/souschef/member/migrations/0018_auto_20161110_2352.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0019_auto_20161111_1750.py` & `souschef-1.3.5/souschef/member/migrations/0019_auto_20161111_1750.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0022_auto_20161215_1936.py` & `souschef-1.3.5/souschef/member/migrations/0022_auto_20161215_1936.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0023_auto_20161220_1401.py` & `souschef-1.3.5/souschef/member/migrations/0023_auto_20161220_1401.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0024_auto_20161227_1819.py` & `souschef-1.3.5/souschef/member/migrations/0024_auto_20161227_1819.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0025_route_vehicle.py` & `souschef-1.3.5/souschef/member/migrations/0025_route_vehicle.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0026_change_to_emergency_contacts.py` & `souschef-1.3.5/souschef/member/migrations/0026_change_to_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0027_auto_20170313_1442.py` & `souschef-1.3.5/souschef/member/migrations/0027_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py` & `souschef-1.3.5/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0029_member_address_fk_to_1to1.py` & `souschef-1.3.5/souschef/member/migrations/0029_member_address_fk_to_1to1.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0030_route_deliveryhistory.py` & `souschef-1.3.5/souschef/member/migrations/0030_route_deliveryhistory.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0031_client_option_allow_reverse_relation.py` & `souschef-1.3.5/souschef/member/migrations/0031_client_option_allow_reverse_relation.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0032_relationship.py` & `souschef-1.3.5/souschef/member/migrations/0032_relationship.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0033_auto_20170801_1607.py` & `souschef-1.3.5/souschef/member/migrations/0033_auto_20170801_1607.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0034_auto_20170816_0850.py` & `souschef-1.3.5/souschef/member/migrations/0034_auto_20170816_0850.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0035_auto_20210115_1155.py` & `souschef-1.3.5/souschef/member/migrations/0035_auto_20210115_1155.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0036_member_addresses.py` & `souschef-1.3.5/souschef/member/migrations/0036_member_addresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0037_one_address_per_member.py` & `souschef-1.3.5/souschef/member/migrations/0037_one_address_per_member.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/migrations/0038_member_verbose_names.py` & `souschef-1.3.5/souschef/member/migrations/0038_member_verbose_names.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/models.py` & `souschef-1.3.5/souschef/member/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -662,14 +662,18 @@
                 datetime.date(2000, today.month, today.day):
             age = today.year - self.birthdate.year
         else:
             age = today.year - self.birthdate.year - 1
         return age
 
     @property
+    def status_verbose(self):
+        return dict(self.CLIENT_STATUS).get(self.status, _('Unknown'))
+
+    @property
     def orders(self):
         """
         Returns orders associated to this client
         """
         return self.client_order.all()
 
     @property
@@ -758,14 +762,29 @@
             return ()
         else:
             for day, meal_schedule in defaults:
                 if day in simple_meals_schedule:
                     prefs.append((day, meal_schedule))
             return prefs
 
+    @property
+    def is_in_error_for_the_kitchen_count(self):
+        """ Return True if the client is in error for the Kitchen Count orders list page.
+
+        The client is in error if either:
+        - is not not geolocalized;
+        - it has no route;
+        - it is not active.
+        """
+        return (
+            not self.is_geolocalized or
+            not self.route or
+            self.status != 'A'
+        )
+
     def set_simple_meals_schedule(self, schedule):
         """
         Set the delivery days for the client.
         @param schedule
             A python list of days.
         """
         meal_schedule_option, _ = Option.objects.get_or_create(
```

### Comparing `souschef-1.3.4/souschef/member/templates/client/base.html` & `souschef-1.3.5/souschef/member/templates/client/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/create/form.html` & `souschef-1.3.5/souschef/member/templates/client/create/form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/create/steps.html` & `souschef-1.3.5/souschef/member/templates/client/create/steps.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/list.html` & `souschef-1.3.5/souschef/member/templates/client/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/birthdays.html` & `souschef-1.3.5/souschef/member/templates/client/partials/birthdays.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/filters.html` & `souschef-1.3.5/souschef/member/templates/client/partials/filters.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/forms/address_information.html` & `souschef-1.3.5/souschef/member/templates/client/partials/forms/address_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/forms/basic_information.html` & `souschef-1.3.5/souschef/member/templates/client/partials/forms/basic_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/forms/dietary_restriction.html` & `souschef-1.3.5/souschef/member/templates/client/partials/forms/dietary_restriction.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/forms/meal_defaults.html` & `souschef-1.3.5/souschef/member/templates/client/partials/forms/meal_defaults.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/forms/payment_information.html` & `souschef-1.3.5/souschef/member/templates/client/partials/forms/payment_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/forms/relationship_form.html` & `souschef-1.3.5/souschef/member/templates/client/partials/forms/relationship_form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/forms/relationships.html` & `souschef-1.3.5/souschef/member/templates/client/partials/forms/relationships.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/partials/menu.html` & `souschef-1.3.5/souschef/member/templates/client/partials/menu.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/update/base.html` & `souschef-1.3.5/souschef/member/templates/client/update/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/update/status.html` & `souschef-1.3.5/souschef/member/templates/client/update/status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/allergies.html` & `souschef-1.3.5/souschef/member/templates/client/view/allergies.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/delete_status_confirmation.html` & `souschef-1.3.5/souschef/member/templates/client/view/delete_status_confirmation.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/information.html` & `souschef-1.3.5/souschef/member/templates/client/view/information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/notes.html` & `souschef-1.3.5/souschef/member/templates/client/view/notes.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/orders.html` & `souschef-1.3.5/souschef/member/templates/client/view/orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/payment.html` & `souschef-1.3.5/souschef/member/templates/client/view/payment.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/referent.html` & `souschef-1.3.5/souschef/member/templates/client/view/referent.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/status.html` & `souschef-1.3.5/souschef/member/templates/client/view/status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/client/view/summary.html` & `souschef-1.3.5/souschef/member/templates/client/view/summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/route/delivery_history_detail.html` & `souschef-1.3.5/souschef/member/templates/route/delivery_history_detail.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/route/detail.html` & `souschef-1.3.5/souschef/member/templates/route/detail.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/route/edit.html` & `souschef-1.3.5/souschef/member/templates/route/edit.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/templates/route/list.html` & `souschef-1.3.5/souschef/member/templates/route/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/tests.py` & `souschef-1.3.5/souschef/member/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/urls.py` & `souschef-1.3.5/souschef/member/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/member/views.py` & `souschef-1.3.5/souschef/member/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/factories.py` & `souschef-1.3.5/souschef/note/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/forms.py` & `souschef-1.3.5/souschef/note/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0001_initial.py` & `souschef-1.3.5/souschef/note/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0002_auto_20160818_2104.py` & `souschef-1.3.5/souschef/note/migrations/0002_auto_20160818_2104.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0003_auto_20160819_2037.py` & `souschef-1.3.5/souschef/note/migrations/0003_auto_20160819_2037.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0004_notepriority.py` & `souschef-1.3.5/souschef/note/migrations/0004_notepriority.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0005_note_priority_old_data_migration.py` & `souschef-1.3.5/souschef/note/migrations/0005_note_priority_old_data_migration.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0006_change_priority_field.py` & `souschef-1.3.5/souschef/note/migrations/0006_change_priority_field.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0007_notecategory.py` & `souschef-1.3.5/souschef/note/migrations/0007_notecategory.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0008_auto_20170116_1441.py` & `souschef-1.3.5/souschef/note/migrations/0008_auto_20170116_1441.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0009_auto_20170116_1543.py` & `souschef-1.3.5/souschef/note/migrations/0009_auto_20170116_1543.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0010_auto_20170313_1442.py` & `souschef-1.3.5/souschef/note/migrations/0010_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/migrations/0011_auto_20170419_1109.py` & `souschef-1.3.5/souschef/note/migrations/0011_auto_20170419_1109.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/models.py` & `souschef-1.3.5/souschef/note/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/templates/notes_add.html` & `souschef-1.3.5/souschef/note/templates/notes_add.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/templates/notes_client_list.html` & `souschef-1.3.5/souschef/note/templates/notes_client_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/templates/notes_list.html` & `souschef-1.3.5/souschef/note/templates/notes_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/tests.py` & `souschef-1.3.5/souschef/note/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/urls.py` & `souschef-1.3.5/souschef/note/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/note/views.py` & `souschef-1.3.5/souschef/note/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/notification/migrations/0001_fix161f.py` & `souschef-1.3.5/souschef/notification/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/notification/models.py` & `souschef-1.3.5/souschef/notification/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/admin.py` & `souschef-1.3.5/souschef/order/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/factories.py` & `souschef-1.3.5/souschef/order/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/forms.py` & `souschef-1.3.5/souschef/order/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/management/commands/generateorders.py` & `souschef-1.3.5/souschef/order/management/commands/generateorders.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/management/commands/setordersdelivered.py` & `souschef-1.3.5/souschef/order/management/commands/setordersdelivered.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0001_fix161f.py` & `souschef-1.3.5/souschef/order/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0002_auto_20160614_1736.py` & `souschef-1.3.5/souschef/order/migrations/0002_auto_20160614_1736.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0003_auto_20160615_1504.py` & `souschef-1.3.5/souschef/order/migrations/0003_auto_20160615_1504.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0004_fix004a.py` & `souschef-1.3.5/souschef/order/migrations/0004_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0005_fix241b.py` & `souschef-1.3.5/souschef/order/migrations/0005_fix241b.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0006_auto_20160803_2217.py` & `souschef-1.3.5/souschef/order/migrations/0006_auto_20160803_2217.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0008_auto_20160912_1509.py` & `souschef-1.3.5/souschef/order/migrations/0008_auto_20160912_1509.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0009_auto_20161012_1919.py` & `souschef-1.3.5/souschef/order/migrations/0009_auto_20161012_1919.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0011_auto_20161014_1901.py` & `souschef-1.3.5/souschef/order/migrations/0011_auto_20161014_1901.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0013_orderstatuschange.py` & `souschef-1.3.5/souschef/order/migrations/0013_orderstatuschange.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0014_auto_20161209_2045.py` & `souschef-1.3.5/souschef/order/migrations/0014_auto_20161209_2045.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0015_auto_20170410_1029.py` & `souschef-1.3.5/souschef/order/migrations/0015_auto_20170410_1029.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/migrations/0016_auto_20180704_1613.py` & `souschef-1.3.5/souschef/order/migrations/0016_auto_20180704_1613.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/mixins.py` & `souschef-1.3.5/souschef/order/mixins.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/models.py` & `souschef-1.3.5/souschef/order/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,27 @@
 MAIN_PRICE_LOW_INCOME = 4.50
 SIDE_PRICE_LOW_INCOME = 0.75
 MAIN_PRICE_SOLIDARY = 3.50
 SIDE_PRICE_SOLIDARY = 0.50
 
 
 class OrderManager(models.Manager):
+    def get_orders(self,
+                   delivery_date=None,
+                   order_statuses=None):
+        # If no date is passed, use the current day
+        if delivery_date is None:
+            delivery_date = date.today()
+        extra_kwargs = {}
+        if order_statuses:
+            extra_kwargs['status__in'] = order_statuses
+        return self.get_queryset().filter(
+            delivery_date=delivery_date,
+            **extra_kwargs,
+        )
 
     def get_shippable_orders(self,
                              delivery_date=None,
                              exclude_non_geolocalized=False):
         """
         Return the orders ready to be delivered for a given date.
         A shippable order must be created in the database, and its ORDER_STATUS
@@ -313,14 +326,15 @@
         for order_item_type, trans in ORDER_ITEM_TYPE_CHOICES:
             if order_item_type != ORDER_ITEM_TYPE_CHOICES_COMPONENT:
                 additional = items.get('{0}_default'.format(order_item_type))
                 if additional:
                     Order_item.objects.create(
                         order=order,
                         price=0,
+                        total_quantity=0,
                         billable_flag=False,
                         order_item_type=order_item_type)
 
         return order
 
     """
     Allow changing status of multiple orders at once.
@@ -613,15 +627,15 @@
                 Order_item.objects.create(
                     order=self,
                     price=0,
                     billable_flag=False,
                     size=None,
                     order_item_type="delivery",
                     remark=None,
-                    total_quantity=None,
+                    total_quantity=0,
                     component_group=None
                 )
         elif value is False:
             if self.includes_a_bill is True:
                 for item in self.orders.all():
                     if item.is_a_client_bill:
                         item.delete()
@@ -1142,16 +1156,14 @@
         verbose_name=_('remark'),
         null=True,
         blank=True,
     )
 
     total_quantity = models.IntegerField(
         verbose_name=_('total quantity'),
-        null=True,
-        blank=True,
     )
 
     free_quantity = models.IntegerField(
         verbose_name=_('free quantity'),
         null=True,
         blank=True,
     )
```

### Comparing `souschef-1.3.4/souschef/order/templates/_form.html` & `souschef-1.3.5/souschef/order/templates/_form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/templates/_order_info.html` & `souschef-1.3.5/souschef/order/templates/_order_info.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/templates/create.html` & `souschef-1.3.5/souschef/order/templates/create.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/templates/list.html` & `souschef-1.3.5/souschef/order/templates/list.html`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 <!-- Load internationalisation utils-->
 {% load i18n %}
 {% load static %}
 {% load rules %}
 
 {% block title %} {% trans 'Orders' %} {% endblock %}
 
+{% block extrajs %}
+<script type="application/javascript">
+enableGeneratedOrdersCancelButton();
+</script>
+{% endblock %}
+
 {% block content %}
 {% has_perm 'sous_chef.edit' request.user as can_edit_data %}
 
 <div class="ui secondary pointing fluid menu">
     <h1 class="ui header">{% trans "Orders" %}</h1>
 </div>
 
@@ -44,24 +50,34 @@
     <th class="">{% trans 'Amount' %}
         <i class="help-text question grey icon link" data-content="{% trans 'Total amount in $CAD.' %}"></i>
     </th>
     <th class="">{% trans 'Actions' %}</th>
   </thead>
   <tbody>
     {% for order in orders %}
-      <tr>
+      <tr {% if order.status == 'O' and order.client.status != 'A' %}class="error"{% endif %}>
         <td><strong><i class="hashtag icon"></i>{{order.id}}</strong></td>
-        <td><a href="{% url 'member:client_information' pk=order.client.id %}">{{order.client.member}}</a></td>
+        <td>
+            <a href="{% url 'member:client_information' pk=order.client.id %}">{{order.client.member}}</a>
+            {% if order.client.status != 'A' %}
+            ({{ order.client.status_verbose }})
+            {% endif %}
+        </td>
         <td>{{order.delivery_date}}</td>
         <td class="center aligned">{{order.get_status_display}}</td>
         <td><i class="dollar icon"></i>{{order.price}}</td>
         <td>
           <a class="ui basic icon button"  href="{% url 'order:view' pk=order.id %}"><i class="icon unhide"></i></a>
-          {% if can_edit_data %}<a class="ui basic icon button"  href="{% url 'order:update' pk=order.id %}"><i class="icon edit"></i></a>{% endif %}
-          {% if can_edit_data %}<a class="ui basic icon button order-delete" href="#" data-order-id="{{order.id}}"><i class="icon trash"></i></a>{% endif %}
+          {% if can_edit_data %}
+            <a class="ui basic icon button" title="{% trans 'Edit the order.' %}" href="{% url 'order:update' pk=order.id %}"><i class="icon edit"></i></a>
+            {% if order.status == 'O' %}
+            <a class="ui basic icon order cancel button" title="{% trans 'Cancel the order.' %}" data-url="{% url 'order:update_status' pk=order.id %}"><i class="icon ban"></i></a>
+            {% endif %}
+            <a class="ui basic icon button order-delete" title="{% trans 'Delete the order.' %}" href="#" data-order-id="{{order.id}}"><i class="icon trash"></i></a>
+          {% endif %}
         </td>
       </tr>
       {% include "order_confirm_delete.html" %}
     {% endfor %}
   </tbody>
   <tfoot>
       <tr>
@@ -95,8 +111,13 @@
 {% endif %}
 
 
 {% else %}
     <div class="ui row"><p>{% trans "Sorry, no result found" %}.</p></div>
 {% endif %}
 
+{# To display the cancel dialog. #}
+{% if can_edit_data %}
+  <div class="ui modal status"></div>
+{% endif %}
+
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,23 +1,19 @@
 {% extends "base.html" %}  {% load i18n %} {% load static %} {% load rules %}
-{% block title %} {% trans 'Orders' %} {% endblock %} {% block content %} {%
-has_perm 'sous_chef.edit' request.user as can_edit_data %}
+{% block title %} {% trans 'Orders' %} {% endblock %} {% block extrajs %}
+ {% endblock %} {% block content %} {% has_perm 'sous_chef.edit' request.user
+as can_edit_data %}
 ****** {% trans "Orders" %} ******
 {% if can_edit_data %}
 {%_trans_'New_orders'_%}
 {% trans 'Or' %}
 {% endif %} {% include 'order/partials/filters.html' %}
 {% if orders %}
-                                                                                                      {% if
-                                                                                                     can_edit_data
-{           {                      {                      {                           {              %}{% endif %}
-{order.id}} {order.client.member}} {order.delivery_date}} {order.get_status_display}} {order.price}} {% if
-                                                                                                     can_edit_data
-                                                                                                     %}{% endif %}
-            {% include "system/_button_export.html" %}
+ {% include "system/_button_export.html" %}
 {% if is_paginated %}
 > {% if page_obj.has_previous %}  {% endif %} {{ page_obj.number }} {% trans
 "of" %} {{ page_obj.paginator.num_pages }} {% if page_obj.has_next %}  {% endif
 %}
 {% endif %} {% else %}
 {% trans "Sorry, no result found" %}.
+{% endif %} {# To display the cancel dialog. #} {% if can_edit_data %}
 {% endif %} {% endblock %}
```

### Comparing `souschef-1.3.4/souschef/order/templates/order/create_batch.html` & `souschef-1.3.5/souschef/order/templates/order/create_batch.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/templates/order/partials/filters.html` & `souschef-1.3.5/souschef/order/templates/order/partials/filters.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/templates/order_confirm_delete.html` & `souschef-1.3.5/souschef/order/templates/order_confirm_delete.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 {% load i18n %}
 
-<div class="ui basic modal order-{{order.id}}">
+<div class="ui basic modal order-delete-{{order.id}}">
   <div class="ui icon header">
       <i class="trash icon"></i>
       {% trans "Delete Order" %} #{{order.id}}
     </div>
-  <div class="content" style="text-align:center;">
-      <p>{% trans 'This order will be deleted and all the info will be lost, are you sure?' %}</p>
+  <div class="content" style="font-size: 1.3em;">
+      <p>{% trans 'This order will be deleted.' %}</p>
+      <p>{% blocktrans with client_name=order.client.member %}Please note that will not prevent a new order from being generated in the Kitchen Count for <span class="confirm-client-name">{{ client_name }}</span> when pressing "Generate orders".{% endblocktrans %}
+      <p>{% trans 'Are you sure?' %}</p>
   </div>
   <div class="actions">
     <form action="{% url 'order:delete' pk=order.id %}?next={% url 'order:list' %}%3F{{request.META.QUERY_STRING|urlencode}}" method="POST" id="order-{{order.id}}-delete-form">{% csrf_token %}
        <div class="ui red cancel button"> <i class="remove icon"></i> {% trans "No" %} </div>
        <button class="ui green button" type="submit"> <i class="checkmark icon"></i> {% trans "Yes" %} </button>
    </form>
      </div>
```

### Comparing `souschef-1.3.4/souschef/order/templates/order_update_status.html` & `souschef-1.3.5/souschef/order/templates/order_update_status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/order/templates/update.html` & `souschef-1.3.5/souschef/order/templates/update.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 {% load static %}
 
 {% block title %} {% trans 'Orders' %} {% endblock %}
 
 {% block content %}
 
 <div class="ui secondary pointing fluid menu">
-    <h2 class="ui header">{% trans "Update Order" %}</h2>
+    <h2 class="ui header">{% trans "Modify Order" %}</h2>
 </div>
 
 <div class="ten wide column form-steps">
     <form action="" method="post" class="ui form error">
         {% if form.errors or formset.errors %}
             <div class="ui error message">
               <div class="header">{% trans 'Required information missing' %}</div>
               <p>{% trans 'Please review the form to make sure that all required fields are filled.' %}</p>
             </div>
         {% endif %}
         {% csrf_token %}
         {% include "_form.html" %}
         <a class="ui default button" href="{{ request.META.HTTP_REFERER }}">{% trans "Cancel" %}</a>
-        <button class="ui primary button" type="submit">{% trans "Update" %}</button>
+        <button class="ui primary button" type="submit">{% trans "Modify" %}</button>
     </form>
 </div>
 
 {% endblock %}
 
 {% block extrajs %}
 <script type="text/javascript">
```

### Comparing `souschef-1.3.4/souschef/order/templates/view.html` & `souschef-1.3.5/souschef/order/templates/view.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 {% block content %}
 {% has_perm 'sous_chef.edit' request.user as can_edit_data %}
 
 <div class="ui secondary pointing fluid menu">
     <h1 class="ui header">{% trans "Order" %} #{{ order.id }}</h1>
     <div class="right menu">
+        <h4 class="ui header" style="margin-top: 1.1em;">{% trans "Update Status:" %}</h4>
         <div class="ui item">
             <div id="order-status " class="ui dropdown order status{% if not can_edit_data %} disabled{% endif %}" data-url="{% url 'order:update_status' pk=order.id %}" data-csrf-token="{{ csrf_token }}">
                 <div class="ui large yellow label text">{{ order.get_status_display }}</div>
                 <i class="dropdown icon"></i>
                 <div class="menu">
                     {% for k,s in status %}
                         <div class="item" data-value={{k}}> {{s}} </div>
@@ -74,17 +75,17 @@
       </tfoot>
   </table>
 </div>
 </div>
 
 {% if can_edit_data %}
 <div class="ui row">
-
-    <a class="ui basic red button order-delete" href="#" data-order-id="{{order.id}}"><i class="icon trash"></i>{% trans "Delete" %}</a>
-    <a class="ui basic green button" href="{% url 'order:update' pk=order.id %}"><i class="icon edit"></i>{% trans "Update" %}</a>
-
+    <div class="ui column right aligned">
+        <a class="ui basic red button order-delete" href="#" data-order-id="{{order.id}}"><i class="icon trash"></i>{% trans "Delete" %}</a>
+        <a class="ui blue button" href="{% url 'order:update' pk=order.id %}"><i class="icon edit"></i>{% trans "Modify" %}</a>
+    </div>
 </div>
 
 {% include 'order_confirm_delete.html' %}
 {% endif %}
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends "base_order.html" %}  {% load i18n %} {% load rules %} {% block
 title %} {% trans 'View Order' %} {% endblock %} {% block content %} {%
 has_perm 'sous_chef.edit' request.user as can_edit_data %}
 ****** {% trans "Order" %} #{{ order.id }} ******
+*** {% trans "Update Status:" %} ***
 {{ order.get_status_display }}
 {% for k,s in status %}
 {{s}}
 {% endfor %}
 {% include "_order_info.html" %}
 {% trans "Order detail" %}
 {% trans "Order items attached to the order" %}.
@@ -14,9 +15,9 @@
                                                                                                                                  {
 {% trans "Total" %}                                                                                                              {
                                                                                                                                  order.price
                                                                                                                                  }}
 {% if can_edit_data %}
 {%_trans_"Delete"_%}
 
-{%_trans_"Update"_%}
+{%_trans_"Modify"_%}
 {% include 'order_confirm_delete.html' %} {% endif %} {% endblock %}
```

### Comparing `souschef-1.3.4/souschef/order/tests.py` & `souschef-1.3.5/souschef/order/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,53 +143,58 @@
             status='B', client=client,
         )
         Order_item.objects.create(
             order=cls.total_zero_order,
             price=22.50,
             billable_flag=False,
             order_item_type='',
-            remark="12"
+            remark="12",
+            total_quantity=0,
         )
         cls.order = Order.objects.create(
             delivery_date=date(2016, 5, 10),
             status='B', client=client,
         )
         Order_item.objects.create(
             order=cls.order,
             price=6.50,
             billable_flag=True,
             order_item_type='',
             remark="testing",
             size="R",
+            total_quantity=0,
         )
         Order_item.objects.create(
             order=cls.order,
             price=12.50,
             billable_flag=False,
             order_item_type='',
             remark="testing",
             size="L",
+            total_quantity=0,
         )
         Order_item.objects.create(
             order=cls.order,
             price=8.00,
             billable_flag=False,
             order_item_type='delivery',
             component_group='main_dish',
             remark="testing",
             size="L",
+            total_quantity=0,
         )
         Order_item.objects.create(
             order=cls.order,
             price=0,
             billable_flag=False,
             order_item_type='delivery',
             component_group=None,
             remark="testing",
             size="L",
+            total_quantity=0,
         )
 
     def test_billable_flag(self):
         billable_order_item = Order_item.objects.get(
             order=self.order, price=6.50)
         self.assertEqual(billable_order_item.billable_flag, True)
 
@@ -276,14 +281,15 @@
             order=self.order,
             price=0,
             billable_flag=False,
             order_item_type='delivery',
             component_group=None,
             remark="testing",
             size="L",
+            total_quantity=0,
         )
         self.assertEqual(Order_item.objects.filter(
             order=self.order,
             order_item_type='delivery',
             component_group=None).count(), 2)
         self.order.refresh_from_db()
         self.assertTrue(self.order.includes_a_bill)
@@ -1585,14 +1591,15 @@
         check(reverse('order:list'))
         check(reverse('order:view', kwargs={'pk': 1}))
         check(reverse('order:create'))
         check(reverse('order:create_batch'))
         check(reverse('order:update', kwargs={'pk': 1}))
         check(reverse('order:update_status', kwargs={'pk': 1}))
         check(reverse('order:update_client_bill', kwargs={'pk': 1}))
+        check(reverse('order:cancel', kwargs={'pk': 1}))
         check(reverse('order:delete', kwargs={'pk': 1}))
 
 
 class CommandsTestCase(TestCase):
     "Test custom manage.py commands"
 
     @classmethod
```

### Comparing `souschef-1.3.4/souschef/order/urls.py` & `souschef-1.3.5/souschef/order/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from django.conf.urls import url
 from django.utils.translation import ugettext_lazy as _
 
 from souschef.order.views import (
-    OrderList,
-    OrderDetail,
+    CancelOrder,
+    CreateDeleteOrderClientBill,
     CreateOrder,
     CreateOrdersBatch,
+    DeleteOrder,
+    OrderDetail,
+    OrderList,
     UpdateOrder,
     UpdateOrderStatus,
-    CreateDeleteOrderClientBill,
-    DeleteOrder)
+)
 
 app_name = "order"
 
 urlpatterns = [
     url(_(r'^list/$'), OrderList.as_view(), name='list'),
     url(_(r'^view/(?P<pk>\d+)/$'), OrderDetail.as_view(), name='view'),
     url(_(r'^create/$'), CreateOrder.as_view(), name='create'),
@@ -28,9 +30,10 @@
         name='update_status'
     ),
     url(
         _(r'^update/(?P<pk>\d+)/client_bill$'),
         CreateDeleteOrderClientBill.as_view(),
         name='update_client_bill'
     ),
+    url(_(r'^cancel/(?P<pk>\d+)/$'), CancelOrder.as_view(), name='cancel'),
     url(_(r'^delete/(?P<pk>\d+)/$'), DeleteOrder.as_view(), name='delete'),
 ]
```

### Comparing `souschef-1.3.4/souschef/order/views.py` & `souschef-1.3.5/souschef/order/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import csv
 import json
+
 from django.http import HttpResponse
+from django.http.response import HttpResponseRedirect
 from django.views import generic, View
 from django.views.decorators.csrf import csrf_exempt
 from django.utils.decorators import method_decorator
 from django.utils.translation import ugettext_lazy as _
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from django.contrib import messages
 from django.urls import reverse_lazy, reverse
 from django.utils import timezone
 from django.shortcuts import get_object_or_404
 from extra_views import CreateWithInlinesView, UpdateWithInlinesView
 
 from datetime import datetime
 
-from souschef.order.models import Order, OrderFilter, \
+from souschef.order.models import ORDER_STATUS_CANCELLED, Order, OrderFilter, \
     ORDER_STATUS, OrderStatusChange
 from souschef.order.mixins import AjaxableResponseMixin, FormValidAjaxableResponseMixin
 from souschef.order.forms import CreateOrderItem, UpdateOrderItem, \
     CreateOrdersBatchForm, OrderStatusChangeForm
 
 from souschef.meal.models import COMPONENT_GROUP_CHOICES, COMPONENT_GROUP_CHOICES_SIDES
 from souschef.meal.settings import COMPONENT_SYSTEM_DEFAULT
@@ -339,15 +341,15 @@
             'status_to': self.request.GET.get('status'),
         }
 
     def form_valid(self, form):
         response = super(UpdateOrderStatus, self).form_valid(form)
         messages.add_message(
             self.request, messages.SUCCESS,
-            _("The status has been changed")
+            _("The order status was updated successfully.")
         )
         return response
 
     def get_success_url(self):
         return reverse(
             'order:view', kwargs={'pk': self.kwargs.get('pk')}
         )
@@ -371,14 +373,25 @@
 
     def delete(self, request, pk, *args, **kwargs):
         order = self.get_object(pk)
         order.includes_a_bill = False
         return HttpResponse('OK', status=200)
 
 
+class CancelOrder(
+        LoginRequiredMixin, PermissionRequiredMixin, View):
+    permission_required = 'sous_chef.edit'
+
+    def post(self, request, pk, *args, **kwargs):
+        order = get_object_or_404(Order, pk=pk)
+        order.status = ORDER_STATUS_CANCELLED
+        order.save()
+        return HttpResponseRedirect(request.GET['next'])
+
+
 class DeleteOrder(
         LoginRequiredMixin, PermissionRequiredMixin, generic.DeleteView):
     model = Order
     permission_required = 'sous_chef.edit'
     template_name = 'order_confirm_delete.html'
 
     def get_success_url(self):
```

### Comparing `souschef-1.3.4/souschef/page/templates/pages/home.html` & `souschef-1.3.5/souschef/page/templates/pages/home.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/page/templates/registration/login.html` & `souschef-1.3.5/souschef/page/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/page/tests.py` & `souschef-1.3.5/souschef/page/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/page/views.py` & `souschef-1.3.5/souschef/page/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/css/main.min.css` & `souschef-1.3.5/souschef/sous_chef/assets/css/main.min.css`

 * *Files 0% similar despite different names*

```diff
@@ -40906,27 +40906,34 @@
 0009fc90: 782e 706e 6729 2169 6d70 6f72 7461 6e74  x.png)!important
 0009fca0: 7d7d 2e6c 6561 666c 6574 2d72 6f75 7469  }}.leaflet-routi
 0009fcb0: 6e67 2d61 6c74 7b64 6973 706c 6179 3a6e  ng-alt{display:n
 0009fcc0: 6f6e 657d 2e72 6f75 7465 2d73 697a 652d  one}.route-size-
 0009fcd0: 6d6f 6e69 746f 7269 6e67 2e74 6162 6c65  monitoring.table
 0009fce0: 2074 666f 6f74 7b62 6163 6b67 726f 756e   tfoot{backgroun
 0009fcf0: 642d 636f 6c6f 723a 2365 3166 3166 667d  d-color:#e1f1ff}
-0009fd00: 7461 626c 652e 7569 2d64 6174 6570 6963  table.ui-datepic
-0009fd10: 6b65 722d 6361 6c65 6e64 6172 7b62 6f72  ker-calendar{bor
-0009fd20: 6465 722d 636f 6c6c 6170 7365 3a73 6570  der-collapse:sep
-0009fd30: 6172 6174 657d 2e75 692d 6461 7465 7069  arate}.ui-datepi
-0009fd40: 636b 6572 2d63 616c 656e 6461 7220 7464  cker-calendar td
-0009fd50: 7b62 6f72 6465 723a 3170 7820 736f 6c69  {border:1px soli
-0009fd60: 6420 7472 616e 7370 6172 656e 7421 696d  d transparent!im
-0009fd70: 706f 7274 616e 747d 2e75 692d 6461 7465  portant}.ui-date
-0009fd80: 7069 636b 6572 202e 7569 2d64 6174 6570  picker .ui-datep
-0009fd90: 6963 6b65 722d 6361 6c65 6e64 6172 202e  icker-calendar .
-0009fda0: 6f72 6465 7265 642d 6461 7465 2061 7b62  ordered-date a{b
-0009fdb0: 6f72 6465 723a 3170 7820 736f 6c69 6420  order:1px solid 
-0009fdc0: 2366 6365 6661 313b 6261 636b 6772 6f75  #fcefa1;backgrou
-0009fdd0: 6e64 3a23 6662 6639 6565 206e 6f6e 657d  nd:#fbf9ee none}
-0009fde0: 2e75 692d 6461 7465 7069 636b 6572 202e  .ui-datepicker .
-0009fdf0: 7569 2d64 6174 6570 6963 6b65 722d 6361  ui-datepicker-ca
-0009fe00: 6c65 6e64 6172 202e 7569 2d73 7461 7465  lendar .ui-state
-0009fe10: 2d68 6967 686c 6967 6874 2061 7b62 6163  -highlight a{bac
-0009fe20: 6b67 726f 756e 643a 2366 6262 6430 3820  kground:#fbbd08 
-0009fe30: 6e6f 6e65 3b63 6f6c 6f72 3a23 6666 667d  none;color:#fff}
+0009fd00: 2e72 6576 6965 772d 6f72 6465 7273 2d63  .review-orders-c
+0009fd10: 6c69 656e 742d 7365 6172 6368 7b6d 6172  lient-search{mar
+0009fd20: 6769 6e2d 626f 7474 6f6d 3a32 656d 7d2e  gin-bottom:2em}.
+0009fd30: 636f 6e66 6972 6d2d 636c 6965 6e74 2d6e  confirm-client-n
+0009fd40: 616d 657b 666f 6e74 2d77 6569 6768 743a  ame{font-weight:
+0009fd50: 3730 303b 7465 7874 2d64 6563 6f72 6174  700;text-decorat
+0009fd60: 696f 6e3a 756e 6465 726c 696e 657d 7461  ion:underline}ta
+0009fd70: 626c 652e 7569 2d64 6174 6570 6963 6b65  ble.ui-datepicke
+0009fd80: 722d 6361 6c65 6e64 6172 7b62 6f72 6465  r-calendar{borde
+0009fd90: 722d 636f 6c6c 6170 7365 3a73 6570 6172  r-collapse:separ
+0009fda0: 6174 657d 2e75 692d 6461 7465 7069 636b  ate}.ui-datepick
+0009fdb0: 6572 2d63 616c 656e 6461 7220 7464 7b62  er-calendar td{b
+0009fdc0: 6f72 6465 723a 3170 7820 736f 6c69 6420  order:1px solid 
+0009fdd0: 7472 616e 7370 6172 656e 7421 696d 706f  transparent!impo
+0009fde0: 7274 616e 747d 2e75 692d 6461 7465 7069  rtant}.ui-datepi
+0009fdf0: 636b 6572 202e 7569 2d64 6174 6570 6963  cker .ui-datepic
+0009fe00: 6b65 722d 6361 6c65 6e64 6172 202e 6f72  ker-calendar .or
+0009fe10: 6465 7265 642d 6461 7465 2061 7b62 6f72  dered-date a{bor
+0009fe20: 6465 723a 3170 7820 736f 6c69 6420 2366  der:1px solid #f
+0009fe30: 6365 6661 313b 6261 636b 6772 6f75 6e64  cefa1;background
+0009fe40: 3a23 6662 6639 6565 206e 6f6e 657d 2e75  :#fbf9ee none}.u
+0009fe50: 692d 6461 7465 7069 636b 6572 202e 7569  i-datepicker .ui
+0009fe60: 2d64 6174 6570 6963 6b65 722d 6361 6c65  -datepicker-cale
+0009fe70: 6e64 6172 202e 7569 2d73 7461 7465 2d68  ndar .ui-state-h
+0009fe80: 6967 686c 6967 6874 2061 7b62 6163 6b67  ighlight a{backg
+0009fe90: 726f 756e 643a 2366 6262 6430 3820 6e6f  round:#fbbd08 no
+0009fea0: 6e65 3b63 6f6c 6f72 3a23 6666 667d       ne;color:#fff}
```

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.eot` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.svg` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.ttf` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.woff` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/brand-icons.woff2` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.eot` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.otf` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.otf`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.svg` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.ttf` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.woff` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/icons.woff2` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.eot` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.svg` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.ttf` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.woff` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/fonts/outline-icons.woff2` & `souschef-1.3.5/souschef/sous_chef/assets/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/bg1.jpg` & `souschef-1.3.5/souschef/sous_chef/assets/images/bg1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/demo.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/demo.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/favicon.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/flags.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/flags.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/glyph-marker-icon.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/glyph-marker-icon.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/glyph-marker-icon.svg` & `souschef-1.3.5/souschef/sous_chef/assets/images/glyph-marker-icon.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/jenny.jpg` & `souschef-1.3.5/souschef/sous_chef/assets/images/jenny.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/joe.jpg` & `souschef-1.3.5/souschef/sous_chef/assets/images/joe.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/katrina.jpg` & `souschef-1.3.5/souschef/sous_chef/assets/images/katrina.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/leaflet.routing.icons.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/leaflet.routing.icons.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/leaflet.routing.icons.svg` & `souschef-1.3.5/souschef/sous_chef/assets/images/leaflet.routing.icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/logo-souschef-coul.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/logo-souschef-coul.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/logo-souschef-nb.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/logo-souschef-nb.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/logo.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/markers-matte.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/markers-matte.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/markers-matte@2x.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/markers-matte@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/markers-plain.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/markers-plain.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/markers-shadow.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/markers-shadow.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/markers-shadow@2x.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/markers-shadow@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/markers-soft.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/markers-soft.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/markers-soft@2x.png` & `souschef-1.3.5/souschef/sous_chef/assets/images/markers-soft@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/images/throbber.gif` & `souschef-1.3.5/souschef/sous_chef/assets/images/throbber.gif`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/js/leaflet.js` & `souschef-1.3.5/souschef/sous_chef/assets/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/js/leaflet.min.js` & `souschef-1.3.5/souschef/sous_chef/assets/js/leaflet.min.js`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/js/multidatespicker.js` & `souschef-1.3.5/souschef/sous_chef/assets/js/multidatespicker.js`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/js/multidatespicker.min.js` & `souschef-1.3.5/souschef/sous_chef/assets/js/multidatespicker.min.js`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/js/sous-chef.js` & `souschef-1.3.5/souschef/sous_chef/assets/js/sous-chef.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -33375,49 +33375,15 @@
                 return date ? dateFormat(date, 'yyyy-mm-dd') : '';
             }
         }
     });
 
 });
 
-$(function() {
-    // Javascript of the delivery application
-    // ****************************************
-
-    $('.ui.dropdown.maindish.selection').dropdown('setting', 'onChange', function(value, text, $selectedItem) {
-        $url = $(".field.dish.selection").data('url');
-        window.location.replace($url + value);
-    });
-
-    $('.ui.dropdown.mainingredients.selection').dropdown('setting', 'onChange', function(value, text, $selectedItem) {
-        $('.button.confirmingredients').removeClass('disabled');
-        $('.button.nextkitchencount').addClass('disabled');
-        $('.button.restorerecipe').removeClass('disabled');
-    });
-
-    $('.ui.dropdown.sidesingredients.selection').dropdown('setting', 'onChange', function(value, text, $selectedItem) {
-        $('.button.confirmingredients').removeClass('disabled');
-        $('.button.nextkitchencount').addClass('disabled');
-    });
-
-    $('.button.orders').click(function() {
-        $('.button.orders i').addClass('loading');
-        $.ajax({
-            type: 'GET',
-            url: $(this).attr('data-url'),
-            success: function(xhr, ajaxOptions, thrownError) {
-                $("#generated-orders").html(xhr)
-                var count = $("#generated-orders tbody tr").length;
-                $('.orders-count span').html(count);
-                $('.orders-count').attr('data-order-count', count);
-                $('.button.orders i').removeClass('loading');
-            },
-        });
-    });
-
+function enableGeneratedOrdersCancelButton() {
     $('.ui.order.cancel.button').click(function() {
         var self = this;
         var modalCtntURL = $(self).attr('data-url');
         $.get(modalCtntURL, {
             status: 'C'
         }, function(data, modalCtntURL) {
             $('.ui.modal.status').html(data).modal("setting", {
@@ -33444,14 +33410,53 @@
                 // When denying modal, restore default value for status dropdown
                 onDeny: function($element) {
                     $('.ui.modal.status').modal("hide");
                 }
             }).modal('setting', 'autofocus', false).modal("show");
         });
     });
+}
+
+$(function() {
+    // Javascript of the delivery application
+    // ****************************************
+
+    enableGeneratedOrdersCancelButton();
+
+    $('.ui.dropdown.maindish.selection').dropdown('setting', 'onChange', function(value, text, $selectedItem) {
+        $url = $(".field.dish.selection").data('url');
+        window.location.replace($url + value);
+    });
+
+    $('.ui.dropdown.mainingredients.selection').dropdown('setting', 'onChange', function(value, text, $selectedItem) {
+        $('.button.confirmingredients').removeClass('disabled');
+        $('.button.nextkitchencount').addClass('disabled');
+        $('.button.restorerecipe').removeClass('disabled');
+    });
+
+    $('.ui.dropdown.sidesingredients.selection').dropdown('setting', 'onChange', function(value, text, $selectedItem) {
+        $('.button.confirmingredients').removeClass('disabled');
+        $('.button.nextkitchencount').addClass('disabled');
+    });
+
+    $('.button.orders').click(function() {
+        $('.button.orders i').addClass('loading');
+        $.ajax({
+            type: 'GET',
+            url: $(this).attr('data-url'),
+            success: function(xhr, ajaxOptions, thrownError) {
+                $("#generated-orders").html(xhr);
+                enableGeneratedOrdersCancelButton();
+                var count = $("#generated-orders-table tbody tr").length;
+                $('.orders-count span').html(count);
+                $('.orders-count').attr('data-order-count', count);
+                $('.button.orders i').removeClass('loading');
+            },
+        });
+    });
 
     $('input[name=include_a_bill]').change(function() {
         var self = this;
         var url = $(self).data('url');
         var checked = $(self).is(':checked');
         $.ajax({
             type: (checked) ? 'POST' : 'DELETE',
@@ -33681,15 +33686,15 @@
         $('#id_override_dates').val($('#id_delivery_dates').val());
         $('#form_create_batch #id_is_submit').val("1");
         $('#form_create_batch').submit();
     });
 
     $('.order-delete').click(function() {
         var order_id = $(this).data('orderId');
-        var selector = '.ui.basic.modal.order-' + order_id;
+        var selector = '.ui.basic.modal.order-delete-' + order_id;
         $(selector).modal('show');
     });
 
     function updateOtherFieldStatus() {
         var value = $('input[name=reason_select]:checked', '#change-status-form').val();
         if (value !== 'other') {
             $('#reason_other_field textarea').attr('disabled', 'disabled');
@@ -33737,15 +33742,15 @@
                 // When approving modal, submit form
                 onApprove: function($element, modalCtntURL) {
                     var origdata = $('#change-status-form').serializeArray();
                     var origdata_o = {};
                     $.each(origdata, function(idx, ele) {
                         origdata_o[ele.name] = ele.value; // build object
                     });
-                    if (origdata_o.reason_select !== 'other') {
+                    if (origdata_o.reason_select && origdata_o.reason_select !== 'other') {
                         origdata_o.reason = origdata_o.reason_select;
                     }
                     delete origdata_o.reason_select;
                     var data = $.param(origdata_o);
 
                     $.ajax({
                         type: 'POST',
```

### Comparing `souschef-1.3.4/souschef/sous_chef/assets/js/sous-chef.min.js` & `souschef-1.3.5/souschef/sous_chef/assets/js/sous-chef.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,34 @@
-! function(e, t) {
+function enableGeneratedOrdersCancelButton() {
+    $(".ui.order.cancel.button").click(function() {
+        var i = this,
+            e = $(i).attr("data-url");
+        $.get(e, {
+            status: "C"
+        }, function(e, t) {
+            $(".ui.modal.status").html(e).modal("setting", {
+                closable: !1,
+                onApprove: function(e, t) {
+                    var n = $("#change-status-form").serializeArray();
+                    return $.ajax({
+                        type: "POST",
+                        url: $(i).attr("data-url"),
+                        data: n,
+                        success: function(e, t, n) {
+                            0 < $(e).find(".errorlist").length ? $(".ui.modal.status").html(e) : ($(".ui.modal.status").modal("hide"), location.reload())
+                        }
+                    }), !1
+                },
+                onDeny: function(e) {
+                    $(".ui.modal.status").modal("hide")
+                }
+            }).modal("setting", "autofocus", !1).modal("show")
+        })
+    })
+}! function(e, t) {
     "use strict";
     "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
         if (!e.document) throw new Error("jQuery requires a window with a document");
         return t(e)
     } : t(e)
 }("undefined" != typeof window ? window : this, function(T, e) {
     "use strict";
@@ -179,16 +205,16 @@
         var e, p, x, r, a, m, f, g, C, l, c, w, T, s, k, h, u, v, b, S = "sizzle" + 1 * new Date,
             y = n.document,
             A = 0,
             i = 0,
             D = le(),
             E = le(),
             R = le(),
-            P = le(),
-            O = function(e, t) {
+            O = le(),
+            P = function(e, t) {
                 return e === t && (c = !0), 0
             },
             F = {}.hasOwnProperty,
             t = [],
             M = t.pop,
             j = t.push,
             q = t.push,
@@ -216,16 +242,16 @@
                 TAG: new RegExp("^(" + z + "|[*])"),
                 ATTR: new RegExp("^" + $),
                 PSEUDO: new RegExp("^" + V),
                 CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + H + "*(even|odd|(([+-]|)(\\d*)n|)" + H + "*(?:([+-]|)" + H + "*(\\d+)|))" + H + "*\\)|)", "i"),
                 bool: new RegExp("^(?:" + I + ")$", "i"),
                 needsContext: new RegExp("^" + H + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + H + "*((?:-\\d)?\\d*)" + H + "*\\)|)(?=[^-]|$)", "i")
             },
-            K = /HTML$/i,
-            G = /^(?:input|select|textarea|button)$/i,
+            G = /HTML$/i,
+            K = /^(?:input|select|textarea|button)$/i,
             Z = /^h\d$/i,
             ee = /^[^{]+\{\s*\[native \w/,
             te = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
             ne = /[+~]/,
             ie = new RegExp("\\\\([\\da-f]{1,6}" + H + "?|(" + H + ")|.)", "ig"),
             oe = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
             re = function(e, t) {
@@ -260,23 +286,23 @@
                         if (9 === f) {
                             if (!(a = e.getElementById(o))) return n;
                             if (a.id === o) return n.push(a), n
                         } else if (d && (a = d.getElementById(o)) && b(e, a) && a.id === o) return n.push(a), n
                     } else {
                         if (l[2]) return q.apply(n, e.getElementsByTagName(t)), n;
                         if ((o = l[3]) && p.getElementsByClassName && e.getElementsByClassName) return q.apply(n, e.getElementsByClassName(o)), n
-                    } if (p.qsa && !P[t + " "] && (!h || !h.test(t)) && (1 !== f || "object" !== e.nodeName.toLowerCase())) {
+                    } if (p.qsa && !O[t + " "] && (!h || !h.test(t)) && (1 !== f || "object" !== e.nodeName.toLowerCase())) {
                     if (u = t, d = e, 1 === f && X.test(t)) {
                         for ((s = e.getAttribute("id")) ? s = s.replace(oe, re) : e.setAttribute("id", s = S), r = (c = m(t)).length; r--;) c[r] = "#" + s + " " + ye(c[r]);
                         u = c.join(","), d = ne.test(t) && ve(e.parentNode) || e
                     }
                     try {
                         return q.apply(n, d.querySelectorAll(u)), n
                     } catch (e) {
-                        P(t, !0)
+                        O(t, !0)
                     } finally {
                         s === S && e.removeAttribute("id")
                     }
                 }
             }
             return g(t.replace(W, "$1"), e, n, i)
         }
@@ -346,15 +372,15 @@
 
         function ve(e) {
             return e && void 0 !== e.getElementsByTagName && e
         }
         for (e in p = se.support = {}, a = se.isXML = function(e) {
                 var t = e.namespaceURI,
                     n = (e.ownerDocument || e).documentElement;
-                return !K.test(t || n && n.nodeName || "HTML")
+                return !G.test(t || n && n.nodeName || "HTML")
             }, w = se.setDocument = function(e) {
                 var t, n, i = e ? e.ownerDocument || e : y;
                 return i !== T && 9 === i.nodeType && i.documentElement && (s = (T = i).documentElement, k = !a(T), y !== T && (n = T.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", o, !1) : n.attachEvent && n.attachEvent("onunload", o)), p.attributes = ue(function(e) {
                     return e.className = "i", !e.getAttribute("className")
                 }), p.getElementsByTagName = ue(function(e) {
                     return e.appendChild(T.createComment("")), !e.getElementsByTagName("*").length
                 }), p.getElementsByClassName = ee.test(T.getElementsByClassName), p.getById = ue(function(e) {
@@ -409,15 +435,15 @@
                         i = t && t.parentNode;
                     return e === i || !(!i || 1 !== i.nodeType || !(n.contains ? n.contains(i) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(i)))
                 } : function(e, t) {
                     if (t)
                         for (; t = t.parentNode;)
                             if (t === e) return !0;
                     return !1
-                }, O = t ? function(e, t) {
+                }, P = t ? function(e, t) {
                     if (e === t) return c = !0, 0;
                     var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
                     return n || (1 & (n = (e.ownerDocument || e) === (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !p.sortDetached && t.compareDocumentPosition(e) === n ? e === T || e.ownerDocument === y && b(y, e) ? -1 : t === T || t.ownerDocument === y && b(y, t) ? 1 : l ? L(l, e) - L(l, t) : 0 : 4 & n ? -1 : 1)
                 } : function(e, t) {
                     if (e === t) return c = !0, 0;
                     var n, i = 0,
                         o = e.parentNode,
@@ -430,19 +456,19 @@
                     for (n = t; n = n.parentNode;) s.unshift(n);
                     for (; a[i] === s[i];) i++;
                     return i ? fe(a[i], s[i]) : a[i] === y ? -1 : s[i] === y ? 1 : 0
                 }), T
             }, se.matches = function(e, t) {
                 return se(e, null, null, t)
             }, se.matchesSelector = function(e, t) {
-                if ((e.ownerDocument || e) !== T && w(e), p.matchesSelector && k && !P[t + " "] && (!u || !u.test(t)) && (!h || !h.test(t))) try {
+                if ((e.ownerDocument || e) !== T && w(e), p.matchesSelector && k && !O[t + " "] && (!u || !u.test(t)) && (!h || !h.test(t))) try {
                     var n = v.call(e, t);
                     if (n || p.disconnectedMatch || e.document && 11 !== e.document.nodeType) return n
                 } catch (e) {
-                    P(t, !0)
+                    O(t, !0)
                 }
                 return 0 < se(t, T, null, [e]).length
             }, se.contains = function(e, t) {
                 return (e.ownerDocument || e) !== T && w(e), b(e, t)
             }, se.attr = function(e, t) {
                 (e.ownerDocument || e) !== T && w(e);
                 var n = x.attrHandle[t.toLowerCase()],
@@ -452,15 +478,15 @@
                 return (e + "").replace(oe, re)
             }, se.error = function(e) {
                 throw new Error("Syntax error, unrecognized expression: " + e)
             }, se.uniqueSort = function(e) {
                 var t, n = [],
                     i = 0,
                     o = 0;
-                if (c = !p.detectDuplicates, l = !p.sortStable && e.slice(0), e.sort(O), c) {
+                if (c = !p.detectDuplicates, l = !p.sortStable && e.slice(0), e.sort(P), c) {
                     for (; t = e[o++];) t === e[o] && (i = n.push(o));
                     for (; i--;) e.splice(n[i], 1)
                 }
                 return l = null, e
             }, r = se.getText = function(e) {
                 var t, n = "",
                     i = 0,
@@ -630,15 +656,15 @@
                     parent: function(e) {
                         return !x.pseudos.empty(e)
                     },
                     header: function(e) {
                         return Z.test(e.nodeName)
                     },
                     input: function(e) {
-                        return G.test(e.nodeName)
+                        return K.test(e.nodeName)
                     },
                     button: function(e) {
                         var t = e.nodeName.toLowerCase();
                         return "input" === t && "button" === e.type || "button" === t
                     },
                     text: function(e) {
                         var t;
@@ -844,15 +870,15 @@
                 for (o = J.needsContext.test(e) ? 0 : r.length; o-- && (a = r[o], !x.relative[s = a.type]);)
                     if ((l = x.find[s]) && (i = l(a.matches[0].replace(ie, d), ne.test(r[0].type) && ve(t.parentNode) || t))) {
                         if (r.splice(o, 1), !(e = i.length && ye(r))) return q.apply(n, i), n;
                         break
                     }
             }
             return (c || f(e, u))(i, t, !k, n, !t || ne.test(e) && ve(t.parentNode) || t), n
-        }, p.sortStable = S.split("").sort(O).join("") === S, p.detectDuplicates = !!c, w(), p.sortDetached = ue(function(e) {
+        }, p.sortStable = S.split("").sort(P).join("") === S, p.detectDuplicates = !!c, w(), p.sortDetached = ue(function(e) {
             return 1 & e.compareDocumentPosition(T.createElement("fieldset"))
         }), ue(function(e) {
             return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
         }) || de("type|href|height|width", function(e, t, n) {
             if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
         }), p.attributes && ue(function(e) {
             return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
@@ -883,15 +909,15 @@
     var D = S.expr.match.needsContext;
 
     function E(e, t) {
         return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
     }
     var R = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
-    function P(e, n, i) {
+    function O(e, n, i) {
         return y(n) ? S.grep(e, function(e, t) {
             return !!n.call(e, t, e) !== i
         }) : n.nodeType ? S.grep(e, function(e) {
             return e === n !== i
         }) : "string" != typeof n ? S.grep(e, function(e) {
             return -1 < o.call(n, e) !== i
         }) : S.filter(n, e, i)
@@ -909,36 +935,36 @@
                 for (t = 0; t < i; t++)
                     if (S.contains(o[t], this)) return !0
             }));
             for (n = this.pushStack([]), t = 0; t < i; t++) S.find(e, o[t], n);
             return 1 < i ? S.uniqueSort(n) : n
         },
         filter: function(e) {
-            return this.pushStack(P(this, e || [], !1))
+            return this.pushStack(O(this, e || [], !1))
         },
         not: function(e) {
-            return this.pushStack(P(this, e || [], !0))
+            return this.pushStack(O(this, e || [], !0))
         },
         is: function(e) {
-            return !!P(this, "string" == typeof e && D.test(e) ? S(e) : e || [], !1).length
+            return !!O(this, "string" == typeof e && D.test(e) ? S(e) : e || [], !1).length
         }
     });
-    var O, F = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    var P, F = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
     (S.fn.init = function(e, t, n) {
         var i, o;
         if (!e) return this;
-        if (n = n || O, "string" != typeof e) return e.nodeType ? (this[0] = e, this.length = 1, this) : y(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this);
+        if (n = n || P, "string" != typeof e) return e.nodeType ? (this[0] = e, this.length = 1, this) : y(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this);
         if (!(i = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : F.exec(e)) || !i[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
         if (i[1]) {
             if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(i[1], t && t.nodeType ? t.ownerDocument || t : k, !0)), R.test(i[1]) && S.isPlainObject(t))
                 for (i in t) y(this[i]) ? this[i](t[i]) : this.attr(i, t[i]);
             return this
         }
         return (o = k.getElementById(i[2])) && (this[0] = o, this.length = 1), this
-    }).prototype = S.fn, O = S(k);
+    }).prototype = S.fn, P = S(k);
     var M = /^(?:parents|prev(?:Until|All))/,
         j = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
@@ -1275,69 +1301,69 @@
         },
         hasData: function(e) {
             var t = e[this.expando];
             return void 0 !== t && !S.isEmptyObject(t)
         }
     };
     var J = new Q,
-        K = new Q,
-        G = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+        G = new Q,
+        K = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
         Z = /[A-Z]/g;
 
     function ee(e, t, n) {
         var i;
         if (void 0 === n && 1 === e.nodeType)
             if (i = "data-" + t.replace(Z, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(i))) {
                 try {
                     n = function(e) {
-                        return "true" === e || "false" !== e && ("null" === e ? null : e === +e + "" ? +e : G.test(e) ? JSON.parse(e) : e)
+                        return "true" === e || "false" !== e && ("null" === e ? null : e === +e + "" ? +e : K.test(e) ? JSON.parse(e) : e)
                     }(n)
                 } catch (e) {}
-                K.set(e, t, n)
+                G.set(e, t, n)
             } else n = void 0;
         return n
     }
     S.extend({
         hasData: function(e) {
-            return K.hasData(e) || J.hasData(e)
+            return G.hasData(e) || J.hasData(e)
         },
         data: function(e, t, n) {
-            return K.access(e, t, n)
+            return G.access(e, t, n)
         },
         removeData: function(e, t) {
-            K.remove(e, t)
+            G.remove(e, t)
         },
         _data: function(e, t, n) {
             return J.access(e, t, n)
         },
         _removeData: function(e, t) {
             J.remove(e, t)
         }
     }), S.fn.extend({
         data: function(n, e) {
             var t, i, o, r = this[0],
                 a = r && r.attributes;
             if (void 0 !== n) return "object" == typeof n ? this.each(function() {
-                K.set(this, n)
+                G.set(this, n)
             }) : U(this, function(e) {
                 var t;
-                if (r && void 0 === e) return void 0 !== (t = K.get(r, n)) ? t : void 0 !== (t = ee(r, n)) ? t : void 0;
+                if (r && void 0 === e) return void 0 !== (t = G.get(r, n)) ? t : void 0 !== (t = ee(r, n)) ? t : void 0;
                 this.each(function() {
-                    K.set(this, n, e)
+                    G.set(this, n, e)
                 })
             }, null, e, 1 < arguments.length, null, !0);
-            if (this.length && (o = K.get(r), 1 === r.nodeType && !J.get(r, "hasDataAttrs"))) {
+            if (this.length && (o = G.get(r), 1 === r.nodeType && !J.get(r, "hasDataAttrs"))) {
                 for (t = a.length; t--;) a[t] && 0 === (i = a[t].name).indexOf("data-") && (i = X(i.slice(5)), ee(r, i, o[i]));
                 J.set(r, "hasDataAttrs", !0)
             }
             return o
         },
         removeData: function(e) {
             return this.each(function() {
-                K.remove(this, e)
+                G.remove(this, e)
             })
         }
     }), S.extend({
         queue: function(e, t, n) {
             var i;
             if (e) return t = (t || "fx") + "queue", i = J.get(e, t), n && (!i || Array.isArray(n) ? i = J.access(e, t, S.makeArray(n)) : i.push(n)), i || []
         },
@@ -1740,16 +1766,16 @@
             if ("object" != typeof e) return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Ae), this.each(function() {
                 S.event.remove(this, e, n, t)
             });
             for (o in e) this.off(o, t, e[o]);
             return this
         }
     });
-    var Pe = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([a-z][^\/\0>\x20\t\r\n\f]*)[^>]*)\/>/gi,
-        Oe = /<script|<style|<link/i,
+    var Oe = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([a-z][^\/\0>\x20\t\r\n\f]*)[^>]*)\/>/gi,
+        Pe = /<script|<style|<link/i,
         Fe = /checked\s*(?:[^=]|=\s*.checked.)/i,
         Me = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
 
     function je(e, t) {
         return E(e, "table") && E(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
     }
 
@@ -1763,15 +1789,15 @@
 
     function Le(e, t) {
         var n, i, o, r, a, s, l, c;
         if (1 === t.nodeType) {
             if (J.hasData(e) && (r = J.access(e), a = J.set(t, r), c = r.events))
                 for (o in delete a.handle, a.events = {}, c)
                     for (n = 0, i = c[o].length; n < i; n++) S.event.add(t, o, c[o][n]);
-            K.hasData(e) && (s = K.access(e), l = S.extend({}, s), K.set(t, l))
+            G.hasData(e) && (s = G.access(e), l = S.extend({}, s), G.set(t, l))
         }
     }
 
     function Ie(n, i, o, r) {
         i = h.apply([], i);
         var e, t, a, s, l, c, u = 0,
             d = n.length,
@@ -1794,15 +1820,15 @@
 
     function He(e, t, n) {
         for (var i, o = t ? S.filter(t, e) : e, r = 0; null != (i = o[r]); r++) n || 1 !== i.nodeType || S.cleanData(he(i)), i.parentNode && (n && re(i) && ve(he(i, "script")), i.parentNode.removeChild(i));
         return e
     }
     S.extend({
         htmlPrefilter: function(e) {
-            return e.replace(Pe, "<$1></$2>")
+            return e.replace(Oe, "<$1></$2>")
         },
         clone: function(e, t, n) {
             var i, o, r, a, s, l, c, u = e.cloneNode(!0),
                 d = re(e);
             if (!(b.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || S.isXMLDoc(e)))
                 for (a = he(u), i = 0, o = (r = he(e)).length; i < o; i++) s = r[i], l = a[i], void 0, "input" === (c = l.nodeName.toLowerCase()) && fe.test(s.type) ? l.checked = s.checked : "input" !== c && "textarea" !== c || (l.defaultValue = s.defaultValue);
             if (t)
@@ -1815,15 +1841,15 @@
             for (var t, n, i, o = S.event.special, r = 0; void 0 !== (n = e[r]); r++)
                 if (Y(n)) {
                     if (t = n[J.expando]) {
                         if (t.events)
                             for (i in t.events) o[i] ? S.event.remove(n, i) : S.removeEvent(n, i, t.handle);
                         n[J.expando] = void 0
                     }
-                    n[K.expando] && (n[K.expando] = void 0)
+                    n[G.expando] && (n[G.expando] = void 0)
                 }
         }
     }), S.fn.extend({
         detach: function(e) {
             return He(this, e, !0)
         },
         remove: function(e) {
@@ -1870,15 +1896,15 @@
         },
         html: function(e) {
             return U(this, function(e) {
                 var t = this[0] || {},
                     n = 0,
                     i = this.length;
                 if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                if ("string" == typeof e && !Oe.test(e) && !ge[(pe.exec(e) || ["", ""])[1].toLowerCase()]) {
+                if ("string" == typeof e && !Pe.test(e) && !ge[(pe.exec(e) || ["", ""])[1].toLowerCase()]) {
                     e = S.htmlPrefilter(e);
                     try {
                         for (; n < i; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(he(t, !1)), t.innerHTML = e);
                         t = 0
                     } catch (e) {}
                 }
                 t && this.empty().append(e)
@@ -1910,23 +1936,23 @@
         },
         Qe = new RegExp(ie.join("|"), "i");
 
     function Je() {
         if (Be) {
             _e.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", Be.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", oe.appendChild(_e).appendChild(Be);
             var e = T.getComputedStyle(Be);
-            ze = "1%" !== e.top, We = 12 === Ke(e.marginLeft), Be.style.right = "60%", Ue = 36 === Ke(e.right), $e = 36 === Ke(e.width), Be.style.position = "absolute", Ve = 12 === Ke(Be.offsetWidth / 3), oe.removeChild(_e), Be = null
+            ze = "1%" !== e.top, We = 12 === Ge(e.marginLeft), Be.style.right = "60%", Ue = 36 === Ge(e.right), $e = 36 === Ge(e.width), Be.style.position = "absolute", Ve = 12 === Ge(Be.offsetWidth / 3), oe.removeChild(_e), Be = null
         }
     }
 
-    function Ke(e) {
+    function Ge(e) {
         return Math.round(parseFloat(e))
     }
 
-    function Ge(e, t, n) {
+    function Ke(e, t, n) {
         var i, o, r, a, s = e.style;
         return (n = n || Ye(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || re(e) || (a = S.style(e, t)), !b.pixelBoxStyles() && Xe.test(a) && Qe.test(t) && (i = s.width, o = s.minWidth, r = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = i, s.minWidth = o, s.maxWidth = r)), void 0 !== a ? a + "" : a
     }
 
     function Ze(e, t) {
         return {
             get: function() {
@@ -1989,15 +2015,15 @@
         return !i && 0 <= r && (l += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - r - l - s - .5)) || 0), l
     }
 
     function ut(e, t, n) {
         var i = Ye(e),
             o = (!b.boxSizingReliable() || n) && "border-box" === S.css(e, "boxSizing", !1, i),
             r = o,
-            a = Ge(e, t, i),
+            a = Ke(e, t, i),
             s = "offset" + t[0].toUpperCase() + t.slice(1);
         if (Xe.test(a)) {
             if (!n) return a;
             a = "auto"
         }
         return (!b.boxSizingReliable() && o || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, i)) && e.getClientRects().length && (o = "border-box" === S.css(e, "boxSizing", !1, i), (r = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + ct(e, t, n || (o ? "border" : "content"), r, i, a) + "px"
     }
@@ -2006,15 +2032,15 @@
         return new dt.prototype.init(e, t, n, i, o)
     }
     S.extend({
         cssHooks: {
             opacity: {
                 get: function(e, t) {
                     if (t) {
-                        var n = Ge(e, "opacity");
+                        var n = Ke(e, "opacity");
                         return "" === n ? "1" : n
                     }
                 }
             }
         },
         cssNumber: {
             animationIterationCount: !0,
@@ -2046,15 +2072,15 @@
                     c = e.style;
                 if (l || (t = it(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (o = a.get(e, !1, i)) ? o : c[t];
                 "string" === (r = typeof n) && (o = ne.exec(n)) && o[1] && (n = ce(e, t, o), r = "number"), null != n && n == n && ("number" !== r || l || (n += o && o[3] || (S.cssNumber[s] ? "" : "px")), b.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (c[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, i)) || (l ? c.setProperty(t, n) : c[t] = n))
             }
         },
         css: function(e, t, n, i) {
             var o, r, a, s = X(t);
-            return rt.test(t) || (t = it(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (o = a.get(e, !0, n)), void 0 === o && (o = Ge(e, t, i)), "normal" === o && t in st && (o = st[t]), "" === n || n ? (r = parseFloat(o), !0 === n || isFinite(r) ? r || 0 : o) : o
+            return rt.test(t) || (t = it(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (o = a.get(e, !0, n)), void 0 === o && (o = Ke(e, t, i)), "normal" === o && t in st && (o = st[t]), "" === n || n ? (r = parseFloat(o), !0 === n || isFinite(r) ? r || 0 : o) : o
         }
     }), S.each(["height", "width"], function(e, l) {
         S.cssHooks[l] = {
             get: function(e, t, n) {
                 if (t) return !ot.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? ut(e, l, n) : se(e, at, function() {
                     return ut(e, l, n)
                 })
@@ -2064,15 +2090,15 @@
                     r = !b.scrollboxSize() && "absolute" === o.position,
                     a = (r || n) && "border-box" === S.css(e, "boxSizing", !1, o),
                     s = n ? ct(e, l, n, a, o) : 0;
                 return a && r && (s -= Math.ceil(e["offset" + l[0].toUpperCase() + l.slice(1)] - parseFloat(o[l]) - ct(e, l, "border", !1, o) - .5)), s && (i = ne.exec(t)) && "px" !== (i[3] || "px") && (e.style[l] = t, t = S.css(e, l)), lt(0, t, s)
             }
         }
     }), S.cssHooks.marginLeft = Ze(b.reliableMarginLeft, function(e, t) {
-        if (t) return (parseFloat(Ge(e, "marginLeft")) || e.getBoundingClientRect().left - se(e, {
+        if (t) return (parseFloat(Ke(e, "marginLeft")) || e.getBoundingClientRect().left - se(e, {
             marginLeft: 0
         }, function() {
             return e.getBoundingClientRect().left
         })) + "px"
     }), S.each({
         margin: "",
         padding: "",
@@ -2486,24 +2512,24 @@
         hasClass: function(e) {
             var t, n, i = 0;
             for (t = " " + e + " "; n = this[i++];)
                 if (1 === n.nodeType && -1 < (" " + Dt(Et(n)) + " ").indexOf(t)) return !0;
             return !1
         }
     });
-    var Pt = /\r/g;
+    var Ot = /\r/g;
     S.fn.extend({
         val: function(n) {
             var i, e, o, t = this[0];
             return arguments.length ? (o = y(n), this.each(function(e) {
                 var t;
                 1 === this.nodeType && (null == (t = o ? n.call(this, e, S(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = S.map(t, function(e) {
                     return null == e ? "" : e + ""
                 })), (i = S.valHooks[this.type] || S.valHooks[this.nodeName.toLowerCase()]) && "set" in i && void 0 !== i.set(this, t, "value") || (this.value = t))
-            })) : t ? (i = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in i && void 0 !== (e = i.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(Pt, "") : null == e ? "" : e : void 0
+            })) : t ? (i = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in i && void 0 !== (e = i.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(Ot, "") : null == e ? "" : e : void 0
         }
     }), S.extend({
         valHooks: {
             option: {
                 get: function(e) {
                     var t = S.find.attr(e, "value");
                     return null != t ? t : Dt(S.text(e))
@@ -2534,15 +2560,15 @@
                 if (Array.isArray(t)) return e.checked = -1 < S.inArray(S(e).val(), t)
             }
         }, b.checkOn || (S.valHooks[this].get = function(e) {
             return null === e.getAttribute("value") ? "on" : e.value
         })
     }), b.focusin = "onfocusin" in T;
 
-    function Ot(e) {
+    function Pt(e) {
         e.stopPropagation()
     }
     var Ft = /^(?:focusinfocus|focusoutblur)$/;
     S.extend(S.event, {
         trigger: function(e, t, n, i) {
             var o, r, a, s, l, c, u, d, f = [n || k],
                 p = v.call(e, "type") ? e.type : e,
@@ -2550,15 +2576,15 @@
             if (r = d = a = n = n || k, 3 !== n.nodeType && 8 !== n.nodeType && !Ft.test(p + S.event.triggered) && (-1 < p.indexOf(".") && (p = (m = p.split(".")).shift(), m.sort()), l = p.indexOf(":") < 0 && "on" + p, (e = e[S.expando] ? e : new S.Event(p, "object" == typeof e && e)).isTrigger = i ? 2 : 3, e.namespace = m.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + m.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), u = S.event.special[p] || {}, i || !u.trigger || !1 !== u.trigger.apply(n, t))) {
                 if (!i && !u.noBubble && !g(n)) {
                     for (s = u.delegateType || p, Ft.test(s + p) || (r = r.parentNode); r; r = r.parentNode) f.push(r), a = r;
                     a === (n.ownerDocument || k) && f.push(a.defaultView || a.parentWindow || T)
                 }
                 for (o = 0;
                     (r = f[o++]) && !e.isPropagationStopped();) d = r, e.type = 1 < o ? s : u.bindType || p, (c = (J.get(r, "events") || {})[e.type] && J.get(r, "handle")) && c.apply(r, t), (c = l && r[l]) && c.apply && Y(r) && (e.result = c.apply(r, t), !1 === e.result && e.preventDefault());
-                return e.type = p, i || e.isDefaultPrevented() || u._default && !1 !== u._default.apply(f.pop(), t) || !Y(n) || l && y(n[p]) && !g(n) && ((a = n[l]) && (n[l] = null), S.event.triggered = p, e.isPropagationStopped() && d.addEventListener(p, Ot), n[p](), e.isPropagationStopped() && d.removeEventListener(p, Ot), S.event.triggered = void 0, a && (n[l] = a)), e.result
+                return e.type = p, i || e.isDefaultPrevented() || u._default && !1 !== u._default.apply(f.pop(), t) || !Y(n) || l && y(n[p]) && !g(n) && ((a = n[l]) && (n[l] = null), S.event.triggered = p, e.isPropagationStopped() && d.addEventListener(p, Pt), n[p](), e.isPropagationStopped() && d.removeEventListener(p, Pt), S.event.triggered = void 0, a && (n[l] = a)), e.result
             }
         },
         simulate: function(e, t, n) {
             var i = S.extend(new S.Event, n, {
                 type: e,
                 isSimulated: !0
             });
@@ -2666,25 +2692,25 @@
         _t = /^(?:GET|HEAD)$/,
         Bt = /^\/\//,
         Xt = {},
         Yt = {},
         Qt = "*/".concat("*"),
         Jt = k.createElement("a");
 
-    function Kt(r) {
+    function Gt(r) {
         return function(e, t) {
             "string" != typeof e && (t = e, e = "*");
             var n, i = 0,
                 o = e.toLowerCase().match(N) || [];
             if (y(t))
                 for (; n = o[i++];) "+" === n[0] ? (n = n.slice(1) || "*", (r[n] = r[n] || []).unshift(t)) : (r[n] = r[n] || []).push(t)
         }
     }
 
-    function Gt(t, o, r, a) {
+    function Kt(t, o, r, a) {
         var s = {},
             l = t === Yt;
 
         function c(e) {
             var i;
             return s[e] = !0, S.each(t[e] || [], function(e, t) {
                 var n = t(o, r, a);
@@ -2738,16 +2764,16 @@
                 url: !0,
                 context: !0
             }
         },
         ajaxSetup: function(e, t) {
             return t ? Zt(Zt(e, S.ajaxSettings), t) : Zt(S.ajaxSettings, e)
         },
-        ajaxPrefilter: Kt(Xt),
-        ajaxTransport: Kt(Yt),
+        ajaxPrefilter: Gt(Xt),
+        ajaxTransport: Gt(Yt),
         ajax: function(e, t) {
             "object" == typeof e && (t = e, e = void 0), t = t || {};
             var u, d, f, n, p, i, m, g, o, r, h = S.ajaxSetup({}, t),
                 v = h.context || h,
                 b = h.context && (v.nodeType || v.jquery) ? S(v) : S.event,
                 y = S.Deferred(),
                 x = S.Callbacks("once memory"),
@@ -2792,18 +2818,18 @@
                 i = k.createElement("a");
                 try {
                     i.href = h.url, i.href = i.href, h.crossDomain = Jt.protocol + "//" + Jt.host != i.protocol + "//" + i.host
                 } catch (e) {
                     h.crossDomain = !0
                 }
             }
-            if (h.data && h.processData && "string" != typeof h.data && (h.data = S.param(h.data, h.traditional)), Gt(Xt, h, t, w), m) return w;
+            if (h.data && h.processData && "string" != typeof h.data && (h.data = S.param(h.data, h.traditional)), Kt(Xt, h, t, w), m) return w;
             for (o in (g = S.event && h.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), h.type = h.type.toUpperCase(), h.hasContent = !_t.test(h.type), d = h.url.replace(Vt, ""), h.hasContent ? h.data && h.processData && 0 === (h.contentType || "").indexOf("application/x-www-form-urlencoded") && (h.data = h.data.replace($t, "+")) : (r = h.url.slice(d.length), h.data && (h.processData || "string" == typeof h.data) && (d += (qt.test(d) ? "&" : "?") + h.data, delete h.data), !1 === h.cache && (d = d.replace(Ut, "$1"), r = (qt.test(d) ? "&" : "?") + "_=" + jt++ + r), h.url = d + r), h.ifModified && (S.lastModified[d] && w.setRequestHeader("If-Modified-Since", S.lastModified[d]), S.etag[d] && w.setRequestHeader("If-None-Match", S.etag[d])), (h.data && h.hasContent && !1 !== h.contentType || t.contentType) && w.setRequestHeader("Content-Type", h.contentType), w.setRequestHeader("Accept", h.dataTypes[0] && h.accepts[h.dataTypes[0]] ? h.accepts[h.dataTypes[0]] + ("*" !== h.dataTypes[0] ? ", " + Qt + "; q=0.01" : "") : h.accepts["*"]), h.headers) w.setRequestHeader(o, h.headers[o]);
             if (h.beforeSend && (!1 === h.beforeSend.call(v, w, h) || m)) return w.abort();
-            if (l = "abort", x.add(h.complete), w.done(h.success), w.fail(h.error), u = Gt(Yt, h, t, w)) {
+            if (l = "abort", x.add(h.complete), w.done(h.success), w.fail(h.error), u = Kt(Yt, h, t, w)) {
                 if (w.readyState = 1, g && b.trigger("ajaxSend", [w, h]), m) return w;
                 h.async && 0 < h.timeout && (p = T.setTimeout(function() {
                     w.abort("timeout")
                 }, h.timeout));
                 try {
                     m = !1, u.send(a, c)
                 } catch (e) {
@@ -3101,15 +3127,15 @@
                 var i;
                 if (g(e) ? i = e : 9 === e.nodeType && (i = e.defaultView), void 0 === n) return i ? i[o] : e[t];
                 i ? i.scrollTo(r ? i.pageXOffset : n, r ? n : i.pageYOffset) : e[t] = n
             }, t, e, arguments.length)
         }
     }), S.each(["top", "left"], function(e, n) {
         S.cssHooks[n] = Ze(b.pixelPosition, function(e, t) {
-            if (t) return t = Ge(e, n), Xe.test(t) ? S(e).position()[n] + "px" : t
+            if (t) return t = Ke(e, n), Xe.test(t) ? S(e).position()[n] + "px" : t
         })
     }), S.each({
         Height: "height",
         Width: "width"
     }, function(a, s) {
         S.each({
             padding: "inner" + a,
@@ -3446,27 +3472,27 @@
                 return !!g.data(e, t)
             }
         }) : function(e, t, n) {
             return !!g.data(e, n[3])
         }
     })
 }(jQuery, window, document),
-function(P, e, O, F) {
+function(O, e, P, F) {
     "use strict";
-    e = void 0 !== e && e.Math == Math ? e : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), P.fn.form = function(x) {
-        var C, w = P(this),
+    e = void 0 !== e && e.Math == Math ? e : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), O.fn.form = function(x) {
+        var C, w = O(this),
             T = w.selector || "",
             k = (new Date).getTime(),
             S = [],
             A = x,
             D = arguments[1],
             E = "string" == typeof A,
             R = [].slice.call(arguments, 1);
         return w.each(function() {
-            var n, l, t, e, d, c, u, f, p, i, s, o, r, m, g, h, a = P(this),
+            var n, l, t, e, d, c, u, f, p, i, s, o, r, m, g, h, a = O(this),
                 v = this,
                 b = [],
                 y = !1;
             (h = {
                 initialize: function() {
                     h.get.settings(), E ? (g === F && h.instantiate(), h.invoke(A)) : (g !== F && g.invoke("destroy"), h.verbose("Initializing form validation", a, d), h.bindEvents(), h.set.defaults(), h.instantiate())
                 },
@@ -3479,108 +3505,108 @@
                 refresh: function() {
                     h.verbose("Refreshing selector cache"), n = a.find(f.field), l = a.find(f.group), t = a.find(f.message), a.find(f.prompt), e = a.find(f.submit), a.find(f.clear), a.find(f.reset)
                 },
                 submit: function() {
                     h.verbose("Submitting form", a), a.submit()
                 },
                 attachEvents: function(e, t) {
-                    t = t || "submit", P(e).on("click" + m, function(e) {
+                    t = t || "submit", O(e).on("click" + m, function(e) {
                         h[t](), e.preventDefault()
                     })
                 },
                 bindEvents: function() {
                     h.verbose("Attaching form events"), a.on("submit" + m, h.validate.form).on("blur" + m, f.field, h.event.field.blur).on("click" + m, f.submit, h.submit).on("click" + m, f.reset, h.reset).on("click" + m, f.clear, h.clear), d.keyboardShortcuts && a.on("keydown" + m, f.field, h.event.field.keydown), n.each(function() {
-                        var e = P(this),
+                        var e = O(this),
                             t = e.prop("type"),
                             n = h.get.changeEvent(t, e);
-                        P(this).on(n + m, h.event.field.change)
+                        O(this).on(n + m, h.event.field.change)
                     })
                 },
                 clear: function() {
                     n.each(function() {
-                        var e = P(this),
+                        var e = O(this),
                             t = e.parent(),
                             n = e.closest(l),
                             i = n.find(f.prompt),
                             o = e.data(u.defaultValue) || "",
                             r = t.is(f.uiCheckbox),
                             a = t.is(f.uiDropdown);
                         n.hasClass(p.error) && (h.verbose("Resetting error on field", n), n.removeClass(p.error), i.remove()), a ? (h.verbose("Resetting dropdown value", t, o), t.dropdown("clear")) : r ? e.prop("checked", !1) : (h.verbose("Resetting field value", e, o), e.val(""))
                     })
                 },
                 reset: function() {
                     n.each(function() {
-                        var e = P(this),
+                        var e = O(this),
                             t = e.parent(),
                             n = e.closest(l),
                             i = n.find(f.prompt),
                             o = e.data(u.defaultValue),
                             r = t.is(f.uiCheckbox),
                             a = t.is(f.uiDropdown),
                             s = n.hasClass(p.error);
                         o !== F && (s && (h.verbose("Resetting error on field", n), n.removeClass(p.error), i.remove()), a ? (h.verbose("Resetting dropdown value", t, o), t.dropdown("restore defaults")) : r ? (h.verbose("Resetting checkbox value", t, o), e.prop("checked", o)) : (h.verbose("Resetting field value", e, o), e.val(o)))
                     })
                 },
                 determine: {
                     isValid: function() {
                         var n = !0;
-                        return P.each(c, function(e, t) {
+                        return O.each(c, function(e, t) {
                             h.validate.field(t, e, !0) || (n = !1)
                         }), n
                     }
                 },
                 is: {
                     bracketedRule: function(e) {
                         return e.type && e.type.match(d.regExp.bracket)
                     },
                     shorthandFields: function(e) {
                         var t = e[Object.keys(e)[0]];
                         return h.is.shorthandRules(t)
                     },
                     shorthandRules: function(e) {
-                        return "string" == typeof e || P.isArray(e)
+                        return "string" == typeof e || O.isArray(e)
                     },
                     empty: function(e) {
                         return !e || 0 === e.length || (e.is('input[type="checkbox"]') ? !e.is(":checked") : h.is.blank(e))
                     },
                     blank: function(e) {
-                        return "" === P.trim(e.val())
+                        return "" === O.trim(e.val())
                     },
                     valid: function(e) {
                         var n = !0;
-                        return e ? (h.verbose("Checking if field is valid", e), h.validate.field(c[e], e, !1)) : (h.verbose("Checking if form is valid"), P.each(c, function(e, t) {
+                        return e ? (h.verbose("Checking if field is valid", e), h.validate.field(c[e], e, !1)) : (h.verbose("Checking if form is valid"), O.each(c, function(e, t) {
                             h.is.valid(e) || (n = !1)
                         }), n)
                     }
                 },
                 removeEvents: function() {
                     a.off(m), n.off(m), e.off(m), n.off(m)
                 },
                 event: {
                     field: {
                         keydown: function(e) {
-                            var t = P(this),
+                            var t = O(this),
                                 n = e.which,
                                 i = t.is(f.input),
                                 o = t.is(f.checkbox),
                                 r = 0 < t.closest(f.uiDropdown).length,
                                 a = 13;
                             n == 27 && (h.verbose("Escape key pressed blurring field"), t.blur()), e.ctrlKey || n != a || !i || r || o || (y || (t.one("keyup" + m, h.event.field.keyup), h.submit(), h.debug("Enter pressed on input submitting form")), y = !0)
                         },
                         keyup: function() {
                             y = !1
                         },
                         blur: function(e) {
-                            var t = P(this),
+                            var t = O(this),
                                 n = t.closest(l),
                                 i = h.get.validation(t);
                             n.hasClass(p.error) ? (h.debug("Revalidating field", t, i), i && h.validate.field(i)) : "blur" == d.on && i && h.validate.field(i)
                         },
                         change: function(e) {
-                            var t = P(this),
+                            var t = O(this),
                                 n = t.closest(l),
                                 i = h.get.validation(t);
                             i && ("change" == d.on || n.hasClass(p.error) && d.revalidate) && (clearTimeout(h.timer), h.timer = setTimeout(function() {
                                 h.debug("Revalidating field", t, h.get.validation(t)), h.validate.field(i)
                             }, d.delay))
                         }
                     }
@@ -3592,69 +3618,69 @@
                     ruleName: function(e) {
                         return h.is.bracketedRule(e) ? e.type.replace(e.type.match(d.regExp.bracket)[0], "") : e.type
                     },
                     changeEvent: function(e, t) {
                         return "checkbox" == e || "radio" == e || "hidden" == e || t.is("select") ? "change" : h.get.inputEvent()
                     },
                     inputEvent: function() {
-                        return O.createElement("input").oninput !== F ? "input" : O.createElement("input").onpropertychange !== F ? "propertychange" : "keyup"
+                        return P.createElement("input").oninput !== F ? "input" : P.createElement("input").onpropertychange !== F ? "propertychange" : "keyup"
                     },
                     fieldsFromShorthand: function(e) {
                         var i = {};
-                        return P.each(e, function(n, e) {
+                        return O.each(e, function(n, e) {
                             "string" == typeof e && (e = [e]), i[n] = {
                                 rules: []
-                            }, P.each(e, function(e, t) {
+                            }, O.each(e, function(e, t) {
                                 i[n].rules.push({
                                     type: t
                                 })
                             })
                         }), i
                     },
                     prompt: function(e, t) {
                         var n, i, o = h.get.ruleName(e),
                             r = h.get.ancillaryValue(e),
                             a = h.get.field(t.identifier),
                             s = a.val(),
-                            l = P.isFunction(e.prompt) ? e.prompt(s) : e.prompt || d.prompt[o] || d.text.unspecifiedRule,
+                            l = O.isFunction(e.prompt) ? e.prompt(s) : e.prompt || d.prompt[o] || d.text.unspecifiedRule,
                             c = -1 !== l.search("{value}"),
                             u = -1 !== l.search("{name}");
                         return c && (l = l.replace("{value}", a.val())), u && (i = 1 == (n = a.closest(f.group).find("label").eq(0)).length ? n.text() : a.prop("placeholder") || d.text.unspecifiedField, l = l.replace("{name}", i)), l = (l = l.replace("{identifier}", t.identifier)).replace("{ruleValue}", r), e.prompt || h.verbose("Using default validation prompt for type", l, o), l
                     },
                     settings: function() {
-                        if (P.isPlainObject(x)) {
+                        if (O.isPlainObject(x)) {
                             var e = Object.keys(x);
-                            0 < e.length && (x[e[0]].identifier !== F && x[e[0]].rules !== F) ? (d = P.extend(!0, {}, P.fn.form.settings, D), c = P.extend({}, P.fn.form.settings.defaults, x), h.error(d.error.oldSyntax, v), h.verbose("Extending settings from legacy parameters", c, d)) : (x.fields && h.is.shorthandFields(x.fields) && (x.fields = h.get.fieldsFromShorthand(x.fields)), d = P.extend(!0, {}, P.fn.form.settings, x), c = P.extend({}, P.fn.form.settings.defaults, d.fields), h.verbose("Extending settings", c, d))
-                        } else d = P.fn.form.settings, c = P.fn.form.settings.defaults, h.verbose("Using default form validation", c, d);
+                            0 < e.length && (x[e[0]].identifier !== F && x[e[0]].rules !== F) ? (d = O.extend(!0, {}, O.fn.form.settings, D), c = O.extend({}, O.fn.form.settings.defaults, x), h.error(d.error.oldSyntax, v), h.verbose("Extending settings from legacy parameters", c, d)) : (x.fields && h.is.shorthandFields(x.fields) && (x.fields = h.get.fieldsFromShorthand(x.fields)), d = O.extend(!0, {}, O.fn.form.settings, x), c = O.extend({}, O.fn.form.settings.defaults, d.fields), h.verbose("Extending settings", c, d))
+                        } else d = O.fn.form.settings, c = O.fn.form.settings.defaults, h.verbose("Using default form validation", c, d);
                         o = d.namespace, u = d.metadata, f = d.selector, p = d.className, i = d.regExp, s = d.error, r = "module-" + o, m = "." + o, g = a.data(r), h.refresh()
                     },
                     field: function(e) {
-                        return h.verbose("Finding field with identifier", e), e = h.escape.string(e), 0 < n.filter("#" + e).length ? n.filter("#" + e) : 0 < n.filter('[name="' + e + '"]').length ? n.filter('[name="' + e + '"]') : 0 < n.filter('[name="' + e + '[]"]').length ? n.filter('[name="' + e + '[]"]') : 0 < n.filter("[data-" + u.validate + '="' + e + '"]').length ? n.filter("[data-" + u.validate + '="' + e + '"]') : P("<input/>")
+                        return h.verbose("Finding field with identifier", e), e = h.escape.string(e), 0 < n.filter("#" + e).length ? n.filter("#" + e) : 0 < n.filter('[name="' + e + '"]').length ? n.filter('[name="' + e + '"]') : 0 < n.filter('[name="' + e + '[]"]').length ? n.filter('[name="' + e + '[]"]') : 0 < n.filter("[data-" + u.validate + '="' + e + '"]').length ? n.filter("[data-" + u.validate + '="' + e + '"]') : O("<input/>")
                     },
                     fields: function(e) {
-                        var n = P();
-                        return P.each(e, function(e, t) {
+                        var n = O();
+                        return O.each(e, function(e, t) {
                             n = n.add(h.get.field(t))
                         }), n
                     },
                     validation: function(n) {
                         var i, o;
-                        return !!c && (P.each(c, function(e, t) {
+                        return !!c && (O.each(c, function(e, t) {
                             o = t.identifier || e, h.get.field(o)[0] == n[0] && (t.identifier = o, i = t)
                         }), i || !1)
                     },
                     value: function(e) {
                         var t = [];
                         return t.push(e), h.get.values.call(v, t)[e]
                     },
                     values: function(e) {
-                        var t = P.isArray(e) ? h.get.fields(e) : n,
+                        var t = O.isArray(e) ? h.get.fields(e) : n,
                             c = {};
                         return t.each(function(e, t) {
-                            var n = P(t),
+                            var n = O(t),
                                 i = (n.prop("type"), n.prop("name")),
                                 o = n.val(),
                                 r = n.is(f.checkbox),
                                 a = n.is(f.radio),
                                 s = -1 !== i.indexOf("[]"),
                                 l = !!r && n.is(":checked");
                             i && (s ? (i = i.replace("[]", ""), c[i] || (c[i] = []), r ? l ? c[i].push(o || !0) : c[i].push(!1) : c[i].push(o)) : a ? c[i] !== F && 0 != c[i] || (c[i] = !!l && (o || !0)) : c[i] = r ? !!l && (o || !0) : o)
@@ -3673,95 +3699,95 @@
                 },
                 add: {
                     rule: function(e, t) {
                         h.add.field(e, t)
                     },
                     field: function(n, e) {
                         var i = {};
-                        h.is.shorthandRules(e) ? (e = P.isArray(e) ? e : [e], i[n] = {
+                        h.is.shorthandRules(e) ? (e = O.isArray(e) ? e : [e], i[n] = {
                             rules: []
-                        }, P.each(e, function(e, t) {
+                        }, O.each(e, function(e, t) {
                             i[n].rules.push({
                                 type: t
                             })
-                        })) : i[n] = e, c = P.extend({}, c, i), h.debug("Adding rules", i, c)
+                        })) : i[n] = e, c = O.extend({}, c, i), h.debug("Adding rules", i, c)
                     },
                     fields: function(e) {
                         var t;
-                        t = e && h.is.shorthandFields(e) ? h.get.fieldsFromShorthand(e) : e, c = P.extend({}, c, t)
+                        t = e && h.is.shorthandFields(e) ? h.get.fieldsFromShorthand(e) : e, c = O.extend({}, c, t)
                     },
                     prompt: function(e, t) {
                         var n = h.get.field(e).closest(l),
                             i = n.children(f.prompt),
                             o = 0 !== i.length;
-                        t = "string" == typeof t ? [t] : t, h.verbose("Adding field error state", e), n.addClass(p.error), d.inline && (o || (i = d.templates.prompt(t)).appendTo(n), i.html(t[0]), o ? h.verbose("Inline errors are disabled, no inline error added", e) : d.transition && P.fn.transition !== F && a.transition("is supported") ? (h.verbose("Displaying error with css transition", d.transition), i.transition(d.transition + " in", d.duration)) : (h.verbose("Displaying error with fallback javascript animation"), i.fadeIn(d.duration)))
+                        t = "string" == typeof t ? [t] : t, h.verbose("Adding field error state", e), n.addClass(p.error), d.inline && (o || (i = d.templates.prompt(t)).appendTo(n), i.html(t[0]), o ? h.verbose("Inline errors are disabled, no inline error added", e) : d.transition && O.fn.transition !== F && a.transition("is supported") ? (h.verbose("Displaying error with css transition", d.transition), i.transition(d.transition + " in", d.duration)) : (h.verbose("Displaying error with fallback javascript animation"), i.fadeIn(d.duration)))
                     },
                     errors: function(e) {
                         h.debug("Adding form error messages", e), h.set.error(), t.html(d.templates.error(e))
                     }
                 },
                 remove: {
                     rule: function(n, e) {
-                        var i = P.isArray(e) ? e : [e];
+                        var i = O.isArray(e) ? e : [e];
                         if (e == F) return h.debug("Removed all rules"), void(c[n].rules = []);
-                        c[n] != F && P.isArray(c[n].rules) && P.each(c[n].rules, function(e, t) {
+                        c[n] != F && O.isArray(c[n].rules) && O.each(c[n].rules, function(e, t) {
                             -1 !== i.indexOf(t.type) && (h.debug("Removed rule", t.type), c[n].rules.splice(e, 1))
                         })
                     },
                     field: function(e) {
-                        var t = P.isArray(e) ? e : [e];
-                        P.each(t, function(e, t) {
+                        var t = O.isArray(e) ? e : [e];
+                        O.each(t, function(e, t) {
                             h.remove.rule(t)
                         })
                     },
                     rules: function(e, n) {
-                        P.isArray(e) ? P.each(fields, function(e, t) {
+                        O.isArray(e) ? O.each(fields, function(e, t) {
                             h.remove.rule(t, n)
                         }) : h.remove.rule(e, n)
                     },
                     fields: function(e) {
                         h.remove.field(e)
                     },
                     prompt: function(e) {
                         var t = h.get.field(e).closest(l),
                             n = t.children(f.prompt);
-                        t.removeClass(p.error), d.inline && n.is(":visible") && (h.verbose("Removing prompt for field", e), d.transition && P.fn.transition !== F && a.transition("is supported") ? n.transition(d.transition + " out", d.duration, function() {
+                        t.removeClass(p.error), d.inline && n.is(":visible") && (h.verbose("Removing prompt for field", e), d.transition && O.fn.transition !== F && a.transition("is supported") ? n.transition(d.transition + " out", d.duration, function() {
                             n.remove()
                         }) : n.fadeOut(d.duration, function() {
                             n.remove()
                         }))
                     }
                 },
                 set: {
                     success: function() {
                         a.removeClass(p.error).addClass(p.success)
                     },
                     defaults: function() {
                         n.each(function() {
-                            var e = P(this),
+                            var e = O(this),
                                 t = 0 < e.filter(f.checkbox).length ? e.is(":checked") : e.val();
                             e.data(u.defaultValue, t)
                         })
                     },
                     error: function() {
                         a.removeClass(p.success).addClass(p.error)
                     },
                     value: function(e, t) {
                         var n = {};
                         return n[e] = t, h.set.values.call(v, n)
                     },
                     values: function(e) {
-                        P.isEmptyObject(e) || P.each(e, function(e, t) {
+                        O.isEmptyObject(e) || O.each(e, function(e, t) {
                             var n, i = h.get.field(e),
                                 o = i.parent(),
-                                r = P.isArray(t),
+                                r = O.isArray(t),
                                 a = o.is(f.uiCheckbox),
                                 s = o.is(f.uiDropdown),
                                 l = i.is(f.radio) && a;
-                            0 < i.length && (r && a ? (h.verbose("Selecting multiple", t, i), o.checkbox("uncheck"), P.each(t, function(e, t) {
+                            0 < i.length && (r && a ? (h.verbose("Selecting multiple", t, i), o.checkbox("uncheck"), O.each(t, function(e, t) {
                                 n = i.filter('[value="' + t + '"]'), o = n.parent(), 0 < n.length && o.checkbox("check")
                             })) : l ? (h.verbose("Selecting radio value", t, i), i.filter('[value="' + t + '"]').parent(f.uiCheckbox).checkbox("check")) : a ? (h.verbose("Setting checkbox value", t, o), !0 === t ? o.checkbox("check") : o.checkbox("uncheck")) : s ? (h.verbose("Setting dropdown value", t, o), o.dropdown("set selected", t)) : (h.verbose("Setting field value", t, i), i.val(t)))
                         })
                     }
                 },
                 validate: {
                     form: function(e, t) {
@@ -3774,37 +3800,37 @@
                     field: function(n, e, t) {
                         t = t === F || t, "string" == typeof n && (h.verbose("Validating field", n), n = c[e = n]);
                         var i = n.identifier || e,
                             o = h.get.field(i),
                             r = !!n.depends && h.get.field(n.depends),
                             a = !0,
                             s = [];
-                        return n.identifier || (h.debug("Using field name as identifier", i), n.identifier = i), o.prop("disabled") ? (h.debug("Field is disabled. Skipping", i), a = !0) : n.optional && h.is.blank(o) ? (h.debug("Field is optional and blank. Skipping", i), a = !0) : n.depends && h.is.empty(r) ? (h.debug("Field depends on another value that is not present or empty. Skipping", r), a = !0) : n.rules !== F && P.each(n.rules, function(e, t) {
+                        return n.identifier || (h.debug("Using field name as identifier", i), n.identifier = i), o.prop("disabled") ? (h.debug("Field is disabled. Skipping", i), a = !0) : n.optional && h.is.blank(o) ? (h.debug("Field is optional and blank. Skipping", i), a = !0) : n.depends && h.is.empty(r) ? (h.debug("Field depends on another value that is not present or empty. Skipping", r), a = !0) : n.rules !== F && O.each(n.rules, function(e, t) {
                             h.has.field(i) && !h.validate.rule(n, t) && (h.debug("Field is invalid", i, t.type), s.push(h.get.prompt(t, n)), a = !1)
                         }), a ? (t && (h.remove.prompt(i, s), d.onValid.call(o)), !0) : (t && (b = b.concat(s), h.add.prompt(i, s), d.onInvalid.call(o, s)), !1)
                     },
                     rule: function(e, t) {
                         var n = h.get.field(e.identifier),
                             i = (t.type, n.val()),
                             o = h.get.ancillaryValue(t),
                             r = h.get.ruleName(t),
                             a = d.rules[r];
-                        if (P.isFunction(a)) return i = i === F || "" === i || null === i ? "" : P.trim(i + ""), a.call(n, i, o);
+                        if (O.isFunction(a)) return i = i === F || "" === i || null === i ? "" : O.trim(i + ""), a.call(n, i, o);
                         h.error(s.noRule, r)
                     }
                 },
                 setting: function(e, t) {
-                    if (P.isPlainObject(e)) P.extend(!0, d, e);
+                    if (O.isPlainObject(e)) O.extend(!0, d, e);
                     else {
                         if (t === F) return d[e];
                         d[e] = t
                     }
                 },
                 internal: function(e, t) {
-                    if (P.isPlainObject(e)) P.extend(!0, h, e);
+                    if (O.isPlainObject(e)) O.extend(!0, h, e);
                     else {
                         if (t === F) return h[e];
                         h[e] = t
                     }
                 },
                 debug: function() {
                     !d.silent && d.debug && (d.performance ? h.performance.log(arguments) : (h.debug = Function.prototype.bind.call(console.info, console, d.name + ":"), h.debug.apply(console, arguments)))
@@ -3824,36 +3850,36 @@
                             Element: v,
                             "Execution Time": n
                         })), clearTimeout(h.performance.timer), h.performance.timer = setTimeout(h.performance.display, 500)
                     },
                     display: function() {
                         var e = d.name + ":",
                             n = 0;
-                        k = !1, clearTimeout(h.performance.timer), P.each(S, function(e, t) {
+                        k = !1, clearTimeout(h.performance.timer), O.each(S, function(e, t) {
                             n += t["Execution Time"]
-                        }), e += " " + n + "ms", T && (e += " '" + T + "'"), 1 < w.length && (e += " (" + w.length + ")"), (console.group !== F || console.table !== F) && 0 < S.length && (console.groupCollapsed(e), console.table ? console.table(S) : P.each(S, function(e, t) {
+                        }), e += " " + n + "ms", T && (e += " '" + T + "'"), 1 < w.length && (e += " (" + w.length + ")"), (console.group !== F || console.table !== F) && 0 < S.length && (console.groupCollapsed(e), console.table ? console.table(S) : O.each(S, function(e, t) {
                             console.log(t.Name + ": " + t["Execution Time"] + "ms")
                         }), console.groupEnd()), S = []
                     }
                 },
                 invoke: function(i, e, t) {
                     var o, r, n, a = g;
-                    return e = e || R, t = v || t, "string" == typeof i && a !== F && (i = i.split(/[\. ]/), o = i.length - 1, P.each(i, function(e, t) {
+                    return e = e || R, t = v || t, "string" == typeof i && a !== F && (i = i.split(/[\. ]/), o = i.length - 1, O.each(i, function(e, t) {
                         var n = e != o ? t + i[e + 1].charAt(0).toUpperCase() + i[e + 1].slice(1) : i;
-                        if (P.isPlainObject(a[n]) && e != o) a = a[n];
+                        if (O.isPlainObject(a[n]) && e != o) a = a[n];
                         else {
                             if (a[n] !== F) return r = a[n], !1;
-                            if (!P.isPlainObject(a[t]) || e == o) return a[t] !== F && (r = a[t]), !1;
+                            if (!O.isPlainObject(a[t]) || e == o) return a[t] !== F && (r = a[t]), !1;
                             a = a[t]
                         }
-                    })), P.isFunction(r) ? n = r.apply(t, e) : r !== F && (n = r), P.isArray(C) ? C.push(n) : C !== F ? C = [C, n] : n !== F && (C = n), r
+                    })), O.isFunction(r) ? n = r.apply(t, e) : r !== F && (n = r), O.isArray(C) ? C.push(n) : C !== F ? C = [C, n] : n !== F && (C = n), r
                 }
             }).initialize()
         }), C !== F ? C : this
-    }, P.fn.form.settings = {
+    }, O.fn.form.settings = {
         name: "Form",
         namespace: "form",
         debug: !1,
         verbose: !1,
         performance: !0,
         fields: !1,
         keyboardShortcuts: !0,
@@ -3943,73 +3969,73 @@
             method: "The method you called is not defined.",
             noRule: "There is no rule matching the one you specified",
             oldSyntax: "Starting in 2.0 forms now only take a single settings object. Validation settings converted to new syntax automatically."
         },
         templates: {
             error: function(e) {
                 var n = '<ul class="list">';
-                return P.each(e, function(e, t) {
+                return O.each(e, function(e, t) {
                     n += "<li>" + t + "</li>"
-                }), P(n += "</ul>")
+                }), O(n += "</ul>")
             },
             prompt: function(e) {
-                return P("<div/>").addClass("ui basic red pointing prompt label").html(e[0])
+                return O("<div/>").addClass("ui basic red pointing prompt label").html(e[0])
             }
         },
         rules: {
             empty: function(e) {
-                return !(e === F || "" === e || P.isArray(e) && 0 === e.length)
+                return !(e === F || "" === e || O.isArray(e) && 0 === e.length)
             },
             checked: function() {
-                return 0 < P(this).filter(":checked").length
+                return 0 < O(this).filter(":checked").length
             },
             email: function(e) {
-                return P.fn.form.settings.regExp.email.test(e)
+                return O.fn.form.settings.regExp.email.test(e)
             },
             url: function(e) {
-                return P.fn.form.settings.regExp.url.test(e)
+                return O.fn.form.settings.regExp.url.test(e)
             },
             regExp: function(e, t) {
                 if (t instanceof RegExp) return e.match(t);
-                var n, i = t.match(P.fn.form.settings.regExp.flags);
+                var n, i = t.match(O.fn.form.settings.regExp.flags);
                 return i && (t = 2 <= i.length ? i[1] : t, n = 3 <= i.length ? i[2] : ""), e.match(new RegExp(t, n))
             },
             integer: function(e, t) {
-                var n, i, o, r = P.fn.form.settings.regExp.integer;
+                var n, i, o, r = O.fn.form.settings.regExp.integer;
                 return t && -1 === ["", ".."].indexOf(t) && (-1 == t.indexOf("..") ? r.test(t) && (n = i = t - 0) : (o = t.split("..", 2), r.test(o[0]) && (n = o[0] - 0), r.test(o[1]) && (i = o[1] - 0))), r.test(e) && (n === F || n <= e) && (i === F || e <= i)
             },
             decimal: function(e) {
-                return P.fn.form.settings.regExp.decimal.test(e)
+                return O.fn.form.settings.regExp.decimal.test(e)
             },
             number: function(e) {
-                return P.fn.form.settings.regExp.number.test(e)
+                return O.fn.form.settings.regExp.number.test(e)
             },
             is: function(e, t) {
                 return t = "string" == typeof t ? t.toLowerCase() : t, (e = "string" == typeof e ? e.toLowerCase() : e) == t
             },
             isExactly: function(e, t) {
                 return e == t
             },
             not: function(e, t) {
                 return (e = "string" == typeof e ? e.toLowerCase() : e) != (t = "string" == typeof t ? t.toLowerCase() : t)
             },
             notExactly: function(e, t) {
                 return e != t
             },
             contains: function(e, t) {
-                return t = t.replace(P.fn.form.settings.regExp.escape, "\\$&"), -1 !== e.search(new RegExp(t, "i"))
+                return t = t.replace(O.fn.form.settings.regExp.escape, "\\$&"), -1 !== e.search(new RegExp(t, "i"))
             },
             containsExactly: function(e, t) {
-                return t = t.replace(P.fn.form.settings.regExp.escape, "\\$&"), -1 !== e.search(new RegExp(t))
+                return t = t.replace(O.fn.form.settings.regExp.escape, "\\$&"), -1 !== e.search(new RegExp(t))
             },
             doesntContain: function(e, t) {
-                return t = t.replace(P.fn.form.settings.regExp.escape, "\\$&"), -1 === e.search(new RegExp(t, "i"))
+                return t = t.replace(O.fn.form.settings.regExp.escape, "\\$&"), -1 === e.search(new RegExp(t, "i"))
             },
             doesntContainExactly: function(e, t) {
-                return t = t.replace(P.fn.form.settings.regExp.escape, "\\$&"), -1 === e.search(new RegExp(t))
+                return t = t.replace(O.fn.form.settings.regExp.escape, "\\$&"), -1 === e.search(new RegExp(t))
             },
             minLength: function(e, t) {
                 return e !== F && e.length >= t
             },
             length: function(e, t) {
                 return e !== F && e.length >= t
             },
@@ -4017,21 +4043,21 @@
                 return e !== F && e.length == t
             },
             maxLength: function(e, t) {
                 return e !== F && e.length <= t
             },
             match: function(e, t) {
                 var n;
-                P(this);
-                return 0 < P('[data-validate="' + t + '"]').length ? n = P('[data-validate="' + t + '"]').val() : 0 < P("#" + t).length ? n = P("#" + t).val() : 0 < P('[name="' + t + '"]').length ? n = P('[name="' + t + '"]').val() : 0 < P('[name="' + t + '[]"]').length && (n = P('[name="' + t + '[]"]')), n !== F && e.toString() == n.toString()
+                O(this);
+                return 0 < O('[data-validate="' + t + '"]').length ? n = O('[data-validate="' + t + '"]').val() : 0 < O("#" + t).length ? n = O("#" + t).val() : 0 < O('[name="' + t + '"]').length ? n = O('[name="' + t + '"]').val() : 0 < O('[name="' + t + '[]"]').length && (n = O('[name="' + t + '[]"]')), n !== F && e.toString() == n.toString()
             },
             different: function(e, t) {
                 var n;
-                P(this);
-                return 0 < P('[data-validate="' + t + '"]').length ? n = P('[data-validate="' + t + '"]').val() : 0 < P("#" + t).length ? n = P("#" + t).val() : 0 < P('[name="' + t + '"]').length ? n = P('[name="' + t + '"]').val() : 0 < P('[name="' + t + '[]"]').length && (n = P('[name="' + t + '[]"]')), n !== F && e.toString() !== n.toString()
+                O(this);
+                return 0 < O('[data-validate="' + t + '"]').length ? n = O('[data-validate="' + t + '"]').val() : 0 < O("#" + t).length ? n = O("#" + t).val() : 0 < O('[name="' + t + '"]').length ? n = O('[name="' + t + '"]').val() : 0 < O('[name="' + t + '[]"]').length && (n = O('[name="' + t + '[]"]')), n !== F && e.toString() !== n.toString()
             },
             creditCard: function(n, e) {
                 var t, i, o = {
                         visa: {
                             pattern: /^4/,
                             length: [16]
                         },
@@ -4072,22 +4098,22 @@
                             length: [16]
                         }
                     },
                     r = {},
                     a = !1,
                     s = "string" == typeof e && e.split(",");
                 if ("string" == typeof n && 0 !== n.length) {
-                    if (n = n.replace(/[\-]/g, ""), s && (P.each(s, function(e, t) {
+                    if (n = n.replace(/[\-]/g, ""), s && (O.each(s, function(e, t) {
                             (i = o[t]) && (r = {
-                                length: -1 !== P.inArray(n.length, i.length),
+                                length: -1 !== O.inArray(n.length, i.length),
                                 pattern: -1 !== n.search(i.pattern)
                             }).length && r.pattern && (a = !0)
                         }), !a)) return !1;
                     if ((t = {
-                            number: -1 !== P.inArray(n.length, o.unionPay.length),
+                            number: -1 !== O.inArray(n.length, o.unionPay.length),
                             pattern: -1 !== n.search(o.unionPay.pattern)
                         }).number && t.pattern) return !0;
                     for (var l = n.length, c = 0, u = [
                             [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
                             [0, 2, 4, 6, 8, 1, 3, 5, 7, 9]
                         ], d = 0; l--;) d += u[c][parseInt(n.charAt(l), 10)], c ^= 1;
                     return d % 10 == 0 && 0 < d
@@ -4960,15 +4986,15 @@
         template: {
             dimmer: function() {
                 return T("<div />").attr("class", "ui dimmer")
             }
         }
     }
 }(jQuery, window, document),
-function(Y, Q, J, K) {
+function(Y, Q, J, G) {
     "use strict";
     Q = void 0 !== Q && Q.Math == Math ? Q : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), Y.fn.dropdown = function(L) {
         var I, H = Y(this),
             z = Y(J),
             $ = H.selector || "",
             V = "ontouchstart" in J.documentElement,
             U = (new Date).getTime(),
@@ -4994,30 +5020,30 @@
                 T = Y(g.context),
                 k = w.find(y.text),
                 S = w.find(y.search),
                 A = w.find(y.sizer),
                 D = w.find(y.input),
                 E = w.find(y.icon),
                 R = 0 < w.prev().find(y.text).length ? w.prev().find(y.text) : w.prev(),
-                P = w.children(y.menu),
-                O = P.find(y.item),
+                O = w.children(y.menu),
+                P = O.find(y.item),
                 F = !1,
                 M = !1,
                 j = !1,
                 q = this,
                 N = w.data(C);
             m = {
                 initialize: function() {
                     m.debug("Initializing dropdown", g), m.is.alreadySetup() ? m.setup.reference() : (m.setup.layout(), g.values && m.change.values(g.values), m.refreshData(), m.save.defaults(), m.restore.selected(), m.create.id(), m.bind.events(), m.observeChanges(), m.instantiate())
                 },
                 instantiate: function() {
                     m.verbose("Storing instance of dropdown", m), N = m, w.data(C, m)
                 },
                 destroy: function() {
-                    m.verbose("Destroying previous dropdown", w), m.remove.tabbable(), w.off(x).removeData(C), P.off(x), z.off(o), m.disconnect.menuObserver(), m.disconnect.selectObserver()
+                    m.verbose("Destroying previous dropdown", w), m.remove.tabbable(), w.off(x).removeData(C), O.off(x), z.off(o), m.disconnect.menuObserver(), m.disconnect.selectObserver()
                 },
                 observeChanges: function() {
                     "MutationObserver" in Q && (a = new MutationObserver(m.event.select.mutation), s = new MutationObserver(m.event.menu.mutation), m.debug("Setting up mutation observer", a, s), m.observe.select(), m.observe.menu())
                 },
                 disconnect: {
                     menuObserver: function() {
                         s && s.disconnect()
@@ -5030,49 +5056,49 @@
                     select: function() {
                         m.has.input() && a.observe(w[0], {
                             childList: !0,
                             subtree: !0
                         })
                     },
                     menu: function() {
-                        m.has.menu() && s.observe(P[0], {
+                        m.has.menu() && s.observe(O[0], {
                             childList: !0,
                             subtree: !0
                         })
                     }
                 },
                 create: {
                     id: function() {
                         r = (Math.random().toString(16) + "000000000").substr(2, 8), o = "." + r, m.verbose("Creating unique id for element", r)
                     },
                     userChoice: function(e) {
                         var n, i, o;
                         return !!(e = e || m.get.userValues()) && (e = Y.isArray(e) ? e : [e], Y.each(e, function(e, t) {
-                            !1 === m.get.item(t) && (o = g.templates.addition(m.add.variables(c.addResult, t)), i = Y("<div />").html(o).attr("data-" + b.value, t).attr("data-" + b.text, t).addClass(h.addition).addClass(h.item), g.hideAdditions && i.addClass(h.hidden), n = n === K ? i : n.add(i), m.verbose("Creating user choices for value", t, i))
+                            !1 === m.get.item(t) && (o = g.templates.addition(m.add.variables(c.addResult, t)), i = Y("<div />").html(o).attr("data-" + b.value, t).attr("data-" + b.text, t).addClass(h.addition).addClass(h.item), g.hideAdditions && i.addClass(h.hidden), n = n === G ? i : n.add(i), m.verbose("Creating user choices for value", t, i))
                         }), n)
                     },
                     userLabels: function(e) {
                         var t = m.get.userValues();
                         t && (m.debug("Adding user labels", t), Y.each(t, function(e, t) {
                             m.verbose("Adding custom user value"), m.add.label(t, t)
                         }))
                     },
                     menu: function() {
-                        P = Y("<div />").addClass(h.menu).appendTo(w)
+                        O = Y("<div />").addClass(h.menu).appendTo(w)
                     },
                     sizer: function() {
                         A = Y("<span />").addClass(h.sizer).insertAfter(S)
                     }
                 },
                 search: function(e) {
-                    e = e !== K ? e : m.get.query(), m.verbose("Searching for query", e), m.has.minCharacters(e) ? m.filter(e) : m.hide()
+                    e = e !== G ? e : m.get.query(), m.verbose("Searching for query", e), m.has.minCharacters(e) ? m.filter(e) : m.hide()
                 },
                 select: {
                     firstUnfiltered: function() {
-                        m.verbose("Selecting first non-filtered element"), m.remove.selectedItem(), O.not(y.unselectable).not(y.addition + y.hidden).eq(0).addClass(h.selected)
+                        m.verbose("Selecting first non-filtered element"), m.remove.selectedItem(), P.not(y.unselectable).not(y.addition + y.hidden).eq(0).addClass(h.selected)
                     },
                     nextAvailable: function(e) {
                         var t = (e = e.eq(0)).nextAll(y.item).not(y.unselectable).eq(0),
                             n = e.prevAll(y.item).not(y.unselectable).eq(0);
                         0 < t.length ? (m.verbose("Moving selection to", t), t.addClass(h.selected)) : (m.verbose("Moving selection to", n), n.addClass(h.selected))
                     }
                 },
@@ -5089,42 +5115,42 @@
                         m.verbose("First request, initializing API"), w.api(e)
                     },
                     layout: function() {
                         w.is("select") && (m.setup.select(), m.setup.returnedObject()), m.has.menu() || m.create.menu(), m.is.search() && !m.has.search() && (m.verbose("Adding search input"), S = Y("<input />").addClass(h.search).prop("autocomplete", "off").insertBefore(k)), m.is.multiple() && m.is.searchSelection() && !m.has.sizer() && m.create.sizer(), g.allowTab && m.set.tabbable()
                     },
                     select: function() {
                         var e = m.get.selectValues();
-                        m.debug("Dropdown initialized on a select", e), w.is("select") && (D = w), 0 < D.parent(y.dropdown).length ? (m.debug("UI dropdown already exists. Creating dropdown menu only"), w = D.closest(y.dropdown), m.has.menu() || m.create.menu(), P = w.children(y.menu), m.setup.menu(e)) : (m.debug("Creating entire dropdown from select"), w = Y("<div />").attr("class", D.attr("class")).addClass(h.selection).addClass(h.dropdown).html(p.dropdown(e)).insertBefore(D), D.hasClass(h.multiple) && !1 === D.prop("multiple") && (m.error(f.missingMultiple), D.prop("multiple", !0)), D.is("[multiple]") && m.set.multiple(), D.prop("disabled") && (m.debug("Disabling dropdown"), w.addClass(h.disabled)), D.removeAttr("class").detach().prependTo(w)), m.refresh()
+                        m.debug("Dropdown initialized on a select", e), w.is("select") && (D = w), 0 < D.parent(y.dropdown).length ? (m.debug("UI dropdown already exists. Creating dropdown menu only"), w = D.closest(y.dropdown), m.has.menu() || m.create.menu(), O = w.children(y.menu), m.setup.menu(e)) : (m.debug("Creating entire dropdown from select"), w = Y("<div />").attr("class", D.attr("class")).addClass(h.selection).addClass(h.dropdown).html(p.dropdown(e)).insertBefore(D), D.hasClass(h.multiple) && !1 === D.prop("multiple") && (m.error(f.missingMultiple), D.prop("multiple", !0)), D.is("[multiple]") && m.set.multiple(), D.prop("disabled") && (m.debug("Disabling dropdown"), w.addClass(h.disabled)), D.removeAttr("class").detach().prependTo(w)), m.refresh()
                     },
                     menu: function(e) {
-                        P.html(p.menu(e, l)), O = P.find(y.item)
+                        O.html(p.menu(e, l)), P = O.find(y.item)
                     },
                     reference: function() {
                         m.debug("Dropdown behavior was called on select, replacing with closest dropdown"), w = w.parent(y.dropdown), N = w.data(C), q = w.get(0), m.refresh(), m.setup.returnedObject()
                     },
                     returnedObject: function() {
                         var e = H.slice(0, n),
                             t = H.slice(n + 1);
                         H = e.add(w).add(t)
                     }
                 },
                 refresh: function() {
                     m.refreshSelectors(), m.refreshData()
                 },
                 refreshItems: function() {
-                    O = P.find(y.item)
+                    P = O.find(y.item)
                 },
                 refreshSelectors: function() {
-                    m.verbose("Refreshing selector cache"), k = w.find(y.text), S = w.find(y.search), D = w.find(y.input), E = w.find(y.icon), R = 0 < w.prev().find(y.text).length ? w.prev().find(y.text) : w.prev(), P = w.children(y.menu), O = P.find(y.item)
+                    m.verbose("Refreshing selector cache"), k = w.find(y.text), S = w.find(y.search), D = w.find(y.input), E = w.find(y.icon), R = 0 < w.prev().find(y.text).length ? w.prev().find(y.text) : w.prev(), O = w.children(y.menu), P = O.find(y.item)
                 },
                 refreshData: function() {
-                    m.verbose("Refreshing cached metadata"), O.removeData(b.text).removeData(b.value)
+                    m.verbose("Refreshing cached metadata"), P.removeData(b.text).removeData(b.value)
                 },
                 clearData: function() {
-                    m.verbose("Clearing metadata"), O.removeData(b.text).removeData(b.value), w.removeData(b.defaultText).removeData(b.defaultValue).removeData(b.placeholderText)
+                    m.verbose("Clearing metadata"), P.removeData(b.text).removeData(b.value), w.removeData(b.defaultText).removeData(b.defaultValue).removeData(b.placeholderText)
                 },
                 toggle: function() {
                     m.verbose("Toggling menu visibility"), m.is.active() ? m.hide() : m.show()
                 },
                 show: function(e) {
                     if (e = Y.isFunction(e) ? e : function() {}, !m.can.show() && m.is.remote() && (m.debug("No API results retrieved, searching before show"), m.queryRemote(m.get.query(), m.show)), m.can.show() && !m.is.active()) {
                         if (m.debug("Showing dropdown"), !m.has.message() || m.has.maxSelections() || m.has.allResultsFiltered() || m.remove.message(), m.is.allFiltered()) return !0;
@@ -5138,50 +5164,50 @@
                         m.remove.visible(), e.call(q)
                     }))
                 },
                 hideOthers: function() {
                     m.verbose("Finding other dropdowns to hide"), H.not(w).has(y.menu + "." + h.visible).dropdown("hide")
                 },
                 hideMenu: function() {
-                    m.verbose("Hiding menu  instantaneously"), m.remove.active(), m.remove.visible(), P.transition("hide")
+                    m.verbose("Hiding menu  instantaneously"), m.remove.active(), m.remove.visible(), O.transition("hide")
                 },
                 hideSubMenus: function() {
-                    var e = P.children(y.item).find(y.menu);
+                    var e = O.children(y.item).find(y.menu);
                     m.verbose("Hiding sub menus", e), e.transition("hide")
                 },
                 bind: {
                     events: function() {
                         V && m.bind.touchEvents(), m.bind.keyboardEvents(), m.bind.inputEvents(), m.bind.mouseEvents()
                     },
                     touchEvents: function() {
-                        m.debug("Touch device detected binding additional touch events"), m.is.searchSelection() || m.is.single() && w.on("touchstart" + x, m.event.test.toggle), P.on("touchstart" + x, y.item, m.event.item.mouseenter)
+                        m.debug("Touch device detected binding additional touch events"), m.is.searchSelection() || m.is.single() && w.on("touchstart" + x, m.event.test.toggle), O.on("touchstart" + x, y.item, m.event.item.mouseenter)
                     },
                     keyboardEvents: function() {
                         m.verbose("Binding keyboard events"), w.on("keydown" + x, m.event.keydown), m.has.search() && w.on(m.get.inputEvent() + x, y.search, m.event.input), m.is.multiple() && z.on("keydown" + o, m.event.document.keydown)
                     },
                     inputEvents: function() {
                         m.verbose("Binding input change events"), w.on("change" + x, y.input, m.event.change)
                     },
                     mouseEvents: function() {
-                        m.verbose("Binding mouse events"), m.is.multiple() && w.on("click" + x, y.label, m.event.label.click).on("click" + x, y.remove, m.event.remove.click), m.is.searchSelection() ? (w.on("mousedown" + x, m.event.mousedown).on("mouseup" + x, m.event.mouseup).on("mousedown" + x, y.menu, m.event.menu.mousedown).on("mouseup" + x, y.menu, m.event.menu.mouseup).on("click" + x, y.icon, m.event.icon.click).on("focus" + x, y.search, m.event.search.focus).on("click" + x, y.search, m.event.search.focus).on("blur" + x, y.search, m.event.search.blur).on("click" + x, y.text, m.event.text.focus), m.is.multiple() && w.on("click" + x, m.event.click)) : ("click" == g.on ? w.on("click" + x, m.event.test.toggle) : "hover" == g.on ? w.on("mouseenter" + x, m.delay.show).on("mouseleave" + x, m.delay.hide) : w.on(g.on + x, m.toggle), w.on("click" + x, y.icon, m.event.icon.click).on("mousedown" + x, m.event.mousedown).on("mouseup" + x, m.event.mouseup).on("focus" + x, m.event.focus), m.has.menuSearch() ? w.on("blur" + x, y.search, m.event.search.blur) : w.on("blur" + x, m.event.blur)), P.on("mouseenter" + x, y.item, m.event.item.mouseenter).on("mouseleave" + x, y.item, m.event.item.mouseleave).on("click" + x, y.item, m.event.item.click)
+                        m.verbose("Binding mouse events"), m.is.multiple() && w.on("click" + x, y.label, m.event.label.click).on("click" + x, y.remove, m.event.remove.click), m.is.searchSelection() ? (w.on("mousedown" + x, m.event.mousedown).on("mouseup" + x, m.event.mouseup).on("mousedown" + x, y.menu, m.event.menu.mousedown).on("mouseup" + x, y.menu, m.event.menu.mouseup).on("click" + x, y.icon, m.event.icon.click).on("focus" + x, y.search, m.event.search.focus).on("click" + x, y.search, m.event.search.focus).on("blur" + x, y.search, m.event.search.blur).on("click" + x, y.text, m.event.text.focus), m.is.multiple() && w.on("click" + x, m.event.click)) : ("click" == g.on ? w.on("click" + x, m.event.test.toggle) : "hover" == g.on ? w.on("mouseenter" + x, m.delay.show).on("mouseleave" + x, m.delay.hide) : w.on(g.on + x, m.toggle), w.on("click" + x, y.icon, m.event.icon.click).on("mousedown" + x, m.event.mousedown).on("mouseup" + x, m.event.mouseup).on("focus" + x, m.event.focus), m.has.menuSearch() ? w.on("blur" + x, y.search, m.event.search.blur) : w.on("blur" + x, m.event.blur)), O.on("mouseenter" + x, y.item, m.event.item.mouseenter).on("mouseleave" + x, y.item, m.event.item.mouseleave).on("click" + x, y.item, m.event.item.click)
                     },
                     intent: function() {
                         m.verbose("Binding hide intent event to document"), V && z.on("touchstart" + o, m.event.test.touch).on("touchmove" + o, m.event.test.touch), z.on("click" + o, m.event.test.hide)
                     }
                 },
                 unbind: {
                     intent: function() {
                         m.verbose("Removing hide intent event from document"), V && z.off("touchstart" + o).off("touchmove" + o), z.off("click" + o)
                     }
                 },
                 filter: function(e) {
                     function t() {
                         m.is.multiple() && m.filterActive(), (e || !e && 0 == m.get.activeItem().length) && m.select.firstUnfiltered(), m.has.allResultsFiltered() ? g.onNoResults.call(q, n) ? g.allowAdditions ? g.hideAdditions && (m.verbose("User addition with no menu, setting empty style"), m.set.empty(), m.hideMenu()) : (m.verbose("All items filtered, showing message", n), m.add.message(c.noResults)) : (m.verbose("All items filtered, hiding dropdown", n), m.hideMenu()) : (m.remove.empty(), m.remove.message()), g.allowAdditions && m.add.userSuggestion(e), m.is.searchSelection() && m.can.show() && m.is.focusedOnSearch() && m.show()
                     }
-                    var n = e !== K ? e : m.get.query();
+                    var n = e !== G ? e : m.get.query();
                     g.useLabels && m.has.maxSelections() || (g.apiSettings ? m.can.useAPI() ? m.queryRemote(n, function() {
                         g.filterRemoteData && m.filterItems(n), t()
                     }) : m.error(f.noAPI) : (m.filterItems(n), t()))
                 },
                 queryRemote: function(e, n) {
                     var t = {
                         errorDuration: !1,
@@ -5202,31 +5228,31 @@
                                 values: e[l.remoteValues]
                             })) : m.add.message(c.noResults), n()
                         }
                     };
                     w.api("get request") || m.setup.api(), t = Y.extend(!0, {}, t, g.apiSettings), w.api("setting", t).api("query")
                 },
                 filterItems: function(e) {
-                    var i = e !== K ? e : m.get.query(),
+                    var i = e !== G ? e : m.get.query(),
                         o = null,
                         t = m.escape.string(i),
                         r = new RegExp("^" + t, "igm");
-                    m.has.query() && (o = [], m.verbose("Searching for matching values", i), O.each(function() {
+                    m.has.query() && (o = [], m.verbose("Searching for matching values", i), P.each(function() {
                         var e, t, n = Y(this);
                         if ("both" == g.match || "text" == g.match) {
                             if (-1 !== (e = String(m.get.choiceText(n, !1))).search(r)) return o.push(this), !0;
                             if ("exact" === g.fullTextSearch && m.exactSearch(i, e)) return o.push(this), !0;
                             if (!0 === g.fullTextSearch && m.fuzzySearch(i, e)) return o.push(this), !0
                         }
                         if ("both" == g.match || "value" == g.match) {
                             if (-1 !== (t = String(m.get.choiceValue(n, e))).search(r)) return o.push(this), !0;
                             if ("exact" === g.fullTextSearch && m.exactSearch(i, t)) return o.push(this), !0;
                             if (!0 === g.fullTextSearch && m.fuzzySearch(i, t)) return o.push(this), !0
                         }
-                    })), m.debug("Showing only matched items", i), m.remove.filteredItem(), o && O.not(o).addClass(h.filtered)
+                    })), m.debug("Showing only matched items", i), m.remove.filteredItem(), o && P.not(o).addClass(h.filtered)
                 },
                 fuzzySearch: function(e, t) {
                     var n = t.length,
                         i = e.length;
                     if (e = e.toLowerCase(), t = t.toLowerCase(), n < i) return !1;
                     if (i === n) return e === t;
                     e: for (var o = 0, r = 0; o < i; o++) {
@@ -5236,22 +5262,22 @@
                     }
                     return !0
                 },
                 exactSearch: function(e, t) {
                     return e = e.toLowerCase(), -1 < (t = t.toLowerCase()).indexOf(e)
                 },
                 filterActive: function() {
-                    g.useLabels && O.filter("." + h.active).addClass(h.filtered)
+                    g.useLabels && P.filter("." + h.active).addClass(h.filtered)
                 },
                 focusSearch: function(e) {
                     m.has.search() && !m.is.focusedOnSearch() && (e ? (w.off("focus" + x, y.search), S.focus(), w.on("focus" + x, y.search, m.event.search.focus)) : S.focus())
                 },
                 forceSelection: function() {
-                    var e = O.not(h.filtered).filter("." + h.selected).eq(0),
-                        t = O.not(h.filtered).filter("." + h.active).eq(0),
+                    var e = P.not(h.filtered).filter("." + h.selected).eq(0),
+                        t = P.not(h.filtered).filter("." + h.active).eq(0),
                         n = 0 < e.length ? e : t;
                     if (0 < n.length && !m.is.multiple()) return m.debug("Forcing partial selection to selected item", n), void m.event.item.click.call(n, {}, !0);
                     g.allowAdditions && m.set.selected(m.get.query()), m.remove.searchTerm()
                 },
                 change: {
                     values: function(e) {
                         g.allowAdditions || m.clear(), m.debug("Creating dropdown with specified values", e), m.setup.menu({
@@ -5410,33 +5436,33 @@
                                 t == v.leftArrow ? !f && !p || a ? a && (e.shiftKey ? m.verbose("Adding previous label to selection") : (m.verbose("Selecting previous label"), n.removeClass(h.active)), l && !s ? i.addClass(h.active) : i.prev(y.siblingLabel).addClass(h.active).end(), e.preventDefault()) : (m.verbose("Selecting previous label"), n.last().addClass(h.active)) : t == v.rightArrow ? (f && !a && n.first().addClass(h.active), a && (e.shiftKey ? m.verbose("Adding next label to selection") : (m.verbose("Selecting next label"), n.removeClass(h.active)), c ? u ? d ? n.removeClass(h.active) : m.focusSearch() : s ? i.next(y.siblingLabel).addClass(h.active) : i.addClass(h.active) : i.next(y.siblingLabel).addClass(h.active), e.preventDefault())) : t == v.deleteKey || t == v.backspace ? a ? (m.verbose("Removing active labels"), c && u && !d && m.focusSearch(), i.last().next(y.siblingLabel).addClass(h.active), m.remove.activeLabels(i), e.preventDefault()) : p && !a && t == v.backspace && (m.verbose("Removing last label on input backspace"), i = n.last().addClass(h.active), m.remove.activeLabels(i)) : i.removeClass(h.active)
                             }
                         }
                     },
                     keydown: function(e) {
                         var t = e.which;
                         if (m.is.inObject(t, v)) {
-                            var n, i = O.not(y.unselectable).filter("." + h.selected).eq(0),
-                                o = P.children("." + h.active).eq(0),
+                            var n, i = P.not(y.unselectable).filter("." + h.selected).eq(0),
+                                o = O.children("." + h.active).eq(0),
                                 r = 0 < i.length ? i : o,
-                                a = 0 < r.length ? r.siblings(":not(." + h.filtered + ")").addBack() : P.children(":not(." + h.filtered + ")"),
+                                a = 0 < r.length ? r.siblings(":not(." + h.filtered + ")").addBack() : O.children(":not(." + h.filtered + ")"),
                                 s = r.children(y.menu),
                                 l = r.closest(y.menu),
                                 c = l.hasClass(h.visible) || l.hasClass(h.animating) || 0 < l.parent(y.menu).length,
                                 u = 0 < s.length,
                                 d = 0 < r.length,
                                 f = 0 < r.not(y.unselectable).length,
                                 p = t == v.delimiter && g.allowAdditions && m.is.multiple();
                             if (g.allowAdditions && g.hideAdditions && (t == v.enter || p) && f && (m.verbose("Selecting item from keyboard shortcut", r), m.event.item.click.call(r, e), m.is.searchSelection() && m.remove.searchTerm()), m.is.visible()) {
-                                if (t != v.enter && !p || (t == v.enter && d && u && !g.allowCategorySelection ? (m.verbose("Pressed enter on unselectable category, opening sub menu"), t = v.rightArrow) : f && (m.verbose("Selecting item from keyboard shortcut", r), m.event.item.click.call(r, e), m.is.searchSelection() && m.remove.searchTerm()), e.preventDefault()), d && (t == v.leftArrow && l[0] !== P[0] && (m.verbose("Left key pressed, closing sub-menu"), m.animate.hide(!1, l), r.removeClass(h.selected), l.closest(y.item).addClass(h.selected), e.preventDefault()), t == v.rightArrow && u && (m.verbose("Right key pressed, opening sub-menu"), m.animate.show(!1, s), r.removeClass(h.selected), s.find(y.item).eq(0).addClass(h.selected), e.preventDefault())), t == v.upArrow) {
-                                    if (n = d && c ? r.prevAll(y.item + ":not(" + y.unselectable + ")").eq(0) : O.eq(0), a.index(n) < 0) return m.verbose("Up key pressed but reached top of current menu"), void e.preventDefault();
+                                if (t != v.enter && !p || (t == v.enter && d && u && !g.allowCategorySelection ? (m.verbose("Pressed enter on unselectable category, opening sub menu"), t = v.rightArrow) : f && (m.verbose("Selecting item from keyboard shortcut", r), m.event.item.click.call(r, e), m.is.searchSelection() && m.remove.searchTerm()), e.preventDefault()), d && (t == v.leftArrow && l[0] !== O[0] && (m.verbose("Left key pressed, closing sub-menu"), m.animate.hide(!1, l), r.removeClass(h.selected), l.closest(y.item).addClass(h.selected), e.preventDefault()), t == v.rightArrow && u && (m.verbose("Right key pressed, opening sub-menu"), m.animate.show(!1, s), r.removeClass(h.selected), s.find(y.item).eq(0).addClass(h.selected), e.preventDefault())), t == v.upArrow) {
+                                    if (n = d && c ? r.prevAll(y.item + ":not(" + y.unselectable + ")").eq(0) : P.eq(0), a.index(n) < 0) return m.verbose("Up key pressed but reached top of current menu"), void e.preventDefault();
                                     m.verbose("Up key pressed, changing active item"), r.removeClass(h.selected), n.addClass(h.selected), m.set.scrollPosition(n), g.selectOnKeydown && m.is.single() && m.set.selectedItem(n), e.preventDefault()
                                 }
                                 if (t == v.downArrow) {
-                                    if (0 === (n = d && c ? n = r.nextAll(y.item + ":not(" + y.unselectable + ")").eq(0) : O.eq(0)).length) return m.verbose("Down key pressed but reached bottom of current menu"), void e.preventDefault();
-                                    m.verbose("Down key pressed, changing active item"), O.removeClass(h.selected), n.addClass(h.selected), m.set.scrollPosition(n), g.selectOnKeydown && m.is.single() && m.set.selectedItem(n), e.preventDefault()
+                                    if (0 === (n = d && c ? n = r.nextAll(y.item + ":not(" + y.unselectable + ")").eq(0) : P.eq(0)).length) return m.verbose("Down key pressed but reached bottom of current menu"), void e.preventDefault();
+                                    m.verbose("Down key pressed, changing active item"), P.removeClass(h.selected), n.addClass(h.selected), m.set.scrollPosition(n), g.selectOnKeydown && m.is.single() && m.set.selectedItem(n), e.preventDefault()
                                 }
                                 t == v.pageUp && (m.scrollPage("up"), e.preventDefault()), t == v.pageDown && (m.scrollPage("down"), e.preventDefault()), t == v.escape && (m.verbose("Escape key pressed, closing dropdown"), m.hide())
                             } else p && e.preventDefault(), t != v.downArrow || m.is.visible() || (m.verbose("Down key pressed, showing dropdown"), m.show(), e.preventDefault())
                         } else m.has.search() || m.set.selectedLetter(String.fromCharCode(t))
                     }
                 },
                 trigger: {
@@ -5457,34 +5483,34 @@
                         return t = Y.isFunction(t) ? t : function() {}, i && !o ? (m.verbose("Triggering event", t), t(), !0) : (m.verbose("Event occurred in dropdown, canceling callback"), !1)
                     },
                     eventOnElement: function(e, t) {
                         var n = Y(e.target),
                             i = n.closest(y.siblingLabel),
                             o = J.body.contains(e.target),
                             r = 0 === w.find(i).length,
-                            a = 0 === n.closest(P).length;
+                            a = 0 === n.closest(O).length;
                         return t = Y.isFunction(t) ? t : function() {}, o && r && a ? (m.verbose("Triggering event", t), t(), !0) : (m.verbose("Event occurred in dropdown menu, canceling callback"), !1)
                     }
                 },
                 action: {
                     nothing: function() {},
                     activate: function(e, t, n) {
-                        if (t = t !== K ? t : e, m.can.activate(Y(n))) {
+                        if (t = t !== G ? t : e, m.can.activate(Y(n))) {
                             if (m.set.selected(t, Y(n)), m.is.multiple() && !m.is.allFiltered()) return;
                             m.hideAndClear()
                         }
                     },
                     select: function(e, t, n) {
-                        if (t = t !== K ? t : e, m.can.activate(Y(n))) {
+                        if (t = t !== G ? t : e, m.can.activate(Y(n))) {
                             if (m.set.value(t, e, Y(n)), m.is.multiple() && !m.is.allFiltered()) return;
                             m.hideAndClear()
                         }
                     },
                     combo: function(e, t, n) {
-                        t = t !== K ? t : e, m.set.selected(t, Y(n)), m.hideAndClear()
+                        t = t !== G ? t : e, m.set.selected(t, Y(n)), m.hideAndClear()
                     },
                     hide: function(e, t, n) {
                         m.set.value(t, e, Y(n)), m.hideAndClear()
                     }
                 },
                 get: {
                     id: function() {
@@ -5502,15 +5528,15 @@
                     text: function() {
                         return k.text()
                     },
                     query: function() {
                         return Y.trim(S.val())
                     },
                     searchWidth: function(e) {
-                        return e = e !== K ? e : S.val(), A.text(e), Math.ceil(A.width() + 1)
+                        return e = e !== G ? e : S.val(), A.text(e), Math.ceil(A.width() + 1)
                     },
                     selectionCount: function() {
                         var e = m.get.values();
                         return m.is.multiple() ? Y.isArray(e) ? e.length : 0 : "" !== m.get.value() ? 1 : 0
                     },
                     transition: function(e) {
                         return "auto" == g.transition ? m.is.upward(e) ? "slide up" : "slide down" : g.transition
@@ -5529,85 +5555,85 @@
                     caretPosition: function() {
                         var e, t, n = S.get(0);
                         return "selectionStart" in n ? n.selectionStart : J.selection ? (n.focus(), t = (e = J.selection.createRange()).text.length, e.moveStart("character", -n.value.length), e.text.length - t) : void 0
                     },
                     value: function() {
                         var e = 0 < D.length ? D.val() : w.data(b.value),
                             t = Y.isArray(e) && 1 === e.length && "" === e[0];
-                        return e === K || t ? "" : e
+                        return e === G || t ? "" : e
                     },
                     values: function() {
                         var e = m.get.value();
                         return "" === e ? "" : !m.has.selectInput() && m.is.multiple() ? "string" == typeof e ? e.split(g.delimiter) : "" : e
                     },
                     remoteValues: function() {
                         var e = m.get.values(),
                             i = !1;
                         return e && ("string" == typeof e && (e = [e]), Y.each(e, function(e, t) {
                             var n = m.read.remoteData(t);
                             m.verbose("Restoring value from session data", n, t), n && ((i = i || {})[t] = n)
                         })), i
                     },
                     choiceText: function(e, t) {
-                        if (t = t !== K ? t : g.preserveHTML, e) return 0 < e.find(y.menu).length && (m.verbose("Retrieving text of element with sub-menu"), (e = e.clone()).find(y.menu).remove(), e.find(y.menuIcon).remove()), e.data(b.text) !== K ? e.data(b.text) : t ? Y.trim(e.html()) : Y.trim(e.text())
+                        if (t = t !== G ? t : g.preserveHTML, e) return 0 < e.find(y.menu).length && (m.verbose("Retrieving text of element with sub-menu"), (e = e.clone()).find(y.menu).remove(), e.find(y.menuIcon).remove()), e.data(b.text) !== G ? e.data(b.text) : t ? Y.trim(e.html()) : Y.trim(e.text())
                     },
                     choiceValue: function(e, t) {
-                        return t = t || m.get.choiceText(e), !!e && (e.data(b.value) !== K ? String(e.data(b.value)) : "string" == typeof t ? Y.trim(t.toLowerCase()) : String(t))
+                        return t = t || m.get.choiceText(e), !!e && (e.data(b.value) !== G ? String(e.data(b.value)) : "string" == typeof t ? Y.trim(t.toLowerCase()) : String(t))
                     },
                     inputEvent: function() {
                         var e = S[0];
-                        return !!e && (e.oninput !== K ? "input" : e.onpropertychange !== K ? "propertychange" : "keyup")
+                        return !!e && (e.oninput !== G ? "input" : e.onpropertychange !== G ? "propertychange" : "keyup")
                     },
                     selectValues: function() {
                         var o = {
                             values: []
                         };
                         return w.find("option").each(function() {
                             var e = Y(this),
                                 t = e.html(),
                                 n = e.attr("disabled"),
-                                i = e.attr("value") !== K ? e.attr("value") : t;
+                                i = e.attr("value") !== G ? e.attr("value") : t;
                             "auto" === g.placeholder && "" === i ? o.placeholder = t : o.values.push({
                                 name: t,
                                 value: i,
                                 disabled: n
                             })
                         }), g.placeholder && "auto" !== g.placeholder && (m.debug("Setting placeholder value to", g.placeholder), o.placeholder = g.placeholder), g.sortSelect ? (o.values.sort(function(e, t) {
                             return e.name > t.name ? 1 : -1
                         }), m.debug("Retrieved and sorted values from select", o)) : m.debug("Retrieved values from select", o), o
                     },
                     activeItem: function() {
-                        return O.filter("." + h.active)
+                        return P.filter("." + h.active)
                     },
                     selectedItem: function() {
-                        var e = O.not(y.unselectable).filter("." + h.selected);
-                        return 0 < e.length ? e : O.eq(0)
+                        var e = P.not(y.unselectable).filter("." + h.selected);
+                        return 0 < e.length ? e : P.eq(0)
                     },
                     itemWithAdditions: function(e) {
                         var t = m.get.item(e),
                             n = m.create.userChoice(e);
                         return n && 0 < n.length && (t = 0 < t.length ? t.add(n) : n), t
                     },
                     item: function(i, o) {
                         var e, r, a = !1;
-                        return i = i !== K ? i : m.get.values() !== K ? m.get.values() : m.get.text(), e = r ? 0 < i.length : i !== K && null !== i, r = m.is.multiple() && Y.isArray(i), o = "" === i || 0 === i || (o || !1), e && O.each(function() {
+                        return i = i !== G ? i : m.get.values() !== G ? m.get.values() : m.get.text(), e = r ? 0 < i.length : i !== G && null !== i, r = m.is.multiple() && Y.isArray(i), o = "" === i || 0 === i || (o || !1), e && P.each(function() {
                             var e = Y(this),
                                 t = m.get.choiceText(e),
                                 n = m.get.choiceValue(e, t);
-                            if (null !== n && n !== K)
+                            if (null !== n && n !== G)
                                 if (r) - 1 === Y.inArray(String(n), i) && -1 === Y.inArray(t, i) || (a = a ? a.add(e) : e);
                                 else if (o) {
                                 if (m.verbose("Ambiguous dropdown value using strict type check", e, i), n === i || t === i) return a = e, !0
                             } else if (String(n) == String(i) || t == i) return m.verbose("Found select item by value", n, i), a = e, !0
                         }), a
                     }
                 },
                 check: {
                     maxSelections: function(e) {
-                        return !g.maxSelections || ((e = e !== K ? e : m.get.selectionCount()) >= g.maxSelections ? (m.debug("Maximum selection count reached"), g.useLabels && (O.addClass(h.filtered), m.add.message(c.maxSelections)), !0) : (m.verbose("No longer at maximum selection count"), m.remove.message(), m.remove.filteredItem(), m.is.searchSelection() && m.filterItems(), !1))
+                        return !g.maxSelections || ((e = e !== G ? e : m.get.selectionCount()) >= g.maxSelections ? (m.debug("Maximum selection count reached"), g.useLabels && (P.addClass(h.filtered), m.add.message(c.maxSelections)), !0) : (m.verbose("No longer at maximum selection count"), m.remove.message(), m.remove.filteredItem(), m.is.searchSelection() && m.filterItems(), !1))
                     }
                 },
                 restore: {
                     defaults: function() {
                         m.clear(), m.restore.defaultText(), m.restore.defaultValue()
                     },
                     defaultText: function() {
@@ -5615,15 +5641,15 @@
                         e === m.get.placeholderText ? (m.debug("Restoring default placeholder text", e), m.set.placeholderText(e)) : (m.debug("Restoring default text", e), m.set.text(e))
                     },
                     placeholderText: function() {
                         m.set.placeholderText()
                     },
                     defaultValue: function() {
                         var e = m.get.defaultValue();
-                        e !== K && (m.debug("Restoring default value", e), "" !== e ? (m.set.value(e), m.set.selected()) : (m.remove.activeItem(), m.remove.selectedItem()))
+                        e !== G && (m.debug("Restoring default value", e), "" !== e ? (m.set.value(e), m.set.selected()) : (m.remove.activeItem(), m.remove.selectedItem()))
                     },
                     labels: function() {
                         g.allowAdditions && (g.useLabels || (m.error(f.labels), g.useLabels = !0), m.debug("Restoring selected values"), m.create.userLabels()), m.check.maxSelections()
                     },
                     selected: function() {
                         m.restore.values(), m.is.multiple() ? (m.debug("Restoring previously selected values and labels"), m.restore.labels()) : m.debug("Restoring previously selected values")
                     },
@@ -5638,15 +5664,15 @@
                             m.add.label(e, t)
                         }))
                     }
                 },
                 read: {
                     remoteData: function(e) {
                         var t;
-                        if (Q.Storage !== K) return (t = sessionStorage.getItem(e)) !== K && t;
+                        if (Q.Storage !== G) return (t = sessionStorage.getItem(e)) !== G && t;
                         m.error(f.noStorage)
                     }
                 },
                 save: {
                     defaults: function() {
                         m.save.defaultText(), m.save.placeholderText(), m.save.defaultValue()
                     },
@@ -5659,32 +5685,32 @@
                         m.verbose("Saving default text as", e), w.data(b.defaultText, e)
                     },
                     placeholderText: function() {
                         var e;
                         !1 !== g.placeholder && k.hasClass(h.placeholder) && (e = m.get.text(), m.verbose("Saving placeholder text as", e), w.data(b.placeholderText, e))
                     },
                     remoteData: function(e, t) {
-                        Q.Storage !== K ? (m.verbose("Saving remote data to session storage", t, e), sessionStorage.setItem(t, e)) : m.error(f.noStorage)
+                        Q.Storage !== G ? (m.verbose("Saving remote data to session storage", t, e), sessionStorage.setItem(t, e)) : m.error(f.noStorage)
                     }
                 },
                 clear: function() {
                     m.is.multiple() && g.useLabels ? m.remove.labels() : (m.remove.activeItem(), m.remove.selectedItem()), m.set.placeholderText(), m.clearValue()
                 },
                 clearValue: function() {
                     m.set.value("")
                 },
                 scrollPage: function(e, t) {
                     var n, i, o = t || m.get.selectedItem(),
                         r = o.closest(y.menu),
                         a = r.outerHeight(),
                         s = r.scrollTop(),
-                        l = O.eq(0).outerHeight(),
+                        l = P.eq(0).outerHeight(),
                         c = Math.floor(a / l),
                         u = (r.prop("scrollHeight"), "up" == e ? s - l * c : s + l * c),
-                        d = O.not(y.unselectable);
+                        d = P.not(y.unselectable);
                     i = "up" == e ? d.index(o) - c : d.index(o) + c, 0 < (n = ("up" == e ? 0 <= i : i < d.length) ? d.eq(i) : "up" == e ? d.first() : d.last()).length && (m.debug("Scrolling page", e, n), o.removeClass(h.selected), n.addClass(h.selected), g.selectOnKeydown && m.is.single() && m.set.selectedItem(n), r.scrollTop(u))
                 },
                 set: {
                     filtered: function() {
                         var e = m.is.multiple(),
                             t = m.is.searchSelection(),
                             n = e && t,
@@ -5700,61 +5726,61 @@
                     loading: function() {
                         w.addClass(h.loading)
                     },
                     placeholderText: function(e) {
                         e = e || m.get.placeholderText(), m.debug("Setting placeholder text", e), m.set.text(e), k.addClass(h.placeholder)
                     },
                     tabbable: function() {
-                        m.is.searchSelection() ? (m.debug("Added tabindex to searchable dropdown"), S.val("").attr("tabindex", 0), P.attr("tabindex", -1)) : (m.debug("Added tabindex to dropdown"), w.attr("tabindex") === K && (w.attr("tabindex", 0), P.attr("tabindex", -1)))
+                        m.is.searchSelection() ? (m.debug("Added tabindex to searchable dropdown"), S.val("").attr("tabindex", 0), O.attr("tabindex", -1)) : (m.debug("Added tabindex to dropdown"), w.attr("tabindex") === G && (w.attr("tabindex", 0), O.attr("tabindex", -1)))
                     },
                     initialLoad: function() {
                         m.verbose("Setting initial load"), e = !0
                     },
                     activeItem: function(e) {
                         g.allowAdditions && 0 < e.filter(y.addition).length ? e.addClass(h.filtered) : e.addClass(h.active)
                     },
                     partialSearch: function(e) {
                         var t = m.get.query().length;
                         S.val(e.substr(0, t))
                     },
                     scrollPosition: function(e, t) {
                         var n, i, o, r, a, s;
-                        n = (e = e || m.get.selectedItem()).closest(y.menu), i = e && 0 < e.length, t = t !== K && t, e && 0 < n.length && i && (e.position().top, n.addClass(h.loading), o = (r = n.scrollTop()) - n.offset().top + e.offset().top, t || (s = r + n.height() < o + 5, a = o - 5 < r), m.debug("Scrolling to active item", o), (t || a || s) && n.scrollTop(o), n.removeClass(h.loading))
+                        n = (e = e || m.get.selectedItem()).closest(y.menu), i = e && 0 < e.length, t = t !== G && t, e && 0 < n.length && i && (e.position().top, n.addClass(h.loading), o = (r = n.scrollTop()) - n.offset().top + e.offset().top, t || (s = r + n.height() < o + 5, a = o - 5 < r), m.debug("Scrolling to active item", o), (t || a || s) && n.scrollTop(o), n.removeClass(h.loading))
                     },
                     text: function(e) {
                         "select" !== g.action && ("combo" == g.action ? (m.debug("Changing combo button text", e, R), g.preserveHTML ? R.html(e) : R.text(e)) : (e !== m.get.placeholderText() && k.removeClass(h.placeholder), m.debug("Changing text", e, k), k.removeClass(h.filtered), g.preserveHTML ? k.html(e) : k.text(e)))
                     },
                     selectedItem: function(e) {
                         var t = m.get.choiceValue(e),
                             n = m.get.choiceText(e, !1),
                             i = m.get.choiceText(e, !0);
                         m.debug("Setting user selection to item", e), m.remove.activeItem(), m.set.partialSearch(n), m.set.activeItem(e), m.set.selected(t, e), m.set.text(i)
                     },
                     selectedLetter: function(e) {
-                        var t, n = O.filter("." + h.selected),
+                        var t, n = P.filter("." + h.selected),
                             i = 0 < n.length && m.has.firstLetter(n, e),
                             o = !1;
-                        i && (t = n.nextAll(O).eq(0), m.has.firstLetter(t, e) && (o = t)), o || O.each(function() {
+                        i && (t = n.nextAll(P).eq(0), m.has.firstLetter(t, e) && (o = t)), o || P.each(function() {
                             if (m.has.firstLetter(Y(this), e)) return o = Y(this), !1
                         }), o && (m.verbose("Scrolling to next value with letter", e), m.set.scrollPosition(o), n.removeClass(h.selected), o.addClass(h.selected), g.selectOnKeydown && m.is.single() && m.set.selectedItem(o))
                     },
                     direction: function(e) {
                         "auto" == g.direction ? (m.remove.upward(), m.can.openDownward(e) ? m.remove.upward(e) : m.set.upward(e), m.is.leftward(e) || m.can.openRightward(e) || m.set.leftward(e)) : "upward" == g.direction && m.set.upward(e)
                     },
                     upward: function(e) {
                         (e || w).addClass(h.upward)
                     },
                     leftward: function(e) {
-                        (e || P).addClass(h.leftward)
+                        (e || O).addClass(h.leftward)
                     },
                     value: function(e, t, n) {
                         var i = m.escape.value(e),
                             o = 0 < D.length,
                             r = m.get.values(),
-                            a = e !== K ? String(e) : e;
+                            a = e !== G ? String(e) : e;
                         if (o) {
                             if (!g.allowReselection && a == r && (m.verbose("Skipping value update already same value", e, r), !m.is.initialLoad())) return;
                             m.is.single() && m.has.selectInput() && m.can.extendSelect() && (m.debug("Adding user option", e), m.add.optionValue(e)), m.debug("Updating input value", i, r), j = !0, D.val(i), !1 === g.fireOnInit && m.is.initialLoad() ? m.debug("Input native change event ignored on initial load") : m.trigger.change(), j = !1
                         } else m.verbose("Storing value in metadata", i, D), i !== r && w.data(b.value, a);
                         m.is.single() && g.clearable && (i ? m.set.clearable() : m.remove.clearable()), !1 === g.fireOnInit && m.is.initialLoad() ? m.verbose("No callback on initial load", g.onChange) : g.onChange.call(q, e, t, n)
                     },
                     active: function() {
@@ -5789,28 +5815,28 @@
                 add: {
                     label: function(e, t, n) {
                         var i, o = m.is.searchSelection() ? S : k,
                             r = m.escape.value(e);
                         g.ignoreCase && (r = r.toLowerCase()), i = Y("<a />").addClass(h.label).attr("data-" + b.value, r).html(p.label(r, t)), i = g.onLabelCreate.call(i, r, t), m.has.label(e) ? m.debug("User selection already exists, skipping", r) : (g.label.variation && i.addClass(g.label.variation), !0 === n ? (m.debug("Animating in label", i), i.addClass(h.hidden).insertBefore(o).transition(g.label.transition, g.label.duration)) : (m.debug("Adding selection label", i), i.insertBefore(o)))
                     },
                     message: function(e) {
-                        var t = P.children(y.message),
+                        var t = O.children(y.message),
                             n = g.templates.message(m.add.variables(e));
-                        0 < t.length ? t.html(n) : t = Y("<div/>").html(n).addClass(h.message).appendTo(P)
+                        0 < t.length ? t.html(n) : t = Y("<div/>").html(n).addClass(h.message).appendTo(O)
                     },
                     optionValue: function(e) {
                         var t = m.escape.value(e);
                         0 < D.find('option[value="' + m.escape.string(t) + '"]').length || (m.disconnect.selectObserver(), m.is.single() && (m.verbose("Removing previous user addition"), D.find("option." + h.addition).remove()), Y("<option/>").prop("value", t).addClass(h.addition).html(e).appendTo(D), m.verbose("Adding user addition as an <option>", e), m.observe.select())
                     },
                     userSuggestion: function(e) {
-                        var t, n = P.children(y.addition),
+                        var t, n = O.children(y.addition),
                             i = m.get.item(e),
                             o = i && i.not(y.addition).length,
                             r = 0 < n.length;
-                        g.useLabels && m.has.maxSelections() || ("" === e || o ? n.remove() : (r ? (n.data(b.value, e).data(b.text, e).attr("data-" + b.value, e).attr("data-" + b.text, e).removeClass(h.filtered), g.hideAdditions || (t = g.templates.addition(m.add.variables(c.addResult, e)), n.html(t)), m.verbose("Replacing user suggestion with new value", n)) : ((n = m.create.userChoice(e)).prependTo(P), m.verbose("Adding item choice to menu corresponding with user choice addition", n)), g.hideAdditions && !m.is.allFiltered() || n.addClass(h.selected).siblings().removeClass(h.selected), m.refreshItems()))
+                        g.useLabels && m.has.maxSelections() || ("" === e || o ? n.remove() : (r ? (n.data(b.value, e).data(b.text, e).attr("data-" + b.value, e).attr("data-" + b.text, e).removeClass(h.filtered), g.hideAdditions || (t = g.templates.addition(m.add.variables(c.addResult, e)), n.html(t)), m.verbose("Replacing user suggestion with new value", n)) : ((n = m.create.userChoice(e)).prependTo(O), m.verbose("Adding item choice to menu corresponding with user choice addition", n)), g.hideAdditions && !m.is.allFiltered() || n.addClass(h.selected).siblings().removeClass(h.selected), m.refreshItems()))
                     },
                     variables: function(e, t) {
                         var n, i, o = -1 !== e.search("{count}"),
                             r = -1 !== e.search("{maxCount}"),
                             a = -1 !== e.search("{term}");
                         return m.verbose("Adding templated variables to message", e), o && (n = m.get.selectionCount(), e = e.replace("{count}", n)), r && (n = m.get.selectionCount(), e = e.replace("{maxCount}", g.maxSelections)), a && (i = t || m.get.query(), e = e.replace("{term}", i)), e
                     },
@@ -5835,56 +5861,56 @@
                     initialLoad: function() {
                         e = !1
                     },
                     upward: function(e) {
                         (e || w).removeClass(h.upward)
                     },
                     leftward: function(e) {
-                        (e || P).removeClass(h.leftward)
+                        (e || O).removeClass(h.leftward)
                     },
                     visible: function() {
                         w.removeClass(h.visible)
                     },
                     activeItem: function() {
-                        O.removeClass(h.active)
+                        P.removeClass(h.active)
                     },
                     filteredItem: function() {
-                        g.useLabels && m.has.maxSelections() || (g.useLabels && m.is.multiple() ? O.not("." + h.active).removeClass(h.filtered) : O.removeClass(h.filtered), m.remove.empty())
+                        g.useLabels && m.has.maxSelections() || (g.useLabels && m.is.multiple() ? P.not("." + h.active).removeClass(h.filtered) : P.removeClass(h.filtered), m.remove.empty())
                     },
                     optionValue: function(e) {
                         var t = m.escape.value(e),
                             n = D.find('option[value="' + m.escape.string(t) + '"]');
                         0 < n.length && n.hasClass(h.addition) && (a && (a.disconnect(), m.verbose("Temporarily disconnecting mutation observer")), n.remove(), m.verbose("Removing user addition as an <option>", t), a && a.observe(D[0], {
                             childList: !0,
                             subtree: !0
                         }))
                     },
                     message: function() {
-                        P.children(y.message).remove()
+                        O.children(y.message).remove()
                     },
                     searchWidth: function() {
                         S.css("width", "")
                     },
                     searchTerm: function() {
                         m.verbose("Cleared search term"), S.val(""), m.set.filtered()
                     },
                     userAddition: function() {
-                        O.filter(y.addition).remove()
+                        P.filter(y.addition).remove()
                     },
                     selected: function(e, t) {
                         if (!(t = g.allowAdditions ? t || m.get.itemWithAdditions(e) : t || m.get.item(e))) return !1;
                         t.each(function() {
                             var e = Y(this),
                                 t = m.get.choiceText(e),
                                 n = m.get.choiceValue(e, t);
                             m.is.multiple() ? g.useLabels ? (m.remove.value(n, t, e), m.remove.label(n)) : (m.remove.value(n, t, e), 0 === m.get.selectionCount() ? m.set.placeholderText() : m.set.text(m.add.variables(c.count))) : m.remove.value(n, t, e), e.removeClass(h.filtered).removeClass(h.active), g.useLabels && e.removeClass(h.selected)
                         })
                     },
                     selectedItem: function() {
-                        O.removeClass(h.selected)
+                        P.removeClass(h.selected)
                     },
                     value: function(e, t, n) {
                         var i, o = m.get.values();
                         m.has.selectInput() ? (m.verbose("Input is <select> removing selected option", e), i = m.remove.arrayValue(e, o), m.remove.optionValue(e)) : (m.verbose("Removing from delimited values", e), i = (i = m.remove.arrayValue(e, o)).join(g.delimiter)), !1 === g.fireOnInit && m.is.initialLoad() ? m.verbose("No callback on initial load", g.onRemove) : g.onRemove.call(q, e, t, n), m.set.value(i, t, n), m.check.maxSelections()
                     },
                     arrayValue: function(t, e) {
                         return Y.isArray(e) || (e = [e]), e = Y.grep(e, function(e) {
@@ -5898,72 +5924,72 @@
                     activeLabels: function(e) {
                         e = e || w.find(y.label).filter("." + h.active), m.verbose("Removing active label selections", e), m.remove.labels(e)
                     },
                     labels: function(e) {
                         e = e || w.find(y.label), m.verbose("Removing labels", e), e.each(function() {
                             var e = Y(this),
                                 t = e.data(b.value),
-                                n = t !== K ? String(t) : t,
+                                n = t !== G ? String(t) : t,
                                 i = m.is.userValue(n);
                             !1 !== g.onLabelRemove.call(e, t) ? (m.remove.message(), i ? (m.remove.value(n), m.remove.label(n)) : m.remove.selected(n)) : m.debug("Label remove callback cancelled removal")
                         })
                     },
                     tabbable: function() {
-                        m.is.searchSelection() ? (m.debug("Searchable dropdown initialized"), S.removeAttr("tabindex")) : (m.debug("Simple selection dropdown initialized"), w.removeAttr("tabindex")), P.removeAttr("tabindex")
+                        m.is.searchSelection() ? (m.debug("Searchable dropdown initialized"), S.removeAttr("tabindex")) : (m.debug("Simple selection dropdown initialized"), w.removeAttr("tabindex")), O.removeAttr("tabindex")
                     },
                     clearable: function() {
                         E.removeClass(h.clear)
                     }
                 },
                 has: {
                     menuSearch: function() {
-                        return m.has.search() && 0 < S.closest(P).length
+                        return m.has.search() && 0 < S.closest(O).length
                     },
                     search: function() {
                         return 0 < S.length
                     },
                     sizer: function() {
                         return 0 < A.length
                     },
                     selectInput: function() {
                         return D.is("select")
                     },
                     minCharacters: function(e) {
-                        return !g.minCharacters || (e = e !== K ? String(e) : String(m.get.query())).length >= g.minCharacters
+                        return !g.minCharacters || (e = e !== G ? String(e) : String(m.get.query())).length >= g.minCharacters
                     },
                     firstLetter: function(e, t) {
                         var n;
                         return !(!e || 0 === e.length || "string" != typeof t) && (n = m.get.choiceText(e, !1), (t = t.toLowerCase()) == String(n).charAt(0).toLowerCase())
                     },
                     input: function() {
                         return 0 < D.length
                     },
                     items: function() {
-                        return 0 < O.length
+                        return 0 < P.length
                     },
                     menu: function() {
-                        return 0 < P.length
+                        return 0 < O.length
                     },
                     message: function() {
-                        return 0 !== P.children(y.message).length
+                        return 0 !== O.children(y.message).length
                     },
                     label: function(e) {
                         var t = m.escape.value(e),
                             n = w.find(y.label);
                         return g.ignoreCase && (t = t.toLowerCase()), 0 < n.filter("[data-" + b.value + '="' + m.escape.string(t) + '"]').length
                     },
                     maxSelections: function() {
                         return g.maxSelections && m.get.selectionCount() >= g.maxSelections
                     },
                     allResultsFiltered: function() {
-                        var e = O.not(y.addition);
+                        var e = P.not(y.addition);
                         return e.filter(y.unselectable).length === e.length
                     },
                     userSuggestion: function() {
-                        return 0 < P.children(y.addition).length
+                        return 0 < O.children(y.addition).length
                     },
                     query: function() {
                         return "" !== m.get.query()
                     },
                     value: function(e) {
                         return g.ignoreCase ? m.has.valueIgnoringCase(e) : m.has.valueMatchingCase(e)
                     },
@@ -5980,33 +6006,33 @@
                     }
                 },
                 is: {
                     active: function() {
                         return w.hasClass(h.active)
                     },
                     animatingInward: function() {
-                        return P.transition("is inward")
+                        return O.transition("is inward")
                     },
                     animatingOutward: function() {
-                        return P.transition("is outward")
+                        return O.transition("is outward")
                     },
                     bubbledLabelClick: function(e) {
                         return Y(e.target).is("select, input") && 0 < w.closest("label").length
                     },
                     bubbledIconClick: function(e) {
                         return 0 < Y(e.target).closest(E).length
                     },
                     alreadySetup: function() {
-                        return w.is("select") && w.parent(y.dropdown).data(C) !== K && 0 === w.prev().length
+                        return w.is("select") && w.parent(y.dropdown).data(C) !== G && 0 === w.prev().length
                     },
                     animating: function(e) {
-                        return e ? e.transition && e.transition("is animating") : P.transition && P.transition("is animating")
+                        return e ? e.transition && e.transition("is animating") : O.transition && O.transition("is animating")
                     },
                     leftward: function(e) {
-                        return (e || P).hasClass(h.leftward)
+                        return (e || O).hasClass(h.leftward)
                     },
                     disabled: function() {
                         return w.hasClass(h.disabled)
                     },
                     focused: function() {
                         return J.activeElement === w[0]
                     },
@@ -6055,15 +6081,15 @@
                     userValue: function(e) {
                         return -1 !== Y.inArray(e, m.get.userValues())
                     },
                     upward: function(e) {
                         return (e || w).hasClass(h.upward)
                     },
                     visible: function(e) {
-                        return e ? e.hasClass(h.visible) : P.hasClass(h.visible)
+                        return e ? e.hasClass(h.visible) : O.hasClass(h.visible)
                     },
                     verticallyScrollableContext: function() {
                         var e = T.get(0) !== Q && T.css("overflow-y");
                         return "auto" == e || "scroll" == e
                     },
                     horizontallyScrollableContext: function() {
                         var e = T.get(0) !== Q && T.css("overflow-X");
@@ -6071,15 +6097,15 @@
                     }
                 },
                 can: {
                     activate: function(e) {
                         return !!g.useLabels || (!m.has.maxSelections() || !(!m.has.maxSelections() || !e.hasClass(h.active)))
                     },
                     openDownward: function(e) {
-                        var t, n, i = e || P,
+                        var t, n, i = e || O,
                             o = !0;
                         return i.addClass(h.loading), n = {
                             context: {
                                 offset: T.get(0) === Q ? {
                                     top: 0,
                                     left: 0
                                 } : T.offset(),
@@ -6092,15 +6118,15 @@
                             }
                         }, m.is.verticallyScrollableContext() && (n.menu.offset.top += n.context.scrollTop), o = (t = {
                             above: n.context.scrollTop <= n.menu.offset.top - n.context.offset.top - n.menu.height,
                             below: n.context.scrollTop + n.context.height >= n.menu.offset.top - n.context.offset.top + n.menu.height
                         }).below ? (m.verbose("Dropdown can fit in context downward", t), !0) : t.below || t.above ? (m.verbose("Dropdown cannot fit below, opening upward", t), !1) : (m.verbose("Dropdown cannot fit in either direction, favoring downward", t), !0), i.removeClass(h.loading), o
                     },
                     openRightward: function(e) {
-                        var t, n, i = e || P,
+                        var t, n, i = e || O,
                             o = !0;
                         return i.addClass(h.loading), n = {
                             context: {
                                 offset: T.get(0) === Q ? {
                                     top: 0,
                                     left: 0
                                 } : T.offset(),
@@ -6119,42 +6145,42 @@
                     extendSelect: function() {
                         return g.allowAdditions || g.apiSettings
                     },
                     show: function() {
                         return !m.is.disabled() && (m.has.items() || m.has.message())
                     },
                     useAPI: function() {
-                        return Y.fn.api !== K
+                        return Y.fn.api !== G
                     }
                 },
                 animate: {
                     show: function(e, t) {
-                        var n, i = t || P,
+                        var n, i = t || O,
                             o = t ? function() {} : function() {
                                 m.hideSubMenus(), m.hideOthers(), m.set.active()
                             };
-                        e = Y.isFunction(e) ? e : function() {}, m.verbose("Doing menu show animation", i), m.set.direction(t), n = m.get.transition(t), m.is.selection() && m.set.scrollPosition(m.get.selectedItem(), !0), (m.is.hidden(i) || m.is.animating(i)) && ("none" == n ? (o(), i.transition("show"), e.call(q)) : Y.fn.transition !== K && w.transition("is supported") ? i.transition({
+                        e = Y.isFunction(e) ? e : function() {}, m.verbose("Doing menu show animation", i), m.set.direction(t), n = m.get.transition(t), m.is.selection() && m.set.scrollPosition(m.get.selectedItem(), !0), (m.is.hidden(i) || m.is.animating(i)) && ("none" == n ? (o(), i.transition("show"), e.call(q)) : Y.fn.transition !== G && w.transition("is supported") ? i.transition({
                             animation: n + " in",
                             debug: g.debug,
                             verbose: g.verbose,
                             duration: g.duration,
                             queue: !0,
                             onStart: o,
                             onComplete: function() {
                                 e.call(q)
                             }
                         }) : m.error(f.noTransition, n))
                     },
                     hide: function(e, t) {
-                        var n = t || P,
+                        var n = t || O,
                             i = (t ? g.duration : g.duration, t ? function() {} : function() {
                                 m.can.click() && m.unbind.intent(), m.remove.active()
                             }),
                             o = m.get.transition(t);
-                        e = Y.isFunction(e) ? e : function() {}, (m.is.visible(n) || m.is.animating(n)) && (m.verbose("Doing menu hide animation", n), "none" == o ? (i(), n.transition("hide"), e.call(q)) : Y.fn.transition !== K && w.transition("is supported") ? n.transition({
+                        e = Y.isFunction(e) ? e : function() {}, (m.is.visible(n) || m.is.animating(n)) && (m.verbose("Doing menu hide animation", n), "none" == o ? (i(), n.transition("hide"), e.call(q)) : Y.fn.transition !== G && w.transition("is supported") ? n.transition({
                             animation: o + " out",
                             duration: g.duration,
                             debug: g.debug,
                             verbose: g.verbose,
                             queue: !1,
                             onStart: i,
                             onComplete: function() {
@@ -6190,22 +6216,22 @@
                     string: function(e) {
                         return (e = String(e)).replace(d.escape, "\\$&")
                     }
                 },
                 setting: function(e, t) {
                     if (m.debug("Changing setting", e, t), Y.isPlainObject(e)) Y.extend(!0, g, e);
                     else {
-                        if (t === K) return g[e];
+                        if (t === G) return g[e];
                         Y.isPlainObject(g[e]) ? Y.extend(!0, g[e], t) : g[e] = t
                     }
                 },
                 internal: function(e, t) {
                     if (Y.isPlainObject(e)) Y.extend(!0, m, e);
                     else {
-                        if (t === K) return m[e];
+                        if (t === G) return m[e];
                         m[e] = t
                     }
                 },
                 debug: function() {
                     !g.silent && g.debug && (g.performance ? m.performance.log(arguments) : (m.debug = Function.prototype.bind.call(console.info, console, g.name + ":"), m.debug.apply(console, arguments)))
                 },
                 verbose: function() {
@@ -6225,33 +6251,33 @@
                         })), clearTimeout(m.performance.timer), m.performance.timer = setTimeout(m.performance.display, 500)
                     },
                     display: function() {
                         var e = g.name + ":",
                             n = 0;
                         U = !1, clearTimeout(m.performance.timer), Y.each(W, function(e, t) {
                             n += t["Execution Time"]
-                        }), e += " " + n + "ms", $ && (e += " '" + $ + "'"), (console.group !== K || console.table !== K) && 0 < W.length && (console.groupCollapsed(e), console.table ? console.table(W) : Y.each(W, function(e, t) {
+                        }), e += " " + n + "ms", $ && (e += " '" + $ + "'"), (console.group !== G || console.table !== G) && 0 < W.length && (console.groupCollapsed(e), console.table ? console.table(W) : Y.each(W, function(e, t) {
                             console.log(t.Name + ": " + t["Execution Time"] + "ms")
                         }), console.groupEnd()), W = []
                     }
                 },
                 invoke: function(i, e, t) {
                     var o, r, n, a = N;
-                    return e = e || X, t = q || t, "string" == typeof i && a !== K && (i = i.split(/[\. ]/), o = i.length - 1, Y.each(i, function(e, t) {
+                    return e = e || X, t = q || t, "string" == typeof i && a !== G && (i = i.split(/[\. ]/), o = i.length - 1, Y.each(i, function(e, t) {
                         var n = e != o ? t + i[e + 1].charAt(0).toUpperCase() + i[e + 1].slice(1) : i;
                         if (Y.isPlainObject(a[n]) && e != o) a = a[n];
                         else {
-                            if (a[n] !== K) return r = a[n], !1;
-                            if (!Y.isPlainObject(a[t]) || e == o) return a[t] !== K ? r = a[t] : m.error(f.method, i), !1;
+                            if (a[n] !== G) return r = a[n], !1;
+                            if (!Y.isPlainObject(a[t]) || e == o) return a[t] !== G ? r = a[t] : m.error(f.method, i), !1;
                             a = a[t]
                         }
-                    })), Y.isFunction(r) ? n = r.apply(t, e) : r !== K && (n = r), Y.isArray(I) ? I.push(n) : I !== K ? I = [I, n] : n !== K && (I = n), r
+                    })), Y.isFunction(r) ? n = r.apply(t, e) : r !== G && (n = r), Y.isArray(I) ? I.push(n) : I !== G ? I = [I, n] : n !== G && (I = n), r
                 }
-            }, B ? (N === K && m.initialize(), m.invoke(_)) : (N !== K && N.invoke("destroy"), m.initialize())
-        }), I !== K ? I : H
+            }, B ? (N === G && m.initialize(), m.invoke(_)) : (N !== G && N.invoke("destroy"), m.initialize())
+        }), I !== G ? I : H
     }, Y.fn.dropdown.settings = {
         silent: !1,
         debug: !1,
         verbose: !1,
         performance: !0,
         on: "click",
         action: "activate",
@@ -6761,16 +6787,16 @@
         var T, e = j(this),
             k = j(q),
             S = j(N),
             A = j("body"),
             D = e.selector || "",
             E = (new Date).getTime(),
             R = [],
-            P = w,
-            O = "string" == typeof P,
+            O = w,
+            P = "string" == typeof O,
             F = [].slice.call(arguments, 1),
             M = q.requestAnimationFrame || q.mozRequestAnimationFrame || q.webkitRequestAnimationFrame || q.msRequestAnimationFrame || function(e) {
                 setTimeout(e, 0)
             };
         return e.each(function() {
             var n, i, e, o, r, t, a, s, l, c = j.isPlainObject(w) ? j.extend(!0, {}, j.fn.modal.settings, w) : j.extend({}, j.fn.modal.settings),
                 u = c.selector,
@@ -7136,15 +7162,15 @@
                         else {
                             if (a[n] !== L) return r = a[n], !1;
                             if (!j.isPlainObject(a[t]) || e == o) return a[t] !== L && (r = a[t]), !1;
                             a = a[t]
                         }
                     })), j.isFunction(r) ? n = r.apply(t, e) : r !== L && (n = r), j.isArray(T) ? T.push(n) : T !== L ? T = [T, n] : n !== L && (T = n), r
                 }
-            }, O ? (x === L && l.initialize(), l.invoke(P)) : (x !== L && x.invoke("destroy"), l.initialize())
+            }, P ? (x === L && l.initialize(), l.invoke(O)) : (x !== L && x.invoke("destroy"), l.initialize())
         }), T !== L ? T : this
     }, j.fn.modal.settings = {
         name: "Modal",
         namespace: "modal",
         useFlex: "auto",
         offset: 0,
         silent: !1,
@@ -7381,16 +7407,16 @@
     "use strict";
     N = void 0 !== N && N.Math == Math ? N : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), q.fn.popup = function(k) {
         var S, e = q(this),
             A = q(L),
             D = q(N),
             E = q("body"),
             R = e.selector || "",
-            P = (new Date).getTime(),
-            O = [],
+            O = (new Date).getTime(),
+            P = [],
             F = k,
             M = "string" == typeof F,
             j = [].slice.call(arguments, 1);
         return e.each(function() {
             var u, c, e, t, n, d, f = q.isPlainObject(k) ? q.extend(!0, {}, q.fn.popup.settings, k) : q.extend({}, q.fn.popup.settings),
                 o = f.selector,
                 p = f.className,
@@ -7901,29 +7927,29 @@
                 },
                 error: function() {
                     f.silent || (d.error = Function.prototype.bind.call(console.error, console, f.name + ":"), d.error.apply(console, arguments))
                 },
                 performance: {
                     log: function(e) {
                         var t, n;
-                        f.performance && (n = (t = (new Date).getTime()) - (P || t), P = t, O.push({
+                        f.performance && (n = (t = (new Date).getTime()) - (O || t), O = t, P.push({
                             Name: e[0],
                             Arguments: [].slice.call(e, 1) || "",
                             Element: w,
                             "Execution Time": n
                         })), clearTimeout(d.performance.timer), d.performance.timer = setTimeout(d.performance.display, 500)
                     },
                     display: function() {
                         var e = f.name + ":",
                             n = 0;
-                        P = !1, clearTimeout(d.performance.timer), q.each(O, function(e, t) {
+                        O = !1, clearTimeout(d.performance.timer), q.each(P, function(e, t) {
                             n += t["Execution Time"]
-                        }), e += " " + n + "ms", R && (e += " '" + R + "'"), (console.group !== I || console.table !== I) && 0 < O.length && (console.groupCollapsed(e), console.table ? console.table(O) : q.each(O, function(e, t) {
+                        }), e += " " + n + "ms", R && (e += " '" + R + "'"), (console.group !== I || console.table !== I) && 0 < P.length && (console.groupCollapsed(e), console.table ? console.table(P) : q.each(P, function(e, t) {
                             console.log(t.Name + ": " + t["Execution Time"] + "ms")
-                        }), console.groupEnd()), O = []
+                        }), console.groupEnd()), P = []
                     }
                 },
                 invoke: function(i, e, t) {
                     var o, r, n, a = T;
                     return e = e || j, t = w || t, "string" == typeof i && a !== I && (i = i.split(/[\. ]/), o = i.length - 1, q.each(i, function(e, t) {
                         var n = e != o ? t + i[e + 1].charAt(0).toUpperCase() + i[e + 1].slice(1) : i;
                         if (q.isPlainObject(a[n]) && e != o) a = a[n];
@@ -8617,17 +8643,17 @@
             icon: function(e) {
                 for (var t = 1, n = ""; t <= e;) n += '<i class="icon"></i>', t++;
                 return n
             }
         }
     }
 }(jQuery, window, document),
-function(R, P, O, F) {
+function(R, O, P, F) {
     "use strict";
-    P = void 0 !== P && P.Math == Math ? P : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), R.fn.search = function(l) {
+    O = void 0 !== O && O.Math == Math ? O : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), R.fn.search = function(l) {
         var C, w = R(this),
             T = w.selector || "",
             k = (new Date).getTime(),
             S = [],
             A = l,
             D = "string" == typeof A,
             E = [].slice.call(arguments, 1);
@@ -8688,15 +8714,15 @@
                             f.can.show() && f.showResults()
                         })
                     },
                     blur: function(e) {
                         function t() {
                             f.cancel.query(), f.remove.focus(), f.timer = setTimeout(f.hideResults, c.hideDelay)
                         }
-                        var n = O.activeElement === this;
+                        var n = P.activeElement === this;
                         n || (x = !1, f.resultsClicked ? (f.debug("Determining if user action caused search to close"), h.one("click.close" + i, m.results, function(e) {
                             f.is.inMessage(e) || y ? v.focus() : (y = !1, f.is.animating() || f.is.hidden() || t())
                         })) : (f.debug("Input blurred without user action, closing results"), t()))
                     },
                     result: {
                         mousedown: function() {
                             f.resultsClicked = !0
@@ -8711,15 +8737,15 @@
                                 i = t.is("a[href]") ? t : t.find("a[href]").eq(0),
                                 o = i.attr("href") || !1,
                                 r = i.attr("target") || !1,
                                 a = (n.html(), 0 < n.length && n.text()),
                                 s = f.get.results(),
                                 l = t.data(u.result) || f.get.result(a, s);
                             if (R.isFunction(c.onSelect) && !1 === c.onSelect.call(b, l, s)) return f.debug("Custom onSelect callback cancelled default select action"), void(y = !0);
-                            f.hideResults(), a && f.set.value(a), o && (f.verbose("Opening search link found in result", i), "_blank" == r || e.ctrlKey ? P.open(o) : P.location.href = o)
+                            f.hideResults(), a && f.set.value(a), o && (f.verbose("Opening search link found in result", i), "_blank" == r || e.ctrlKey ? O.open(o) : O.location.href = o)
                         }
                     }
                 },
                 handleKeyboard: function(e) {
                     var t, n = h.find(m.result),
                         i = h.find(m.category),
                         o = n.filter("." + p.active),
@@ -8775,15 +8801,15 @@
                     },
                     hidden: function() {
                         return o.hasClass(p.hidden)
                     },
                     inMessage: function(e) {
                         if (e.target) {
                             var t = R(e.target);
-                            return R.contains(O.documentElement, e.target) && 0 < t.closest(m.message).length
+                            return R.contains(P.documentElement, e.target) && 0 < t.closest(m.message).length
                         }
                     },
                     empty: function() {
                         return "" === o.html()
                     },
                     visible: function() {
                         return 0 < o.filter(":visible").length
@@ -9591,16 +9617,16 @@
             T = M(q),
             k = M("html"),
             S = M("head"),
             A = e.selector || "",
             D = (new Date).getTime(),
             E = [],
             R = x,
-            P = "string" == typeof R,
-            O = [].slice.call(arguments, 1),
+            O = "string" == typeof R,
+            P = [].slice.call(arguments, 1),
             F = j.requestAnimationFrame || j.mozRequestAnimationFrame || j.webkitRequestAnimationFrame || j.msRequestAnimationFrame || function(e) {
                 setTimeout(e, 0)
             };
         return e.each(function() {
             var a, s, e, t, l, c, u = M.isPlainObject(x) ? M.extend(!0, {}, M.fn.sidebar.settings, x) : M.extend({}, M.fn.sidebar.settings),
                 n = u.selector,
                 r = u.className,
@@ -9933,25 +9959,25 @@
                         }), e += " " + n + "ms", A && (e += " '" + A + "'"), (console.group !== N || console.table !== N) && 0 < E.length && (console.groupCollapsed(e), console.table ? console.table(E) : M.each(E, function(e, t) {
                             console.log(t.Name + ": " + t["Execution Time"] + "ms")
                         }), console.groupEnd()), E = []
                     }
                 },
                 invoke: function(i, e, t) {
                     var o, r, n, a = y;
-                    return e = e || O, t = b || t, "string" == typeof i && a !== N && (i = i.split(/[\. ]/), o = i.length - 1, M.each(i, function(e, t) {
+                    return e = e || P, t = b || t, "string" == typeof i && a !== N && (i = i.split(/[\. ]/), o = i.length - 1, M.each(i, function(e, t) {
                         var n = e != o ? t + i[e + 1].charAt(0).toUpperCase() + i[e + 1].slice(1) : i;
                         if (M.isPlainObject(a[n]) && e != o) a = a[n];
                         else {
                             if (a[n] !== N) return r = a[n], !1;
                             if (!M.isPlainObject(a[t]) || e == o) return a[t] !== N ? r = a[t] : c.error(d.method, i), !1;
                             a = a[t]
                         }
                     })), M.isFunction(r) ? n = r.apply(t, e) : r !== N && (n = r), M.isArray(C) ? C.push(n) : C !== N ? C = [C, n] : n !== N && (C = n), r
                 }
-            }, P ? (y === N && c.initialize(), c.invoke(R)) : (y !== N && c.invoke("destroy"), c.initialize())
+            }, O ? (y === N && c.initialize(), c.invoke(R)) : (y !== N && c.invoke("destroy"), c.initialize())
         }), C !== N ? C : this
     }, M.fn.sidebar.settings = {
         name: "Sidebar",
         namespace: "sidebar",
         silent: !1,
         debug: !1,
         verbose: !1,
@@ -10398,18 +10424,18 @@
             fixed: "fixed",
             supported: "native",
             top: "top",
             bottom: "bottom"
         }
     }
 }(jQuery, window, document),
-function(R, P, O, F) {
+function(R, O, P, F) {
     "use strict";
-    P = void 0 !== P && P.Math == Math ? P : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), R.fn.tab = function(a) {
-        var c, u = R.isFunction(this) ? R(P) : R(this),
+    O = void 0 !== O && O.Math == Math ? O : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), R.fn.tab = function(a) {
+        var c, u = R.isFunction(this) ? R(O) : R(this),
             d = u.selector || "",
             f = (new Date).getTime(),
             p = [],
             m = a,
             A = "string" == typeof m,
             D = [].slice.call(arguments, 1),
             E = !1;
@@ -10498,15 +10524,15 @@
                         t.hasClass(C.loading) || (b.verbose("Setting loading state for", t), t.addClass(C.loading).siblings(r).removeClass(C.active + " " + C.loading), 0 < t.length && x.onRequest.call(t[0], e))
                     },
                     state: function(e) {
                         R.address.value(e)
                     }
                 },
                 changeTab: function(d) {
-                    var f = P.history && P.history.pushState && x.ignoreFirstLoad && S,
+                    var f = O.history && O.history.pushState && x.ignoreFirstLoad && S,
                         p = x.auto || R.isPlainObject(x.apiSettings),
                         m = p && !f ? b.utilities.pathToArray(d) : b.get.defaultPathArray(d);
                     d = b.utilities.arrayToPath(m), R.each(m, function(e, t) {
                         var n, i, o, r, a = m.slice(0, e + 1),
                             s = b.utilities.arrayToPath(a),
                             l = b.is.tab(s),
                             c = e + 1 == m.length,
@@ -10520,15 +10546,15 @@
                                 b.scrollTo(n)
                             }, 0), b.activate.all(s), b.cache.read(s) || (b.cache.add(s, !0), b.debug("First time tab loaded calling tab init"), x.onFirstLoad.call(u[0], s, v, y)), x.onLoad.call(u[0], s, v, y), !1
                         }
                     })
                 },
                 scrollTo: function(e) {
                     var t = !!(e && 0 < e.length) && e.offset().top;
-                    !1 !== t && (b.debug("Forcing scroll to an in-page link in a hidden tab", t, e), R(O).scrollTop(t))
+                    !1 !== t && (b.debug("Forcing scroll to an in-page link in a hidden tab", t, e), R(P).scrollTop(t))
                 },
                 update: {
                     content: function(e, t, n) {
                         var i = b.get.tabElement(e),
                             o = i[0];
                         n = n !== F ? n : x.evaluateScripts, "string" == typeof x.cacheType && "dom" == x.cacheType.toLowerCase() && "string" != typeof t ? i.empty().append(R(t).clone(!0)) : n ? (b.debug("Updating HTML and evaluating inline scripts", e, t), i.html(t)) : (b.debug("Updating HTML", e, t), o.innerHTML = t)
                     }
@@ -10691,15 +10717,15 @@
                             a = a[t]
                         }
                     })), R.isFunction(r) ? n = r.apply(t, e) : r !== F && (n = r), R.isArray(c) ? c.push(n) : c !== F ? c = [c, n] : n !== F && (c = n), r
                 }
             }, A ? (l === F && b.initialize(), b.invoke(m)) : (l !== F && l.invoke("destroy"), b.initialize())
         }), c !== F ? c : this
     }, R.tab = function() {
-        R(P).tab.apply(this, arguments)
+        R(O).tab.apply(this, arguments)
     }, R.fn.tab.settings = {
         name: "Tab",
         namespace: "tab",
         silent: !1,
         debug: !1,
         verbose: !1,
         performance: !0,
@@ -11180,15 +11206,15 @@
             noAnimation: "Element is no longer attached to DOM. Unable to animate.  Use silent setting to surpress this warning in production.",
             repeated: "That animation is already occurring, cancelling repeated animation",
             method: "The method you called is not defined",
             support: "This browser does not support CSS animations"
         }
     }
 }(jQuery, window, document),
-function(E, R, e, P) {
+function(E, R, e, O) {
     "use strict";
     R = void 0 !== R && R.Math == Math ? R : "undefined" != typeof self && self.Math == Math ? self : Function("return this")();
     E.api = E.fn.api = function(x) {
         var C, e = E.isFunction(this) ? E(R) : E(this),
             w = e.selector || "",
             T = (new Date).getTime(),
             k = [],
@@ -11224,30 +11250,30 @@
                     events: function() {
                         var e = l.get.event();
                         e ? (l.verbose("Attaching API events to element", e), m.on(e + f, l.event.trigger)) : "now" == c.on && (l.debug("Querying API endpoint immediately"), l.query())
                     }
                 },
                 decode: {
                     json: function(e) {
-                        if (e !== P && "string" == typeof e) try {
+                        if (e !== O && "string" == typeof e) try {
                             e = JSON.parse(e)
                         } catch (e) {}
                         return e
                     }
                 },
                 read: {
                     cachedResponse: function(e) {
                         var t;
-                        if (R.Storage !== P) return t = sessionStorage.getItem(e), l.debug("Using cached response", e, t), t = l.decode.json(t);
+                        if (R.Storage !== O) return t = sessionStorage.getItem(e), l.debug("Using cached response", e, t), t = l.decode.json(t);
                         l.error(u.noStorage)
                     }
                 },
                 write: {
                     cachedResponse: function(e, t) {
-                        t && "" === t ? l.debug("Response empty, not caching", t) : R.Storage !== P ? (E.isPlainObject(t) && (t = JSON.stringify(t)), sessionStorage.setItem(e, t), l.verbose("Storing cached response for url", e, t)) : l.error(u.noStorage)
+                        t && "" === t ? l.debug("Response empty, not caching", t) : R.Storage !== O ? (E.isPlainObject(t) && (t = JSON.stringify(t)), sessionStorage.setItem(e, t), l.verbose("Storing cached response for url", e, t)) : l.error(u.noStorage)
                     }
                 },
                 query: function() {
                     if (l.is.disabled()) l.debug("Element is disabled API request aborted");
                     else {
                         if (l.is.loading()) {
                             if (!c.interruptRequests) return void l.debug("Cancelling request, previous request is still pending");
@@ -11293,15 +11319,15 @@
                     input: function() {
                         return m.is("input")
                     },
                     loading: function() {
                         return !!l.request && "pending" == l.request.state()
                     },
                     abortedRequest: function(e) {
-                        return e && e.readyState !== P && 0 === e.readyState ? (l.verbose("XHR request determined to be aborted"), !0) : (l.verbose("XHR request was not aborted"), !1)
+                        return e && e.readyState !== O && 0 === e.readyState ? (l.verbose("XHR request determined to be aborted"), !0) : (l.verbose("XHR request was not aborted"), !1)
                     },
                     validResponse: function(e) {
                         return l.is.expectingJSON() && E.isFunction(c.successTest) ? (l.debug("Checking JSON returned success", c.successTest, e), c.successTest(e) ? (l.debug("Response passed success test", e), !0) : (l.debug("Response failed success test", e), !1)) : (l.verbose("Response is not JSON, skipping validation", c.successTest, e), !0)
                     }
                 },
                 was: {
                     cancelled: function() {
@@ -11318,25 +11344,25 @@
                     }
                 },
                 add: {
                     urlData: function(o, r) {
                         var e, t;
                         return o && (e = o.match(c.regExp.required), t = o.match(c.regExp.optional), r = r || c.urlData, e && (l.debug("Looking for required URL variables", e), E.each(e, function(e, t) {
                             var n = -1 !== t.indexOf("$") ? t.substr(2, t.length - 3) : t.substr(1, t.length - 2),
-                                i = E.isPlainObject(r) && r[n] !== P ? r[n] : m.data(n) !== P ? m.data(n) : h.data(n) !== P ? h.data(n) : r[n];
-                            if (i === P) return l.error(u.requiredParameter, n, o), o = !1;
+                                i = E.isPlainObject(r) && r[n] !== O ? r[n] : m.data(n) !== O ? m.data(n) : h.data(n) !== O ? h.data(n) : r[n];
+                            if (i === O) return l.error(u.requiredParameter, n, o), o = !1;
                             l.verbose("Found required variable", n, i), i = c.encodeParameters ? l.get.urlEncodedValue(i) : i, o = o.replace(t, i)
                         })), t && (l.debug("Looking for optional URL variables", e), E.each(t, function(e, t) {
                             var n = -1 !== t.indexOf("$") ? t.substr(3, t.length - 4) : t.substr(2, t.length - 3),
-                                i = E.isPlainObject(r) && r[n] !== P ? r[n] : m.data(n) !== P ? m.data(n) : h.data(n) !== P ? h.data(n) : r[n];
-                            o = i !== P ? (l.verbose("Optional variable Found", n, i), o.replace(t, i)) : (l.verbose("Optional variable not found", n), -1 !== o.indexOf("/" + t) ? o.replace("/" + t, "") : o.replace(t, ""))
+                                i = E.isPlainObject(r) && r[n] !== O ? r[n] : m.data(n) !== O ? m.data(n) : h.data(n) !== O ? h.data(n) : r[n];
+                            o = i !== O ? (l.verbose("Optional variable Found", n, i), o.replace(t, i)) : (l.verbose("Optional variable not found", n), -1 !== o.indexOf("/" + t) ? o.replace("/" + t, "") : o.replace(t, ""))
                         }))), o
                     },
                     formData: function(e) {
-                        var t = E.fn.serializeObject !== P,
+                        var t = E.fn.serializeObject !== O,
                             n = t ? g.serializeObject() : g.serialize();
                         return e = e || c.data, e = E.isPlainObject(e) ? t ? (l.debug("Extending existing data with form data", e, n), E.extend(!0, {}, e, n)) : (l.error(u.missingSerialize), l.debug("Cant extend data. Replacing data with form data", e, n), n) : (l.debug("Adding form data", n), n)
                     }
                 },
                 send: {
                     request: function() {
                         l.set.loading(), l.request = l.create.request(), l.is.mocked() ? l.mockedXHR = l.create.mockedXHR() : l.xhr = l.create.xhr(), c.onRequest.call(b, l.request, l.xhr)
@@ -11374,15 +11400,15 @@
                             var n, i;
                             l.was.succesful() ? (i = e, n = t) : (n = e, i = l.get.responseFromXHR(n)), l.remove.loading(), c.onComplete.call(b, i, m, n)
                         },
                         fail: function(e, t, n) {
                             var i = l.get.responseFromXHR(e),
                                 o = l.get.errorFromRequest(i, t, n);
                             if ("aborted" == t) return l.debug("XHR Aborted (Most likely caused by page navigation or CORS Policy)", t, n), c.onAbort.call(b, t, m, e), !0;
-                            "invalid" == t ? l.debug("JSON did not pass success test. A server-side error has most likely occurred", i) : "error" == t && e !== P && (l.debug("XHR produced a server error", t, n), 200 != e.status && n !== P && "" !== n && l.error(u.statusMessage + n, r.url), c.onError.call(b, o, m, e)), c.errorDuration && "aborted" !== t && (l.debug("Adding error state"), l.set.error(), l.should.removeError() && setTimeout(l.remove.error, c.errorDuration)), l.debug("API Request failed", o, e), c.onFailure.call(b, i, m, e)
+                            "invalid" == t ? l.debug("JSON did not pass success test. A server-side error has most likely occurred", i) : "error" == t && e !== O && (l.debug("XHR produced a server error", t, n), 200 != e.status && n !== O && "" !== n && l.error(u.statusMessage + n, r.url), c.onError.call(b, o, m, e)), c.errorDuration && "aborted" !== t && (l.debug("Adding error state"), l.set.error(), l.should.removeError() && setTimeout(l.remove.error, c.errorDuration)), l.debug("API Request failed", o, e), c.onFailure.call(b, i, m, e)
                         }
                     }
                 },
                 create: {
                     request: function() {
                         return E.Deferred().always(l.event.request.complete).done(l.event.request.done).fail(l.event.request.fail)
                     },
@@ -11421,42 +11447,42 @@
                     }
                 },
                 get: {
                     responseFromXHR: function(e) {
                         return !!E.isPlainObject(e) && (l.is.expectingJSON() ? l.decode.json(e.responseText) : e.responseText)
                     },
                     errorFromRequest: function(e, t, n) {
-                        return E.isPlainObject(e) && e.error !== P ? e.error : c.error[t] !== P ? c.error[t] : n
+                        return E.isPlainObject(e) && e.error !== O ? e.error : c.error[t] !== O ? c.error[t] : n
                     },
                     request: function() {
                         return l.request || !1
                     },
                     xhr: function() {
                         return l.xhr || !1
                     },
                     settings: function() {
                         var e;
-                        return (e = c.beforeSend.call(b, c)) && (e.success !== P && (l.debug("Legacy success callback detected", e), l.error(u.legacyParameters, e.success), e.onSuccess = e.success), e.failure !== P && (l.debug("Legacy failure callback detected", e), l.error(u.legacyParameters, e.failure), e.onFailure = e.failure), e.complete !== P && (l.debug("Legacy complete callback detected", e), l.error(u.legacyParameters, e.complete), e.onComplete = e.complete)), e === P && l.error(u.noReturnedValue), !1 === e ? e : e !== P ? E.extend(!0, {}, e) : E.extend(!0, {}, c)
+                        return (e = c.beforeSend.call(b, c)) && (e.success !== O && (l.debug("Legacy success callback detected", e), l.error(u.legacyParameters, e.success), e.onSuccess = e.success), e.failure !== O && (l.debug("Legacy failure callback detected", e), l.error(u.legacyParameters, e.failure), e.onFailure = e.failure), e.complete !== O && (l.debug("Legacy complete callback detected", e), l.error(u.legacyParameters, e.complete), e.onComplete = e.complete)), e === O && l.error(u.noReturnedValue), !1 === e ? e : e !== O ? E.extend(!0, {}, e) : E.extend(!0, {}, c)
                     },
                     urlEncodedValue: function(e) {
                         var t = R.decodeURIComponent(e),
                             n = R.encodeURIComponent(e);
                         return t !== e ? (l.debug("URL value is already encoded, avoiding double encoding", e), e) : (l.verbose("Encoding value using encodeURIComponent", e, n), n)
                     },
                     defaultData: function() {
                         var e = {};
                         return E.isWindow(v) || (l.is.input() ? e.value = m.val() : l.is.form() || (e.text = m.text())), e
                     },
                     event: function() {
-                        return E.isWindow(v) || "now" == c.on ? (l.debug("API called without element, no events attached"), !1) : "auto" == c.on ? m.is("input") ? v.oninput !== P ? "input" : v.onpropertychange !== P ? "propertychange" : "keyup" : m.is("form") ? "submit" : "click" : c.on
+                        return E.isWindow(v) || "now" == c.on ? (l.debug("API called without element, no events attached"), !1) : "auto" == c.on ? m.is("input") ? v.oninput !== O ? "input" : v.onpropertychange !== O ? "propertychange" : "keyup" : m.is("form") ? "submit" : "click" : c.on
                     },
                     templatedURL: function(e) {
                         if (e = e || m.data(i.action) || c.action || !1, n = m.data(i.url) || c.url || !1) return l.debug("Using specified url", n), n;
                         if (e) {
-                            if (l.debug("Looking up url for action", e, c.api), c.api[e] === P && !l.is.mocked()) return void l.error(u.missingAction, c.action, c.api);
+                            if (l.debug("Looking up url for action", e, c.api), c.api[e] === O && !l.is.mocked()) return void l.error(u.missingAction, c.action, c.api);
                             n = c.api[e]
                         } else l.is.form() && (n = m.attr("action") || h.attr("action") || !1, l.debug("No url or action specified, defaulting to form action", n));
                         return n
                     }
                 },
                 abort: function() {
                     var e = l.get.xhr();
@@ -11464,22 +11490,22 @@
                 },
                 reset: function() {
                     l.remove.error(), l.remove.loading()
                 },
                 setting: function(e, t) {
                     if (l.debug("Changing setting", e, t), E.isPlainObject(e)) E.extend(!0, c, e);
                     else {
-                        if (t === P) return c[e];
+                        if (t === O) return c[e];
                         E.isPlainObject(c[e]) ? E.extend(!0, c[e], t) : c[e] = t
                     }
                 },
                 internal: function(e, t) {
                     if (E.isPlainObject(e)) E.extend(!0, l, e);
                     else {
-                        if (t === P) return l[e];
+                        if (t === O) return l[e];
                         l[e] = t
                     }
                 },
                 debug: function() {
                     !c.silent && c.debug && (c.performance ? l.performance.log(arguments) : (l.debug = Function.prototype.bind.call(console.info, console, c.name + ":"), l.debug.apply(console, arguments)))
                 },
                 verbose: function() {
@@ -11498,33 +11524,33 @@
                         })), clearTimeout(l.performance.timer), l.performance.timer = setTimeout(l.performance.display, 500)
                     },
                     display: function() {
                         var e = c.name + ":",
                             n = 0;
                         T = !1, clearTimeout(l.performance.timer), E.each(k, function(e, t) {
                             n += t["Execution Time"]
-                        }), e += " " + n + "ms", w && (e += " '" + w + "'"), (console.group !== P || console.table !== P) && 0 < k.length && (console.groupCollapsed(e), console.table ? console.table(k) : E.each(k, function(e, t) {
+                        }), e += " " + n + "ms", w && (e += " '" + w + "'"), (console.group !== O || console.table !== O) && 0 < k.length && (console.groupCollapsed(e), console.table ? console.table(k) : E.each(k, function(e, t) {
                             console.log(t.Name + ": " + t["Execution Time"] + "ms")
                         }), console.groupEnd()), k = []
                     }
                 },
                 invoke: function(i, e, t) {
                     var o, r, n, a = y;
-                    return e = e || D, t = v || t, "string" == typeof i && a !== P && (i = i.split(/[\. ]/), o = i.length - 1, E.each(i, function(e, t) {
+                    return e = e || D, t = v || t, "string" == typeof i && a !== O && (i = i.split(/[\. ]/), o = i.length - 1, E.each(i, function(e, t) {
                         var n = e != o ? t + i[e + 1].charAt(0).toUpperCase() + i[e + 1].slice(1) : i;
                         if (E.isPlainObject(a[n]) && e != o) a = a[n];
                         else {
-                            if (a[n] !== P) return r = a[n], !1;
-                            if (!E.isPlainObject(a[t]) || e == o) return a[t] !== P ? r = a[t] : l.error(u.method, i), !1;
+                            if (a[n] !== O) return r = a[n], !1;
+                            if (!E.isPlainObject(a[t]) || e == o) return a[t] !== O ? r = a[t] : l.error(u.method, i), !1;
                             a = a[t]
                         }
-                    })), E.isFunction(r) ? n = r.apply(t, e) : r !== P && (n = r), E.isArray(C) ? C.push(n) : C !== P ? C = [C, n] : n !== P && (C = n), r
+                    })), E.isFunction(r) ? n = r.apply(t, e) : r !== O && (n = r), E.isArray(C) ? C.push(n) : C !== O ? C = [C, n] : n !== O && (C = n), r
                 }
-            }, A ? (y === P && l.initialize(), l.invoke(S)) : (y !== P && y.invoke("destroy"), l.initialize())
-        }), C !== P ? C : this
+            }, A ? (y === O && l.initialize(), l.invoke(S)) : (y !== O && y.invoke("destroy"), l.initialize())
+        }), C !== O ? C : this
     }, E.api.settings = {
         name: "API",
         namespace: "api",
         debug: !1,
         verbose: !1,
         performance: !0,
         api: {},
@@ -11594,15 +11620,15 @@
         },
         metadata: {
             action: "action",
             url: "url"
         }
     }
 }(jQuery, window, document),
-function(E, R, P, O) {
+function(E, R, O, P) {
     "use strict";
     R = void 0 !== R && R.Math == Math ? R : "undefined" != typeof self && self.Math == Math ? self : Function("return this")(), E.fn.visibility = function(b) {
         var y, e = E(this),
             x = e.selector || "",
             C = (new Date).getTime(),
             w = [],
             T = b,
@@ -11634,15 +11660,15 @@
                 instantiate: function() {
                     s.debug("Storing instance", s), f.data(u, s), m = s
                 },
                 destroy: function() {
                     s.verbose("Destroying previous module"), n && n.disconnect(), t && t.disconnect(), d.off("load" + c, s.event.load).off("resize" + c, s.event.resize), p.off("scroll" + c, s.event.scroll).off("scrollchange" + c, s.event.scrollchange), "fixed" == o.type && (s.resetFixed(), s.remove.placeholder()), f.off(c).removeData(u)
                 },
                 observeChanges: function() {
-                    "MutationObserver" in R && (t = new MutationObserver(s.event.contextChanged), n = new MutationObserver(s.event.changed), t.observe(P, {
+                    "MutationObserver" in R && (t = new MutationObserver(s.event.contextChanged), n = new MutationObserver(s.event.changed), t.observe(O, {
                         childList: !0,
                         subtree: !0
                     }), n.observe(h, {
                         childList: !0,
                         subtree: !0
                     }), s.debug("Setting up mutation observer", n))
                 },
@@ -11679,17 +11705,17 @@
                     },
                     scrollchange: function(e, t) {
                         s.checkVisibility(t)
                     }
                 },
                 precache: function(e, t) {
                     e instanceof Array || (e = [e]);
-                    for (var n = e.length, i = 0, o = [], r = P.createElement("img"), a = function() {
+                    for (var n = e.length, i = 0, o = [], r = O.createElement("img"), a = function() {
                             ++i >= e.length && E.isFunction(t) && t()
-                        }; n--;)(r = P.createElement("img")).onload = a, r.onerror = a, r.src = e[n], o.push(r)
+                        }; n--;)(r = O.createElement("img")).onload = a, r.onerror = a, r.src = e[n], o.push(r)
                 },
                 enableCallbacks: function() {
                     s.debug("Allowing callbacks to occur"), v = !1
                 },
                 disableCallbacks: function() {
                     s.debug("Disabling all callbacks temporarily"), v = !0
                 },
@@ -11714,15 +11740,15 @@
                                     ++D == A && o.onAllLoaded.call(this), o.onLoad.call(this)
                                 })
                             })
                         })
                     },
                     fixed: function() {
                         s.debug("Setting up fixed"), o.once = !1, o.observeChanges = !1, o.initialCheck = !0, o.refreshOnLoad = !0, b.transition || (o.transition = !1), s.create.placeholder(), s.debug("Added placeholder", e), o.onTopPassed = function() {
-                            s.debug("Element passed, adding fixed position", f), s.show.placeholder(), s.set.fixed(), o.transition && E.fn.transition !== O && f.transition(o.transition, o.duration)
+                            s.debug("Element passed, adding fixed position", f), s.show.placeholder(), s.set.fixed(), o.transition && E.fn.transition !== P && f.transition(o.transition, o.duration)
                         }, o.onTopPassedReverse = function() {
                             s.debug("Element returned to position, removing fixed", f), s.hide.placeholder(), s.remove.fixed()
                         }
                     }
                 },
                 create: {
                     placeholder: function() {
@@ -11746,15 +11772,15 @@
                             top: o.offset + "px",
                             left: "auto",
                             zIndex: o.zIndex
                         }), o.onFixed.call(h)
                     },
                     image: function(e, t) {
                         if (f.attr("src", e), o.transition)
-                            if (E.fn.transition !== O) {
+                            if (E.fn.transition !== P) {
                                 if (f.hasClass(i.visible)) return void s.debug("Transition already occurred on this image, skipping animation");
                                 f.transition(o.transition, o.duration, t)
                             } else f.fadeIn(o.duration, t);
                         else f.show()
                     }
                 },
                 is: {
@@ -11788,87 +11814,87 @@
                 checkVisibility: function(e) {
                     s.verbose("Checking visibility of element", s.cache.element), !v && s.is.visible() && (s.save.scroll(e), s.save.calculations(), s.passed(), s.passingReverse(), s.topVisibleReverse(), s.bottomVisibleReverse(), s.topPassedReverse(), s.bottomPassedReverse(), s.onScreen(), s.offScreen(), s.passing(), s.topVisible(), s.bottomVisible(), s.topPassed(), s.bottomPassed(), o.onUpdate && o.onUpdate.call(h, s.get.elementCalculations()))
                 },
                 passed: function(e, t) {
                     var n = s.get.elementCalculations();
                     if (e && t) o.onPassed[e] = t;
                     else {
-                        if (e !== O) return s.get.pixelsPassed(e) > n.pixelsPassed;
+                        if (e !== P) return s.get.pixelsPassed(e) > n.pixelsPassed;
                         n.passing && E.each(o.onPassed, function(e, t) {
                             n.bottomVisible || n.pixelsPassed > s.get.pixelsPassed(e) ? s.execute(t, e) : o.once || s.remove.occurred(t)
                         })
                     }
                 },
                 onScreen: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onOnScreen;
-                    if (e && (s.debug("Adding callback for onScreen", e), o.onOnScreen = e), t.onScreen ? s.execute(n, "onScreen") : o.once || s.remove.occurred("onScreen"), e !== O) return t.onOnScreen
+                    if (e && (s.debug("Adding callback for onScreen", e), o.onOnScreen = e), t.onScreen ? s.execute(n, "onScreen") : o.once || s.remove.occurred("onScreen"), e !== P) return t.onOnScreen
                 },
                 offScreen: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onOffScreen;
-                    if (e && (s.debug("Adding callback for offScreen", e), o.onOffScreen = e), t.offScreen ? s.execute(n, "offScreen") : o.once || s.remove.occurred("offScreen"), e !== O) return t.onOffScreen
+                    if (e && (s.debug("Adding callback for offScreen", e), o.onOffScreen = e), t.offScreen ? s.execute(n, "offScreen") : o.once || s.remove.occurred("offScreen"), e !== P) return t.onOffScreen
                 },
                 passing: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onPassing;
-                    if (e && (s.debug("Adding callback for passing", e), o.onPassing = e), t.passing ? s.execute(n, "passing") : o.once || s.remove.occurred("passing"), e !== O) return t.passing
+                    if (e && (s.debug("Adding callback for passing", e), o.onPassing = e), t.passing ? s.execute(n, "passing") : o.once || s.remove.occurred("passing"), e !== P) return t.passing
                 },
                 topVisible: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onTopVisible,
                         i = "topVisible";
-                    if (e && (s.debug("Adding callback for top visible", e), o.onTopVisible = e), t.topVisible ? s.execute(n, i) : o.once || s.remove.occurred(i), e === O) return t.topVisible
+                    if (e && (s.debug("Adding callback for top visible", e), o.onTopVisible = e), t.topVisible ? s.execute(n, i) : o.once || s.remove.occurred(i), e === P) return t.topVisible
                 },
                 bottomVisible: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onBottomVisible,
                         i = "bottomVisible";
-                    if (e && (s.debug("Adding callback for bottom visible", e), o.onBottomVisible = e), t.bottomVisible ? s.execute(n, i) : o.once || s.remove.occurred(i), e === O) return t.bottomVisible
+                    if (e && (s.debug("Adding callback for bottom visible", e), o.onBottomVisible = e), t.bottomVisible ? s.execute(n, i) : o.once || s.remove.occurred(i), e === P) return t.bottomVisible
                 },
                 topPassed: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onTopPassed;
-                    if (e && (s.debug("Adding callback for top passed", e), o.onTopPassed = e), t.topPassed ? s.execute(n, "topPassed") : o.once || s.remove.occurred("topPassed"), e === O) return t.topPassed
+                    if (e && (s.debug("Adding callback for top passed", e), o.onTopPassed = e), t.topPassed ? s.execute(n, "topPassed") : o.once || s.remove.occurred("topPassed"), e === P) return t.topPassed
                 },
                 bottomPassed: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onBottomPassed,
                         i = "bottomPassed";
-                    if (e && (s.debug("Adding callback for bottom passed", e), o.onBottomPassed = e), t.bottomPassed ? s.execute(n, i) : o.once || s.remove.occurred(i), e === O) return t.bottomPassed
+                    if (e && (s.debug("Adding callback for bottom passed", e), o.onBottomPassed = e), t.bottomPassed ? s.execute(n, i) : o.once || s.remove.occurred(i), e === P) return t.bottomPassed
                 },
                 passingReverse: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onPassingReverse,
                         i = "passingReverse";
-                    if (e && (s.debug("Adding callback for passing reverse", e), o.onPassingReverse = e), t.passing ? o.once || s.remove.occurred(i) : s.get.occurred("passing") && s.execute(n, i), e !== O) return !t.passing
+                    if (e && (s.debug("Adding callback for passing reverse", e), o.onPassingReverse = e), t.passing ? o.once || s.remove.occurred(i) : s.get.occurred("passing") && s.execute(n, i), e !== P) return !t.passing
                 },
                 topVisibleReverse: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onTopVisibleReverse,
                         i = "topVisibleReverse";
-                    if (e && (s.debug("Adding callback for top visible reverse", e), o.onTopVisibleReverse = e), t.topVisible ? o.once || s.remove.occurred(i) : s.get.occurred("topVisible") && s.execute(n, i), e === O) return !t.topVisible
+                    if (e && (s.debug("Adding callback for top visible reverse", e), o.onTopVisibleReverse = e), t.topVisible ? o.once || s.remove.occurred(i) : s.get.occurred("topVisible") && s.execute(n, i), e === P) return !t.topVisible
                 },
                 bottomVisibleReverse: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onBottomVisibleReverse,
                         i = "bottomVisibleReverse";
-                    if (e && (s.debug("Adding callback for bottom visible reverse", e), o.onBottomVisibleReverse = e), t.bottomVisible ? o.once || s.remove.occurred(i) : s.get.occurred("bottomVisible") && s.execute(n, i), e === O) return !t.bottomVisible
+                    if (e && (s.debug("Adding callback for bottom visible reverse", e), o.onBottomVisibleReverse = e), t.bottomVisible ? o.once || s.remove.occurred(i) : s.get.occurred("bottomVisible") && s.execute(n, i), e === P) return !t.bottomVisible
                 },
                 topPassedReverse: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onTopPassedReverse,
                         i = "topPassedReverse";
-                    if (e && (s.debug("Adding callback for top passed reverse", e), o.onTopPassedReverse = e), t.topPassed ? o.once || s.remove.occurred(i) : s.get.occurred("topPassed") && s.execute(n, i), e === O) return !t.onTopPassed
+                    if (e && (s.debug("Adding callback for top passed reverse", e), o.onTopPassedReverse = e), t.topPassed ? o.once || s.remove.occurred(i) : s.get.occurred("topPassed") && s.execute(n, i), e === P) return !t.onTopPassed
                 },
                 bottomPassedReverse: function(e) {
                     var t = s.get.elementCalculations(),
                         n = e || o.onBottomPassedReverse,
                         i = "bottomPassedReverse";
-                    if (e && (s.debug("Adding callback for bottom passed reverse", e), o.onBottomPassedReverse = e), t.bottomPassed ? o.once || s.remove.occurred(i) : s.get.occurred("bottomPassed") && s.execute(n, i), e === O) return !t.bottomPassed
+                    if (e && (s.debug("Adding callback for bottom passed reverse", e), o.onBottomPassedReverse = e), t.bottomPassed ? o.once || s.remove.occurred(i) : s.get.occurred("bottomPassed") && s.execute(n, i), e === P) return !t.bottomPassed
                 },
                 execute: function(e, t) {
                     var n = s.get.elementCalculations(),
                         i = s.get.screenCalculations();
                     (e = e || !1) && (o.continuous ? (s.debug("Callback being called continuously", t, n), e.call(h, n, i)) : s.get.occurred(t) || (s.debug("Conditions met", t, n), e.call(h, n, i))), s.save.occurred(t)
                 },
                 remove: {
@@ -11882,24 +11908,24 @@
                     },
                     placeholder: function() {
                         s.debug("Removing placeholder content"), e && e.remove()
                     },
                     occurred: function(e) {
                         if (e) {
                             var t = s.cache.occurred;
-                            t[e] !== O && !0 === t[e] && (s.debug("Callback can now be called again", e), s.cache.occurred[e] = !1)
+                            t[e] !== P && !0 === t[e] && (s.debug("Callback can now be called again", e), s.cache.occurred[e] = !1)
                         } else s.cache.occurred = {}
                     }
                 },
                 save: {
                     calculations: function() {
                         s.verbose("Saving all calculations necessary to determine positioning"), s.save.direction(), s.save.screenCalculations(), s.save.elementCalculations()
                     },
                     occurred: function(e) {
-                        e && (s.cache.occurred[e] !== O && !0 === s.cache.occurred[e] || (s.verbose("Saving callback occurred", e), s.cache.occurred[e] = !0))
+                        e && (s.cache.occurred[e] !== P && !0 === s.cache.occurred[e] || (s.verbose("Saving callback occurred", e), s.cache.occurred[e] = !0))
                     },
                     scroll: function(e) {
                         e = e + o.offset || p.scrollTop() + o.offset, s.cache.scroll = e
                     },
                     direction: function() {
                         var e, t = s.get.scroll(),
                             n = s.get.lastScroll();
@@ -11930,49 +11956,49 @@
                 },
                 get: {
                     pixelsPassed: function(e) {
                         var t = s.get.elementCalculations();
                         return -1 < e.search("%") ? t.height * (parseInt(e, 10) / 100) : parseInt(e, 10)
                     },
                     occurred: function(e) {
-                        return s.cache.occurred !== O && s.cache.occurred[e] || !1
+                        return s.cache.occurred !== P && s.cache.occurred[e] || !1
                     },
                     direction: function() {
-                        return s.cache.direction === O && s.save.direction(), s.cache.direction
+                        return s.cache.direction === P && s.save.direction(), s.cache.direction
                     },
                     elementPosition: function() {
-                        return s.cache.element === O && s.save.elementPosition(), s.cache.element
+                        return s.cache.element === P && s.save.elementPosition(), s.cache.element
                     },
                     elementCalculations: function() {
-                        return s.cache.element === O && s.save.elementCalculations(), s.cache.element
+                        return s.cache.element === P && s.save.elementCalculations(), s.cache.element
                     },
                     screenCalculations: function() {
-                        return s.cache.screen === O && s.save.screenCalculations(), s.cache.screen
+                        return s.cache.screen === P && s.save.screenCalculations(), s.cache.screen
                     },
                     screenSize: function() {
-                        return s.cache.screen === O && s.save.screenSize(), s.cache.screen
+                        return s.cache.screen === P && s.save.screenSize(), s.cache.screen
                     },
                     scroll: function() {
-                        return s.cache.scroll === O && s.save.scroll(), s.cache.scroll
+                        return s.cache.scroll === P && s.save.scroll(), s.cache.scroll
                     },
                     lastScroll: function() {
-                        return s.cache.screen === O ? (s.debug("First scroll event, no last scroll could be found"), !1) : s.cache.screen.top
+                        return s.cache.screen === P ? (s.debug("First scroll event, no last scroll could be found"), !1) : s.cache.screen.top
                     }
                 },
                 setting: function(e, t) {
                     if (E.isPlainObject(e)) E.extend(!0, o, e);
                     else {
-                        if (t === O) return o[e];
+                        if (t === P) return o[e];
                         o[e] = t
                     }
                 },
                 internal: function(e, t) {
                     if (E.isPlainObject(e)) E.extend(!0, s, e);
                     else {
-                        if (t === O) return s[e];
+                        if (t === P) return s[e];
                         s[e] = t
                     }
                 },
                 debug: function() {
                     !o.silent && o.debug && (o.performance ? s.performance.log(arguments) : (s.debug = Function.prototype.bind.call(console.info, console, o.name + ":"), s.debug.apply(console, arguments)))
                 },
                 verbose: function() {
@@ -11992,33 +12018,33 @@
                         })), clearTimeout(s.performance.timer), s.performance.timer = setTimeout(s.performance.display, 500)
                     },
                     display: function() {
                         var e = o.name + ":",
                             n = 0;
                         C = !1, clearTimeout(s.performance.timer), E.each(w, function(e, t) {
                             n += t["Execution Time"]
-                        }), e += " " + n + "ms", x && (e += " '" + x + "'"), (console.group !== O || console.table !== O) && 0 < w.length && (console.groupCollapsed(e), console.table ? console.table(w) : E.each(w, function(e, t) {
+                        }), e += " " + n + "ms", x && (e += " '" + x + "'"), (console.group !== P || console.table !== P) && 0 < w.length && (console.groupCollapsed(e), console.table ? console.table(w) : E.each(w, function(e, t) {
                             console.log(t.Name + ": " + t["Execution Time"] + "ms")
                         }), console.groupEnd()), w = []
                     }
                 },
                 invoke: function(i, e, t) {
                     var o, r, n, a = m;
-                    return e = e || S, t = h || t, "string" == typeof i && a !== O && (i = i.split(/[\. ]/), o = i.length - 1, E.each(i, function(e, t) {
+                    return e = e || S, t = h || t, "string" == typeof i && a !== P && (i = i.split(/[\. ]/), o = i.length - 1, E.each(i, function(e, t) {
                         var n = e != o ? t + i[e + 1].charAt(0).toUpperCase() + i[e + 1].slice(1) : i;
                         if (E.isPlainObject(a[n]) && e != o) a = a[n];
                         else {
-                            if (a[n] !== O) return r = a[n], !1;
-                            if (!E.isPlainObject(a[t]) || e == o) return a[t] !== O ? r = a[t] : s.error(l.method, i), !1;
+                            if (a[n] !== P) return r = a[n], !1;
+                            if (!E.isPlainObject(a[t]) || e == o) return a[t] !== P ? r = a[t] : s.error(l.method, i), !1;
                             a = a[t]
                         }
-                    })), E.isFunction(r) ? n = r.apply(t, e) : r !== O && (n = r), E.isArray(y) ? y.push(n) : y !== O ? y = [y, n] : n !== O && (y = n), r
+                    })), E.isFunction(r) ? n = r.apply(t, e) : r !== P && (n = r), E.isArray(y) ? y.push(n) : y !== P ? y = [y, n] : n !== P && (y = n), r
                 }
-            }, k ? (m === O && s.initialize(), m.save.scroll(), m.save.calculations(), s.invoke(T)) : (m !== O && m.invoke("destroy"), s.initialize())
-        }), y !== O ? y : this
+            }, k ? (m === P && s.initialize(), m.save.scroll(), m.save.calculations(), s.invoke(T)) : (m !== P && m.invoke("destroy"), s.initialize())
+        }), y !== P ? y : this
     }, E.fn.visibility.settings = {
         name: "Visibility",
         namespace: "visibility",
         debug: !1,
         verbose: !1,
         performance: !0,
         observeChanges: !0,
@@ -12173,33 +12199,33 @@
                             S = m ? 7 : g ? 4 : 3,
                             A = 7 == S ? "seven" : 4 == S ? "four" : "three",
                             D = m || g ? 6 : 4,
                             E = m ? b : 1,
                             R = ce;
                         for (R.empty(), 1 < E && (a = ue("<div/>").addClass(ae.grid).appendTo(R)), i = 0; i < E; i++) {
                             if (1 < E) R = ue("<div/>").addClass(ae.column).appendTo(a);
-                            var P = T + i,
-                                O = (new Date(k, P, 1).getDay() - re.firstDayOfWeek % 7 + 7) % 7;
+                            var O = T + i,
+                                P = (new Date(k, O, 1).getDay() - re.firstDayOfWeek % 7 + 7) % 7;
                             if (!re.constantHeight && m) {
-                                var F = new Date(k, P + 1, 0).getDate() + O;
+                                var F = new Date(k, O + 1, 0).getDate() + P;
                                 D = Math.ceil(F / 7)
                             }
                             var M = f ? 10 : p ? 1 : 0,
                                 j = m ? 1 : 0,
                                 q = g || h ? 1 : 0,
                                 N = g || h ? w : 1,
-                                L = new Date(k - M, P - j, N - q, C),
-                                I = new Date(k + M, P + j, N + q, C),
-                                H = f ? new Date(10 * Math.ceil(k / 10) - 9, 0, 0) : p ? new Date(k, 0, 0) : m ? new Date(k, P, 0) : new Date(k, P, w, -1),
-                                z = f ? new Date(10 * Math.ceil(k / 10) + 1, 0, 1) : p ? new Date(k + 1, 0, 1) : m ? new Date(k, P + 1, 1) : new Date(k, P, w + 1),
+                                L = new Date(k - M, O - j, N - q, C),
+                                I = new Date(k + M, O + j, N + q, C),
+                                H = f ? new Date(10 * Math.ceil(k / 10) - 9, 0, 0) : p ? new Date(k, 0, 0) : m ? new Date(k, O, 0) : new Date(k, O, w, -1),
+                                z = f ? new Date(10 * Math.ceil(k / 10) + 1, 0, 1) : p ? new Date(k + 1, 0, 1) : m ? new Date(k, O + 1, 1) : new Date(k, O, w + 1),
                                 $ = ue("<table/>").addClass(ae.table).addClass(A + " column").addClass(s).appendTo(R);
                             if (!v) {
                                 var V = ue("<thead/>").appendTo($);
                                 o = ue("<tr/>").appendTo(V), r = ue("<th/>").attr("colspan", "" + S).appendTo(o);
-                                var U = f || p ? new Date(k, 0, 1) : m ? new Date(k, P, 1) : new Date(k, P, w, C, x),
+                                var U = f || p ? new Date(k, 0, 1) : m ? new Date(k, O, 1) : new Date(k, O, w, C, x),
                                     W = ue("<span/>").addClass(ae.link).appendTo(r);
                                 W.text(se.header(U, s, re));
                                 var _ = p ? re.disableYear ? "day" : "year" : m ? re.disableMonth ? "year" : "month" : "day";
                                 if (W.data(le.mode, _), 0 === i) {
                                     var B = ue("<span/>").addClass(ae.prev).appendTo(r);
                                     B.data(le.focusDate, L), B.toggleClass(ae.disabledCell, !oe.helper.isDateInRange(H, s)), ue("<i/>").addClass(ae.prevIcon).appendTo(B)
                                 }
@@ -12207,28 +12233,28 @@
                                     var X = ue("<span/>").addClass(ae.next).appendTo(r);
                                     X.data(le.focusDate, I), X.toggleClass(ae.disabledCell, !oe.helper.isDateInRange(z, s)), ue("<i/>").addClass(ae.nextIcon).appendTo(X)
                                 }
                                 if (m)
                                     for (o = ue("<tr/>").appendTo(V), e = 0; e < S; e++)(r = ue("<th/>").appendTo(o)).text(se.dayColumnHeader((e + re.firstDayOfWeek) % 7, re))
                             }
                             var Y = ue("<tbody/>").appendTo($);
-                            for (e = f ? 10 * Math.ceil(k / 10) - 9 : m ? 1 - O : 0, t = 0; t < D; t++)
+                            for (e = f ? 10 * Math.ceil(k / 10) - 9 : m ? 1 - P : 0, t = 0; t < D; t++)
                                 for (o = ue("<tr/>").appendTo(Y), n = 0; n < S; n++, e++) {
-                                    var Q = f ? new Date(e, P, 1, C, x) : p ? new Date(k, e, 1, C, x) : m ? new Date(k, P, e, C, x) : g ? new Date(k, P, w, e) : new Date(k, P, w, C, 5 * e),
+                                    var Q = f ? new Date(e, O, 1, C, x) : p ? new Date(k, e, 1, C, x) : m ? new Date(k, O, e, C, x) : g ? new Date(k, O, w, e) : new Date(k, O, w, C, 5 * e),
                                         J = f ? e : p ? re.text.monthsShort[e] : m ? Q.getDate() : se.time(Q, re, !0);
                                     (r = ue("<td/>").addClass(ae.cell).appendTo(o)).text(J), r.data(le.date, Q);
-                                    var K = m && Q.getMonth() !== (P + 12) % 12,
-                                        G = K || !oe.helper.isDateInRange(Q, s) || re.isDisabled(Q, s),
+                                    var G = m && Q.getMonth() !== (O + 12) % 12,
+                                        K = G || !oe.helper.isDateInRange(Q, s) || re.isDisabled(Q, s),
                                         Z = oe.helper.dateEqual(Q, c, s),
                                         ee = oe.helper.dateEqual(Q, l, s);
-                                    r.toggleClass(ae.adjacentCell, K), r.toggleClass(ae.disabledCell, G), r.toggleClass(ae.activeCell, Z && !K), g || h || r.toggleClass(ae.todayCell, !K && ee);
+                                    r.toggleClass(ae.adjacentCell, G), r.toggleClass(ae.disabledCell, K), r.toggleClass(ae.activeCell, Z && !G), g || h || r.toggleClass(ae.todayCell, !G && ee);
                                     var te = {
                                         mode: s,
-                                        adjacent: K,
-                                        disabled: G,
+                                        adjacent: G,
+                                        disabled: K,
                                         active: Z,
                                         today: ee
                                     };
                                     se.cell(r, Q, te), oe.helper.dateEqual(Q, u, s) && oe.set.focusDate(Q, !1, !1)
                                 }
                             if (re.today) {
                                 var ne = ue("<tr/>").appendTo(Y),
@@ -12871,54 +12897,30 @@
         formatter: {
             date: function(e, t) {
                 return e ? dateFormat(e, "yyyy-mm-dd") : ""
             }
         }
     })
 }), $(function() {
-    $(".ui.dropdown.maindish.selection").dropdown("setting", "onChange", function(e, t, n) {
+    enableGeneratedOrdersCancelButton(), $(".ui.dropdown.maindish.selection").dropdown("setting", "onChange", function(e, t, n) {
         $url = $(".field.dish.selection").data("url"), window.location.replace($url + e)
     }), $(".ui.dropdown.mainingredients.selection").dropdown("setting", "onChange", function(e, t, n) {
         $(".button.confirmingredients").removeClass("disabled"), $(".button.nextkitchencount").addClass("disabled"), $(".button.restorerecipe").removeClass("disabled")
     }), $(".ui.dropdown.sidesingredients.selection").dropdown("setting", "onChange", function(e, t, n) {
         $(".button.confirmingredients").removeClass("disabled"), $(".button.nextkitchencount").addClass("disabled")
     }), $(".button.orders").click(function() {
         $(".button.orders i").addClass("loading"), $.ajax({
             type: "GET",
             url: $(this).attr("data-url"),
             success: function(e, t, n) {
-                $("#generated-orders").html(e);
-                var i = $("#generated-orders tbody tr").length;
+                $("#generated-orders").html(e), enableGeneratedOrdersCancelButton();
+                var i = $("#generated-orders-table tbody tr").length;
                 $(".orders-count span").html(i), $(".orders-count").attr("data-order-count", i), $(".button.orders i").removeClass("loading")
             }
         })
-    }), $(".ui.order.cancel.button").click(function() {
-        var i = this,
-            e = $(i).attr("data-url");
-        $.get(e, {
-            status: "C"
-        }, function(e, t) {
-            $(".ui.modal.status").html(e).modal("setting", {
-                closable: !1,
-                onApprove: function(e, t) {
-                    var n = $("#change-status-form").serializeArray();
-                    return $.ajax({
-                        type: "POST",
-                        url: $(i).attr("data-url"),
-                        data: n,
-                        success: function(e, t, n) {
-                            0 < $(e).find(".errorlist").length ? $(".ui.modal.status").html(e) : ($(".ui.modal.status").modal("hide"), location.reload())
-                        }
-                    }), !1
-                },
-                onDeny: function(e) {
-                    $(".ui.modal.status").modal("hide")
-                }
-            }).modal("setting", "autofocus", !1).modal("show")
-        })
     }), $("input[name=include_a_bill]").change(function() {
         var i = this,
             e = $(i).data("url"),
             t = $(i).is(":checked");
         $.ajax({
             type: t ? "POST" : "DELETE",
             url: e,
@@ -13066,15 +13068,15 @@
                 return -1 === t.indexOf(e)
             });
         $("#id_delivery_dates").val(n.join("|")), $("#form_create_batch #id_is_submit").val("0"), $("#form_create_batch").submit()
     }), $(".order-override.override.button").click(function() {
         $("#id_override_dates").val($("#id_delivery_dates").val()), $("#form_create_batch #id_is_submit").val("1"), $("#form_create_batch").submit()
     }), $(".order-delete").click(function() {
         var e = $(this).data("orderId");
-        $(".ui.basic.modal.order-" + e).modal("show")
+        $(".ui.basic.modal.order-delete-" + e).modal("show")
     }), $(".ui.dropdown.order.status .menu > .item").click(function() {
         $(".ui.dropdown.order.status").addClass("loading");
         var e = $(this).data("value"),
             t = $(".ui.dropdown.status").attr("data-url");
         $.get(t, {
             status: e
         }, function(e, t) {
@@ -13084,15 +13086,15 @@
                     $(".ui.status_to.dropdown").dropdown(), a(), r()
                 },
                 onApprove: function(e, t) {
                     var n = $("#change-status-form").serializeArray(),
                         i = {};
                     $.each(n, function(e, t) {
                         i[t.name] = t.value
-                    }), "other" !== i.reason_select && (i.reason = i.reason_select), delete i.reason_select;
+                    }), i.reason_select && "other" !== i.reason_select && (i.reason = i.reason_select), delete i.reason_select;
                     var o = $.param(i);
                     return $.ajax({
                         type: "POST",
                         url: $(".ui.dropdown.status").attr("data-url"),
                         data: o,
                         success: function(e, t, n) {
                             0 < $(e).find(".errorlist").length ? ($(".ui.modal.status").html(e), $(".ui.status_to.dropdown").dropdown(), a(), r()) : ($(".ui.modal.status").modal("hide"), location.reload())
```

### Comparing `souschef-1.3.4/souschef/sous_chef/context_processors.py` & `souschef-1.3.5/souschef/sous_chef/context_processors.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/management/commands/makemessages.py` & `souschef-1.3.5/souschef/sous_chef/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/rules.py` & `souschef-1.3.5/souschef/sous_chef/rules.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/settings.py` & `souschef-1.3.5/souschef/sous_chef/settings.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/templates/404.html` & `souschef-1.3.5/souschef/sous_chef/templates/404.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/templates/avatar/change.html` & `souschef-1.3.5/souschef/sous_chef/templates/avatar/change.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/templates/avatar/confirm_delete.html` & `souschef-1.3.5/souschef/sous_chef/templates/avatar/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/templates/base.html` & `souschef-1.3.5/souschef/sous_chef/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                     <a class="launch icon item sidebar-toggle ui open-menu">
                         <i class="sidebar icon"></i>
                     </a>
                 </div>
             </div>
             <div class="ui main grid">
                 {% for message in messages %}
-                <div class="ui {{ message.tags }} message sixteen wide column">
+                <div class="ui large {{ message.tags }} message sixteen wide column">
                     <i class="close icon"></i>
                     <div class="center aligned header">{{ message|safe }}</div>
                 </div>
                 {% endfor %}
                 {%block message%}{%endblock%}
 
                 {%block content%}{%endblock%}
```

### Comparing `souschef-1.3.4/souschef/sous_chef/templates/dashboard/statistics.html` & `souschef-1.3.5/souschef/sous_chef/templates/dashboard/statistics.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/templates/splash.html` & `souschef-1.3.5/souschef/sous_chef/templates/splash.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/templates/system/menu.html` & `souschef-1.3.5/souschef/sous_chef/templates/system/menu.html`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/tests.py` & `souschef-1.3.5/souschef/sous_chef/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef/sous_chef/urls.py` & `souschef-1.3.5/souschef/sous_chef/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.3.4/souschef.egg-info/PKG-INFO` & `souschef-1.3.5/souschef.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souschef
-Version: 1.3.4
+Version: 1.3.5
 Summary: Webapp used to manage orders for meals-on-wheel delivery
 Home-page: https://github.com/pypa/sous-chef
 Author: Santropol Roulant and Savoir Faire Linux
 Author-email: info@santropolroulant.org
 License: AGPL-3.0
 Description: # Sous-Chef
```

### Comparing `souschef-1.3.4/souschef.egg-info/SOURCES.txt` & `souschef-1.3.5/souschef.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 souschef/delivery/templates/ingredients.html
 souschef/delivery/templates/kitchen_count.html
 souschef/delivery/templates/kitchen_count_steps.html
 souschef/delivery/templates/review_orders.html
 souschef/delivery/templates/route_sheet.html
 souschef/delivery/templates/routes.html
 souschef/delivery/templates/partials/generated_orders.html
+souschef/delivery/templates/partials/generated_orders_order_row_content.html
+souschef/delivery/templates/partials/generated_orders_table_head.html
 souschef/frontend/images/bg1.jpg
 souschef/frontend/images/jenny.jpg
 souschef/frontend/images/joe.jpg
 souschef/frontend/images/katrina.jpg
 souschef/meal/__init__.py
 souschef/meal/admin.py
 souschef/meal/apps.py
@@ -248,26 +250,28 @@
 souschef/order/migrations/0010_auto_20161012_1921.py
 souschef/order/migrations/0011_auto_20161014_1901.py
 souschef/order/migrations/0012_auto_20161122_0458.py
 souschef/order/migrations/0013_orderstatuschange.py
 souschef/order/migrations/0014_auto_20161209_2045.py
 souschef/order/migrations/0015_auto_20170410_1029.py
 souschef/order/migrations/0016_auto_20180704_1613.py
+souschef/order/migrations/0017_total_quantity_not_nullable.py
 souschef/order/migrations/__init__.py
 souschef/order/templates/_form.html
 souschef/order/templates/_order_info.html
 souschef/order/templates/base_order.html
 souschef/order/templates/create.html
 souschef/order/templates/list.html
 souschef/order/templates/order_confirm_delete.html
 souschef/order/templates/order_update_status.html
 souschef/order/templates/update.html
 souschef/order/templates/view.html
 souschef/order/templates/order/create_batch.html
 souschef/order/templates/order/partials/filters.html
+souschef/order/templates/order/partials/order_history.html
 souschef/page/__init__.py
 souschef/page/admin.py
 souschef/page/apps.py
 souschef/page/models.py
 souschef/page/tests.py
 souschef/page/urls.py
 souschef/page/views.py
```

